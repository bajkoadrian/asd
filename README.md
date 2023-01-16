
kiralyok = []
kiralyok.push(new kiraly('I. (Szent) István',1000,1038,'Árpád-ház'));
kiralyok.push(new kiraly('Péter',1038,1041,'Árpád-ház'));
kiralyok.push(new kiraly('Aba Sámuel',1041,1044,'Árpád-ház'));
kiralyok.push(new kiraly('Péter (másodszor)',1044,1046,'Árpád-ház'));
kiralyok.push(new kiraly('I. András',1046,1060,'Árpád-ház'));
kiralyok.push(new kiraly('I. Béla',1060,1063,'Árpád-ház'));
kiralyok.push(new kiraly('Salamon',1063,1074,'Árpád-ház'));
kiralyok.push(new kiraly('I. Géza',1074,1077,'Árpád-ház'));
kiralyok.push(new kiraly('I. (Szent) László',1077,1095,'Árpád-ház'));
kiralyok.push(new kiraly('(Könyves) Kálmán',1095,1116,'Árpád-ház'));
kiralyok.push(new kiraly('II. István',1116,1131,'Árpád-ház'));
kiralyok.push(new kiraly('II. (Vak) Béla',1131,1141,'Árpád-ház'));
kiralyok.push(new kiraly('II. Géza',1141,1162,'Árpád-ház'));
kiralyok.push(new kiraly('III. István',1162,1172,'Árpád-ház'));
kiralyok.push(new kiraly('II. László ellenkirály',1162,1163,'Árpád-ház'));
kiralyok.push(new kiraly('IV. István ellenkirály',1163,1165,'Árpád-ház'));
kiralyok.push(new kiraly('III. Béla',1172,1196,'Árpád-ház'));
kiralyok.push(new kiraly('Imre',1196,1204,'Árpád-ház'));
kiralyok.push(new kiraly('III. László (kiskorú)',1204,1205,'Árpád-ház'));
kiralyok.push(new kiraly('II. András',1205,1235,'Árpád-ház'));
kiralyok.push(new kiraly('IV. Béla',1235,1270,'Árpád-ház'));
kiralyok.push(new kiraly('V. István',1270,1272,'Árpád-ház'));
kiralyok.push(new kiraly('IV. (Kun) László',1272,1290,'Árpád-ház'));
kiralyok.push(new kiraly('III. András',1290,1301,'Árpád-ház'));
kiralyok.push(new kiraly('(Cseh) Vencel',1301,1305,'Premysl-ház'));
kiralyok.push(new kiraly('(Bajor) Ottó',1305,1307,'Wittelsbach-ház'));
kiralyok.push(new kiraly('I. Károly Róbert',1308,1342,'Anjou-ház'));
kiralyok.push(new kiraly('I. (Nagy) Lajos',1342,1382,'Anjou-ház'));
kiralyok.push(new kiraly('Mária',1382,1385,'Anjou-ház'));
kiralyok.push(new kiraly('II. (Kis) Károly',1385,1386,'Anjou-ház'));
kiralyok.push(new kiraly('Mária (másodszor)',1386,1395,'Anjou-ház'));
kiralyok.push(new kiraly('Zsigmond',1387,1437,'Luxemburgi-ház'));
kiralyok.push(new kiraly('(Habsburg) Albert',1438,1439,'Habsburg-ház'));
kiralyok.push(new kiraly('I. Ulászló',1440,1444,'Jagelló-ház'));
kiralyok.push(new kiraly('V. László',1444,1457,'Habsburg-ház'));
kiralyok.push(new kiraly('I. Mátyás',1458,1490,'Hunyadi-ház'));
kiralyok.push(new kiraly('II. Ulászló',1490,1516,'Jagelló-ház'));
kiralyok.push(new kiraly('II. Lajos',1516,1526,'Jagelló-ház'));
kiralyok.push(new kiraly('I. János',1526,1540,'Szapolyai-ház'));
kiralyok.push(new kiraly('II. János',1540,1571,'Szapolyai-ház'));
kiralyok.push(new kiraly('I. Ferdinánd',1526,1564,'Habsburg-ház'));
kiralyok.push(new kiraly('I. Miksa',1564,1576,'Habsburg-ház'));
kiralyok.push(new kiraly('II. Rudolf',1576,1608,'Habsburg-ház'));
kiralyok.push(new kiraly('II. Mátyás',1608,1619,'Habsburg-ház'));
kiralyok.push(new kiraly('II. Ferdinánd',1619,1637,'Habsburg-ház'));
kiralyok.push(new kiraly('III. Ferdinánd',1637,1657,'Habsburg-ház'));
kiralyok.push(new kiraly('IV. Ferdinánd',1647,1654,'Habsburg-ház'));
kiralyok.push(new kiraly('I. Lipót',1657,1705,'Habsburg-ház'));
kiralyok.push(new kiraly('I. József',1705,1711,'Habsburg-ház'));
kiralyok.push(new kiraly('III. Károly',1711,1740,'Habsburg-ház'));
kiralyok.push(new kiraly('Mária Terézia',1740,1780,'Habsburg-ház'));
kiralyok.push(new kiraly('II. József',1780,1790,'Habsburg-Lotaringiai-ház'));
kiralyok.push(new kiraly('II. Lipót',1790,1792,'Habsburg-Lotaringiai-ház'));
kiralyok.push(new kiraly('I. Ferenc',1792,1835,'Habsburg-Lotaringiai-ház'));
kiralyok.push(new kiraly('V. Ferdinánd',1835,1848,'Habsburg-Lotaringiai-ház'));
kiralyok.push(new kiraly('I. Ferenc József',1848,1916,'Habsburg-Lotaringiai-ház'));
kiralyok.push(new kiraly('IV. Károly',1916,1918,'Habsburg-Lotaringiai-ház'));

