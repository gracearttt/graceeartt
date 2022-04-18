- 👋 Hi, I’m @graceeartt
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
graceeartt/graceeartt is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
import React, { useState } from 'react';
import logo from './logo.svg';
import './App.css';


  // fonksiyon tanımlıyoruz
  const App = () => {
    const [write, setWrite] = useState("");
   
  
   const [count, setCount] = useState(14);
  
   return (

      <div className='container'>
      
      <p><h2>React JS İle Fonksiyon Kullanımı Örnek Uygulaması</h2></p>

       <h4>   {count} kere  tıkladın</h4>
       <button onClick={() => setCount(count + 1)}>
         artır
       </button>
       <button onClick={() => setCount(count -1)}>
         azalt
       </button>
       <p>inputta Yazılan yazi :{write}</p>
       <input onChange={(e)=>setWrite(e.target.value)}></input>
      
      <p><h2>Ödevimi Nasıl Yaptım? Yazdığım Kodlar Ne İşe Yarıyor?</h2></p>
       <p> <b>React JS Nedir? : </b>React bir JavaScript kütüphanesi olup web uygulamaları için hızlı ve interaktif kullanıcı arayüzleri oluşturmada kullanılır.  </p>
       <p> <b>Fonksiyon Nedir? :</b>  fonksiyon bir veya daha fazla işlem satırından oluşan kodların bir kod bloğu şeklinde yapılandırılması ile oluşturulur.
        Fonksiyonlar oluşturulduktan sonra programın herhangi bir yerinden sadece fonksiyon adı kullanılarak çağrılabilir.</p>
       <p>Yaptığım uygulamada anlatmak istediğim şey arttır butonuna tıklandığında sayacımızı birer birer artırması ve azalt butonuna tıklandığında sayacımızı birer birer azaltması. Ve inputa yazdığımız yazının üst tarafta da yazılması. Bunları React JS ile fonksiyon kullanarak yaptım. Kullanımına örnek vermek amacıyla da sayfa başındaki uygulamayı yaptım</p>
       <p>Fonksiyon kullanımını bu kodlar ile gerçekleştirdim. </p>
       <p><b>const App Nedir? </b>Fonksiyonumuzu burada oluştuyoruz.</p>
       <p><b>onClick Ne İşe Yarar:</b>Butona tıkladığımızı işaret eder.</p>
       <p><b>setCount Ne işe Yarar:</b>setCount butona her tıkladığımızda üstteki sayacımızın güncellenmesini sağlar.</p>
       <p><b>onChange Ne İşe Yarar:</b>Bir metin kutusu, metin alanı ya da seçim listesindeki bir metin değiştiği zaman ya da kontrol nesnesi odaktan çıkınca bir eylem grubunu harekete geçirir.</p>
       <p><b>setWrite Ne İşe Yarar:</b>İnputa yazdığımız yazıyı bize yazdırır.</p>




     </div>
   )
  }
export default App;
