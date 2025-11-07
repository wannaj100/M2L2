import discord
from discord.ext import commands
import random

intents = discord.Intents.default()
intents.message_content = True

bot = commands.Bot(command_prefix='$', intents=intents)

@bot.event
async def on_ready():
    print(f'Zalogowaliśmy się jako {bot.user}')
    

@bot.command()
async def seg(ctx, nazwa_odpadu = ""):
    zolty = [
    "puszka", "konserwa", "aluminium", "butelka_plastikowa", "karton_po_soku",
    "nakrętka", "folia_aluminiowa", "opakowanie_po_chipsach", "butelka_PET",
    "pojemnik_po_jogurcie", "reklamówka", "folia_spożywcza", "torebka_foliowa",
    "opakowanie_po_kosmetykach", "butelka_po_płynie_do_naczyń", "opakowanie_po_proszku"
    ]

    niebieski = [
    "gazeta", "karton", "tektura", "ulotka", "zeszyt", "papier_biurowy",
    "książka", "papier_pakowy", "pudełko_po_butach", "papier_do_drukarki",
    "ręcznik_papierowy_czysty", "torba papierowa", "koperta_bez_folii","papier"
    ]

    zielony = [
    "butelka_szklana", "słoik", "szkło_kolorowe", "szkło_bezbarwne",
    "butelka_po_winie", "butelka _po_piwie", "butelka_po_soku_szklana",
    "słoik_po_dżemie", "słoik _po_ogórkach", "butelka_po_oliwie"
    ]
    brazowy = [
    "resztki_jedzenia", "skórka_od_banana", "fus_z_kawy", "liście", "obierki_warzyw",
    "resztki_owoców", "skorupka_od_jajka", "papierowy_ręcznik_brudny",
    "chleb", "zwiędłe_kwiaty", "fusy_po_herbacie", "łupina_orzecha", "gałązka"
    ]

    czarny = [
    "pielucha", "ceramika", "żarówka", "popiół", "tekstylia", "but", "lustro",
    "porcelana", "odkurzaczowy_kurz", "papier_tłusty", "worek_po_cemencie",
    "kubek_jednorazowy_powlekany", "plastikowy_talerz", "mięso", "kości"
    ]
    if nazwa_odpadu in zolty :
        await ctx.send("wrzuć do żółtego pokemnika")
    elif nazwa_odpadu in niebieski :
        await ctx.send("wrzuć do niebieskiego pokemnika")
    elif nazwa_odpadu in zielony :
        await ctx.send("wrzuć do zielonego pokemnika")
    elif nazwa_odpadu in brazowy :
        await ctx.send("wrzuć do brązowego pokemnika")
    elif nazwa_odpadu in czarny :
        await ctx.send("wrzuć do czarnego pokemnika")
    else:
        await ctx.send("nie mam takiego odpadu w naszej bibliotece")
        
@bot.command()
async def recykling(ctx):
    await ctx.send("Recykling to proces ponownego przetwarzania odpadów w surowce, z których można wytwarzać nowe produkty. Jego głównym celem jest ochrona środowiska poprzez ograniczenie ilości śmieci trafiających na wysypiska oraz zmniejszenie zużycia surowców naturalnych. W Polsce obowiązuje system segregacji odpadów, który obejmuje pięć podstawowych frakcji. Do niebieskiego pojemnika trafia papier, taki jak gazety, zeszyty, kartony czy pudełka, jednak nie należy wrzucać tam zabrudzonego papieru, ręczników papierowych ani tapet. Zielony pojemnik przeznaczony jest na szkło, np. butelki i słoiki, ale nie wolno wrzucać do niego szkła okiennego, ceramiki czy żarówek. W żółtym pojemniku zbiera się metale i tworzywa sztuczne, takie jak plastikowe butelki, puszki czy zakrętki, natomiast należy unikać wyrzucania opakowań po oleju i lekach. Brązowy pojemnik służy do bioodpadów, czyli resztek jedzenia, obierek, fusów z kawy czy liści, jednak nie powinno się tam wrzucać mięsa, kości ani odchodów zwierząt. Do czarnego pojemnika trafiają odpady zmieszane, czyli te, których nie da się odzyskać w inny sposób. Recykling przynosi wiele korzyści – pozwala oszczędzać energię, ogranicza zanieczyszczenia, chroni lasy oraz surowce naturalne, a także zmniejsza ilość odpadów na wysypiskach. Przykładowo, recykling aluminium pozwala zaoszczędzić aż 95% energii w porównaniu z produkcją z rudy. Co ciekawe, szkło można przetwarzać nieskończenie wiele razy bez utraty jakości, z 35 plastikowych butelek PET można zrobić polarową bluzę, a papier można odzyskać od czterech do sześciu razy, zanim włókna celulozy staną się zbyt krótkie. Recykling to prosty, ale niezwykle ważny sposób na dbanie o środowisko i przyszłość naszej planety.")

