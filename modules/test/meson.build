unity_dep = dependency('unity',
    fallback: ['unity', 'unity_dep'],
    not_found_message: 'Will not be able to do Unit testing!')

test_exe = executable('test-prog',
    files('test_runner.c', 'test_cases.c'),
    dependencies : [unity_dep, code_dep])

test('Running: Project unit test', test_exe)
