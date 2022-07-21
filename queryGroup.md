1) Contare quanti iscritti ci sono stati ogni anno
    answer 1)
       SELECT COUNT(`id`), YEAR(`enrolment_date`) AS `numero_iscritti`
        FROM `students`
        GROUP BY `numero_iscritti`;
2) Contare gli insegnanti che hanno l'ufficio nello stesso edificio
    answer 2)
        SELECT COUNT(*)
        `office_address`
        FROM `teachers`
        GROUP BY `office_address`;
3) Calcolare la media dei voti di ogni appello d'esame
    answer 3)
        SELECT AVG(`vote`)
        FROM `exam_student`
        GROUP BY `vote`;
4) Contare quanti corsi di laurea ci sono per ogni dipartimento
    answer 4)
        SELECT COUNT(`name`)
            `department_id`
        FROM `degrees`
        GROUP BY `department_id`;








        
