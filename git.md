**chery-pick** komutu bir branch'ten bir comit seçip başka bir branch'e eklemenizi sağlar. Örnek olarak **A** branch'inde çalıştığınızı 
varsayalım ve **B** branch'ınden **9772dd** hash'li commit'i almak istiyorsunuz o zaman:

    $ git cherry-pick <commit hash>
    $ git cherry-pick 9772dd