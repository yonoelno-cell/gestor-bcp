import { useState, useEffect, useCallback, useRef } from "react";

/* ═══════════════════════════════════════════════════════════
   GLOBAL STYLES — Dark Banking Premium UI
═══════════════════════════════════════════════════════════ */
const GlobalStyles = () => (
  <style>{`
    @import url('https://fonts.googleapis.com/css2?family=Sora:wght@300;400;500;600;700;800&family=JetBrains+Mono:wght@400;500;600&display=swap');

    :root {
      --bg:        #07090D;
      --bg2:       #0C0F16;
      --bg3:       #111827;
      --card:      rgba(255,255,255,0.04);
      --card-h:    rgba(255,255,255,0.07);
      --blue:      #1A4FA0;
      --blue-l:    #2563EB;
      --blue-xl:   #60A5FA;
      --gold:      #D4A843;
      --gold-l:    #F0C040;
      --teal:      #2EC4B6;
      --purple:    #9B59B6;
      --red:       #EF4444;
      --green:     #22C55E;
      --text:      #F1F5F9;
      --text2:     #94A3B8;
      --text3:     #475569;
      --border:    rgba(255,255,255,0.07);
      --border2:   rgba(255,255,255,0.12);
      --shadow:    0 8px 32px rgba(0,0,0,0.5);
      --shadow2:   0 4px 16px rgba(0,0,0,0.3);
      --radius:    18px;
      --radius-sm: 12px;
      --radius-xs: 8px;
    }

    .theme-light {
      --bg:     #EEF2F7;
      --bg2:    #E3E9F2;
      --bg3:    #D6DFEe;
      --card:   rgba(255,255,255,0.85);
      --card-h: rgba(255,255,255,1);
      --border: rgba(0,0,0,0.07);
      --border2:rgba(0,0,0,0.13);
      --text:   #0F172A;
      --text2:  #475569;
      --text3:  #94A3B8;
    }

    *, *::before, *::after { box-sizing: border-box; margin:0; padding:0; }

    body, #root {
      font-family: 'Sora', sans-serif;
      background: var(--bg);
      color: var(--text);
      -webkit-font-smoothing: antialiased;
    }

    .mono { font-family: 'JetBrains Mono', monospace !important; }

    /* ── Glass card ── */
    .glass {
      background: var(--card);
      backdrop-filter: blur(14px);
      -webkit-backdrop-filter: blur(14px);
      border: 1px solid var(--border);
      border-radius: var(--radius);
    }
    .glass:hover { background: var(--card-h); }

    /* ── Nav blur ── */
    .nav-blur {
      background: rgba(7,9,13,0.88);
      backdrop-filter: blur(24px);
      -webkit-backdrop-filter: blur(24px);
      border-top: 1px solid rgba(255,255,255,0.06);
    }

    /* ── Buttons ── */
    .btn { font-family:'Sora',sans-serif; cursor:pointer; transition: all .2s ease; }

    .btn-primary {
      background: linear-gradient(135deg, var(--blue) 0%, var(--blue-l) 100%);
      color: #fff; border: none; border-radius: var(--radius-sm);
      padding: 12px 20px; font-weight: 600; font-size: 14px;
      box-shadow: 0 4px 18px rgba(26,79,160,.4);
    }
    .btn-primary:hover { transform: translateY(-2px); box-shadow: 0 8px 24px rgba(26,79,160,.55); }
    .btn-primary:active { transform: translateY(0); }

    .btn-gold {
      background: linear-gradient(135deg, var(--gold), var(--gold-l));
      color: #07090D; border: none; border-radius: var(--radius-sm);
      padding: 11px 18px; font-weight: 700; font-size: 13px;
    }
    .btn-gold:hover { transform: translateY(-1px); box-shadow: 0 6px 18px rgba(212,168,67,.45); }

    .btn-teal {
      background: linear-gradient(135deg, #1A8F87, var(--teal));
      color: #fff; border: none; border-radius: var(--radius-sm);
      padding: 10px 16px; font-weight: 600; font-size: 13px;
    }

    .btn-ghost {
      background: transparent; color: var(--text2);
      border: 1px solid var(--border2); border-radius: var(--radius-xs);
      padding: 9px 14px; font-size: 13px;
    }
    .btn-ghost:hover { background: var(--card-h); color: var(--text); }

    .btn-danger {
      background: rgba(239,68,68,.1); color: #F87171;
      border: 1px solid rgba(239,68,68,.25); border-radius: var(--radius-xs);
      padding: 8px 12px; font-size: 12px;
    }
    .btn-danger:hover { background: rgba(239,68,68,.2); }

    /* ── Inputs ── */
    .field {
      background: rgba(255,255,255,0.05);
      border: 1px solid var(--border2);
      border-radius: var(--radius-sm);
      padding: 11px 14px;
      color: var(--text);
      font-family: 'Sora', sans-serif;
      font-size: 14px; width: 100%;
      outline: none; transition: border-color .2s, background .2s;
    }
    .field:focus { border-color: rgba(37,99,235,.55); background: rgba(37,99,235,.06); }
    .field::placeholder { color: var(--text3); }
    .field option { background: #0D1117; color: #F1F5F9; }
    textarea.field { resize: vertical; min-height: 96px; line-height: 1.65; }

    /* ── Chips / badges ── */
    .chip {
      display: inline-flex; align-items: center; gap: 3px;
      padding: 3px 10px; border-radius: 20px;
      font-size: 11px; font-weight: 700; white-space: nowrap;
    }
    .badge {
      display: inline-flex; align-items: center; gap: 3px;
      padding: 2px 8px; border-radius: 6px;
      font-size: 11px; font-weight: 600;
    }

    /* ── Toggle switch ── */
    .toggle-track {
      width: 50px; height: 27px; border-radius: 14px;
      border: none; cursor: pointer; position: relative;
      transition: background .3s; padding: 0;
    }
    .toggle-thumb {
      width: 21px; height: 21px; border-radius: 50%; background: white;
      position: absolute; top: 3px; transition: left .3s;
      box-shadow: 0 2px 6px rgba(0,0,0,.35);
    }

    /* ── Animations ── */
    @keyframes fadeUp {
      from { opacity:0; transform:translateY(10px); }
      to   { opacity:1; transform:translateY(0); }
    }
    @keyframes pulse {
      0%,100% { opacity:1; } 50% { opacity:.4; }
    }
    @keyframes barGrow {
      from { width:0; } to { width:var(--w); }
    }
    @keyframes spin {
      to { transform: rotate(360deg); }
    }
    .fade-up  { animation: fadeUp .3s ease both; }
    .blink    { animation: pulse 2s infinite; }
    .spin     { animation: spin .8s linear infinite; }

    /* ── Scrollbar ── */
    ::-webkit-scrollbar { width: 4px; height: 4px; }
    ::-webkit-scrollbar-track { background: transparent; }
    ::-webkit-scrollbar-thumb { background: rgba(255,255,255,0.12); border-radius: 4px; }

    /* ── Section label ── */
    .sec-label {
      font-size: 10px; font-weight: 700; letter-spacing: 1.8px;
      text-transform: uppercase; color: var(--text3);
      margin-bottom: 10px;
    }

    /* ── Card hover lift ── */
    .lift { transition: transform .2s ease, box-shadow .2s ease; }
    .lift:hover { transform: translateY(-2px); box-shadow: 0 12px 32px rgba(0,0,0,.4); }

    /* ── Gradient text ── */
    .grad-text {
      background: linear-gradient(135deg, var(--teal), var(--gold));
      -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;
    }

    /* ── Divider ── */
    .divider { height:1px; background: var(--border); margin: 12px 0; }

    /* ── Modal overlay ── */
    .overlay {
      position: fixed; inset: 0; z-index: 200;
      background: rgba(0,0,0,.72);
      backdrop-filter: blur(6px); -webkit-backdrop-filter: blur(6px);
      display: flex; align-items: center; justify-content: center; padding: 20px;
    }

    /* ── Responsive centering ── */
    .app-shell {
      max-width: 480px; margin: 0 auto;
      min-height: 100vh; background: var(--bg);
      position: relative; overflow: hidden;
    }
  `}</style>
);

