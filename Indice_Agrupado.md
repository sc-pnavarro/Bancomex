# Índice de Productos y Módulos

## Productos y Módulos

- **Exportaciones**
  - [EXPCBE](#expcbe)
  - [EXPCCE](#expcce)
  - [expdex](#expdex)
  - [EXPNEG](#expneg)
  - [expret](#expret)

- **Financiamiento**
  - [ADMIN](#admin)
  - [COL_NEG](#col_neg)
  - [INGRESO](#ingreso)
  - [MODIFIC](#modific)
  - [OBLIGA](#obliga)
  - [PAGOS](#pagos)
  - [PGOEXT](#pgoext)

- **Importaciones**
  - [ARCOS](#arcos)

---

## Detalles de Módulos

### EXPCBE
**Archivos:**
- CBE00101.FRM
- CBE00201.FRM
- CBE00202.FRM

**Segmentos:**
- Form_Activate
- Form_Load
- ingcomg_Click

**Procedimientos Almacenados:**
- CMXsrv_expcbe_lee_prm
- CMXsrv_cmx_busc_suc_usu
- CMXsrv_expcbe_lee_cbe

### EXPCCE
**Archivos:**
- CCE00101.FRM
- CCE00201.FRM

**Segmentos:**
- Form_Activate
- MCCEANL_CLICK
- Mccectb_click

**Procedimientos Almacenados:**
- CMXsrv_expcce_lee_cce
- CMXsrv_expcce_trd_cce
- CMXsrv_expcce_anl_cce

### expdex
**Archivos:**
- DEX00101.FRM
- DEX00102.FRM

**Segmentos:**
- form_activate
- Mdexeli_Click
- ACEPTAR_Click

**Procedimientos Almacenados:**
- CMXsrv_expcbe_lee_prm
- CMXsrv_dex_lee_dex
- CMXsrv_dex_eli_dex

### EXPNEG
**Archivos:**
- CCE00601.FRM
- CCE00801.FRM

**Segmentos:**
- Form_Activate
- Mccealznge_click
- Mcceanlnge_click

**Procedimientos Almacenados:**
- CMXsrv_expcce_lee_bas
- CMXsrv_expcce_lee_neg
- CMXsrv_expcce_alz_dis

### expret
**Archivos:**
- RET00101.FRM
- RET00201.FRM

**Segmentos:**
- Form_Activate
- M_cgyc_Click
- mvalid_Click

**Procedimientos Almacenados:**
- CMXsrv_expret_lee_ret
- CMXsrv_expret_avs_cyg1
- CMXsrv_expret_val_ret

### ADMIN
**Archivos:**
- ADM00201.FRM
- ADM00202.FRM

**Segmentos:**
- COMMAND4_Click
- Form_Load
- Command1_Click

**Procedimientos Almacenados:**
- CMXsrv_finadm_imod_desti
- CMXsrv_finadm_cons_dtip
- CMXsrv_finadm_imod_ectb

### COL_NEG
**Archivos:**
- COL00102.FRM
- COL00103.FRM

**Segmentos:**
- CANCELAR_Click
- Form_Activate
- ingresar_Click

**Procedimientos Almacenados:**
- CMXsrv_busc_tip_tas
- CMXsrv_fincol_ecuo
- CMXsrv_fincol_cons_plnpa

### INGRESO
**Archivos:**
- COL00104.FRM
- COL00701.FRM

**Segmentos:**
- aceptar_Click
- FLD_COL_COD_CLI_LOSTFOCUS
- Form_Activate

**Procedimientos Almacenados:**
- CMXsrv_fincol_gmod_ctr
- CMXsrv_icrd_lee_bco_swf
- CMXsrv_fincol_lee_cln

### MODIFIC
**Archivos:**
- COL00303.FRM
- COL00901.FRM

**Segmentos:**
- Form_Activate
- EFECTUAR_Click

**Procedimientos Almacenados:**
- CMXsrv_fincol_cons_tas
- CMXsrv_fincol_rev_eve

### OBLIGA
**Archivos:**
- OBL00103.FRM
- OBL00104.FRM

**Segmentos:**
- anunctb_Click
- buscar_Click

**Procedimientos Almacenados:**
- CMXsrv_finobl_calc_anu
- CMXsrv_finobl_bsc_obl

### PAGOS
**Archivos:**
- COL00301.FRM
- COL00501.FRM

**Segmentos:**
- CALCULAR_Click
- Aceptar_Click

**Procedimientos Almacenados:**
- CMXsrv_fincol_efec_calpa
- CMXsrv_busc_cod_ope

### PGOEXT
**Archivos:**
- PGOCOL01.FRM
- PGOOBL01.FRM

**Segmentos:**
- calcular_Click
- Contabilizar_Click

**Procedimientos Almacenados:**
- CMXsrv_fincol_cal_pext
- CMXsrv_fincol_ctb_pext

### ARCOS
**Archivos:**
- ARC00100.FRM
- ARC00101.FRM

**Segmentos:**
- Eliminar_Click
- aceptar_click

**Procedimientos Almacenados:**
- CMXsrv_iarc_eli_arc
- CMXsrv_iinf_busc_inf
