# class
class marks{
    constructor(typeName){
        this.studentName=typeName;
        this.Mark=[];
        this.Total=""
    }    
    
    setMarks(entermarks){
        this.Mark.push(entermarks)
        return this.Mark
    }
    total(total0,total1,total3,total2,total4){
        
        this.Total=(total0+total1+total2+total3+total4);
        return this.Total
    }
    result(){
        return console.log(`${this.studentName} mark is ${this.Mark} and total is ${this.Total}`)
    }
}

const Ranks= new marks("ganesan");

Ranks.setMarks(98);
Ranks.setMarks(97);
Ranks.setMarks(95);
Ranks.setMarks(99);
Ranks.setMarks(100);
 

total0=Ranks.Mark[0]
total1=Ranks.Mark[1]
total2=Ranks.Mark[2]
total3=Ranks.Mark[3]
total4=Ranks.Mark[4]

Ranks.total(total0,total1,total2,total3,total4)
Ranks.result()
