# Currency-ID

Merubah format double ke Format Currency ID yaitu format mata Uang Rupiah, seperti : 10000 -> Rp10,000

Import Lib :
```swift
import java.util.Locale;
import java.text.NumberFormat;
```
Fungsi CurrencyID :
```swift
public static String currencyID(double nominal){
    Locale localeID = new Locale("in", "ID");
    NumberFormat formatRupiah = NumberFormat.getCurrencyInstance(localeID);
    return formatRupiah.format((double)nominal);
}
```
Contoh penggunaan :
```swift
double nominal = 10000;
String output = currencyID(nominal);
Log.i("outputCurrency",output);
```

untuk melihat tutorial lainnya bisa kunjungi blog saya https://blog.kamil.co.id