/* ═══════════════════════════════════════════════════════════
   CONSTANTS
═══════════════════════════════════════════════════════════ */
const BANKS = ["BCP","Interbank","BBVA","Scotiabank","BanBif","Pichincha","GNB","Yape","Plin","Banco de la Nación"];

const LABELS = [
  { id:"urgente",   text:"⚡ Urgente",   bg:"#EF4444", fg:"#fff"     },
  { id:"pagado",    text:"✅ Pagado",    bg:"#2EC4B6", fg:"#fff"     },
  { id:"pendiente", text:"⏳ Pendiente", bg:"#D4A843", fg:"#07090D"  },
  { id:"verificar", text:"🔍 Verificar", bg:"#9B59B6", fg:"#fff"     },
  { id:"fraude",    text:"🚨 Fraude",   bg:"#FF6B35", fg:"#fff"     },
];
const LABEL_MAP = Object.fromEntries(LABELS.map(l=>[l.id,l]));

const TABS = [
  { id:"registrar", icon:"📋", label:"Registrar" },
  { id:"historial", icon:"📊", label:"Historial"  },
  { id:"buscar",    icon:"🔍", label:"Buscar"     },
  { id:"usuarios",  icon:"👥", label:"Usuarios"   },
  { id:"config",    icon:"⚙️",  label:"Config"    },
];

/* ── Mock seed data ── */
const MOCK_USERS = [
  { dni:"12345678", nombre:"Carlos Mendoza",  bancoPrincipal:"BCP",       cuentas:[{banco:"BCP",       numero:"191-12345678-0-12"}],                        nota:"Cliente frecuente"  },
  { dni:"87654321", nombre:"María Torres",    bancoPrincipal:"Interbank", cuentas:[{banco:"Interbank", numero:"200-3001234567"},{banco:"BBVA",numero:"0011-0175-0100012345"}], nota:""               },
  { dni:"45678901", nombre:"Jorge Quispe",    bancoPrincipal:"Yape",      cuentas:[{banco:"Yape",      numero:"987654321"}],                                nota:"Proveedor principal"},
  { dni:"11223344", nombre:"Lucía Vargas",    bancoPrincipal:"BBVA",      cuentas:[{banco:"BBVA",      numero:"0011-0222-0200034567"}],                     nota:""               },
];

const MOCK_OPS = [
  { id:"op1", monto:1500.00, fecha:"2026-03-21", hora:"10:30", nroOperacion:"12345678901", emisor:"12345678", receptor:"87654321", bancoEmisor:"BCP",       bancoReceptor:"Interbank", etiqueta:"pagado",    nota:"Pago mensual",        sunatEstado:"ok",   foto:null },
  { id:"op2", monto: 850.50, fecha:"2026-03-20", hora:"14:15", nroOperacion:"98765432101", emisor:"87654321", receptor:"45678901", bancoEmisor:"Interbank", bancoReceptor:"Yape",      etiqueta:"pendiente", nota:"",                    sunatEstado:"pend", foto:null },
  { id:"op3", monto:3200.00, fecha:"2026-03-18", hora:"09:00", nroOperacion:"11223344556", emisor:"12345678", receptor:"45678901", bancoEmisor:"BCP",       bancoReceptor:"Yape",      etiqueta:"urgente",   nota:"Urgente – verificar", sunatEstado:"pend", foto:null },
  { id:"op4", monto: 450.00, fecha:"2026-02-28", hora:"16:45", nroOperacion:"55443322110", emisor:"45678901", receptor:"12345678", bancoEmisor:"Yape",      bancoReceptor:"BCP",       etiqueta:"pagado",    nota:"",                    sunatEstado:"ok",   foto:null },
  { id:"op5", monto: 920.75, fecha:"2026-02-15", hora:"11:20", nroOperacion:"66778899001", emisor:"87654321", receptor:"12345678", bancoEmisor:"BBVA",      bancoReceptor:"BCP",       etiqueta:"verificar", nota:"Revisar comprobante", sunatEstado:"pend", foto:null },
  { id:"op6", monto:2100.00, fecha:"2026-01-30", hora:"08:10", nroOperacion:"77889900112", emisor:"11223344", receptor:"87654321", bancoEmisor:"BBVA",      bancoReceptor:"Interbank", etiqueta:"pagado",    nota:"",                    sunatEstado:"ok",   foto:null },
];

/* ═══════════════════════════════════════════════════════════
   HOOKS
═══════════════════════════════════════════════════════════ */
function useLocalStorage(key, init) {
  const [val, setVal] = useState(() => {
    try { const s = localStorage.getItem(key); return s ? JSON.parse(s) : init; }
    catch { return init; }
  });
  const set = useCallback(v => {
    setVal(prev => {
      const next = typeof v === "function" ? v(prev) : v;
      try { localStorage.setItem(key, JSON.stringify(next)); } catch {}
      return next;
    });
  }, [key]);
  return [val, set];
}

// TODO: Replace with real Tesseract.js call
// eslint-disable-next-line no-unused-vars
const runTesseractOCR = async (imageBase64) => {
  // Tesseract.recognize(imageBase64, 'spa', { logger: m => console.log(m) })
  return null;
};

// TODO: Replace with real Claude Vision API call
const useClaudeVision = () => {
  return async (imageBase64) => {
    // const res = await fetch('https://api.anthropic.com/v1/messages', { ... })
    return null;
  };
};

// TODO: Replace with real DNI API call
const fetchDNIData = async (dni) => {
  // const res = await fetch(`https://api.reniec.gob.pe/dni/${dni}`)
  return null;
};

// TODO: Google Apps Script sync
const syncToGoogleDrive = async (url, data) => {
  // const res = await fetch(url, { method:'POST', body: JSON.stringify(data) })
  return false;
};

/* ═══════════════════════════════════════════════════════════
   UTILS
═══════════════════════════════════════════════════════════ */
const fmtMonto = n => `S/ ${Number(n).toLocaleString("es-PE",{minimumFractionDigits:2,maximumFractionDigits:2})}`;

const fmtDate = iso => {
  if (!iso) return "—";
  const [y,m,d] = iso.split("-");
  const M = ["","Ene","Feb","Mar","Abr","May","Jun","Jul","Ago","Sep","Oct","Nov","Dic"];
  return `${d} ${M[+m]} ${y}`;
};

const monthLabel = key => {
  if (!key) return "";
  const [y,m] = key.split("-");
  const M = ["","Enero","Febrero","Marzo","Abril","Mayo","Junio","Julio","Agosto","Septiembre","Octubre","Noviembre","Diciembre"];
  return `${M[+m]} ${y}`;
};

const groupByMonth = ops =>
  Object.entries(
    ops.reduce((acc,op)=>{ const k=op.fecha?.slice(0,7)||"unknown"; (acc[k]??=[]).push(op); return acc; }, {})
  ).sort(([a],[b])=>b<a?-1:1);

const getUser = (dni, users) => users.find(u=>u.dni===dni);
const getUserName = (dni, users) => getUser(dni, users)?.nombre ?? dni;
const initials = name => name.split(" ").map(w=>w[0]).slice(0,2).join("").toUpperCase();

function parseVoucher(text) {
  const r = { monto:null, nroOperacion:null, fecha:null, hora:null, bancoEmisor:null, bancoReceptor:null };

  const mM = text.match(/S\/\s*([\d,]+\.?\d*)|(\d{1,3}(?:,\d{3})*(?:\.\d{2})?)\s*(?:soles?|PEN)/i);
  if (mM) r.monto = parseFloat((mM[1]||mM[2]).replace(/,/g,""));

  const opM = text.match(/(?:op(?:erac[ió]n)?\.?\s*n[°º]?\.?\s*|n[°º]\s*op\.?\s*)(\d{8,12})|(?<!\d)(\d{10,12})(?!\d)/i);
  if (opM) r.nroOperacion = opM[1]||opM[2];

  const months = {enero:1,febrero:2,marzo:3,abril:4,mayo:5,junio:6,julio:7,agosto:8,septiembre:9,octubre:10,noviembre:11,diciembre:12};
  const fM = text.match(/(\d{1,2})[\/\-](\d{1,2})[\/\-](\d{4})|(\d{1,2})\s+(?:de\s+)?(enero|febrero|marzo|abril|mayo|junio|julio|agosto|septiembre|octubre|noviembre|diciembre)\s+(?:de\s+)?(\d{4})/i);
  if (fM) {
    if (fM[4]) { const m=months[fM[5].toLowerCase()]; r.fecha=`${fM[6]}-${String(m).padStart(2,"0")}-${String(fM[4]).padStart(2,"0")}`; }
    else r.fecha=`${fM[3]}-${fM[2].padStart(2,"0")}-${fM[1].padStart(2,"0")}`;
  }

  const hM = text.match(/(\d{1,2}):(\d{2})\s*(AM|PM)?/i);
  if (hM) { let h=+hM[1]; if(hM[3]?.toUpperCase()==="PM"&&h<12)h+=12; if(hM[3]?.toUpperCase()==="AM"&&h===12)h=0; r.hora=`${String(h).padStart(2,"0")}:${hM[2]}`; }

  const rx = new RegExp(BANKS.map(b=>b.replace(/[.*+?^${}()|[\]\\]/g,"\\$&")).join("|"),"gi");
  const found = [...text.matchAll(rx)].map(m=>m[0]);
  if (found[0]) r.bancoEmisor = found[0];
  if (found[1]) r.bancoReceptor = found[1];

  return r;
}

