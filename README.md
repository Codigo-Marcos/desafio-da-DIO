//ultilezei array para armazenar os nomes dos herois com os poderes
let herois=[
    {nome:"batman",xp:8600},
    {nome:"laterna",xp:1500},
    {nome:"superman",xp:3000},
    {nome:"xavier",xp:11000},
    {nome:"tempestade",xp:5000},
]

function determinarNivel(heroi){
    let nivel;
    if(heroi.xp<1000){
        nivel="Ferro";
    }else if (heroi.xp<2000){
        nivel="Bronze";
    }else if (heroi.xp<5000){
        nivel="Prata";
    }else if (heroi.xp<7000){
        nivel="Ouro";
    }else if (heroi.xp<8000){
        nivel="platina";
    }else if (heroi.xp<9000){
        nivel="Ascendente";
    }else if (heroi.xp<10000){
        nivel="Radiante"
    }
    return nivel
}
herois.forEach(heroi=>{
    let nivel= determinarNivel(heroi);
    console.log(o heroi ${heroi.nome }esta no nivel${nivel});
})
