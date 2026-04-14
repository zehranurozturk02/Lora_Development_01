# Lora_Development_01

İçinde olan ana şeyler:

ATM komut altyapısı
AT+MCONF=<freq>,<sf>,<bw>,<cr>,<preamble>,<symbTimeout> ile LoRa ayarı girme
AT+MCONF? ile aktif config’i görme
AT+MRX=1 ile RX başlatma
AT+MRX=0 ile RX durdurma
ATMRST ile yazılımsal reset
Gelen paketi anlamlı formatta UART’a basma:
Company ID, Device ID, MAC Address, Control Number, RSSI, SNR, Payload
Teknik olarak içerik:

AT komutları ayrı klasörde toplandı
at_commands.h
at_commands.c
LoRa config runtime değişebilir hale getirildi
AT+MCONF ile verilen değerler AT+MRX=1 öncesi gerçekten radioya uygulanıyor
RX kapatma davranışı düzeltildi; MRX=0 sonrası sonradan paket düşme problemi azaltıldı
Kod tabanından gereksiz TX example parçaları temizlendi

yedek olarak tutuyorum 