/* ═══════════════════════════════════════════════════════════
   SHARED UI COMPONENTS
═══════════════════════════════════════════════════════════ */
const LabelChip = ({ id }) => {
  const l = LABEL_MAP[id];
  if (!l) return null;
  return <span className="chip" style={{background:l.bg,color:l.fg}}>{l.text}</span>;
};

const SunatBadge = ({ state }) => (
  <span className="badge" style={{
    background: state==="ok" ? "rgba(46,196,182,.15)" : "rgba(212,168,67,.15)",
    color: state==="ok" ? "#2EC4B6" : "#D4A843",
    border: `1px solid ${state==="ok"?"rgba(46,196,182,.3)":"rgba(212,168,67,.3)"}`,
  }}>
    {state==="ok" ? "✓ SUNAT" : "⏳ SUNAT"}
  </span>
);

function StatCard({ icon, label, value, sub, accent }) {
  return (
    <div className="glass lift" style={{
      padding:"14px 12px",
      background: accent ? `linear-gradient(135deg,${accent}20,${accent}08)` : "var(--card)",
      border: accent ? `1px solid ${accent}25` : undefined,
    }}>
      <div style={{fontSize:20,marginBottom:4}}>{icon}</div>
      <div style={{fontSize:10,color:"var(--text2)",marginBottom:3,fontWeight:600,letterSpacing:0.5}}>{label}</div>
      <div style={{fontSize:17,fontWeight:700,color:accent||"var(--text)",lineHeight:1.1,fontFamily:"JetBrains Mono,monospace"}}>{value}</div>
      {sub && <div style={{fontSize:10,color:"var(--text3)",marginTop:3}}>{sub}</div>}
    </div>
  );
}

function SectionLabel({ children }) {
  return <div className="sec-label">{children}</div>;
}

function Divider() { return <div className="divider"/>; }

function Modal({ onClose, children, title, maxW=400 }) {
  return (
    <div className="overlay" onClick={onClose}>
      <div className="glass fade-up" style={{width:"100%",maxWidth:maxW,padding:22,maxHeight:"88vh",overflowY:"auto"}} onClick={e=>e.stopPropagation()}>
        <div style={{display:"flex",justifyContent:"space-between",alignItems:"center",marginBottom:16}}>
          <div style={{fontSize:15,fontWeight:700}}>{title}</div>
          <button onClick={onClose} style={{background:"none",border:"none",color:"var(--text2)",cursor:"pointer",fontSize:22,lineHeight:1}}>×</button>
        </div>
        {children}
      </div>
    </div>
  );
}

function RowBtn({ icon, label, color, bg, border, onClick, flex=1 }) {
  return (
    <button className="btn" onClick={onClick} style={{flex,padding:"7px 0",borderRadius:"var(--radius-xs)",border:`1px solid ${border}`,background:bg,color,fontFamily:"Sora",fontSize:11,fontWeight:600}}>
      {icon} {label}
    </button>
  );
}

