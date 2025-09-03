✅ Tłumaczenie widoczne w Advisory – wtyczka tworzy klona zgłoszenia jako [PL] <oryginalna_nazwa> i w polu Advisory ma polski opis (wrzucony do Issue description / Background). Dzięki temu widzisz tłumaczenie dokładnie tam, gdzie patrzysz na screenie.

✅ Kopiowanie jako czysty tekst – dodałem przycisk Copy AdvisoryPL (plain text) oraz pozycję menu kontekstowego Copy translated (plain text). Kopiuje do schowka bez HTML.

✅ Zakładka „AdvisoryPL” – w naszej karcie „PL Translate” masz teraz subzakładkę AdvisoryPL z dużym polem tekstowym (łatwo skopiować/edytować).

✅ Edytowalny prompt w ustawieniach – w sekcji ustawień dodana duża textarea „Custom prompt”. Możesz dopisać np. generowanie ASVS mapping i wszystko będzie dodane do AdvisoryPL oraz do klona [PL].


Jak tego używać (zgodnie z Twoimi wymaganiami)

Ustawienia → Custom prompt

Np. taki promptyk (dowolnie modyfikuj):

Przetłumacz na polski i zachowaj sekcje: "Issue description", "Remediation", "References".

Na końcu dodaj sekcję "ASVS mapping" z odpowiednią kategorią i poziomem (np. V5.x, L1/L2/L3),

jeżeli można ją jednoznacznie wskazać.

Zapisz (Save Settings).

Automatycznie do Advisory + klon [PL]

Zostaw zaznaczone Auto-translate new issues oraz Clone translated into Issues as [PL]

– nowe wykryte Issues będą miały tworzonego klona ze spolszczeniem w Advisory.

Ręcznie na istniejących

Zaznacz Issue → PPM → Translate selected issue(s) → AdvisoryPL + [PL] clone.

Kopiowanie bez HTML

W naszej karcie „PL Translate → AdvisoryPL” kliknij Copy AdvisoryPL (plain text), lub

PPM na zaznaczonych issue → Copy translated (plain text).




WAZNE:
```
➜  burp-autotranslate-1-2 cat pom.xml |grep Path 
      <systemPath>/Applications/Burp Suite Professional.app/Contents/Resources/app/burpsuite_pro.jar</systemPath>
➜  burp-autotranslate-1-2 
```
Podaj tam link do twojego burpa przed zbudowaniem


Jak zbudować i użyć

cd burp-autotranslate-1.1.1

mvn clean package -DskipTests -q

Załaduj w Burpie fat JAR:

target/burp-autotranslate-pl-1.1.1-fat.jar




