# Coffee-Quality-Data---2023-
# Linear Regression Analysis#
İşlemlerin adımları şu şekildedir:

İlk olarak, Aftertaste özelliği bağımsız değişken olarak X'e, Flavor özelliği bağımlı değişken olarak y'ye atanır.

Ardından, veri seti train_test_split fonksiyonu kullanılarak rastgele bir şekilde eğitim ve test kümelerine bölünür. Bu sayede veri seti, modelin eğitiminde kullanılmak üzere bir eğitim kümesine ve modelin performansını değerlendirmek için kullanılmak üzere bir test kümesine ayrılmış olur. test_size parametresi, test kümesinin boyutunu belirlerken, random_state parametresi ise bölme işleminin tekrarlanabilirliğini sağlar.

Daha sonra, LinearRegression sınıfından bir model oluşturulur ve eğitim kümesine fit yöntemi kullanılarak uyarlanır. Bu adımda, model, eğitim kümesindeki X_train ve y_train verilerini kullanarak doğrusal regresyonu öğrenir.

Modelin eğitim sonucunda elde ettiği doğrusal regresyonu kullanarak, test kümesindeki X_test verilerine dayalı olarak y_pred tahmin değerlerini hesaplar.

r2_score fonksiyonu kullanılarak, gerçek y_test değerleriyle tahmin edilen y_pred değerleri arasındaki R2 skoru hesaplanır. R2 skoru, modelin ne kadar iyi bir şekilde gözlem verilerini açıkladığını gösteren bir ölçüdür. Değer 1'e ne kadar yakınsa, modelin daha iyi performans gösterdiği anlamına gelir.

Son olarak, scatter plot (dağılım grafiği) kullanılarak, gerçek ve tahmin edilen değerlerin görselleştirilmesi yapılır. Mavi renkteki noktalar gerçek değerleri temsil ederken, kırmızı renkteki noktalar tahmin edilen değerleri temsil eder. Grafiğin ekseni Aftertaste ve Flavor özelliklerini gösterir. Başlık ve etiketlerle grafiğin anlaşılırlığı artırılır.

Bu kod bloğu, Aftertaste özelliğinin Flavor değerlerini tahmin etmek için kullanıldığı bir doğrusal regresyon modelinin oluşturulması ve performansının değerlendirilmesi işlemlerini gerçekleştirir.