/* ═══════════════════════════════════════════════════════════
   PAGE: REGISTRAR
═══════════════════════════════════════════════════════════ */
function PageRegistrar({ operations, setOperations, users }) {
  const [voucher, setVoucher]           = useState("");
  const [parsed, setParsed]             = useState({});
  const [dniE, setDniE]                 = useState("");
  const [nomE, setNomE]                 = useState("");
  const [dniR, setDniR]                 = useState("");
  const [nomR, setNomR]                 = useState("");
  const [bancoE, setBancoE]             = useState("");
  const [bancoR, setBancoR]             = useState("");
  const [etiqueta, setEtiqueta]         = useState("");
  const [nota, setNota]                 = useState("");
  const [imgPrev, setImgPrev]           = useState(null);
  const [ocrState, setOcrState]         = useState(null); // null|'processing'|'done'
  const [dupModal, setDupModal]         = useState(false);
  const [pendingOp, setPendingOp]       = useState(null);
  const [flash, setFlash]               = useState(false);
  const claudeVision = useClaudeVision();

  /* auto-parse */
  useEffect(()=>{ setParsed(voucher.trim() ? parseVoucher(voucher) : {}); }, [voucher]);

  /* autofill emisor */
  useEffect(()=>{
    if (dniE.length===8) {
      const u=getUser(dniE,users);
      if(u){ setNomE(u.nombre); if(u.bancoPrincipal) setBancoE(u.bancoPrincipal); }
    }
  },[dniE,users]);

  /* autofill receptor */
  useEffect(()=>{
    if (dniR.length===8) {
      const u=getUser(dniR,users);
      if(u){ setNomR(u.nombre); if(u.bancoPrincipal) setBancoR(u.bancoPrincipal); }
    }
  },[dniR,users]);

  const handleImg = e => {
    const f = e.target.files?.[0]; if(!f) return;
    const reader = new FileReader();
    reader.onload = ev => {
      setImgPrev(ev.target.result);
      setOcrState("processing");
      // TODO: run Tesseract + claudeVision(ev.target.result)
      setTimeout(()=>setOcrState("done"), 2000);
    };
    reader.readAsDataURL(f);
  };

  const summary = () => {
    const bE = parsed.bancoEmisor||bancoE||"?", bR = parsed.bancoReceptor||bancoR||"?";
    return `Comisión por depósito de ${bE} a ${bR}, monto ${fmtMonto(parsed.monto||0)} (Op. ${parsed.nroOperacion||"—"}), ${fmtDate(parsed.fecha)} ${parsed.hora||""}. Emisor: ${nomE||dniE||"—"} (DNI ${dniE||"—"}). Receptor: ${nomR||dniR||"—"} (DNI ${dniR||"—"}).`;
  };

  const buildOp = () => ({
    id: "op"+Date.now(),
    monto:        parsed.monto||0,
    fecha:        parsed.fecha||new Date().toISOString().slice(0,10),
    hora:         parsed.hora||"00:00",
    nroOperacion: parsed.nroOperacion||"",
    emisor: dniE, receptor: dniR,
    bancoEmisor:  parsed.bancoEmisor||bancoE,
    bancoReceptor:parsed.bancoReceptor||bancoR,
    foto: imgPrev, etiqueta, nota, sunatEstado:"pend",
  });

  const handleSave = () => {
    const op = buildOp();
    const dup = operations.find(o=> (op.nroOperacion && o.nroOperacion===op.nroOperacion) || (o.monto===op.monto && o.fecha===op.fecha));
    if (dup) { setPendingOp(op); setDupModal(true); return; }
    doSave(op);
  };

  const doSave = op => {
    setOperations(p=>[op,...p]);
    setFlash(true); setDupModal(false);
    setTimeout(()=>setFlash(false),3000);
  };

  const PFIELDS = [
    {k:"monto",      label:"💰 Monto",        fmt:fmtMonto},
    {k:"nroOperacion",label:"🔢 N° Operación", fmt:v=>v},
    {k:"fecha",      label:"📅 Fecha",         fmt:fmtDate},
    {k:"hora",       label:"⏰ Hora",          fmt:v=>v},
    {k:"bancoEmisor",label:"🏦 Banco Emisor",  fmt:v=>v},
    {k:"bancoReceptor",label:"🏦 Banco Recep.",fmt:v=>v},
  ];

  return (
    <div className="fade-up" style={{padding:16,display:"flex",flexDirection:"column",gap:14}}>

      {/* OCR Card */}
      <div className="glass" style={{padding:16,background:"linear-gradient(135deg,rgba(26,79,160,.12),rgba(46,196,182,.06))"}}>
        <SectionLabel>📸 Captura / OCR</SectionLabel>
        <div style={{display:"flex",gap:8,marginBottom:12}}>
          <label className="btn btn-primary" style={{flex:1,textAlign:"center",padding:"10px 8px",fontSize:13}}>
            📷 Tomar foto
            <input type="file" accept="image/*" capture="environment" style={{display:"none"}} onChange={handleImg}/>
          </label>
          <label className="btn btn-ghost" style={{flex:1,textAlign:"center",padding:"10px 8px",fontSize:13}}>
            🖼 Galería
            <input type="file" accept="image/*" style={{display:"none"}} onChange={handleImg}/>
          </label>
        </div>
        {imgPrev && <img src={imgPrev} alt="voucher" style={{width:"100%",maxHeight:150,objectFit:"cover",borderRadius:12,marginBottom:10,border:"1px solid rgba(37,99,235,.3)"}}/>}
        {ocrState==="processing" && <div className="blink" style={{textAlign:"center",color:"var(--gold)",fontSize:13}}>⚙️ Procesando con Tesseract…</div>}
        {ocrState==="done"       && <div style={{textAlign:"center",color:"var(--teal)",fontSize:13}}>✅ OCR completado (stub listo)</div>}
      </div>

      {/* Paste Text */}
      <div className="glass" style={{padding:16}}>
        <SectionLabel>📋 Texto del comprobante</SectionLabel>
        <textarea className="field mono" placeholder="Pega aquí el texto del comprobante…" value={voucher} onChange={e=>setVoucher(e.target.value)} style={{fontSize:12}}/>
        {Object.keys(parsed).some(k=>parsed[k]) && (
          <div style={{marginTop:12,display:"grid",gridTemplateColumns:"1fr 1fr",gap:7}}>
            {PFIELDS.map(f=>(
              <div key={f.k} style={{
                background: parsed[f.k] ? "rgba(46,196,182,.1)" : "rgba(212,168,67,.1)",
                border: `1px solid ${parsed[f.k]?"rgba(46,196,182,.3)":"rgba(212,168,67,.3)"}`,
                borderRadius:10, padding:"8px 10px",
              }}>
                <div style={{fontSize:9,color:"var(--text2)",marginBottom:2,fontWeight:600}}>{f.label}</div>
                {parsed[f.k]
                  ? <div className="mono" style={{fontSize:12,color:"var(--teal)",fontWeight:600}}>{f.fmt(parsed[f.k])}</div>
                  : <div style={{fontSize:11,color:"var(--gold)"}}>No detectado</div>
                }
              </div>
            ))}
          </div>
        )}
      </div>

      {/* Emisor / Receptor */}
      <div className="glass" style={{padding:16}}>
        <SectionLabel>👤 Emisor</SectionLabel>
        <div style={{display:"grid",gridTemplateColumns:"1fr 1fr",gap:8,marginBottom:8}}>
          <input className="field mono" placeholder="DNI Emisor" value={dniE} onChange={e=>setDniE(e.target.value)} maxLength={8}/>
          <input className="field"      placeholder="Nombre"     value={nomE} onChange={e=>setNomE(e.target.value)}/>
        </div>
        <select className="field" value={bancoE} onChange={e=>setBancoE(e.target.value)}>
          <option value="">Banco emisor…</option>
          {BANKS.map(b=><option key={b}>{b}</option>)}
        </select>

        <Divider/>
        <SectionLabel>🎯 Receptor</SectionLabel>
        <div style={{display:"grid",gridTemplateColumns:"1fr 1fr",gap:8,marginBottom:8}}>
          <input className="field mono" placeholder="DNI Receptor" value={dniR} onChange={e=>setDniR(e.target.value)} maxLength={8}/>
          <input className="field"      placeholder="Nombre"       value={nomR} onChange={e=>setNomR(e.target.value)}/>
        </div>
        <select className="field" value={bancoR} onChange={e=>setBancoR(e.target.value)}>
          <option value="">Banco receptor…</option>
          {BANKS.map(b=><option key={b}>{b}</option>)}
        </select>
      </div>

      {/* Labels + nota */}
      <div className="glass" style={{padding:16}}>
        <SectionLabel>🏷 Etiqueta</SectionLabel>
        <div style={{display:"flex",gap:6,flexWrap:"wrap",marginBottom:10}}>
          {LABELS.map(l=>(
            <button key={l.id} className="btn" onClick={()=>setEtiqueta(etiqueta===l.id?"":l.id)}
              style={{padding:"5px 12px",borderRadius:20,fontSize:12,fontFamily:"Sora",fontWeight:700,
                border:`1.5px solid ${etiqueta===l.id?l.bg:"transparent"}`,
                background: etiqueta===l.id ? l.bg : "rgba(255,255,255,.05)",
                color: etiqueta===l.id ? l.fg : "var(--text2)",
              }}>
              {l.text}
            </button>
          ))}
        </div>
        <input className="field" placeholder="Nota adicional…" value={nota} onChange={e=>setNota(e.target.value)}/>
      </div>

      {/* Summary */}
      <div className="glass" style={{padding:16,background:"linear-gradient(135deg,rgba(26,79,160,.16),rgba(46,196,182,.08))"}}>
        <SectionLabel>📄 Resumen generado</SectionLabel>
        <div className="mono" style={{fontSize:12,color:"#E2E8F0",lineHeight:1.75,background:"rgba(0,0,0,.3)",borderRadius:10,padding:"12px 14px",marginBottom:12}}>
          {summary()}
        </div>
        <div style={{display:"flex",gap:8}}>
          <button className="btn btn-ghost" style={{flex:1,fontSize:12}} onClick={()=>navigator.clipboard?.writeText(summary())}>📋 Copiar</button>
          <button className="btn btn-primary" style={{flex:2,fontSize:14}} onClick={handleSave}>💾 Guardar operación</button>
        </div>
        {flash && (
          <div style={{marginTop:10,textAlign:"center",color:"var(--teal)",fontWeight:600,fontSize:13}}>
            ✅ ¡Operación guardada exitosamente!
          </div>
        )}
      </div>

      {dupModal && (
        <Modal title="⚠️ Posible duplicado" onClose={()=>setDupModal(false)}>
          <div style={{color:"var(--gold)",fontSize:14,textAlign:"center",marginBottom:8}}>Ya existe una operación similar.</div>
          <div style={{color:"var(--text2)",fontSize:13,textAlign:"center",marginBottom:20}}>¿Deseas guardarla de todas formas?</div>
          <div style={{display:"flex",gap:10}}>
            <button className="btn btn-ghost" style={{flex:1}} onClick={()=>setDupModal(false)}>Cancelar</button>
            <button className="btn btn-primary" style={{flex:1}} onClick={()=>doSave(pendingOp)}>Guardar igual</button>
          </div>
        </Modal>
      )}
    </div>
  );
}

