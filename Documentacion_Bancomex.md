# Documentación de Bancomex

Este archivo documenta los módulos, archivos y procedimientos almacenados extraídos de los datos proporcionados.


# Detalle de Módulos y Procedimientos

## Módulo: ADMIN

### Archivo: ADM00201.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| COMMAND4_Click | CMXsrv_finadm_imod_desti | TIP | CMXsrv_finadm_val_tipop, sp_procxmode |
| Form_Load | CMXsrv_finadm_cons_dtip | TIP | sp_procxmode |

### Archivo: ADM00202.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Command1_Click | CMXsrv_finadm_imod_ectb | TIP | CMXsrv_finadm_val_tipop, sp_procxmode |
| Command2_Click | CMXsrv_finadm_eli_tipop | TIP, TIP_CTA | sp_procxmode |
| Form_Load | CMXsrv_finadm_cons_ectb | TIP | sp_procxmode |

### Archivo: ADM00203.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| COMMAND3_Click | CMXsrv_finadm_eli_tipop | TIP, TIP_CTA | sp_procxmode |
| COMMAND4_Click | CMXsrv_finadm_imod_itip | TIP | CMXsrv_finadm_val_tipop, sp_procxmode |
| Form_Load | CMXsrv_finadm_cons_itip | TIP | sp_procxmode |

### Archivo: ADM00204.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_finadm_lee_tipop | TIP, ACMXPLAZO, ACMXPROCMX, ACMXMB1 | sp_procxmode |
| Form_Load | CMXsrv_grl_fec_serv | N/A | SRV_MessageService, sp_procxmode |
| Mdel_Click | CMXsrv_finadm_eli_tipop | TIP, TIP_CTA | sp_procxmode |
| Mval_Click | CMXsrv_finadm_val_tipop | APEPROR, TIP, TAS, CUO, ACMXPLNCTAN, ACMXMONEDAFEC, PANCTL, ACLNCBCABCI, ACMXPLNCTAX, TIP_CTA, ACMXMONEDA, warnmsg, EVE, ACMXSUCSAL, PANVTO, ACMXINTEREFEC, COL, PANMOR | CMXsrv_fincol_eval_tbat, CMXsrv_util_fecha2, SRV_MessageService, sp_procxmode |

### Archivo: ADM00205.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| buscar_Click | CMXsrv_finadm_bus_tipope | TIP | sp_procxmode |
| proximas_Click | CMXsrv_finadm_bus_tipope | TIP | sp_procxmode |

## Módulo: COL_NEG

### Archivo: COL00102.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| CANCELAR_Click | CMXsrv_busc_tip_tas | CRD | sp_procxmode |
| ELIMINAR_Click | CMXsrv_fincol_ecuo | CUO_REN, COL, CUO | CMXsrv_fincol_pre_cuad_tas, sp_procxmode |
| Form_Activate | CMXsrv_fincol_cons_plnpa | CUO_REN, COL_REN, COL, CUO | sp_procxmode |
| Form_Load | CMXsrv_pertas_val_display | TAS | sp_procxmode |

### Archivo: COL00103.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ELIMINAR_Click | CMXsrv_fincol_eava | DAC, AVAL, AVAL_REN, COL | sp_procxmode |
| Form_Activate | CMXsrv_fincol_cons_aval | CRDCLON, AVAL, AVAL_REN, COL | sp_procxmode |

### Archivo: COL00113.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ingresar_Click | CMXsrv_fincol_iava | AVAL, AVAL_REN, CLN, COL | sp_procxmode |

### Archivo: COL00303.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_fincol_cons_pag | CAN, COL | sp_procxmode |
| proximos_Click | CMXsrv_fincol_cons_pag | CAN, COL | sp_procxmode |

### Archivo: COL00304.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_fincol_trae_det_pag | CAN, EVE | sp_procxmode |

### Archivo: COL00403.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_fincol_cons_pror | EVE, COL | sp_procxmode |

### Archivo: COL00901.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_fincol_cons_eve | EVE, COL | sp_procxmode |

### Archivo: CRD00602.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_icrd_lee_bco_swf | ACMXPAIS, COR | CMXsrv_icrd_lee_cln, sp_procxmode |
| buscar_Click | CMXsrv_icrd_busc_bco | COR | sp_procxmode |
| proximo_Click | CMXsrv_icrd_busc_bco | COR | sp_procxmode |

### Archivo: CRD01401.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_fincol_vtocre_prov | TIP, comex..ACMXINTEREFEC, COR, CRD, CUO, OBL, NEG, NEG_ADI, DAC, ACMXINTERE, ACMXMONEDA, ACMXINTEREFEC, AVAL, MYC, COL, CTO | CMXsrv_fincol_gpln, CMXsrv_finobl_imod_obl, CMXsrv_util_fecha, CMXsrv_util_val_tasas, CMXsrv_fincol_efec_calpa, sp_procxmode, CMXsrv_fincol_ctb_vcp, sp_cmx_sii_1870 |
| Form_Load | CMXsrv_fincol_prec_vtocre | TIP, CRD, CNEG, NEG, COL | sp_procxmode |

### Archivo: CRD02001.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| buscar_Click | CMXsrv_icrd_bus_lcr_bco | COR | sp_procxmode |
| proximo_Click | CMXsrv_icrd_bus_lcr_bco | COR | sp_procxmode |

### Archivo: PREFER.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Load | CMXsrv_grl_fec_serv | N/A | SRV_MessageService, sp_procxmode |
| Form_Load | CMXsrv_lee_fpro | ACMXFECPRO | sp_procxmode |

## Módulo: INGRESO

### Archivo: COL00102.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| cancelar_Click | CMXsrv_fincol_ren_fin | COL_REN, TIP, TAS, TAS_REN, EVE_REN, DAC_REN, ITA, CUO_REN, AVAL_REN, EVE, CAN_REN, COL | CMXsrv_cmx_fec_hoy, CMXsrv_fincol_pre_cuad_tas, sp_procxmode, CMXsrv_fincol_grb_col_ren, CMXsrv_lee_fpro |
| ELIMINAR_Click | CMXsrv_fincol_ecuo | CUO_REN, COL, CUO | CMXsrv_fincol_pre_cuad_tas, sp_procxmode |
| form_activate | CMXsrv_fincol_cons_plnpa | CUO_REN, COL_REN, COL, CUO | sp_procxmode |

### Archivo: COL00103.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| cancelar_Click | CMXsrv_fincol_ren_fin | COL_REN, TIP, TAS, TAS_REN, EVE_REN, DAC_REN, ITA, CUO_REN, AVAL_REN, EVE, CAN_REN, COL | CMXsrv_cmx_fec_hoy, CMXsrv_fincol_pre_cuad_tas, sp_procxmode, CMXsrv_fincol_grb_col_ren, CMXsrv_lee_fpro |
| ELIMINAR_Click | CMXsrv_fincol_eava | DAC, AVAL, AVAL_REN, COL | sp_procxmode |
| form_activate | CMXsrv_fincol_cons_aval | CRDCLON, AVAL, AVAL_REN, COL | sp_procxmode |

### Archivo: COL00104.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_Click | CMXsrv_fincol_gmod_ctr | TIP, CUO, OBL, CTR, CLN, COL, CTO | sp_procxmode |
| busca_bco | CMXsrv_icrd_lee_bco_swf | ACMXPAIS, COR | CMXsrv_icrd_lee_cln, sp_procxmode |
| fld_obl_bco_acr_LostFocus | CMXsrv_fincol_lee_bco | COR | sp_procxmode |
| fld_obl_rut_acr_LostFocus | CMXsrv_fincol_lee_cln | CLN | sp_procxmode |
| form_activate | CMXsrv_fincol_cons_ctr | OBL, CTR | sp_procxmode |

### Archivo: COL00105.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_Click | CMXsrv_fincol_ctb_oto | TIP, ACMXDESEMB, CUO, COD, vig_cmx, COL_ADI, ACMXPRMGRL, OBL, COM, MYC, ACMXMONEDA, LIB, OPE_BCI, CLN, COL, CCO | CMXsrv_mbyte_gen, CMXsrv_cmx_ing_lib, CMXsrv_ctb_impto_tim, CMXsrv_ctb_otorga, CMXsrv_cnt_gen_vig, CMXsrv_nibx_upd_tran, CMXsrv_ctb_impto_tim2, CMXsrv_vig_gra_vig, CMXsrv_nibx_nilive, CMXsrv_cyo_dsc, sp_procxmode, CMXsrv_fincol_val_col, CMXsrv_cnt_999999, sp_cmx_sii_1870, CMXsrv_util_pesos, CMXsrv_lee_fpro |

### Archivo: COL00106.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Avi5_Click | CMXsrv_icrd_dat_liq_ope | ACMXDESEMB, ASND, EVO, CRD, CNO, OBL, CUO, TRSD, NEG, COM, EVE, ACMXTIPEVE, CAN, COL | sp_procxmode |
| form_activate | CMXsrv_fincol_lee_col | COR, TAS, NEG_ADI, ACMXINTERE, TIP, CUO, CCL, ACMXFINVER, ACMXAPROBAC, COL_ADI, ACMXACTIVIDA, ACMXINTEREFEC, AVAL, ACMXSUCSAL, CLN, comex..ACMXINTEREFEC, COM, ACMXMONEDA, EVE, tbl_User, COL | PrmACMXESPECI, PrmACLNEJECTA, sp_procxmode |
| Form_Load | CMXsrv_lee_fpro | ACMXFECPRO | sp_procxmode |
| MCOLCOMI_CLICK | CMXsrv_busc_cod_ope | TIP, COL | sp_procxmode |
| MCOLCOMI_CLICK | CMXsrv_col_trae_num_ope | COL | sp_procxmode |
| MCOLCONTOTOR_CLICK | CMXsrv_busc_cod_ope | TIP, COL | sp_procxmode |
| MCOLCONTOTOR_CLICK | CMXsrv_col_trae_num_ope | COL | sp_procxmode |
| MCOLCONTOTOR_CLICK | CMXsrv_fincol_ctb_oto | TIP, ACMXDESEMB, CUO, COD, vig_cmx, COL_ADI, ACMXPRMGRL, OBL, COM, MYC, ACMXMONEDA, LIB, OPE_BCI, CLN, COL, CCO | CMXsrv_mbyte_gen, CMXsrv_cmx_ing_lib, CMXsrv_ctb_impto_tim, CMXsrv_ctb_otorga, CMXsrv_cnt_gen_vig, CMXsrv_nibx_upd_tran, CMXsrv_ctb_impto_tim2, CMXsrv_vig_gra_vig, CMXsrv_nibx_nilive, CMXsrv_cyo_dsc, sp_procxmode, CMXsrv_fincol_val_col, CMXsrv_cnt_999999, sp_cmx_sii_1870, CMXsrv_util_pesos, CMXsrv_lee_fpro |
| MCOLELI_CLICK | CMXsrv_fincol_eli_col | COL_REN, COL_ADI, COM, TAS_REN, DAC_REN, EVE_REN, DAC, CUO_REN, AVAL_REN, LIB, CAN_REN, COL | sp_procxmode |
| valida | CMXsrv_fincol_val_col | TIP, COL, warnmsg | CMXsrv_fincol_val_err, CMXsrv_fincol_val_per_tas, CMXsrv_fincol_val_adv, sp_procxmode |

### Archivo: COL00107.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_Click | CMXsrv_fincol_lee_col | COR, TAS, NEG_ADI, ACMXINTERE, TIP, CUO, CCL, ACMXFINVER, ACMXAPROBAC, COL_ADI, ACMXACTIVIDA, ACMXINTEREFEC, AVAL, ACMXSUCSAL, CLN, comex..ACMXINTEREFEC, COM, ACMXMONEDA, EVE, tbl_User, COL | PrmACMXESPECI, PrmACLNEJECTA, sp_procxmode |
| buscar_Click | CMXsrv_fincol_bsc_col | TIP | sp_procxmode |
| fld_col_tip_ope_lostfocus | CMXsrv_fincol_lee_tip | TIP | sp_procxmode |
| PROXIMAS_Click | CMXsrv_fincol_bsc_col | TIP | sp_procxmode |

### Archivo: COL00113.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ingresar_Click | CMXsrv_fincol_iava | AVAL, AVAL_REN, CLN, COL | sp_procxmode |

### Archivo: COL00701.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_Click | CMXsrv_busc_cod_ope | TIP, COL | sp_procxmode |
| aceptar_Click | CMXsrv_col_trae_num_ope | COL | sp_procxmode |
| aceptar_Click | CMXsrv_fincol_ctb_novf | CLN, COL | CMXsrv_fincol_ctb_nov, sp_procxmode, CMXsrv_lee_fpro |
| FLD_COL_COD_CLI_LOSTFOCUS | CMXsrv_fincol_lee_cln | CLN | sp_procxmode |
| FLD_COL_RUT_DEU_NOV_LostFocus | CMXsrv_fincol_lee_cln | CLN | sp_procxmode |

### Archivo: COL00702.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| form_activate | CMXsrv_fincol_cons_nov | EVE, COL | sp_procxmode |

### Archivo: COL00703.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| FLD_COL_COD_CLI_LOSTFOCUS | CMXsrv_fincol_lee_cln | CLN | sp_procxmode |
| FLD_COL_RUT_DEU_NOV_LostFocus | CMXsrv_fincol_lee_cln | CLN | sp_procxmode |

### Archivo: CRD00602.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_icrd_lee_bco_swf | ACMXPAIS, COR | CMXsrv_icrd_lee_cln, sp_procxmode |
| buscar_Click | CMXsrv_icrd_busc_bco | COR | sp_procxmode |
| proximo_Click | CMXsrv_icrd_busc_bco | COR | sp_procxmode |

### Archivo: PREFER.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Load | CMXsrv_cmx_get_codes | N/A | sp_procxmode |
| Form_Load | CMXsrv_grl_trae_cod_bco | N/A | sp_procxmode |

## Módulo: MODIFIC

### Archivo: COL00303.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_fincol_cons_tas | TAS | sp_procxmode |

### Archivo: COL00801.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_click | CMXsrv_fincol_efec_tras | TIP, comex..ACMXMONEDAFEC, COL, CUO | CMXsrv_fincol_ctb_cnd, CMXsrv_fincol_ctb_cob, CMXsrv_cnt_9000, CMXsrv_fincol_ctb_cst, sp_procxmode, CMXsrv_fincol_calc_cven |

### Archivo: COL00802.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_fincol_cons_trasp | EVE, COL | sp_procxmode |

### Archivo: COL00803.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_fincol_cons_dtrs | EVE, COL | sp_procxmode |

### Archivo: COL00901.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_fincol_cons_eve | EVE, COL | sp_procxmode |

### Archivo: COL00902.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Load | CMXsrv_fincol_cons_deve | EVE, COL | sp_procxmode |

### Archivo: COL01001.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_click | CMXsrv_fincol_cont_gst | N/A | sp_procxmode |

### Archivo: COL01002.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_fincol_cons_gst | EVE, COL | sp_procxmode |

### Archivo: COL01003.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_fincol_cons_dgst | N/A | sp_procxmode |

### Archivo: PREFER.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Load | CMXsrv_lee_fpro | ACMXFECPRO | sp_procxmode |

## Módulo: OBLIGA

### Archivo: COL00108.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| buscar_Click | CMXsrv_fincol_bsc_tip | TIP | sp_procxmode |
| Proxima_Click | CMXsrv_fincol_bsc_tip | TIP | sp_procxmode |
| proximo_Click | CMXsrv_fincol_bsc_tip | TIP | sp_procxmode |

### Archivo: Copy of OBL00103.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| anunctb_Click | CMXsrv_finobl_calc_anu | OBL | sp_procxmode, CMXsrv_finobl_efec_calpa, CMXsrv_lee_fpro |
| form_activate | CMXsrv_finobl_lee_obl | TIP, COR, OBL, ACMXINTERE, ACMXMONEDA, ACMXSUCSAL, CLN | sp_procxmode |
| Form_Load | CMXsrv_lee_fpro | ACMXFECPRO | sp_procxmode |
| Mcbeanl_Click | CMXsrv_finobl_calc_anu | OBL | sp_procxmode, CMXsrv_finobl_efec_calpa, CMXsrv_lee_fpro |
| Mcbectb_Click | CMXsrv_finobl_ctb_oto | ACMXDESEMB, TIP, COD, OBL, CTO, CCO | CMXsrv_ctbo_otorga, CMXsrv_finobl_val_obl, sp_procxmode, CMXsrv_lee_fpro |
| Mcbedel_Click | CMXsrv_fincol_eli_obl | OBL, OBL_ADI | sp_procxmode |
| Mobl_liq_ope_Click | CMXsrv_icrd_dat_liq_ope | ACMXDESEMB, ASND, EVO, CRD, CNO, OBL, CUO, TRSD, NEG, COM, EVE, ACMXTIPEVE, CAN, COL | sp_procxmode |
| valida_error | CMXsrv_finobl_val_obl | TIP, OBL, ACMXINTERE, warnmsg, OBL_ADI | CMXsrv_util_det_habil_tasa, CMXsrv_finobl_val_adv, sp_procxmode |

### Archivo: CRD00602.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| buscar_Click | CMXsrv_finobl_bus_cor | COR | sp_procxmode |
| proximo_Click | CMXsrv_finobl_bus_cor | COR | sp_procxmode |

### Archivo: OBL00102.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ELIMINAR_Click | CMXsrv_finobl_ecuo | OBL, CTO | sp_procxmode |
| form_activate | CMXsrv_finobl_gpln | OBL, CTO | CMXsrv_util_det_habil_tasa, sp_procxmode |
| form_activate | CMXsrv_finobl_cons_plnpa | OBL, CTO | sp_procxmode |

### Archivo: OBL00103.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| anunctb_Click | CMXsrv_finobl_calc_anu | OBL | sp_procxmode, CMXsrv_finobl_efec_calpa, CMXsrv_lee_fpro |
| form_activate | CMXsrv_finobl_lee_obl | TIP, COR, OBL, ACMXINTERE, ACMXMONEDA, ACMXSUCSAL, CLN | sp_procxmode |
| Form_Load | CMXsrv_lee_fpro | ACMXFECPRO | sp_procxmode |
| Mcbeanl_Click | CMXsrv_finobl_calc_anu | OBL | sp_procxmode, CMXsrv_finobl_efec_calpa, CMXsrv_lee_fpro |
| Mcbectb_Click | CMXsrv_finobl_ctb_oto | ACMXDESEMB, TIP, COD, OBL, CTO, CCO | CMXsrv_ctbo_otorga, CMXsrv_finobl_val_obl, sp_procxmode, CMXsrv_lee_fpro |
| Mcbedel_Click | CMXsrv_fincol_eli_obl | OBL, OBL_ADI | sp_procxmode |
| Mobl_liq_ope_Click | CMXsrv_icrd_dat_liq_ope | ACMXDESEMB, ASND, EVO, CRD, CNO, OBL, CUO, TRSD, NEG, COM, EVE, ACMXTIPEVE, CAN, COL | sp_procxmode |
| valida_error | CMXsrv_finobl_val_obl | TIP, OBL, ACMXINTERE, warnmsg, OBL_ADI | CMXsrv_util_det_habil_tasa, CMXsrv_finobl_val_adv, sp_procxmode |

### Archivo: OBL00104.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| buscar_Click | CMXsrv_finobl_bsc_obl | OBL | CMXsrv_finobl_bsc_obl2, sp_procxmode, CMXsrv_finobl_bsc_obl3 |
| fld_obl_tip_ope_LostFocus | CMXsrv_fincol_lee_tip | TIP | sp_procxmode |
| Proxima_Click | CMXsrv_finobl_bsc_obl | OBL | CMXsrv_finobl_bsc_obl2, sp_procxmode, CMXsrv_finobl_bsc_obl3 |

### Archivo: OBL00202.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| contabilizar_Click | CMXsrv_finobl_ictb_pag | OBL, CTO, EVO | CMXsrv_finobl_ctb_pag, sp_procxmode, CMXsrv_lee_fpro |
| contabilizar_Click | CMXsrv_finobl_obt_sdocuo | OBL, CTO | sp_procxmode |
| form_activate | CMXsrv_finobl_new_tas | CTO | sp_procxmode |

### Archivo: OBL00203.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| form_activate | CMXsrv_finobl_cons_pag | CNO | sp_procxmode |

### Archivo: OBL00204.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| form_activate | CMXsrv_finobl_cons_detp | OBL, CTO, EVO | sp_procxmode |

### Archivo: OBL00301.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| calcular_Click | CMXsrv_finobl_calc_pror | OBL | sp_procxmode, CMXsrv_finobl_efec_calpa, CMXsrv_lee_fpro |

### Archivo: OBL00303.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| form_activate | CMXsrv_finobl_cons_pror | OBL, EVO | sp_procxmode |

### Archivo: OBL00304.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| form_activate | CMXsrv_finobl_cons_dpror | OBL, EVO | sp_procxmode |

### Archivo: OBL00401.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| contabilizar_Click | CMXsrv_finobl_ctb_anu | TIP, COR, OBL, COL, CTO | CMXsrv_finobl_cbo_anu, CMXsrv_ctbo_anula, sp_procxmode, CMXsrv_lee_fpro |

### Archivo: OBL00402.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| calcular_Click | CMXsrv_finobl_calc_anu | OBL | sp_procxmode, CMXsrv_finobl_efec_calpa, CMXsrv_lee_fpro |
| form_activate | CMXsrv_finobl_cons_anu | CNO, EVO | sp_procxmode |

### Archivo: OBL00502.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| form_activate | CMXsrv_finobl_cons_mod | OBL, EVO | sp_procxmode |

### Archivo: OBL00503.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| form_activate | CMXsrv_finobl_cons_dmod | CNO, EVO | sp_procxmode |

### Archivo: OBL00601.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| efectuar_Click | CMXsrv_finobl_rev_eve | OBL, TRSD, APRCBL, EVO | CMXsrv_ctl_marc_rev, CMXsrv_ctl_chq_aprcbl, CMXsrv_finobl_rctb_pext, CMXsrv_rctb_cesi, sp_procxmode, CMXsrv_finobl_rctb_pag, CMXsrv_finobl_rctb_pror, CMXsrv_finobl_rctb_mod, CMXsrv_finobl_rctb_anu, CMXsrv_finobl_rctb_oto |
| form_activate | CMXsrv_finobl_cons_eve | EVO | sp_procxmode |

### Archivo: OBL00602.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| form_activate | CMXsrv_finobl_cons_deve | EVO | sp_procxmode |

### Archivo: OBL00701.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ELIMINAR_Click | CMXsrv_finobl_eli_ctr | CTR | sp_procxmode |
| form_activate | CMXsrv_finobl_cons_ctr | CTR | sp_procxmode |

### Archivo: OBL00702.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| nuevo_Click | CMXsrv_finobl_ing_ctr | COL, OBL, TIP, CTR | sp_procxmode |

### Archivo: OBL130.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_Click | CMXsrv_finobl_cesion_obl | OBL, COR | CMXsrv_ctl_crea_apr, sp_procxmode, CMXsrv_lee_fpro |
| banco_acreedor | CMXsrv_comgrl_lee_nom_cor | COR | sp_procxmode |
| fld_obl_cod_bco_acre_lostfocus | CMXsrv_comgrl_lee_nom_cor | COR | sp_procxmode |
| fld_obl_rut_acre_lostfocus | CMXsrv_lee_cln | CLN | sp_procxmode |
| form_activate | CMXsrv_finobl_busc_acre | OBL | sp_procxmode |

### Archivo: PREFER.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Load | CMXsrv_cmx_get_codes | N/A | sp_procxmode |

## Módulo: PAGOS

### Archivo: COL00301.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| CALCULAR_Click | CMXsrv_fincol_efec_calpa | TF_PPAG, TIP, TAS, CUO, comex..ACMXMONEDA, COL_ADI, OBL, CTR, NEG_ADI, ACMXINTERE, CAN, ICR, COL | CMXsrv_fincol_eval_tnem, CMXsrv_fincol_eval_tmor, CMXsrv_util_det_habil, sp_procxmode, CMXsrv_fincol_calc_reba, CMXsrv_fincol_eval_tasa, CMXsrv_fincol_eval_tneg, CMXsrv_fincol_efcal_cv, CMXsrv_fincol_cal_tas_sfr |

### Archivo: COL00303.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_fincol_cons_pag | CAN, COL | sp_procxmode |

### Archivo: COL00304.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Load | CMXsrv_fincol_cons_detp | ACMXDESEMB, EVE, COL, CUO | sp_procxmode |

### Archivo: COL00401.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_fincol_calc_pror | ACMXINTERE, COL | CMXsrv_call_val_tas, sp_procxmode, CMXsrv_fincol_efec_calpa |

### Archivo: COL00402.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Contabilizar_Click | CMXsrv_fincol_cont_pror | TAS, CRD, NEG_ADI, ACMXINTERE, TIP, CUO, OBL, CAM_TAS, ACMXPLAZO, COL_ADI, LIB, ACMXINTEREFEC, CLN, ACMXOPEIMP, CTO, de, comex..ACMXINTEREFEC, COD, COM, ACMXMONEDAFEC, EVE, CAN, COL | CMXsrv_mbyte_gen, CMXsrv_fincol_ctb_pror, CMXsrv_get_ult_dia_habil, CMXsrv_cmx_ing_lib, CMXsrv_ctb_impto_tim, CMXsrv_ipuc_gen_pln, CMXsrv_util_val_tasas, sp_procxmode, CMXsrv_pertas_pror_tas, CMXsrv_cmx_get_codes, CMXsrv_int_ccx_cns, CMXsrv_util_pesos, CMXsrv_fincol_cam_new_tas, CMXsrv_lee_fpro |

### Archivo: COL00403.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_fincol_cons_pror | EVE, COL | sp_procxmode |

### Archivo: COL00404.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_fincol_cons_dpror | ACMXDESEMB, EVE, COL | sp_procxmode |

### Archivo: COL00501.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_busc_cod_ope | TIP, COL | sp_procxmode |
| Aceptar_Click | CMXsrv_col_trae_num_ope | COL | sp_procxmode |
| Aceptar_Click | CMXsrv_fincol_cctb_anu | TIP, CUO, COD, OBL, TF_ENL, ENL, CAN, COL, CTO | CMXsrv_busc_cod_ope, CMXsrv_enl_act_enl, sp_procxmode, CMXsrv_fincol_ctb_anu, sp_cmx_sii_1870, CMXsrv_lee_fpro |
| Form_Load | CMXsrv_fincol_calc_anu | TIP, COL | sp_procxmode, CMXsrv_fincol_efec_calpa |
| Form_Load | CMXsrv_busc_cod_ope | TIP, COL | sp_procxmode |

### Archivo: COL00502.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| CALCULAR_Click | CMXsrv_fincol_calc_anu | TIP, COL | sp_procxmode, CMXsrv_fincol_efec_calpa |
| Form_Activate | CMXsrv_fincol_cons_anu | ACMXDESEMB, CAN, EVE, COL | sp_procxmode |

### Archivo: COL00602.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_fincol_cons_mod | EVE, COL | sp_procxmode |

### Archivo: COL00603.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_fincol_cons_dmod | CAN, EVE | sp_procxmode |

### Archivo: PREFER.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Load | CMXsrv_lee_fpro | ACMXFECPRO | sp_procxmode |
| Form_Load | CMXsrv_grl_trae_cod_bco | N/A | sp_procxmode |

## Módulo: PGOEXT

### Archivo: PGOCOL01.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| calcular_Click | CMXsrv_fincol_cal_pext | TIP, CUO, comex..ACMXMONEDA, OBL, CTR, COL, CTO | CMXsrv_fincol_calc_reba, CMXsrv_fincol_eval_tasa, sp_procxmode |
| Contabilizar_Click | CMXsrv_busc_cod_ope | TIP, COL | sp_procxmode |
| Contabilizar_Click | CMXsrv_fincol_ctb_pext | TIP, ACMXDESEMB, comex..ACMXINTEREFEC, TAS, CUO, COD, OBL, COL_ADI, ACMXMONEDAFEC, CTR, NEG_ADI, ACMXINTERE, EVE, ACMXINTEREFEC, COL, CTO, CCO | CMXsrv_ctb_pago, CMXsrv_util_gen_vig, sp_procxmode, CMXsrv_lee_fpro |

### Archivo: PGOOBL01.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| calcular_Click | CMXsrv_finobl_cal_pext | TIP, OBL, ACMXINTERE, ACMXMONEDA, OBL_ADI, CTO | CMXsrv_finobl_eval_tasa, sp_procxmode, CMXsrv_fincol_cal_tas_sfr |
| Contabilizar_Click | CMXsrv_finobl_ctb_pext | ACMXDESEMB, TIP, COD, OBL, ACMXMONEDAFEC, CTO, CCO | CMXsrv_ctbo_pago, sp_procxmode, CMXsrv_lee_fpro |

### Archivo: PREFER.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Load | CMXsrv_grl_fec_serv | N/A | SRV_MessageService, sp_procxmode |
| Form_Load | CMXsrv_lee_fpro | ACMXFECPRO | sp_procxmode |

## Módulo: ARCOS

### Archivo: ARC00100.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Eliminar_Click | CMXsrv_iarc_eli_arc | ADI, CRD, ARC, NEG, COB, INF, COL | sp_procxmode |
| Form_activate | CMXsrv_iarc_busc_arc | ARC | sp_procxmode |

### Archivo: ARC00101.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_click | CMXsrv_iinf_busc_inf | INF | sp_procxmode |
| aceptar_click | CMXsrv_iarc_act_arc | CRD, comex..ACMXMONEDA, ARC, NEG, CBR, ACMXMONEDAFEC, INF, COL | CMXsrv_cmx_get_codes, PrmACMXMONEDAFEC, CMXsrv_util_opr_fec, sp_procxmode |
| Form_Load | CMXsrv_iarc_lee_arc | ARC | sp_procxmode |

### Archivo: INFO0201.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| buscar_Click | CMXsrv_iinf_busc_opr | ARC | sp_procxmode |
| Form_activate | CMXsrv_iinf_lee_vlr | INF | PrmACMXCLACOM, sp_procxmode |

### Archivo: INFO0202.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_click | CMXsrv_iarc_act_arc | CRD, comex..ACMXMONEDA, ARC, NEG, CBR, ACMXMONEDAFEC, INF, COL | CMXsrv_cmx_get_codes, PrmACMXMONEDAFEC, CMXsrv_util_opr_fec, sp_procxmode |
| Form_activate | CMXsrv_iinf_busc_inf | INF | sp_procxmode |
| reversar_Click | CMXsrv_iinf_rev_evi | INF, ARC, INC, EVI | CMXsrv_com_rev, sp_procxmode |

## Módulo: COBERIMP

### Archivo: COB00101.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_icob_lee_pln | DIC, POSBCX10, COB, ACMXBCOCEN, ACMXMONEDA, ACMXPAIS | CMXsrv_cmx_get_codes, CMXsrv_icob_obs_pln, sp_procxmode |
| Mcobcur_Click | CMXsrv_icob_cur_cob | comex.dbo, COB | CMXsrv_icob_ctb_reem, sp_procxmode, CMXsrv_icob_val_cob |
| Mcobcur_Click | CMXsrv_icob_pag_sop | DDI, ACMXDESEMB, ADI, DIC, ACMXPRMGRL, ACMXMONEDAFEC, COB, INF, warnmsg | CMXsrv_get_ult_dia_habil, CMXsrv_icob_refresh_pos, CMXsrv_val_cta_cte, CMXsrv_calc_imp_4pct, CMXsrv_icbr_act_rem, sp_procxmode, CMXsrv_icob_ctb_sop, CMXsrv_ctb_imp_ddi_so, CMXsrv_cmx_get_codes, CMXsrv_iddi_marc_ddi2, CMXsrv_icob_val_cob |
| MCOBELI_CLICK | CMXsrv_icob_eli_pln | COB | sp_procxmode |
| Mcobrev_Click | CMXsrv_icob_rev_etd | POSBCX10, TRSD, PSO, comex..COB, COB | CMXsrv_icob_refresh_pos, CMXsrv_ctl_chq_aprcbl, CMXsrv_icob_ctb_anu, CMXsrv_icob_ctb_reem, sp_procxmode, CMXsrv_pos_eli_010, CMXsrv_icob_rctb_sop |
| Mcobvali_Click | CMXsrv_icob_val_cob | DDI, LCB, ADI, CUO, ARC, NEG, CBR, COB, INF, ACMXFPAIMP, warnmsg, COL | PrmACMXPAIS, CMXsrv_pos_bcx_lee_cob, CMXsrv_util_fecha, sp_procxmode |

### Archivo: COB00201.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| buscar_click | CMXsrv_icob_busc_pln | COB | sp_procxmode |
| FLD_COB_COD_CLI_LostFocus | CMXsrv_icob_lee_cln | CLN | sp_procxmode |
| PROXIMAS_Click | CMXsrv_icob_busc_pln | COB | sp_procxmode |

### Archivo: COB00300.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ACEPTAR_Click | CMXsrv_icob_crea_norm | CRD, ARC, CBR, COB, INF, tbl_User, CLN, COL | sp_procxmode, CMXsrv_icob_get_num |

### Archivo: COB00301.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ACEPTAR_Click | CMXsrv_icob_crea_reem | DIC, COB | sp_procxmode, CMXsrv_icob_get_num, CMXsrv_cmx_get_codes, CMXsrv_pos_bcx_lee_cob, CMXsrv_pos_bcx_ing_cob |

### Archivo: COB00302.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ACEPTAR_Click | CMXsrv_icob_act_gral | CLN, COB | sp_procxmode, CMXsrv_icob_num_con, CMXsrv_icob_val_cob, CMXsrv_pos_bcx_act_cob |
| FLD_COB_COD_CLI_LostFocus | CMXsrv_icob_lee_cln2 | CLN | sp_procxmode |
| Form_Activate | CMXsrv_icob_lee_gral | ACMXBCOCEN, ACMXPAIS, COB | CMXsrv_pos_bcx_lee_cob, sp_procxmode |

### Archivo: COB00303.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ACEPTAR_Click | CMXsrv_icob_act_val | ACMXMONEDAFEC, COB | CMXsrv_get_ult_dia_habil, sp_procxmode, CMXsrv_icob_val_cob |
| Form_Activate | CMXsrv_icob_lee_val | COB | sp_procxmode |

### Archivo: COB00304.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ACEPTAR_Click | CMXsrv_icob_act_acu | COB | sp_procxmode, CMXsrv_icob_val_cob |
| Form_Activate | CMXsrv_icob_lee_acu | ACMXPAIS, COB | sp_procxmode |
| Form_Load | CMXsrv_icob_lee_acu | ACMXPAIS, COB | sp_procxmode |

### Archivo: COB00305.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ELIMINAR_Click | CMXsrv_icob_eli_int | DIC, COB | sp_procxmode |
| Form_Activate | CMXsrv_icob_busc_int | DIC | sp_procxmode |

### Archivo: COB00306.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ACEPTAR_Click | CMXsrv_icob_ingmod_int | DIC, COB | PrmACMXMONEDA, sp_procxmode, CMXsrv_icob_val_cob |
| Form_Activate | CMXsrv_icob_lee_int | DIC | sp_procxmode |

### Archivo: COB00307.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ACEPTAR_Click | CMXsrv_icob_ing_mod_srf | CLN, tbl_User, COB | CMXsrv_pos_bcx_ing_cob, sp_procxmode, CMXsrv_icob_get_num, CMXsrv_pos_bcx_act_cob |
| CmdEliminar_Click | CMXsrv_icob_eli_pln | COB | sp_procxmode |
| CmdReversar_Click | CMXsrv_icob_rev_etd | POSBCX10, TRSD, PSO, comex..COB, COB | CMXsrv_icob_refresh_pos, CMXsrv_ctl_chq_aprcbl, CMXsrv_icob_ctb_anu, CMXsrv_icob_ctb_reem, sp_procxmode, CMXsrv_pos_eli_010, CMXsrv_icob_rctb_sop |
| CURSAR_Click | CMXsrv_icob_ing_mod_srf | CLN, tbl_User, COB | CMXsrv_pos_bcx_ing_cob, sp_procxmode, CMXsrv_icob_get_num, CMXsrv_pos_bcx_act_cob |
| CURSAR_Click | CMXsrv_icob_pag_sop | DDI, ACMXDESEMB, ADI, DIC, ACMXPRMGRL, ACMXMONEDAFEC, COB, INF, warnmsg | CMXsrv_get_ult_dia_habil, CMXsrv_icob_refresh_pos, CMXsrv_val_cta_cte, CMXsrv_calc_imp_4pct, CMXsrv_icbr_act_rem, sp_procxmode, CMXsrv_icob_ctb_sop, CMXsrv_ctb_imp_ddi_so, CMXsrv_cmx_get_codes, CMXsrv_iddi_marc_ddi2, CMXsrv_icob_val_cob |
| FLD_COB_COD_CLI_LostFocus | CMXsrv_icob_lee_cln2 | CLN | sp_procxmode |
| Reversar_Click | CMXsrv_icob_rev_etd | POSBCX10, TRSD, PSO, comex..COB, COB | CMXsrv_icob_refresh_pos, CMXsrv_ctl_chq_aprcbl, CMXsrv_icob_ctb_anu, CMXsrv_icob_ctb_reem, sp_procxmode, CMXsrv_pos_eli_010, CMXsrv_icob_rctb_sop |

### Archivo: COB00501.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ACEPTAR_Click | CMXsrv_icob_anu | DIC, POSBCX10, ACMXMONEDAFEC, PSO, COB, ACMXTPOAUTN | CMXsrv_get_ult_dia_habil, CMXsrv_icob_refresh_pos, CMXsrv_icob_ctb_anu, sp_procxmode, CMXsrv_pos_bcx_act_cob, CMXsrv_icob_get_num, CMXsrv_cmx_get_codes, CMXsrv_pos_bcx_lee_cob, CMXsrv_pos_bcx_ing_cob |
| Form_Load | CMXsrv_icob_lee_anu | COB | CMXsrv_pos_bcx_lee_cob, sp_procxmode |

### Archivo: COB0601.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| FLD_COB_COD_CLI_LostFocus | CMXsrv_icob_lee_cln | CLN | sp_procxmode |

### Archivo: FORM2.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ACEPTAR_Click | CMXsrv_icob_pag_sop | DDI, ACMXDESEMB, ADI, DIC, ACMXPRMGRL, ACMXMONEDAFEC, COB, INF, warnmsg | CMXsrv_get_ult_dia_habil, CMXsrv_icob_refresh_pos, CMXsrv_val_cta_cte, CMXsrv_calc_imp_4pct, CMXsrv_icbr_act_rem, sp_procxmode, CMXsrv_icob_ctb_sop, CMXsrv_ctb_imp_ddi_so, CMXsrv_cmx_get_codes, CMXsrv_iddi_marc_ddi2, CMXsrv_icob_val_cob |

### Archivo: ORI_DEST.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ACEPTAR_Click | CMXsrv_icob_cur_reem | comex..COB, COB | CMXsrv_icob_ctb_reem, sp_procxmode, CMXsrv_icob_refresh_pos, CMXsrv_icob_val_cob |

### Archivo: PREFER.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Load | CMXsrv_grl_fec_serv | N/A | SRV_MessageService, sp_procxmode |

## Módulo: COBRANZA

### Archivo: CBR00101.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ejecut_avi_imp_999 | CMXsrv_busc_cor_swf | SWT | sp_procxmode |
| ejecut_avi_imp_999 | CMXsrv_swf_bus_sms | SMS | sp_procxmode |
| Form_Activate | CMXsrv_icbr_lee_cbr | ACMXPAIS, COR, LCB, ACMXVIATPT, ACMXBCOBCC, CBR, ACMXMONEDA, ACMXCLACOM, tbl_User, ACMXSUCSAL, CLN | PrmACMXESPECI, PrmACLNEJECTA, sp_procxmode |
| Form_Load | CMXsrv_grl_fec_serv | N/A | SRV_MessageService, sp_procxmode |
| Mcbrace_Click | CMXsrv_icbr_acep_let | comex..CBR, LCB, CBR | CMXsrv_ctl_crea_apr, sp_procxmode |
| Mcbrcon_Click | CMXsrv_icbr_cont_cbr | OPE_BCI, APRCBL, LCB, CBR | CMXsrv_ctl_marc_firma, CMXsrv_mbyte_gen, CMXsrv_icbr_val_cbr, CMXsrv_nibx_upd_tran, CMXsrv_cnt_gen_vig, sp_procxmode, CMXsrv_ctb_cbr, CMXsrv_nibx_nilive |
| Mcbreli_click | CMXsrv_icbr_eli_cbr | ARC, REMENT, CBR, comex..COL | sp_procxmode |
| McbrTxt999_Click | CMXsrv_icbr_lee_ctp | ACMXSUCSAL, MCBRCTP, CBR, ACMXPAIS, CLN, CBRANX | sp_procxmode |
| Mcbrtxtrec_Click | CMXsrv_icbr_avi1 | ACMXDESEMB, ASND, ACMXBCOBCC, ARC, CBR, ACMXINTERE, PCX, ECE, ACMXMONEDA, ACMXSUCSAL, CLN | sp_procxmode |

### Archivo: CBR00102.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_Click | CMXsrv_val_suc | ACMXSUCSAL, tbl_User | sp_procxmode |
| buscar_Click | CMXsrv_icbr_busc_cbr | ACMXSUCSAL, ACMXMONEDA, CLN, CBR | sp_procxmode |
| fld_aux_glo_ofi_LostFocus | CMXsrv_val_suc | ACMXSUCSAL, tbl_User | sp_procxmode |
| fld_cbr_cod_gdo_LostFocus | CMXsrv_icbr_lee_cln | CLN | sp_procxmode |
| fld_cbr_cod_ofi_lostfocus | CMXsrv_val_suc | ACMXSUCSAL, tbl_User | sp_procxmode |
| proximas_Click | CMXsrv_icbr_busc_cbr | ACMXSUCSAL, ACMXMONEDA, CLN, CBR | sp_procxmode |

### Archivo: CBR00103.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| crear_Click | CMXsrv_icbr_crea_cbr | CLN, tbl_User | srv_icbr_asig_num, sp_procxmode, CMXsrv_util_num_ope |
| fld_cbr_cod_gdo_LostFocus | CMXsrv_icbr_lee_cln | CLN | sp_procxmode |
| fld_cbr_cod_ofi_lostfocus | CMXsrv_val_suc | ACMXSUCSAL, tbl_User | sp_procxmode |
| INGRESAR_Click | CMXsrv_icbr_crea_cbr | CLN, tbl_User | srv_icbr_asig_num, sp_procxmode, CMXsrv_util_num_ope |

### Archivo: CBR00201.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| fld_cbr_cod_gdo_LostFocus | CMXsrv_icbr_lee_cln | CLN | sp_procxmode |
| Form_Activate | CMXsrv_icbr_lee_cob | COB | sp_procxmode |
| Form_Load | CMXsrv_icbr_lee_ctp | ACMXSUCSAL, MCBRCTP, CBR, ACMXPAIS, CLN, CBRANX | sp_procxmode |
| INGRESAR_Click | CMXsrv_icbr_act_ctp | comex..CBR, MCBRCTP, CBRANX, CBR | sp_procxmode |

### Archivo: CBR00202.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_icbr_lee_cob | COB | sp_procxmode |
| Form_Load | CMXsrv_icbr_lee_trm | ACMXVIATPT, CBR, ACMXINTERE, ACMXMONEDA, MCBRTER, ACMXCLACOM, ACMXPAIS | sp_procxmode |
| INGRESAR_Click | CMXsrv_icbr_act_trm | LCB, COM, CBR, MCBRTER, warnmsg, CLN | CMXsrv_util_fecha, CMXsrv_icbr_val_cbr, sp_procxmode |

### Archivo: CBR00203.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_icbr_lee_cob | COB | sp_procxmode |
| Form_Load | CMXsrv_icbr_lee_doc | LCB, MCBRDOC, MLCB, CBR, ACMXMONEDA | sp_procxmode |
| INGRESAR_Click | CMXsrv_icbr_act_doc | LCB, MCBRDOC, MLCB, CBR, comex..CBR | sp_procxmode |

### Archivo: CBR00301.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_icbr_busc_let | MLCB, comex..MLCB, comex..LCB | sp_procxmode |

### Archivo: CBR00302.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_Click | CMXsrv_icbr_ingmod_let | LCB, CBR, comex.dbo | CMXsrv_util_fecha, sp_procxmode |
| eliminar_Click | CMXsrv_icbr_eli_let | LCB, MCBRDOC, MLCB, CBR, comex..COL | sp_procxmode |
| Form_Activate | CMXsrv_icbr_lee_let | ACMXNOTARIO, LCB, MLCB | sp_procxmode |

### Archivo: CBR00305.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_Click | CMXsrv_icbr_prorr | comex..CBR, LCB, CBR | CMXsrv_util_fecha, CMXsrv_cnt_2600, sp_procxmode, CMXsrv_cnt_2610, CMXsrv_cnt_2620 |

### Archivo: CBR00401.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| EFECTUAR_Click | CMXsrv_icbr_rev_eve | APRCBL, TRSD, CBR, vig_trs, ECE, DIP, LIB, tbl_User | CMXsrv_icbr_rev_mod_cbr, CMXsrv_mbyte_gen, CMXsrv_ctl_marc_rev, CMXsrv_ctl_chq_aprcbl, CMXsrv_icbr_rev_prot, CMXsrv_icbr_rev_ent, CMXsrv_ctl_eli_firma, CMXsrv_icbr_rev_trfo, CMXsrv_icbr_rev_vis, CMXsrv_cnt_rev_vig, CMXsrv_icbr_rev_acep, CMXsrv_icbr_rev_inst, CMXsrv_icbr_rev_trfb, CMXsrv_rctb_rem, CMXsrv_icbr_rev_ing, CMXsrv_icbr_rev_prorr, CMXsrv_icbr_rev_liq, sp_procxmode, CMXsrv_com_rev, CMXsrv_icbr_rev_pag, sp_cmx_sii_1870 |
| Form_Activate | CMXsrv_icbr_busc_eve | ECE | sp_procxmode |

### Archivo: CBR00402.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Load | CMXsrv_icbr_lee_eve | ECE, ACMXDESEMB | sp_procxmode |
| Form_Load | CMXsrv_icbr_lee_ent_doc | CBR | sp_procxmode |

### Archivo: CBR00701.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_Click | CMXsrv_icbr_prot | LCB, CBR | sp_procxmode, CMXsrv_ctl_crea_apr, CMXsrv_cnt_950 |
| Form_Load | CMXsrv_icbr_pcg_prot | LCB, CBR | sp_procxmode |

### Archivo: CBR00801.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_Click | CMXsrv_icbr_liq_sdo | comex..CBR, LCB, CBR | CMXsrv_ctb_liq_sdo, sp_procxmode, CMXsrv_cnt_gen_vig |

### Archivo: CBR00802.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_Click | CMXsrv_icbr_act_vis | comex..CBR, CBR | sp_procxmode |
| eliminar_Click | CMXsrv_icbr_eli_rep | REP | sp_procxmode |
| Form_Activate | CMXsrv_icbr_busc_rep | REP | sp_procxmode |

### Archivo: CBR00803.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_Click | CMXsrv_icbr_imod_rep | REP, CBR | sp_procxmode |

### Archivo: CBR00804.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_Click | CMXsrv_icbr_ent_doc | comex..CBR, LCB, CBR | CMXsrv_ctl_crea_apr, sp_procxmode |
| Form_Load | CMXsrv_icbr_lee_ent_doc | CBR | sp_procxmode |

### Archivo: CBR00901.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_Click | CMXsrv_icbr_trf_ofi | comex..CBR, ACMXSUCSAL, CBR | CMXsrv_ctb_trfo, sp_procxmode |
| aceptar_Click | CMXsrv_val_suc | ACMXSUCSAL, tbl_User | sp_procxmode |

### Archivo: CBR00902.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_Click | CMXsrv_icbr_trf_bco | comex..CBR, ARC, CBR, LCB | CMXsrv_ctb_trfb, sp_procxmode |

### Archivo: COBERTU.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_Click | CMXsrv_icbr_act_inst | comex..CBR, CBR | sp_procxmode |

### Archivo: GRL00101.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| enviar_Click | CMXsrv_iswf_a_pru | switxt, switxt1 | CMXsrv_iswf_a_732, CMXsrv_iswf_esp_707b, CMXsrv_iswf_a_747, CMXsrv_iswf_a_412, CMXsrv_iswf_a_707b, CMXsrv_iswf_esp_740, CMXsrv_iswf_a_410, CMXsrv_iswf_esp_747, CMXsrv_iswf_neg_730, CMXsrv_iswf_neg_752, CMXsrv_iswf_a_700a, CMXsrv_iswf_a_707a, CMXsrv_iswf_esp_700b, CMXsrv_iswf_a_740, CMXsrv_iswf_a_700b, CMXsrv_iswf_esp_707a, srv_irem_imp_202, CMXsrv_iswf_747_neg, srv_irem_imp_100, sp_procxmode, CMXsrv_iswf_esp_700a |
| Form_Load | CMXsrv_icbr_val_cbr | DDI, LCB, COR, ADI, ARC, ACMXMONEDAFEC, CBR, ACMXINTEREFEC, warnmsg | PrmACMXPAIS, CMXsrv_icbr_val_arc, CMXsrv_util_fecha, sp_procxmode, PrmACMXMONEDAFEC |
| word_Click | CMXsrv_icbr_val_cbr | DDI, LCB, COR, ADI, ARC, ACMXMONEDAFEC, CBR, ACMXINTEREFEC, warnmsg | PrmACMXPAIS, CMXsrv_icbr_val_arc, CMXsrv_util_fecha, sp_procxmode, PrmACMXMONEDAFEC |
| word_Click | CMXsrv_iswf_a_pru | switxt, switxt1 | CMXsrv_iswf_a_732, CMXsrv_iswf_esp_707b, CMXsrv_iswf_a_747, CMXsrv_iswf_a_412, CMXsrv_iswf_a_707b, CMXsrv_iswf_esp_740, CMXsrv_iswf_a_410, CMXsrv_iswf_esp_747, CMXsrv_iswf_neg_730, CMXsrv_iswf_neg_752, CMXsrv_iswf_a_700a, CMXsrv_iswf_a_707a, CMXsrv_iswf_esp_700b, CMXsrv_iswf_a_740, CMXsrv_iswf_a_700b, CMXsrv_iswf_esp_707a, srv_irem_imp_202, CMXsrv_iswf_747_neg, srv_irem_imp_100, sp_procxmode, CMXsrv_iswf_esp_700a |

## Módulo: CRDEXT

### Archivo: BCO_BCO.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_icrd_a_ibab | MIBAB, IBAB | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_glo_ibab | IBAB, COL, MIBAB | sp_procxmode, CMXsrv_icrd_pre_78 |

### Archivo: BCO_REM.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_icrd_a_ibar | MIBAR, IBAR | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_glo_ibar | MIBAR, COL, IBAR | CMXsrv_icrd_pre_72_740, sp_procxmode |

### Archivo: BUSC_COD.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| buscar_click | CMXsrv_icrd_lee_tex_swf | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |

### Archivo: BUSC_TXT.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_icrd_lee_cod_txt_swf | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |
| buscar_click | CMXsrv_icrd_lee_txt_swf_all | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_ind_esp_ing | MCTP, CRD | sp_procxmode |
| llena_arreglo | CMXsrv_icrd_lee_tex_swf | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |
| proximo_Click | CMXsrv_icrd_lee_txt_swf_all | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |

### Archivo: CRD00207.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_Click | CMXsrv_icrd_ing_acu | CRD | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_acu | CRD | sp_procxmode |

### Archivo: CRD00701.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_Click | CMXsrv_icrd_rech_sol | CRD, comex..COL, OPE_BCI, COL, comex..CRD | CMXsrv_nibx_upd_tran, CMXsrv_ctl_crea_apr, sp_procxmode, CMXsrv_nibx_nilive |

### Archivo: CRD00801.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_Click | CMXsrv_icrd_end | INF, ARC, COL, CRD | CMXsrv_ctl_crea_apr, sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_dat_end | CRD | sp_procxmode |

### Archivo: CRD02001.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_Click | CMXsrv_icrd_asignar_cor | COR, ACMXMONEDAFEC, CRD, LCR | sp_procxmode |
| buscar_Click | CMXsrv_icrd_bus_lcr_bco | COR | sp_procxmode |
| proximo_Click | CMXsrv_icrd_bus_lcr_bco | COR | sp_procxmode |

### Archivo: PREFER.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Load | CMXsrv_grl_fec_serv | N/A | SRV_MessageService, sp_procxmode |

## Módulo: CRD_CORR

### Archivo: COR00202.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_Click | CMXsrv_icrd_asignar_cor | COR, ACMXMONEDAFEC, CRD, LCR | sp_procxmode |
| buscar_Click | CMXsrv_icrd_bus_lcr_bco | COR | sp_procxmode |
| fld_cor_cod_mtr_LostFocus | CMXsrv_icrd_lee_bco_mtr | comex..ACMXBANCOS | sp_procxmode |
| fld_cor_cod_pais_Lostfocus | CMXsrv_icrd_cor_lee_pais | comex..ACMXPAIS | sp_procxmode |
| fld_cor_cod_plz_Lostfocus | CMXsrv_icrd_lee_plz | ACMXPLAZAS | sp_procxmode |
| proximo_Click | CMXsrv_icrd_bus_lcr_bco | COR | sp_procxmode |

### Archivo: COR00906.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| buscar_Click | CMXsrv_icrd_busc_plz | comex..ACMXPLAZAS | sp_procxmode |
| proximos_Click | CMXsrv_icrd_busc_plz | comex..ACMXPLAZAS | sp_procxmode |

### Archivo: COR00907.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| buscar_Click | CMXsrv_icrd_cor_busc_pais | comex, comex..ACMXPAIS | sp_procxmode |
| proximos_Click | CMXsrv_icrd_cor_busc_pais | comex, comex..ACMXPAIS | sp_procxmode |

### Archivo: GRID_BUS.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| buscar_Click | CMXsrv_icrd_busc_bco_mtr | comex | sp_procxmode |
| proximos_Click | CMXsrv_icrd_busc_bco_mtr | comex | sp_procxmode |

## Módulo: DDI

