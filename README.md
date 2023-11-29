# SD500-Objects
Create a TypeScript workspace, and implement CRUD operations for students and courses. 
* Solve the question and store the data in both `data_1` and `data_2`.
* All of the functions should not mutate `data_1` and `data_2`, but rather make the changes in immutable way.
* Use utility types when needed.

```typescript
type Course = { id: number, title: string, description: string; };
type Student = { id: number, name: string, courses: Course[]; };

let data_1: readonly Student[] = Object.freeze([]);
let data_2: { [student_id: string]: { name: string, courses: Course[]; }; } = Object.freeze({});

getStudent(student_id: number): Student{ }
addStudent(student: Student): boolean{ }
updateStudent(student: Student): boolean{ }
removeStudent(student_id: number): boolean{ }

getCourse(student_id: number, course_id: number): Course{ }
addCourse(student_id: number, course: Course): boolean{ }
updateCourse(student_id: number, course: Course): boolean{ }
removeCourse(student_id: number, course_id: number): boolean{ }
```
