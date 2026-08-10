import React, { useState, useMemo } from "react";

/* ============================================================
   ESTILOS COMPARTIDOS
   ============================================================ */
const GlobalStyles = () => (
  <style>{`
    @import url('https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&family=IBM+Plex+Sans:wght@400;500;600&family=IBM+Plex+Mono:wght@400;500;600&display=swap');
    * { box-sizing: border-box; }
    .eyebrow {
      font-family: 'IBM Plex Mono', monospace;
      font-size: 11px;
      letter-spacing: 0.14em;
      text-transform: uppercase;
      color: #6B7A72;
    }
    .num { font-family: 'IBM Plex Mono', monospace; font-variant-numeric: tabular-nums; }
    .chip {
      cursor: pointer;
      border: 1px solid #D8D5CB;
      background: #FFFFFF;
      border-radius: 999px;
      padding: 7px 14px;
      font-size: 12.5px;
      font-weight: 500;
      color: #4A544E;
      white-space: nowrap;
      transition: all 0.15s ease;
    }
    .chip:hover { border-color: #1C2321; }
    .chip.active { background: #1C2321; color: #F5F4F0; border-color: #1C2321; }
    .row:hover { background: #EFEEE8; }
    .card-row:hover { background: #EFEEE8; }
    input[type="text"], input[type="number"], select { font-family: 'IBM Plex Sans', sans-serif; }
    .chips-scroll::-webkit-scrollbar { height: 0px; }
    .tab-btn {
      cursor: pointer;
      padding: 10px 18px;
      border-radius: 10px;
      font-size: 14px;
      font-weight: 600;
      color: #6B7A72;
      background: transparent;
      border: none;
      font-family: 'IBM Plex Sans', sans-serif;
      transition: all 0.15s ease;
      white-space: nowrap;
    }
    .tab-btn:hover { color: #1C2321; }
    .tab-btn.active { background: #1C2321; color: #F5F4F0; }
    @media (max-width: 640px) {
      .grid-cols-resp { grid-template-columns: 1fr !important; }
    }
  `}</style>
);

/* ============================================================
   MÓDULO 1 — EQUIVALENCIAS DE CORTICOIDES
   ============================================================ */
const CORTICOIDES = [
  { id: "hidrocortisona", nombre: "Hidrocortisona", equivalenciaMg: 20, potenciaGC: 1, mineralocorticoide: 1, duracionHoras: "8–12 h" },
  { id: "cortisona", nombre: "Cortisona", equivalenciaMg: 25, potenciaGC: 0.8, mineralocorticoide: 0.8, duracionHoras: "8–12 h" },
  { id: "prednisona", nombre: "Prednisona", equivalenciaMg: 5, potenciaGC: 4, mineralocorticoide: 0.25, duracionHoras: "18–36 h" },
  { id: "prednisolona", nombre: "Prednisolona", equivalenciaMg: 5, potenciaGC: 4, mineralocorticoide: 0.25, duracionHoras: "18–36 h" },
  { id: "metilprednisolona", nombre: "Metilprednisolona", equivalenciaMg: 4, potenciaGC: 5, mineralocorticoide: 0, duracionHoras: "18–36 h" },
  { id: "triamcinolona", nombre: "Triamcinolona", equivalenciaMg: 4, potenciaGC: 5, mineralocorticoide: 0, duracionHoras: "18–36 h" },
  { id: "deflazacort", nombre: "Deflazacort", equivalenciaMg: 6, potenciaGC: 3.3, mineralocorticoide: 0, duracionHoras: "18–36 h" },
  { id: "dexametasona", nombre: "Dexametasona", equivalenciaMg: 0.75, potenciaGC: 25, mineralocorticoide: 0, duracionHoras: "36–54 h" },
  { id: "betametasona", nombre: "Betametasona", equivalenciaMg: 0.6, potenciaGC: 30, mineralocorticoide: 0, duracionHoras: "36–54 h" },
];

const DURACION_COLOR = { "8–12 h": "#3F7D6E", "18–36 h": "#B4841F", "36–54 h": "#A2483A" };

function CorticoidesTab() {
  const [origenId, setOrigenId] = useState("prednisona");
  const [dosis, setDosis] = useState(10);
  const origen = CORTICOIDES.find((c) => c.id === origenId);

  const resultados = useMemo(() => {
    const dosisNum = parseFloat(dosis) || 0;
    const factor = dosisNum / origen.equivalenciaMg;
    return CORTICOIDES.map((c) => ({ ...c, dosisEquivalente: factor * c.equivalenciaMg }));
  }, [origenId, dosis, origen]);

  const maxPotencia = Math.max(...CORTICOIDES.map((c) => c.potenciaGC));

  return (
    <div>
      <div style={{ background: "#1C2321", borderRadius: "14px", padding: "28px", marginBottom: "28px", display: "grid", gridTemplateColumns: "1fr 1fr", gap: "24px" }} className="grid-cols-resp">
        <div>
          <label className="eyebrow" style={{ color: "#9BA89F", display: "block", marginBottom: "10px" }}>Corticoide de partida</label>
          <select value={origenId} onChange={(e) => setOrigenId(e.target.value)} style={{ width: "100%", background: "#2A322E", color: "#F5F4F0", border: "1px solid #3D4A43", borderRadius: "8px", padding: "12px 14px", fontSize: "15px", fontWeight: 500 }}>
            {CORTICOIDES.map((c) => <option key={c.id} value={c.id}>{c.nombre}</option>)}
          </select>
        </div>
        <div>
          <label className="eyebrow" style={{ color: "#9BA89F", display: "block", marginBottom: "10px" }}>Dosis (mg/día)</label>
          <input type="number" min="0" step="0.25" value={dosis} onChange={(e) => setDosis(e.target.value)} style={{ width: "100%", background: "#2A322E", color: "#F5F4F0", border: "1px solid #3D4A43", borderRadius: "8px", padding: "12px 14px", fontSize: "15px", fontWeight: 500 }} />
        </div>
      </div>

      <div style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "14px", overflow: "hidden", marginBottom: "28px" }}>
        <div style={{ display: "grid", gridTemplateColumns: "1.6fr 1fr 1fr 1.3fr", padding: "12px 20px", borderBottom: "1px solid #E4E1D6", background: "#FAF9F5" }}>
          <div className="eyebrow">Corticoide</div>
          <div className="eyebrow">Dosis equiv.</div>
          <div className="eyebrow">Potencia GC</div>
          <div className="eyebrow">Mineralocort. / Duración</div>
        </div>
        {resultados.map((c) => {
          const esOrigen = c.id === origenId;
          return (
            <div key={c.id} className="card-row" style={{ display: "grid", gridTemplateColumns: "1.6fr 1fr 1fr 1.3fr", padding: "16px 20px", alignItems: "center", borderBottom: "1px solid #F0EEE6", background: esOrigen ? "#F0EEE3" : "transparent" }}>
              <div style={{ fontWeight: 600, fontSize: "14.5px", display: "flex", alignItems: "center", gap: "8px" }}>
                {c.nombre}
                {esOrigen && <span className="eyebrow" style={{ background: "#1C2321", color: "#F5F4F0", borderRadius: "4px", padding: "2px 6px", fontSize: "9px" }}>base</span>}
              </div>
              <div className="num" style={{ fontSize: "16px", fontWeight: 600 }}>{c.dosisEquivalente.toFixed(2).replace(/\.00$/, "")} mg</div>
              <div className="num" style={{ fontSize: "14px", color: "#4A544E" }}>×{c.potenciaGC}</div>
              <div style={{ display: "flex", alignItems: "center", gap: "10px" }}>
                <span className="num" style={{ fontSize: "13px", color: "#4A544E" }}>MC {c.mineralocorticoide}</span>
                <span style={{ fontSize: "11px", fontWeight: 600, color: DURACION_COLOR[c.duracionHoras], background: DURACION_COLOR[c.duracionHoras] + "1A", borderRadius: "4px", padding: "2px 7px", whiteSpace: "nowrap" }}>{c.duracionHoras}</span>
              </div>
            </div>
          );
        })}
      </div>

      <div style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "14px", padding: "26px 24px 22px", marginBottom: "28px" }}>
        <div className="eyebrow" style={{ marginBottom: "18px" }}>Escala de potencia glucocorticoide relativa (hidrocortisona = 1)</div>
        <div style={{ position: "relative", height: "64px" }}>
          <div style={{ position: "absolute", top: "32px", left: 0, right: 0, height: "2px", background: "#E4E1D6" }} />
          {CORTICOIDES.map((c) => {
            const pct = (c.potenciaGC / maxPotencia) * 100;
            const esOrigen = c.id === origenId;
            return (
              <div key={c.id} style={{ position: "absolute", left: `${pct}%`, top: 0, transform: "translateX(-50%)", display: "flex", flexDirection: "column", alignItems: "center", width: "84px" }}>
                <div className="num" style={{ fontSize: "10px", color: esOrigen ? "#1C2321" : "#8A9089", fontWeight: esOrigen ? 700 : 500, marginBottom: "4px" }}>×{c.potenciaGC}</div>
                <div style={{ width: esOrigen ? "12px" : "8px", height: esOrigen ? "12px" : "8px", borderRadius: "50%", background: esOrigen ? "#A2483A" : "#1C2321", border: "2px solid #FFFFFF", boxShadow: "0 0 0 1px " + (esOrigen ? "#A2483A" : "#1C2321"), marginTop: esOrigen ? "-1px" : "1px" }} />
                <div style={{ fontSize: "10.5px", color: esOrigen ? "#1C2321" : "#6B7A72", fontWeight: esOrigen ? 700 : 500, marginTop: "6px", textAlign: "center", lineHeight: 1.2 }}>{c.nombre}</div>
              </div>
            );
          })}
        </div>
      </div>

      <Disclaimer texto='Las equivalencias son aproximadas y de valor docente; no contemplan variabilidad interindividual, vía de administración, insuficiencia hepática/renal ni interacciones. Actividad mineralocorticoide (MC) expresada en relación a hidrocortisona = 1. Confirmar siempre con criterio clínico y guías institucionales vigentes antes de indicar un cambio de corticoide.' />
    </div>
  );
}

/* ============================================================
   MÓDULO 2 — VALORES DE REFERENCIA HORMONALES
   ============================================================ */
const EJES = [
  { id: "tiroideo", nombre: "Eje tiroideo", color: "#3F7D6E", items: [
    { det: "TSH", valor: "0.4 – 4.0", unidad: "mUI/L", obs: "Adultos, sin patología conocida" },
    { det: "T4 libre", valor: "0.8 – 1.8", unidad: "ng/dL", obs: "" },
    { det: "T4 total", valor: "5.0 – 12.0", unidad: "µg/dL", obs: "" },
    { det: "T3 libre", valor: "2.3 – 4.2", unidad: "pg/mL", obs: "" },
    { det: "T3 total", valor: "80 – 200", unidad: "ng/dL", obs: "" },
    { det: "Anti-TPO", valor: "< 35", unidad: "UI/mL", obs: "Cutoff variable según método" },
    { det: "Anti-tiroglobulina", valor: "< 40", unidad: "UI/mL", obs: "Cutoff variable según método" },
    { det: "Tiroglobulina", valor: "< 55", unidad: "ng/mL", obs: "Objetivo < 1 ng/mL post-tiroidectomía total" },
    { det: "TRAb / TSI", valor: "< 1.75", unidad: "UI/L", obs: "Cutoff variable según kit" },
  ]},
  { id: "suprarrenal", nombre: "Eje suprarrenal", color: "#A2483A", items: [
    { det: "Cortisol matutino (8h)", valor: "5 – 25", unidad: "µg/dL", obs: "" },
    { det: "Cortisol vespertino (20h)", valor: "2 – 9", unidad: "µg/dL", obs: "Ritmo circadiano conservado" },
    { det: "Cortisol libre urinario 24h", valor: "10 – 100", unidad: "µg/24h", obs: "Muy variable según método" },
    { det: "ACTH matutina", valor: "7.2 – 63", unidad: "pg/mL", obs: "" },
    { det: "Aldosterona (decúbito)", valor: "3 – 16", unidad: "ng/dL", obs: "4–31 ng/dL de pie" },
    { det: "Actividad de renina plasmática", valor: "0.5 – 3.3", unidad: "ng/mL/h", obs: "Decúbito; aumenta de pie" },
    { det: "Relación aldosterona/renina", valor: "< 20 – 30", unidad: "—", obs: "Cutoff según unidades del laboratorio" },
    { det: "DHEA-S (mujer)", valor: "35 – 430", unidad: "µg/dL", obs: "Premenopáusica; disminuye con edad" },
    { det: "DHEA-S (hombre)", valor: "80 – 560", unidad: "µg/dL", obs: "Disminuye con edad" },
    { det: "17-OH-progesterona", valor: "< 200", unidad: "ng/dL", obs: "Fase folicular" },
    { det: "Metanefrina libre plasmática", valor: "< 0.5", unidad: "nmol/L", obs: "" },
    { det: "Normetanefrina libre plasmática", valor: "< 0.9", unidad: "nmol/L", obs: "" },
    { det: "Catecolaminas urinarias 24h", valor: "Adr < 20 / NA < 100", unidad: "µg/24h", obs: "" },
  ]},
  { id: "gonadal-f", nombre: "Eje gonadal — mujer", color: "#B4841F", items: [
    { det: "LH", valor: "2–12 (F) · 15–70 (ovul.) · 1–12 (L) · 15–60 (post-menop.)", unidad: "UI/L", obs: "Según fase del ciclo" },
    { det: "FSH", valor: "3–10 (F) · 6–20 (ovul.) · 1–9 (L) · 20–140 (post-menop.)", unidad: "UI/L", obs: "Según fase del ciclo" },
    { det: "Estradiol", valor: "20–150 (F) · 150–750 (ovul.) · 30–450 (L) · <30 (post-menop.)", unidad: "pg/mL", obs: "Según fase del ciclo" },
    { det: "Progesterona", valor: "< 1.5 (folicular) · 2–25 (lútea)", unidad: "ng/mL", obs: "" },
    { det: "Testosterona total", valor: "15 – 70", unidad: "ng/dL", obs: "" },
    { det: "Testosterona libre", valor: "0.1 – 6.4", unidad: "pg/mL", obs: "Muy variable según método" },
    { det: "SHBG", valor: "20 – 130", unidad: "nmol/L", obs: "" },
    { det: "AMH", valor: "1.0 – 4.0", unidad: "ng/mL", obs: "Orientativo; disminuye con edad" },
    { det: "Prolactina", valor: "4.8 – 23.3", unidad: "ng/mL", obs: "No gestante" },
  ]},
  { id: "gonadal-m", nombre: "Eje gonadal — hombre", color: "#B4841F", items: [
    { det: "LH", valor: "1.7 – 8.6", unidad: "UI/L", obs: "" },
    { det: "FSH", valor: "1.5 – 12.4", unidad: "UI/L", obs: "" },
    { det: "Testosterona total", valor: "300 – 1000", unidad: "ng/dL", obs: "Medir 7–10 h, ayuno" },
    { det: "Testosterona libre", valor: "50 – 210", unidad: "pg/mL", obs: "Muy variable según método" },
    { det: "SHBG", valor: "10 – 57", unidad: "nmol/L", obs: "" },
    { det: "Estradiol", valor: "10 – 40", unidad: "pg/mL", obs: "" },
    { det: "Prolactina", valor: "4 – 15.2", unidad: "ng/mL", obs: "" },
    { det: "Inhibina B", valor: "80 – 300", unidad: "pg/mL", obs: "Marcador de espermatogénesis" },
  ]},
  { id: "somatotrofo", nombre: "Eje somatotrofo", color: "#4A6FA5", items: [
    { det: "GH basal", valor: "< 5", unidad: "ng/mL", obs: "Secreción pulsátil, poco valor aislado" },
    { det: "GH nadir post-SOG", valor: "< 0.4", unidad: "ng/mL", obs: "Criterio actual para descartar acromegalia" },
    { det: "IGF-1", valor: "Según edad y sexo", unidad: "ng/mL", obs: "Usar tabla específica del laboratorio por edad" },
  ]},
  { id: "fosfocalcico", nombre: "Metabolismo fosfocálcico", color: "#6B5B95", items: [
    { det: "PTH intacta", valor: "15 – 65", unidad: "pg/mL", obs: "" },
    { det: "Calcio total", valor: "8.5 – 10.5", unidad: "mg/dL", obs: "Corregir por albúmina" },
    { det: "Calcio iónico", valor: "1.12 – 1.32", unidad: "mmol/L", obs: "" },
    { det: "Fósforo", valor: "2.5 – 4.5", unidad: "mg/dL", obs: "" },
    { det: "25-OH vitamina D", valor: "Suf. >30 · Insuf. 20–29 · Déf. <20", unidad: "ng/mL", obs: "" },
    { det: "1,25-(OH)₂ vitamina D", valor: "18 – 72", unidad: "pg/mL", obs: "Calcitriol" },
    { det: "Calcitonina", valor: "< 8.4 (H) · < 5 (M)", unidad: "pg/mL", obs: "" },
    { det: "Magnesio", valor: "1.7 – 2.4", unidad: "mg/dL", obs: "" },
  ]},
  { id: "metabolico", nombre: "Metabolismo glucídico", color: "#3F7D6E", items: [
    { det: "Glucemia en ayunas", valor: "70 – 100", unidad: "mg/dL", obs: "" },
    { det: "Insulina basal", valor: "2.6 – 24.9", unidad: "µUI/mL", obs: "Ayuno" },
    { det: "Péptido C", valor: "0.9 – 7.1", unidad: "ng/mL", obs: "Ayuno" },
    { det: "HbA1c", valor: "< 5.7 normal · 5.7–6.4 prediabetes · ≥ 6.5 diabetes", unidad: "%", obs: "" },
    { det: "HOMA-IR", valor: "< 2.5", unidad: "—", obs: "Orientativo, punto de corte variable" },
  ]},
];

function ValoresReferenciaTab() {
  const [busqueda, setBusqueda] = useState("");
  const [ejeActivo, setEjeActivo] = useState("todos");

  const ejesFiltrados = useMemo(() => {
    const q = busqueda.trim().toLowerCase();
    return EJES.map((eje) => ({
      ...eje,
      items: eje.items.filter((it) => {
        const matchEje = ejeActivo === "todos" || eje.id === ejeActivo;
        const matchQuery = q === "" || it.det.toLowerCase().includes(q);
        return matchEje && matchQuery;
      }),
    })).filter((eje) => eje.items.length > 0);
  }, [busqueda, ejeActivo]);

  return (
    <div>
      <input type="text" placeholder="Buscar determinación (ej: TSH, cortisol, testosterona...)" value={busqueda} onChange={(e) => setBusqueda(e.target.value)} style={{ width: "100%", padding: "13px 16px", borderRadius: "10px", border: "1px solid #D8D5CB", background: "#FFFFFF", fontSize: "14.5px", marginBottom: "16px", outline: "none" }} />

      <div className="chips-scroll" style={{ display: "flex", gap: "8px", overflowX: "auto", marginBottom: "28px", paddingBottom: "2px" }}>
        <div className={`chip ${ejeActivo === "todos" ? "active" : ""}`} onClick={() => setEjeActivo("todos")}>Todos los ejes</div>
        {EJES.map((eje) => (
          <div key={eje.id} className={`chip ${ejeActivo === eje.id ? "active" : ""}`} onClick={() => setEjeActivo(eje.id)}>{eje.nombre}</div>
        ))}
      </div>

      {ejesFiltrados.length === 0 && <div style={{ color: "#6B7A72", fontSize: "14px", padding: "24px 0" }}>No se encontraron determinaciones para "{busqueda}".</div>}

      {ejesFiltrados.map((eje) => (
        <div key={eje.id} style={{ marginBottom: "22px" }}>
          <div style={{ display: "flex", alignItems: "center", gap: "8px", marginBottom: "10px" }}>
            <div style={{ width: "8px", height: "8px", borderRadius: "50%", background: eje.color }} />
            <div style={{ fontFamily: "'Space Grotesk', sans-serif", fontWeight: 600, fontSize: "16px" }}>{eje.nombre}</div>
          </div>
          <div style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "12px", overflow: "hidden" }}>
            <div style={{ display: "grid", gridTemplateColumns: "1.3fr 1.6fr 0.8fr 1.3fr", padding: "10px 18px", background: "#FAF9F5", borderBottom: "1px solid #E4E1D6" }}>
              <div className="eyebrow">Determinación</div>
              <div className="eyebrow">Valor de referencia</div>
              <div className="eyebrow">Unidad</div>
              <div className="eyebrow">Observaciones</div>
            </div>
            {eje.items.map((it, i) => (
              <div key={i} className="row" style={{ display: "grid", gridTemplateColumns: "1.3fr 1.6fr 0.8fr 1.3fr", padding: "13px 18px", borderBottom: i === eje.items.length - 1 ? "none" : "1px solid #F0EEE6", alignItems: "center", fontSize: "13.5px" }}>
                <div style={{ fontWeight: 600 }}>{it.det}</div>
                <div className="num" style={{ fontWeight: 600 }}>{it.valor}</div>
                <div className="num" style={{ color: "#4A544E" }}>{it.unidad}</div>
                <div style={{ color: "#6B7A72", fontSize: "12.5px" }}>{it.obs}</div>
              </div>
            ))}
          </div>
        </div>
      ))}

      <Disclaimer texto="Los rangos de referencia hormonales dependen fuertemente del método analítico, el kit y la población de cada laboratorio — especialmente en testosterona libre, cortisol urinario, aldosterona y catecolaminas. Estos valores son orientativos para adultos fuera de embarazo, compilados de literatura internacional estándar (no existe una tabla única oficial de FBA o SAEM); siempre priorizar el rango informado por el laboratorio que procesó la muestra y ajustar por edad, sexo, fase del ciclo y condición clínica." />
    </div>
  );
}

/* ============================================================
   MÓDULO 3 — CONVERSOR DE UNIDADES HORMONALES
   ============================================================ */
// factor: multiplicar valor convencional × factor = valor SI
const CONVERSIONES = [
  { id: "cortisol", nombre: "Cortisol", unidConv: "µg/dL", unidSI: "nmol/L", factor: 27.59 },
  { id: "t4libre", nombre: "T4 libre", unidConv: "ng/dL", unidSI: "pmol/L", factor: 12.87 },
  { id: "t4total", nombre: "T4 total", unidConv: "µg/dL", unidSI: "nmol/L", factor: 12.87 },
  { id: "t3libre", nombre: "T3 libre", unidConv: "pg/mL", unidSI: "pmol/L", factor: 1.536 },
  { id: "t3total", nombre: "T3 total", unidConv: "ng/dL", unidSI: "nmol/L", factor: 0.01536 },
  { id: "testosterona", nombre: "Testosterona total", unidConv: "ng/dL", unidSI: "nmol/L", factor: 0.03467 },
  { id: "estradiol", nombre: "Estradiol", unidConv: "pg/mL", unidSI: "pmol/L", factor: 3.671 },
  { id: "progesterona", nombre: "Progesterona", unidConv: "ng/mL", unidSI: "nmol/L", factor: 3.18 },
  { id: "dheas", nombre: "DHEA-S", unidConv: "µg/dL", unidSI: "µmol/L", factor: 0.02714 },
  { id: "aldosterona", nombre: "Aldosterona", unidConv: "ng/dL", unidSI: "pmol/L", factor: 27.74 },
  { id: "acth", nombre: "ACTH", unidConv: "pg/mL", unidSI: "pmol/L", factor: 0.2202 },
  { id: "insulina", nombre: "Insulina", unidConv: "µUI/mL", unidSI: "pmol/L", factor: 6.945, nota: "Factor aproximado; puede variar levemente según el estándar de calibración del ensayo." },
  { id: "igf1", nombre: "IGF-1", unidConv: "ng/mL", unidSI: "nmol/L", factor: 0.1307 },
  { id: "pth", nombre: "PTH intacta", unidConv: "pg/mL", unidSI: "pmol/L", factor: 0.106 },
  { id: "vitd", nombre: "25-OH vitamina D", unidConv: "ng/mL", unidSI: "nmol/L", factor: 2.496 },
  { id: "calcio", nombre: "Calcio total", unidConv: "mg/dL", unidSI: "mmol/L", factor: 0.2495 },
  { id: "fosforo", nombre: "Fósforo", unidConv: "mg/dL", unidSI: "mmol/L", factor: 0.3229 },
  { id: "magnesio", nombre: "Magnesio", unidConv: "mg/dL", unidSI: "mmol/L", factor: 0.4114 },
  { id: "glucosa", nombre: "Glucosa", unidConv: "mg/dL", unidSI: "mmol/L", factor: 0.0555 },
  { id: "prolactina", nombre: "Prolactina", unidConv: "ng/mL", unidSI: "mIU/L", factor: 21.2, nota: "Factor de conversión aproximado; varía según el estándar de calibración de cada inmunoensayo — confirmar con el laboratorio." },
  { id: "reninaActividad", nombre: "Renina — actividad (ARP)", unidConv: "ng/mL/h", unidSI: "ng/(L·s)", factor: 0.2778, nota: "Conversión de unidades de tiempo/volumen (exacta); no depende del método de ensayo." },
  { id: "reninaConcentracion", nombre: "Renina — concentración directa", unidConv: "pg/mL", unidSI: "mUI/L", factor: 1.15, nota: "Factor aproximado; la equivalencia pg/mL–mUI/L depende del estándar de calibración del ensayo (quimioluminiscencia vs. RIA) — confirmar con el laboratorio." },
];

function ConversorTab() {
  const [hormonaId, setHormonaId] = useState("cortisol");
  const [valorConv, setValorConv] = useState("20");
  const [ultimoEditado, setUltimoEditado] = useState("conv"); // "conv" | "si"

  const hormona = CONVERSIONES.find((h) => h.id === hormonaId);

  const valorSI = useMemo(() => {
    const n = parseFloat(valorConv);
    if (isNaN(n)) return "";
    return (n * hormona.factor);
  }, [valorConv, hormona]);

  const handleHormonaChange = (id) => {
    setHormonaId(id);
    setValorConv("");
  };

  const handleConvChange = (v) => {
    setValorConv(v);
    setUltimoEditado("conv");
  };

  const handleSIChange = (v) => {
    const n = parseFloat(v);
    if (isNaN(n)) {
      setValorConv("");
    } else {
      setValorConv((n / hormona.factor).toString());
    }
    setUltimoEditado("si");
  };

  const displaySI = ultimoEditado === "si" ? undefined : (valorSI === "" ? "" : Number(valorSI.toFixed(4)).toString());

  return (
    <div>
      <div style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "14px", padding: "24px", marginBottom: "20px" }}>
        <label className="eyebrow" style={{ display: "block", marginBottom: "10px" }}>Determinación</label>
        <select value={hormonaId} onChange={(e) => handleHormonaChange(e.target.value)} style={{ width: "100%", background: "#FAF9F5", color: "#1C2321", border: "1px solid #D8D5CB", borderRadius: "8px", padding: "12px 14px", fontSize: "15px", fontWeight: 500 }}>
          {CONVERSIONES.map((h) => <option key={h.id} value={h.id}>{h.nombre}</option>)}
        </select>
      </div>

      <div style={{ display: "grid", gridTemplateColumns: "1fr auto 1fr", gap: "16px", alignItems: "center", marginBottom: "20px" }} className="grid-cols-resp">
        <div style={{ background: "#1C2321", borderRadius: "14px", padding: "22px" }}>
          <div className="eyebrow" style={{ color: "#9BA89F", marginBottom: "10px" }}>Unidad convencional</div>
          <div style={{ display: "flex", alignItems: "baseline", gap: "8px" }}>
            <input
              type="number"
              value={ultimoEditado === "si" ? Number(valorConv === "" ? "" : Number(valorConv).toFixed(4)) : valorConv}
              onChange={(e) => handleConvChange(e.target.value)}
              placeholder="0"
              style={{ width: "100%", background: "#2A322E", color: "#F5F4F0", border: "1px solid #3D4A43", borderRadius: "8px", padding: "12px 14px", fontSize: "20px", fontWeight: 600 }}
              className="num"
            />
            <span className="num" style={{ color: "#9BA89F", fontSize: "14px", whiteSpace: "nowrap" }}>{hormona.unidConv}</span>
          </div>
        </div>

        <div style={{ display: "flex", justifyContent: "center", color: "#8A9089", fontSize: "20px" }}>⇌</div>

        <div style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "14px", padding: "22px" }}>
          <div className="eyebrow" style={{ marginBottom: "10px" }}>Unidad SI</div>
          <div style={{ display: "flex", alignItems: "baseline", gap: "8px" }}>
            <input
              type="number"
              value={displaySI !== undefined ? displaySI : valorConv === "" ? "" : Number((parseFloat(valorConv) * hormona.factor).toFixed(4))}
              onChange={(e) => handleSIChange(e.target.value)}
              placeholder="0"
              style={{ width: "100%", background: "#FAF9F5", color: "#1C2321", border: "1px solid #D8D5CB", borderRadius: "8px", padding: "12px 14px", fontSize: "20px", fontWeight: 600 }}
              className="num"
            />
            <span className="num" style={{ color: "#6B7A72", fontSize: "14px", whiteSpace: "nowrap" }}>{hormona.unidSI}</span>
          </div>
        </div>
      </div>

      <div style={{ background: "#FAF9F5", border: "1px solid #E4E1D6", borderRadius: "10px", padding: "14px 18px", marginBottom: "20px", fontSize: "13px", color: "#4A544E" }}>
        <span className="eyebrow" style={{ marginRight: "8px" }}>Factor</span>
        1 {hormona.unidConv} = <span className="num" style={{ fontWeight: 600 }}>{hormona.factor}</span> {hormona.unidSI}
        {hormona.nota && <div style={{ marginTop: "6px", color: "#A2483A" }}>⚠ {hormona.nota}</div>}
      </div>

      <Disclaimer texto="Los factores de conversión están basados en el peso molecular de cada analito y son válidos para la mayoría de los inmunoensayos estándar. En hormonas medidas por bioensayo o con calibración específica (insulina, prolactina), el factor puede variar levemente según el kit — confirmar con el laboratorio ante resultados límite." />
    </div>
  );
}

/* ============================================================
   MÓDULO 4 — ALGORITMOS TERAPÉUTICOS
   ============================================================ */
const ALGORITMOS = [
  {
    id: "tiroides-funcional",
    nombre: "Hipo / hipertiroidismo",
    color: "#3F7D6E",
    fuentes: ["ATA Guidelines", "SAEM — Dpto. de Tiroides", "Endocrine Society"],
    bloques: [
      {
        titulo: "1 · Hipotiroidismo — diagnóstico",
        items: [
          "Manifiesto: TSH elevada + T4 libre baja.",
          "Subclínico: TSH elevada (4.5–10 mUI/L) con T4 libre normal.",
          "Solicitar anti-TPO si TSH subclínica, para estimar riesgo de progresión.",
        ],
      },
      {
        titulo: "2 · Hipotiroidismo — indicación de tratamiento",
        items: [
          "Manifiesto: tratar siempre.",
          "Subclínico con TSH > 10 mUI/L: tratar.",
          "Subclínico TSH 4.5–10 mUI/L: tratar si síntomas, anti-TPO positivo, embarazo/búsqueda de embarazo, o riesgo cardiovascular elevado; si no, control en 6–12 meses.",
        ],
      },
      {
        titulo: "3 · Hipotiroidismo — tratamiento y seguimiento",
        items: [
          "Levotiroxina ~1.6 µg/kg/día en adultos jóvenes sanos; iniciar con dosis bajas (25–50 µg/día) en > 60 años o cardiopatía, con incrementos graduales.",
          "Tomar en ayunas, separada de calcio/hierro/IBP por ≥ 4 h.",
          "Control de TSH a las 6–8 semanas tras cada ajuste; objetivo TSH dentro de rango normal (individualizar en añosos).",
        ],
      },
      {
        titulo: "4 · Hipertiroidismo — diagnóstico diferencial",
        items: [
          "TSH suprimida + T4L/T3L elevadas → confirmar etiología.",
          "TRAb positivo y bocio difuso → enfermedad de Graves.",
          "Captación de I-131 heterogénea + nódulos → bocio multinodular tóxico / adenoma tóxico.",
          "Captación baja + tirotoxicosis → tiroiditis (subaguda, silente, posparto) — manejo sintomático, no antitiroideos.",
        ],
      },
      {
        titulo: "5 · Hipertiroidismo (Graves) — tratamiento",
        items: [
          "Primera línea: metimazol (evitar primer trimestre de embarazo → propiltiouracilo).",
          "Trial de 12–18 meses; evaluar remisión con TRAb negativo antes de suspender.",
          "Si recidiva o contraindicación a antitiroideos: terapia definitiva con yodo radioactivo o tiroidectomía total.",
          "Beta-bloqueantes (propranolol) para control sintomático mientras se define etiología/tratamiento.",
        ],
      },
    ],
  },
  {
    id: "nodulo-tiroideo",
    nombre: "Nódulo tiroideo / cáncer diferenciado",
    color: "#B4841F",
    fuentes: ["Consenso Delphi FASEN·SAEM·AACCyC·AABYMN·AAOC (2026)", "ATA 2025", "Sistema Bethesda"],
    bloques: [
      {
        titulo: "1 · Evaluación prequirúrgica",
        items: [
          "Ecografía cervical por operador experimentado: estudio de primera línea, evaluando de forma sistemática los compartimentos ganglionares centrales y laterales.",
          "PAAF de ganglios sospechosos solo cuando el resultado pueda modificar la conducta quirúrgica; la tiroglobulina en lavado de aguja es una herramienta complementaria, no un criterio diagnóstico aislado.",
          "Laboratorio mínimo: TSH y calcemia basal. Calcitonina no es de rutina — reservarla para sospecha de carcinoma medular o citología atípica.",
          "TC/RMN y PET/TC con 18F-FDG: no se piden de rutina; solo ante signos clínicos/ecográficos de extensión extratiroidea, síntomas (disnea, disfagia) o sospecha de enfermedad agresiva.",
          "Estudios moleculares prequirúrgicos: no indicados de rutina en citología ya confirmada como maligna (Bethesda V-VI).",
        ],
      },
      {
        titulo: "2 · Citología — sistema Bethesda",
        items: [
          "I No diagnóstica: repetir PAAF.",
          "II Benigna: seguimiento ecográfico periódico.",
          "III / IV Indeterminada: repetir PAAF, test molecular si disponible, o cirugía diagnóstica según riesgo clínico-ecográfico.",
          "V Sospechosa / VI Maligna: definir estrategia quirúrgica.",
        ],
      },
      {
        titulo: "3 · Estrategia terapéutica y extensión quirúrgica",
        items: [
          "Vigilancia activa: opción en carcinoma papilar de bajo riesgo seleccionado (≤1 cm, intratiroideo, cN0, sin histología agresiva), solo con ecografía de alta calidad y decisión compartida con el paciente.",
          "Lesiones únicas < 2 cm de bajo riesgo, sin compromiso ganglionar: hemitiroidectomía como opción de elección.",
          "Tumores 2–4 cm sin factores de alto riesgo: hemitiroidectomía puede considerarse en pacientes seleccionados según preferencias informadas.",
          "Enfermedad localmente avanzada: derivar a centro de mayor complejidad; evaluar cuerdas vocales antes de la cirugía si hay disfonía, disnea o crecimiento significativo.",
          "Disección ganglionar central profiláctica: no de rutina en cN0; sí terapéutica (asociada a tiroidectomía total) si hay compromiso central (cN1a) o lateral (cN1b) clínicamente evidente.",
        ],
      },
      {
        titulo: "4 · Completar tiroidectomía / seguimiento post-hemitiroidectomía",
        items: [
          "Completar a tiroidectomía total si aparecen hallazgos histopatológicos adversos no conocidos antes de operar (invasión vascular, extensión extratiroidea, márgenes comprometidos, variantes agresivas) y si eso cambia la conducta (radioyodo, seguimiento con Tg).",
          "El hallazgo incidental de CDT de bajo riesgo tras hemitiroidectomía no justifica por sí solo completar a tiroidectomía total.",
          "Si se decide completar, puede hacerse de forma diferida sin comprometer el resultado oncológico.",
        ],
      },
      {
        titulo: "5 · Radioyodo (¹³¹I) posquirúrgico",
        items: [
          "Bajo riesgo con resección completa: no indicado de rutina.",
          "Riesgo intermedio: individualizar según histología adversa, Tg/aTg postoperatorios, extensión ganglionar y respuesta inicial.",
          "Alto riesgo: indicado con intención adyuvante salvo contraindicación.",
          "Preparación: dieta baja en yodo 7 días antes / 2 después; TSH objetivo > 30 mUI/L (suspensión hormonal o rhTSH).",
        ],
      },
      {
        titulo: "6 · Estratificación dinámica, TSH y seguimiento",
        items: [
          "Reevaluar la respuesta al tratamiento de forma periódica (excelente / indeterminada / bioquímica incompleta / estructural incompleta) — esta reclasificación dinámica pesa más que el riesgo inicial aislado para decidir conducta.",
          "Objetivo de TSH: subnormal en alto riesgo o enfermedad estructural persistente; 0.1–0.5 mUI/L en riesgo intermedio sin evidencia estructural; rango normal o bajo-normal en bajo riesgo sin evidencia de enfermedad.",
          "Primera evaluación a los 3–6 meses; Tg/aTg/TSH a las 6–12 semanas postoperatorias; ecografía integrada con marcadores bioquímicos a los 6 meses.",
          "Con respuesta excelente sostenida, no se recomienda ecografía sistemática ni rastreo con radioyodo de rutina.",
        ],
      },
      {
        titulo: "7 · Enfermedad persistente, recurrente o metastásica",
        items: [
          "Enfermedad bioquímica persistente sin hallazgo estructural: observación activa, priorizando la tendencia de Tg/aTg por sobre valores aislados.",
          "Enfermedad locorregional estructural: cirugía de elección si es resecable; observación activa si es de bajo volumen, estable y asintomática.",
          "Metástasis a distancia captantes de yodo: el radioyodo es una opción terapéutica; la sola presencia de metástasis no implica indicar terapia sistémica de forma automática.",
          "Terapia sistémica: reservada para progresión estructural clínicamente relevante (RECIST 1.1) tras confirmar refractariedad al radioyodo. Solicitar interrogación genómica (BRAF V600E, fusiones RET/NTRK) para orientar terapias dirigidas antes de indicar inhibidores multiquinasa no selectivos.",
        ],
      },
    ],
  },
  {
    id: "hiperparatiroidismo",
    nombre: "Hiperparatiroidismo primario",
    color: "#6B5B95",
    fuentes: ["Consenso Delphi FASEN sobre hiperparatiroidismo primario", "Guías internacionales de consenso (Workshop internacional)"],
    bloques: [
      {
        titulo: "1 · Diagnóstico bioquímico",
        items: [
          "PTH elevada o inapropiadamente normal en presencia de calcemia elevada (corregida por albúmina) o calcio iónico elevado.",
          "Confirmar hipercalcemia con al menos dos determinaciones; descartar hipercalcemia hipocalciúrica familiar con calciuria de 24 h y clearance de calcio/creatinina.",
          "Solicitar 25-OH vitamina D basal — su déficit puede exagerar la elevación de PTH y debe corregirse antes de reevaluar.",
        ],
      },
      {
        titulo: "2 · Formas clínicas",
        items: [
          "Clásico: hipercalcemia + PTH elevada, con o sin síntomas (nefrolitiasis, fracturas, osteoporosis).",
          "Normocalcémico: PTH elevada con calcemia persistentemente normal, habiendo descartado causas secundarias (déficit de vitamina D, enfermedad renal, hipercalciuria).",
          "Asintomático: hallazgo bioquímico sin manifestaciones clásicas — la mayoría de los casos actuales.",
        ],
      },
      {
        titulo: "3 · Evaluación de órgano blanco",
        items: [
          "Densitometría ósea (columna, cadera y radio distal — este último especialmente sensible al hiperparatiroidismo).",
          "Función renal, calciuria de 24 h e imagen renal (ecografía o TC) para nefrolitiasis/nefrocalcinosis.",
          "Localización prequirúrgica: ecografía cervical + centellograma con sestamibi (o 4D-CT en casos seleccionados) una vez decidida la cirugía — no para el diagnóstico.",
        ],
      },
      {
        titulo: "4 · Indicación de cirugía",
        items: [
          "Todo paciente sintomático (nefrolitiasis, fractura por fragilidad, síntomas neuromusculares).",
          "Asintomático con: calcemia > 1 mg/dL sobre el límite superior normal, T-score ≤ −2.5 en cualquier sitio o fractura vertebral, clearance de creatinina < 60 mL/min, calciuria > 400 mg/24h con riesgo de litiasis, o edad < 50 años.",
          "Paratiroidectomía mínimamente invasiva guiada por localización preoperatoria y PTH intraoperatoria, a cargo de cirujano con experiencia específica.",
        ],
      },
      {
        titulo: "5 · Manejo no quirúrgico / seguimiento",
        items: [
          "Si no cumple criterios quirúrgicos o el paciente no puede/quiere operarse: control anual de calcemia, función renal y densitometría cada 1–2 años.",
          "Cinacalcet: opción para controlar la hipercalcemia cuando la cirugía no es posible.",
          "Bifosfonatos o denosumab: pueden usarse para proteger la masa ósea en quienes no se operan, sin corregir la hipercalcemia.",
          "Asegurar suficiencia de vitamina D (objetivo ~30 ng/mL) de forma cautelosa, monitoreando calcemia al suplementar.",
        ],
      },
    ],
  },
  {
    id: "osteoporosis",
    nombre: "Osteoporosis",
    color: "#6B5B95",
    fuentes: ["AACE / ACE Osteoporosis CPG", "ISCD", "Endocrine Society"],
    bloques: [
      {
        titulo: "1 · Diagnóstico",
        items: [
          "DXA con T-score ≤ −2.5 en columna, cuello femoral, cadera total o radio 33%.",
          "Fractura de fragilidad de cadera o vertebral, independientemente del T-score.",
          "Osteopenia (T-score −1.0 a −2.5) + riesgo alto por FRAX.",
        ],
      },
      {
        titulo: "2 · Estratificación de riesgo",
        items: [
          "Riesgo alto: T-score ≤ −2.5, o FRAX fractura mayor ≥ 20% / cadera ≥ 3% (ajustar umbral según el país).",
          "Riesgo muy alto: fractura reciente (< 2 años), fracturas múltiples, T-score < −3.0, tratamiento con glucocorticoides en dosis altas, o riesgo elevado de caídas.",
        ],
      },
      {
        titulo: "3 · Medidas generales (todos los pacientes)",
        items: [
          "Calcio 1000–1200 mg/día (preferentemente dieta) + vitamina D ~800–1000 UI/día, corrigiendo déficit previo.",
          "Ejercicio de carga y equilibrio; cesación tabáquica; moderar alcohol.",
          "Evaluación y corrección de riesgo de caídas.",
        ],
      },
      {
        titulo: "4 · Tratamiento farmacológico",
        items: [
          "Riesgo alto: antirresortivo de primera línea — bisfosfonato oral (alendronato, risedronato) o IV (zoledronato), o denosumab.",
          "Riesgo muy alto: considerar anabólico primero (teriparatida, abaloparatida o romosozumab) seguido de antirresortivo para consolidar la ganancia ósea.",
          "Osteoporosis inducida por glucocorticoides: umbral de tratamiento más bajo; bisfosfonato o teriparatida según riesgo.",
        ],
      },
      {
        titulo: "5 · Seguimiento",
        items: [
          "DXA de control cada 1–2 años.",
          "Bisfosfonato oral: reevaluar a los 5 años (3 años si IV) — considerar pausa terapéutica si el riesgo bajó.",
          "Denosumab: no suspender sin terapia de transición (riesgo de fracturas vertebrales múltiples por rebote).",
        ],
      },
    ],
  },
  {
    id: "obesidad",
    nombre: "Obesidad",
    color: "#A2483A",
    fuentes: ["EASO — Marco farmacológico 2026", "ACP", "AACE/Endocrine Society"],
    bloques: [
      {
        titulo: "1 · Diagnóstico y evaluación",
        items: [
          "IMC ≥ 30 kg/m² (obesidad), o ≥ 27 kg/m² con al menos una comorbilidad (DM2, HTA, dislipidemia, SAHOS, enfermedad cardiovascular).",
          "Diferenciar complicaciones de 'adiposidad metabólica' (disfunción endocrino-metabólica) vs. 'adiposidad mecánica' (carga articular, SAHOS) para orientar el tratamiento.",
          "Evaluar comorbilidades: perfil glucémico, lipídico, hepático (MASLD/MASH), función respiratoria del sueño.",
        ],
      },
      {
        titulo: "2 · Base del tratamiento — todos los pacientes",
        items: [
          "Intervención en estilo de vida: plan nutricional con déficit calórico, actividad física regular, terapia conductual.",
          "Reevaluar respuesta a los 3 meses antes de intensificar.",
        ],
      },
      {
        titulo: "3 · Farmacoterapia (IMC ≥ 30, o ≥ 27 con comorbilidad)",
        items: [
          "Primera línea: semaglutida o tirzepatida — mayor eficacia comparativa y beneficio cardiometabólico demostrado.",
          "Segunda línea: fentermina-topiramato.",
          "Tercera línea: liraglutida.",
          "Cuarta línea: naltrexona-bupropión.",
          "Selección orientada por complicación predominante: MASH → semaglutida o tirzepatida; DM2 → agonista dual GIP/GLP-1 o GLP-1 RA; enfermedad cardiovascular → GLP-1 RA con beneficio CV probado.",
        ],
      },
      {
        titulo: "4 · Cirugía bariátrica",
        items: [
          "Indicada con IMC ≥ 40, o ≥ 35 con comorbilidad significativa.",
          "Considerar tras respuesta insuficiente a tratamiento médico intensivo, o de entrada en casos seleccionados de alto riesgo.",
        ],
      },
    ],
  },
  {
    id: "diabetes2",
    nombre: "Diabetes tipo 2",
    color: "#4A6FA5",
    fuentes: ["ADA — Standards of Care 2026", "redGDPS", "SAEM"],
    bloques: [
      {
        titulo: "1 · Diagnóstico",
        items: [
          "Glucemia en ayunas ≥ 126 mg/dL, o HbA1c ≥ 6.5%, o glucemia 2h post-PTOG ≥ 200 mg/dL.",
          "Glucemia al azar ≥ 200 mg/dL + síntomas clásicos de hiperglucemia.",
          "Confirmar con una segunda determinación si el paciente está asintomático.",
        ],
      },
      {
        titulo: "2 · Base del tratamiento",
        items: [
          "Metformina + modificación de estilo de vida (nutrición, actividad física) para la mayoría de los pacientes al inicio.",
          "Objetivo de HbA1c individualizado: general < 7%; más laxo (~7.5–8%) en fragilidad, adultos mayores o alto riesgo de hipoglucemia.",
        ],
      },
      {
        titulo: "3 · Selección de segundo fármaco según perfil cardio-renal-metabólico",
        items: [
          "Enfermedad cardiovascular aterosclerótica establecida o alto riesgo: GLP-1 RA o SGLT2i con beneficio cardiovascular comprobado.",
          "Insuficiencia cardíaca: SGLT2i.",
          "Enfermedad renal crónica: SGLT2i (± GLP-1 RA según proteinuria y FGe).",
          "Obesidad / necesidad de pérdida de peso: GLP-1 RA o agonista dual GIP/GLP-1 (tirzepatida), priorizando eficacia sobre el peso.",
          "Esta selección es independiente de la HbA1c basal o del uso previo de metformina.",
        ],
      },
      {
        titulo: "4 · Intensificación",
        items: [
          "Reevaluar a los 3 meses de cada cambio; evitar la inercia terapéutica.",
          "Si no se alcanza el objetivo, intensificar de forma temprana combinando mecanismos de acción complementarios antes de escalar a insulina.",
          "Insulina basal si hiperglucemia marcada, catabolismo o falla de combinación oral/inyectable no insulínica.",
        ],
      },
    ],
  },
  {
    id: "suprarrenal",
    nombre: "Insuficiencia suprarrenal",
    color: "#3F7D6E",
    fuentes: ["Endocrine Society (2016)", "SAEM"],
    bloques: [
      {
        titulo: "1 · Sospecha diagnóstica",
        items: [
          "Cortisol matutino (8h) < 3–5 µg/dL: sugiere insuficiencia suprarrenal.",
          "Cortisol matutino > 15–18 µg/dL: la hace poco probable.",
          "Valores intermedios: requieren test de estimulación.",
        ],
      },
      {
        titulo: "2 · Confirmación",
        items: [
          "Test de estimulación con ACTH 250 µg: cortisol post-estímulo (30–60 min) < 18–20 µg/dL confirma insuficiencia suprarrenal.",
          "ACTH basal elevada + cortisol bajo → insuficiencia primaria (Addison).",
          "ACTH basal baja o inapropiadamente normal + cortisol bajo → insuficiencia secundaria (origen hipofisario) o terciaria (supresión por corticoides exógenos).",
        ],
      },
      {
        titulo: "3 · Tratamiento de reemplazo",
        items: [
          "Hidrocortisona 15–25 mg/día divididos en 2–3 tomas, dosis mayor por la mañana (imita el ritmo circadiano).",
          "Insuficiencia primaria: agregar fludrocortisona 0.05–0.2 mg/día, ajustando según presión arterial, potasio y actividad de renina.",
          "Evitar la supresión excesiva: usar la dosis mínima eficaz que controle los síntomas.",
        ],
      },
      {
        titulo: "4 · Educación y manejo de situaciones de estrés",
        items: [
          "Duplicar o triplicar la dosis oral de hidrocortisona ante enfermedad febril, cirugía menor o estrés significativo.",
          "Hidrocortisona intramuscular de emergencia ante vómitos, incapacidad de vía oral, o crisis suprarrenal.",
          "Brazalete o tarjeta de alerta médica; educación al paciente y su entorno sobre el reconocimiento de una crisis suprarrenal.",
        ],
      },
    ],
  },
];

