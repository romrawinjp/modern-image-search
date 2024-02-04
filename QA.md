# Question Answering From The Lecture

1. เวลาเรา query image ที่คล้ายกันใน database ถ้า data เยอะ จะใช้เวลา query นานมาก อาจารย์พอจะมีเทคนิค หรือ datastructure ตัวไหนแนะนำที่ทำให้ query ข้อมูลได้ไวขึ้นไหมครับ
    
    Answer: เท่าที่รู้มามีการลดขนาดข้อมูลจาก float64 เป็น float32 ก็ทำให้การคำนวณเร็วขึ้นนะ ส่วน data structure อาจจะลองเน้นไปดู Big O (https://images.app.goo.gl/PGaqcneoeLht4Do49) ว่าการ Search แบบไหนดี ใน hands-on จะเป็นการเปรียบเทียบทั้งหมด เพราะว่ามีแค่ 1000 ตัว ถ้า database ใหญ่มาก ๆ น่าจะต้อง group embeddings แล้วทำ binary search tree น่าจะทำให้เร็วขึ้นค่ะ

2.  ตอนแข่งจะมีเคสที่เราต้อง train embedding model เองไหมครับ

    Answer: มีไหมนะ ถ้ามี แนะนำว่าอาจจะลองใช้วิธีการ finetuning มากกว่า เพราะว่าถ้า train อาจจะต้องใช้พลังงานเยอะมาก :)

3. ถ้าไม่ใช้เรื่องของกินเป็นเรื่องอื่นๆ เราจะหา model  จากไหนได้อีกบ้างครับ

    Answer: https://huggingface.co/models

4. ยกตัวอย่างการทำ image search โดยใช้ดาต้าเซตอื่นๆให้หน่อยได้มั้ยคะ แบบเขียนโค้ดและอธิบายคร่าวๆได้มั้ยคะ

    Answer:

5. ในการทำ image search มีเรื่องอะไรที่ต้องระวังใหมครับ

    Answer:

6. Search image by image กับ Search image by text การทำงานต่างกันไหมครับ

    Answer:

7. แนะนำการเลือก Pretrain หน่อยครับ

    Answer:


8. ตอน encode อ่ะค่ะ latent space ของ image กับ latent space ของ query มันจะเป็นอันเเดียวไหม แล้วถ้าไม่ใช่อันเดียวกัน มันหา similarity(เทียบจากคนละ space ได้ไหมคะ) ได้ยังไงหรอคะ

    Answer:


9. ใช้ metric ตัวไหนครับปกติที่ไว้เช็ค model ที่อาจจะไม่ได้เช็คแค่เรื่อง label ดูพวกภาพรวมของภาพ

    Answer:

10. อธิบายเพิ่มเติมหน่อยครับว่า แบบไหนควรsearch on the flyได้เลย หรือต้องทำแบบoffline - online

    Answer:

11. ตอนทำจริงอะไรยากที่สุดหรอครับ

    Answer:

12. เราสามารถทำ fine turning ได้ไหมครับ

    Answer:
