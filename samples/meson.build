samples = [
	'demo',
	'positional_arguments',
	'optional_arguments',
	'flag_arguments',
	'positional_and_optional_arguments',
	'enum_class_argument',
	'remaining_arguments',
	'compound_arguments',
	'positional_and_compound_arguments',
	'integer_literals',
	'float_literals',
	'double_dash_argument',
	'pair_argument',
	'tuple_arguments',
	'nested_structures',
	'nested_structures_2',
	'printing_help',
	'printing_help_custom',
	'option_delimiters',
]

foreach sample : samples
	executable(sample, sample + '.cpp', dependencies: [structopt_dep])
endforeach