@bot.command()
async def ciekawostka(ctx):
    ciekawostki = [
    "♻️ Szklane butelki 🪟 można przetwarzać nieskończenie wiele razy bez utraty jakości.",
    "🥤 Z 35 plastikowych butelek PET można zrobić polarową bluzę 🧥.",
    "📄 Papier można odzyskać 4–6 razy, zanim włókna celulozy staną się zbyt krótkie.",
    "⚡ Recykling aluminium pozwala zaoszczędzić aż 95% energii w porównaniu z produkcją z rudy.",
    "🗑️ Segregacja odpadów w pięć podstawowych frakcji ułatwia recykling: papier, szkło, metale i plastik, bioodpady, odpady zmieszane.",
    "🌳 Recykling pomaga chronić lasy, zmniejsza zanieczyszczenia i ogranicza ilość odpadów na wysypiskach.",
    "🥤 Wyrzucenie jednej butelki PET do recyklingu zamiast do śmieci oszczędza energię potrzebną do produkcji nowej butelki ⚡.",
    "🌍 Recykling plastiku zmniejsza emisję CO2 i pomaga walczyć ze zmianami klimatu.",
    "🥫 Opakowania metalowe, takie jak puszki po napojach, można przetwarzać w nieskończoność.",
    "🌳 Dzięki recyklingowi papieru ratujemy około 17 drzew na każdą tonę odzyskanego papieru.",
    "💧 Recykling szkła i metalu wymaga znacznie mniej wody niż produkcja od podstaw.",
    "💰 Niektóre kraje mają system depozytowy, dzięki któremu oddanie butelki do recyklingu daje zwrot pieniędzy.",
    "🍂 Segregacja bioodpadów pozwala na produkcję kompostu, który może zasilać rośliny w ogrodach i uprawach.",
    "📱 Elektroniczne odpady (telefony, baterie) zawierają cenne metale, które można odzyskać dzięki recyklingowi.",
    "🚮 Recykling zmniejsza ilość odpadów trafiających do spalarni i wysypisk, co chroni środowisko i zdrowie ludzi."
]
    """Losuje ciekawostkę o recyklingu i wysyła ją na kanał."""
    wiadomosc = random.choice(ciekawostki)
    await ctx.send(wiadomosc)

