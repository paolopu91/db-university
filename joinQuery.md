1) Selezionare tutti gli studenti iscritti al Corso di Laurea in Economia
    answer 1)
        SELECT * 
        FROM `degrees`
        JOIN `students`
            ON `students`.`id`
        WHERE `degrees`.`name`= "Corso di Laurea in Economia";

2) Selezionare tutti i Corsi di Laurea Magistrale del Dipartimento di Neuroscienze
    answer 2)
        SELECT * 
        FROM `degrees`
        JOIN `departments`
            ON `departments`.`id` = `degrees`.`department_id`
        WHERE `degrees`.`level`= "magistrale"
            AND `departments`.`name`= "Dipartimento di Neuroscienze";

3) Selezionare tutti i corsi in cui insegna Fulvio Amato (id=44) 
    answer 3)
        SELECT * 
        FROM `teachers`
        JOIN `course_teacher`
            ON `course_teacher`.`teacher_id` = `teachers`.`id`
        JOIN `courses`
            ON `courses`.`id` = `course_teacher`.`course_id`
        WHERE `teachers`.`name`="Fulvio"
            AND`teachers`.`surname`="Amato";

4) Selezionare tutti gli studenti con i dati relativi al corso di laurea a cui sono iscritti e il relativo dipartimento, in ordine alfabetico per cognome e nome
    answer 4)
         



5) Selezionare tutti i corsi di laurea con i relativi corsi e insegnanti
    answer 5)

6) Selezionare tutti i docenti che insegnano nel Dipartimento di Matematica (54)
    answer 6) 

7) BONUS: Selezionare per ogni studente quanti tentativi d’esame ha sostenuto per superare ciascuno dei suoi esami
    answer 7) 