### Archivo: DDI00101.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_Click | CMXsrv_iddi_ingmod_ddi | INF, DDI | sp_procxmode |
| continuar_Click | CMXsrv_iddi_lee_dec | DDI, ACMXVIATPT, ACMXRGMIMP, INF, ACMXBCOCEN, ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM, ACMXPAIS, CLN | sp_procxmode, CMXsrv_iddi_val_num_ddi |
| eliminar_Click | CMXsrv_iddi_eli_ddi | DDI | sp_procxmode |
| fld_ddi_fec_ii_lostfocus | CMXsrv_iddi_lee_inf | INF | sp_procxmode |
| fld_ddi_rut_imp_lostfocus | CMXsrv_iddi_lee_cln | CLN | sp_procxmode |

### Archivo: DDI01001.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Asociar_Click | CMXsrv_iddi_lee_rut | DDI | sp_procxmode |
| Asociar_Click | CMXsrv_iddi_asoc_ddi | DDI, ARC, ACMXMONEDAFEC, CBR, COB, INF, ACMXMONEDA, COL | CMXsrv_cmx_get_codes, CMXsrv_get_ult_dia_habil, CMXsrv_util_opr_fec, sp_procxmode |
| Command2_Click | CMXsrv_iddi_des_ddi | DDI, ADI, COB | sp_procxmode |
| Desasociar_Click | CMXsrv_iddi_lee_rut | DDI | sp_procxmode |
| Desasociar_Click | CMXsrv_iddi_des_ddi | DDI, ADI, COB | sp_procxmode |
| fld_aux_rut_cli_lostfocus | CMXsrv_iddi_lee_cln | CLN | sp_procxmode |
| inicio_asoc | CMXsrv_iddi_busc_asoc | ADI | sp_procxmode |
| inicio_noasoc | CMXsrv_iddi_busc_noasoc | DDI, ADI | CMXsrv_iddi_bus_noasoc_cob, CMXsrv_iddi_bus_noasoc_opr, sp_procxmode |
| proximo_no_aso_Click | CMXsrv_iddi_busc_noasoc | DDI, ADI | CMXsrv_iddi_bus_noasoc_cob, CMXsrv_iddi_bus_noasoc_opr, sp_procxmode |

## Módulo: IMPORT

### Archivo: BUSCADIR.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| buscar_Click | CMXsrv_icrd_lee_dir_cln | DIRCLN | sp_procxmode |

### Archivo: BUSC_COD.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| buscar_click | CMXsrv_icrd_lee_tex_swf | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |

### Archivo: BUSC_TXT.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_icrd_lee_cod_txt_swf | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |
| buscar_click | CMXsrv_icrd_lee_txt_swf_all | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_ind_esp_ing | MCTP, CRD | sp_procxmode |
| llena_arreglo | CMXsrv_icrd_lee_tex_swf | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |
| proximo_Click | CMXsrv_icrd_lee_txt_swf_all | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |

### Archivo: CONDESP.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXCRDsrv_icrd_a_cnd_esp | CND | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_cnd_esp | MMCND, COL, CND | sp_procxmode, CMXsrv_icrd_pre_47 |

### Archivo: CRD00101.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| clon_Click | CMXCRDsrv_icrd_clon_crd | CRS, MER, CRD, TAS, CRDCLON, COL_ADI, CND, DAC, ODOC, AVAL, COL, EMB | CMXCRDsrv_icrd_lee_tas_cln, sp_procxmode, CMXsrv_fincol_ing_modcol, CMXsrv_util_num_ope |
| Form_Activate | CMXCRDsrv_icrd_lee_crdcre | CRD_ADI, ACMXFORPAG, ACMXPAIS, ACMXVIATPT, CRD, COR, COL_ADI, ACMXFINVER, PMIX, NEG, ACMXMONEDA, tbl_User, OPE_BCI, ACMXSUCSAL, CLN, COL, DIRCLN, EMB | sp_procxmode |
| Form_Activate | CMXsrv_icrd_lee_ind_esp_ing | MCTP, CRD | sp_procxmode |
| Form_Activate | CMXsrv_icrd_lee_top | COL | sp_procxmode |
| Form_Load | CMXsrv_grl_fec_serv | N/A | SRV_MessageService, sp_procxmode |
| Form_Load | CMXsrv_cmx_get_codes | N/A | sp_procxmode |
| Form_Load | CMXsrv_trae_glo_fec | ACMXSUCSAL, ACMXDL3475FEC, tbl_User | sp_procxmode |
| Mcrdapr_Click | CMXCRDsrv_icrd_val_crd | warnmsg | sp_procxmode, CMXsrv_icrd_val_adv, CMXsrv_icrd_val_err |
| Mcrdeli_click | CMXCRDsrv_icrd_eli_crd | comex..COL, OPE_BCI, CRD | sp_procxmode |
| Mcrdtxtliq_Click | CMXsrv_icrd_lee_dat_trs | ASND, EVI, TRSD, EVE, ACMXMONEDA, COL | CMXsrv_icrd_forlin, sp_procxmode |
| Mcrdtxtope_Click | CMXsrv_icrd_dat_liq_ope | ACMXDESEMB, ASND, EVO, CRD, CNO, OBL, CUO, TRSD, NEG, COM, EVE, ACMXTIPEVE, CAN, COL | sp_procxmode |
| msg_swift | CMXsrv_iswf_a_pru | switxt, switxt1 | CMXsrv_iswf_a_732, CMXsrv_iswf_esp_707b, CMXsrv_iswf_a_747, CMXsrv_iswf_a_412, CMXsrv_iswf_a_707b, CMXsrv_iswf_esp_740, CMXsrv_iswf_a_410, CMXsrv_iswf_esp_747, CMXsrv_iswf_neg_730, CMXsrv_iswf_neg_752, CMXsrv_iswf_a_700a, CMXsrv_iswf_a_707a, CMXsrv_iswf_esp_700b, CMXsrv_iswf_a_740, CMXsrv_iswf_a_700b, CMXsrv_iswf_esp_707a, srv_irem_imp_202, CMXsrv_iswf_747_neg, srv_irem_imp_100, sp_procxmode, CMXsrv_iswf_esp_700a |

### Archivo: CRD00201.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_icrd_a_ctp | CRD, CRDCLON, MCTP, comex..COL, COL | CMXCRDsrv_icrd_lee_tas_cln, CMXsrv_fincol_imod_colcc, sp_procxmode |
| FLD_COL_COD_CLI_LostFocus | CMXsrv_icrd_lee_cln | CLN, DIRCLN | sp_procxmode |
| Form_Load | CMXsrv_lee_fpro | ACMXFECPRO | sp_procxmode |

### Archivo: CRD00202.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_icrd_a_cnd | TIP, CRD_ADI, CRD, CRDCLON, COL_ADI, COM, ACMXMONEDA, LIB, comex..COL, MAPR, MCND, COL, ACMXOPEIMP, comex..CRD | CMXMCRDsrv_icrd_lee_mapr, CMXsrv_ctb_impto_tim, CMXsrv_icrd_a_dat_apr, CMXsrv_imp_calc_aladi, CMXsrv_ctb_impto_tim2, CMXsrv_busc_cod_ope, sp_procxmode, CMXsrv_ctb_impto_tim3, CMXsrv_icrd_act_pag_mix, CMXsrv_util_pesos |
| Aceptar_Click | CMXCRDsrv_icrd_crea_crd | CRD_ADI, PMIX, ACMXMONEDA, CLN, COL | CMXsrv_imp_calc_aladi, CMXsrv_fincol_imod_colcc, sp_procxmode, CMXCRDsrv_icrd_lee_tas_cln, CMXsrv_util_num_ope, CMXsrv_fincol_ing_modcol |
| fld_col_fec_vto_LostFocus | CMXsrv_util_det_habil | ACMXFERIADO | sp_procxmode |

### Archivo: CRD00203.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_icrd_busc_emb | comex..EMB, comex..MEMB | sp_procxmode |

### Archivo: CRD00204.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ELIMINAR_Click | CMXsrv_icrd_eli_emb | comex..COL, EMB, COL, CRD | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_emb1 | CRS, COL, EMB | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_emb2 | COL, EMB | sp_procxmode |
| ingresar_Click | CMXsrv_icrd_a_emb1 | CRS, MEMB, CRD, MCRS, CRDCLON, COL, EMB | sp_procxmode |
| ingresar_Click | CMXsrv_icrd_a_emb2 | EMB, COL, MEMB, CRD | sp_procxmode |
| VALIDA_EMBARQUE | CMXsrv_icrd_val_emb2 | warnmsg | sp_procxmode |
| VALIDA_EMBARQUE | CMXsrv_icrd_val_emb1 | INF, ARC, warnmsg | sp_procxmode |

### Archivo: CRD00205.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_icrd_act_ref | MREF, CRD, CRDCLON, comex..MREF, comex..COL, COL | sp_procxmode |
| Form_Load | CMXsrv_icrd_act_ref | MREF, CRD, CRDCLON, comex..MREF, comex..COL, COL | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_ref | COR, COL, CRD | sp_procxmode |

### Archivo: CRD00301.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| FLD_COL_COD_CLI_LostFocus | CMXsrv_icrd_lee_cln | CLN, DIRCLN | sp_procxmode |

### Archivo: CRD0063.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXCRDsrv_icrd_apr_sol | TIP, CRD, COL_ADI, COM, LIB, OPE_BCI, sysobjects, CLN, COL | CMXsrv_mbyte_gen, CMXsrv_icrd_asignar_cor, CMXsrv_ctb_impto_tim, CMXsrv_cmx_ing_lib, CMXsrv_nibx_upd_tran, CMXsrv_ctb_impto_tim2, CMXsrv_lee_paridad, CMXsrv_iswf_a_700, CMXsrv_fincol_imod_colcc, sp_procxmode, CMXsrv_ctb_impto_tim22, CMXsrv_ctb_impto_tim3, CMXsrv_icrd_val_crd, CMXsrv_util_pesos, CMXsrv_nibx_nilive |
| Form_Load | CMXsrv_icrd_lee_crdapr | CRS, CRD, COL_ADI, DAC, ACMXAPROBAC | CMXsrv_icrd_pre_72, sp_procxmode |

### Archivo: CRD00701.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_icrd_rech_sol | CRD, comex..COL, OPE_BCI, COL, comex..CRD | CMXsrv_nibx_upd_tran, CMXsrv_ctl_crea_apr, sp_procxmode, CMXsrv_nibx_nilive |

### Archivo: DESCMERC.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXCRDsrv_icrd_a_desc_merc | MER | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_desc_merc | MMER, MER | sp_procxmode |

### Archivo: DOCUMENT.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_icrd_a_otr_doc | ODOC, MODOC | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_otr_doc | ODOC, MODOC | sp_procxmode, CMXsrv_icrd_pre_46 |

### Archivo: GRL00101.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| enviar_Click | CMXsrv_iswf_a_pru | switxt, switxt1 | CMXsrv_iswf_a_732, CMXsrv_iswf_esp_707b, CMXsrv_iswf_a_747, CMXsrv_iswf_a_412, CMXsrv_iswf_a_707b, CMXsrv_iswf_esp_740, CMXsrv_iswf_a_410, CMXsrv_iswf_esp_747, CMXsrv_iswf_neg_730, CMXsrv_iswf_neg_752, CMXsrv_iswf_a_700a, CMXsrv_iswf_a_707a, CMXsrv_iswf_esp_700b, CMXsrv_iswf_a_740, CMXsrv_iswf_a_700b, CMXsrv_iswf_esp_707a, srv_irem_imp_202, CMXsrv_iswf_747_neg, srv_irem_imp_100, sp_procxmode, CMXsrv_iswf_esp_700a |

## Módulo: INFORME

### Archivo: ARC00100.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Eliminar_Click | CMXsrv_iarc_eli_arc | ADI, CRD, ARC, NEG, COB, INF, COL | sp_procxmode |
| Form_Activate | CMXsrv_iarc_busc_arc | ARC | sp_procxmode |