/* ═══════════════════════════════════════════════════════════
   PAGE: HISTORIAL
═══════════════════════════════════════════════════════════ */
function PageHistorial({ operations, setOperations, users }) {
  const [detail, setDetail] = useState(null);
  const [edit,   setEdit]   = useState(null);

  const del    = id  => setOperations(p=>p.filter(o=>o.id!==id));
  const sunat  = id  => setOperations(p=>p.map(o=>o.id===id?{...o,sunatEstado:o.sunatEstado==="ok"?"pend":"ok"}:o));
  const saveEd = ()  => { setOperations(p=>p.map(o=>o.id===edit.id?edit:o)); setEdit(null); };

  const grouped = groupByMonth(operations);

  return (
    <div className="fade-up" style={{padding:16}}>
      {grouped.length===0 && (
        <div style={{textAlign:"center",padding:48,color:"var(--text3)"}}>
          <div style={{fontSize:44}}>📊</div>
          <div style={{marginTop:10,fontSize:14}}>Sin operaciones aún</div>
          <div style={{fontSize:12,marginTop:4}}>Registra tu primera transferencia</div>
        </div>
      )}

      {grouped.map(([key,ops])=>(
        <div key={key} style={{marginBottom:26}}>
          {/* Month header */}
          <div style={{display:"flex",alignItems:"center",gap:10,marginBottom:12}}>
            <div style={{height:1,flex:1,background:"linear-gradient(90deg,var(--gold),transparent)"}}/>
            <span style={{fontSize:11,fontWeight:800,color:"var(--gold)",letterSpacing:2,textTransform:"uppercase"}}>{monthLabel(key)}</span>
            <div style={{height:1,flex:1,background:"linear-gradient(270deg,var(--gold),transparent)"}}/>
          </div>

          <div style={{display:"flex",flexDirection:"column",gap:10}}>
            {ops.map(op=>(
              <div key={op.id} className="glass lift" style={{padding:14}}>
                <div style={{display:"flex",justifyContent:"space-between",alignItems:"flex-start",marginBottom:8}}>
                  <div>
                    <div className="mono" style={{fontSize:24,fontWeight:700,color:"var(--gold)"}}>{fmtMonto(op.monto)}</div>
                    <div style={{fontSize:12,color:"var(--text2)",marginTop:2}}>
                      {getUserName(op.emisor,users)} <span style={{color:"var(--text3)"}}>→</span> {getUserName(op.receptor,users)}
                    </div>
                  </div>
                  <div style={{display:"flex",flexDirection:"column",alignItems:"flex-end",gap:5}}>
                    <LabelChip id={op.etiqueta}/>
                    <SunatBadge state={op.sunatEstado}/>
                  </div>
                </div>

                <div style={{display:"flex",gap:10,fontSize:11,color:"var(--text3)",marginBottom:11,flexWrap:"wrap"}}>
                  <span>🏦 {op.bancoEmisor}→{op.bancoReceptor}</span>
                  <span>📅 {fmtDate(op.fecha)} {op.hora}</span>
                  <span className="mono">#{op.nroOperacion}</span>
                </div>

                <div style={{display:"flex",gap:6}}>
                  <RowBtn icon="👁"  label="Ver"    color="var(--text2)"  bg="transparent"              border="var(--border2)"                onClick={()=>setDetail(op)}/>
                  <RowBtn icon="✏️" label="Editar" color="var(--blue-xl)" bg="rgba(37,99,235,.08)"       border="rgba(37,99,235,.3)"            onClick={()=>setEdit({...op})}/>
                  <RowBtn icon="📋"  label="SUNAT"  color="var(--teal)"   bg="rgba(46,196,182,.08)"      border="rgba(46,196,182,.3)"           onClick={()=>sunat(op.id)}/>
                  <RowBtn icon="🗑"  label=""        color="#F87171"       bg="rgba(239,68,68,.08)"       border="rgba(239,68,68,.25)"           onClick={()=>del(op.id)} flex="0.6"/>
                </div>
              </div>
            ))}
          </div>
        </div>
      ))}

      {/* Detail modal */}
      {detail && (
        <Modal title="Detalle de Operación" onClose={()=>setDetail(null)}>
          {detail.foto && <img src={detail.foto} alt="comp" style={{width:"100%",borderRadius:10,marginBottom:14,objectFit:"cover",maxHeight:150}}/>}
          <div className="mono" style={{fontSize:30,fontWeight:800,color:"var(--gold)",textAlign:"center",marginBottom:14}}>{fmtMonto(detail.monto)}</div>
          {[
            ["N° Operación",  detail.nroOperacion],
            ["Fecha",         fmtDate(detail.fecha)],
            ["Hora",          detail.hora],
            ["Emisor",        `${getUserName(detail.emisor,users)} (DNI ${detail.emisor})`],
            ["Receptor",      `${getUserName(detail.receptor,users)} (DNI ${detail.receptor})`],
            ["Banco Emisor",  detail.bancoEmisor],
            ["Banco Receptor",detail.bancoReceptor],
            ["SUNAT",         detail.sunatEstado==="ok"?"✅ OK":"⏳ Pendiente"],
            ["Nota",          detail.nota||"—"],
          ].map(([k,v])=>(
            <div key={k} style={{display:"flex",justifyContent:"space-between",padding:"7px 0",borderBottom:"1px solid var(--border)",fontSize:13}}>
              <span style={{color:"var(--text2)"}}>{k}</span>
              <span style={{fontWeight:500,maxWidth:"58%",textAlign:"right"}}>{v}</span>
            </div>
          ))}
        </Modal>
      )}

      {/* Edit modal */}
      {edit && (
        <Modal title="✏️ Editar Operación" onClose={()=>setEdit(null)}>
          <div style={{display:"flex",flexDirection:"column",gap:9}}>
            <input className="field mono" placeholder="Monto"         value={edit.monto}         onChange={e=>setEdit(p=>({...p,monto:e.target.value}))}/>
            <input className="field"      placeholder="Fecha (YYYY-MM-DD)" value={edit.fecha}    onChange={e=>setEdit(p=>({...p,fecha:e.target.value}))}/>
            <input className="field mono" placeholder="N° Operación"  value={edit.nroOperacion} onChange={e=>setEdit(p=>({...p,nroOperacion:e.target.value}))}/>
            <input className="field"      placeholder="Nota"           value={edit.nota||""}     onChange={e=>setEdit(p=>({...p,nota:e.target.value}))}/>
          </div>
          <div style={{display:"flex",gap:10,marginTop:14}}>
            <button className="btn btn-ghost"   style={{flex:1}} onClick={()=>setEdit(null)}>Cancelar</button>
            <button className="btn btn-primary" style={{flex:1}} onClick={saveEd}>Guardar</button>
          </div>
        </Modal>
      )}
    </div>
  );
}