@bot.command()
async def quiz(ctx):
    await ctx.send("1. co to jest recykling?"+"\n"+
    "a) Proces spalania śmieci dla energii"+"\n"+
    "b) Proces przetwarzania odpadów w surowce do ponownego wykorzystania"+"\n"+
    "c) Składowanie śmieci w specjalnych pojemnikach")

    await ctx.send("2. Ile frakcji odpadów obowiązuje w Polsce?"+"\n"+
    "a) Trzy"+"\n"+
    "b) Pięć"+"\n"+
    "c) Sześć")

    await ctx.send("3. Jaki kolor pojemnika przeznaczony jest na papier?"+"\n"+
    "a) Zielony"+"\n"+
    "b) Niebieski"+"\n"+
    "c) Żółty")

    await ctx.send("4. co należy wrzucać do pojemnika na szkło?"+"\n"+
    "a) Słoiki i butelki"+"\n"+
    "b) ceramikę i lustra"+"\n"+
    "c) Żarówki i szyby")

    await ctx.send("5. co wrzucamy do żółtego pojemnika?"+"\n"+
    "a) Plastikowe butelki, puszki, metalowe zakrętki"+"\n"+
    "b) Papier, kartony i tekturę"+"\n"+
    "c) Resztki jedzenia")

    await ctx.send("6. czego nie należy wrzucać do pojemnika na papier?"+"\n"+
    "a) Kartonów po mleku"+"\n"+
    "b) Zeszytów i gazet"+"\n"+
    "c) Pudełek po butach")

    await ctx.send("7. Jaki kolor ma pojemnik na bioodpady?"+"\n"+
    "a) brązowy"+"\n"+
    "b) czarny"+"\n"+
    "c) Niebieski")

    await ctx.send("8. co trafia do pojemnika czarnego (zmieszane)?"+"\n"+
    "a) Szkło i plastik"+"\n"+
    "b) Tylko odpady nieprzetwarzalne"+"\n"+
    "c) Wszystkie odpady bez wyjątku")

    await ctx.send("9. Które z poniższych to bioodpady?"+"\n"+
    "a) Fusy z kawy, obierki, liście"+"\n"+
    "b) Puszki po napojach"+"\n"+
    "c) Plastikowe opakowania")

    await ctx.send("10. czego nie wolno wrzucać do bioodpadów?"+"\n"+
    "a) Skorupek jajek"+"\n"+
    "b) Mięsa i kości"+"\n"+
    "c) Obierek z warzyw")

    await ctx.send("11. Jakie korzyści daje recykling?"+"\n"+
    "a) Zwiększa ilość odpadów"+"\n"+
    "b) Oszczędza energię i chroni środowisko"+"\n"+
    "c) Powoduje więcej zanieczyszczeń")

    await ctx.send("12. Ile energii można zaoszczędzić dzięki recyklingowi aluminium?"+"\n"+
    "a) 25%"+"\n"+
    "b) 50%"+"\n"+
    "c) 95%")

    await ctx.send("13. Ile razy można przetworzyć papier zanim straci swoje właściwości?"+"\n"+
    "a) 2–3 razy"+"\n"+
    "b) 4–6 razy"+"\n"+
    "c) Nieskończenie wiele razy")

    await ctx.send("14. co można zrobić z 35 plastikowych butelek PET?"+"\n"+
    "a) Kurtkę polarową"+"\n"+
    "b) buty sportowe"+"\n"+
    "c) Plecak szkolny")

    await ctx.send("15. Który materiał można przetwarzać nieskończenie wiele razy?"+"\n"+
    "a) Papier"+"\n"+
    "b) Szkło"+"\n"+
    "c) Plastik")

    await ctx.send("16. Jakie surowce naturalne pomaga chronić recykling papieru?"+"\n"+
    "a) Wodę i powietrze"+"\n"+
    "b) Drewno i lasy"+"\n"+
    "c) Piasek i żwir")

    await ctx.send("17. co oznacza symbol trzech strzałek ułożonych w trójkąt ♻️?"+"\n"+
    "a) Odpady niebezpieczne"+"\n"+
    "b) Segregacja odpadów"+"\n"+
    "c) Recykling")

    await ctx.send("18. Jak należy przygotować butelki PET do recyklingu?"+"\n"+
    "a) Zgnieść i zdjąć zakrętkę"+"\n"+
    "b) Zostawić pełną"+"\n"+
    "c) Wrzucić bez opróżniania")

    await ctx.send("19. Jakie odpady powinny trafić do punktu selektywnej zbiórki (PSZOK)?"+"\n"+
    "a) Lekarstwa, baterie, elektrośmieci"+"\n"+
    "b) Zwykły papier"+"\n"+
    "c) Resztki jedzenia")

    await ctx.send("20. Dlaczego warto segregować odpady już w domu?"+"\n"+
    "a) bo to obowiązek i ułatwia recykling"+"\n"+
    "b) bo dzięki temu śmieci ładnie wyglądają"+"\n"+
    "c) bo to wymysł firm recyklingowych")