// Clasificación semántica de cada bloque para asignar ícono + color consistente
// en todos los algoritmos (mismo código de color = mismo tipo de paso clínico).
const BLOCK_TYPES = [
  { key: "diagnostico", label: "Diagnóstico", accent: "#4A6FA5", icon: "search",
    match: ["diagnóstic", "evaluación inicial", "evaluación prequirúrgica", "sospecha diagnóstica", "confirmación", "citología", "evaluación de órgano"] },
  { key: "estratificacion", label: "Estratificación", accent: "#B4841F", icon: "layers",
    match: ["estratificación", "indicación de paaf", "formas clínicas"] },
  { key: "tratamiento", label: "Tratamiento", accent: "#3F7D6E", icon: "pill",
    match: ["tratamiento", "farmacoterapia", "cirugía", "quirúrgic", "manejo farmacológico", "radioyodo", "base del tratamiento", "selección de", "intensificación", "indicación de cirugía", "medidas generales", "completar tiroidectomía"] },
  { key: "seguimiento", label: "Seguimiento", accent: "#6B5B95", icon: "eye",
    match: ["seguimiento", "alta del seguimiento"] },
  { key: "especial", label: "Situaciones especiales", accent: "#A2483A", icon: "alert",
    match: ["situaciones especiales", "educación", "eventos adversos", "enfermedad persistente", "manejo de situaciones de estrés"] },
];

function classifyBlock(titulo) {
  const t = titulo.toLowerCase();
  for (const bt of BLOCK_TYPES) {
    if (bt.match.some((k) => t.includes(k))) return bt;
  }
  return { key: "otro", label: "Paso", accent: "#4A544E", icon: "circle" };
}

function StepIcon({ type, color, size = 15 }) {
  const common = { width: size, height: size, viewBox: "0 0 24 24", fill: "none", stroke: color, strokeWidth: 2.2, strokeLinecap: "round", strokeLinejoin: "round" };
  switch (type) {
    case "search":
      return (<svg {...common}><circle cx="10.5" cy="10.5" r="6.5" /><line x1="20" y1="20" x2="15.3" y2="15.3" /></svg>);
    case "layers":
      return (<svg {...common}><rect x="4" y="13" width="4" height="7" /><rect x="10" y="8" width="4" height="12" /><rect x="16" y="4" width="4" height="16" /></svg>);
    case "pill":
      return (<svg {...common}><rect x="3" y="10.5" width="18" height="7" rx="3.5" transform="rotate(-35 12 14)" /><line x1="10.2" y1="10.2" x2="13.8" y2="17.8" transform="rotate(-35 12 14)" /></svg>);
    case "eye":
      return (<svg {...common}><path d="M2 12s3.8-6.5 10-6.5S22 12 22 12s-3.8 6.5-10 6.5S2 12 2 12z" /><circle cx="12" cy="12" r="2.6" /></svg>);
    case "alert":
      return (<svg {...common}><path d="M12 3.5 22 20H2L12 3.5z" /><line x1="12" y1="10" x2="12" y2="14.5" /><circle cx="12" cy="17.3" r="0.6" fill={color} stroke="none" /></svg>);
    default:
      return (<svg {...common}><circle cx="12" cy="12" r="8" /></svg>);
  }
}

function AlgoritmosTab() {
  const [algoId, setAlgoId] = useState(ALGORITMOS[0].id);
  const algo = ALGORITMOS.find((a) => a.id === algoId);

  return (
    <div>
      <div className="chips-scroll" style={{ display: "flex", gap: "8px", overflowX: "auto", marginBottom: "24px", paddingBottom: "2px" }}>
        {ALGORITMOS.map((a) => (
          <div key={a.id} className={`chip ${algoId === a.id ? "active" : ""}`} onClick={() => setAlgoId(a.id)}>{a.nombre}</div>
        ))}
      </div>

      <div style={{ display: "flex", alignItems: "center", gap: "8px", marginBottom: "6px" }}>
        <div style={{ width: "8px", height: "8px", borderRadius: "50%", background: algo.color }} />
        <div style={{ fontFamily: "'Space Grotesk', sans-serif", fontWeight: 600, fontSize: "19px" }}>{algo.nombre}</div>
      </div>
      <div style={{ display: "flex", gap: "6px", flexWrap: "wrap", marginBottom: "18px" }}>
        {algo.fuentes.map((f, i) => (
          <span key={i} className="eyebrow" style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "5px", padding: "3px 8px", fontSize: "10px" }}>{f}</span>
        ))}
      </div>

      {/* Leyenda de tipos de paso */}
      <div style={{ display: "flex", gap: "14px", flexWrap: "wrap", marginBottom: "24px", padding: "10px 14px", background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "10px" }}>
        {BLOCK_TYPES.map((bt) => (
          <div key={bt.key} style={{ display: "flex", alignItems: "center", gap: "5px" }}>
            <StepIcon type={bt.icon} color={bt.accent} size={12} />
            <span style={{ fontSize: "11px", color: "#4A544E", fontWeight: 500 }}>{bt.label}</span>
          </div>
        ))}
      </div>

      {/* Flujo de pasos */}
      <div>
        {algo.bloques.map((b, i) => {
          const meta = classifyBlock(b.titulo);
          const isLast = i === algo.bloques.length - 1;
          return (
            <div key={i}>
              <div
                style={{
                  background: "#FFFFFF",
                  border: "1px solid #E4E1D6",
                  borderLeft: `4px solid ${meta.accent}`,
                  borderRadius: "12px",
                  padding: "18px 20px",
                  boxShadow: "0 1px 2px rgba(28,35,33,0.04)",
                }}
              >
                <div style={{ display: "flex", alignItems: "center", gap: "10px", marginBottom: "12px" }}>
                  <div
                    style={{
                      width: "30px",
                      height: "30px",
                      borderRadius: "9px",
                      background: meta.accent + "17",
                      display: "flex",
                      alignItems: "center",
                      justifyContent: "center",
                      flexShrink: 0,
                    }}
                  >
                    <StepIcon type={meta.icon} color={meta.accent} size={15} />
                  </div>
                  <div>
                    <div style={{ fontFamily: "'Space Grotesk', sans-serif", fontWeight: 600, fontSize: "14.5px", color: "#1C2321", lineHeight: 1.3 }}>
                      {b.titulo.replace(/^\d+\s*·\s*/, "")}
                    </div>
                    <div className="eyebrow" style={{ color: meta.accent, fontSize: "9.5px", marginTop: "1px" }}>{meta.label}</div>
                  </div>
                </div>
                <ul style={{ margin: 0, paddingLeft: "4px", display: "flex", flexDirection: "column", gap: "8px", listStyle: "none" }}>
                  {b.items.map((it, j) => (
                    <li key={j} style={{ fontSize: "13.5px", color: "#3A423E", lineHeight: 1.55, display: "flex", gap: "9px" }}>
                      <span style={{ color: meta.accent, fontWeight: 700, flexShrink: 0 }}>–</span>
                      <span>{it}</span>
                    </li>
                  ))}
                </ul>
              </div>

              {!isLast && (
                <div style={{ display: "flex", justifyContent: "flex-start", paddingLeft: "14px" }}>
                  <svg width="16" height="26" viewBox="0 0 16 26" fill="none">
                    <line x1="8" y1="0" x2="8" y2="16" stroke="#D8D5CB" strokeWidth="2" />
                    <path d="M2 14 L8 22 L14 14" stroke="#D8D5CB" strokeWidth="2" fill="none" strokeLinecap="round" strokeLinejoin="round" />
                  </svg>
                </div>
              )}
            </div>
          );
        })}
      </div>

      <div style={{ marginTop: "20px" }}>
        <Disclaimer texto="Estos algoritmos resumen lineamientos generales de guías internacionales y de sociedades nacionales vigentes al momento de su elaboración; no reemplazan el juicio clínico individualizado, las políticas de cobertura locales, ni las actualizaciones que cada sociedad publique con posterioridad. Verificar siempre la versión más reciente de la guía correspondiente antes de tomar una decisión terapéutica." />
      </div>
    </div>
  );
}

/* ============================================================
   MÓDULO 5 — RIESGO CARDIOVASCULAR (PREVENT)
   ============================================================ */
// Hazard ratios reales del modelo PREVENT "mejorado" (base + UACR + HbA1c),
// tomados de la Tabla 3 de Khan SS, et al. "Development and Validation of
// the American Heart Association's PREVENT Equations." Circulation.
// 2024;149:430–449. Modelo centrado en: 55 años, non-HDL-C 3.5 mmol/L,
// HDL-C 1.3 mmol/L, PAS 130 mmHg, IMC 25 kg/m², eGFR 90 mL/min/1.73m²,
// sin diabetes, no fumador, sin medicación, ACR 1 mg/g, HbA1c 5.3%.
// El colesterol y el IMC NO son intercambiables entre modelos: el paper
// no incluye IMC como predictor de CVD total/ASCVD (marcado "*" en la
// Tabla 3), y no incluye colesterol como predictor de insuficiencia
// cardíaca — se respeta esa estructura tal cual está publicada.
const PREVENT_TOTAL = {
  mujer: {
    nonHDL: 1.00, HDL: 0.86, sbpLow: 0.82, sbpHigh: 1.36,
    diabetes: 1.65, smoking: 1.62, egfrLow: 1.72, egfrHigh: 1.05,
    antiHTA: 1.35, statin: 0.85, treatedSBP: 0.93, treatedNonHDL: 1.11,
    age_nonHDL: 0.93, age_HDL: 1.03, age_sbpHigh: 0.92, age_diabetes: 0.80,
    age_smoking: 0.94, age_egfrLow: 0.89,
    lnUACR: 1.19, noUACR: 1.02, hba1cDM: 1.14, hba1cNoDM: 1.15, noHbA1c: 0.99,
  },
  hombre: {
    nonHDL: 1.05, HDL: 0.92, sbpLow: 0.59, sbpHigh: 1.35,
    diabetes: 1.58, smoking: 1.48, egfrLow: 1.61, egfrHigh: 1.00,
    antiHTA: 1.29, statin: 0.84, treatedSBP: 0.95, treatedNonHDL: 1.15,
    age_nonHDL: 0.95, age_HDL: 1.02, age_sbpHigh: 0.90, age_diabetes: 0.85,
    age_smoking: 0.94, age_egfrLow: 0.91,
    lnUACR: 1.21, noUACR: 1.12, hba1cDM: 1.13, hba1cNoDM: 1.11, noHbA1c: 0.97,
  },
};

const PREVENT_HF = {
  mujer: {
    sbpLow: 0.65, sbpHigh: 1.36, diabetes: 1.87, smoking: 1.75,
    bmiLow: 0.97, bmiHigh: 1.32, egfrLow: 1.96, egfrHigh: 1.06,
    antiHTA: 1.39, treatedSBP: 0.90,
    age_sbpHigh: 0.93, age_diabetes: 0.75, age_smoking: 0.90,
    age_bmiHigh: 0.99, age_egfrLow: 0.87,
    lnUACR: 1.23, noUACR: 1.04, hba1cDM: 1.20, hba1cNoDM: 1.18, noHbA1c: 1.00,
  },
  hombre: {
    sbpLow: 0.49, sbpHigh: 1.37, diabetes: 1.75, smoking: 1.58,
    bmiLow: 0.89, bmiHigh: 1.43, egfrLow: 1.83, egfrHigh: 1.01,
    antiHTA: 1.29, treatedSBP: 0.94,
    age_sbpHigh: 0.89, age_diabetes: 0.80, age_smoking: 0.91,
    age_bmiHigh: 1.00, age_egfrLow: 0.89,
    lnUACR: 1.27, noUACR: 1.19, hba1cDM: 1.17, hba1cNoDM: 1.13, noHbA1c: 0.97,
  },
};

function calcularUACRyHbA1c(hr, form, ln) {
  const uacr = form.uacr === "" ? null : parseFloat(form.uacr);
  const hba1c = form.hba1c === "" ? null : parseFloat(form.hba1c);
  const diabetes = form.diabetes === "si";

  const uacrTerm = uacr && uacr > 0 ? ln(uacr) * ln(hr.lnUACR) : ln(hr.noUACR);
  const hba1cTerm =
    hba1c != null
      ? (hba1c - 5.3) * ln(diabetes ? hr.hba1cDM : hr.hba1cNoDM)
      : ln(hr.noHbA1c);

  return uacrTerm + hba1cTerm;
}

function calcularIndiceTotalCVD(form) {
  const hr = PREVENT_TOTAL[form.sexo];
  const ln = Math.log;
  const edad = parseFloat(form.edad) || 55;
  const sbp = parseFloat(form.pas) || 130;
  const egfr = parseFloat(form.egfr) || 90;
  const nonHDLmmol = (parseFloat(form.colTotal) - parseFloat(form.colHDL)) / 38.67;
  const HDLmmol = parseFloat(form.colHDL) / 38.67;
  const diabetes = form.diabetes === "si";
  const smoking = form.fumador === "si";
  const antiHTA = form.tratHTA === "si";
  const statin = form.estatina === "si";
  const dAge = (edad - 55) / 10;

  const nonHDLdev = nonHDLmmol - 3.5;
  const HDLdev = (HDLmmol - 1.3) / 0.3;

  let sbpMain, sbpAgeInt;
  if (sbp >= 110) {
    sbpMain = ((sbp - 130) / 20) * ln(hr.sbpHigh);
    sbpAgeInt = dAge * ((sbp - 130) / 20) * ln(hr.age_sbpHigh);
  } else {
    sbpMain = ((sbp - 110) / 20) * ln(hr.sbpLow) - ln(hr.sbpHigh);
    sbpAgeInt = dAge * -ln(hr.age_sbpHigh);
  }

  let egfrMain, egfrAgeInt;
  if (egfr >= 60) {
    egfrMain = ((90 - egfr) / 15) * ln(hr.egfrHigh);
    egfrAgeInt = 0;
  } else {
    egfrMain = 2 * ln(hr.egfrHigh) + ((60 - egfr) / 15) * ln(hr.egfrLow);
    egfrAgeInt = dAge * ((60 - egfr) / 15) * ln(hr.age_egfrLow);
  }

  const diabetesMain = diabetes ? ln(hr.diabetes) : 0;
  const diabetesAgeInt = diabetes ? dAge * ln(hr.age_diabetes) : 0;
  const smokingMain = smoking ? ln(hr.smoking) : 0;
  const smokingAgeInt = smoking ? dAge * ln(hr.age_smoking) : 0;
  const antiHTAMain = antiHTA ? ln(hr.antiHTA) : 0;
  const statinMain = statin ? ln(hr.statin) : 0;
  const treatedSBPterm = antiHTA && sbp >= 110 ? ((sbp - 130) / 20) * ln(hr.treatedSBP) : 0;
  const treatedNonHDLterm = statin ? nonHDLdev * ln(hr.treatedNonHDL) : 0;

  const L =
    nonHDLdev * ln(hr.nonHDL) +
    HDLdev * ln(hr.HDL) +
    sbpMain + sbpAgeInt +
    egfrMain + egfrAgeInt +
    diabetesMain + diabetesAgeInt +
    smokingMain + smokingAgeInt +
    antiHTAMain + statinMain +
    treatedSBPterm + treatedNonHDLterm +
    dAge * (nonHDLdev * ln(hr.age_nonHDL) + HDLdev * ln(hr.age_HDL)) +
    calcularUACRyHbA1c(hr, form, ln);

  return Math.exp(L);
}

function calcularIndiceHF(form) {
  const hr = PREVENT_HF[form.sexo];
  const ln = Math.log;
  const edad = parseFloat(form.edad) || 55;
  const sbp = parseFloat(form.pas) || 130;
  const egfr = parseFloat(form.egfr) || 90;
  const bmi = parseFloat(form.bmi) || 25;
  const diabetes = form.diabetes === "si";
  const smoking = form.fumador === "si";
  const antiHTA = form.tratHTA === "si";
  const dAge = (edad - 55) / 10;

  let sbpMain, sbpAgeInt;
  if (sbp >= 110) {
    sbpMain = ((sbp - 130) / 20) * ln(hr.sbpHigh);
    sbpAgeInt = dAge * ((sbp - 130) / 20) * ln(hr.age_sbpHigh);
  } else {
    sbpMain = ((sbp - 110) / 20) * ln(hr.sbpLow) - ln(hr.sbpHigh);
    sbpAgeInt = dAge * -ln(hr.age_sbpHigh);
  }

  let egfrMain, egfrAgeInt;
  if (egfr >= 60) {
    egfrMain = ((90 - egfr) / 15) * ln(hr.egfrHigh);
    egfrAgeInt = 0;
  } else {
    egfrMain = 2 * ln(hr.egfrHigh) + ((60 - egfr) / 15) * ln(hr.egfrLow);
    egfrAgeInt = dAge * ((60 - egfr) / 15) * ln(hr.age_egfrLow);
  }

  // Spline de IMC (nudo en 30, centrado en 25 — el ancla queda en el tramo bajo)
  let bmiMain, bmiAgeInt;
  if (bmi <= 30) {
    bmiMain = ((bmi - 25) / 5) * ln(hr.bmiLow);
    bmiAgeInt = 0;
  } else {
    bmiMain = ((30 - 25) / 5) * ln(hr.bmiLow) + ((bmi - 30) / 5) * ln(hr.bmiHigh);
    bmiAgeInt = dAge * ((bmi - 30) / 5) * ln(hr.age_bmiHigh);
  }

  const diabetesMain = diabetes ? ln(hr.diabetes) : 0;
  const diabetesAgeInt = diabetes ? dAge * ln(hr.age_diabetes) : 0;
  const smokingMain = smoking ? ln(hr.smoking) : 0;
  const smokingAgeInt = smoking ? dAge * ln(hr.age_smoking) : 0;
  const antiHTAMain = antiHTA ? ln(hr.antiHTA) : 0;
  const treatedSBPterm = antiHTA && sbp >= 110 ? ((sbp - 130) / 20) * ln(hr.treatedSBP) : 0;

  const L =
    sbpMain + sbpAgeInt +
    egfrMain + egfrAgeInt +
    bmiMain + bmiAgeInt +
    diabetesMain + diabetesAgeInt +
    smokingMain + smokingAgeInt +
    antiHTAMain + treatedSBPterm +
    calcularUACRyHbA1c(hr, form, ln);

  return Math.exp(L);
}

function PreventTab() {
  const [form, setForm] = useState({
    sexo: "mujer",
    edad: 55,
    colTotal: 200,
    colHDL: 50,
    pas: 130,
    tratHTA: "no",
    estatina: "no",
    diabetes: "no",
    fumador: "no",
    egfr: 90,
    bmi: 25,
    hba1c: "",
    uacr: "",
  });

  const set = (k) => (e) => setForm({ ...form, [k]: e.target.value });
  const indiceTotal = useMemo(() => calcularIndiceTotalCVD(form), [form]);
  const indiceHF = useMemo(() => calcularIndiceHF(form), [form]);
  const buildOfficialUrl = () => "https://professional.heart.org/en/guidelines-and-statements/prevent-calculator";

  return (
    <div>
      <div
        style={{
          background: "#1C2321",
          borderRadius: "14px",
          padding: "24px",
          marginBottom: "20px",
        }}
      >
        <div className="eyebrow" style={{ color: "#9BA89F", marginBottom: "4px" }}>
          AHA · Predicting Risk of CVD EVENTs — Khan et al., Circulation 2024
        </div>
        <div style={{ color: "#F5F4F0", fontFamily: "'Space Grotesk', sans-serif", fontWeight: 600, fontSize: "18px", marginBottom: "10px" }}>
          Índice de riesgo relativo — modelo mejorado (+ HbA1c, microalbuminuria, IMC)
        </div>
        <div style={{ color: "#C9CFC9", fontSize: "13px", lineHeight: 1.6 }}>
          El índice de CVD total usa la Tabla 3 (modelo base + UACR + HbA1c). El IMC no es predictor de
          CVD total ni de ASCVD en el modelo publicado — sí lo es del riesgo específico de insuficiencia
          cardíaca, que se muestra aparte, tal como está estructurado el artículo original.
        </div>
      </div>

      <div style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "14px", padding: "24px", marginBottom: "20px" }}>
        <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr", gap: "16px" }} className="grid-cols-resp">
          <Field label="Sexo biológico">
            <select value={form.sexo} onChange={set("sexo")} style={selectStyle}>
              <option value="mujer">Mujer</option>
              <option value="hombre">Hombre</option>
            </select>
          </Field>
          <Field label="Edad (30–79 años)">
            <input type="number" min="30" max="79" value={form.edad} onChange={set("edad")} style={inputStyle} />
          </Field>
          <Field label="Colesterol total (mg/dL)">
            <input type="number" value={form.colTotal} onChange={set("colTotal")} style={inputStyle} />
          </Field>
          <Field label="Colesterol HDL (mg/dL)">
            <input type="number" value={form.colHDL} onChange={set("colHDL")} style={inputStyle} />
          </Field>
          <Field label="Presión arterial sistólica (mmHg)">
            <input type="number" value={form.pas} onChange={set("pas")} style={inputStyle} />
          </Field>
          <Field label="eGFR (mL/min/1.73m²)">
            <input type="number" value={form.egfr} onChange={set("egfr")} style={inputStyle} />
          </Field>
          <Field label="IMC (kg/m²) — usado solo en insuf. cardíaca">
            <input type="number" step="0.1" value={form.bmi} onChange={set("bmi")} style={inputStyle} />
          </Field>
          <Field label="HbA1c % (opcional)">
            <input type="number" step="0.1" placeholder="no disponible" value={form.hba1c} onChange={set("hba1c")} style={inputStyle} />
          </Field>
          <Field label="Microalbuminuria — UACR mg/g (opcional)">
            <input type="number" step="0.1" placeholder="no disponible" value={form.uacr} onChange={set("uacr")} style={inputStyle} />
          </Field>
          <Field label="Tratamiento antihipertensivo">
            <select value={form.tratHTA} onChange={set("tratHTA")} style={selectStyle}>
              <option value="no">No</option>
              <option value="si">Sí</option>
            </select>
          </Field>
          <Field label="Uso de estatinas">
            <select value={form.estatina} onChange={set("estatina")} style={selectStyle}>
              <option value="no">No</option>
              <option value="si">Sí</option>
            </select>
          </Field>
          <Field label="Diabetes">
            <select value={form.diabetes} onChange={set("diabetes")} style={selectStyle}>
              <option value="no">No</option>
              <option value="si">Sí</option>
            </select>
          </Field>
          <Field label="Tabaquismo actual">
            <select value={form.fumador} onChange={set("fumador")} style={selectStyle}>
              <option value="no">No</option>
              <option value="si">Sí</option>
            </select>
          </Field>
        </div>
      </div>

      {/* Resultados */}
      <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr", gap: "16px", marginBottom: "20px" }} className="grid-cols-resp">
        <div style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "14px", padding: "24px", textAlign: "center" }}>
          <div className="eyebrow" style={{ marginBottom: "10px" }}>CVD total (+ UACR, HbA1c)</div>
          <div className="num" style={{ fontSize: "36px", fontWeight: 700, color: indiceTotal >= 2 ? "#A2483A" : indiceTotal >= 1.3 ? "#B4841F" : "#3F7D6E" }}>
            {indiceTotal.toFixed(2)}×
          </div>
          <div style={{ fontSize: "12px", color: "#4A544E", marginTop: "6px" }}>vs. referencia óptima de 55 años</div>
        </div>
        <div style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "14px", padding: "24px", textAlign: "center" }}>
          <div className="eyebrow" style={{ marginBottom: "10px" }}>Insuficiencia cardíaca (+ IMC)</div>
          <div className="num" style={{ fontSize: "36px", fontWeight: 700, color: indiceHF >= 2 ? "#A2483A" : indiceHF >= 1.3 ? "#B4841F" : "#3F7D6E" }}>
            {indiceHF.toFixed(2)}×
          </div>
          <div style={{ fontSize: "12px", color: "#4A544E", marginTop: "6px" }}>vs. referencia óptima de 55 años</div>
        </div>
      </div>

      <div style={{ textAlign: "center", marginBottom: "20px" }}>
        <a
          href={buildOfficialUrl()}
          target="_blank"
          rel="noopener noreferrer"
          style={{
            display: "inline-block",
            background: "#1C2321",
            color: "#F5F4F0",
            borderRadius: "10px",
            padding: "12px 22px",
            fontWeight: 600,
            fontSize: "13.5px",
            textDecoration: "none",
          }}
        >
          Obtener el % de riesgo absoluto en la calculadora oficial de la AHA ↗
        </a>
      </div>

      {/* Interpretación de categorías de riesgo */}
      <div style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "14px", padding: "22px 24px", marginBottom: "20px" }}>
        <div className="eyebrow" style={{ marginBottom: "14px" }}>Interpretación del riesgo ASCVD a 10 años (guía ACC/AHA de colesterol)</div>
        {[
          { rango: "< 5%", cat: "Bajo", color: "#3F7D6E", conducta: "Reforzar estilo de vida; reevaluar en 4–6 años." },
          { rango: "5 – 7.4%", cat: "Límite", color: "#B4841F", conducta: "Considerar factores agravantes; discutir estatina si hay potenciadores de riesgo." },
          { rango: "7.5 – 19.9%", cat: "Intermedio", color: "#B4841F", conducta: "Estatina de intensidad moderada, con decisión compartida." },
          { rango: "≥ 20%", cat: "Alto", color: "#A2483A", conducta: "Estatina de alta intensidad." },
        ].map((r, i) => (
          <div key={i} style={{ display: "grid", gridTemplateColumns: "0.8fr 0.8fr 2fr", gap: "12px", padding: "10px 0", borderBottom: i < 3 ? "1px solid #F0EEE6" : "none", alignItems: "center" }}>
            <div className="num" style={{ fontWeight: 600, fontSize: "13.5px" }}>{r.rango}</div>
            <div>
              <span style={{ fontSize: "11px", fontWeight: 700, color: r.color, background: r.color + "1A", borderRadius: "4px", padding: "2px 8px" }}>{r.cat}</span>
            </div>
            <div style={{ fontSize: "12.5px", color: "#4A544E" }}>{r.conducta}</div>
          </div>
        ))}
      </div>

      <Disclaimer texto="Estos índices usan los hazard ratios reales y verificados de la Tabla 3 del artículo original de PREVENT (Khan et al., Circulation 2024) — el modelo con UACR y HbA1c sumados al modelo base, incluyendo splines de presión arterial, eGFR e IMC, e interacciones con la edad. El IMC solo interviene en el índice de insuficiencia cardíaca porque así está publicado el modelo (no es predictor de CVD total ni de ASCVD en este artículo). Si dejás HbA1c o microalbuminuria en blanco, se usa el coeficiente publicado para 'dato no disponible', igual que hace el modelo original. Estos índices NO calculan el porcentaje de riesgo absoluto a 10 años: para eso falta la función de riesgo basal específica por edad y sexo, publicada solo en el material suplementario (Tablas S12, que seguimos sin tener). Usalos para comparar perfiles de riesgo entre pacientes o el impacto de modificar un factor, y la calculadora oficial ACC/AHA para el porcentaje que efectivamente se usa en la decisión clínica de estatinas." />
    </div>
  );
}

const inputStyle = { width: "100%", background: "#FAF9F5", color: "#1C2321", border: "1px solid #D8D5CB", borderRadius: "8px", padding: "11px 12px", fontSize: "14px", fontWeight: 500, fontFamily: "'IBM Plex Mono', monospace" };
const selectStyle = { ...inputStyle, fontFamily: "'IBM Plex Sans', sans-serif" };

function Field({ label, children }) {
  return (
    <div>
      <label className="eyebrow" style={{ display: "block", marginBottom: "7px" }}>{label}</label>
      {children}
    </div>
  );
}

/* ============================================================
   MÓDULO 6 — MASLD: CALCULADORA FIB-4 + ALGORITMO EASL-EASD-EASO
   ============================================================ */
const MASLD_BLOQUES = [
  {
    titulo: "Población a tamizar (case-finding)",
    items: [
      "Diabetes tipo 2 (cualquier edad): tamizar FIB-4 de rutina, independientemente de las enzimas hepáticas.",
      "Obesidad o sobrepeso con ≥1 factor de riesgo cardiometabólico adicional (HTA, dislipidemia, prediabetes, síndrome metabólico).",
      "Elevación persistente e inexplicada de transaminasas.",
      "Hallazgo incidental de esteatosis hepática en una ecografía u otro estudio de imagen.",
    ],
  },
  {
    titulo: "Diagnóstico de MASLD (definición)",
    items: [
      "Esteatosis hepática (por imagen o histología) + al menos 1 factor de riesgo cardiometabólico (IMC ≥25, circunferencia de cintura aumentada, prediabetes/DM2, HTA, dislipidemia).",
      "Ausencia de consumo de alcohol de riesgo (evaluar cantidad, patrón y tipo de consumo con historia clínica detallada y/o biomarcadores) y de otras causas de enfermedad hepática.",
      "Reemplaza a la antigua denominación NAFLD; el espectro incluye esteatosis simple, MASH (antes NASH), fibrosis, cirrosis y hepatocarcinoma asociado a MASH.",
    ],
  },
  {
    titulo: "Algoritmo diagnóstico escalonado — paso 1: FIB-4",
    items: [
      "FIB-4 < 1.3 (< 65 años) o < 2.0 (≥ 65 años): riesgo bajo de fibrosis avanzada — no requiere estudios adicionales; reevaluar cada 1–2 años si persisten los factores de riesgo.",
      "FIB-4 1.3–2.67 (< 65 años) o 2.0–2.67 (≥ 65 años): riesgo indeterminado — pasar a elastografía de transición (VCTE/FibroScan).",
      "FIB-4 > 2.67: riesgo alto de fibrosis avanzada — VCTE o derivación directa a hepatología según disponibilidad.",
    ],
  },
  {
    titulo: "Algoritmo diagnóstico escalonado — paso 2: elastografía (VCTE)",
    items: [
      "LSM < 8 kPa: riesgo bajo — mantener seguimiento en atención primaria/endocrinología.",
      "LSM 8–12 kPa: riesgo indeterminado — considerar reevaluación en 1–2 años, optimizar factores metabólicos, o ELF/pruebas de segunda línea si están disponibles.",
      "LSM > 12 kPa: alta probabilidad de fibrosis avanzada — derivar a hepatología para confirmación (eventual biopsia) y estadificación.",
    ],
  },
  {
    titulo: "Tratamiento — pilar de estilo de vida (todos los pacientes)",
    items: [
      "Pérdida de peso ≥5% para mejorar la esteatosis; ≥7–10% para mejorar la esteatohepatitis; >10% puede lograr regresión de la fibrosis.",
      "Dieta con reducción calórica (patrón mediterráneo preferido) y actividad física regular, independientemente del descenso de peso logrado.",
      "Desalentar activamente el consumo de alcohol.",
      "Optimizar las comorbilidades metabólicas (diabetes, dislipidemia, hipertensión) como parte central del tratamiento, no como algo secundario.",
    ],
  },
  {
    titulo: "Tratamiento — manejo de comorbilidades y fármacos con beneficio hepático",
    items: [
      "Terapias basadas en incretinas (agonistas GLP-1, agonistas duales GIP/GLP-1) recomendadas cuando hay indicación de descenso de peso y/o diabetes — con beneficio adicional sobre la esteatohepatitis.",
      "Las estatinas son seguras en MASLD, incluso con transaminasas moderadamente elevadas, y deben usarse según el riesgo cardiovascular del paciente.",
      "Evitar sulfonilureas en pacientes con descompensación hepática, por riesgo de hipoglucemia.",
      "No se recomiendan agentes para el descenso de peso no basados en incretinas como terapia dirigida a MASH.",
    ],
  },
  {
    titulo: "Tratamiento — farmacoterapia dirigida a MASH",
    items: [
      "Considerar resmetirom en adultos con MASH no cirróticos y fibrosis significativa (estadio ≥2).",
      "No se recomienda vitamina E como terapia dirigida a MASH (cambio respecto de guías previas).",
      "En la etapa cirrótica, actualmente no hay farmacoterapia dirigida a MASH recomendada.",
      "Toda indicación de terapia dirigida a MASH debe evaluarse en conjunto con hepatología.",
    ],
  },
  {
    titulo: "Seguimiento y derivación",
    items: [
      "Riesgo bajo persistente: control de FIB-4 cada 1–2 años junto con el manejo metabólico habitual.",
      "Riesgo indeterminado o alto, o progresión documentada: seguimiento conjunto con hepatología.",
      "Reevaluar el riesgo si cambian significativamente el peso corporal o el control glucémico, ya que pueden modificar la trayectoria de la enfermedad.",
    ],
  },
];

function FIB4Calculator() {
  const [edad, setEdad] = useState(55);
  const [ast, setAst] = useState(30);
  const [alt, setAlt] = useState(30);
  const [plaquetas, setPlaquetas] = useState(220);

  const fib4 = useMemo(() => {
    const a = parseFloat(edad), s = parseFloat(ast), l = parseFloat(alt), p = parseFloat(plaquetas);
    if (!a || !s || !l || !p || l <= 0 || p <= 0) return null;
    return (a * s) / (p * Math.sqrt(l));
  }, [edad, ast, alt, plaquetas]);

  const edadNum = parseFloat(edad) || 0;
  const umbralBajo = edadNum >= 65 ? 2.0 : 1.3;

  let categoria = null;
  if (fib4 != null) {
    if (fib4 < umbralBajo) categoria = { label: "Riesgo bajo", color: "#3F7D6E", texto: "No requiere estudios adicionales por ahora. Reevaluar en 1–2 años si persisten factores de riesgo." };
    else if (fib4 <= 2.67) categoria = { label: "Riesgo indeterminado", color: "#B4841F", texto: "Continuar con elastografía de transición (VCTE/FibroScan)." };
    else categoria = { label: "Riesgo alto", color: "#A2483A", texto: "Alta probabilidad de fibrosis avanzada — VCTE o derivación a hepatología." };
  }

  return (
    <div style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "14px", padding: "24px", marginBottom: "20px" }}>
      <div className="eyebrow" style={{ marginBottom: "16px" }}>Calculadora FIB-4</div>
      <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr", gap: "16px", marginBottom: "20px" }} className="grid-cols-resp">
        <Field label="Edad (años)">
          <input type="number" value={edad} onChange={(e) => setEdad(e.target.value)} style={inputStyle} />
        </Field>
        <Field label="Plaquetas (×10⁹/L)">
          <input type="number" value={plaquetas} onChange={(e) => setPlaquetas(e.target.value)} style={inputStyle} />
        </Field>
        <Field label="AST / GOT (U/L)">
          <input type="number" value={ast} onChange={(e) => setAst(e.target.value)} style={inputStyle} />
        </Field>
        <Field label="ALT / GPT (U/L)">
          <input type="number" value={alt} onChange={(e) => setAlt(e.target.value)} style={inputStyle} />
        </Field>
      </div>

      <div style={{ background: "#FAF9F5", border: "1px solid #E4E1D6", borderRadius: "10px", padding: "10px 14px", marginBottom: "18px", fontSize: "12px", color: "#4A544E" }}>
        <span className="eyebrow" style={{ marginRight: "6px" }}>Fórmula</span>
        FIB-4 = (Edad × AST) / (Plaquetas × √ALT)
      </div>

      {fib4 != null && (
        <div style={{ textAlign: "center", padding: "20px 0", borderTop: "1px solid #F0EEE6" }}>
          <div className="num" style={{ fontSize: "40px", fontWeight: 700, color: categoria.color }}>
            {fib4.toFixed(2)}
          </div>
          <div style={{ marginTop: "8px" }}>
            <span style={{ fontSize: "12px", fontWeight: 700, color: categoria.color, background: categoria.color + "1A", borderRadius: "5px", padding: "3px 10px" }}>
              {categoria.label}
            </span>
          </div>
          <div style={{ fontSize: "13px", color: "#4A544E", maxWidth: "420px", margin: "10px auto 0" }}>
            {categoria.texto}
          </div>
          <div className="eyebrow" style={{ marginTop: "10px", color: "#8A9089" }}>
            Umbral de riesgo bajo aplicado: FIB-4 &lt; {umbralBajo} ({edadNum >= 65 ? "≥ 65 años" : "< 65 años"})
          </div>
        </div>
      )}
    </div>
  );
}

function MasldTab() {
  return (
    <div>
      <div style={{ display: "flex", alignItems: "center", gap: "8px", marginBottom: "6px" }}>
        <div style={{ width: "8px", height: "8px", borderRadius: "50%", background: "#B4841F" }} />
        <div style={{ fontFamily: "'Space Grotesk', sans-serif", fontWeight: 600, fontSize: "19px" }}>
          MASLD — Enfermedad hepática esteatósica asociada a disfunción metabólica
        </div>
      </div>
      <div style={{ display: "flex", gap: "6px", flexWrap: "wrap", marginBottom: "22px" }}>
        <span className="eyebrow" style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "5px", padding: "3px 8px", fontSize: "10px" }}>
          EASL · EASD · EASO (2024) — J Hepatol 2024;81:492–542
        </span>
      </div>

      <FIB4Calculator />

      <div style={{ position: "relative" }}>
        {MASLD_BLOQUES.map((b, i) => {
          const meta = classifyBlock(b.titulo);
          const isLast = i === MASLD_BLOQUES.length - 1;
          return (
            <div key={i}>
              <div
                style={{
                  background: "#FFFFFF",
                  border: "1px solid #E4E1D6",
                  borderLeft: `4px solid ${meta.accent}`,
                  borderRadius: "12px",
                  padding: "18px 20px",
                  boxShadow: "0 1px 2px rgba(28,35,33,0.04)",
                }}
              >
                <div style={{ display: "flex", alignItems: "center", gap: "10px", marginBottom: "12px" }}>
                  <div style={{ width: "30px", height: "30px", borderRadius: "9px", background: meta.accent + "17", display: "flex", alignItems: "center", justifyContent: "center", flexShrink: 0 }}>
                    <StepIcon type={meta.icon} color={meta.accent} size={15} />
                  </div>
                  <div>
                    <div style={{ fontFamily: "'Space Grotesk', sans-serif", fontWeight: 600, fontSize: "14.5px", color: "#1C2321", lineHeight: 1.3 }}>
                      {b.titulo}
                    </div>
                    <div className="eyebrow" style={{ color: meta.accent, fontSize: "9.5px", marginTop: "1px" }}>{meta.label}</div>
                  </div>
                </div>
                <ul style={{ margin: 0, paddingLeft: "4px", display: "flex", flexDirection: "column", gap: "8px", listStyle: "none" }}>
                  {b.items.map((it, j) => (
                    <li key={j} style={{ fontSize: "13.5px", color: "#3A423E", lineHeight: 1.55, display: "flex", gap: "9px" }}>
                      <span style={{ color: meta.accent, fontWeight: 700, flexShrink: 0 }}>–</span>
                      <span>{it}</span>
                    </li>
                  ))}
                </ul>
              </div>
              {!isLast && (
                <div style={{ display: "flex", justifyContent: "flex-start", paddingLeft: "14px" }}>
                  <svg width="16" height="26" viewBox="0 0 16 26" fill="none">
                    <line x1="8" y1="0" x2="8" y2="16" stroke="#D8D5CB" strokeWidth="2" />
                    <path d="M2 14 L8 22 L14 14" stroke="#D8D5CB" strokeWidth="2" fill="none" strokeLinecap="round" strokeLinejoin="round" />
                  </svg>
                </div>
              )}
            </div>
          );
        })}
      </div>

      <div style={{ marginTop: "20px" }}>
        <Disclaimer texto="El FIB-4 tiene menor rendimiento en extremos de edad (sobreestima riesgo en adultos jóvenes y en > 65 años, de ahí el umbral ajustado) y no es válido con transaminasas muy elevadas por causas agudas. No reemplaza la evaluación clínica completa: descartar siempre consumo de alcohol de riesgo y otras causas de enfermedad hepática antes de atribuir los hallazgos a MASLD. Esta solapa resume la guía conjunta EASL-EASD-EASO 2024; verificar la versión vigente antes de decisiones terapéuticas." />
      </div>
    </div>
  );
}