/* ═══════════════════════════════════════════════════════════
   PAGE: BUSCAR
═══════════════════════════════════════════════════════════ */
function PageBuscar({ operations, users }) {
  const [q, setQ]                     = useState("");
  const [showF, setShowF]             = useState(false);
  const [filters, setFilters]         = useState({desde:"",hasta:"",banco:"",montoMin:"",montoMax:"",etiqueta:""});
  const setF = k => v => setFilters(p=>({...p,[k]:v}));

  const filtered = operations.filter(op=>{
    const eN=getUserName(op.emisor,users).toLowerCase(), rN=getUserName(op.receptor,users).toLowerCase();
    const qq=q.toLowerCase();
    return (
      (!qq || eN.includes(qq)||rN.includes(qq)||op.emisor.includes(qq)||op.receptor.includes(qq)||op.nroOperacion?.includes(qq)) &&
      (!filters.desde   || op.fecha>=filters.desde) &&
      (!filters.hasta   || op.fecha<=filters.hasta) &&
      (!filters.banco   || op.bancoEmisor===filters.banco||op.bancoReceptor===filters.banco) &&
      (!filters.montoMin|| +op.monto>=+filters.montoMin) &&
      (!filters.montoMax|| +op.monto<=+filters.montoMax) &&
      (!filters.etiqueta|| op.etiqueta===filters.etiqueta)
    );
  });

  const total = filtered.reduce((a,o)=>a+(+o.monto),0);
  const avg   = filtered.length ? total/filtered.length : 0;

  /* bank bar chart */
  const bTotals={};
  filtered.forEach(o=>{ bTotals[o.bancoEmisor]=(bTotals[o.bancoEmisor]||0)+(+o.monto); });
  const topBanks=Object.entries(bTotals).sort((a,b)=>b[1]-a[1]).slice(0,5);
  const maxBT=Math.max(...topBanks.map(x=>x[1]),1);

  return (
    <div className="fade-up" style={{padding:16,display:"flex",flexDirection:"column",gap:13}}>
      {/* Search bar */}
      <div style={{position:"relative"}}>
        <span style={{position:"absolute",left:12,top:"50%",transform:"translateY(-50%)",fontSize:16,color:"var(--text3)"}}>🔍</span>
        <input className="field" placeholder="Nombre, DNI, N° operación…" value={q} onChange={e=>setQ(e.target.value)} style={{paddingLeft:38,paddingRight:42}}/>
        <button onClick={()=>setShowF(s=>!s)} style={{position:"absolute",right:10,top:"50%",transform:"translateY(-50%)",background:"none",border:"none",cursor:"pointer",fontSize:18,color:showF?"var(--blue-xl)":"var(--text3)"}}>
          ⚙️
        </button>
      </div>

      {/* Filters */}
      {showF && (
        <div className="glass fade-up" style={{padding:14}}>
          <SectionLabel>Filtros avanzados</SectionLabel>
          <div style={{display:"grid",gridTemplateColumns:"1fr 1fr",gap:8,marginBottom:8}}>
            <input className="field" type="date" value={filters.desde}    onChange={e=>setF("desde")(e.target.value)}    style={{fontSize:12}}/>
            <input className="field" type="date" value={filters.hasta}    onChange={e=>setF("hasta")(e.target.value)}    style={{fontSize:12}}/>
            <input className="field mono"        placeholder="Monto mín" value={filters.montoMin} onChange={e=>setF("montoMin")(e.target.value)} style={{fontSize:12}}/>
            <input className="field mono"        placeholder="Monto máx" value={filters.montoMax} onChange={e=>setF("montoMax")(e.target.value)} style={{fontSize:12}}/>
          </div>
          <select className="field" value={filters.banco}    onChange={e=>setF("banco")(e.target.value)}    style={{fontSize:12,marginBottom:8}}>
            <option value="">Todos los bancos</option>
            {BANKS.map(b=><option key={b}>{b}</option>)}
          </select>
          <select className="field" value={filters.etiqueta} onChange={e=>setF("etiqueta")(e.target.value)} style={{fontSize:12,marginBottom:8}}>
            <option value="">Todas las etiquetas</option>
            {LABELS.map(l=><option key={l.id} value={l.id}>{l.text}</option>)}
          </select>
          <button className="btn btn-ghost" style={{width:"100%",fontSize:12}} onClick={()=>setFilters({desde:"",hasta:"",banco:"",montoMin:"",montoMax:"",etiqueta:""})}>
            🗑 Limpiar filtros
          </button>
        </div>
      )}

      {/* Stats row */}
      <div style={{display:"grid",gridTemplateColumns:"1fr 1fr 1fr",gap:8}}>
        <StatCard icon="📊" label="Ops." value={filtered.length} accent="var(--blue-l)"/>
        <StatCard icon="💰" label="Total" value={`S/ ${Math.round(total).toLocaleString()}`} accent="var(--gold)"/>
        <StatCard icon="📈" label="Prom." value={`S/ ${Math.round(avg).toLocaleString()}`}   accent="var(--teal)"/>
      </div>

      {/* Bank chart */}
      {topBanks.length>0 && (
        <div className="glass" style={{padding:14}}>
          <SectionLabel>Top bancos emisores</SectionLabel>
          {topBanks.map(([bank,val])=>(
            <div key={bank} style={{marginBottom:8}}>
              <div style={{display:"flex",justifyContent:"space-between",fontSize:12,marginBottom:3}}>
                <span style={{color:"var(--text)"}}>{bank}</span>
                <span className="mono" style={{color:"var(--gold)",fontSize:11}}>{fmtMonto(val)}</span>
              </div>
              <div style={{background:"rgba(255,255,255,.07)",borderRadius:4,height:7,overflow:"hidden"}}>
                <div style={{width:`${(val/maxBT)*100}%`,height:"100%",background:"linear-gradient(90deg,var(--blue),var(--teal))",borderRadius:4,transition:"width .8s ease"}}/>
              </div>
            </div>
          ))}
        </div>
      )}

      {/* Results */}
      <div style={{display:"flex",flexDirection:"column",gap:8}}>
        {filtered.length===0 && (
          <div style={{textAlign:"center",padding:36,color:"var(--text3)"}}>
            <div style={{fontSize:36}}>🔍</div>
            <div style={{marginTop:8,fontSize:13}}>Sin resultados para esta búsqueda</div>
          </div>
        )}
        {filtered.map(op=>(
          <div key={op.id} className="glass" style={{padding:"11px 14px",display:"flex",justifyContent:"space-between",alignItems:"center"}}>
            <div>
              <div style={{fontSize:12,color:"var(--text)"}}>
                {getUserName(op.emisor,users)} <span style={{color:"var(--text3)"}}>→</span> {getUserName(op.receptor,users)}
              </div>
              <div style={{fontSize:11,color:"var(--text3)",marginTop:2}}>{op.bancoEmisor} · {fmtDate(op.fecha)}</div>
            </div>
            <div style={{display:"flex",flexDirection:"column",alignItems:"flex-end",gap:4}}>
              <span className="mono" style={{fontSize:16,fontWeight:700,color:"var(--gold)"}}>{fmtMonto(op.monto)}</span>
              <LabelChip id={op.etiqueta}/>
            </div>
          </div>
        ))}
      </div>
    </div>
  );
}

/* ═══════════════════════════════════════════════════════════
   PAGE: USUARIOS
═══════════════════════════════════════════════════════════ */
function PageUsuarios({ users, setUsers, operations, setPage }) {
  const [form, setForm]     = useState({dni:"",nombre:"",bancoPrincipal:"",nota:""});
  const [open, setOpen]     = useState(false);
  const [err,  setErr]      = useState("");
  const setF = k => v => setForm(p=>({...p,[k]:v}));

  const add = () => {
    if (!form.dni || form.dni.length!==8)  { setErr("El DNI debe tener 8 dígitos."); return; }
    if (!form.nombre.trim())               { setErr("Ingresa el nombre."); return; }
    if (users.find(u=>u.dni===form.dni))   { setErr("Ya existe un usuario con ese DNI."); return; }
    setUsers(p=>[...p,{...form,cuentas:[]}]);
    setForm({dni:"",nombre:"",bancoPrincipal:"",nota:""});
    setErr(""); setOpen(false);
  };

  /* gradient colors by index */
  const GRAD=[
    ["#1A4FA0","#2EC4B6"],["#9B59B6","#2563EB"],["#D4A843","#FF6B35"],["#22C55E","#2EC4B6"],
  ];

  return (
    <div className="fade-up" style={{padding:16}}>
      <button className="btn btn-primary" style={{width:"100%",marginBottom:14}} onClick={()=>{setOpen(o=>!o);setErr("");}}>
        {open?"✕ Cancelar":"➕ Nuevo usuario"}
      </button>

      {open && (
        <div className="glass fade-up" style={{padding:16,marginBottom:14}}>
          <SectionLabel>Nuevo usuario</SectionLabel>
          <div style={{display:"flex",flexDirection:"column",gap:8}}>
            <input className="field mono" placeholder="DNI (8 dígitos)" value={form.dni}          onChange={e=>setF("dni")(e.target.value)}          maxLength={8}/>
            <input className="field"      placeholder="Nombre completo" value={form.nombre}        onChange={e=>setF("nombre")(e.target.value)}/>
            <select className="field"                                    value={form.bancoPrincipal} onChange={e=>setF("bancoPrincipal")(e.target.value)}>
              <option value="">Banco principal…</option>
              {BANKS.map(b=><option key={b}>{b}</option>)}
            </select>
            <input className="field" placeholder="Nota opcional" value={form.nota} onChange={e=>setF("nota")(e.target.value)}/>
            {err && <div style={{fontSize:12,color:"#F87171"}}>{err}</div>}
            <button className="btn btn-primary" onClick={add}>Guardar usuario</button>
          </div>
        </div>
      )}

      {users.length===0 && (
        <div style={{textAlign:"center",padding:40,color:"var(--text3)"}}>
          <div style={{fontSize:40}}>👥</div>
          <div style={{marginTop:8}}>Sin usuarios registrados</div>
        </div>
      )}

      <div style={{display:"flex",flexDirection:"column",gap:10}}>
        {users.map((u,i)=>{
          const uOps=operations.filter(o=>o.emisor===u.dni||o.receptor===u.dni);
          const uTotal=uOps.reduce((a,o)=>a+(+o.monto),0);
          const [g1,g2]=GRAD[i%GRAD.length];
          return (
            <div key={u.dni} className="glass lift" style={{padding:16}}>
              <div style={{display:"flex",gap:14,alignItems:"flex-start"}}>
                {/* Avatar */}
                <div style={{width:50,height:50,borderRadius:"50%",background:`linear-gradient(135deg,${g1},${g2})`,display:"flex",alignItems:"center",justifyContent:"center",fontSize:18,fontWeight:700,color:"white",flexShrink:0,boxShadow:`0 4px 14px ${g1}55`}}>
                  {initials(u.nombre)}
                </div>
                <div style={{flex:1}}>
                  <div style={{fontSize:15,fontWeight:700,marginBottom:2}}>{u.nombre}</div>
                  <div className="mono" style={{fontSize:11,color:"var(--text2)"}}>DNI: {u.dni}</div>
                  {u.bancoPrincipal && <div style={{fontSize:12,color:"var(--teal)",marginTop:3}}>🏦 {u.bancoPrincipal}</div>}
                  <div style={{display:"flex",gap:14,marginTop:7}}>
                    <span style={{fontSize:11,color:"var(--text2)"}}>📊 {uOps.length} ops.</span>
                    <span className="mono" style={{fontSize:11,color:"var(--gold)",fontWeight:600}}>{fmtMonto(uTotal)}</span>
                  </div>
                  {u.cuentas?.length>0 && (
                    <div style={{marginTop:8,display:"flex",flexWrap:"wrap",gap:4}}>
                      {u.cuentas.map((c,j)=>(
                        <span key={j} style={{fontSize:10,background:"rgba(26,79,160,.2)",border:"1px solid rgba(26,79,160,.3)",borderRadius:6,padding:"2px 7px",color:"var(--blue-xl)"}}>
                          {c.banco}: {c.numero}
                        </span>
                      ))}
                    </div>
                  )}
                  {u.nota && <div style={{fontSize:11,color:"var(--text3)",marginTop:6,fontStyle:"italic"}}>"{u.nota}"</div>}
                </div>
              </div>
              <div style={{display:"flex",gap:7,marginTop:12}}>
                <RowBtn icon="🔍" label="Ver ops."  color="var(--blue-xl)" bg="rgba(37,99,235,.08)" border="rgba(37,99,235,.3)" onClick={()=>setPage("buscar")} flex={2}/>
                <RowBtn icon="🗑"  label="Eliminar" color="#F87171"         bg="rgba(239,68,68,.08)" border="rgba(239,68,68,.25)" onClick={()=>setUsers(p=>p.filter(x=>x.dni!==u.dni))}/>
              </div>
            </div>
          );
        })}
      </div>
    </div>
  );
}

