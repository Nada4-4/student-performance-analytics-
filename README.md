Begin
Input student_id, modules[] with marks
total ← 0
FOR each module IN modules
    IF module.mark >= 0 THEN         
        total ← total + module.mark
    END IF
END FOR

average ← total / number_of_modules
strong_subjects ← empty list

FOR each module IN modules
    IF module.mark < 55 THEN
        ADD module.name TO strong_subjects
    END IF
END FOR

OUTPUT student_id, average, strong_subjects
End
