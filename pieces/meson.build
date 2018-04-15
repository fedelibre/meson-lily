filebases = [
  'song',
  'violin',
]

foreach fb : filebases
  custom_target(fb + '_build',
    output : fb + '.pdf',
    input : fb + '.ly',
    depend_files : fb + '.ily',
#    command : ['ls', '@INPUT@', '@OUTPUT@'],
#    command : ['lilypond', '--output=pieces', '@INPUT@'],
    command : ['lilypond', '@INPUT@'],
    build_by_default : true)
endforeach