/* ============================================================
   MÓDULO 7 — PARÁMETROS DE OBESIDAD Y ADIPOSIDAD CENTRAL
   ============================================================ */
function categoriaIMC(imc) {
  if (imc < 18.5) return { label: "Bajo peso", color: "#4A6FA5" };
  if (imc < 25) return { label: "Normal", color: "#3F7D6E" };
  if (imc < 30) return { label: "Sobrepeso", color: "#B4841F" };
  if (imc < 35) return { label: "Obesidad grado I", color: "#A2483A" };
  if (imc < 40) return { label: "Obesidad grado II", color: "#A2483A" };
  return { label: "Obesidad grado III", color: "#A2483A" };
}

function categoriaICT(ict) {
  if (ict < 0.5) return { label: "Riesgo bajo", color: "#3F7D6E" };
  if (ict < 0.6) return { label: "Riesgo aumentado", color: "#B4841F" };
  return { label: "Riesgo alto", color: "#A2483A" };
}

function categoriaICC(icc, sexo) {
  const umbralAlto = sexo === "mujer" ? 0.85 : 1.0;
  const umbralModerado = sexo === "mujer" ? 0.8 : 0.9;
  if (icc < umbralModerado) return { label: "Riesgo bajo", color: "#3F7D6E" };
  if (icc < umbralAlto) return { label: "Riesgo moderado", color: "#B4841F" };
  return { label: "Riesgo alto", color: "#A2483A" };
}

function categoriaTGHDL(r) {
  if (r < 2) return { label: "Óptimo", color: "#3F7D6E" };
  if (r < 3) return { label: "Intermedio", color: "#B4841F" };
  return { label: "Elevado — sugiere insulinorresistencia", color: "#A2483A" };
}

function categoriaVAT(area) {
  if (area < 100) return { label: "Riesgo bajo (orientativo)", color: "#3F7D6E" };
  if (area <= 160) return { label: "Riesgo aumentado (orientativo)", color: "#B4841F" };
  return { label: "Riesgo alto (orientativo)", color: "#A2483A" };
}

function ResultCard({ titulo, valor, unidad, categoria }) {
  return (
    <div style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "12px", padding: "18px", textAlign: "center" }}>
      <div className="eyebrow" style={{ marginBottom: "8px" }}>{titulo}</div>
      <div className="num" style={{ fontSize: "28px", fontWeight: 700, color: categoria ? categoria.color : "#1C2321" }}>
        {valor}{unidad ? <span style={{ fontSize: "14px", fontWeight: 500 }}> {unidad}</span> : null}
      </div>
      {categoria && (
        <span style={{ display: "inline-block", marginTop: "8px", fontSize: "11px", fontWeight: 700, color: categoria.color, background: categoria.color + "1A", borderRadius: "5px", padding: "3px 9px" }}>
          {categoria.label}
        </span>
      )}
    </div>
  );
}

function ObesidadTab() {
  const [form, setForm] = useState({
    sexo: "mujer",
    peso: 80,
    altura: 165,
    cintura: 95,
    cadera: 105,
    trigliceridos: 150,
    glucosa: 95,
    hdl: 45,
  });
  const [vatArea, setVatArea] = useState("");
  const [agRatio, setAgRatio] = useState("");

  const set = (k) => (e) => setForm({ ...form, [k]: e.target.value });

  const alturaM = (parseFloat(form.altura) || 0) / 100;
  const imc = alturaM > 0 ? (parseFloat(form.peso) || 0) / (alturaM * alturaM) : null;
  const ict = form.altura > 0 ? (parseFloat(form.cintura) || 0) / (parseFloat(form.altura) || 1) : null;
  const icc = form.cadera > 0 ? (parseFloat(form.cintura) || 0) / (parseFloat(form.cadera) || 1) : null;
  const tyg =
    form.trigliceridos && form.glucosa
      ? Math.log((parseFloat(form.trigliceridos) * parseFloat(form.glucosa)) / 2)
      : null;
  const tgHdl = form.hdl > 0 ? (parseFloat(form.trigliceridos) || 0) / (parseFloat(form.hdl) || 1) : null;

  return (
    <div>
      <div style={{ display: "flex", alignItems: "center", gap: "8px", marginBottom: "6px" }}>
        <div style={{ width: "8px", height: "8px", borderRadius: "50%", background: "#B4841F" }} />
        <div style={{ fontFamily: "'Space Grotesk', sans-serif", fontWeight: 600, fontSize: "19px" }}>
          Parámetros de obesidad y adiposidad central
        </div>
      </div>
      <p style={{ color: "#4A544E", fontSize: "13.5px", marginBottom: "22px", maxWidth: "600px", lineHeight: 1.5 }}>
        Antropometría, índices metabólicos derivados de laboratorio, y referencia orientativa de grasa
        visceral por DXA.
      </p>

      {/* Formulario antropometría */}
      <div style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "14px", padding: "24px", marginBottom: "16px" }}>
        <div className="eyebrow" style={{ marginBottom: "16px" }}>Antropometría</div>
        <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr", gap: "16px" }} className="grid-cols-resp">
          <Field label="Sexo biológico">
            <select value={form.sexo} onChange={set("sexo")} style={selectStyle}>
              <option value="mujer">Mujer</option>
              <option value="hombre">Hombre</option>
            </select>
          </Field>
          <Field label="Peso (kg)">
            <input type="number" value={form.peso} onChange={set("peso")} style={inputStyle} />
          </Field>
          <Field label="Altura (cm)">
            <input type="number" value={form.altura} onChange={set("altura")} style={inputStyle} />
          </Field>
          <Field label="Circunferencia de cintura (cm)">
            <input type="number" value={form.cintura} onChange={set("cintura")} style={inputStyle} />
          </Field>
          <Field label="Circunferencia de cadera (cm)">
            <input type="number" value={form.cadera} onChange={set("cadera")} style={inputStyle} />
          </Field>
        </div>
      </div>

      <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr 1fr", gap: "12px", marginBottom: "24px" }} className="grid-cols-resp">
        <ResultCard titulo="IMC" valor={imc ? imc.toFixed(1) : "—"} unidad="kg/m²" categoria={imc ? categoriaIMC(imc) : null} />
        <ResultCard titulo="Índice cintura/talla" valor={ict ? ict.toFixed(2) : "—"} categoria={ict ? categoriaICT(ict) : null} />
        <ResultCard titulo="Índice cintura/cadera" valor={icc ? icc.toFixed(2) : "—"} categoria={icc ? categoriaICC(icc, form.sexo) : null} />
      </div>

      {/* Formulario índices metabólicos */}
      <div style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "14px", padding: "24px", marginBottom: "16px" }}>
        <div className="eyebrow" style={{ marginBottom: "16px" }}>Índices metabólicos (laboratorio en ayunas)</div>
        <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr 1fr", gap: "16px" }} className="grid-cols-resp">
          <Field label="Triglicéridos (mg/dL)">
            <input type="number" value={form.trigliceridos} onChange={set("trigliceridos")} style={inputStyle} />
          </Field>
          <Field label="Glucosa (mg/dL)">
            <input type="number" value={form.glucosa} onChange={set("glucosa")} style={inputStyle} />
          </Field>
          <Field label="HDL (mg/dL)">
            <input type="number" value={form.hdl} onChange={set("hdl")} style={inputStyle} />
          </Field>
        </div>
      </div>

      <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr", gap: "12px", marginBottom: "10px" }} className="grid-cols-resp">
        <ResultCard titulo="Índice TyG" valor={tyg ? tyg.toFixed(2) : "—"} categoria={null} />
        <ResultCard titulo="TG / HDL" valor={tgHdl ? tgHdl.toFixed(2) : "—"} categoria={tgHdl ? categoriaTGHDL(tgHdl) : null} />
      </div>
      <div style={{ fontSize: "12px", color: "#6B7A72", marginBottom: "24px", lineHeight: 1.5 }}>
        <strong style={{ color: "#4A544E" }}>Sobre el índice TyG:</strong> fórmula Ln[triglicéridos(mg/dL) × glucosa(mg/dL) / 2]. No tiene un punto de corte único validado — distintos estudios reportan umbrales de insulinorresistencia entre 8.3 y 9.0 según la población. Se muestra el valor sin categorizar por esa razón; interpretalo en conjunto con el cuadro clínico.
      </div>

      {/* DXA */}
      <div style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "14px", padding: "24px", marginBottom: "16px" }}>
        <div className="eyebrow" style={{ marginBottom: "16px" }}>DXA — grasa visceral y adiposidad central (referencia orientativa)</div>

        <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr", gap: "16px", marginBottom: "18px" }} className="grid-cols-resp">
          <Field label="Área de grasa visceral — VAT (cm²)">
            <input type="number" placeholder="ej: 120" value={vatArea} onChange={(e) => setVatArea(e.target.value)} style={inputStyle} />
          </Field>
          <Field label="Relación androide/ginoide (A/G)">
            <input type="number" step="0.01" placeholder="ej: 1.05" value={agRatio} onChange={(e) => setAgRatio(e.target.value)} style={inputStyle} />
          </Field>
        </div>

        {vatArea !== "" && (
          <div style={{ marginBottom: "14px" }}>
            <ResultCard titulo="Interpretación VAT" valor={parseFloat(vatArea).toFixed(0)} unidad="cm²" categoria={categoriaVAT(parseFloat(vatArea))} />
          </div>
        )}
        {agRatio !== "" && (
          <div style={{ fontSize: "13px", color: "#3A423E", background: "#FAF9F5", border: "1px solid #E4E1D6", borderRadius: "10px", padding: "12px 14px", marginBottom: "14px" }}>
            Relación A/G = <strong className="num">{parseFloat(agRatio).toFixed(2)}</strong>.{" "}
            {parseFloat(agRatio) >= 1.0
              ? "Valores ≥1.0 sugieren un patrón de distribución de grasa androide/central, asociado a mayor riesgo cardiometabólico."
              : "Valor por debajo de 1.0 — patrón de distribución más ginoide (periférico)."}{" "}
            No existe un punto de corte único estandarizado entre fabricantes de DXA.
          </div>
        )}

        <div style={{ marginTop: "8px" }}>
          <table style={{ width: "100%", borderCollapse: "collapse", fontSize: "12.5px" }}>
            <thead>
              <tr style={{ borderBottom: "1px solid #E4E1D6" }}>
                <th style={{ textAlign: "left", padding: "8px 6px", color: "#6B7A72", fontWeight: 600 }}>Parámetro DXA</th>
                <th style={{ textAlign: "left", padding: "8px 6px", color: "#6B7A72", fontWeight: 600 }}>Referencia orientativa</th>
              </tr>
            </thead>
            <tbody>
              {[
                ["Área de VAT", "< 100 cm² riesgo bajo · 100–160 cm² riesgo aumentado · > 160 cm² riesgo alto (rangos de distintos estudios de validación, no un corte único)"],
                ["Masa de VAT", "Sin corte universal — depende del software (Hologic APEX / GE CoreScan) y la población; usar siempre el rango de referencia propio del equipo/informe"],
                ["Relación A/G (androide/ginoide)", "Sin corte único estandarizado; valores más altos (aprox. ≥1.0) se asocian a mayor riesgo cardiometabólico, sobre todo en mujeres posmenopáusicas"],
                ["% grasa corporal total — hombres", "Esencial 2–5% · Atlético 6–13% · Fitness 14–17% · Promedio 18–24% · Obesidad ≥25%"],
                ["% grasa corporal total — mujeres", "Esencial 10–13% · Atlético 14–20% · Fitness 21–24% · Promedio 25–31% · Obesidad ≥32%"],
              ].map((row, i) => (
                <tr key={i} style={{ borderBottom: "1px solid #F0EEE6" }}>
                  <td style={{ padding: "9px 6px", fontWeight: 600 }}>{row[0]}</td>
                  <td style={{ padding: "9px 6px", color: "#4A544E" }}>{row[1]}</td>
                </tr>
              ))}
            </tbody>
          </table>
        </div>
      </div>

      <Disclaimer texto="Los valores de grasa visceral (VAT) por DXA dependen del equipo, el software (Hologic APEX/CoreScan, GE Lunar) y la población de referencia usada para calibrarlo — no existe un punto de corte único aceptado universalmente, a diferencia de lo que ocurre con el IMC. Priorizá siempre el rango de referencia que trae el informe de tu propio equipo. Los índices cintura/talla y cintura/cadera son complementarios al IMC, no sustitutos, especialmente útiles para detectar riesgo cardiometabólico en personas con IMC normal (obesidad de peso normal)." />
    </div>
  );
}
/* ============================================================
   MÓDULO 9 — NÓDULO TIROIDEO: TI-RADS (ACR 2017) Y PATRONES ATA (2015)
   ============================================================ */
const TIRADS_CATEGORIAS = {
  composicion: {
    label: "Composición",
    opciones: [
      { label: "Quístico o casi completamente quístico", pts: 0 },
      { label: "Espongiforme", pts: 0 },
      { label: "Mixto quístico y sólido", pts: 1 },
      { label: "Sólido o casi completamente sólido", pts: 2 },
      { label: "No se puede determinar", pts: 2 },
    ],
  },
  ecogenicidad: {
    label: "Ecogenicidad",
    opciones: [
      { label: "Anecoico", pts: 0 },
      { label: "Hiperecoico o isoecoico", pts: 1 },
      { label: "Hipoecoico", pts: 2 },
      { label: "Muy hipoecoico", pts: 3 },
      { label: "No se puede determinar", pts: 1 },
    ],
  },
  forma: {
    label: "Forma",
    opciones: [
      { label: "Más ancho que alto", pts: 0 },
      { label: "Más alto que ancho", pts: 3 },
    ],
  },
  margen: {
    label: "Márgenes",
    opciones: [
      { label: "Liso", pts: 0 },
      { label: "Mal definido", pts: 0 },
      { label: "Lobulado o irregular", pts: 2 },
      { label: "Extensión extratiroidea", pts: 3 },
    ],
  },
};

const TIRADS_FOCOS = [
  { label: "Ninguno, o artefactos en cola de cometa grandes", pts: 0 },
  { label: "Macrocalcificaciones", pts: 1 },
  { label: "Calcificaciones periféricas (en anillo)", pts: 2 },
  { label: "Focos ecogénicos puntiformes", pts: 3 },
];

function categoriaTIRADS(total) {
  if (total === 0) return { nivel: "TR1", label: "Benigno", color: "#3F7D6E", umbralPAAF: null, umbralSeguimiento: null };
  if (total === 2) return { nivel: "TR2", label: "No sospechoso", color: "#3F7D6E", umbralPAAF: null, umbralSeguimiento: null };
  if (total === 3) return { nivel: "TR3", label: "Levemente sospechoso", color: "#B4841F", umbralPAAF: 2.5, umbralSeguimiento: 1.5 };
  if (total >= 4 && total <= 6) return { nivel: "TR4", label: "Moderadamente sospechoso", color: "#B4841F", umbralPAAF: 1.5, umbralSeguimiento: 1.0 };
  return { nivel: "TR5", label: "Altamente sospechoso", color: "#A2483A", umbralPAAF: 1.0, umbralSeguimiento: 0.5 };
}

function recomendacionPorUmbral(tamanioCm, umbralPAAF, umbralSeguimiento) {
  if (umbralPAAF == null) return "No se recomienda PAAF por tamaño en esta categoría.";
  if (tamanioCm >= umbralPAAF) return `PAAF recomendada (nódulo ≥ ${umbralPAAF} cm).`;
  if (umbralSeguimiento != null && tamanioCm >= umbralSeguimiento) return `No requiere PAAF; seguimiento ecográfico (nódulo ≥ ${umbralSeguimiento} cm, < ${umbralPAAF} cm).`;
  return "No requiere PAAF ni seguimiento activo por tamaño.";
}

function TiradsCalculadora() {
  const [sel, setSel] = useState({ composicion: 0, ecogenicidad: 0, forma: 0, margen: 0 });
  const [focos, setFocos] = useState([0]);
  const [tamanio, setTamanio] = useState(1.2);

  const toggleFoco = (idx) => {
    if (idx === 0) { setFocos([0]); return; }
    setFocos((prev) => {
      const sinNinguno = prev.filter((i) => i !== 0);
      return sinNinguno.includes(idx) ? sinNinguno.filter((i) => i !== idx) : [...sinNinguno, idx];
    });
  };

  const totalPts = useMemo(() => {
    let t = 0;
    Object.keys(sel).forEach((cat) => {
      t += TIRADS_CATEGORIAS[cat].opciones[sel[cat]].pts;
    });
    focos.forEach((idx) => { t += TIRADS_FOCOS[idx].pts; });
    return t;
  }, [sel, focos]);

  const cat = categoriaTIRADS(totalPts);
  const recomendacion = recomendacionPorUmbral(parseFloat(tamanio) || 0, cat.umbralPAAF, cat.umbralSeguimiento);

  return (
    <div style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "14px", padding: "24px", marginBottom: "20px" }}>
      <div className="eyebrow" style={{ marginBottom: "16px" }}>ACR TI-RADS (2017) — sistema de puntaje</div>

      {Object.keys(TIRADS_CATEGORIAS).map((cat_key) => (
        <div key={cat_key} style={{ marginBottom: "16px" }}>
          <Field label={TIRADS_CATEGORIAS[cat_key].label}>
            <select
              value={sel[cat_key]}
              onChange={(e) => setSel({ ...sel, [cat_key]: parseInt(e.target.value) })}
              style={selectStyle}
            >
              {TIRADS_CATEGORIAS[cat_key].opciones.map((op, i) => (
                <option key={i} value={i}>{op.label} (+{op.pts})</option>
              ))}
            </select>
          </Field>
        </div>
      ))}

      <div style={{ marginBottom: "16px" }}>
        <label className="eyebrow" style={{ display: "block", marginBottom: "8px" }}>
          Focos ecogénicos (marcar todos los que apliquen)
        </label>
        <div style={{ display: "flex", flexDirection: "column", gap: "6px" }}>
          {TIRADS_FOCOS.map((f, i) => (
            <label key={i} style={{ display: "flex", alignItems: "center", gap: "8px", fontSize: "13px", color: "#3A423E", cursor: "pointer" }}>
              <input type="checkbox" checked={focos.includes(i)} onChange={() => toggleFoco(i)} />
              {f.label} (+{f.pts})
            </label>
          ))}
        </div>
      </div>

      <Field label="Tamaño del nódulo (diámetro mayor, cm)">
        <input type="number" step="0.1" value={tamanio} onChange={(e) => setTamanio(e.target.value)} style={inputStyle} />
      </Field>

      <div style={{ textAlign: "center", padding: "20px 0", marginTop: "16px", borderTop: "1px solid #F0EEE6" }}>
        <div className="eyebrow" style={{ marginBottom: "8px" }}>Puntaje total: {totalPts}</div>
        <div className="num" style={{ fontSize: "34px", fontWeight: 700, color: cat.color }}>{cat.nivel}</div>
        <div style={{ marginTop: "6px" }}>
          <span style={{ fontSize: "12px", fontWeight: 700, color: cat.color, background: cat.color + "1A", borderRadius: "5px", padding: "3px 10px" }}>
            {cat.label}
          </span>
        </div>
        <div style={{ fontSize: "13.5px", color: "#3A423E", maxWidth: "420px", margin: "12px auto 0", fontWeight: 600 }}>
          {recomendacion}
        </div>
      </div>
    </div>
  );
}

const ATA_PATRONES = [
  {
    id: "alta",
    label: "Alta sospecha",
    riesgo: "70–90%",
    color: "#A2483A",
    umbralPAAF: 1.0,
    descripcion: "Nódulo sólido hipoecoico (o componente sólido hipoecoico de un nódulo parcialmente quístico) con ≥1 de: márgenes irregulares, microcalcificaciones, forma más alta que ancha, calcificaciones periféricas con extrusión de tejido blando, extensión extratiroidea.",
  },
  {
    id: "intermedia",
    label: "Sospecha intermedia",
    riesgo: "10–20%",
    color: "#B4841F",
    umbralPAAF: 1.0,
    descripcion: "Nódulo sólido hipoecoico de márgenes lisos, sin microcalcificaciones, extensión extratiroidea ni forma más alta que ancha.",
  },
  {
    id: "baja",
    label: "Baja sospecha",
    riesgo: "5–10%",
    color: "#B4841F",
    umbralPAAF: 1.5,
    descripcion: "Nódulo sólido isoecoico o hiperecoico, o parcialmente quístico con áreas sólidas excéntricas, sin microcalcificaciones, márgenes irregulares, extensión extratiroidea ni forma más alta que ancha.",
  },
  {
    id: "muybaja",
    label: "Muy baja sospecha",
    riesgo: "< 3%",
    color: "#3F7D6E",
    umbralPAAF: 2.0,
    descripcion: "Nódulo espongiforme o parcialmente quístico, sin ninguna de las características sonográficas de los patrones anteriores.",
  },
  {
    id: "benigno",
    label: "Benigno",
    riesgo: "< 1%",
    color: "#3F7D6E",
    umbralPAAF: null,
    descripcion: "Nódulo puramente quístico, sin componente sólido.",
  },
];