### Archivo: INFO0101.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_iinf_lee0_inf | INF | PrmACMXFPAIMP, PrmACMXMONEDA, PrmACLNEJECTA, sp_procxmode |
| Form_Activate | CMXsrv_iinf_lee_tablas | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | sp_procxmode |
| Form_Activate | CMXsrv_iinf_lee1_inf | INF, CLN | PrmACMXCLACOM, PrmACMXESPECI, sp_procxmode, PrmACLNEJECTA, PrmACMXETDINF |
| Form_Activate | CMXsrv_iinf_lee_cln | CLN | PrmACLNEJECTA, sp_procxmode |
| Form_Activate | CMXsrv_iinf_lee2_inf | INF | PrmACMXPAIS, PrmACMXORIDVS, PrmACMXRGMIMP, sp_procxmode, PrmACMXBCOBCC, PrmACMXBCOCEN, PrmACMXSUCSAL |
| Form_Activate | CMXsrv_iinf_avi_miscb | INF | PrmACMXBCOBCC, sp_procxmode |
| Maviapr_Click | CMXsrv_iinf_avi_misca | INF, CLN | PrmACMXPAIS, PrmACMXORIDVS, PrmACMXRGMIMP, PrmACMXCLACOM, sp_procxmode, PrmACMXFPAIMP, PrmACLNEJECTA, PrmACMXSUCSAL, PrmACMXMONEDA, PrmACMXETDINF |
| Maviapr_Click | CMXsrv_iinf_avi_miscb | INF | PrmACMXBCOBCC, sp_procxmode |
| Mavicom_Click | CMXsrv_iinf_avi_misca | INF, CLN | PrmACMXPAIS, PrmACMXORIDVS, PrmACMXRGMIMP, PrmACMXCLACOM, sp_procxmode, PrmACMXFPAIMP, PrmACLNEJECTA, PrmACMXSUCSAL, PrmACMXMONEDA, PrmACMXETDINF |
| Mavicom_Click | CMXsrv_iinf_avi_miscb | INF | PrmACMXBCOBCC, sp_procxmode |
| Mavicom_Click | CMXsrv_icrd_lee_dat_com | TIP, ACMXDESEMB, ASND, CRD, EVI, COM, TRSD, EVE, ACMXMONEDA | PrmACMXMONEDA, sp_procxmode |
| Mavimis1_Click | CMXsrv_iinf_avi_misca | INF, CLN | PrmACMXPAIS, PrmACMXORIDVS, PrmACMXRGMIMP, PrmACMXCLACOM, sp_procxmode, PrmACMXFPAIMP, PrmACLNEJECTA, PrmACMXSUCSAL, PrmACMXMONEDA, PrmACMXETDINF |
| Mavimis1_Click | CMXsrv_iinf_avi_miscb | INF | PrmACMXBCOBCC, sp_procxmode |
| Mavimis2_Click | CMXsrv_iinf_avi_misca | INF, CLN | PrmACMXPAIS, PrmACMXORIDVS, PrmACMXRGMIMP, PrmACMXCLACOM, sp_procxmode, PrmACMXFPAIMP, PrmACLNEJECTA, PrmACMXSUCSAL, PrmACMXMONEDA, PrmACMXETDINF |
| Mavimis2_Click | CMXsrv_iinf_avi_miscb | INF | PrmACMXBCOBCC, sp_procxmode |
| Mavirec_Click | CMXsrv_iinf_avi_misca | INF, CLN | PrmACMXPAIS, PrmACMXORIDVS, PrmACMXRGMIMP, PrmACMXCLACOM, sp_procxmode, PrmACMXFPAIMP, PrmACLNEJECTA, PrmACMXSUCSAL, PrmACMXMONEDA, PrmACMXETDINF |
| Mavirec_Click | CMXsrv_iinf_avi_miscb | INF | PrmACMXBCOBCC, sp_procxmode |
| Mavitib_Click | CMXsrv_iinf_avi_misca | INF, CLN | PrmACMXPAIS, PrmACMXORIDVS, PrmACMXRGMIMP, PrmACMXCLACOM, sp_procxmode, PrmACMXFPAIMP, PrmACLNEJECTA, PrmACMXSUCSAL, PrmACMXMONEDA, PrmACMXETDINF |
| Mavitib_Click | CMXsrv_iinf_avi_miscb | INF | PrmACMXBCOBCC, sp_procxmode |
| Mavitras_Click | CMXsrv_iinf_avi_misca | INF, CLN | PrmACMXPAIS, PrmACMXORIDVS, PrmACMXRGMIMP, PrmACMXCLACOM, sp_procxmode, PrmACMXFPAIMP, PrmACLNEJECTA, PrmACMXSUCSAL, PrmACMXMONEDA, PrmACMXETDINF |
| Mavitras_Click | CMXsrv_iinf_avi_miscb | INF | PrmACMXBCOBCC, sp_procxmode |
| Mavitras_Click | CMXsrv_icrd_lee_dat_trs | ASND, EVI, TRSD, EVE, ACMXMONEDA, COL | CMXsrv_icrd_forlin, sp_procxmode |
| Minfoeli_click | CMXsrv_iinf_eli_inf | INF, ARC | sp_procxmode |
| Minforev_Click | CMXsrv_iinf_busc_evi | EVI | sp_procxmode |
| Minfoval_click | CMXsrv_iinf_val_inf | INF, ACMXPAIS, warnmsg | CMXsrv_cmx_get_codes, PrmACMXPAIS, PrmACMXCLACOM, sp_procxmode |

### Archivo: INFO0102.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_iinf_ingmod_inf | INF, tbl_User, warnmsg | CMXsrv_util_fecha, sp_procxmode, PrmACMXMONEDAFEC, CMXsrv_cmx_get_codes, CMXsrv_iinf_val_inf, CMXsrv_iinf_get_num |
| Fec_pre | CMXsrv_iinf_lee_fec | N/A | CMXsrv_util_fecha, sp_procxmode |
| fld_aux_glo_cls_com_LostFocus | CMXsrv_iinf_lee_tablas | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | sp_procxmode |
| fld_aux_glo_for_pag1_LostFocus | CMXsrv_iinf_lee_tablas | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | sp_procxmode |
| fld_aux_glo_for_pag2_LostFocus | CMXsrv_iinf_lee_tablas | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | sp_procxmode |
| fld_aux_glo_for_pag3_LostFocus | CMXsrv_iinf_lee_tablas | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | sp_procxmode |
| fld_aux_glo_mon_LostFocus | CMXsrv_iinf_lee_tablas | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | sp_procxmode |
| fld_inf_cls_com_Lostfocus | CMXsrv_iinf_lee_tablas | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | sp_procxmode |
| fld_inf_cod_imp_LostFocus | CMXsrv_iinf_lee_cln | CLN | PrmACLNEJECTA, sp_procxmode |
| fld_inf_for_pag1_lostfocus | CMXsrv_iinf_lee_tablas | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | sp_procxmode |
| fld_inf_for_pag2_LostFocus | CMXsrv_iinf_lee_tablas | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | sp_procxmode |
| fld_inf_for_pag3_LostFocus | CMXsrv_iinf_lee_tablas | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | sp_procxmode |
| fld_inf_mon_inf_lostfocus | CMXsrv_iinf_lee_tablas | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | sp_procxmode |
| Form_Load | CMXsrv_iinf_lee0_inf | INF | PrmACMXFPAIMP, PrmACMXMONEDA, PrmACLNEJECTA, sp_procxmode |
| Form_Load | CMXsrv_iinf_lee1_inf | INF, CLN | PrmACMXCLACOM, PrmACMXESPECI, sp_procxmode, PrmACLNEJECTA, PrmACMXETDINF |
| Form_Load | CMXsrv_iinf_lee2_inf | INF | PrmACMXPAIS, PrmACMXORIDVS, PrmACMXRGMIMP, sp_procxmode, PrmACMXBCOBCC, PrmACMXBCOCEN, PrmACMXSUCSAL |
| valor_usd | CMXsrv_iinf_lee_usd | N/A | CMXsrv_cmx_get_codes, PrmACMXMONEDAFEC, sp_procxmode |

### Archivo: INFO0103.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_iinf_busc_inf | INF | sp_procxmode |
| buscar_Click | CMXsrv_iinf_busc_inf | INF | sp_procxmode |
| Fec_pre | CMXsrv_iinf_lee_fec | N/A | CMXsrv_util_fecha, sp_procxmode |
| fld_inf_cod_imp_LostFocus | CMXsrv_iinf_lee_cln | CLN | PrmACLNEJECTA, sp_procxmode |
| PROXIMA_Click | CMXsrv_iinf_busc_inf | INF | sp_procxmode |

### Archivo: INFO0104.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_iinf_act_apr | INF | CMXsrv_iinf_val_inf, CMXsrv_util_fecha, sp_procxmode |

### Archivo: INFO0105.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_iinf_busc_evi | EVI | sp_procxmode |
| reversar_Click | CMXsrv_iinf_rev_evi | INF, ARC, INC, EVI | CMXsrv_com_rev, sp_procxmode |

### Archivo: INFO0106.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Load | CMXsrv_iinf_lee_evi | EVI | PrmACMXSUCSAL, PrmACMXBCOCEN, sp_procxmode, PrmACMXETDINF |

### Archivo: INFO0107.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_iinf_act_tib | INF | CMXsrv_cmx_get_codes, sp_procxmode |

### Archivo: INFO0108.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_iinf_act_rec | INF | CMXsrv_util_fecha, sp_procxmode |

### Archivo: INFO0109.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_iinf_act_rib | INF | CMXsrv_cmx_get_codes, sp_procxmode |

### Archivo: INFO0110.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_iinf_busc_comp | INF | sp_procxmode |
| proximos_Click | CMXsrv_iinf_busc_comp | INF | sp_procxmode |

### Archivo: INFO0111.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_iinf_ingmod_comp | INF, warnmsg | CMXsrv_util_fecha, sp_procxmode, PrmACMXMONEDAFEC, CMXsrv_cmx_get_codes, CMXsrv_iinf_val_inf, CMXsrv_iinf_get_num |
| Fec_pre | CMXsrv_iinf_lee_fec | N/A | CMXsrv_util_fecha, sp_procxmode |
| Form_Activate | CMXsrv_iinf_lee_comp | INF | PrmACMXPAIS, PrmACMXORIDVS, PrmACMXRGMIMP, PrmACMXCLACOM, sp_procxmode, PrmACMXFPAIMP, PrmACMXVIATPT, PrmACMXMONEDA |
| Form_Activate | CMXsrv_iinf_lee_tablas | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | sp_procxmode |

### Archivo: INFO0112.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_click | CMXsrv_iinf_lee_bco | COR | PrmACMXPAIS, sp_procxmode |
| buscar_Click | CMXsrv_iinf_busc_bco | ACMXBCOBCC | sp_procxmode |

### Archivo: PREFER.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Load | CMXsrv_grl_fec_serv | N/A | SRV_MessageService, sp_procxmode |

## Módulo: MOD_ADI

### Archivo: CRD00202.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_icrd_a_cnd | TIP, CRD_ADI, CRD, CRDCLON, COL_ADI, COM, ACMXMONEDA, LIB, comex..COL, MAPR, MCND, COL, ACMXOPEIMP, comex..CRD | CMXMCRDsrv_icrd_lee_mapr, CMXsrv_ctb_impto_tim, CMXsrv_icrd_a_dat_apr, CMXsrv_imp_calc_aladi, CMXsrv_ctb_impto_tim2, CMXsrv_busc_cod_ope, sp_procxmode, CMXsrv_ctb_impto_tim3, CMXsrv_icrd_act_pag_mix, CMXsrv_util_pesos |
| busca_bco | CMXsrv_icrd_lee_bco_swf | ACMXPAIS, COR | CMXsrv_icrd_lee_cln, sp_procxmode |
| fld_col_fec_vto_LostFocus | CMXsrv_util_det_habil | ACMXFERIADO | sp_procxmode |
| Form_Load | CMXMCRDsrv_icrd_lee_mcnd | CRD_ADI, ACMXFORPAG, CRD, PMIX, ACMXMONEDA, MPMIX, MCND | sp_procxmode |

### Archivo: PREFER.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Load | CMXsrv_grl_fec_serv | N/A | SRV_MessageService, sp_procxmode |

## Módulo: MOD_CBR

### Archivo: CBR00201.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| fld_cbr_cod_gdo_LostFocus | CMXsrv_icbr_lee_cln | CLN | sp_procxmode |
| Form_Load | CMXsrv_icbr_lee_ctp | ACMXSUCSAL, MCBRCTP, CBR, ACMXPAIS, CLN, CBRANX | sp_procxmode |
| INGRESAR_Click | CMXsrv_icbr_act_ctp | comex..CBR, MCBRCTP, CBRANX, CBR | sp_procxmode |

### Archivo: CBR00202.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Load | CMXsrv_icbr_lee_trm | ACMXVIATPT, CBR, ACMXINTERE, ACMXMONEDA, MCBRTER, ACMXCLACOM, ACMXPAIS | sp_procxmode |
| INGRESAR_Click | CMXsrv_icbr_act_trm | LCB, COM, CBR, MCBRTER, warnmsg, CLN | CMXsrv_util_fecha, CMXsrv_icbr_val_cbr, sp_procxmode |

### Archivo: CBR00203.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Load | CMXsrv_icbr_lee_doc | LCB, MCBRDOC, MLCB, CBR, ACMXMONEDA | sp_procxmode |
| INGRESAR_Click | CMXsrv_icbr_act_doc | LCB, MCBRDOC, MLCB, CBR, comex..CBR | sp_procxmode |

### Archivo: CBR00301.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_icbr_busc_let | MLCB, comex..MLCB, comex..LCB | sp_procxmode |

### Archivo: CBR00302.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_Click | CMXsrv_icbr_mod_ing_let | LCB, MLCB, CBR, end | CMXsrv_util_opr_fec, sp_procxmode |
| eliminar_Click | CMXsrv_icbr_eli_let | LCB, MCBRDOC, MLCB, CBR, comex..COL | sp_procxmode |
| Form_Activate | CMXsrv_icbr_lee_let | ACMXNOTARIO, LCB, MLCB | sp_procxmode |

### Archivo: PANBASE.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| actualizar_Click | CMXsrv_icbr_acep_mod_cbr | LCB, MCBRDOC, MCBRCTP, MLCB, CBR, MCBRTER, warnmsg | CMXsrv_cnt_2800, CMXsrv_icbr_cheq_mdoc, CMXsrv_icbr_val_cbr, CMXsrv_icbr_cheq_mctp, CMXsrv_icbr_cheq_mter, sp_procxmode, CMXsrv_icbr_cheq_mlcb |
| Cancelar_Click | CMXsrv_icbr_eli_no_cont | MCBRDOC, MCBRCTP, MLCB, CBR, MCBRTER | sp_procxmode |

## Módulo: MOD_CRD

### Archivo: BCO_BCO.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_icrd_a_ibab | MIBAB, IBAB | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_glo_ibab | IBAB, COL, MIBAB | sp_procxmode, CMXsrv_icrd_pre_78 |

### Archivo: BCO_REM.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_icrd_a_ibar | MIBAR, IBAR | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_glo_ibar | MIBAR, COL, IBAR | CMXsrv_icrd_pre_72_740, sp_procxmode |

### Archivo: BUSCADIR.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| buscar_click | CMXsrv_icrd_lee_dir_cln | DIRCLN | sp_procxmode |

### Archivo: BUSCA_TE.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| buscar_Click | CMXsrv_icrd_lee_tex_swf | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |

### Archivo: BUSC_COD.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| buscar_click | CMXsrv_icrd_lee_tex_swf | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |

### Archivo: BUSC_TXT.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_icrd_lee_cod_txt_swf | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |
| buscar_click | CMXsrv_icrd_lee_txt_swf_all | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_ind_esp_ing | MCTP, CRD | sp_procxmode |
| llena_arreglo | CMXsrv_icrd_lee_tex_swf | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |
| proximo_Click | CMXsrv_icrd_lee_txt_swf_all | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |

### Archivo: CONDESP.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXMCRDsrv_icrd_a_mmcnd | MMCND | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_cnd_esp | MMCND, COL, CND | sp_procxmode, CMXsrv_icrd_pre_47 |

### Archivo: CRD00201.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_icrd_a_ctp | CRD, CRDCLON, MCTP, comex..COL, COL | CMXCRDsrv_icrd_lee_tas_cln, CMXsrv_fincol_imod_colcc, sp_procxmode |
| FLD_COL_COD_CLI_LostFocus | CMXsrv_icrd_lee_cln | CLN, DIRCLN | sp_procxmode |
| Form_Load | CMXMCRDsrv_icrd_lee_mctp | ACMXPAIS, MCTP, DIRCLN, CRD | sp_procxmode |

### Archivo: CRD00202.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_icrd_a_cnd | TIP, CRD_ADI, CRD, CRDCLON, COL_ADI, COM, ACMXMONEDA, LIB, comex..COL, MAPR, MCND, COL, ACMXOPEIMP, comex..CRD | CMXMCRDsrv_icrd_lee_mapr, CMXsrv_ctb_impto_tim, CMXsrv_icrd_a_dat_apr, CMXsrv_imp_calc_aladi, CMXsrv_ctb_impto_tim2, CMXsrv_busc_cod_ope, sp_procxmode, CMXsrv_ctb_impto_tim3, CMXsrv_icrd_act_pag_mix, CMXsrv_util_pesos |
| Form_Load | CMXMCRDsrv_icrd_lee_mcnd | CRD_ADI, ACMXFORPAG, CRD, PMIX, ACMXMONEDA, MPMIX, MCND | sp_procxmode |

### Archivo: CRD00203.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_icrd_busc_emb | comex..EMB, comex..MEMB | sp_procxmode |

### Archivo: CRD00204.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| cancelar_Click | CMXsrv_icrd_lee_desc_merc | MMER, MER | sp_procxmode |
| ELIMINAR_Click | CMXsrv_icrd_eli_emb | comex..COL, EMB, COL, CRD | sp_procxmode |
| Form_Load | CMXMCRDsrv_icrd_lee_memb2 | MEMB, EMB | sp_procxmode |
| Form_Load | CMXMCRDsrv_icrd_lee_memb1 | CRS, MEMB, EMB, MCRS | sp_procxmode |
| ingresar_Click | CMXsrv_icrd_a_emb1 | CRS, MEMB, CRD, MCRS, CRDCLON, COL, EMB | sp_procxmode |
| ingresar_Click | CMXsrv_icrd_a_emb2 | EMB, COL, MEMB, CRD | sp_procxmode |
| VALIDA_EMBARQUE | CMXsrv_icrd_val_emb2 | warnmsg | sp_procxmode |
| VALIDA_EMBARQUE | CMXsrv_icrd_val_emb1 | INF, ARC, warnmsg | sp_procxmode |

### Archivo: CRD00205.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_icrd_act_ref | MREF, CRD, CRDCLON, comex..MREF, comex..COL, COL | sp_procxmode |
| fld_obl_cod_bco_acre_DblClick | CMXsrv_icrd_lee_bco_swf | ACMXPAIS, COR | CMXsrv_icrd_lee_cln, sp_procxmode |
| fld_obl_cod_bco_acre_LostFocus | CMXsrv_icrd_lee_bco_swf | ACMXPAIS, COR | CMXsrv_icrd_lee_cln, sp_procxmode |
| Form_Load | CMXMCRDsrv_icrd_lee_mref | MREF, COR, COL, CRD | sp_procxmode |

### Archivo: CRD00206.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_icrd_ing_txt | MTXT | sp_procxmode |
| Form_Load | CMXCRDsrv_icrd_get_ing_esp | ACMXPAIS, MCTP, CRD | sp_procxmode |
| Form_Load | CMXMCRDsrv_icrd_lee_mtxt | MTXT | sp_procxmode |

### Archivo: CRD00207.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Load | CMXCRDsrv_icrd_get_pre_fra | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |

### Archivo: DESCMERC.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXMCRDsrv_icrd_a_mmer | MMER | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_desc_merc | MMER, MER | sp_procxmode |

### Archivo: DOCUME.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_icrd_a_otr_doc | ODOC, MODOC | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_otr_doc | ODOC, MODOC | sp_procxmode, CMXsrv_icrd_pre_46 |

### Archivo: MOD00603.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_fincol_lee_cod_eve | MCND, COL, CRD, COM | sp_procxmode |
| Aceptar_Click | CMXMCRDsrv_icrd_acep_mod_crd | de, TIP, CRD, COD, MCRS, OBL, EVE, LIB, warnmsg, OPE_BCI, sysobjects, COL | CMXsrv_icrd_cheq_modoc, CMXCRDsrv_icrd_val_crd, CMXsrv_icrd_cheq_memb, CMXsrv_nibx_upd_tran, CMXsrv_expcce_anl_cce, CMXsrv_fincol_ctb_mod, CMXsrv_icrd_cheq_mtxt, CMXsrv_icrd_cheq_mcnd, CMXsrv_icrd_cheq_mmer, CMXsrv_icrd_cheq_mref, CMXsrv_nibx_nilive, CMXsrv_icrd_cheq_mpmix, CMXsrv_ctl_crea_apr, CMXsrv_icrd_cheq_mibar, CMXMCRDsrv_icrd_eli_no_cont, CMXsrv_icrd_lee_tip_ope, CMXsrv_icrd_cheq_mmcnd, CMXsrv_icrd_cheq_mibab, sp_procxmode, CMXsrv_icrd_cheq_mctp, CMXsrv_icrd_cheq_mapr, CMXsrv_cnt_950 |
| cancelar_Click | CMXMCRDsrv_icrd_eli_no_cont | MREF, MEMB, MCRS, MMCND, COM, MODOC, MIBAB, CRD_AMD, MPMIX, MCTP, MMER, MCND, MIBAR, TNIH, MAPR, FE_IN_REJECTED_TRANS, MTXT | sp_procxmode |
| fld_crd_cod_bco_rem_LostFocus | CMXsrv_icrd_lee_bco_swf | ACMXPAIS, COR | CMXsrv_icrd_lee_cln, sp_procxmode |
| fld_crd_fec_mod_lostFocus | CMXsrv_fincol_efec_calpa | TF_PPAG, TIP, TAS, CUO, comex..ACMXMONEDA, COL_ADI, OBL, CTR, NEG_ADI, ACMXINTERE, CAN, ICR, COL | CMXsrv_fincol_eval_tnem, CMXsrv_fincol_eval_tmor, CMXsrv_util_det_habil, sp_procxmode, CMXsrv_fincol_calc_reba, CMXsrv_fincol_eval_tasa, CMXsrv_fincol_eval_tneg, CMXsrv_fincol_efcal_cv, CMXsrv_fincol_cal_tas_sfr |
| Form_Activate | CMXsrv_icrd_lee_ind_esp_ing | MCTP, CRD | sp_procxmode |
| Form_Load | CMXsrv_fincol_efec_calpa | TF_PPAG, TIP, TAS, CUO, comex..ACMXMONEDA, COL_ADI, OBL, CTR, NEG_ADI, ACMXINTERE, CAN, ICR, COL | CMXsrv_fincol_eval_tnem, CMXsrv_fincol_eval_tmor, CMXsrv_util_det_habil, sp_procxmode, CMXsrv_fincol_calc_reba, CMXsrv_fincol_eval_tasa, CMXsrv_fincol_eval_tneg, CMXsrv_fincol_efcal_cv, CMXsrv_fincol_cal_tas_sfr |
| Form_Load | CMXMCRDsrv_icrd_lee_mcnd | CRD_ADI, ACMXFORPAG, CRD, PMIX, ACMXMONEDA, MPMIX, MCND | sp_procxmode |

### Archivo: PREFER.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Load | CMXsrv_grl_fec_serv | N/A | SRV_MessageService, sp_procxmode |

## Módulo: NEGO_AV

### Archivo: AVISOS.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aviso1 | CMXsrv_icrd_a_rec_age | COR, TAS, CRD, CUO, CNEG, COM, NEG, TRSD, DIS, EVE, ACMXMONEDA, ACMXINTERE, ACMXSUCSAL, COL | CMXsrv_util_fecha, sp_procxmode |
| aviso1 | CMXsrv_busc_ofi_cta | CLN | PrmACMXESPECI, PrmACLNEJECTA, sp_procxmode |
| aviso1 | CMXsrv_neg_busc_arc | ARC | sp_procxmode |
| aviso1 | CMXsrv_icrd_lee_avi_adi | CRD | sp_procxmode |
| aviso3 | CMXsrv_icrd_lee_dat_trs | ASND, EVI, TRSD, EVE, ACMXMONEDA, COL | CMXsrv_icrd_forlin, sp_procxmode |
| Aviso4 | CMXsrv_icrd_dat_liq_ope | ACMXDESEMB, ASND, EVO, CRD, CNO, OBL, CUO, TRSD, NEG, COM, EVE, ACMXTIPEVE, CAN, COL | sp_procxmode |
| Aviso4 | CMXsrv_icrd_lee_dat_cln | NEG, CLN, COL | CMXsrv_trae_glo_fec, sp_procxmode |
| Aviso5 | CMXsrv_icrd_lee_dat_cln | NEG, CLN, COL | CMXsrv_trae_glo_fec, sp_procxmode |
| Aviso5 | CMXsrv_icrd_lee_avi_dis | DIS, COL | sp_procxmode |
| Aviso5 | CMXsrv_icrd_lee_avi_adi | CRD | sp_procxmode |
| Aviso5 | CMXsrv_neg_ddi_asoc | ADI | sp_procxmode |
| Aviso5 | CMXsrv_neg_busc_arc | ARC | sp_procxmode |
| Aviso5 | CMXsrv_neg_trae_vcto_mcf | COL, CUO | sp_procxmode |
| lee_aval | CMXsrv_neg_avi_lee_aval | TAS, CNEG, AVAL, CLN, COL | sp_procxmode |
| lee_nego | CMXsrv_icrd_neg_lee_crd | NEG, COL | sp_procxmode |
| lee_nego | CMXsrv_icrd_lee_neg | TAS, CRD, ACMXFINVER, NEG, NEG_ADI, DIS, COL | sp_procxmode |

### Archivo: AVI_COL.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| avi_col1 | CMXsrv_col_avi_dat_cln | TIP, CRD, DAC, ACMXESPECI, ACMXSUCSAL, CLN, COL, ACLNEJECTA | sp_procxmode |
| avi_col1 | CMXsrv_col_avi_det_pag | CCX, TIP, TAS, CRD, COB, ACMXINTERE, EVE, ACMXMONEDA, ACMXINTEREFEC, CAN, CAN_REN, COL | CMX_srv_pone_punto, CMXsrv_util_fecha, sp_procxmode |
| avi_col2 | CMXsrv_col_avi_dat_cln | TIP, CRD, DAC, ACMXESPECI, ACMXSUCSAL, CLN, COL, ACLNEJECTA | sp_procxmode |
| avi_col2 | CMXsrv_col_avi_det_oto | TIP, ACMXDESEMB, ASND, TAS, CUO, COD, NEG, ACMXINTERE, EVE, ACMXMONEDA, ACMXINTEREFEC, AVAL, CLN, COL | CMX_srv_pone_punto, CMXsrv_trae_glo_fec, sp_procxmode |
| avi_col4 | CMXsrv_col_avi_dat_cln | TIP, CRD, DAC, ACMXESPECI, ACMXSUCSAL, CLN, COL, ACLNEJECTA | sp_procxmode |
| avi_col4 | CMXsrv_col_lee_num_trs | EVE, COL, TIP, COD | CMXsrv_avigrl_lee_avitemp, sp_procxmode |
| lee_obl_pag | CMXsrv_finobl_avi_pag | CNO, EVO | CMX_srv_pone_punto, sp_procxmode |
| traspaso | CMXsrv_neg_avi_trae_asnd_mn | ACMXDESEMB, ASND, COD, TRSD, ACMXMONEDA | CMX_srv_pone_punto, sp_procxmode |
| traspaso | CMXsrv_neg_avi_trae_asnd_mx | ACMXDESEMB, ACMXMONEDA, ASND | CMX_srv_pone_punto, sp_procxmode |

### Archivo: CRD01001.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_icrd_neg_lee_crd | NEG, COL | sp_procxmode |
| Form_Activate | CMXsrv_icrd_lee_neg | TAS, CRD, ACMXFINVER, NEG, NEG_ADI, DIS, COL | sp_procxmode |
| Mcrdtxtliq_Click | CMXsrv_icrd_lee_dat_trs | ASND, EVI, TRSD, EVE, ACMXMONEDA, COL | CMXsrv_icrd_forlin, sp_procxmode |
| Mcrdtxtope_Click | CMXsrv_icrd_dat_liq_ope | ACMXDESEMB, ASND, EVO, CRD, CNO, OBL, CUO, TRSD, NEG, COM, EVE, ACMXTIPEVE, CAN, COL | sp_procxmode |
| MNEGCONT_Click | CMXsrv_icrd_cont_neg | COL, NEG, CRD, COD | CMXsrv_icrd_val_neg, CMXsrv_mbyte_gen, sp_procxmode, sp_cmx_sii_1870, CMXsrv_fincol_ictb_neg_aux |
| MNEGELI_CLICK | CMXsrv_icrd_eli_neg | CRD, COM, NEG, CND, NEG_ADI, ACMXTXTSWF, comex..COL | CMXsrv_swf_graba_det, sp_procxmode |
| precarga_datos | CMXsrv_icrd_a_rec_age | COR, TAS, CRD, CUO, CNEG, COM, NEG, TRSD, DIS, EVE, ACMXMONEDA, ACMXINTERE, ACMXSUCSAL, COL | CMXsrv_util_fecha, sp_procxmode |
| precarga_datos | CMXsrv_busc_ofi_cta | CLN | PrmACMXESPECI, PrmACLNEJECTA, sp_procxmode |