/* ═══════════════════════════════════════════════════════════
   PAGE: CONFIG
═══════════════════════════════════════════════════════════ */
function PageConfig({ darkMode, setDarkMode, operations, users }) {
  const [driveUrl,  setDriveUrl]  = useState("");
  const [driveS,    setDriveS]    = useState(null); // null|ok|error|syncing
  const [fontSize,  setFontSize]  = useState("normal");
  const [limit,     setLimit]     = useState("");
  const [dayModal,  setDayModal]  = useState(false);

  const testDrive = () => {
    setDriveS("syncing");
    // TODO: syncToGoogleDrive(driveUrl, { operations, users })
    setTimeout(()=>setDriveS(driveUrl?"ok":"error"),1600);
  };

  /* quick stats */
  const thisM = new Date().toISOString().slice(0,7);
  const mOps  = operations.filter(o=>o.fecha?.startsWith(thisM));
  const mTotal= mOps.reduce((a,o)=>a+(+o.monto),0);

  const bCount={}; operations.forEach(o=>{ bCount[o.bancoEmisor]=(bCount[o.bancoEmisor]||0)+1; });
  const topBank= Object.entries(bCount).sort((a,b)=>b[1]-a[1])[0]?.[0]||"—";

  const rCount={}; operations.forEach(o=>{ rCount[o.receptor]=(rCount[o.receptor]||0)+1; });
  const topRec = Object.entries(rCount).sort((a,b)=>b[1]-a[1])[0]?.[0];
  const topRecN= topRec ? getUserName(topRec,users):"—";

  const lsOk = (()=>{ try{ localStorage.setItem("_chk","1"); localStorage.removeItem("_chk"); return true; } catch{ return false; } })();

  const dayResumen = () => {
    const today=new Date().toISOString().slice(0,10);
    const todayOps=operations.filter(o=>o.fecha===today);
    if (!todayOps.length) return "No hay operaciones registradas hoy.";
    const t=todayOps.reduce((a,o)=>a+(+o.monto),0);
    return `📋 RESUMEN DEL ${fmtDate(today)}\n${"─".repeat(36)}\nTotal operaciones: ${todayOps.length}\nMonto total:       ${fmtMonto(t)}\n${"─".repeat(36)}\n\n`+
      todayOps.map(o=>`• ${fmtMonto(o.monto).padEnd(14)} ${getUserName(o.emisor,users)} → ${getUserName(o.receptor,users)}\n  ${o.bancoEmisor}→${o.bancoReceptor}  Op.${o.nroOperacion}`).join("\n\n");
  };

  return (
    <div className="fade-up" style={{padding:16,display:"flex",flexDirection:"column",gap:13}}>

      {/* Quick stats */}
      <div className="glass" style={{padding:16,background:"linear-gradient(135deg,rgba(26,79,160,.18),rgba(46,196,182,.09))"}}>
        <SectionLabel>📊 resumen rápido</SectionLabel>
        <div style={{display:"grid",gridTemplateColumns:"1fr 1fr 1fr",gap:8}}>
          <div style={{textAlign:"center"}}>
            <div className="mono" style={{fontSize:15,fontWeight:700,color:"var(--gold)"}}>{fmtMonto(mTotal)}</div>
            <div style={{fontSize:10,color:"var(--text3)"}}>Mes actual</div>
          </div>
          <div style={{textAlign:"center"}}>
            <div style={{fontSize:13,fontWeight:600,color:"var(--teal)"}}>{topBank}</div>
            <div style={{fontSize:10,color:"var(--text3)"}}>Top banco</div>
          </div>
          <div style={{textAlign:"center"}}>
            <div style={{fontSize:12,fontWeight:600,color:"var(--purple)",wordBreak:"break-word"}}>{topRecN}</div>
            <div style={{fontSize:10,color:"var(--text3)"}}>Top receptor</div>
          </div>
        </div>
      </div>

      {/* Personalization */}
      <div className="glass" style={{padding:16}}>
        <SectionLabel>🎨 personalización</SectionLabel>
        <div style={{display:"flex",justifyContent:"space-between",alignItems:"center",marginBottom:14}}>
          <span style={{fontSize:14}}>🌙 Modo oscuro</span>
          <button className="toggle-track btn" onClick={()=>setDarkMode(d=>!d)}
            style={{background:darkMode?"linear-gradient(135deg,var(--blue),var(--blue-l))":"#374151"}}>
            <div className="toggle-thumb" style={{left:darkMode?26:3}}/>
          </button>
        </div>
        <div style={{fontSize:13,marginBottom:8,color:"var(--text2)"}}>Tamaño de texto</div>
        <div style={{display:"flex",gap:6}}>
          {["small","normal","large"].map(s=>(
            <button key={s} className="btn" onClick={()=>setFontSize(s)} style={{
              flex:1,padding:"7px 0",borderRadius:"var(--radius-xs)",fontFamily:"Sora",fontSize:12,fontWeight:600,textTransform:"capitalize",
              border:`1.5px solid ${fontSize===s?"var(--blue-l)":"var(--border2)"}`,
              background:fontSize===s?"rgba(37,99,235,.15)":"transparent",
              color:fontSize===s?"var(--blue-xl)":"var(--text2)",
            }}>{s}</button>
          ))}
        </div>
      </div>

      {/* Google Drive */}
      <div className="glass" style={{padding:16}}>
        <SectionLabel>☁️ google drive / apps script</SectionLabel>
        <input className="field" placeholder="https://script.google.com/macros/s/…" value={driveUrl} onChange={e=>setDriveUrl(e.target.value)} style={{fontSize:12,marginBottom:8}}/>
        <div style={{display:"flex",gap:8}}>
          <button className="btn btn-ghost" style={{flex:1,fontSize:12}} onClick={testDrive}>🔌 Probar</button>
          <button className="btn btn-primary" style={{flex:1,fontSize:12}} onClick={testDrive}>🔄 Sincronizar</button>
        </div>
        {driveS && (
          <div style={{marginTop:10,textAlign:"center",fontSize:12,
            color:driveS==="ok"?"var(--teal)":driveS==="error"?"#F87171":"var(--gold)"}}>
            {driveS==="ok"?"✅ Conectado":driveS==="error"?"❌ Error de conexión":<span className="blink">⏳ Sincronizando…</span>}
          </div>
        )}
      </div>

      {/* Export / Import */}
      <div className="glass" style={{padding:16}}>
        <SectionLabel>💾 exportar / importar</SectionLabel>
        <div style={{display:"grid",gridTemplateColumns:"1fr 1fr",gap:8}}>
          {["📊 Exportar Excel","📄 Exportar PDF","💾 Backup JSON","📥 Importar"].map(lbl=>(
            <button key={lbl} className="btn btn-ghost" style={{fontSize:12,padding:"10px 8px"}}
              onClick={()=>alert(`${lbl} — Servicio pendiente de implementación`)}>
              {lbl}
            </button>
          ))}
        </div>
      </div>

      {/* Daily limit */}
      <div className="glass" style={{padding:16}}>
        <SectionLabel>🚦 límite diario</SectionLabel>
        <input className="field mono" placeholder="Límite S/ por día…" value={limit} onChange={e=>setLimit(e.target.value)} style={{fontSize:13}}/>
        {limit && <div style={{fontSize:12,color:"var(--gold)",marginTop:7}}>⚠️ Límite configurado: {fmtMonto(+limit||0)}</div>}
      </div>

      {/* Resumen del día */}
      <button className="btn btn-gold" style={{width:"100%",fontSize:14}} onClick={()=>setDayModal(true)}>
        📋 Generar resumen del día
      </button>

      {/* System status */}
      <div className="glass" style={{padding:16}}>
        <SectionLabel>🔧 estado del sistema</SectionLabel>
        {[
          ["localStorage",    lsOk  ?"✅ Operativo":"❌ Error",         lsOk],
          ["Tesseract (stub)", true  ?"✅ Listo (stub)":"❌",            true],
          ["Claude Vision",   true  ?"✅ Hook listo (stub)":"❌",       true],
          ["Drive URL",       !!driveUrl?"✅ Configurada":"⚠️ Sin URL", !!driveUrl],
        ].map(([k,v,ok])=>(
          <div key={k} style={{display:"flex",justifyContent:"space-between",padding:"6px 0",borderBottom:"1px solid var(--border)",fontSize:12}}>
            <span style={{color:"var(--text2)"}}>{k}</span>
            <span style={{color:ok?"var(--teal)":"var(--gold)",fontWeight:600}}>{v}</span>
          </div>
        ))}
        <div style={{fontSize:11,color:"var(--text3)",marginTop:8}}>v1.0.0 · Gestor de Transferencias BCP</div>
      </div>

      {dayModal && (
        <Modal title="📋 Resumen del día" onClose={()=>setDayModal(false)}>
          <pre className="mono" style={{fontSize:11,color:"#E2E8F0",background:"rgba(0,0,0,.35)",borderRadius:10,padding:"12px 14px",whiteSpace:"pre-wrap",lineHeight:1.7,maxHeight:260,overflowY:"auto"}}>
            {dayResumen()}
          </pre>
          <div style={{display:"flex",gap:8,marginTop:12}}>
            <button className="btn btn-ghost"   style={{flex:1}} onClick={()=>navigator.clipboard?.writeText(dayResumen())}>📋 Copiar</button>
            <button className="btn btn-primary" style={{flex:1}} onClick={()=>setDayModal(false)}>Cerrar</button>
          </div>
        </Modal>
      )}
    </div>
  );
}

