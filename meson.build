project(
  'soloud', 'c', 'cpp', version : '202002', license: 'zlib', default_options : ['cpp_std=c++14']
)

cpp_args = [
  '-DWITH_MINIAUDIO',
]

includes = [
	'include',
]

dependencies = [

]

source = [
  'src/audiosource/vic/soloud_vic.cpp',
  'src/audiosource/wav/stb_vorbis.c',
  'src/audiosource/wav/soloud_wavstream.cpp',
  'src/audiosource/wav/dr_impl.cpp',
  'src/audiosource/wav/soloud_wav.cpp',
  'src/audiosource/ay/sndchip.cpp',
  'src/audiosource/ay/chipplayer.cpp',
  'src/audiosource/ay/sndbuffer.cpp',
  'src/audiosource/ay/soloud_ay.cpp',
  'src/audiosource/ay/sndrender.cpp',
  'src/audiosource/sfxr/soloud_sfxr.cpp',
  'src/audiosource/speech/tts.cpp',
  'src/audiosource/speech/resonator.cpp',
  'src/audiosource/speech/klatt.cpp',
  'src/audiosource/speech/darray.cpp',
  'src/audiosource/speech/soloud_speech.cpp',
  'src/audiosource/tedsid/ted.cpp',
  'src/audiosource/tedsid/soloud_tedsid.cpp',
  'src/audiosource/tedsid/sid.cpp',
  'src/audiosource/noise/soloud_noise.cpp',
  'src/audiosource/monotone/soloud_monotone.cpp',
  'src/audiosource/vizsn/soloud_vizsn.cpp',
  'src/audiosource/openmpt/soloud_openmpt_dll.c',
  'src/audiosource/openmpt/soloud_openmpt.cpp',
  'src/filter/soloud_eqfilter.cpp',
  'src/filter/soloud_bassboostfilter.cpp',
  'src/filter/soloud_echofilter.cpp',
  'src/filter/soloud_fftfilter.cpp',
  'src/filter/soloud_robotizefilter.cpp',
  'src/filter/soloud_dcremovalfilter.cpp',
  'src/filter/soloud_lofifilter.cpp',
  'src/filter/soloud_flangerfilter.cpp',
  'src/filter/soloud_freeverbfilter.cpp',
  'src/filter/soloud_biquadresonantfilter.cpp',
  'src/filter/soloud_waveshaperfilter.cpp',
  'src/core/soloud_core_filterops.cpp',
  'src/core/soloud_fft_lut.cpp',
  'src/core/soloud_core_voicegroup.cpp',
  'src/core/soloud_bus.cpp',
  'src/core/soloud_fader.cpp',
  'src/core/soloud_file.cpp',
  'src/core/soloud.cpp',
  'src/core/soloud_audiosource.cpp',
  'src/core/soloud_fft.cpp',
  'src/core/soloud_core_setters.cpp',
  'src/core/soloud_core_voiceops.cpp',
  'src/core/soloud_filter.cpp',
  'src/core/soloud_queue.cpp',
  'src/core/soloud_core_faderops.cpp',
  'src/core/soloud_core_basicops.cpp',
  'src/core/soloud_thread.cpp',
  'src/core/soloud_core_getters.cpp',
  'src/core/soloud_core_3d.cpp',
  'src/core/soloud_misc.cpp',
  'src/backend/miniaudio/soloud_miniaudio.cpp',
]

soloud_lib = static_library(
	'soloud',
	source,
	include_directories : includes,
	dependencies        : dependencies,
  cpp_args            : cpp_args,
)

soloud_dep = declare_dependency(include_directories : includes, link_with: soloud_lib, dependencies: dependencies)
