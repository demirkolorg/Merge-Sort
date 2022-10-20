# MERGE SORT

Abdullah Demirkol'a patika.dev sitesinde [ademirkol](https://app.patika.dev/ademirkol) kullanıcı adı ile ulaşabilirsiniz.

## Patika.dev'de veri yapıları kursu için yapılan proje


## **SORU 1 -** [16,21,11,8,12,22] -> Merge Sort

> **Merge Sort Hatırlatma** 
> >Bir listeyi her adımda parçaya ayırıp tek eleman kalıncaya kadar bölüyor. Böldükten sonra sıralı bir şekilde bize sunuyor.

### A - Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.

```mermaid
  graph TD;
      16,21,11,8,12,22-->8,12,22;
      16,21,11,8,12,22-->16,21,11;


      8,12,22-->8;
      8,12,22-->12,22;

      16,21,11-->16;
      16,21,11-->21,11;
      
      21,11-->11,21;
      16-->.16;
      8-->.8;
      12,22-->.12,22;
      .8-->.8,12,22;
      .12,22-->.8,12,22;
      .16-->.11,16,21;
       11,21-->.11,16,21;
      .11,16,21-->8,11,12,16,21,22;
      .8,12,22-->8,11,12,16,21,22;
      


    
```

**Toplam islem sayısı 6**

### B - Big-O gösterimini yazınız.

 O(nlogn) -> O(6log6)