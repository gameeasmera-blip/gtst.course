## Grep (Global Regular Expression Print) ajaja Linux keessatti baay'ee barbaachisaa ta'eefii hojii barruu (text) barbaaduuf gargaarudha. Fayyadaan isaa inni guddaan fayila tokko ykn baay'ee keessaa jecha, faallaa, ykn barruu adda ta'e tokko saffisaan barbaadanii adda baasuudha.

## Gubbaa fi jala (qubee guddaa fi xiqqaa) osoo garagar hin baasin barbaaduuf sarara -i fayyadamuun danda'ama.

    ........grep -i "python" fayila.txt....

## grep -n "Total" awk.gmn Jechi sun sarara meeqaffaa irratti akka argamu siif argasiisa (-n)

## Grep fi Awk lamaan isaaniiyyuu ajajoota barruu (text) keessaa odeeffannoo barbaaduuf fi xinxaluuf Linux keessatti baay'ee beekamoodha. Garuu bu'uuraan kaayyoo fi dandeettii garagaraa qabu.

# grep =Sararoota jecha tokko qaban barbaaduu fi adda baasuu (Filtering/Searching)

# awk =Barruu fi sararoota xinxaluu, faayidaaf jijjiiruu fi gabaasa hojjechuu (Text Processing/Reporting).

# grep -l filname only

# grep -o display that specific word only

# sed ===1Jecha Bakka Buusuu (Find & Replace):

Jecha fayila keessa jiru tokko jecha biraatiin bakka buusuu.=sed 's/Error/Warning/' filname.txt

# Sarara Haquu (Delete Lines):

Fakkeenyaaf, sarara 1ffaa ykn sararoota jecha tokko qaban haquu:===
sed '1d' data.txt # Sarara 1ffaa haqa
sed '/duudaa/d' data.txt # Sarara jecha "duudaa" qabu haqa

# sed '/duudaa/d' data.txt # Sarara jecha "duudaa" qabu haqa

Fayila Keessatti Jijjiirrama Mirkaneessuu (-i):sed -i 's/2025/2026/g' report.txt

# tee== tee ajaja Linux keessatti bu'aa (output) ajaja tokkorraa argamu skriinii (terminal) irratti agarsiisaa, al-takkaaniin fayila keessatti waraabee (save) gochuuf gargaarudha.

Odeeffannoo Dabalataa Fayila Keessatti Ida'uu (-a / Appen)=echo "Barruu haaraa" | tee -a list.txt
Bu'aa Skriinii Irratti Arginaa Fayilatti Unchuu (Overwrite):ls -l | tee list.txt
Fayila Baay'ee Keessatti Al-takkaaniin Barreessuu:echo "System Update Done" | tee file1.txt file2.txt file3.txt
Sudo (Mirga Administrator) Waliin Fayyadamuu:echo "127.0.0.1 mylocal.site" | sudo tee -a /etc/hosts