function AtaCalculadora() {
  const [patronId, setPatronId] = useState("intermedia");
  const [tamanio, setTamanio] = useState(1.2);
  const patron = ATA_PATRONES.find((p) => p.id === patronId);
  const tamanioNum = parseFloat(tamanio) || 0;

  let recomendacion;
  if (patron.umbralPAAF == null) recomendacion = "No se recomienda PAAF — patrón benigno.";
  else if (tamanioNum >= patron.umbralPAAF) recomendacion = `PAAF recomendada (nódulo ≥ ${patron.umbralPAAF} cm).`;
  else recomendacion = patron.id === "muybaja" ? "Considerar observación sin PAAF, o seguimiento ecográfico." : "No requiere PAAF por tamaño; seguimiento ecográfico.";

  return (
    <div style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "14px", padding: "24px", marginBottom: "20px" }}>
      <div className="eyebrow" style={{ marginBottom: "16px" }}>Patrones ecográficos ATA (2015)</div>

      <div style={{ display: "flex", flexDirection: "column", gap: "8px", marginBottom: "18px" }}>
        {ATA_PATRONES.map((p) => (
          <label
            key={p.id}
            style={{
              display: "flex",
              gap: "10px",
              padding: "12px 14px",
              borderRadius: "10px",
              border: `1px solid ${patronId === p.id ? p.color : "#E4E1D6"}`,
              background: patronId === p.id ? p.color + "0D" : "#FAF9F5",
              cursor: "pointer",
            }}
          >
            <input type="radio" name="ata" checked={patronId === p.id} onChange={() => setPatronId(p.id)} style={{ marginTop: "3px" }} />
            <div>
              <div style={{ display: "flex", alignItems: "center", gap: "8px" }}>
                <span style={{ fontWeight: 700, fontSize: "13.5px" }}>{p.label}</span>
                <span className="num" style={{ fontSize: "11px", fontWeight: 700, color: p.color, background: p.color + "1A", borderRadius: "4px", padding: "2px 7px" }}>
                  {p.riesgo}
                </span>
              </div>
              <div style={{ fontSize: "12px", color: "#4A544E", marginTop: "3px", lineHeight: 1.45 }}>{p.descripcion}</div>
            </div>
          </label>
        ))}
      </div>

      <Field label="Tamaño del nódulo (diámetro mayor, cm)">
        <input type="number" step="0.1" value={tamanio} onChange={(e) => setTamanio(e.target.value)} style={inputStyle} />
      </Field>

      <div style={{ textAlign: "center", padding: "20px 0", marginTop: "16px", borderTop: "1px solid #F0EEE6" }}>
        <div className="eyebrow" style={{ marginBottom: "8px" }}>Patrón seleccionado</div>
        <div className="num" style={{ fontSize: "24px", fontWeight: 700, color: patron.color }}>{patron.label}</div>
        <div style={{ fontSize: "13.5px", color: "#3A423E", maxWidth: "420px", margin: "10px auto 0", fontWeight: 600 }}>
          {recomendacion}
        </div>
      </div>
    </div>
  );
}

/* ============================================================
   ATA 2025 — RIESGO DE RECURRENCIA (reconstrucción a partir de fuentes
   publicadas: Ringel MD, et al. Thyroid 2025;35(8):841-985, y resúmenes
   de Clinical Thyroidology / revisiones especializadas. No es el motor
   de decisión original de ninguna calculadora comercial — ver disclaimer.
   ============================================================ */
function clasificarATA2025(f) {
  const bajoIntermedio = [];
  const intermedioAlto = [];
  const alto = [];

  const esFolicular = f.histologia === "ftc" || f.histologia === "otc";
  const etiquetaHist = f.histologia === "ftc" ? "FTC/IEFVPTC" : f.histologia === "otc" ? "oncocítico (OTC)" : "PTC";

  // Extensión extratiroidea
  if (f.ete === "micro") bajoIntermedio.push("Extensión extratiroidea microscópica (pETE)");
  if (f.ete === "macroLimitada") intermedioAlto.push("Extensión extratiroidea macroscópica limitada a músculos pretiroideos");
  if (f.ete === "macroMayor") alto.push("Extensión extratiroidea macroscópica mayor (más allá de músculos pretiroideos)");

  // Subtipo histológico agresivo / alto grado
  if (f.subtipoAgresivo === "si") intermedioAlto.push("Subtipo histológico agresivo (célula alta, hobnail, columnar, esclerosante difuso)");
  if (f.altoGrado === "si") alto.push("Alto grado / pobremente diferenciado");

  // Invasión vascular
  if (!esFolicular && f.vascularPTC === "presente") bajoIntermedio.push("Invasión vascular presente (PTC)");
  if (esFolicular && f.vascularFTC === "limitada") bajoIntermedio.push(`Invasión vascular limitada (< 4 focos, ${etiquetaHist})`);
  if (esFolicular && f.vascularFTC === "extensa") alto.push(`Invasión vascular extensa (≥ 4 focos, ${etiquetaHist})`);

  // Invasión capsular (relevante en FTC/OTC)
  if (esFolicular && f.invasionCapsular === "amplia") intermedioAlto.push(`Invasión ampliamente invasiva (${etiquetaHist})`);

  // Resección
  if (f.reseccion === "incompleta") alto.push("Resección incompleta (R2 / residuo macroscópico)");

  // Focalidad
  if (f.focalidad === "unilateral" || f.focalidad === "bilateral") bajoIntermedio.push("Enfermedad multifocal");

  // Márgenes
  if (f.margenPositivo === "si") {
    if (f.margenAnterior === "microscopico" || f.margenPosterior === "microscopico") {
      bajoIntermedio.push("Margen quirúrgico microscópicamente positivo (R1)");
    }
    if (f.margenAnterior === "grueso" || f.margenPosterior === "grueso") {
      alto.push("Margen quirúrgico groseramente positivo");
    }
  }

  // Ganglios centrales
  if (f.centralPositivos === "si") {
    if (f.centralNumero === "pocos" && f.centralTamanio === "micro") {
      // N0/Nx equivalente — ≤5 nodos, todos <2mm: no agrega riesgo (bajo)
    } else if (f.centralNumero === "muchos" && f.centralTamanio !== "grande") {
      bajoIntermedio.push("N1a central, > 5 ganglios, volumen pequeño (< 3 cm)");
    } else if (f.centralTamanio === "grande") {
      intermedioAlto.push("N1a central con ganglios de gran tamaño (≥ 3 cm)");
    } else {
      bajoIntermedio.push("N1a central de bajo volumen");
    }
  }

  // Ganglios laterales
  if (f.lateralPositivos === "si") {
    if (f.lateralTamanio === "grande") alto.push("N1b lateral con ganglio ≥ 3 cm");
    else intermedioAlto.push("N1b — metástasis en compartimento lateral");
  }

  // Extensión extranodal
  if (f.ene === "si") alto.push("Extensión extranodal (ENE) presente");

  // Metástasis a distancia
  if (f.m1 === "si") alto.push("Metástasis a distancia (M1)");

  // Tamaño tumoral > 4cm confinado, sin otros factores adversos
  const tam = parseFloat(f.tamanio) || 0;
  if (tam > 4 && f.ete === "ninguna" && bajoIntermedio.length === 0 && intermedioAlto.length === 0 && alto.length === 0) {
    bajoIntermedio.push("Tumor > 4 cm confinado a la tiroides, sin otros factores adversos");
  }

  // Determinación final
  let categoria;
  if (alto.length > 0) categoria = "alto";
  else if (intermedioAlto.length > 0) categoria = "intermedioAlto";
  else if (bajoIntermedio.length >= 2) categoria = "intermedioAlto"; // regla aditiva
  else if (bajoIntermedio.length === 1) categoria = "bajoIntermedio";
  else categoria = "bajo";

  const META = {
    bajo: { label: "Bajo riesgo", color: "#3F7D6E", riesgo: "< 5%" },
    bajoIntermedio: { label: "Bajo-intermedio", color: "#7A9B6E", riesgo: "5–15% (orientativo)" },
    intermedioAlto: { label: "Intermedio-alto", color: "#B4841F", riesgo: "15–30% (orientativo)" },
    alto: { label: "Alto riesgo", color: "#A2483A", riesgo: "≥ 30%" },
  };

  return { categoria, meta: META[categoria], factores: { bajoIntermedio, intermedioAlto, alto } };
}

function Ata2025Calculadora() {
  const [f, setF] = useState({
    histologia: "ptc",
    tamanio: 1.5,
    ete: "ninguna",
    subtipoAgresivo: "no",
    altoGrado: "no",
    vascularPTC: "ausente",
    vascularFTC: "ninguna",
    invasionCapsular: "ninguna",
    reseccion: "completa",
    focalidad: "unifocal",
    margenPositivo: "no",
    margenAnterior: "negativo",
    margenPosterior: "negativo",
    centralPositivos: "no",
    centralNumero: "pocos",
    centralTamanio: "micro",
    lateralPositivos: "no",
    lateralTamanio: "chico",
    ene: "no",
    m1: "no",
  });

  const set = (k) => (e) => setF({ ...f, [k]: e.target.value });
  const resultado = useMemo(() => clasificarATA2025(f), [f]);
  const esFolicular = f.histologia === "ftc" || f.histologia === "otc";

  return (
    <div>
      <div style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "14px", padding: "24px", marginBottom: "16px" }}>
        <div className="eyebrow" style={{ marginBottom: "16px" }}>1 · Histología y tamaño</div>
        <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr", gap: "16px" }} className="grid-cols-resp">
          <Field label="Histología">
            <select value={f.histologia} onChange={set("histologia")} style={selectStyle}>
              <option value="ptc">PTC</option>
              <option value="ftc">FTC / IEFVPTC</option>
              <option value="otc">Oncocítico (OTC)</option>
            </select>
          </Field>
          <Field label="Tamaño tumoral (cm)">
            <input type="number" step="0.1" value={f.tamanio} onChange={set("tamanio")} style={inputStyle} />
          </Field>
        </div>
      </div>

      <div style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "14px", padding: "24px", marginBottom: "16px" }}>
        <div className="eyebrow" style={{ marginBottom: "16px" }}>2 · Características del tumor</div>
        <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr", gap: "16px" }} className="grid-cols-resp">
          <Field label="Extensión extratiroidea (ETE)">
            <select value={f.ete} onChange={set("ete")} style={selectStyle}>
              <option value="ninguna">Ninguna</option>
              <option value="micro">Microscópica</option>
              <option value="macroLimitada">Macroscópica, limitada a músculos pretiroideos</option>
              <option value="macroMayor">Macroscópica mayor</option>
            </select>
          </Field>
          <Field label="Subtipo histológico agresivo">
            <select value={f.subtipoAgresivo} onChange={set("subtipoAgresivo")} style={selectStyle}>
              <option value="no">No</option>
              <option value="si">Sí (célula alta, hobnail, columnar, esclerosante difuso)</option>
            </select>
          </Field>
          <Field label="Alto grado / pobremente diferenciado">
            <select value={f.altoGrado} onChange={set("altoGrado")} style={selectStyle}>
              <option value="no">No</option>
              <option value="si">Sí</option>
            </select>
          </Field>
          {!esFolicular ? (
            <Field label="Invasión vascular (PTC)">
              <select value={f.vascularPTC} onChange={set("vascularPTC")} style={selectStyle}>
                <option value="ausente">Ausente</option>
                <option value="presente">Presente</option>
              </select>
            </Field>
          ) : (
            <>
              <Field label={`Invasión vascular (${f.histologia === "ftc" ? "FTC/IEFVPTC" : "OTC"})`}>
                <select value={f.vascularFTC} onChange={set("vascularFTC")} style={selectStyle}>
                  <option value="ninguna">Ninguna</option>
                  <option value="limitada">Limitada (&lt; 4 focos)</option>
                  <option value="extensa">Extensa (≥ 4 focos)</option>
                </select>
              </Field>
              <Field label="Invasión capsular/tumoral">
                <select value={f.invasionCapsular} onChange={set("invasionCapsular")} style={selectStyle}>
                  <option value="ninguna">Ninguna</option>
                  <option value="minima">Mínimamente invasivo (solo capsular)</option>
                  <option value="amplia">Ampliamente invasivo</option>
                </select>
              </Field>
            </>
          )}
          <Field label="Estado de la resección">
            <select value={f.reseccion} onChange={set("reseccion")} style={selectStyle}>
              <option value="completa">Completa (R0/R1)</option>
              <option value="incompleta">Incompleta (R2/residuo macroscópico)</option>
            </select>
          </Field>
          <Field label="Focalidad">
            <select value={f.focalidad} onChange={set("focalidad")} style={selectStyle}>
              <option value="unifocal">Unifocal</option>
              <option value="unilateral">Multifocal unilateral</option>
              <option value="bilateral">Multifocal bilateral &gt; 1 cm</option>
            </select>
          </Field>
        </div>
      </div>

      <div style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "14px", padding: "24px", marginBottom: "16px" }}>
        <div className="eyebrow" style={{ marginBottom: "16px" }}>3 · Márgenes y ganglios</div>

        <Field label="¿Margen quirúrgico positivo?">
          <select value={f.margenPositivo} onChange={set("margenPositivo")} style={selectStyle}>
            <option value="no">No (negativo)</option>
            <option value="si">Sí</option>
          </select>
        </Field>

        {f.margenPositivo === "si" && (
          <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr", gap: "16px", marginTop: "14px" }} className="grid-cols-resp">
            <Field label="Margen anterior">
              <select value={f.margenAnterior} onChange={set("margenAnterior")} style={selectStyle}>
                <option value="negativo">Negativo</option>
                <option value="microscopico">Microscópico (+)</option>
                <option value="grueso">Grueso (+)</option>
              </select>
            </Field>
            <Field label="Margen posterior">
              <select value={f.margenPosterior} onChange={set("margenPosterior")} style={selectStyle}>
                <option value="negativo">Negativo</option>
                <option value="microscopico">Microscópico (+)</option>
                <option value="grueso">Grueso (+)</option>
              </select>
            </Field>
          </div>
        )}

        <div style={{ borderTop: "1px solid #F0EEE6", marginTop: "18px", paddingTop: "16px" }}>
          <Field label="Ganglios centrales (nivel VI/VII) — ¿positivos?">
            <select value={f.centralPositivos} onChange={set("centralPositivos")} style={selectStyle}>
              <option value="no">Sin participación</option>
              <option value="si">Nodos positivos presentes</option>
            </select>
          </Field>
          {f.centralPositivos === "si" && (
            <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr", gap: "16px", marginTop: "14px" }} className="grid-cols-resp">
              <Field label="Número de nodos">
                <select value={f.centralNumero} onChange={set("centralNumero")} style={selectStyle}>
                  <option value="pocos">≤ 5 nodos</option>
                  <option value="muchos">&gt; 5 nodos</option>
                </select>
              </Field>
              <Field label="Tamaño máximo del nodo">
                <select value={f.centralTamanio} onChange={set("centralTamanio")} style={selectStyle}>
                  <option value="micro">≤ 2 mm</option>
                  <option value="mediano">&gt; 2 mm y &lt; 3 cm</option>
                  <option value="grande">≥ 3 cm</option>
                </select>
              </Field>
            </div>
          )}
        </div>

        <div style={{ borderTop: "1px solid #F0EEE6", marginTop: "18px", paddingTop: "16px" }}>
          <Field label="Ganglios laterales (niveles II-V) — ¿positivos?">
            <select value={f.lateralPositivos} onChange={set("lateralPositivos")} style={selectStyle}>
              <option value="no">Sin participación</option>
              <option value="si">Nodos positivos presentes</option>
            </select>
          </Field>
          {f.lateralPositivos === "si" && (
            <div style={{ marginTop: "14px" }}>
              <Field label="Tamaño máximo del nodo">
                <select value={f.lateralTamanio} onChange={set("lateralTamanio")} style={selectStyle}>
                  <option value="chico">&lt; 3 cm</option>
                  <option value="grande">≥ 3 cm</option>
                </select>
              </Field>
            </div>
          )}
        </div>

        <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr", gap: "16px", marginTop: "18px", paddingTop: "16px", borderTop: "1px solid #F0EEE6" }} className="grid-cols-resp">
          <Field label="Extensión extranodal (ENE)">
            <select value={f.ene} onChange={set("ene")} style={selectStyle}>
              <option value="no">Ausente</option>
              <option value="si">Presente</option>
            </select>
          </Field>
          <Field label="Metástasis a distancia (M1)">
            <select value={f.m1} onChange={set("m1")} style={selectStyle}>
              <option value="no">No</option>
              <option value="si">Sí</option>
            </select>
          </Field>
        </div>
      </div>

      <div style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "14px", padding: "26px 24px", marginBottom: "16px", textAlign: "center" }}>
        <div className="eyebrow" style={{ marginBottom: "10px" }}>Categoría de riesgo de recurrencia — ATA 2025</div>
        <div className="num" style={{ fontSize: "32px", fontWeight: 700, color: resultado.meta.color }}>{resultado.meta.label}</div>
        <div style={{ marginTop: "6px" }}>
          <span className="num" style={{ fontSize: "12px", fontWeight: 700, color: resultado.meta.color, background: resultado.meta.color + "1A", borderRadius: "5px", padding: "3px 10px" }}>
            Riesgo estimado {resultado.meta.riesgo}
          </span>
        </div>

        {["alto", "intermedioAlto", "bajoIntermedio"].map((k) =>
          resultado.factores[k].length > 0 ? (
            <div key={k} style={{ textAlign: "left", maxWidth: "460px", margin: "14px auto 0" }}>
              <div className="eyebrow" style={{ marginBottom: "6px" }}>
                {k === "alto" ? "Factores de alto riesgo" : k === "intermedioAlto" ? "Factores intermedio-alto" : "Factores bajo-intermedio"}
              </div>
              <ul style={{ margin: 0, paddingLeft: "18px" }}>
                {resultado.factores[k].map((t, i) => (
                  <li key={i} style={{ fontSize: "12.5px", color: "#3A423E", marginBottom: "3px" }}>{t}</li>
                ))}
              </ul>
            </div>
          ) : null
        )}
      </div>

      <a
        href="https://tiro.expert/es/ata-2025-risk-of-recurrence-calculator/"
        target="_blank"
        rel="noopener noreferrer"
        style={{
          display: "block",
          textAlign: "center",
          background: "#1C2321",
          color: "#F5F4F0",
          borderRadius: "10px",
          padding: "13px",
          fontWeight: 600,
          fontSize: "14px",
          textDecoration: "none",
          marginBottom: "16px",
        }}
      >
        Contrastar con la calculadora oficial de TIRO ↗
      </a>

      <Disclaimer texto="Este clasificador es una reconstrucción propia a partir de fuentes publicadas sobre la guía ATA 2025 (Ringel MD, et al. Thyroid 2025;35(8):841-985, y resúmenes de revisión especializados) — no es el motor de decisión original de TIRO ni de ningún otro sitio, y puede no capturar cada regla combinatoria exacta de la guía oficial (que incluye matices adicionales, especialmente en la estadificación ganglionar y las reglas aditivas). Usalo como apoyo de estudio y orientación rápida, y contrastá siempre los casos límite o de alto impacto terapéutico (indicación de yodo radioactivo) con la calculadora oficial o el texto completo de la guía." />
    </div>
  );
}


/* ============================================================
   ATA — RIESGO DINÁMICO POSOPERATORIO (Dynamic Risk Stratification)
   Reconstrucción a partir de fuentes publicadas sobre ATA 2015/2016
   (Momesso et al.) y la actualización ATA 2025 — ver disclaimer.
   ============================================================ */
function clasificarRiesgoDinamico(f) {
  const tg = parseFloat(f.tg);
  const tieneTg = !isNaN(tg);

  // 1. Imagen estructural manda por sobre todo
  if (f.imagen === "estructural") {
    return {
      categoria: "estructural",
      label: "Respuesta estructural incompleta",
      color: "#A2483A",
      riesgo: "Persistencia/progresión documentada",
      tsh: "Suprimido (< 0.1 mUI/L), salvo contraindicación",
      detalle: "Enfermedad estructural identificada en imágenes — reevaluar conducta terapéutica activa (cirugía, RAI, terapia sistémica según extensión) con el equipo tratante.",
    };
  }

  // 2. Imagen no específica → indeterminada, salvo marcadores muy alterados
  if (f.imagen === "noespecifico") {
    return {
      categoria: "indeterminada",
      label: "Respuesta indeterminada",
      color: "#B4841F",
      riesgo: "~15–20% de progresión a enfermedad estructural",
      tsh: "Bajo-normal, con seguimiento más cercano",
      detalle: "Hallazgo de imagen no específico (no claramente benigno ni maligno) — reevaluar con imagen dirigida o seguimiento en 6–12 meses.",
    };
  }

  // 3. Imagen negativa → depende de Tg / TgAb / alcance quirúrgico
  const tgAbSubiendo = f.tgAb === "subiendo";
  const tgAbFavorable = f.tgAb === "negativo" || f.tgAb === "estable" || f.tgAb === "caida";

  if (f.alcance === "lobectomia") {
    const favorable = (f.tendenciaTg === "estable" || f.tendenciaTg === "caida") && !tgAbSubiendo;
    if (favorable) {
      return {
        categoria: "excelente",
        label: "Respuesta favorable",
        color: "#3F7D6E",
        riesgo: "Bajo",
        tsh: "Rango normal",
        detalle: "Tras lobectomía no se espera Tg indetectable (queda tejido tiroideo remanente) — se evalúa por tendencia, no por valor absoluto. Tendencia estable o en descenso, sin ascenso de TgAb.",
      };
    }
    return {
      categoria: "bioquimica",
      label: "Respuesta bioquímica incompleta (equivalente)",
      color: "#B4841F",
      riesgo: "Intermedio — requiere seguimiento más cercano",
      tsh: "Bajo-normal",
      detalle: "Tendencia ascendente de Tg y/o TgAb tras lobectomía — considerar imagen dirigida y reevaluar en intervalo corto.",
    };
  }

  // Total con o sin RAI
  const umbral = f.alcance === "totalConRAI" ? (f.estadoTg === "suprimido" ? 0.2 : 1) : 2.5;
  const tgFavorable = tieneTg ? tg <= umbral : true;

  if (tgFavorable && tgAbFavorable) {
    return {
      categoria: "excelente",
      label: "Respuesta excelente",
      color: "#3F7D6E",
      riesgo: "< 1–4% de recurrencia estructural",
      tsh: "Puede relajarse hacia rango normal (o normal-bajo si el riesgo inicial era alto)",
      detalle: `Tg ${f.alcance === "totalConRAI" ? "por debajo del umbral post-ablación" : "por debajo de 2.5 ng/mL (umbral ATA 2025 sin ablación)"}, TgAb favorable, imagen negativa.`,
    };
  }

  return {
    categoria: "bioquimica",
    label: "Respuesta bioquímica incompleta",
    color: "#B4841F",
    riesgo: "~15–20% progresa a enfermedad estructural con el tiempo",
    tsh: "Suprimido-bajo mientras persista la alteración bioquímica",
    detalle: "Tg por encima del umbral esperado y/o TgAb en ascenso, con imagen negativa — intensificar seguimiento bioquímico e imagenológico.",
  };
}

