<h1 align="center">NoteHub</h1>

<p align="center">
  Kotlin ile geliştirilmiş, sade bir Android not uygulaması.
</p>

<p align="center">
  <a href="https://osmnnuri.github.io"><b>Ekran görüntüleri için siteme göz at</b></a>
</p>

---

## Proje hakkında

NoteHub, başlık ve içerikten oluşan notlarını cihazında tutmanı sağlayan temel
bir not uygulamasıdır. Notlar en yeniden eskiye listelenir; liste veritabanı
değiştikçe kendiliğinden güncellenir.

## Özellikler

| | |
|---|---|
| **Not ekleme** | Başlık ve içerikle yeni not oluşturma |
| **Not listesi** | Notlar en yeniden eskiye, oluşturulma zamanıyla listelenir |
| **Kaydırarak silme** | Notu yana kaydırarak silme |
| **Canlı liste** | Ekleme ve silme sonrası liste anında güncellenir |
| **Yerel kayıt** | Notlar Room veritabanında yalnızca cihazda saklanır |

## Nasıl çalışıyor?

```
NotesFragment / AddFragment  ◄──  NoteViewModel (LiveData)
                                        │
                                  NoteRepository
                                        │
                                Room (NoteDao, Flow)
```

## Kullanılan teknolojiler

| Katman | Teknoloji |
|---|---|
| Dil | Kotlin |
| Arayüz | Fragment, RecyclerView, ViewBinding |
| Mimari | MVVM, Repository, Coroutines |
| Gezinme | Navigation |
| Yerel veri | Room (Flow → LiveData) |
| Geliştirme ortamı | Android Studio |

Uygulamadaki görseller yapay zekâ ile üretildi.

## Neden yaptım?

Android ve Kotlin becerilerimi geliştirmek, MVVM ve Room ile katmanlı bir yapı
kurmayı pratik etmek için.

## Kaynak kod

Kaynak kod özel bir depoda tutuluyor; inceleme için talep üzerine paylaşılabilir.

## İletişim

**osmnnuri** · [Web sitesi](https://osmnnuri.github.io) · [GitHub](https://github.com/osmnnuri) · osmannuriyasar57@gmail.com