function kiraly(nev,kezdet,vege,hely)
{
    this.nev = nev;
    this.kezdet = kezdet;
    this.vege = vege;
    this.hely = hely;
}
lista1=[]


function kiir()
{
    lista1 = []
   a = ""
     
    for (let i = 0; i < kiralyok.length; i++) 
    {
       if(kiralyok[i].hely.includes(document.getElementById("bevitel").value))
       {
            lista1.push(kiralyok[i])
       }

       
    }
    console.log(lista1)
    a += "<table>"
    for (let i = 0; i < lista1.length; i++) 
    {
        a += ` 
            <tr>
                <td>Neve:${lista1[i].nev}</td>
                <td>Kezdet:${lista1[i].kezdet}</td>
                <td>Vege:${lista1[i].vege}</td>
                <td>hely:${lista1[i].hely}</td>
            </tr>
        `
    }
    a += "</table>"


    document.getElementById("div1").innerHTML = a
}

function veletlen()
{
    if(lista1.length != 0)
    {
        rand = Math.floor(Math.random()*lista1.length)
        console.log(rand)
        console.log(lista1[rand])
        b = ""
        b += `${lista1[rand].nev}
            <br>
            <input type="text" id="tipp1">
            <input type="button" value="tipp" onclick="ellenor()">
            <input type="checkbox" id="check">
        `
        document.getElementById("eredmeny").innerHTML = b   
    }
    else
    {
        b = ""
        document.getElementById("eredmeny").innerHTML = b
    }
}

function ellenor() 
{
    if(document.getElementById("check").checked)
    {
        if(lista1[rand].kezdet-10<=document.getElementById("tipp1").value && lista1[rand].vege+10>= document.getElementById("tipp1").value)    
        {
            document.getElementById("score").innerHTML = "Nyertél"
        }
        else
        {
            document.getElementById("score").innerHTML = "vesztettél"
        }
        console.log(c)
    }
    else

        if(lista1[rand].kezdet<=document.getElementById("tipp1").value && lista1[rand].vege>= document.getElementById("tipp1").value)    
            {
                document.getElementById("score").innerHTML = "Nyertél"
            }
            else
            {
                document.getElementById("score").innerHTML = "vesztettél"
            }
}

