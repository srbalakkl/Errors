## error TS7006: Parameter 'user' implicitly has an 'any' type.
### fix: Change / method parrameter value to Any

onSubmit(user:any) {
    console.log(user)
}
