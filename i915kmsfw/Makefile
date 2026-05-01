_VALID_I915KMODS=skylake broxton kabylake geminilake cannonlake \
	icelake elkhartlake tigerlake rocketlake alderlake \
	dg1 dg2 meteorlake battlemage lunarlake pantherlake

I915KMODS?=	${_VALID_I915KMODS}

.for var in ${I915KMODS}
.if empty(_VALID_I915KMODS:M${var})
_INVALID_I915_KMODS+=	${var}
.endif
.endfor
.if !empty(_INVALID_I915_KMODS)
.error "${_INVALID_I915_KMODS} firmware doesn't exists"
.endif

.if ${I915KMODS:Mskylake}
SUBDIR+=	skldmc_123 \
		skldmc_126 \
		skldmc_127 \
		sklguc_1 \
		sklguc_3203 \
		sklguc_3300 \
		sklguc_4 \
		sklguc_4901 \
		sklguc_61 \
		sklguc_6200 \
		sklguc_6903 \
		sklguc_7011 \
		sklguc_933 \
		sklhuc_01071398 \
		sklhuc_200
.endif

.if ${I915KMODS:Mbroxton}
SUBDIR+=	bxtdmc_107 \
		bxtguc_3203 \
		bxtguc_3300 \
		bxtguc_4901 \
		bxtguc_6200 \
		bxtguc_6903 \
		bxtguc_7011 \
		bxtguc_87 \
		bxtguc_929 \
		bxthuc_01071398 \
		bxthuc_0182893 \
		bxthuc_200
.endif

.if ${I915KMODS:Mkabylake}
SUBDIR+=	kbldmc_101 \
		kbldmc_104 \
		kblguc_3203 \
		kblguc_3300 \
		kblguc_4901 \
		kblguc_6200 \
		kblguc_6903 \
		kblguc_7011 \
		kblguc_914 \
		kblguc_939 \
		kblhuc_02001810 \
		kblhuc_400 \
		cmlguc_3300 \
		cmlguc_4901 \
		cmlguc_6200 \
		cmlguc_6903 \
		cmlguc_7011 \
		cmlhuc_400
.endif

.if ${I915KMODS:Mgeminilake}
SUBDIR+=	glkdmc_104 \
		glkguc_3203 \
		glkguc_3300 \
		glkguc_4901 \
		glkguc_6200 \
		glkguc_6903 \
		glkguc_7011 \
		glkhuc_03012893 \
		glkhuc_400
.endif

.if ${I915KMODS:Mcannonlake}
SUBDIR+=	cnldmc_106 \
		cnldmc_107
.endif

.if ${I915KMODS:Micelake}
SUBDIR+=	icldmc_107 \
		icldmc_109 \
		iclguc_3203 \
		iclguc_3300 \
		iclguc_4901 \
		iclguc_6200 \
		iclguc_6903 \
		iclguc_7011 \
		iclhuc_843238 \
		iclhuc_900
.endif

.if ${I915KMODS:Melkhartlake}
SUBDIR+=	ehlguc_3304 \
		ehlguc_4901 \
		ehlguc_6200 \
		ehlguc_6903 \
		ehlguc_7011 \
		ehlhuc_900
.endif

.if ${I915KMODS:Mtigerlake}
SUBDIR+=	tgldmc_204 \
		tgldmc_206 \
		tgldmc_208 \
		tgldmc_212 \
		tglguc_3520 \
		tglguc_4901 \
		tglguc_6200 \
		tglguc_6903 \
		tglguc_7011 \
		tglguc_70 \
		tglhuc \
		tglhuc_703 \
		tglhuc_7012 \
		tglhuc_750 \
		tglhuc_793
.endif

.if ${I915KMODS:Mrocketlake}
SUBDIR+=	rkldmc_202 \
		rkldmc_203
.endif

.if ${I915KMODS:Malderlake}
SUBDIR+=	adlpdmc \
		adlsdmc_201 \
		adlpdmc_209 \
		adlpdmc_210 \
		adlpdmc_212 \
		adlpdmc_214 \
		adlpdmc_216 \
		adlpguc_6203 \
		adlpguc_6903 \
		adlpguc_70 \
		adlpguc_7011
.endif

.if ${I915KMODS:Mdg1}
SUBDIR+=	dg1dmc_202 \
		dg1guc_4901 \
		dg1guc_6200 \
		dg1guc_6903 \
		dg1guc_70 \
		dg1guc_7011 \
		dg1huc \
		dg1huc_771 \
		dg1huc_793
.endif

.if ${I915KMODS:Mdg2}
SUBDIR+=	dg2dmc_206 \
		dg2dmc_207 \
		dg2dmc_208 \
		dg2guc_70 \
		dg2guc_7012 \
		dg2guc_7041 \
		dg2hucgsc
.endif

.if ${I915KMODS:Mmeteorlake}
SUBDIR+=	mtldmc_210 \
		mtldmc \
		mtlgsc_1 \
		mtlguc_70 \
		mtlhucgsc
.endif

.if ${I915KMODS:Mbattlemage}
SUBDIR+=	bmgdmc
.endif

.if ${I915KMODS:Mlunarlake}
SUBDIR+=	xe2lpddmc
.endif

.if ${I915KMODS:Mpantherlake}
SUBDIR+=	xe3lpddmc \
		xe3lpd3002dmc \
		xe3plpddmc
.endif

SUBDIR_PARALLEL=

.include <bsd.subdir.mk>
