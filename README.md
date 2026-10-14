# Java PDF CV Generator

## Kullanılan Bileşenler ve Nesneler
- **PdfWriter:** PDF dosyasının fiziksel olarak diske yazılmasını sağlayan I/O nesnesidir.
- **PdfDocument:** PDF dosya yapısını, sayfalarını ve doküman özelliklerini yöneten çekirdek nesnedir.
- **Document:** İçeriklerin (metin, görsel) eklendiği yüksek seviyeli sayfa düzenleyicisidir.
- **Paragraph & Image:** Sayfadaki metin bloklarını ve fotoğraf verisini temsil eden görsel bileşenlerdir.
- **CvGenerator:** PDF üretim mantığını `main` metodundan izole etmek, sorumlulukların ayrılığı (SoC) prensibine uymak amacıyla özel olarak tanımlanmış nesnedir.

## Neden Kullanıldı?
- iText 7 kütüphanesi saf Java ile hızlı, arayüzsüz ve doğrudan PDF akışı üretmeyi sağladığı için tercih edilmiştir.
- `CvGenerator` sınıfı nesne yönelimli programlama standartlarına uygun şekilde veriyi ve davranışı kapsüllemektedir.