### Archivo: PREFER.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Load | CMXsrv_trae_glo_fec | ACMXSUCSAL, ACMXDL3475FEC, tbl_User | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_num_col | COL | sp_procxmode |

### Archivo: VER_PAGO.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Load | CMXsrv_icrd_bus_pago | CAN | sp_procxmode |

## Módulo: NNEGO

### Archivo: Copy of CRD02004.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ACEPTAR_Click | CMXsrv_icrd_act_doc_neg | NEG, COL, DOCNEG | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_doc_neg | NEG, EMB | sp_procxmode |

### Archivo: CRD01001.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_icrd_neg_lee_crd | NEG, COL | sp_procxmode |
| Form_Activate | CMXsrv_icrd_lee_neg | TAS, CRD, ACMXFINVER, NEG, NEG_ADI, DIS, COL | sp_procxmode |
| gen_mens_swift | CMXsrv_iswf_a_pru | switxt, switxt1 | CMXsrv_iswf_a_732, CMXsrv_iswf_esp_707b, CMXsrv_iswf_a_747, CMXsrv_iswf_a_412, CMXsrv_iswf_a_707b, CMXsrv_iswf_esp_740, CMXsrv_iswf_a_410, CMXsrv_iswf_esp_747, CMXsrv_iswf_neg_730, CMXsrv_iswf_neg_752, CMXsrv_iswf_a_700a, CMXsrv_iswf_a_707a, CMXsrv_iswf_esp_700b, CMXsrv_iswf_a_740, CMXsrv_iswf_a_700b, CMXsrv_iswf_esp_707a, srv_irem_imp_202, CMXsrv_iswf_747_neg, srv_irem_imp_100, sp_procxmode, CMXsrv_iswf_esp_700a |
| llama_pagos | CMXsrv_icrd_lee_col | CCL, COL, TAS | sp_procxmode |
| Mnegavi9_Click | CMXsrv_iswf_a_pru | switxt, switxt1 | CMXsrv_iswf_a_732, CMXsrv_iswf_esp_707b, CMXsrv_iswf_a_747, CMXsrv_iswf_a_412, CMXsrv_iswf_a_707b, CMXsrv_iswf_esp_740, CMXsrv_iswf_a_410, CMXsrv_iswf_esp_747, CMXsrv_iswf_neg_730, CMXsrv_iswf_neg_752, CMXsrv_iswf_a_700a, CMXsrv_iswf_a_707a, CMXsrv_iswf_esp_700b, CMXsrv_iswf_a_740, CMXsrv_iswf_a_700b, CMXsrv_iswf_esp_707a, srv_irem_imp_202, CMXsrv_iswf_747_neg, srv_irem_imp_100, sp_procxmode, CMXsrv_iswf_esp_700a |
| MNEGCONT_Click | CMXsrv_icrd_cont_neg | COL, NEG, CRD, COD | CMXsrv_icrd_val_neg, CMXsrv_mbyte_gen, sp_procxmode, sp_cmx_sii_1870, CMXsrv_fincol_ictb_neg_aux |
| MNEGELI_CLICK | CMXsrv_icrd_eli_neg | CRD, COM, NEG, CND, NEG_ADI, ACMXTXTSWF, comex..COL | CMXsrv_swf_graba_det, sp_procxmode |
| pertas_Click | CMXsrv_icrd_lee_col | CCL, COL, TAS | sp_procxmode |

### Archivo: CRD01002.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_icrd_busc_neg | NEG | sp_procxmode |

### Archivo: CRD01003.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Load | CMXsrv_icrd_busc_emb | comex..EMB, comex..MEMB | sp_procxmode |

### Archivo: CRD01005.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ACEPTAR_Click | CMXsrv_icrd_a_neg_emb1 | TAS, CNEG, NEG, COL, DOCNEG | sp_procxmode |
| ACEPTAR_Click | CMXsrv_icrd_a_neg_emb2 | NEG, COL, comex..COL, DOCNEG | sp_procxmode, CMXsrv_icrd_chq_doc_neg |
| CANCELAR_Click | CMXsrv_icrd_eli_doc_neg | COL, DOCNEG | sp_procxmode |
| Form_Activate | CMXsrv_icrd_lee_emb1 | CRS, COL, EMB | sp_procxmode |
| Form_Activate | CMXsrv_icrd_lee_emb2 | COL, EMB | sp_procxmode |
| Form_Activate | CMXsrv_icrd_lee_neg_emb1 | COL, NEG | sp_procxmode |
| Form_Activate | CMXsrv_icrd_lee_neg_emb2 | COL, NEG | sp_procxmode |
| Form_Activate | CMXsrv_icrd_lee_cnd_esp | MMCND, COL, CND | sp_procxmode, CMXsrv_icrd_pre_47 |
| Form_Activate | CMXsrv_icrd_lee_desc_merc | MMER, MER | sp_procxmode |

### Archivo: CRD01006.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ACEPTAR_Click | CMXsrv_icrd_a_neg_disc | COL, DIS, NEG | sp_procxmode |
| Form_Load | CMXsrv_icrd_neg_lee_disc | DIS, NEG | sp_procxmode, CMXsrv_icrd_gen_disc |

### Archivo: CRD01201.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ACEPTAR_Click | CMXsrv_icrd_ent_doc | COL, NEG, comex..COL | CMXsrv_mbyte_gen, CMXsrv_swf_graba_det, sp_procxmode |
| ELIMINAR_Click | CMXsrv_icrd_ent_doc | COL, NEG, comex..COL | CMXsrv_mbyte_gen, CMXsrv_swf_graba_det, sp_procxmode |
| Form_Load | CMXsrv_icrd_ent_doc | COL, NEG, comex..COL | CMXsrv_mbyte_gen, CMXsrv_swf_graba_det, sp_procxmode |

### Archivo: CRD01301.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ACEPTAR_Click | CMXsrv_icrd_alz_disc | comex..ACMXINTEREFEC, COR, TAS, CRD, CUO, COD, CNEG, NEG, ACMXMONEDAFEC, NEG_ADI, ACMXINTERE, ACMXBCOUSU, ACMXINTEREFEC, sysobjects, COL | CMXsrv_get_ult_dia_habil, CMXsrv_icrd_cont_alz, CMXsrv_ipuc_gen_pln, sp_procxmode, CMXsrv_cnt_950, CMXsrv_cmx_get_codes, CMXsrv_fincol_cal_tas_sfr |

### Archivo: CRD02001.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| aceptar_click | CMXCRDsrv_icrd_asignar_cor | COR, ACMXMONEDAFEC, CRD, LCR | sp_procxmode |
| BUSCAR_Click | CMXCRDsrv_icrd_bus_lcr_bco | COR | sp_procxmode |
| proximo_Click | CMXCRDsrv_icrd_bus_lcr_bco | COR | sp_procxmode |

### Archivo: CRD02004.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ACEPTAR_Click | CMXsrv_icrd_act_doc_neg | NEG, COL, DOCNEG | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_doc_neg | NEG, EMB | sp_procxmode |

### Archivo: GRL00101.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| enviar_Click | CMXsrv_iswf_a_pru | switxt, switxt1 | CMXsrv_iswf_a_732, CMXsrv_iswf_esp_707b, CMXsrv_iswf_a_747, CMXsrv_iswf_a_412, CMXsrv_iswf_a_707b, CMXsrv_iswf_esp_740, CMXsrv_iswf_a_410, CMXsrv_iswf_esp_747, CMXsrv_iswf_neg_730, CMXsrv_iswf_neg_752, CMXsrv_iswf_a_700a, CMXsrv_iswf_a_707a, CMXsrv_iswf_esp_700b, CMXsrv_iswf_a_740, CMXsrv_iswf_a_700b, CMXsrv_iswf_esp_707a, srv_irem_imp_202, CMXsrv_iswf_747_neg, srv_irem_imp_100, sp_procxmode, CMXsrv_iswf_esp_700a |
| Form_Load | CMXsrv_icrd_val_neg | DDI, COR, ADI, TAS, CUO, NEG, ACMXMONEDAFEC, DAC, ACMXINTERE, ACMXMONEDA, ACMXSIGGAR, ACMXINTEREFEC, CAN, DIS, warnmsg, AVAL, COL, CCO | CMXsrv_util_det_habil_tasa, CMXsrv_fincol_val_per_tas, CMXsrv_util_fecha, sp_procxmode |

### Archivo: PREFER.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Load | CMXsrv_grl_fec_serv | N/A | SRV_MessageService, sp_procxmode |

### Archivo: VER_PAGO.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Load | CMXsrv_icrd_bus_pago | CAN | sp_procxmode |

## Módulo: PAGCBR

### Archivo: CBR01006.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ACEPTAR_Click | CMXsrv_icbr_lee_dat_var | ACMXMONEDAFEC, CBR, ACMXPRMENL | sp_procxmode |
| ACEPTAR_Click | CMXsrv_icbr_val_pag | LCB, CBR, CCO | CMXsrv_val_cta_cte, CMXsrv_calc_imp_4pct, CMXsrv_util_fecha, sp_procxmode, CMXsrv_enl_val_sel, CMXsrv_ctb_impto_ddi |
| ACEPTAR_Click | CMXsrv_icbr_ctb_pag | LCB, ACMXDESEMB, vig_cmx, COD, ICX, COM, ACMXMONEDAFEC, CBR, PCX, DIP, LIB, CLN, CCO | CMXsrv_mbyte_gen, CMXsrv_get_ult_dia_habil, CMXsrv_val_cta_cte, CMXsrv_cnt_gen_vig, CMXsrv_calc_imp_4pct, CMXsrv_util_fecha, CMXsrv_vig_gra_vig, CMXsrv_ipuc_gen_pln, CMXsrv_icbr_act_rem, CMXsrv_enl_act_enl, sp_procxmode, CMXsrv_icbr_ctb_pag1, sp_cmx_sii_1870, CMXsrv_iddi2_gen_det_pag, CMXsrv_cmx_get_codes, CMXsrv_ctb_impto_ddi, CMXsrv_util_pesos |
| Calcular_Click | CMXsrv_icbr_cal_pag | DDI, ADI, ACMXMONEDAFEC, CBR, COB, ACMXMONEDA | CMXsrv_get_ult_dia_habil, sp_procxmode, CMXsrv_valida_tc, CMXsrv_icbr_cal_int, CMXsrv_icbr_cre_pln |
| CANCELAR_Click | CMXsrv_icbr_eli_pag | ECE, PCX, COB, ICX | sp_procxmode |
| fld_cbr_cod_des_mn_pag_lostfocus | CMXsrv_val_vig | ACMXPLNCTAN, ACMXDESEMB, ACMXPLNCTAX | sp_procxmode |
| fld_cbr_cod_des_mx_pag_lostfocus | CMXsrv_val_vig | ACMXPLNCTAN, ACMXDESEMB, ACMXPLNCTAX | sp_procxmode |
| Form_Load | CMXsrv_icbr_lee_cbr0 | ACMXMONEDA, CBR | CMXsrv_icrd_lee_cln, sp_procxmode |
| Form_Load | CMXsrv_icbr_obt_mon_nac | N/A | CMXsrv_cmx_get_codes, sp_procxmode |
| Form_Load | CMXsrv_icbr_lee_dat_pag | ACMXDESEMB, ECE, PCX, CBR | sp_procxmode |
| Form_Load | CMXsrv_icbr_pcg_pag | ACMXMONEDAFEC, CBR | PrmACMXMONEDAFEC, sp_procxmode |
| lee_cta | CMXsrv_vig_lee_cta | ACMXPLNCTAN, ACMXDESEMB, ACMXPLNCTAX | sp_procxmode |

### Archivo: CBR01007.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Activate | CMXsrv_icbr_busc_pago | PCX | sp_procxmode |

### Archivo: CBR01008.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ACEPTAR_Click | CMXsrv_icbr_val_pag | LCB, CBR, CCO | CMXsrv_val_cta_cte, CMXsrv_calc_imp_4pct, CMXsrv_util_fecha, sp_procxmode, CMXsrv_enl_val_sel, CMXsrv_ctb_impto_ddi |

### Archivo: COB00303.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_icob_act_val | ACMXMONEDAFEC, COB | CMXsrv_get_ult_dia_habil, sp_procxmode, CMXsrv_icob_val_cob |
| Form_Activate | CMXsrv_icob_lee_val | COB | sp_procxmode |

### Archivo: COB00305.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| ELIMINAR_Click | CMXsrv_icbr_eli_int_pago | PCX, ICX | sp_procxmode |
| Form_Activate | CMXsrv_icbr_busc_int | ICX | sp_procxmode |

### Archivo: COB00306.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_icbr_ingmod_int | PCX, CBR, ICX, ACMXINTEREFEC | sp_procxmode |
| Form_Activate | CMXsrv_icbr_lee_int_pago | ICX | sp_procxmode |

### Archivo: CRD00602.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Aceptar_Click | CMXsrv_icbr_lee_bco | ACMXPAIS, COR | sp_procxmode |
| buscar_Click | CMXsrv_icbr_busc_bco | COR | sp_procxmode |

### Archivo: PREFER.FRM

| Segmento          | Procedimiento Almacenado        | Tablas Referenciadas | Procedimientos Referenciados          |
|-------------------|----------------------------------|-----------------------|----------------------------------------|
| Form_Load | CMXsrv_grl_fec_serv | N/A | SRV_MessageService, sp_procxmode |