/* ═══════════════════════════════════════════════════════════
   BOTTOM NAV
═══════════════════════════════════════════════════════════ */
function BottomNav({ page, setPage }) {
  return (
    <nav className="nav-blur" style={{
      position:"fixed",bottom:0,left:"50%",transform:"translateX(-50%)",
      width:"100%",maxWidth:480,
      display:"flex",padding:"7px 0 calc(7px + env(safe-area-inset-bottom))",zIndex:50,
    }}>
      {TABS.map(tab=>{
        const active = page===tab.id;
        return (
          <button key={tab.id} className="btn" onClick={()=>setPage(tab.id)} style={{
            flex:1,background:"none",border:"none",
            display:"flex",flexDirection:"column",alignItems:"center",gap:2,
            padding:"3px 0",position:"relative",
          }}>
            {active && (
              <div style={{
                position:"absolute",top:0,left:"50%",transform:"translateX(-50%)",
                width:32,height:3,
                background:"linear-gradient(90deg,var(--blue),var(--teal))",
                borderRadius:"0 0 4px 4px",
              }}/>
            )}
            <span style={{fontSize:21,transition:"all .2s",filter:active?"none":"grayscale(50%)",opacity:active?1:.45}}>
              {tab.icon}
            </span>
            <span style={{fontSize:9.5,fontFamily:"Sora",fontWeight:active?700:400,transition:"color .2s",
              color:active?"var(--blue-xl)":"var(--text3)"}}>
              {tab.label}
            </span>
          </button>
        );
      })}
    </nav>
  );
}

/* ═══════════════════════════════════════════════════════════
   TOP HEADER
═══════════════════════════════════════════════════════════ */
function TopBar({ page, opCount }) {
  const tab = TABS.find(t=>t.id===page);
  return (
    <header style={{
      position:"sticky",top:0,zIndex:40,
      background:"rgba(7,9,13,.9)",backdropFilter:"blur(24px)",WebkitBackdropFilter:"blur(24px)",
      borderBottom:"1px solid rgba(255,255,255,.055)",
      padding:"11px 18px",
      display:"flex",alignItems:"center",gap:12,
    }}>
      {/* Logo */}
      <div style={{
        width:38,height:38,borderRadius:11,flexShrink:0,
        background:"linear-gradient(135deg,#1A4FA0,#2563EB)",
        display:"flex",alignItems:"center",justifyContent:"center",fontSize:19,
        boxShadow:"0 4px 14px rgba(26,79,160,.5)",
      }}>🏦</div>

      <div style={{flex:1}}>
        <div style={{fontSize:14,fontWeight:700,letterSpacing:.2,lineHeight:1.1}}>
          Gestor de Transferencias
        </div>
        <div style={{fontSize:11,color:"var(--teal)",fontWeight:600,marginTop:1}}>
          {tab?.icon} {tab?.label}
        </div>
      </div>

      {/* Right side */}
      <div style={{display:"flex",alignItems:"center",gap:8}}>
        <div style={{textAlign:"right"}}>
          <div className="mono" style={{fontSize:13,fontWeight:700,color:"var(--gold)"}}>{opCount}</div>
          <div style={{fontSize:9,color:"var(--text3)"}}>operaciones</div>
        </div>
        <div style={{display:"flex",alignItems:"center",gap:4}}>
          <div className="blink" style={{width:7,height:7,borderRadius:"50%",background:"var(--teal)"}}/>
          <span style={{fontSize:10,color:"var(--teal)",fontWeight:700}}>BCP</span>
        </div>
      </div>
    </header>
  );
}

/* ═══════════════════════════════════════════════════════════
   ROOT APP
═══════════════════════════════════════════════════════════ */
export default function App() {
  const [page,       setPage]      = useState("registrar");
  const [darkMode,   setDarkMode]  = useState(true);
  const [operations, setOperations]= useLocalStorage("bcp_v2_ops",   MOCK_OPS);
  const [users,      setUsers]     = useLocalStorage("bcp_v2_users", MOCK_USERS);

  const pages = {
    registrar: <PageRegistrar operations={operations} setOperations={setOperations} users={users}/>,
    historial: <PageHistorial operations={operations} setOperations={setOperations} users={users}/>,
    buscar:    <PageBuscar    operations={operations} users={users}/>,
    usuarios:  <PageUsuarios  users={users} setUsers={setUsers} operations={operations} setPage={setPage}/>,
    config:    <PageConfig    darkMode={darkMode} setDarkMode={setDarkMode} operations={operations} users={users}/>,
  };

  return (
    <div className={darkMode?"":"theme-light"} style={{minHeight:"100vh",background:"var(--bg)"}}>
      <GlobalStyles/>
      <div className="app-shell">
        <TopBar page={page} opCount={operations.length}/>
        <main style={{paddingBottom:88,minHeight:"calc(100vh - 64px)"}}>
          {pages[page]}
        </main>
        <BottomNav page={page} setPage={setPage}/>
      </div>
    </div>
  );
}
