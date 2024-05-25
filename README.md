{
    let total = v-d
    let nivel = ""
        if (total<=10){
        nivel = "Ferro"
}
            else if (total > 10 && total < 20)
{
            nivel = "Bronze"
}
                else if (total > 20 && total < 50)
{
                nivel = "Prata"
}   
                    else if (total > 50 && total < 80)
{
                    nivel = "Ouro"
}
                        else if (total > 80 && total < 90)
{
                        nivel = "Diamante"       
}
                            else if (total > 90 && total < 100)
{
                            nivel = "Lendário"
}
                                else
{
                                nivel = "Imortal"
}
return nivel 
}

let v = 0 ,d = 0


    for(let i =0;i <150;i++){
    let random = Math.floor(Math.random() * 100) + 1;
    
        if (random <= 25)
{
        d++
}           else{
            v++
}
    }
let nivel = calculadoraRankeada (v,d)

console.log (`O herói tem saldo de ${v-d}, e está no nível de ${nivel}`)