function RiesgoDinamicoCalculadora() {
  const [f, setF] = useState({
    alcance: "totalConRAI",
    tg: "",
    estadoTg: "suprimido",
    tendenciaTg: "estable",
    tgAb: "negativo",
    imagen: "negativo",
  });
  const set = (k) => (e) => setF({ ...f, [k]: e.target.value });
  const r = useMemo(() => clasificarRiesgoDinamico(f), [f]);

  return (
    <div>
      <div style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "14px", padding: "24px", marginBottom: "16px" }}>
        <div className="eyebrow" style={{ marginBottom: "16px" }}>Datos de seguimiento posoperatorio</div>
        <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr", gap: "16px" }} className="grid-cols-resp">
          <Field label="Alcance de la cirugía">
            <select value={f.alcance} onChange={set("alcance")} style={selectStyle}>
              <option value="totalConRAI">Tiroidectomía total + yodo radioactivo</option>
              <option value="totalSinRAI">Tiroidectomía total (sin yodo radioactivo)</option>
              <option value="lobectomia">Lobectomía / hemitiroidectomía</option>
            </select>
          </Field>
          {f.alcance !== "lobectomia" && (
            <>
              <Field label="Tg sérica (ng/mL)">
                <input type="number" step="0.01" placeholder="ej: 0.15" value={f.tg} onChange={set("tg")} style={inputStyle} />
              </Field>
              <Field label="Estado de la Tg">
                <select value={f.estadoTg} onChange={set("estadoTg")} style={selectStyle}>
                  <option value="suprimido">Suprimido (bajo LT4)</option>
                  <option value="estimulado">Estimulado (rhTSH o suspensión hormonal)</option>
                </select>
              </Field>
            </>
          )}
          {f.alcance === "lobectomia" && (
            <Field label="Tendencia de la Tg">
              <select value={f.tendenciaTg} onChange={set("tendenciaTg")} style={selectStyle}>
                <option value="estable">Estable</option>
                <option value="caida">En descenso</option>
                <option value="subiendo">En ascenso</option>
              </select>
            </Field>
          )}
          <Field label="Anticuerpos anti-Tg (TgAb)">
            <select value={f.tgAb} onChange={set("tgAb")} style={selectStyle}>
              <option value="negativo">Negativo</option>
              <option value="estable">Positivo, estable</option>
              <option value="caida">Positivo, en descenso</option>
              <option value="subiendo">Positivo, en ascenso</option>
            </select>
          </Field>
          <Field label="Resultado de imágenes (ecografía/TC/RAI)">
            <select value={f.imagen} onChange={set("imagen")} style={selectStyle}>
              <option value="negativo">Negativo</option>
              <option value="noespecifico">No específico</option>
              <option value="estructural">Estructural (enfermedad identificada)</option>
            </select>
          </Field>
        </div>
      </div>

      <div style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "14px", padding: "26px 24px", marginBottom: "16px", textAlign: "center" }}>
        <div className="eyebrow" style={{ marginBottom: "10px" }}>Categoría de respuesta</div>
        <div className="num" style={{ fontSize: "26px", fontWeight: 700, color: r.color }}>{r.label}</div>
        <div style={{ marginTop: "8px" }}>
          <span className="num" style={{ fontSize: "12px", fontWeight: 700, color: r.color, background: r.color + "1A", borderRadius: "5px", padding: "3px 10px" }}>
            {r.riesgo}
          </span>
        </div>
        <div style={{ fontSize: "13px", color: "#3A423E", maxWidth: "460px", margin: "12px auto 0", lineHeight: 1.5 }}>{r.detalle}</div>
        <div style={{ marginTop: "14px", paddingTop: "14px", borderTop: "1px solid #F0EEE6" }}>
          <span className="eyebrow">Nivel objetivo de TSH sugerido</span>
          <div style={{ fontSize: "13.5px", fontWeight: 600, color: "#1C2321", marginTop: "4px" }}>{r.tsh}</div>
        </div>
      </div>

      <a
        href="https://tiro.expert/es/ata-2025-risk-of-recurrence-calculator/"
        target="_blank"
        rel="noopener noreferrer"
        style={{
          display: "block",
          textAlign: "center",
          background: "#1C2321",
          color: "#F5F4F0",
          borderRadius: "10px",
          padding: "13px",
          fontWeight: 600,
          fontSize: "14px",
          textDecoration: "none",
          marginBottom: "16px",
        }}
      >
        Contrastar con la calculadora oficial de TIRO ↗
      </a>

      <Disclaimer texto="La estratificación de riesgo dinámico integra la respuesta al tratamiento (Tg, TgAb, imágenes) con el riesgo inicial para reclasificar el pronóstico durante el seguimiento — es más predictiva que el riesgo inicial aislado. Esta reconstrucción usa los umbrales generales descritos en fuentes publicadas sobre ATA 2015/2016 y la actualización 2025 (incluyendo el nuevo umbral de Tg de 2.5 ng/mL en pacientes sin ablación); no es el motor exacto de TIRO. Objetivo de TSH sugerido: orientativo, siempre debe ajustarse según el riesgo inicial completo del paciente y la respuesta dinámica combinada, no solo esta única evaluación." />
    </div>
  );
}


function NoduloTab() {
  const [modo, setModo] = useState("tirads");
  return (
    <div>
      <div style={{ display: "flex", alignItems: "center", gap: "8px", marginBottom: "6px" }}>
        <div style={{ width: "8px", height: "8px", borderRadius: "50%", background: "#B4841F" }} />
        <div style={{ fontFamily: "'Space Grotesk', sans-serif", fontWeight: 600, fontSize: "19px" }}>
          Riesgo de malignidad de nódulo tiroideo
        </div>
      </div>
      <p style={{ color: "#4A544E", fontSize: "13.5px", marginBottom: "18px", maxWidth: "600px", lineHeight: 1.5 }}>
        Estratificación ecográfica prequirúrgica (malignidad) y estratificación posquirúrgica
        (recurrencia) — elegí según la etapa clínica en la que estés.
      </p>

      <div className="chips-scroll" style={{ display: "flex", gap: "8px", marginBottom: "20px" }}>
        <div className={`chip ${modo === "tirads" ? "active" : ""}`} onClick={() => setModo("tirads")}>ACR TI-RADS (2017)</div>
        <div className={`chip ${modo === "ata" ? "active" : ""}`} onClick={() => setModo("ata")}>Patrones ATA (2015)</div>
        <div className={`chip ${modo === "ata2025" ? "active" : ""}`} onClick={() => setModo("ata2025")}>Riesgo de recurrencia — ATA 2025</div>
        <div className={`chip ${modo === "dinamico" ? "active" : ""}`} onClick={() => setModo("dinamico")}>Riesgo dinámico (posoperatorio)</div>
      </div>

      {modo === "tirads" && <TiradsCalculadora />}
      {modo === "ata" && <AtaCalculadora />}
      {modo === "ata2025" && <Ata2025Calculadora />}
      {modo === "dinamico" && <RiesgoDinamicoCalculadora />}

      {(modo === "tirads" || modo === "ata") && (
        <Disclaimer texto="TI-RADS y ATA son sistemas de estratificación ecográfica concordantes en la mayoría de los casos, pero no idénticos — usá el que corresponda al informe que tenés, y priorizá siempre la descripción del operador que realizó la ecografía por sobre esta herramienta. Ninguno de los dos sistemas diagnostica malignidad: solo estratifican el riesgo para decidir si está indicada la PAAF. El resultado citológico (sistema Bethesda) sigue siendo el paso siguiente para la conducta definitiva." />
      )}
    </div>
  );
}

/* ============================================================
   MÓDULO 10 — FUNCIÓN RENAL: CKD-EPI 2021 Y COCKCROFT-GAULT
   ============================================================ */
function calcularCKDEPI(sexo, edad, creatinina) {
  const scr = parseFloat(creatinina);
  const age = parseFloat(edad);
  if (!scr || !age || scr <= 0 || age <= 0) return null;

  let egfr;
  if (sexo === "mujer") {
    const k = 0.7;
    const alpha = scr <= k ? -0.241 : -1.200;
    egfr = 142 * Math.pow(scr / k, alpha) * Math.pow(0.9938, age) * 1.012;
  } else {
    const k = 0.9;
    const alpha = scr <= k ? -0.302 : -1.200;
    egfr = 142 * Math.pow(scr / k, alpha) * Math.pow(0.9938, age);
  }
  return egfr;
}

function categoriaCKD(egfr) {
  if (egfr >= 90) return { nivel: "G1", label: "Normal o alto", color: "#3F7D6E" };
  if (egfr >= 60) return { nivel: "G2", label: "Levemente disminuido", color: "#3F7D6E" };
  if (egfr >= 45) return { nivel: "G3a", label: "Leve a moderadamente disminuido", color: "#B4841F" };
  if (egfr >= 30) return { nivel: "G3b", label: "Moderada a severamente disminuido", color: "#B4841F" };
  if (egfr >= 15) return { nivel: "G4", label: "Severamente disminuido", color: "#A2483A" };
  return { nivel: "G5", label: "Falla renal", color: "#A2483A" };
}

function calcularCockcroftGault(sexo, edad, peso, creatinina) {
  const scr = parseFloat(creatinina);
  const age = parseFloat(edad);
  const w = parseFloat(peso);
  if (!scr || !age || !w || scr <= 0 || age <= 0 || w <= 0) return null;
  let crcl = ((140 - age) * w) / (72 * scr);
  if (sexo === "mujer") crcl *= 0.85;
  return crcl;
}

function RenalTab() {
  const [sexo, setSexo] = useState("mujer");
  const [edad, setEdad] = useState(55);
  const [peso, setPeso] = useState(70);
  const [creatinina, setCreatinina] = useState(0.9);

  const egfr = useMemo(() => calcularCKDEPI(sexo, edad, creatinina), [sexo, edad, creatinina]);
  const crcl = useMemo(() => calcularCockcroftGault(sexo, edad, peso, creatinina), [sexo, edad, peso, creatinina]);
  const cat = egfr != null ? categoriaCKD(egfr) : null;

  return (
    <div>
      <div style={{ display: "flex", alignItems: "center", gap: "8px", marginBottom: "6px" }}>
        <div style={{ width: "8px", height: "8px", borderRadius: "50%", background: "#4A6FA5" }} />
        <div style={{ fontFamily: "'Space Grotesk', sans-serif", fontWeight: 600, fontSize: "19px" }}>
          Función renal
        </div>
      </div>
      <p style={{ color: "#4A544E", fontSize: "13.5px", marginBottom: "18px", maxWidth: "620px", lineHeight: 1.5 }}>
        <strong>Aclaración terminológica:</strong> CKD-EPI estima la <em>tasa de filtrado glomerular</em> (eGFR),
        no el clearance de creatinina propiamente dicho — es la fórmula recomendada actualmente para
        estadificar función renal. Si necesitás el clearance de creatinina clásico (por ejemplo, para
        ajuste de dosis de algunos fármacos), usá Cockcroft-Gault, que también incluyo abajo.
      </p>

      <div style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "14px", padding: "24px", marginBottom: "20px" }}>
        <div className="eyebrow" style={{ marginBottom: "16px" }}>Datos del paciente</div>
        <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr", gap: "16px" }} className="grid-cols-resp">
          <Field label="Sexo biológico">
            <select value={sexo} onChange={(e) => setSexo(e.target.value)} style={selectStyle}>
              <option value="mujer">Mujer</option>
              <option value="hombre">Hombre</option>
            </select>
          </Field>
          <Field label="Edad (años)">
            <input type="number" value={edad} onChange={(e) => setEdad(e.target.value)} style={inputStyle} />
          </Field>
          <Field label="Peso (kg) — solo para Cockcroft-Gault">
            <input type="number" value={peso} onChange={(e) => setPeso(e.target.value)} style={inputStyle} />
          </Field>
          <Field label="Creatinina sérica (mg/dL)">
            <input type="number" step="0.01" value={creatinina} onChange={(e) => setCreatinina(e.target.value)} style={inputStyle} />
          </Field>
        </div>
      </div>

      <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr", gap: "16px", marginBottom: "20px" }} className="grid-cols-resp">
        <div style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "14px", padding: "24px", textAlign: "center" }}>
          <div className="eyebrow" style={{ marginBottom: "10px" }}>CKD-EPI 2021 (eGFR)</div>
          <div className="num" style={{ fontSize: "34px", fontWeight: 700, color: cat ? cat.color : "#1C2321" }}>
            {egfr != null ? egfr.toFixed(0) : "—"}
          </div>
          <div style={{ fontSize: "12px", color: "#6B7A72" }}>mL/min/1.73m²</div>
          {cat && (
            <div style={{ marginTop: "10px" }}>
              <span style={{ fontSize: "12px", fontWeight: 700, color: cat.color, background: cat.color + "1A", borderRadius: "5px", padding: "3px 10px" }}>
                {cat.nivel} — {cat.label}
              </span>
            </div>
          )}
        </div>
        <div style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "14px", padding: "24px", textAlign: "center" }}>
          <div className="eyebrow" style={{ marginBottom: "10px" }}>Cockcroft-Gault (CrCl)</div>
          <div className="num" style={{ fontSize: "34px", fontWeight: 700, color: "#1C2321" }}>
            {crcl != null ? crcl.toFixed(0) : "—"}
          </div>
          <div style={{ fontSize: "12px", color: "#6B7A72" }}>mL/min</div>
          <div style={{ fontSize: "11px", color: "#8A9089", marginTop: "10px" }}>
            Usa peso corporal real — considerar peso ideal/ajustado en obesidad
          </div>
        </div>
      </div>

      {/* Tabla de estadios KDIGO */}
      <div style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "14px", padding: "22px 24px", marginBottom: "20px" }}>
        <div className="eyebrow" style={{ marginBottom: "14px" }}>Estadios de enfermedad renal crónica (KDIGO)</div>
        {[
          { nivel: "G1", rango: "≥ 90", label: "Normal o alto", color: "#3F7D6E" },
          { nivel: "G2", rango: "60 – 89", label: "Levemente disminuido", color: "#3F7D6E" },
          { nivel: "G3a", rango: "45 – 59", label: "Leve a moderadamente disminuido", color: "#B4841F" },
          { nivel: "G3b", rango: "30 – 44", label: "Moderada a severamente disminuido", color: "#B4841F" },
          { nivel: "G4", rango: "15 – 29", label: "Severamente disminuido", color: "#A2483A" },
          { nivel: "G5", rango: "< 15", label: "Falla renal", color: "#A2483A" },
        ].map((r, i) => (
          <div key={i} style={{ display: "grid", gridTemplateColumns: "0.6fr 0.8fr 2fr", gap: "12px", padding: "9px 0", borderBottom: i < 5 ? "1px solid #F0EEE6" : "none", alignItems: "center" }}>
            <span style={{ fontSize: "11px", fontWeight: 700, color: r.color, background: r.color + "1A", borderRadius: "4px", padding: "2px 8px", width: "fit-content" }}>{r.nivel}</span>
            <div className="num" style={{ fontSize: "13px", fontWeight: 600 }}>{r.rango} mL/min/1.73m²</div>
            <div style={{ fontSize: "12.5px", color: "#4A544E" }}>{r.label}</div>
          </div>
        ))}
      </div>

      <Disclaimer texto="CKD-EPI 2021 (ecuación basada en creatinina, sin variable de raza) es la fórmula recomendada actualmente por KDIGO para estimar la tasa de filtrado glomerular en la práctica clínica general. Cockcroft-Gault sigue usándose en algunos protocolos de ajuste de dosis de fármacos por su validación histórica, pero tiende a sobreestimar el clearance en personas con obesidad si se usa el peso real sin ajustar. Ambas fórmulas requieren una creatinina en estado estable (no válidas en injuria renal aguda). Confirmar con la función renal medida (clearance con orina de 24 h) ante discrepancias clínicas relevantes." />
    </div>
  );
}

/* ============================================================
   MÓDULO 11 — INTERACCIONES FARMACOLÓGICAS Y AJUSTES RENAL/HEPÁTICO
   ============================================================ */
