# Índice de Módulos y Procedimientos

## Producto

- [Módulo](#Módulo)
## ----------

- [--------](#--------)
## Financiamiento

- [ADMIN](#ADMIN)
- [COL_NEG](#COL_NEG)
- [INGRESO](#INGRESO)
- [MODIFIC](#MODIFIC)
- [OBLIGA](#OBLIGA)
- [PAGOS](#PAGOS)
- [PGOEXT](#PGOEXT)
## Importaciones

- [ARCOS](#ARCOS)
- [COBERIMP](#COBERIMP)
- [COBRANZA](#COBRANZA)
- [CRDEXT](#CRDEXT)
- [CRD_CORR](#CRD_CORR)
- [DDI](#DDI)
- [IMPORT](#IMPORT)
- [INFORME](#INFORME)
- [MOD_ADI](#MOD_ADI)
- [MOD_CBR](#MOD_CBR)
- [MOD_CRD](#MOD_CRD)
- [NEGO_AV](#NEGO_AV)
- [NNEGO](#NNEGO)
- [PAGCBR](#PAGCBR)

## Módulo <a name="Módulo"></a>

| Archivo | Segmento | Procedimiento Almacenado |
|---------|---------|--------------------------|
| Archivo | `Segmento` | `Procedimiento Almacenado` |

[🔝 Volver al índice](#Índice-de-Módulos-y-Procedimientos)


## -------- <a name="--------"></a>

| Archivo | Segmento | Procedimiento Almacenado |
|---------|---------|--------------------------|
| --------- | `----------` | `--------------------------` |

[🔝 Volver al índice](#Índice-de-Módulos-y-Procedimientos)


## ADMIN <a name="ADMIN"></a>

| Archivo | Segmento | Procedimiento Almacenado |
|---------|---------|--------------------------|
| [ADM00201.FRM](./ADM00201.FRM) | ``COMMAND4_Click`` | ``CMXsrv_finadm_imod_desti`` |
| [ADM00201.FRM](./ADM00201.FRM) | ``Form_Load`` | ``CMXsrv_finadm_cons_dtip`` |
| [ADM00202.FRM](./ADM00202.FRM) | ``Command1_Click`` | ``CMXsrv_finadm_imod_ectb`` |
| [ADM00202.FRM](./ADM00202.FRM) | ``Command2_Click`` | ``CMXsrv_finadm_eli_tipop`` |
| [ADM00202.FRM](./ADM00202.FRM) | ``Form_Load`` | ``CMXsrv_finadm_cons_ectb`` |
| [ADM00203.FRM](./ADM00203.FRM) | ``COMMAND3_Click`` | ``CMXsrv_finadm_eli_tipop`` |
| [ADM00203.FRM](./ADM00203.FRM) | ``COMMAND4_Click`` | ``CMXsrv_finadm_imod_itip`` |
| [ADM00203.FRM](./ADM00203.FRM) | ``Form_Load`` | ``CMXsrv_finadm_cons_itip`` |
| [ADM00204.FRM](./ADM00204.FRM) | ``Form_Activate`` | ``CMXsrv_finadm_lee_tipop`` |
| [ADM00204.FRM](./ADM00204.FRM) | ``Form_Load`` | ``CMXsrv_grl_fec_serv`` |
| [ADM00204.FRM](./ADM00204.FRM) | ``Mdel_Click`` | ``CMXsrv_finadm_eli_tipop`` |
| [ADM00204.FRM](./ADM00204.FRM) | ``Mval_Click`` | ``CMXsrv_finadm_val_tipop`` |
| [ADM00205.FRM](./ADM00205.FRM) | ``buscar_Click`` | ``CMXsrv_finadm_bus_tipope`` |
| [ADM00205.FRM](./ADM00205.FRM) | ``proximas_Click`` | ``CMXsrv_finadm_bus_tipope`` |

[🔝 Volver al índice](#Índice-de-Módulos-y-Procedimientos)


## COL_NEG <a name="COL_NEG"></a>

| Archivo | Segmento | Procedimiento Almacenado |
|---------|---------|--------------------------|
| [COL00102.FRM](./COL00102.FRM) | ``CANCELAR_Click`` | ``CMXsrv_busc_tip_tas`` |
| [COL00102.FRM](./COL00102.FRM) | ``ELIMINAR_Click`` | ``CMXsrv_fincol_ecuo`` |
| [COL00102.FRM](./COL00102.FRM) | ``Form_Activate`` | ``CMXsrv_fincol_cons_plnpa`` |
| [COL00102.FRM](./COL00102.FRM) | ``Form_Load`` | ``CMXsrv_pertas_val_display`` |
| [COL00103.FRM](./COL00103.FRM) | ``ELIMINAR_Click`` | ``CMXsrv_fincol_eava`` |
| [COL00103.FRM](./COL00103.FRM) | ``Form_Activate`` | ``CMXsrv_fincol_cons_aval`` |
| [COL00113.FRM](./COL00113.FRM) | ``ingresar_Click`` | ``CMXsrv_fincol_iava`` |
| [COL00302.FRM](./COL00302.FRM) | ``CONTABILIZAR_Click`` | ``CMXsrv_fincol_ictb_pag`` |
| [COL00303.FRM](./COL00303.FRM) | ``aviso_Click`` | ``CMXsrv_fincol_avi_2_fin`` |
| [COL00303.FRM](./COL00303.FRM) | ``Form_Activate`` | ``CMXsrv_fincol_cons_pag`` |
| [COL00303.FRM](./COL00303.FRM) | ``proximos_Click`` | ``CMXsrv_fincol_cons_pag`` |
| [COL00304.FRM](./COL00304.FRM) | ``Form_Activate`` | ``CMXsrv_fincol_trae_det_pag`` |
| [COL00403.FRM](./COL00403.FRM) | ``aviso_Click`` | ``CMXsrv_fincol_avi_3_fin`` |
| [COL00403.FRM](./COL00403.FRM) | ``Form_Activate`` | ``CMXsrv_fincol_cons_pror`` |
| [COL00901.FRM](./COL00901.FRM) | ``EFECTUAR_Click`` | ``CMXsrv_fincol_rev_eve`` |
| [COL00901.FRM](./COL00901.FRM) | ``Form_Activate`` | ``CMXsrv_fincol_cons_eve`` |
| [CRD00602.FRM](./CRD00602.FRM) | ``Aceptar_Click`` | ``CMXsrv_icrd_lee_bco_swf`` |
| [CRD00602.FRM](./CRD00602.FRM) | ``buscar_Click`` | ``CMXsrv_icrd_busc_bco`` |
| [CRD00602.FRM](./CRD00602.FRM) | ``proximo_Click`` | ``CMXsrv_icrd_busc_bco`` |
| [CRD01401.FRM](./CRD01401.FRM) | ``Aceptar_Click`` | ``CMXsrv_fincol_vtocre_prov`` |
| [CRD01401.FRM](./CRD01401.FRM) | ``Form_Load`` | ``CMXsrv_fincol_prec_vtocre`` |
| [CRD02001.FRM](./CRD02001.FRM) | ``buscar_Click`` | ``CMXsrv_icrd_bus_lcr_bco`` |
| [CRD02001.FRM](./CRD02001.FRM) | ``proximo_Click`` | ``CMXsrv_icrd_bus_lcr_bco`` |
| [PREFER.FRM](./PREFER.FRM) | ``Form_Load`` | ``CMXsrv_grl_fec_serv`` |
| [PREFER.FRM](./PREFER.FRM) | ``Form_Load`` | ``CMXsrv_lee_fpro`` |

[🔝 Volver al índice](#Índice-de-Módulos-y-Procedimientos)


## INGRESO <a name="INGRESO"></a>

| Archivo | Segmento | Procedimiento Almacenado |
|---------|---------|--------------------------|
| [COL00102.FRM](./COL00102.FRM) | ``cancelar_Click`` | ``CMXsrv_fincol_ren_fin`` |
| [COL00102.FRM](./COL00102.FRM) | ``ELIMINAR_Click`` | ``CMXsrv_fincol_ecuo`` |
| [COL00102.FRM](./COL00102.FRM) | ``form_activate`` | ``CMXsrv_fincol_gpln`` |
| [COL00102.FRM](./COL00102.FRM) | ``form_activate`` | ``CMXsrv_fincol_cons_plnpa`` |
| [COL00103.FRM](./COL00103.FRM) | ``cancelar_Click`` | ``CMXsrv_fincol_ren_fin`` |
| [COL00103.FRM](./COL00103.FRM) | ``ELIMINAR_Click`` | ``CMXsrv_fincol_eava`` |
| [COL00103.FRM](./COL00103.FRM) | ``form_activate`` | ``CMXsrv_fincol_cons_aval`` |
| [COL00104.FRM](./COL00104.FRM) | ``aceptar_Click`` | ``CMXsrv_fincol_gmod_ctr`` |
| [COL00104.FRM](./COL00104.FRM) | ``busca_bco`` | ``CMXsrv_icrd_lee_bco_swf`` |
| [COL00104.FRM](./COL00104.FRM) | ``fld_obl_bco_acr_LostFocus`` | ``CMXsrv_fincol_lee_bco`` |
| [COL00104.FRM](./COL00104.FRM) | ``fld_obl_rut_acr_LostFocus`` | ``CMXsrv_fincol_lee_cln`` |
| [COL00104.FRM](./COL00104.FRM) | ``form_activate`` | ``CMXsrv_fincol_cons_ctr`` |
| [COL00105.FRM](./COL00105.FRM) | ``aceptar_Click`` | ``CMXsrv_fincol_ctb_oto`` |
| [COL00106.FRM](./COL00106.FRM) | ``avi1_Click`` | ``CMXsrv_icrd_avi_crd`` |
| [COL00106.FRM](./COL00106.FRM) | ``Avi5_Click`` | ``CMXsrv_icrd_dat_liq_ope`` |
| [COL00106.FRM](./COL00106.FRM) | ``form_activate`` | ``CMXsrv_fincol_lee_col`` |
| [COL00106.FRM](./COL00106.FRM) | ``Form_Load`` | ``CMXsrv_lee_fpro`` |
| [COL00106.FRM](./COL00106.FRM) | ``MCOLCOMI_CLICK`` | ``CMXsrv_busc_cod_ope`` |
| [COL00106.FRM](./COL00106.FRM) | ``MCOLCOMI_CLICK`` | ``CMXsrv_col_trae_num_ope`` |
| [COL00106.FRM](./COL00106.FRM) | ``MCOLCONTOTOR_CLICK`` | ``CMXsrv_busc_cod_ope`` |
| [COL00106.FRM](./COL00106.FRM) | ``MCOLCONTOTOR_CLICK`` | ``CMXsrv_col_trae_num_ope`` |
| [COL00106.FRM](./COL00106.FRM) | ``MCOLCONTOTOR_CLICK`` | ``CMXsrv_fincol_ctb_oto`` |
| [COL00106.FRM](./COL00106.FRM) | ``MCOLELI_CLICK`` | ``CMXsrv_fincol_eli_col`` |
| [COL00106.FRM](./COL00106.FRM) | ``valida`` | ``CMXsrv_fincol_val_col`` |
| [COL00107.FRM](./COL00107.FRM) | ``aceptar_Click`` | ``CMXsrv_fincol_lee_col`` |
| [COL00107.FRM](./COL00107.FRM) | ``buscar_Click`` | ``CMXsrv_fincol_bsc_col`` |
| [COL00107.FRM](./COL00107.FRM) | ``fld_col_tip_ope_lostfocus`` | ``CMXsrv_fincol_lee_tip`` |
| [COL00107.FRM](./COL00107.FRM) | ``PROXIMAS_Click`` | ``CMXsrv_fincol_bsc_col`` |
| [COL00108.FRM](./COL00108.FRM) | ``buscar_Click`` | ``CMXsrv_fincol_bsc_TIP`` |
| [COL00113.FRM](./COL00113.FRM) | ``ingresar_Click`` | ``CMXsrv_fincol_iava`` |
| [COL00701.FRM](./COL00701.FRM) | ``aceptar_Click`` | ``CMXsrv_busc_cod_ope`` |
| [COL00701.FRM](./COL00701.FRM) | ``aceptar_Click`` | ``CMXsrv_col_trae_num_ope`` |
| [COL00701.FRM](./COL00701.FRM) | ``aceptar_Click`` | ``CMXsrv_fincol_ctb_novf`` |
| [COL00701.FRM](./COL00701.FRM) | ``FLD_COL_COD_CLI_LOSTFOCUS`` | ``CMXsrv_fincol_lee_cln`` |
| [COL00701.FRM](./COL00701.FRM) | ``FLD_COL_RUT_DEU_NOV_LostFocus`` | ``CMXsrv_fincol_lee_cln`` |
| [COL00702.FRM](./COL00702.FRM) | ``form_activate`` | ``CMXsrv_fincol_cons_nov`` |
| [COL00703.FRM](./COL00703.FRM) | ``FLD_COL_COD_CLI_LOSTFOCUS`` | ``CMXsrv_fincol_lee_cln`` |
| [COL00703.FRM](./COL00703.FRM) | ``FLD_COL_RUT_DEU_NOV_LostFocus`` | ``CMXsrv_fincol_lee_cln`` |
| [COL00703.FRM](./COL00703.FRM) | ``form_activate`` | ``CMXsrv_fincol_cons_dnov`` |
| [COL00704.FRM](./COL00704.FRM) | ``cmdAceptar_Click`` | ``CMXsrv_grabar_pag_adi_dus`` |
| [COL00704.FRM](./COL00704.FRM) | ``Form_Load`` | ``CMXsrv_buscar_pag_adi_dus`` |
| [CRD00602.FRM](./CRD00602.FRM) | ``Aceptar_Click`` | ``CMXsrv_icrd_lee_bco_swf`` |
| [CRD00602.FRM](./CRD00602.FRM) | ``buscar_Click`` | ``CMXsrv_icrd_busc_bco`` |
| [CRD00602.FRM](./CRD00602.FRM) | ``proximo_Click`` | ``CMXsrv_icrd_busc_bco`` |
| [PREFER.FRM](./PREFER.FRM) | ``Form_Load`` | ``CMXsrv_cmx_get_codes`` |
| [PREFER.FRM](./PREFER.FRM) | ``Form_Load`` | ``CMXsrv_grl_trae_cod_bco`` |

[🔝 Volver al índice](#Índice-de-Módulos-y-Procedimientos)


## MODIFIC <a name="MODIFIC"></a>

| Archivo | Segmento | Procedimiento Almacenado |
|---------|---------|--------------------------|
| [COL00303.FRM](./COL00303.FRM) | ``Form_Activate`` | ``CMXsrv_fincol_cons_tas`` |
| [COL00801.FRM](./COL00801.FRM) | ``aceptar_click`` | ``CMXsrv_fincol_efec_tras`` |
| [COL00802.FRM](./COL00802.FRM) | ``Form_Activate`` | ``CMXsrv_fincol_cons_trasp`` |
| [COL00803.FRM](./COL00803.FRM) | ``Form_Activate`` | ``CMXsrv_fincol_cons_dtrs`` |
| [COL00901.FRM](./COL00901.FRM) | ``EFECTUAR_Click`` | ``CMXsrv_fincol_rev_eve`` |
| [COL00901.FRM](./COL00901.FRM) | ``Form_Activate`` | ``CMXsrv_fincol_cons_eve`` |
| [COL00902.FRM](./COL00902.FRM) | ``Form_Load`` | ``CMXsrv_fincol_cons_deve`` |
| [COL01001.FRM](./COL01001.FRM) | ``aceptar_click`` | ``CMXsrv_fincol_cont_gst`` |
| [COL01002.FRM](./COL01002.FRM) | ``Form_Activate`` | ``CMXsrv_fincol_cons_gst`` |
| [COL01003.FRM](./COL01003.FRM) | ``Form_Activate`` | ``CMXsrv_fincol_cons_dgst`` |
| [PREFER.FRM](./PREFER.FRM) | ``Form_Load`` | ``CMXsrv_lee_fpro`` |

[🔝 Volver al índice](#Índice-de-Módulos-y-Procedimientos)


## OBLIGA <a name="OBLIGA"></a>

| Archivo | Segmento | Procedimiento Almacenado |
|---------|---------|--------------------------|
| [COL00108.FRM](./COL00108.FRM) | ``buscar_Click`` | ``CMXsrv_fincol_bsc_tip`` |
| [COL00108.FRM](./COL00108.FRM) | ``Proxima_Click`` | ``CMXsrv_fincol_bsc_tip`` |
| [COL00108.FRM](./COL00108.FRM) | ``proximo_Click`` | ``CMXsrv_fincol_bsc_tip`` |
| [Copy of OBL00103.FRM](./Copy of OBL00103.FRM) | ``anunctb_Click`` | ``CMXsrv_finobl_calc_anu`` |
| [Copy of OBL00103.FRM](./Copy of OBL00103.FRM) | ``form_activate`` | ``CMXsrv_finobl_lee_obl`` |
| [Copy of OBL00103.FRM](./Copy of OBL00103.FRM) | ``Form_Load`` | ``CMXsrv_lee_fpro`` |
| [Copy of OBL00103.FRM](./Copy of OBL00103.FRM) | ``Mcbeanl_Click`` | ``CMXsrv_finobl_calc_anu`` |
| [Copy of OBL00103.FRM](./Copy of OBL00103.FRM) | ``Mcbectb_Click`` | ``CMXsrv_finobl_ctb_oto`` |
| [Copy of OBL00103.FRM](./Copy of OBL00103.FRM) | ``Mcbedel_Click`` | ``CMXsrv_fincol_eli_obl`` |
| [Copy of OBL00103.FRM](./Copy of OBL00103.FRM) | ``Mobl_liq_ope_Click`` | ``CMXsrv_icrd_dat_liq_ope`` |
| [Copy of OBL00103.FRM](./Copy of OBL00103.FRM) | ``valida_error`` | ``CMXsrv_finobl_val_obl`` |
| [CRD00602.FRM](./CRD00602.FRM) | ``buscar_Click`` | ``CMXsrv_finobl_bus_cor`` |
| [CRD00602.FRM](./CRD00602.FRM) | ``proximo_Click`` | ``CMXsrv_finobl_bus_cor`` |
| [OBL00102.FRM](./OBL00102.FRM) | ``ELIMINAR_Click`` | ``CMXsrv_finobl_ecuo`` |
| [OBL00102.FRM](./OBL00102.FRM) | ``form_activate`` | ``CMXsrv_finobl_gpln`` |
| [OBL00102.FRM](./OBL00102.FRM) | ``form_activate`` | ``CMXsrv_finobl_cons_plnpa`` |
| [OBL00103.FRM](./OBL00103.FRM) | ``anunctb_Click`` | ``CMXsrv_finobl_calc_anu`` |
| [OBL00103.FRM](./OBL00103.FRM) | ``form_activate`` | ``CMXsrv_finobl_lee_obl`` |
| [OBL00103.FRM](./OBL00103.FRM) | ``Form_Load`` | ``CMXsrv_lee_fpro`` |
| [OBL00103.FRM](./OBL00103.FRM) | ``Mcbeanl_Click`` | ``CMXsrv_finobl_calc_anu`` |
| [OBL00103.FRM](./OBL00103.FRM) | ``Mcbectb_Click`` | ``CMXsrv_finobl_ctb_oto`` |
| [OBL00103.FRM](./OBL00103.FRM) | ``Mcbedel_Click`` | ``CMXsrv_fincol_eli_obl`` |
| [OBL00103.FRM](./OBL00103.FRM) | ``Mobl_liq_ope_Click`` | ``CMXsrv_icrd_dat_liq_ope`` |
| [OBL00103.FRM](./OBL00103.FRM) | ``valida_error`` | ``CMXsrv_finobl_val_obl`` |
| [OBL00104.FRM](./OBL00104.FRM) | ``buscar_Click`` | ``CMXsrv_finobl_bsc_obl`` |
| [OBL00104.FRM](./OBL00104.FRM) | ``fld_obl_tip_ope_LostFocus`` | ``CMXsrv_fincol_lee_tip`` |
| [OBL00104.FRM](./OBL00104.FRM) | ``Proxima_Click`` | ``CMXsrv_finobl_bsc_obl`` |
| [OBL00202.FRM](./OBL00202.FRM) | ``contabilizar_Click`` | ``CMXsrv_finobl_ictb_pag`` |
| [OBL00202.FRM](./OBL00202.FRM) | ``contabilizar_Click`` | ``CMXsrv_finobl_obt_sdocuo`` |
| [OBL00202.FRM](./OBL00202.FRM) | ``form_activate`` | ``CMXsrv_finobl_new_tas`` |
| [OBL00203.FRM](./OBL00203.FRM) | ``form_activate`` | ``CMXsrv_finobl_cons_pag`` |
| [OBL00204.FRM](./OBL00204.FRM) | ``form_activate`` | ``CMXsrv_finobl_cons_detp`` |
| [OBL00301.FRM](./OBL00301.FRM) | ``calcular_Click`` | ``CMXsrv_finobl_calc_pror`` |
| [OBL00303.FRM](./OBL00303.FRM) | ``form_activate`` | ``CMXsrv_finobl_cons_pror`` |
| [OBL00304.FRM](./OBL00304.FRM) | ``form_activate`` | ``CMXsrv_finobl_cons_dpror`` |
| [OBL00401.FRM](./OBL00401.FRM) | ``contabilizar_Click`` | ``CMXsrv_finobl_ctb_anu`` |
| [OBL00402.FRM](./OBL00402.FRM) | ``calcular_Click`` | ``CMXsrv_finobl_calc_anu`` |
| [OBL00402.FRM](./OBL00402.FRM) | ``form_activate`` | ``CMXsrv_finobl_cons_anu`` |
| [OBL00502.FRM](./OBL00502.FRM) | ``form_activate`` | ``CMXsrv_finobl_cons_mod`` |
| [OBL00503.FRM](./OBL00503.FRM) | ``form_activate`` | ``CMXsrv_finobl_cons_dmod`` |
| [OBL00601.FRM](./OBL00601.FRM) | ``efectuar_Click`` | ``CMXsrv_finobl_rev_eve`` |
| [OBL00601.FRM](./OBL00601.FRM) | ``form_activate`` | ``CMXsrv_finobl_cons_eve`` |
| [OBL00602.FRM](./OBL00602.FRM) | ``form_activate`` | ``CMXsrv_finobl_cons_deve`` |
| [OBL00701.FRM](./OBL00701.FRM) | ``ELIMINAR_Click`` | ``CMXsrv_finobl_eli_ctr`` |
| [OBL00701.FRM](./OBL00701.FRM) | ``form_activate`` | ``CMXsrv_finobl_cons_ctr`` |
| [OBL00702.FRM](./OBL00702.FRM) | ``nuevo_Click`` | ``CMXsrv_finobl_ing_ctr`` |
| [OBL130.FRM](./OBL130.FRM) | ``aceptar_Click`` | ``CMXsrv_finobl_cesion_obl`` |
| [OBL130.FRM](./OBL130.FRM) | ``banco_acreedor`` | ``CMXsrv_comgrl_lee_nom_cor`` |
| [OBL130.FRM](./OBL130.FRM) | ``fld_obl_cod_bco_acre_lostfocus`` | ``CMXsrv_comgrl_lee_nom_cor`` |
| [OBL130.FRM](./OBL130.FRM) | ``fld_obl_rut_acre_lostfocus`` | ``CMXsrv_lee_cln`` |
| [OBL130.FRM](./OBL130.FRM) | ``form_activate`` | ``CMXsrv_finobl_busc_acre`` |
| [PREFER.FRM](./PREFER.FRM) | ``Form_Load`` | ``CMXsrv_cmx_get_codes`` |

[🔝 Volver al índice](#Índice-de-Módulos-y-Procedimientos)


## PAGOS <a name="PAGOS"></a>

| Archivo | Segmento | Procedimiento Almacenado |
|---------|---------|--------------------------|
| [COL00108.FRM](./COL00108.FRM) | ``buscar_Click`` | ``CMXsrv_fincol_bsc_TIP`` |
| [COL00301.FRM](./COL00301.FRM) | ``CALCULAR_Click`` | ``CMXsrv_fincol_efec_calpa`` |
| [COL00302.FRM](./COL00302.FRM) | ``Contabilizar_Click`` | ``CMXsrv_fincol_ictb_pag`` |
| [COL00303.FRM](./COL00303.FRM) | ``Form_Activate`` | ``CMXsrv_fincol_cons_pag`` |
| [COL00304.FRM](./COL00304.FRM) | ``Form_Load`` | ``CMXsrv_fincol_cons_detp`` |
| [COL00401.FRM](./COL00401.FRM) | ``Aceptar_Click`` | ``CMXsrv_fincol_calc_pror`` |
| [COL00402.FRM](./COL00402.FRM) | ``Contabilizar_Click`` | ``CMXsrv_fincol_cont_pror`` |
| [COL00403.FRM](./COL00403.FRM) | ``Form_Activate`` | ``CMXsrv_fincol_cons_pror`` |
| [COL00404.FRM](./COL00404.FRM) | ``Form_Activate`` | ``CMXsrv_fincol_cons_dpror`` |
| [COL00501.FRM](./COL00501.FRM) | ``Aceptar_Click`` | ``CMXsrv_busc_cod_ope`` |
| [COL00501.FRM](./COL00501.FRM) | ``Aceptar_Click`` | ``CMXsrv_col_trae_num_ope`` |
| [COL00501.FRM](./COL00501.FRM) | ``Aceptar_Click`` | ``CMXsrv_fincol_cctb_anu`` |
| [COL00501.FRM](./COL00501.FRM) | ``Form_Load`` | ``CMXsrv_fincol_calc_anu`` |
| [COL00501.FRM](./COL00501.FRM) | ``Form_Load`` | ``CMXsrv_busc_cod_ope`` |
| [COL00502.FRM](./COL00502.FRM) | ``CALCULAR_Click`` | ``CMXsrv_fincol_calc_anu`` |
| [COL00502.FRM](./COL00502.FRM) | ``Form_Activate`` | ``CMXsrv_fincol_cons_anu`` |
| [COL00602.FRM](./COL00602.FRM) | ``Form_Activate`` | ``CMXsrv_fincol_cons_mod`` |
| [COL00603.FRM](./COL00603.FRM) | ``Form_Activate`` | ``CMXsrv_fincol_cons_dmod`` |
| [PREFER.FRM](./PREFER.FRM) | ``Form_Load`` | ``CMXsrv_lee_fpro`` |
| [PREFER.FRM](./PREFER.FRM) | ``Form_Load`` | ``CMXsrv_grl_trae_cod_bco`` |

[🔝 Volver al índice](#Índice-de-Módulos-y-Procedimientos)


## PGOEXT <a name="PGOEXT"></a>

| Archivo | Segmento | Procedimiento Almacenado |
|---------|---------|--------------------------|
| [PGOCOL01.FRM](./PGOCOL01.FRM) | ``calcular_Click`` | ``CMXsrv_fincol_cal_pext`` |
| [PGOCOL01.FRM](./PGOCOL01.FRM) | ``Contabilizar_Click`` | ``CMXsrv_busc_cod_ope`` |
| [PGOCOL01.FRM](./PGOCOL01.FRM) | ``Contabilizar_Click`` | ``CMXsrv_fincol_ctb_pext`` |
| [PGOOBL01.FRM](./PGOOBL01.FRM) | ``calcular_Click`` | ``CMXsrv_finobl_cal_pext`` |
| [PGOOBL01.FRM](./PGOOBL01.FRM) | ``Contabilizar_Click`` | ``CMXsrv_finobl_ctb_pext`` |
| [PREFER.FRM](./PREFER.FRM) | ``Form_Load`` | ``CMXsrv_grl_fec_serv`` |
| [PREFER.FRM](./PREFER.FRM) | ``Form_Load`` | ``CMXsrv_lee_fpro`` |

[🔝 Volver al índice](#Índice-de-Módulos-y-Procedimientos)


## ARCOS <a name="ARCOS"></a>

| Archivo | Segmento | Procedimiento Almacenado |
|---------|---------|--------------------------|
| [ARC00100.FRM](./ARC00100.FRM) | ``Eliminar_Click`` | ``CMXsrv_iarc_eli_arc`` |
| [ARC00100.FRM](./ARC00100.FRM) | ``Form_activate`` | ``CMXsrv_iarc_busc_arc`` |
| [ARC00101.FRM](./ARC00101.FRM) | ``aceptar_click`` | ``CMXsrv_iinf_busc_inf`` |
| [ARC00101.FRM](./ARC00101.FRM) | ``aceptar_click`` | ``CMXsrv_iarc_act_arc`` |
| [ARC00101.FRM](./ARC00101.FRM) | ``Form_Load`` | ``CMXsrv_iarc_lee_arc`` |
| [INFO0201.FRM](./INFO0201.FRM) | ``buscar_Click`` | ``CMXsrv_iinf_busc_opr`` |
| [INFO0201.FRM](./INFO0201.FRM) | ``Form_activate`` | ``CMXsrv_iinf_lee_vlr`` |
| [INFO0202.FRM](./INFO0202.FRM) | ``aceptar_click`` | ``CMXsrv_iarc_act_arc`` |
| [INFO0202.FRM](./INFO0202.FRM) | ``Form_activate`` | ``CMXsrv_iinf_busc_inf`` |
| [INFO0202.FRM](./INFO0202.FRM) | ``reversar_Click`` | ``CMXsrv_iinf_rev_evi`` |

[🔝 Volver al índice](#Índice-de-Módulos-y-Procedimientos)


## COBERIMP <a name="COBERIMP"></a>

| Archivo | Segmento | Procedimiento Almacenado |
|---------|---------|--------------------------|
| [COB00101.FRM](./COB00101.FRM) | ``Form_Activate`` | ``CMXsrv_icob_lee_pln`` |
| [COB00101.FRM](./COB00101.FRM) | ``Mcobcur_Click`` | ``CMXsrv_icob_cur_cob`` |
| [COB00101.FRM](./COB00101.FRM) | ``Mcobcur_Click`` | ``CMXsrv_icob_pag_sop`` |
| [COB00101.FRM](./COB00101.FRM) | ``MCOBELI_CLICK`` | ``CMXsrv_icob_eli_pln`` |
| [COB00101.FRM](./COB00101.FRM) | ``Mcobrev_Click`` | ``CMXsrv_icob_rev_etd`` |
| [COB00101.FRM](./COB00101.FRM) | ``Mcobvali_Click`` | ``CMXsrv_icob_val_cob`` |
| [COB00201.FRM](./COB00201.FRM) | ``buscar_click`` | ``CMXsrv_icob_busc_pln`` |
| [COB00201.FRM](./COB00201.FRM) | ``FLD_COB_COD_CLI_LostFocus`` | ``CMXsrv_icob_lee_cln`` |
| [COB00201.FRM](./COB00201.FRM) | ``PROXIMAS_Click`` | ``CMXsrv_icob_busc_pln`` |
| [COB00300.FRM](./COB00300.FRM) | ``ACEPTAR_Click`` | ``CMXsrv_icob_crea_norm`` |
| [COB00301.FRM](./COB00301.FRM) | ``ACEPTAR_Click`` | ``CMXsrv_icob_crea_reem`` |
| [COB00302.FRM](./COB00302.FRM) | ``ACEPTAR_Click`` | ``CMXsrv_icob_act_gral`` |
| [COB00302.FRM](./COB00302.FRM) | ``FLD_COB_COD_CLI_LostFocus`` | ``CMXsrv_icob_lee_cln2`` |
| [COB00302.FRM](./COB00302.FRM) | ``Form_Activate`` | ``CMXsrv_icob_lee_gral`` |
| [COB00303.FRM](./COB00303.FRM) | ``ACEPTAR_Click`` | ``CMXsrv_icob_act_val`` |
| [COB00303.FRM](./COB00303.FRM) | ``Form_Activate`` | ``CMXsrv_icob_lee_val`` |
| [COB00304.FRM](./COB00304.FRM) | ``ACEPTAR_Click`` | ``CMXsrv_icob_act_acu`` |
| [COB00304.FRM](./COB00304.FRM) | ``Form_Activate`` | ``CMXsrv_icob_lee_acu`` |
| [COB00304.FRM](./COB00304.FRM) | ``Form_Load`` | ``CMXsrv_icob_lee_acu`` |
| [COB00305.FRM](./COB00305.FRM) | ``ELIMINAR_Click`` | ``CMXsrv_icob_eli_int`` |
| [COB00305.FRM](./COB00305.FRM) | ``Form_Activate`` | ``CMXsrv_icob_busc_int`` |
| [COB00306.FRM](./COB00306.FRM) | ``ACEPTAR_Click`` | ``CMXsrv_icob_ingmod_int`` |
| [COB00306.FRM](./COB00306.FRM) | ``Form_Activate`` | ``CMXsrv_icob_lee_int`` |
| [COB00307.FRM](./COB00307.FRM) | ``ACEPTAR_Click`` | ``CMXsrv_icob_ing_mod_srf`` |
| [COB00307.FRM](./COB00307.FRM) | ``CmdEliminar_Click`` | ``CMXsrv_icob_eli_pln`` |
| [COB00307.FRM](./COB00307.FRM) | ``CmdReversar_Click`` | ``CMXsrv_icob_rev_etd`` |
| [COB00307.FRM](./COB00307.FRM) | ``CURSAR_Click`` | ``CMXsrv_icob_ing_mod_srf`` |
| [COB00307.FRM](./COB00307.FRM) | ``CURSAR_Click`` | ``CMXsrv_icob_pag_sop`` |
| [COB00307.FRM](./COB00307.FRM) | ``FLD_COB_COD_CLI_LostFocus`` | ``CMXsrv_icob_lee_cln2`` |
| [COB00307.FRM](./COB00307.FRM) | ``Form_Activate`` | ``CMXsrv_icob_lee_srf`` |
| [COB00307.FRM](./COB00307.FRM) | ``Reversar_Click`` | ``CMXsrv_icob_rev_etd`` |
| [COB00501.FRM](./COB00501.FRM) | ``ACEPTAR_Click`` | ``CMXsrv_icob_anu`` |
| [COB00501.FRM](./COB00501.FRM) | ``Form_Load`` | ``CMXsrv_icob_lee_anu`` |
| [COB0601.FRM](./COB0601.FRM) | ``ACEPTAR_Click`` | ``CMXsrv_icob_act_cur_a_pag`` |
| [COB0601.FRM](./COB0601.FRM) | ``buscar_click`` | ``CMXsrv_icob_bus_cur_a_pag`` |
| [COB0601.FRM](./COB0601.FRM) | ``FLD_COB_COD_CLI_LostFocus`` | ``CMXsrv_icob_lee_cln`` |
| [FORM2.FRM](./FORM2.FRM) | ``ACEPTAR_Click`` | ``CMXsrv_icob_pag_sop`` |
| [ORI_DEST.FRM](./ORI_DEST.FRM) | ``ACEPTAR_Click`` | ``CMXsrv_icob_cur_reem`` |
| [PREFER.FRM](./PREFER.FRM) | ``Form_Load`` | ``CMXsrv_grl_fec_serv`` |

[🔝 Volver al índice](#Índice-de-Módulos-y-Procedimientos)


## COBRANZA <a name="COBRANZA"></a>

| Archivo | Segmento | Procedimiento Almacenado |
|---------|---------|--------------------------|
| [CBR00101.FRM](./CBR00101.FRM) | ``ejecut_avi_imp_999`` | ``CMXsrv_busc_cor_swf`` |
| [CBR00101.FRM](./CBR00101.FRM) | ``ejecut_avi_imp_999`` | ``CMXsrv_swf_bus_sms`` |
| [CBR00101.FRM](./CBR00101.FRM) | ``Form_Activate`` | ``CMXsrv_icbr_lee_cbr`` |
| [CBR00101.FRM](./CBR00101.FRM) | ``Form_Load`` | ``CMXsrv_grl_fec_serv`` |
| [CBR00101.FRM](./CBR00101.FRM) | ``Mcbrace_Click`` | ``CMXsrv_icbr_acep_let`` |
| [CBR00101.FRM](./CBR00101.FRM) | ``Mcbrcon_Click`` | ``CMXsrv_icbr_cont_cbr`` |
| [CBR00101.FRM](./CBR00101.FRM) | ``Mcbreli_click`` | ``CMXsrv_icbr_eli_cbr`` |
| [CBR00101.FRM](./CBR00101.FRM) | ``McbrTxt999_Click`` | ``CMXsrv_icbr_lee_ctp`` |
| [CBR00101.FRM](./CBR00101.FRM) | ``Mcbrtxtrec_Click`` | ``CMXsrv_icbr_avi1`` |
| [CBR00102.FRM](./CBR00102.FRM) | ``aceptar_Click`` | ``CMXsrv_val_suc`` |
| [CBR00102.FRM](./CBR00102.FRM) | ``buscar_Click`` | ``CMXsrv_icbr_busc_cbr`` |
| [CBR00102.FRM](./CBR00102.FRM) | ``fld_aux_glo_ofi_LostFocus`` | ``CMXsrv_val_suc`` |
| [CBR00102.FRM](./CBR00102.FRM) | ``fld_cbr_cod_gdo_LostFocus`` | ``CMXsrv_icbr_lee_cln`` |
| [CBR00102.FRM](./CBR00102.FRM) | ``fld_cbr_cod_ofi_lostfocus`` | ``CMXsrv_val_suc`` |
| [CBR00102.FRM](./CBR00102.FRM) | ``proximas_Click`` | ``CMXsrv_icbr_busc_cbr`` |
| [CBR00103.FRM](./CBR00103.FRM) | ``crear_Click`` | ``CMXsrv_icbr_crea_cbr`` |
| [CBR00103.FRM](./CBR00103.FRM) | ``fld_cbr_cod_gdo_LostFocus`` | ``CMXsrv_icbr_lee_cln`` |
| [CBR00103.FRM](./CBR00103.FRM) | ``fld_cbr_cod_ofi_lostfocus`` | ``CMXsrv_val_suc`` |
| [CBR00103.FRM](./CBR00103.FRM) | ``INGRESAR_Click`` | ``CMXsrv_icbr_crea_cbr`` |
| [CBR00201.FRM](./CBR00201.FRM) | ``fld_cbr_cod_gdo_LostFocus`` | ``CMXsrv_icbr_lee_cln`` |
| [CBR00201.FRM](./CBR00201.FRM) | ``Form_Activate`` | ``CMXsrv_icbr_lee_cob`` |
| [CBR00201.FRM](./CBR00201.FRM) | ``Form_Load`` | ``CMXsrv_icbr_lee_ctp`` |
| [CBR00201.FRM](./CBR00201.FRM) | ``INGRESAR_Click`` | ``CMXsrv_icbr_act_ctp`` |
| [CBR00202.FRM](./CBR00202.FRM) | ``Form_Activate`` | ``CMXsrv_icbr_lee_cob`` |
| [CBR00202.FRM](./CBR00202.FRM) | ``Form_Load`` | ``CMXsrv_icbr_lee_trm`` |
| [CBR00202.FRM](./CBR00202.FRM) | ``INGRESAR_Click`` | ``CMXsrv_icbr_act_trm`` |
| [CBR00203.FRM](./CBR00203.FRM) | ``Form_Activate`` | ``CMXsrv_icbr_lee_cob`` |
| [CBR00203.FRM](./CBR00203.FRM) | ``Form_Load`` | ``CMXsrv_icbr_lee_doc`` |
| [CBR00203.FRM](./CBR00203.FRM) | ``INGRESAR_Click`` | ``CMXsrv_icbr_act_doc`` |
| [CBR00301.FRM](./CBR00301.FRM) | ``Form_Activate`` | ``CMXsrv_icbr_busc_let`` |
| [CBR00302.FRM](./CBR00302.FRM) | ``aceptar_Click`` | ``CMXsrv_icbr_ingmod_let`` |
| [CBR00302.FRM](./CBR00302.FRM) | ``eliminar_Click`` | ``CMXsrv_icbr_eli_let`` |
| [CBR00302.FRM](./CBR00302.FRM) | ``Form_Activate`` | ``CMXsrv_icbr_lee_let`` |
| [CBR00305.FRM](./CBR00305.FRM) | ``aceptar_Click`` | ``CMXsrv_icbr_prorr`` |
| [CBR00401.FRM](./CBR00401.FRM) | ``EFECTUAR_Click`` | ``CMXsrv_icbr_rev_eve`` |
| [CBR00401.FRM](./CBR00401.FRM) | ``Form_Activate`` | ``CMXsrv_icbr_busc_eve`` |
| [CBR00402.FRM](./CBR00402.FRM) | ``Form_Load`` | ``CMXsrv_icbr_lee_eve`` |
| [CBR00402.FRM](./CBR00402.FRM) | ``Form_Load`` | ``CMXsrv_icbr_lee_ent_doc`` |
| [CBR00701.FRM](./CBR00701.FRM) | ``aceptar_Click`` | ``CMXsrv_icbr_prot`` |
| [CBR00701.FRM](./CBR00701.FRM) | ``Form_Load`` | ``CMXsrv_icbr_pcg_prot`` |
| [CBR00801.FRM](./CBR00801.FRM) | ``aceptar_Click`` | ``CMXsrv_icbr_liq_sdo`` |
| [CBR00802.FRM](./CBR00802.FRM) | ``aceptar_Click`` | ``CMXsrv_icbr_act_vis`` |
| [CBR00802.FRM](./CBR00802.FRM) | ``eliminar_Click`` | ``CMXsrv_icbr_eli_rep`` |
| [CBR00802.FRM](./CBR00802.FRM) | ``Form_Activate`` | ``CMXsrv_icbr_busc_rep`` |
| [CBR00803.FRM](./CBR00803.FRM) | ``aceptar_Click`` | ``CMXsrv_icbr_imod_rep`` |
| [CBR00804.FRM](./CBR00804.FRM) | ``aceptar_Click`` | ``CMXsrv_icbr_ent_doc`` |
| [CBR00804.FRM](./CBR00804.FRM) | ``Form_Load`` | ``CMXsrv_icbr_lee_ent_doc`` |
| [CBR00901.FRM](./CBR00901.FRM) | ``aceptar_Click`` | ``CMXsrv_icbr_trf_ofi`` |
| [CBR00901.FRM](./CBR00901.FRM) | ``aceptar_Click`` | ``CMXsrv_val_suc`` |
| [CBR00902.FRM](./CBR00902.FRM) | ``aceptar_Click`` | ``CMXsrv_icbr_trf_bco`` |
| [COBERTU.FRM](./COBERTU.FRM) | ``aceptar_Click`` | ``CMXsrv_icbr_act_inst`` |
| [GRL00101.FRM](./GRL00101.FRM) | ``enviar_Click`` | ``CMXsrv_iswf_a_pru`` |
| [GRL00101.FRM](./GRL00101.FRM) | ``Form_Load`` | ``CMXsrv_icbr_val_cbr`` |
| [GRL00101.FRM](./GRL00101.FRM) | ``word_Click`` | ``CMXsrv_icbr_val_cbr`` |
| [GRL00101.FRM](./GRL00101.FRM) | ``word_Click`` | ``CMXsrv_iswf_a_pru`` |

[🔝 Volver al índice](#Índice-de-Módulos-y-Procedimientos)


## CRDEXT <a name="CRDEXT"></a>

| Archivo | Segmento | Procedimiento Almacenado |
|---------|---------|--------------------------|
| [BCO_BCO.FRM](./BCO_BCO.FRM) | ``Aceptar_Click`` | ``CMXsrv_icrd_a_ibab`` |
| [BCO_BCO.FRM](./BCO_BCO.FRM) | ``Form_Load`` | ``CMXsrv_icrd_lee_glo_ibab`` |
| [BCO_REM.FRM](./BCO_REM.FRM) | ``Aceptar_Click`` | ``CMXsrv_icrd_a_ibar`` |
| [BCO_REM.FRM](./BCO_REM.FRM) | ``Form_Load`` | ``CMXsrv_icrd_lee_glo_ibar`` |
| [BUSC_COD.FRM](./BUSC_COD.FRM) | ``buscar_click`` | ``CMXsrv_icrd_lee_tex_swf`` |
| [BUSC_TXT.FRM](./BUSC_TXT.FRM) | ``Aceptar_Click`` | ``CMXsrv_icrd_lee_cod_txt_swf`` |
| [BUSC_TXT.FRM](./BUSC_TXT.FRM) | ``buscar_click`` | ``CMXsrv_icrd_lee_txt_swf_all`` |
| [BUSC_TXT.FRM](./BUSC_TXT.FRM) | ``Form_Load`` | ``CMXsrv_icrd_lee_ind_esp_ing`` |
| [BUSC_TXT.FRM](./BUSC_TXT.FRM) | ``llena_arreglo`` | ``CMXsrv_icrd_lee_tex_swf`` |
| [BUSC_TXT.FRM](./BUSC_TXT.FRM) | ``proximo_Click`` | ``CMXsrv_icrd_lee_txt_swf_all`` |
| [CRD00207.FRM](./CRD00207.FRM) | ``aceptar_Click`` | ``CMXsrv_icrd_ing_acu`` |
| [CRD00207.FRM](./CRD00207.FRM) | ``Form_Load`` | ``CMXsrv_icrd_lee_acu`` |
| [CRD00701.FRM](./CRD00701.FRM) | ``aceptar_Click`` | ``CMXsrv_icrd_rech_sol`` |
| [CRD00801.FRM](./CRD00801.FRM) | ``aceptar_Click`` | ``CMXsrv_icrd_end`` |
| [CRD00801.FRM](./CRD00801.FRM) | ``Form_Load`` | ``CMXsrv_icrd_lee_dat_end`` |
| [CRD02001.FRM](./CRD02001.FRM) | ``aceptar_Click`` | ``CMXsrv_icrd_asignar_cor`` |
| [CRD02001.FRM](./CRD02001.FRM) | ``buscar_Click`` | ``CMXsrv_icrd_bus_lcr_bco`` |
| [CRD02001.FRM](./CRD02001.FRM) | ``proximo_Click`` | ``CMXsrv_icrd_bus_lcr_bco`` |
| [PREFER.FRM](./PREFER.FRM) | ``Form_Load`` | ``CMXsrv_grl_fec_serv`` |

[🔝 Volver al índice](#Índice-de-Módulos-y-Procedimientos)


## CRD_CORR <a name="CRD_CORR"></a>

| Archivo | Segmento | Procedimiento Almacenado |
|---------|---------|--------------------------|
| [COR00202.FRM](./COR00202.FRM) | ``aceptar_Click`` | ``CMXsrv_icrd_asignar_cor`` |
| [COR00202.FRM](./COR00202.FRM) | ``buscar_Click`` | ``CMXsrv_icrd_bus_lcr_bco`` |
| [COR00202.FRM](./COR00202.FRM) | ``fld_cor_cod_mtr_LostFocus`` | ``CMXsrv_icrd_lee_bco_mtr`` |
| [COR00202.FRM](./COR00202.FRM) | ``fld_cor_cod_pais_Lostfocus`` | ``CMXsrv_icrd_cor_lee_pais`` |
| [COR00202.FRM](./COR00202.FRM) | ``fld_cor_cod_plz_Lostfocus`` | ``CMXsrv_icrd_lee_plz`` |
| [COR00202.FRM](./COR00202.FRM) | ``proximo_Click`` | ``CMXsrv_icrd_bus_lcr_bco`` |
| [COR00906.FRM](./COR00906.FRM) | ``buscar_Click`` | ``CMXsrv_icrd_busc_plz`` |
| [COR00906.FRM](./COR00906.FRM) | ``proximos_Click`` | ``CMXsrv_icrd_busc_plz`` |
| [COR00907.FRM](./COR00907.FRM) | ``buscar_Click`` | ``CMXsrv_icrd_cor_busc_pais`` |
| [COR00907.FRM](./COR00907.FRM) | ``proximos_Click`` | ``CMXsrv_icrd_cor_busc_pais`` |
| [GRID_BUS.FRM](./GRID_BUS.FRM) | ``buscar_Click`` | ``CMXsrv_icrd_busc_bco_mtr`` |
| [GRID_BUS.FRM](./GRID_BUS.FRM) | ``proximos_Click`` | ``CMXsrv_icrd_busc_bco_mtr`` |

[🔝 Volver al índice](#Índice-de-Módulos-y-Procedimientos)


## DDI <a name="DDI"></a>

| Archivo | Segmento | Procedimiento Almacenado |
|---------|---------|--------------------------|
| [DDI00101.FRM](./DDI00101.FRM) | ``aceptar_Click`` | ``CMXsrv_iddi_ingmod_ddi`` |
| [DDI00101.FRM](./DDI00101.FRM) | ``continuar_Click`` | ``CMXsrv_iddi_lee_dec`` |
| [DDI00101.FRM](./DDI00101.FRM) | ``eliminar_Click`` | ``CMXsrv_iddi_eli_ddi`` |
| [DDI00101.FRM](./DDI00101.FRM) | ``fld_ddi_fec_ii_lostfocus`` | ``CMXsrv_iddi_lee_inf`` |
| [DDI00101.FRM](./DDI00101.FRM) | ``fld_ddi_rut_imp_lostfocus`` | ``CMXsrv_iddi_lee_cln`` |
| [DDI01001.FRM](./DDI01001.FRM) | ``Asociar_Click`` | ``CMXsrv_iddi_lee_rut`` |
| [DDI01001.FRM](./DDI01001.FRM) | ``Asociar_Click`` | ``CMXsrv_iddi_asoc_ddi`` |
| [DDI01001.FRM](./DDI01001.FRM) | ``Command2_Click`` | ``CMXsrv_iddi_des_ddi`` |
| [DDI01001.FRM](./DDI01001.FRM) | ``Desasociar_Click`` | ``CMXsrv_iddi_lee_rut`` |
| [DDI01001.FRM](./DDI01001.FRM) | ``Desasociar_Click`` | ``CMXsrv_iddi_des_ddi`` |
| [DDI01001.FRM](./DDI01001.FRM) | ``fld_aux_rut_cli_lostfocus`` | ``CMXsrv_iddi_lee_cln`` |
| [DDI01001.FRM](./DDI01001.FRM) | ``inicio_asoc`` | ``CMXsrv_iddi_busc_asoc`` |
| [DDI01001.FRM](./DDI01001.FRM) | ``inicio_noasoc`` | ``CMXsrv_iddi_busc_noasoc`` |
| [DDI01001.FRM](./DDI01001.FRM) | ``proximo_no_aso_Click`` | ``CMXsrv_iddi_busc_noasoc`` |

[🔝 Volver al índice](#Índice-de-Módulos-y-Procedimientos)


## IMPORT <a name="IMPORT"></a>

| Archivo | Segmento | Procedimiento Almacenado |
|---------|---------|--------------------------|
| [BUSCADIR.FRM](./BUSCADIR.FRM) | ``buscar_Click`` | ``CMXsrv_icrd_lee_dir_cln`` |
| [BUSC_COD.FRM](./BUSC_COD.FRM) | ``buscar_click`` | ``CMXsrv_icrd_lee_tex_swf`` |
| [BUSC_TXT.FRM](./BUSC_TXT.FRM) | ``Aceptar_Click`` | ``CMXsrv_icrd_lee_cod_txt_swf`` |
| [BUSC_TXT.FRM](./BUSC_TXT.FRM) | ``buscar_click`` | ``CMXsrv_icrd_lee_txt_swf_all`` |
| [BUSC_TXT.FRM](./BUSC_TXT.FRM) | ``Form_Load`` | ``CMXsrv_icrd_lee_ind_esp_ing`` |
| [BUSC_TXT.FRM](./BUSC_TXT.FRM) | ``llena_arreglo`` | ``CMXsrv_icrd_lee_tex_swf`` |
| [BUSC_TXT.FRM](./BUSC_TXT.FRM) | ``proximo_Click`` | ``CMXsrv_icrd_lee_txt_swf_all`` |
| [CONDESP.FRM](./CONDESP.FRM) | ``Aceptar_Click`` | ``CMXCRDsrv_icrd_a_cnd_esp`` |
| [CONDESP.FRM](./CONDESP.FRM) | ``Form_Load`` | ``CMXsrv_icrd_lee_cnd_esp`` |
| [CRD00101.FRM](./CRD00101.FRM) | ``clon_Click`` | ``CMXCRDsrv_icrd_clon_crd`` |
| [CRD00101.FRM](./CRD00101.FRM) | ``Form_Activate`` | ``CMXCRDsrv_icrd_lee_crdcre`` |
| [CRD00101.FRM](./CRD00101.FRM) | ``Form_Activate`` | ``CMXsrv_icrd_lee_ind_esp_ing`` |
| [CRD00101.FRM](./CRD00101.FRM) | ``Form_Activate`` | ``CMXsrv_icrd_lee_top`` |
| [CRD00101.FRM](./CRD00101.FRM) | ``Form_Load`` | ``CMXsrv_grl_fec_serv`` |
| [CRD00101.FRM](./CRD00101.FRM) | ``Form_Load`` | ``CMXsrv_cmx_get_codes`` |
| [CRD00101.FRM](./CRD00101.FRM) | ``Form_Load`` | ``CMXsrv_trae_glo_fec`` |
| [CRD00101.FRM](./CRD00101.FRM) | ``Mcrdapr_Click`` | ``CMXCRDsrv_icrd_val_crd`` |
| [CRD00101.FRM](./CRD00101.FRM) | ``Mcrdeli_click`` | ``CMXCRDsrv_icrd_eli_crd`` |
| [CRD00101.FRM](./CRD00101.FRM) | ``Mcrdtxtliq_Click`` | ``CMXsrv_icrd_lee_dat_trs`` |
| [CRD00101.FRM](./CRD00101.FRM) | ``Mcrdtxtope_Click`` | ``CMXsrv_icrd_dat_liq_ope`` |
| [CRD00101.FRM](./CRD00101.FRM) | ``msg_swift`` | ``CMXsrv_iswf_a_pru`` |
| [CRD00201.FRM](./CRD00201.FRM) | ``Aceptar_Click`` | ``CMXsrv_icrd_a_ctp`` |
| [CRD00201.FRM](./CRD00201.FRM) | ``FLD_COL_COD_CLI_LostFocus`` | ``CMXsrv_icrd_lee_cln`` |
| [CRD00201.FRM](./CRD00201.FRM) | ``Form_Load`` | ``CMXsrv_lee_fpro`` |
| [CRD00202.FRM](./CRD00202.FRM) | ``Aceptar_Click`` | ``CMXsrv_icrd_a_cnd`` |
| [CRD00202.FRM](./CRD00202.FRM) | ``Aceptar_Click`` | ``CMXCRDsrv_icrd_crea_crd`` |
| [CRD00202.FRM](./CRD00202.FRM) | ``fld_col_fec_vto_LostFocus`` | ``CMXsrv_util_det_habil`` |
| [CRD00203.FRM](./CRD00203.FRM) | ``Form_Activate`` | ``CMXsrv_icrd_busc_emb`` |
| [CRD00204.FRM](./CRD00204.FRM) | ``ELIMINAR_Click`` | ``CMXsrv_icrd_eli_emb`` |
| [CRD00204.FRM](./CRD00204.FRM) | ``Form_Load`` | ``CMXsrv_icrd_lee_emb1`` |
| [CRD00204.FRM](./CRD00204.FRM) | ``Form_Load`` | ``CMXsrv_icrd_lee_emb2`` |
| [CRD00204.FRM](./CRD00204.FRM) | ``ingresar_Click`` | ``CMXsrv_icrd_a_emb1`` |
| [CRD00204.FRM](./CRD00204.FRM) | ``ingresar_Click`` | ``CMXsrv_icrd_a_emb2`` |
| [CRD00204.FRM](./CRD00204.FRM) | ``VALIDA_EMBARQUE`` | ``CMXsrv_icrd_val_emb2`` |
| [CRD00204.FRM](./CRD00204.FRM) | ``VALIDA_EMBARQUE`` | ``CMXsrv_icrd_val_emb1`` |
| [CRD00205.FRM](./CRD00205.FRM) | ``Aceptar_Click`` | ``CMXsrv_icrd_act_ref`` |
| [CRD00205.FRM](./CRD00205.FRM) | ``Form_Load`` | ``CMXsrv_icrd_act_ref`` |
| [CRD00205.FRM](./CRD00205.FRM) | ``Form_Load`` | ``CMXsrv_icrd_lee_ref`` |
| [CRD00301.FRM](./CRD00301.FRM) | ``buscar_click`` | ``CMXCRDsrv_icrd_busc_crd`` |
| [CRD00301.FRM](./CRD00301.FRM) | ``FLD_COL_COD_CLI_LostFocus`` | ``CMXsrv_icrd_lee_cln`` |
| [CRD00301.FRM](./CRD00301.FRM) | ``PROXIMA_Click`` | ``CMXCRDsrv_icrd_busc_crd`` |
| [CRD0063.FRM](./CRD0063.FRM) | ``Aceptar_Click`` | ``CMXCRDsrv_icrd_apr_sol`` |
| [CRD0063.FRM](./CRD0063.FRM) | ``Form_Load`` | ``CMXsrv_icrd_lee_crdapr`` |
| [CRD00701.FRM](./CRD00701.FRM) | ``Aceptar_Click`` | ``CMXsrv_icrd_rech_sol`` |
| [DESCMERC.FRM](./DESCMERC.FRM) | ``Aceptar_Click`` | ``CMXCRDsrv_icrd_a_desc_merc`` |
| [DESCMERC.FRM](./DESCMERC.FRM) | ``Form_Load`` | ``CMXsrv_icrd_lee_desc_merc`` |
| [DOCUMENT.FRM](./DOCUMENT.FRM) | ``Aceptar_Click`` | ``CMXsrv_icrd_a_otr_doc`` |
| [DOCUMENT.FRM](./DOCUMENT.FRM) | ``Form_Load`` | ``CMXsrv_icrd_lee_otr_doc`` |
| [GRL00101.FRM](./GRL00101.FRM) | ``enviar_Click`` | ``CMXsrv_iswf_a_pru`` |

[🔝 Volver al índice](#Índice-de-Módulos-y-Procedimientos)


## INFORME <a name="INFORME"></a>

| Archivo | Segmento | Procedimiento Almacenado |
|---------|---------|--------------------------|
| [ARC00100.FRM](./ARC00100.FRM) | ``Eliminar_Click`` | ``CMXsrv_iarc_eli_arc`` |
| [ARC00100.FRM](./ARC00100.FRM) | ``Form_Activate`` | ``CMXsrv_iarc_busc_arc`` |
| [INFO0101.FRM](./INFO0101.FRM) | ``Form_Activate`` | ``CMXsrv_iinf_lee0_inf`` |
| [INFO0101.FRM](./INFO0101.FRM) | ``Form_Activate`` | ``CMXsrv_iinf_lee_tablas`` |
| [INFO0101.FRM](./INFO0101.FRM) | ``Form_Activate`` | ``CMXsrv_iinf_lee1_inf`` |
| [INFO0101.FRM](./INFO0101.FRM) | ``Form_Activate`` | ``CMXsrv_iinf_lee_cln`` |
| [INFO0101.FRM](./INFO0101.FRM) | ``Form_Activate`` | ``CMXsrv_iinf_lee2_inf`` |
| [INFO0101.FRM](./INFO0101.FRM) | ``Form_Activate`` | ``CMXsrv_iinf_avi_miscb`` |
| [INFO0101.FRM](./INFO0101.FRM) | ``Maviapr_Click`` | ``CMXsrv_iinf_avi_misca`` |
| [INFO0101.FRM](./INFO0101.FRM) | ``Maviapr_Click`` | ``CMXsrv_iinf_avi_miscb`` |
| [INFO0101.FRM](./INFO0101.FRM) | ``Mavicom_Click`` | ``CMXsrv_iinf_avi_misca`` |
| [INFO0101.FRM](./INFO0101.FRM) | ``Mavicom_Click`` | ``CMXsrv_iinf_avi_miscb`` |
| [INFO0101.FRM](./INFO0101.FRM) | ``Mavicom_Click`` | ``CMXsrv_icrd_lee_dat_com`` |
| [INFO0101.FRM](./INFO0101.FRM) | ``Mavimis1_Click`` | ``CMXsrv_iinf_avi_misca`` |
| [INFO0101.FRM](./INFO0101.FRM) | ``Mavimis1_Click`` | ``CMXsrv_iinf_avi_miscb`` |
| [INFO0101.FRM](./INFO0101.FRM) | ``Mavimis2_Click`` | ``CMXsrv_iinf_avi_misca`` |
| [INFO0101.FRM](./INFO0101.FRM) | ``Mavimis2_Click`` | ``CMXsrv_iinf_avi_miscb`` |
| [INFO0101.FRM](./INFO0101.FRM) | ``Mavirec_Click`` | ``CMXsrv_iinf_avi_misca`` |
| [INFO0101.FRM](./INFO0101.FRM) | ``Mavirec_Click`` | ``CMXsrv_iinf_avi_miscb`` |
| [INFO0101.FRM](./INFO0101.FRM) | ``Mavitib_Click`` | ``CMXsrv_iinf_avi_misca`` |
| [INFO0101.FRM](./INFO0101.FRM) | ``Mavitib_Click`` | ``CMXsrv_iinf_avi_miscb`` |
| [INFO0101.FRM](./INFO0101.FRM) | ``Mavitras_Click`` | ``CMXsrv_iinf_avi_misca`` |
| [INFO0101.FRM](./INFO0101.FRM) | ``Mavitras_Click`` | ``CMXsrv_iinf_avi_miscb`` |
| [INFO0101.FRM](./INFO0101.FRM) | ``Mavitras_Click`` | ``CMXsrv_icrd_lee_dat_trs`` |
| [INFO0101.FRM](./INFO0101.FRM) | ``Minfoeli_click`` | ``CMXsrv_iinf_eli_inf`` |
| [INFO0101.FRM](./INFO0101.FRM) | ``Minforev_Click`` | ``CMXsrv_iinf_busc_evi`` |
| [INFO0101.FRM](./INFO0101.FRM) | ``Minfoval_click`` | ``CMXsrv_iinf_val_inf`` |
| [INFO0102.FRM](./INFO0102.FRM) | ``Aceptar_Click`` | ``CMXsrv_iinf_ingmod_inf`` |
| [INFO0102.FRM](./INFO0102.FRM) | ``Fec_pre`` | ``CMXsrv_iinf_lee_fec`` |
| [INFO0102.FRM](./INFO0102.FRM) | ``fld_aux_glo_cls_com_LostFocus`` | ``CMXsrv_iinf_lee_tablas`` |
| [INFO0102.FRM](./INFO0102.FRM) | ``fld_aux_glo_for_pag1_LostFocus`` | ``CMXsrv_iinf_lee_tablas`` |
| [INFO0102.FRM](./INFO0102.FRM) | ``fld_aux_glo_for_pag2_LostFocus`` | ``CMXsrv_iinf_lee_tablas`` |
| [INFO0102.FRM](./INFO0102.FRM) | ``fld_aux_glo_for_pag3_LostFocus`` | ``CMXsrv_iinf_lee_tablas`` |
| [INFO0102.FRM](./INFO0102.FRM) | ``fld_aux_glo_mon_LostFocus`` | ``CMXsrv_iinf_lee_tablas`` |
| [INFO0102.FRM](./INFO0102.FRM) | ``fld_inf_cls_com_Lostfocus`` | ``CMXsrv_iinf_lee_tablas`` |
| [INFO0102.FRM](./INFO0102.FRM) | ``fld_inf_cod_imp_LostFocus`` | ``CMXsrv_iinf_lee_cln`` |
| [INFO0102.FRM](./INFO0102.FRM) | ``fld_inf_for_pag1_lostfocus`` | ``CMXsrv_iinf_lee_tablas`` |
| [INFO0102.FRM](./INFO0102.FRM) | ``fld_inf_for_pag2_LostFocus`` | ``CMXsrv_iinf_lee_tablas`` |
| [INFO0102.FRM](./INFO0102.FRM) | ``fld_inf_for_pag3_LostFocus`` | ``CMXsrv_iinf_lee_tablas`` |
| [INFO0102.FRM](./INFO0102.FRM) | ``fld_inf_mon_inf_lostfocus`` | ``CMXsrv_iinf_lee_tablas`` |
| [INFO0102.FRM](./INFO0102.FRM) | ``Form_Load`` | ``CMXsrv_iinf_lee0_inf`` |
| [INFO0102.FRM](./INFO0102.FRM) | ``Form_Load`` | ``CMXsrv_iinf_lee1_inf`` |
| [INFO0102.FRM](./INFO0102.FRM) | ``Form_Load`` | ``CMXsrv_iinf_lee2_inf`` |
| [INFO0102.FRM](./INFO0102.FRM) | ``valor_usd`` | ``CMXsrv_iinf_lee_usd`` |
| [INFO0103.FRM](./INFO0103.FRM) | ``Aceptar_Click`` | ``CMXsrv_iinf_busc_inf`` |
| [INFO0103.FRM](./INFO0103.FRM) | ``buscar_Click`` | ``CMXsrv_iinf_busc_inf`` |
| [INFO0103.FRM](./INFO0103.FRM) | ``Fec_pre`` | ``CMXsrv_iinf_lee_fec`` |
| [INFO0103.FRM](./INFO0103.FRM) | ``fld_inf_cod_imp_LostFocus`` | ``CMXsrv_iinf_lee_cln`` |
| [INFO0103.FRM](./INFO0103.FRM) | ``PROXIMA_Click`` | ``CMXsrv_iinf_busc_inf`` |
| [INFO0104.FRM](./INFO0104.FRM) | ``Aceptar_Click`` | ``CMXsrv_iinf_act_apr`` |
| [INFO0105.FRM](./INFO0105.FRM) | ``Form_Activate`` | ``CMXsrv_iinf_busc_evi`` |
| [INFO0105.FRM](./INFO0105.FRM) | ``reversar_Click`` | ``CMXsrv_iinf_rev_evi`` |
| [INFO0106.FRM](./INFO0106.FRM) | ``Form_Load`` | ``CMXsrv_iinf_lee_evi`` |
| [INFO0107.FRM](./INFO0107.FRM) | ``Aceptar_Click`` | ``CMXsrv_iinf_act_tib`` |
| [INFO0108.FRM](./INFO0108.FRM) | ``Aceptar_Click`` | ``CMXsrv_iinf_act_rec`` |
| [INFO0109.FRM](./INFO0109.FRM) | ``Aceptar_Click`` | ``CMXsrv_iinf_act_rib`` |
| [INFO0110.FRM](./INFO0110.FRM) | ``Form_Activate`` | ``CMXsrv_iinf_busc_comp`` |
| [INFO0110.FRM](./INFO0110.FRM) | ``proximos_Click`` | ``CMXsrv_iinf_busc_comp`` |
| [INFO0111.FRM](./INFO0111.FRM) | ``Aceptar_Click`` | ``CMXsrv_iinf_ingmod_comp`` |
| [INFO0111.FRM](./INFO0111.FRM) | ``Fec_pre`` | ``CMXsrv_iinf_lee_fec`` |
| [INFO0111.FRM](./INFO0111.FRM) | ``Form_Activate`` | ``CMXsrv_iinf_lee_comp`` |
| [INFO0111.FRM](./INFO0111.FRM) | ``Form_Activate`` | ``CMXsrv_iinf_lee_tablas`` |
| [INFO0112.FRM](./INFO0112.FRM) | ``aceptar_click`` | ``CMXsrv_iinf_lee_bco`` |
| [INFO0112.FRM](./INFO0112.FRM) | ``buscar_Click`` | ``CMXsrv_iinf_busc_bco`` |
| [PREFER.FRM](./PREFER.FRM) | ``Form_Load`` | ``CMXsrv_grl_fec_serv`` |

[🔝 Volver al índice](#Índice-de-Módulos-y-Procedimientos)


## MOD_ADI <a name="MOD_ADI"></a>

| Archivo | Segmento | Procedimiento Almacenado |
|---------|---------|--------------------------|
| [CRD00202.FRM](./CRD00202.FRM) | ``Aceptar_Click`` | ``CMXsrv_icrd_a_cnd`` |
| [CRD00202.FRM](./CRD00202.FRM) | ``busca_bco`` | ``CMXsrv_icrd_lee_bco_swf`` |
| [CRD00202.FRM](./CRD00202.FRM) | ``fld_col_fec_vto_LostFocus`` | ``CMXsrv_util_det_habil`` |
| [CRD00202.FRM](./CRD00202.FRM) | ``Form_Load`` | ``CMXMCRDsrv_icrd_lee_mcnd`` |
| [PREFER.FRM](./PREFER.FRM) | ``Form_Load`` | ``CMXsrv_grl_fec_serv`` |

[🔝 Volver al índice](#Índice-de-Módulos-y-Procedimientos)


## MOD_CBR <a name="MOD_CBR"></a>

| Archivo | Segmento | Procedimiento Almacenado |
|---------|---------|--------------------------|
| [CBR00201.FRM](./CBR00201.FRM) | ``fld_cbr_cod_gdo_LostFocus`` | ``CMXsrv_icbr_lee_cln`` |
| [CBR00201.FRM](./CBR00201.FRM) | ``Form_Load`` | ``CMXsrv_icbr_lee_ctp`` |
| [CBR00201.FRM](./CBR00201.FRM) | ``INGRESAR_Click`` | ``CMXsrv_icbr_act_ctp`` |
| [CBR00202.FRM](./CBR00202.FRM) | ``Form_Load`` | ``CMXsrv_icbr_lee_trm`` |
| [CBR00202.FRM](./CBR00202.FRM) | ``INGRESAR_Click`` | ``CMXsrv_icbr_act_trm`` |
| [CBR00203.FRM](./CBR00203.FRM) | ``Form_Load`` | ``CMXsrv_icbr_lee_doc`` |
| [CBR00203.FRM](./CBR00203.FRM) | ``INGRESAR_Click`` | ``CMXsrv_icbr_act_doc`` |
| [CBR00301.FRM](./CBR00301.FRM) | ``Form_Activate`` | ``CMXsrv_icbr_busc_let`` |
| [CBR00302.FRM](./CBR00302.FRM) | ``aceptar_Click`` | ``CMXsrv_icbr_mod_ing_let`` |
| [CBR00302.FRM](./CBR00302.FRM) | ``eliminar_Click`` | ``CMXsrv_icbr_eli_let`` |
| [CBR00302.FRM](./CBR00302.FRM) | ``Form_Activate`` | ``CMXsrv_icbr_lee_let`` |
| [PANBASE.FRM](./PANBASE.FRM) | ``actualizar_Click`` | ``CMXsrv_icbr_acep_mod_cbr`` |
| [PANBASE.FRM](./PANBASE.FRM) | ``Cancelar_Click`` | ``CMXsrv_icbr_eli_no_cont`` |

[🔝 Volver al índice](#Índice-de-Módulos-y-Procedimientos)


## MOD_CRD <a name="MOD_CRD"></a>

| Archivo | Segmento | Procedimiento Almacenado |
|---------|---------|--------------------------|
| [BCO_BCO.FRM](./BCO_BCO.FRM) | ``Aceptar_Click`` | ``CMXsrv_icrd_a_ibab`` |
| [BCO_BCO.FRM](./BCO_BCO.FRM) | ``Form_Load`` | ``CMXsrv_icrd_lee_glo_ibab`` |
| [BCO_REM.FRM](./BCO_REM.FRM) | ``Aceptar_Click`` | ``CMXsrv_icrd_a_ibar`` |
| [BCO_REM.FRM](./BCO_REM.FRM) | ``Form_Load`` | ``CMXsrv_icrd_lee_glo_ibar`` |
| [BUSCADIR.FRM](./BUSCADIR.FRM) | ``buscar_click`` | ``CMXsrv_icrd_lee_dir_cln`` |
| [BUSCA_TE.FRM](./BUSCA_TE.FRM) | ``buscar_Click`` | ``CMXsrv_icrd_lee_tex_swf`` |
| [BUSC_COD.FRM](./BUSC_COD.FRM) | ``buscar_click`` | ``CMXsrv_icrd_lee_tex_swf`` |
| [BUSC_TXT.FRM](./BUSC_TXT.FRM) | ``Aceptar_Click`` | ``CMXsrv_icrd_lee_cod_txt_swf`` |
| [BUSC_TXT.FRM](./BUSC_TXT.FRM) | ``buscar_click`` | ``CMXsrv_icrd_lee_txt_swf_all`` |
| [BUSC_TXT.FRM](./BUSC_TXT.FRM) | ``Form_Load`` | ``CMXsrv_icrd_lee_ind_esp_ing`` |
| [BUSC_TXT.FRM](./BUSC_TXT.FRM) | ``llena_arreglo`` | ``CMXsrv_icrd_lee_tex_swf`` |
| [BUSC_TXT.FRM](./BUSC_TXT.FRM) | ``proximo_Click`` | ``CMXsrv_icrd_lee_txt_swf_all`` |
| [CONDESP.FRM](./CONDESP.FRM) | ``Aceptar_Click`` | ``CMXMCRDsrv_icrd_a_mmcnd`` |
| [CONDESP.FRM](./CONDESP.FRM) | ``Form_Load`` | ``CMXsrv_icrd_lee_cnd_esp`` |
| [CRD00201.FRM](./CRD00201.FRM) | ``Aceptar_Click`` | ``CMXsrv_icrd_a_ctp`` |
| [CRD00201.FRM](./CRD00201.FRM) | ``FLD_COL_COD_CLI_LostFocus`` | ``CMXsrv_icrd_lee_cln`` |
| [CRD00201.FRM](./CRD00201.FRM) | ``Form_Load`` | ``CMXMCRDsrv_icrd_lee_mctp`` |
| [CRD00202.FRM](./CRD00202.FRM) | ``Aceptar_Click`` | ``CMXsrv_icrd_a_cnd`` |
| [CRD00202.FRM](./CRD00202.FRM) | ``Form_Load`` | ``CMXMCRDsrv_icrd_lee_mcnd`` |
| [CRD00203.FRM](./CRD00203.FRM) | ``Form_Activate`` | ``CMXsrv_icrd_busc_emb`` |
| [CRD00204.FRM](./CRD00204.FRM) | ``cancelar_Click`` | ``CMXsrv_icrd_lee_desc_merc`` |
| [CRD00204.FRM](./CRD00204.FRM) | ``ELIMINAR_Click`` | ``CMXsrv_icrd_eli_emb`` |
| [CRD00204.FRM](./CRD00204.FRM) | ``Form_Load`` | ``CMXMCRDsrv_icrd_lee_memb2`` |
| [CRD00204.FRM](./CRD00204.FRM) | ``Form_Load`` | ``CMXMCRDsrv_icrd_lee_memb1`` |
| [CRD00204.FRM](./CRD00204.FRM) | ``ingresar_Click`` | ``CMXsrv_icrd_a_emb1`` |
| [CRD00204.FRM](./CRD00204.FRM) | ``ingresar_Click`` | ``CMXsrv_icrd_a_emb2`` |
| [CRD00204.FRM](./CRD00204.FRM) | ``VALIDA_EMBARQUE`` | ``CMXsrv_icrd_val_emb2`` |
| [CRD00204.FRM](./CRD00204.FRM) | ``VALIDA_EMBARQUE`` | ``CMXsrv_icrd_val_emb1`` |
| [CRD00205.FRM](./CRD00205.FRM) | ``Aceptar_Click`` | ``CMXsrv_icrd_act_ref`` |
| [CRD00205.FRM](./CRD00205.FRM) | ``fld_obl_cod_bco_acre_DblClick`` | ``CMXsrv_icrd_lee_bco_swf`` |
| [CRD00205.FRM](./CRD00205.FRM) | ``fld_obl_cod_bco_acre_LostFocus`` | ``CMXsrv_icrd_lee_bco_swf`` |
| [CRD00205.FRM](./CRD00205.FRM) | ``Form_Load`` | ``CMXMCRDsrv_icrd_lee_mref`` |
| [CRD00206.FRM](./CRD00206.FRM) | ``Aceptar_Click`` | ``CMXsrv_icrd_ing_txt`` |
| [CRD00206.FRM](./CRD00206.FRM) | ``Form_Load`` | ``CMXCRDsrv_icrd_get_ing_esp`` |
| [CRD00206.FRM](./CRD00206.FRM) | ``Form_Load`` | ``CMXMCRDsrv_icrd_lee_mtxt`` |
| [CRD00207.FRM](./CRD00207.FRM) | ``Form_Load`` | ``CMXCRDsrv_icrd_get_pre_fra`` |
| [DESCMERC.FRM](./DESCMERC.FRM) | ``Aceptar_Click`` | ``CMXMCRDsrv_icrd_a_mmer`` |
| [DESCMERC.FRM](./DESCMERC.FRM) | ``Form_Load`` | ``CMXsrv_icrd_lee_desc_merc`` |
| [DOCUME.FRM](./DOCUME.FRM) | ``Aceptar_Click`` | ``CMXsrv_icrd_a_otr_doc`` |
| [DOCUME.FRM](./DOCUME.FRM) | ``Form_Load`` | ``CMXsrv_icrd_lee_otr_doc`` |
| [MOD00603.FRM](./MOD00603.FRM) | ``Aceptar_Click`` | ``CMXsrv_fincol_lee_cod_eve`` |
| [MOD00603.FRM](./MOD00603.FRM) | ``Aceptar_Click`` | ``CMXMCRDsrv_icrd_acep_mod_crd`` |
| [MOD00603.FRM](./MOD00603.FRM) | ``cancelar_Click`` | ``CMXMCRDsrv_icrd_eli_no_cont`` |
| [MOD00603.FRM](./MOD00603.FRM) | ``fld_crd_cod_bco_rem_LostFocus`` | ``CMXsrv_icrd_lee_bco_swf`` |
| [MOD00603.FRM](./MOD00603.FRM) | ``fld_crd_fec_mod_lostFocus`` | ``CMXsrv_fincol_efec_calpa`` |
| [MOD00603.FRM](./MOD00603.FRM) | ``Form_Activate`` | ``CMXsrv_icrd_lee_ind_esp_ing`` |
| [MOD00603.FRM](./MOD00603.FRM) | ``Form_Load`` | ``CMXsrv_fincol_efec_calpa`` |
| [MOD00603.FRM](./MOD00603.FRM) | ``Form_Load`` | ``CMXMCRDsrv_icrd_lee_mcnd`` |
| [PREFER.FRM](./PREFER.FRM) | ``Form_Load`` | ``CMXsrv_grl_fec_serv`` |

[🔝 Volver al índice](#Índice-de-Módulos-y-Procedimientos)


## NEGO_AV <a name="NEGO_AV"></a>

| Archivo | Segmento | Procedimiento Almacenado |
|---------|---------|--------------------------|
| [AVISOS.FRM](./AVISOS.FRM) | ``aviso1`` | ``CMXsrv_icrd_a_rec_age`` |
| [AVISOS.FRM](./AVISOS.FRM) | ``aviso1`` | ``CMXsrv_busc_ofi_cta`` |
| [AVISOS.FRM](./AVISOS.FRM) | ``aviso1`` | ``CMXsrv_neg_busc_arc`` |
| [AVISOS.FRM](./AVISOS.FRM) | ``aviso1`` | ``CMXsrv_icrd_lee_avi_adi`` |
| [AVISOS.FRM](./AVISOS.FRM) | ``aviso3`` | ``CMXsrv_icrd_lee_dat_trs`` |
| [AVISOS.FRM](./AVISOS.FRM) | ``Aviso4`` | ``CMXsrv_icrd_dat_liq_ope`` |
| [AVISOS.FRM](./AVISOS.FRM) | ``Aviso4`` | ``CMXsrv_icrd_lee_dat_cln`` |
| [AVISOS.FRM](./AVISOS.FRM) | ``Aviso5`` | ``CMXsrv_icrd_lee_dat_cln`` |
| [AVISOS.FRM](./AVISOS.FRM) | ``Aviso5`` | ``CMXsrv_icrd_lee_avi_dis`` |
| [AVISOS.FRM](./AVISOS.FRM) | ``Aviso5`` | ``CMXsrv_icrd_lee_avi_adi`` |
| [AVISOS.FRM](./AVISOS.FRM) | ``Aviso5`` | ``CMXsrv_neg_ddi_asoc`` |
| [AVISOS.FRM](./AVISOS.FRM) | ``Aviso5`` | ``CMXsrv_neg_busc_arc`` |
| [AVISOS.FRM](./AVISOS.FRM) | ``Aviso5`` | ``CMXsrv_neg_trae_vcto_mcf`` |
| [AVISOS.FRM](./AVISOS.FRM) | ``Aviso6`` | ``CMXsrv_icrd_avs_cyg1`` |
| [AVISOS.FRM](./AVISOS.FRM) | ``Aviso6`` | ``CMXsrv_icrd_avs_cyg2`` |
| [AVISOS.FRM](./AVISOS.FRM) | ``lee_aval`` | ``CMXsrv_neg_avi_lee_aval`` |
| [AVISOS.FRM](./AVISOS.FRM) | ``lee_nego`` | ``CMXsrv_icrd_neg_lee_crd`` |
| [AVISOS.FRM](./AVISOS.FRM) | ``lee_nego`` | ``CMXsrv_icrd_lee_neg`` |
| [AVI_COL.FRM](./AVI_COL.FRM) | ``avi_col1`` | ``CMXsrv_col_avi_dat_cln`` |
| [AVI_COL.FRM](./AVI_COL.FRM) | ``avi_col1`` | ``CMXsrv_col_avi_det_pag`` |
| [AVI_COL.FRM](./AVI_COL.FRM) | ``avi_col2`` | ``CMXsrv_col_avi_dat_cln`` |
| [AVI_COL.FRM](./AVI_COL.FRM) | ``avi_col2`` | ``CMXsrv_col_avi_det_oto`` |
| [AVI_COL.FRM](./AVI_COL.FRM) | ``avi_col4`` | ``CMXsrv_col_avi_dat_cln`` |
| [AVI_COL.FRM](./AVI_COL.FRM) | ``avi_col4`` | ``CMXsrv_col_lee_num_trs`` |
| [AVI_COL.FRM](./AVI_COL.FRM) | ``lee_obl_oto`` | ``CMXsrv_finobl_avi_oto`` |
| [AVI_COL.FRM](./AVI_COL.FRM) | ``lee_obl_pag`` | ``CMXsrv_finobl_avi_pag`` |
| [AVI_COL.FRM](./AVI_COL.FRM) | ``traspaso`` | ``CMXsrv_neg_avi_trae_asnd_mn`` |
| [AVI_COL.FRM](./AVI_COL.FRM) | ``traspaso`` | ``CMXsrv_neg_avi_trae_asnd_mx`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``Form_Activate`` | ``CMXsrv_icrd_neg_lee_crd`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``Form_Activate`` | ``CMXsrv_icrd_lee_neg`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``Mcrdtxtliq_Click`` | ``CMXsrv_icrd_lee_dat_trs`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``Mcrdtxtope_Click`` | ``CMXsrv_icrd_dat_liq_ope`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``Mnegavi3_Click`` | ``CMXsrv_icrd_avs_cyg1`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``Mnegavi3_Click`` | ``CMXsrv_icrd_avs_cyg2`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``Mnegavi4_Click`` | ``CMXsrv_icrd_lee_dat_liq`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``MNEGCONT_Click`` | ``CMXsrv_icrd_cont_neg`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``MNEGELI_CLICK`` | ``CMXsrv_icrd_eli_neg`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``precarga_datos`` | ``CMXsrv_icrd_a_rec_age`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``precarga_datos`` | ``CMXsrv_busc_ofi_cta`` |
| [PREFER.FRM](./PREFER.FRM) | ``Form_Load`` | ``CMXsrv_trae_glo_fec`` |
| [PREFER.FRM](./PREFER.FRM) | ``Form_Load`` | ``CMXsrv_icrd_lee_num_col`` |
| [VER_PAGO.FRM](./VER_PAGO.FRM) | ``Form_Load`` | ``CMXsrv_icrd_bus_pago`` |

[🔝 Volver al índice](#Índice-de-Módulos-y-Procedimientos)


## NNEGO <a name="NNEGO"></a>

| Archivo | Segmento | Procedimiento Almacenado |
|---------|---------|--------------------------|
| [Copy of CRD02004.FRM](./Copy of CRD02004.FRM) | ``ACEPTAR_Click`` | ``CMXsrv_icrd_act_doc_neg`` |
| [Copy of CRD02004.FRM](./Copy of CRD02004.FRM) | ``Form_Load`` | ``CMXsrv_icrd_lee_doc_neg`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``Form_Activate`` | ``CMXsrv_icrd_neg_lee_crd`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``Form_Activate`` | ``CMXsrv_icrd_lee_neg`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``gen_mens_swift`` | ``CMXsrv_iswf_a_pru`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``llama_pagos`` | ``CMXsrv_icrd_lee_col`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``Mnegavi9_Click`` | ``CMXsrv_iswf_a_pru`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``MNEGCONT_Click`` | ``CMXsrv_icrd_cont_neg`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``MNEGELI_CLICK`` | ``CMXsrv_icrd_eli_neg`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``pertas_Click`` | ``CMXsrv_icrd_lee_col`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``prueba_Click`` | ``CMX2srv_neg_avi_dat_cln`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``prueba_Click`` | ``CMX2srv_neg_avi_det_int`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``prueba_Click`` | ``CMX2srv_neg_avi_trae_asnd_mn`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``prueba_Click`` | ``CMX2srv_neg_avi_trae_asnd_mx`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``prueba_pag_Click`` | ``CMX2srv_neg_avi_dat_cln`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``prueba_pag_Click`` | ``CMX2srv_neg_avi_det_pag`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``prueba_pag_Click`` | ``CMX2srv_neg_avi_trae_asnd_mn`` |
| [CRD01001.FRM](./CRD01001.FRM) | ``prueba_pag_Click`` | ``CMX2srv_neg_avi_trae_asnd_mx`` |
| [CRD01002.FRM](./CRD01002.FRM) | ``Form_Activate`` | ``CMXsrv_icrd_busc_neg`` |
| [CRD01003.FRM](./CRD01003.FRM) | ``Form_Load`` | ``CMXsrv_icrd_busc_emb`` |
| [CRD01005.FRM](./CRD01005.FRM) | ``ACEPTAR_Click`` | ``CMXsrv_icrd_a_neg_emb1`` |
| [CRD01005.FRM](./CRD01005.FRM) | ``ACEPTAR_Click`` | ``CMXsrv_icrd_a_neg_emb2`` |
| [CRD01005.FRM](./CRD01005.FRM) | ``CANCELAR_Click`` | ``CMXsrv_icrd_eli_doc_neg`` |
| [CRD01005.FRM](./CRD01005.FRM) | ``Form_Activate`` | ``CMXsrv_icrd_lee_emb1`` |
| [CRD01005.FRM](./CRD01005.FRM) | ``Form_Activate`` | ``CMXsrv_icrd_lee_emb2`` |
| [CRD01005.FRM](./CRD01005.FRM) | ``Form_Activate`` | ``CMXsrv_icrd_lee_neg_emb1`` |
| [CRD01005.FRM](./CRD01005.FRM) | ``Form_Activate`` | ``CMXsrv_icrd_lee_neg_emb2`` |
| [CRD01005.FRM](./CRD01005.FRM) | ``Form_Activate`` | ``CMXsrv_icrd_lee_cnd_esp`` |
| [CRD01005.FRM](./CRD01005.FRM) | ``Form_Activate`` | ``CMXsrv_icrd_lee_desc_merc`` |
| [CRD01006.FRM](./CRD01006.FRM) | ``ACEPTAR_Click`` | ``CMXsrv_icrd_a_neg_disc`` |
| [CRD01006.FRM](./CRD01006.FRM) | ``Form_Load`` | ``CMXsrv_icrd_neg_lee_disc`` |
| [CRD01201.FRM](./CRD01201.FRM) | ``ACEPTAR_Click`` | ``CMXsrv_icrd_ent_doc`` |
| [CRD01201.FRM](./CRD01201.FRM) | ``ELIMINAR_Click`` | ``CMXsrv_icrd_ent_doc`` |
| [CRD01201.FRM](./CRD01201.FRM) | ``Form_Load`` | ``CMXsrv_icrd_ent_doc`` |
| [CRD01301.FRM](./CRD01301.FRM) | ``ACEPTAR_Click`` | ``MIGRCMXsrv_neg_grb_ind_com_disc`` |
| [CRD01301.FRM](./CRD01301.FRM) | ``ACEPTAR_Click`` | ``CMXsrv_con_convenio_banco`` |
| [CRD01301.FRM](./CRD01301.FRM) | ``ACEPTAR_Click`` | ``CMXsrv_icrd_alz_disc`` |
| [CRD02001.FRM](./CRD02001.FRM) | ``aceptar_click`` | ``CMXCRDsrv_icrd_asignar_cor`` |
| [CRD02001.FRM](./CRD02001.FRM) | ``BUSCAR_Click`` | ``CMXCRDsrv_icrd_bus_lcr_bco`` |
| [CRD02001.FRM](./CRD02001.FRM) | ``proximo_Click`` | ``CMXCRDsrv_icrd_bus_lcr_bco`` |
| [CRD02004.FRM](./CRD02004.FRM) | ``ACEPTAR_Click`` | ``CMXsrv_icrd_act_doc_neg`` |
| [CRD02004.FRM](./CRD02004.FRM) | ``Form_Load`` | ``CMXsrv_icrd_lee_doc_neg`` |
| [GRL00101.FRM](./GRL00101.FRM) | ``enviar_Click`` | ``CMXsrv_iswf_a_pru`` |
| [GRL00101.FRM](./GRL00101.FRM) | ``Form_Load`` | ``CMXsrv_icrd_val_neg`` |
| [PREFER.FRM](./PREFER.FRM) | ``Form_Load`` | ``CMXsrv_grl_fec_serv`` |
| [VER_PAGO.FRM](./VER_PAGO.FRM) | ``Form_Load`` | ``CMXsrv_icrd_bus_pago`` |

[🔝 Volver al índice](#Índice-de-Módulos-y-Procedimientos)


## PAGCBR <a name="PAGCBR"></a>

| Archivo | Segmento | Procedimiento Almacenado |
|---------|---------|--------------------------|
| [CBR01005.FRM](./CBR01005.FRM) | ``Aceptar_Click`` | ``CMXsrv_icbr_calc_pag`` |
| [CBR01006.FRM](./CBR01006.FRM) | ``ACEPTAR_Click`` | ``CMXsrv_icbr_lee_dat_var`` |
| [CBR01006.FRM](./CBR01006.FRM) | ``ACEPTAR_Click`` | ``CMXsrv_icbr_val_pag`` |
| [CBR01006.FRM](./CBR01006.FRM) | ``ACEPTAR_Click`` | ``CMXsrv_icbr_ctb_pag`` |
| [CBR01006.FRM](./CBR01006.FRM) | ``Calcular_Click`` | ``CMXsrv_icbr_cal_pag`` |
| [CBR01006.FRM](./CBR01006.FRM) | ``CANCELAR_Click`` | ``CMXsrv_icbr_eli_pag`` |
| [CBR01006.FRM](./CBR01006.FRM) | ``fld_cbr_cod_des_mn_pag_lostfocus`` | ``CMXsrv_val_vig`` |
| [CBR01006.FRM](./CBR01006.FRM) | ``fld_cbr_cod_des_mx_pag_lostfocus`` | ``CMXsrv_val_vig`` |
| [CBR01006.FRM](./CBR01006.FRM) | ``Form_Load`` | ``CMXsrv_icbr_lee_cbr0`` |
| [CBR01006.FRM](./CBR01006.FRM) | ``Form_Load`` | ``CMXsrv_icbr_obt_mon_nac`` |
| [CBR01006.FRM](./CBR01006.FRM) | ``Form_Load`` | ``CMXsrv_icbr_lee_dat_pag`` |
| [CBR01006.FRM](./CBR01006.FRM) | ``Form_Load`` | ``CMXsrv_icbr_pcg_pag`` |
| [CBR01006.FRM](./CBR01006.FRM) | ``lee_cta`` | ``CMXsrv_vig_lee_cta`` |
| [CBR01007.FRM](./CBR01007.FRM) | ``Form_Activate`` | ``CMXsrv_icbr_busc_pago`` |
| [CBR01008.FRM](./CBR01008.FRM) | ``ACEPTAR_Click`` | ``CMXsrv_icbr_val_pag`` |
| [COB00303.FRM](./COB00303.FRM) | ``Aceptar_Click`` | ``CMXsrv_icob_act_val`` |
| [COB00303.FRM](./COB00303.FRM) | ``Form_Activate`` | ``CMXsrv_icob_lee_val`` |
| [COB00305.FRM](./COB00305.FRM) | ``ELIMINAR_Click`` | ``CMXsrv_icbr_eli_int_pago`` |
| [COB00305.FRM](./COB00305.FRM) | ``Form_Activate`` | ``CMXsrv_icbr_busc_int`` |
| [COB00306.FRM](./COB00306.FRM) | ``Aceptar_Click`` | ``CMXsrv_icbr_ingmod_int`` |
| [COB00306.FRM](./COB00306.FRM) | ``Form_Activate`` | ``CMXsrv_icbr_lee_int_pago`` |
| [CRD00602.FRM](./CRD00602.FRM) | ``Aceptar_Click`` | ``CMXsrv_icbr_lee_bco`` |
| [CRD00602.FRM](./CRD00602.FRM) | ``buscar_Click`` | ``CMXsrv_icbr_busc_bco`` |
| [PREFER.FRM](./PREFER.FRM) | ``Form_Load`` | ``CMXsrv_grl_fec_serv`` |

[🔝 Volver al índice](#Índice-de-Módulos-y-Procedimientos)