@bot.command()
async def odp( ctx, I = "", II = "", III ="", IV = "", V = "", VI = "", VII = "", VIII="", IX = "", X = "" ,XI = "", XII = "", XIII ="", XIV = "", XV = "", XVI = "", XVII = "", XVIII="", XIX = "",XX = "" ):
    # I
    if I == "b":
        await ctx.send("Odpowiedź jest poprawna ✅")
    elif I == "a" or I == "c":
        await ctx.send("Odpowiedź jest błędna ❌")
    else:
        await ctx.send("Nie ma takiej odpowiedzi")

    # II
    if II == "b":
        await ctx.send("Odpowiedź jest poprawna ✅")
    elif II == "a" or II == "c":
        await ctx.send("Odpowiedź jest błędna ❌")
    else:
        await ctx.send("Nie ma takiej odpowiedzi")

    # III
    if III == "b":
        await ctx.send("Odpowiedź jest poprawna ✅")
    elif III == "a" or III == "c":
        await ctx.send("Odpowiedź jest błędna ❌")
    else:
        await ctx.send("Nie ma takiej odpowiedzi")

    # IV
    if IV == "a":
        await ctx.send("Odpowiedź jest poprawna ✅")
    elif IV == "b" or IV == "c":
        await ctx.send("Odpowiedź jest błędna ❌")
    else:
        await ctx.send("Nie ma takiej odpowiedzi")

    # V
    if V == "a":
        await ctx.send("Odpowiedź jest poprawna ✅")
    elif V == "b" or V == "c":
        await ctx.send("Odpowiedź jest błędna ❌")
    else:
        await ctx.send("Nie ma takiej odpowiedzi")

    # VI
    if VI == "a":
        await ctx.send("Odpowiedź jest poprawna ✅")
    elif VI == "b" or VI == "c":
        await ctx.send("Odpowiedź jest błędna ❌")
    else:
        await ctx.send("Nie ma takiej odpowiedzi")

    # VII
    if VII == "a":
        await ctx.send("Odpowiedź jest poprawna ✅")
    elif VII == "b" or VII == "c":
        await ctx.send("Odpowiedź jest błędna ❌")
    else:
        await ctx.send("Nie ma takiej odpowiedzi")

    # VIII
    if VIII == "b":
        await ctx.send("Odpowiedź jest poprawna ✅")
    elif VIII == "a" or VIII == "c":
        await ctx.send("Odpowiedź jest błędna ❌")
    else:
        await ctx.send("Nie ma takiej odpowiedzi")

    # IX
    if IX == "a":
        await ctx.send("Odpowiedź jest poprawna ✅")
    elif IX == "b" or IX == "c":
        await ctx.send("Odpowiedź jest błędna ❌")
    else:
        await ctx.send("Nie ma takiej odpowiedzi")

    # X
    if X == "b":
        await ctx.send("Odpowiedź jest poprawna ✅")
    elif X == "a" or X == "c":
        await ctx.send("Odpowiedź jest błędna ❌")
    else:
        await ctx.send("Nie ma takiej odpowiedzi")

    # XI
    if XI == "b":
        await ctx.send("Odpowiedź jest poprawna ✅")
    elif XI == "a" or XI == "c":
        await ctx.send("Odpowiedź jest błędna ❌")
    else:
        await ctx.send("Nie ma takiej odpowiedzi")

    # XII
    if XII == "c":
        await ctx.send("Odpowiedź jest poprawna ✅")
    elif XII == "a" or XII == "b":
        await ctx.send("Odpowiedź jest błędna ❌")
    else:
        await ctx.send("Nie ma takiej odpowiedzi")

    # XIII
    if XIII == "b":
        await ctx.send("Odpowiedź jest poprawna ✅")
    elif XIII == "a" or XIII == "c":
        await ctx.send("Odpowiedź jest błędna ❌")
    else:
        await ctx.send("Nie ma takiej odpowiedzi")

    # XIV
    if XIV == "a":
        await ctx.send("Odpowiedź jest poprawna ✅")
    elif XIV == "b" or XIV == "c":
        await ctx.send("Odpowiedź jest błędna ❌")
    else:
        await ctx.send("Nie ma takiej odpowiedzi")

    # XV
    if XV == "b":
        await ctx.send("Odpowiedź jest poprawna ✅")
    elif XV == "a" or XV == "c":
        await ctx.send("Odpowiedź jest błędna ❌")
    else:
        await ctx.send("Nie ma takiej odpowiedzi")

    # XVI
    if XVI == "b":
        await ctx.send("Odpowiedź jest poprawna ✅")
    elif XVI == "a" or XVI == "c":
        await ctx.send("Odpowiedź jest błędna ❌")
    else:
        await ctx.send("Nie ma takiej odpowiedzi")

    # XVII
    if XVII == "c":
        await ctx.send("Odpowiedź jest poprawna ✅")
    elif XVII == "a" or XVII == "b":
        await ctx.send("Odpowiedź jest błędna ❌")
    else:
        await ctx.send("Nie ma takiej odpowiedzi")

    # XVIII
    if XVIII == "a":
        await ctx.send("Odpowiedź jest poprawna ✅")
    elif XVIII == "b" or XVIII == "c":
        await ctx.send("Odpowiedź jest błędna ❌")
    else:
        await ctx.send("Nie ma takiej odpowiedzi")

    # XIX
    if XIX == "a":
        await ctx.send("Odpowiedź jest poprawna ✅")
    elif XIX == "b" or XIX == "c":
        await ctx.send("Odpowiedź jest błędna ❌")
    else:
        await ctx.send("Nie ma takiej odpowiedzi")

    # XX
    if XX == "a":
        await ctx.send("Odpowiedź jest poprawna ✅")
    elif XX == "b" or XX == "c":
        await ctx.send("Odpowiedź jest błędna ❌")
    else:
        await ctx.send("Nie ma takiej odpowiedzi")

@bot.command()
async def pomoc(ctx):
    await ctx.send(" ➤ $seg + obpad który posiadasz, bot powie ci gdzie umieścić ")
    await ctx.send(" ➤ $recykling, bot poda ci informacje na temat recyklingu")
    await ctx.send(" ➤ $quiz, bot zrobi quiz o recyklingu") 
    await ctx.send(" ➤ $odp, bot pyta się o odpowiedzi do quizu i je sprawdza") 
    
bot.run("token")