const FARMACOS_CATEGORIAS = [
  {
    id: "antidiabeticos",
    nombre: "Antidiabéticos orales e inyectables",
    color: "#4A6FA5",
    items: [
      {
        farmaco: "Metformina",
        renal: "eGFR 45–59: sin restricción. eGFR 30–44: reducir dosis (máx. ~1000 mg/día) y monitorear más seguido. eGFR < 30: contraindicada.",
        hepatica: "Evitar en insuficiencia hepática significativa — riesgo de acidosis láctica.",
        interacciones: "Suspender transitoriamente con contraste yodado IV si eGFR < 60. Alcohol potencia el riesgo de acidosis láctica. Cimetidina aumenta sus niveles plasmáticos.",
        adversos: "Diarrea, náuseas, sabor metálico (frecuentes, dependientes de dosis). Déficit de vitamina B12 con uso crónico. Acidosis láctica (rara, pero grave).",
      },
      {
        farmaco: "Glibenclamida",
        renal: "Evitar si eGFR < 60 — sus metabolitos activos se acumulan, alto riesgo de hipoglucemia prolongada.",
        hepatica: "Evitar en insuficiencia hepática.",
        interacciones: "Potencia hipoglucemia con warfarina, fluoroquinolonas, sulfonamidas, alcohol, azoles y fibratos.",
        adversos: "Hipoglucemia (la más frecuente y prolongada de las sulfonilureas), aumento de peso.",
      },
      {
        farmaco: "Glimepirida / Gliclazida",
        renal: "Usar con precaución, iniciar con dosis bajas si hay deterioro renal; gliclazida es algo más segura que glibenclamida en este contexto.",
        hepatica: "Evitar en insuficiencia hepática severa.",
        interacciones: "Similares a glibenclamida — potencian hipoglucemia con alcohol, azoles, fibratos.",
        adversos: "Hipoglucemia (menos prolongada que glibenclamida), aumento de peso.",
      },
      {
        farmaco: "Empagliflozina",
        renal: "10 mg/día, se puede subir a 25 mg/día. No iniciar con eGFR < 20. Dentro del rango permitido, no requiere ajuste de dosis (misma dosis independientemente del eGFR).",
        hepatica: "Sin ajuste en insuficiencia leve, moderada ni severa (datos limitados en severa — usar con precaución).",
        interacciones: "Potencia hipoglucemia si se combina con insulina o sulfonilureas. Diuréticos aumentan el riesgo de depleción de volumen/hipotensión.",
        adversos: "Infecciones micóticas genitales, ITU, poliuria, depleción de volumen/hipotensión, cetoacidosis euglucémica (rara pero grave — sospechar aunque la glucemia sea normal).",
      },
      {
        farmaco: "Dapagliflozina",
        renal: "10 mg/día (dosis única, sin escalado). No iniciar con eGFR < 25 para indicación glucémica; puede continuarse con eGFR más bajo para indicación renal/cardíaca específica según ficha técnica.",
        hepatica: "Sin ajuste en insuficiencia leve-moderada. En severa, considerar dosis inicial menor y monitorear.",
        interacciones: "Igual que empagliflozina — potencia hipoglucemia con insulina/sulfonilureas; diuréticos aumentan riesgo de depleción de volumen.",
        adversos: "Igual que empagliflozina: infecciones micóticas genitales, ITU, depleción de volumen, cetoacidosis euglucémica (rara).",
      },
      {
        farmaco: "Canagliflozina",
        renal: "100 mg/día inicial, se puede subir a 300 mg/día si eGFR ≥ 60. Con eGFR 30–59: máximo 100 mg/día (no escalar a 300). No iniciar con eGFR < 30.",
        hepatica: "Sin ajuste en insuficiencia leve-moderada. No recomendada en insuficiencia hepática severa (datos limitados).",
        interacciones: "Igual que el resto de la clase — potencia hipoglucemia con insulina/sulfonilureas; diuréticos aumentan riesgo de hipotensión.",
        adversos: "Además de los efectos de clase (micóticas genitales, ITU, depleción de volumen, cetoacidosis euglucémica): señal específica de mayor riesgo de amputación de miembros inferiores y de fractura — tener en cuenta en pacientes con enfermedad vascular periférica u osteoporosis.",
      },
      {
        farmaco: "Liraglutida / Semaglutida / Dulaglutida (GLP-1)",
        renal: "Sin ajuste de dosis necesario en la mayoría de los grados de deterioro renal.",
        hepatica: "Sin ajuste mayor descrito; datos limitados en insuficiencia hepática severa.",
        interacciones: "El retraso del vaciamiento gástrico puede alterar la absorción de otros fármacos orales tomados simultáneamente.",
        adversos: "Náuseas, vómitos y diarrea (frecuentes, sobre todo al inicio o al escalar dosis). Pancreatitis (rara). Contraindicados si antecedente personal/familiar de carcinoma medular de tiroides o MEN2 (señal en modelos animales).",
      },
      {
        farmaco: "Exenatida",
        renal: "Evitar si eGFR < 30 (a diferencia de otros GLP-1, sí tiene eliminación renal relevante).",
        hepatica: "Sin ajuste mayor descrito.",
        interacciones: "Igual que otros GLP-1 — puede alterar absorción de fármacos orales por enlentecimiento del vaciamiento gástrico.",
        adversos: "Náuseas, vómitos, diarrea; pancreatitis (rara); reacciones en el sitio de inyección más frecuentes que con otros GLP-1.",
      },
      {
        farmaco: "Sitagliptina",
        renal: "100 mg/día con eGFR ≥ 60. eGFR 45–59: 50 mg/día. eGFR < 45 (incluye diálisis): 25 mg/día.",
        hepatica: "Sin ajuste en insuficiencia leve-moderada (Child-Pugh A/B); sin datos suficientes en severa.",
        interacciones: "Pocas interacciones mayores; potencia hipoglucemia si se combina con sulfonilureas o insulina.",
        adversos: "Nasofaringitis, cefalea. Pancreatitis (rara). Artralgia severa (descrita como efecto de clase). Penfigoide ampolloso (raro).",
      },
      {
        farmaco: "Vildagliptina",
        renal: "50 mg cada 12 h (100 mg/día) con eGFR ≥ 50. Con eGFR < 50 (incluye diálisis): 50 mg una vez al día.",
        hepatica: "No recomendada en ningún grado de insuficiencia hepática, incluida la leve — riesgo de hepatotoxicidad; controlar transaminasas antes de iniciar y periódicamente durante el primer año.",
        interacciones: "Pocas interacciones mayores; potencia hipoglucemia con sulfonilureas.",
        adversos: "Nasofaringitis, mareos. Elevación de transaminasas/hepatotoxicidad (la vigilancia hepática es más estricta que en otros iDPP4). Angioedema (poco frecuente).",
      },
      {
        farmaco: "Saxagliptina",
        renal: "5 mg/día con eGFR > 45. Con eGFR ≤ 45 (incluye diálisis): 2.5 mg/día.",
        hepatica: "Sin ajuste en insuficiencia leve-moderada; usar con precaución en severa (datos limitados).",
        interacciones: "Pocas interacciones mayores; potencia hipoglucemia con sulfonilureas.",
        adversos: "Nasofaringitis, cefalea. Señal de mayor riesgo de hospitalización por insuficiencia cardíaca (estudio SAVOR-TIMI) — precaución en pacientes con IC.",
      },
      {
        farmaco: "Linagliptina",
        renal: "5 mg/día — no requiere ajuste en ningún grado de insuficiencia renal (eliminación predominantemente biliar/entérica, no renal).",
        hepatica: "Sin ajuste mayor en ningún grado de insuficiencia hepática.",
        interacciones: "Pocas interacciones relevantes; potencia hipoglucemia con sulfonilureas.",
        adversos: "Nasofaringitis, tos. Pancreatitis (rara). Es el iDPP4 de elección cuando hay deterioro renal/hepático significativo, precisamente por no requerir ajuste.",
      },
      {
        farmaco: "Pioglitazona",
        renal: "Sin ajuste mayor por función renal.",
        hepatica: "Contraindicada en enfermedad hepática activa — monitorear transaminasas periódicamente.",
        interacciones: "Contraindicada en insuficiencia cardíaca (retención de líquidos). Gemfibrozilo aumenta sus niveles plasmáticos.",
        adversos: "Retención de líquidos/edema, aumento de peso, mayor riesgo de fracturas (sobre todo en mujeres), posible asociación con cáncer de vejiga (controvertida), puede precipitar insuficiencia cardíaca.",
      },
      {
        farmaco: "Insulina (todas las formas)",
        renal: "Reducir dosis con eGFR < 30–45 — menor clearance y degradación renal de insulina, mayor riesgo de hipoglucemia.",
        hepatica: "Reducir dosis en insuficiencia hepática significativa — menor gluconeogénesis hepática.",
        interacciones: "Alcohol, salicilatos e IECA potencian la hipoglucemia. Corticoides y diuréticos tiazídicos aumentan el requerimiento de insulina.",
        adversos: "Hipoglucemia (el más frecuente y relevante), aumento de peso, lipodistrofia en los sitios de inyección con uso prolongado sin rotación.",
      },
    ],
  },
  {
    id: "tiroideos",
    nombre: "Tiroideos",
    color: "#3F7D6E",
    items: [
      {
        farmaco: "Levotiroxina",
        renal: "Sin ajuste de dosis por función renal en general.",
        hepatica: "Sin ajuste mayor, aunque la enfermedad hepática puede alterar las proteínas transportadoras de hormona tiroidea.",
        interacciones: "Absorción reducida por calcio, hierro, IBP, sucralfato y colestiramina — separar la toma por ≥ 4 h. Metabolismo aumentado por rifampicina, fenitoína y carbamazepina (puede requerir aumentar la dosis).",
        adversos: "Los del sobrereemplazo: palpitaciones, insomnio, temblor, pérdida de peso; con exceso mantenido en el tiempo, mayor riesgo de fibrilación auricular y pérdida de masa ósea.",
      },
      {
        farmaco: "Metimazol",
        renal: "Sin ajuste mayor por función renal.",
        hepatica: "Usar dosis bajas y monitorear en insuficiencia hepática — hepatotoxicidad colestásica infrecuente pero descrita.",
        interacciones: "Potencia el efecto anticoagulante de warfarina.",
        adversos: "Rash, prurito. Agranulocitosis (rara pero grave — advertir al paciente que consulte de inmediato ante fiebre u odinofagia). Hepatotoxicidad colestásica. Vasculitis ANCA-positiva (rara).",
      },
      {
        farmaco: "Propiltiouracilo",
        renal: "Sin ajuste mayor por función renal.",
        hepatica: "Evitar — riesgo de hepatotoxicidad grave (incluye alerta de caja negra); reservar para primer trimestre de embarazo o intolerancia a metimazol.",
        interacciones: "Similar a metimazol — potencia el efecto de warfarina.",
        adversos: "Hepatotoxicidad grave, incluida falla hepática fulminante (el riesgo más relevante de este fármaco). Agranulocitosis. Vasculitis ANCA-positiva.",
      },
    ],
  },
  {
    id: "corticoides",
    nombre: "Corticoides",
    color: "#A2483A",
    items: [
      {
        farmaco: "Prednisona / Metilprednisolona",
        renal: "Sin ajuste mayor por función renal.",
        hepatica: "En insuficiencia hepática severa, la prednisona (profármaco) tiene conversión hepática reducida a prednisolona — preferir prednisolona directamente.",
        interacciones: "Rifampicina, fenitoína y carbamazepina reducen su efecto (inducción CYP3A4). Azoles, macrólidos e inhibidores de proteasa aumentan su efecto. AINEs aumentan el riesgo de sangrado digestivo. Diuréticos potencian la hipopotasemia.",
        adversos: "Hiperglucemia, hipertensión, osteoporosis, insuficiencia suprarrenal si se suspende abruptamente tras uso prolongado, aumento de peso, cambios de humor, mayor riesgo de infecciones, cataratas y glaucoma con uso crónico.",
      },
      {
        farmaco: "Hidrocortisona",
        renal: "Sin ajuste mayor por función renal.",
        hepatica: "No requiere conversión hepática (es la forma activa) — preferible en insuficiencia hepática severa sobre prednisona.",
        interacciones: "Similares a otros corticoides — inductores/inhibidores de CYP3A4, AINEs, diuréticos.",
        adversos: "Similares a prednisona, aunque con menor potencia relativa por dosis — igualmente relevante en dosis suprafisiológicas prolongadas.",
      },
    ],
  },
  {
    id: "oseos",
    nombre: "Osteoporosis",
    color: "#6B5B95",
    items: [
      {
        farmaco: "Bifosfonatos orales (alendronato, risedronato)",
        renal: "Contraindicados si eGFR < 30–35 (varía según el agente).",
        hepatica: "Sin ajuste — no tienen metabolismo hepático significativo.",
        interacciones: "Absorción muy reducida por calcio, hierro, antiácidos y alimentos — tomar en ayunas, separar 30–60 min de cualquier ingesta.",
        adversos: "Esofagitis/pirosis (mantener posición erguida 30 min tras la toma). Osteonecrosis de mandíbula (rara). Fractura atípica de fémur (con uso prolongado, > 5 años).",
      },
      {
        farmaco: "Ácido zoledrónico (IV)",
        renal: "Contraindicado si eGFR < 35. Ajustar tiempo de infusión y controlar función renal antes de cada dosis.",
        hepatica: "Sin ajuste mayor.",
        interacciones: "Aminoglucósidos aumentan el riesgo de hipocalcemia.",
        adversos: "Síndrome pseudogripal post-infusión (frecuente en la primera dosis, autolimitado). Hipocalcemia. Osteonecrosis de mandíbula (rara). Deterioro agudo de función renal (raro, más frecuente si hay deshidratación previa).",
      },
      {
        farmaco: "Denosumab",
        renal: "Puede usarse en ERC avanzada (no depende de excreción renal), pero con mayor riesgo de hipocalcemia severa cuando el eGFR es muy bajo — monitorear calcemia de cerca.",
        hepatica: "Sin ajuste descrito.",
        interacciones: "Pocas interacciones mayores; asegurar siempre suplementación de calcio y vitamina D concomitante.",
        adversos: "Hipocalcemia (más marcada que con bifosfonatos, especialmente en ERC). Riesgo de fracturas vertebrales múltiples por rebote si se suspende sin terapia de transición. Osteonecrosis de mandíbula e infecciones cutáneas (raras).",
      },
      {
        farmaco: "Teriparatida / Abaloparatida",
        renal: "Evitar en insuficiencia renal severa.",
        hepatica: "Sin ajuste mayor descrito.",
        interacciones: "Pocas interacciones mayores relevantes.",
        adversos: "Hipercalcemia leve transitoria, mareos, calambres en piernas. Riesgo teórico de osteosarcoma (visto en ratas a dosis altas, no confirmado en humanos — por eso el uso se limita a 2 años).",
      },
    ],
  },
  {
    id: "hipofisosuprarrenal",
    nombre: "Hipofisarios y suprarrenales",
    color: "#8B5A8C",
    items: [
      {
        farmaco: "Análogos de somatostatina (octreotide, lanreotide)",
        renal: "Reducir la dosis de mantenimiento en insuficiencia renal severa — el clearance de octreotide se reduce significativamente.",
        hepatica: "Reducir dosis en cirrosis — octreotide tiene metabolismo hepático relevante, ajustar según respuesta.",
        interacciones: "Puede alterar la absorción de ciclosporina (reducir su nivel) y afectar el control glucémico en pacientes con insulina/hipoglucemiantes (requiere ajuste). Bradicardizantes (betabloqueantes) potencian la bradicardia.",
        adversos: "Síntomas gastrointestinales (dolor abdominal, diarrea, esteatorrea) — muy frecuentes al inicio. Colelitiasis con uso prolongado (mayor riesgo, controlar con ecografía periódica). Alteración del control glucémico (hiperglucemia más frecuente que hipoglucemia). Bradicardia. Dolor en el sitio de inyección con las formulaciones de depósito.",
      },
      {
        farmaco: "Pasireotide",
        renal: "Sin ajuste mayor establecido; usar con precaución en insuficiencia renal severa (datos limitados).",
        hepatica: "Reducir dosis en insuficiencia hepática moderada; evitar en severa.",
        interacciones: "Igual que otros análogos de somatostatina — atención especial con fármacos que prolongan el QT (pasireotide también lo prolonga).",
        adversos: "Hiperglucemia marcada (más frecuente e intensa que con octreotide/lanreotide — inhibe más la secreción de incretinas; requiere monitoreo glucémico estrecho desde el inicio). Además, los efectos de clase: GI, colelitiasis, bradicardia. Prolongación del intervalo QT.",
      },
      {
        farmaco: "Cabergolina",
        renal: "Sin ajuste mayor establecido (datos limitados en insuficiencia renal).",
        hepatica: "Usar con precaución en insuficiencia hepática severa — tiene metabolismo hepático; considerar reducir dosis.",
        interacciones: "Evitar con antipsicóticos y otros antagonistas dopaminérgicos (reducen su eficacia). Antihipertensivos potencian la hipotensión ortostática.",
        adversos: "Náuseas, mareos, hipotensión ortostática (sobre todo al iniciar o escalar dosis — titular lentamente). Fibrosis valvular cardíaca con dosis altas y uso prolongado (más descrito en dosis de Parkinson; en dosis bajas de prolactinoma se recomienda igual ecocardiograma si la dosis acumulada es alta). Trastornos del control de impulsos (raro, efecto de clase de los agonistas dopaminérgicos). Somnolencia.",
      },
      {
        farmaco: "Metirapona",
        renal: "Sin ajustes estandarizados publicados; usar con monitoreo estrecho de cortisol y electrolitos independientemente de la función renal.",
        hepatica: "Usar con precaución y monitoreo estrecho en insuficiencia hepática — tiene metabolismo hepático relevante.",
        interacciones: "Fenitoína acelera su metabolismo y puede reducir su eficacia.",
        adversos: "Náuseas, vértigo, cefalea. Hirsutismo y acné (por acumulación de precursores androgénicos, 11-desoxicortisol y andrógenos suprarrenales). Hipertensión, edema e hipopotasemia (por acumulación de precursores mineralocorticoides, 11-desoxicorticosterona). Insuficiencia suprarrenal si se sobre-suprime la síntesis de cortisol — requiere monitoreo clínico y bioquímico frecuente.",
      },
      {
        farmaco: "Fluconazol (uso off-label como inhibidor de esteroidogénesis, dosis altas)",
        renal: "Sí requiere ajuste — tiene eliminación renal significativa. Dosis de carga completa, luego reducir aproximadamente 50% si eGFR 21–50, y 25% si eGFR ≤ 20 o diálisis.",
        hepatica: "Usar con precaución y monitorear transaminasas periódicamente; no hay reducción de dosis estandarizada pero sí vigilancia estrecha recomendada.",
        interacciones: "Inhibidor potente de CYP2C9 y CYP3A4 — aumenta niveles de warfarina, sulfonilureas (riesgo de hipoglucemia), estatinas (riesgo de miopatía), fenitoína y ciclosporina. Prolonga el intervalo QT, con riesgo aumentado si se combina con otros fármacos QT-prolongantes.",
        adversos: "Hepatotoxicidad (elevación de transaminasas — el efecto más relevante a vigilar en este uso). Náuseas, cefalea. Prolongación del QT (riesgo de arritmias). Rash.",
      },
    ],
  },
  {
    id: "otros",
    nombre: "Otros relevantes en endocrinología",
    color: "#B4841F",
    items: [
      {
        farmaco: "Estatinas (atorvastatina, simvastatina)",
        renal: "Sin ajuste mayor en la mayoría de los grados de deterioro; algunas requieren reducción en ERC avanzada (ej. rosuvastatina).",
        hepatica: "Contraindicadas en enfermedad hepática activa — monitorear transaminasas.",
        interacciones: "Azoles, macrólidos, inhibidores de proteasa y pomelo aumentan el riesgo de miopatía/rabdomiólisis (vía CYP3A4). Fibratos —especialmente gemfibrozilo— aumentan ese mismo riesgo.",
        adversos: "Mialgia/miopatía (la más frecuente en la práctica). Elevación de transaminasas. Rabdomiólisis (rara pero grave). Aumento leve del riesgo de desarrollar diabetes.",
      },
      {
        farmaco: "Espironolactona (SOP / hirsutismo)",
        renal: "Evitar o usar con mucha precaución en ERC avanzada — riesgo de hiperpotasemia; contraindicada con eGFR muy bajo.",
        hepatica: "Sin ajuste mayor descrito.",
        interacciones: "IECA, ARA2 y AINEs aumentan el riesgo de hiperpotasemia. Potencia niveles de digoxina.",
        adversos: "Hiperpotasemia (el más relevante a vigilar). Ginecomastia y mastalgia por efecto antiandrogénico. Irregularidades menstruales.",
      },
    ],
  },
];

function InteraccionesTab() {
  const [busqueda, setBusqueda] = useState("");
  const [catActiva, setCatActiva] = useState("todos");

  const filtradas = useMemo(() => {
    const q = busqueda.trim().toLowerCase();
    return FARMACOS_CATEGORIAS.map((cat) => ({
      ...cat,
      items: cat.items.filter((it) => {
        const matchCat = catActiva === "todos" || cat.id === catActiva;
        const matchQuery = q === "" || it.farmaco.toLowerCase().includes(q);
        return matchCat && matchQuery;
      }),
    })).filter((cat) => cat.items.length > 0);
  }, [busqueda, catActiva]);

  return (
    <div>
      <div style={{ display: "flex", alignItems: "center", gap: "8px", marginBottom: "6px" }}>
        <div style={{ width: "8px", height: "8px", borderRadius: "50%", background: "#B4841F" }} />
        <div style={{ fontFamily: "'Space Grotesk', sans-serif", fontWeight: 600, fontSize: "19px" }}>
          Interacciones y ajustes renal/hepático
        </div>
      </div>
      <p style={{ color: "#4A544E", fontSize: "13.5px", marginBottom: "18px", maxWidth: "620px", lineHeight: 1.5 }}>
        Fármacos de uso frecuente en endocrinología y diabetes — ajuste por función renal, ajuste por
        función hepática, e interacciones clave a tener en cuenta.
      </p>

      <input
        type="text"
        placeholder="Buscar fármaco (ej: metformina, levotiroxina, estatinas...)"
        value={busqueda}
        onChange={(e) => setBusqueda(e.target.value)}
        style={{ width: "100%", padding: "13px 16px", borderRadius: "10px", border: "1px solid #D8D5CB", background: "#FFFFFF", fontSize: "14.5px", marginBottom: "16px", outline: "none" }}
      />

      <div className="chips-scroll" style={{ display: "flex", gap: "8px", overflowX: "auto", marginBottom: "24px", paddingBottom: "2px" }}>
        <div className={`chip ${catActiva === "todos" ? "active" : ""}`} onClick={() => setCatActiva("todos")}>Todas las categorías</div>
        {FARMACOS_CATEGORIAS.map((cat) => (
          <div key={cat.id} className={`chip ${catActiva === cat.id ? "active" : ""}`} onClick={() => setCatActiva(cat.id)}>{cat.nombre}</div>
        ))}
      </div>

      {filtradas.length === 0 && <div style={{ color: "#6B7A72", fontSize: "14px", padding: "24px 0" }}>No se encontraron fármacos para "{busqueda}".</div>}

      {filtradas.map((cat) => (
        <div key={cat.id} style={{ marginBottom: "24px" }}>
          <div style={{ display: "flex", alignItems: "center", gap: "8px", marginBottom: "12px" }}>
            <div style={{ width: "8px", height: "8px", borderRadius: "50%", background: cat.color }} />
            <div style={{ fontFamily: "'Space Grotesk', sans-serif", fontWeight: 600, fontSize: "15.5px" }}>{cat.nombre}</div>
          </div>
          <div style={{ display: "flex", flexDirection: "column", gap: "10px" }}>
            {cat.items.map((it, i) => (
              <div key={i} style={{ background: "#FFFFFF", border: "1px solid #E4E1D6", borderLeft: `4px solid ${cat.color}`, borderRadius: "12px", padding: "16px 20px" }}>
                <div style={{ fontFamily: "'Space Grotesk', sans-serif", fontWeight: 600, fontSize: "14.5px", marginBottom: "10px" }}>{it.farmaco}</div>
                <div style={{ display: "flex", flexDirection: "column", gap: "8px" }}>
                  <div>
                    <span className="eyebrow" style={{ color: "#4A6FA5" }}>Ajuste renal</span>
                    <div style={{ fontSize: "13px", color: "#3A423E", lineHeight: 1.5, marginTop: "2px" }}>{it.renal}</div>
                  </div>
                  <div>
                    <span className="eyebrow" style={{ color: "#A2483A" }}>Ajuste hepático</span>
                    <div style={{ fontSize: "13px", color: "#3A423E", lineHeight: 1.5, marginTop: "2px" }}>{it.hepatica}</div>
                  </div>
                  <div>
                    <span className="eyebrow" style={{ color: "#B4841F" }}>Interacciones clave</span>
                    <div style={{ fontSize: "13px", color: "#3A423E", lineHeight: 1.5, marginTop: "2px" }}>{it.interacciones}</div>
                  </div>
                  <div>
                    <span className="eyebrow" style={{ color: "#6B5B95" }}>Efectos adversos principales</span>
                    <div style={{ fontSize: "13px", color: "#3A423E", lineHeight: 1.5, marginTop: "2px" }}>{it.adversos}</div>
                  </div>
                </div>
              </div>
            ))}
          </div>
        </div>
      ))}

      <Disclaimer texto="Esta tabla resume interacciones y ajustes frecuentes de uso práctico diario; no reemplaza la consulta a una fuente farmacológica completa (ej. UpToDate Lexicomp, Vademécum) ante casos complejos, polifarmacia significativa, o pacientes con múltiples comorbilidades. Los puntos de corte de eGFR para ajuste de dosis pueden variar levemente según el prospecto/ficha técnica local — confirmar siempre contra la información del fabricante vigente en Argentina antes de prescribir." />
    </div>
  );
}

/* ============================================================
   COMPONENTES COMUNES
   ============================================================ */
function Disclaimer({ texto }) {
  return (
    <div style={{ fontSize: "12.5px", color: "#6B7A72", lineHeight: 1.6, borderTop: "1px solid #E4E1D6", paddingTop: "18px", marginTop: "8px" }}>
      <strong style={{ color: "#4A544E" }}>Nota clínica:</strong> {texto}
    </div>
  );
}

/* ============================================================
   APP PRINCIPAL
   ============================================================ */
const TABS = [
  { id: "obesidad", label: "Parámetros metabólicos" },
  { id: "nodulo", label: "Nódulo tiroideo (TI-RADS/ATA)" },
  { id: "prevent", label: "Riesgo CV (PREVENT)" },
  { id: "masld", label: "MASLD (FIB-4)" },
  { id: "corticoides", label: "Equivalencias de corticoides" },
  { id: "referencia", label: "Valores de referencia" },
  { id: "conversor", label: "Conversor de unidades" },
  { id: "algoritmos", label: "Algoritmos terapéuticos" },
  { id: "renal", label: "Función renal (CKD-EPI)" },
  { id: "interacciones", label: "Interacciones y ajustes" },
];

export default function App() {
  const [tab, setTab] = useState("corticoides");

  return (
    <div style={{ minHeight: "100%", background: "#F5F4F0", fontFamily: "'IBM Plex Sans', sans-serif", color: "#1C2321" }}>
      <GlobalStyles />
      <div style={{ maxWidth: "960px", margin: "0 auto", padding: "48px 24px 80px" }}>
        <div style={{ marginBottom: "28px" }}>
          <div className="eyebrow" style={{ marginBottom: "10px" }}>Referencia rápida · Endocrinología clínica</div>
          <h1 style={{ fontFamily: "'Space Grotesk', sans-serif", fontSize: "32px", fontWeight: 600, letterSpacing: "-0.02em", margin: 0, lineHeight: 1.15 }}>
            Toolkit de endocrinología
          </h1>
          <p style={{ marginTop: "10px", color: "#4A544E", fontSize: "15px", maxWidth: "600px", lineHeight: 1.5 }}>
            Herramientas de referencia rápida para la práctica clínica diaria.
          </p>
        </div>

        <div className="chips-scroll" style={{ display: "flex", gap: "6px", overflowX: "auto", marginBottom: "28px", background: "#FFFFFF", border: "1px solid #E4E1D6", borderRadius: "12px", padding: "6px" }}>
          {TABS.map((t) => (
            <button key={t.id} className={`tab-btn ${tab === t.id ? "active" : ""}`} onClick={() => setTab(t.id)}>
              {t.label}
            </button>
          ))}
        </div>

        {tab === "corticoides" && <CorticoidesTab />}
        {tab === "referencia" && <ValoresReferenciaTab />}
        {tab === "conversor" && <ConversorTab />}
        {tab === "algoritmos" && <AlgoritmosTab />}
        {tab === "prevent" && <PreventTab />}
        {tab === "masld" && <MasldTab />}
        {tab === "obesidad" && <ObesidadTab />}
        {tab === "nodulo" && <NoduloTab />}
        {tab === "renal" && <RenalTab />}
        {tab === "interacciones" && <InteraccionesTab />}
      </div>
    </div>
  );
}
