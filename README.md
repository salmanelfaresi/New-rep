\begin{tikzpicture}[node distance=1cm and 1.5cm,
    mynode/.style={rectangle,draw,align=center,minimum height=1.2cm}]
  
  % Level 1
  \node[mynode] (pres) {Presiden Direktur};
  \node[mynode,below=of pres] (vpfin) {Wakil Presiden Direktur Keuangan};
  \node[mynode,left=of vpfin] (vpprod) {Wakil Presiden Direktur Produksi};
  \node[mynode,right=of vpfin] (vpmar) {Wakil Presiden Direktur Pemasaran};
  
  % Level 2
  \node[mynode,below left=of vpfin] (fd) {Direktur Finance};
  \node[mynode,below=of vpfin] (hd) {Direktur Sumber Daya Manusia};
  \node[mynode,below right=of vpfin] (opd) {Direktur Operasi};
  
  \node[mynode,below left=of vpprod] (rfd) {Direktur R&D dan Teknologi};
  \node[mynode,below right=of vpprod] (pd) {Direktur Produksi Makanan dan Minuman};
  
  \node[mynode,below left=of vpmar] (idd) {Direktur Bisnis Indofood CBP};
  \node[mynode,below right=of vpmar] (imd) {Direktur Bisnis Indofood Agri};
  
  % Level 3
  \node[mynode,below left=of hd] (hcr) {Kepala Divisi SDM};
  \node[mynode,below right=of hd] (hcd) {Kepala Divisi Hukum};
  
  \node[mynode,below=of opd] (cfo) {Chief Financial Officer};
  \node[mynode,below=of cfo] (cd) {Kepala Divisi Akuntansi};
  
  \node[mynode,below left=of pd] (mdp) {Manajer Divisi Produksi};
  \node[mynode,below right=of pd] (mdm) {Manajer Divisi Pemasaran};
  
  \node[mynode,below left=of idd] (ibd) {Direktur Bisnis Indofood Noodle};
  \node[mynode,below=of idd] (icd) {Direktur Bisnis Indofood Snack};
  \node[mynode,below right=of idd] (ipd) {Direktur Bisnis Indofood Seasoning};
  
  \node[mynode,below left=of imd] (iaed) {Direktur Bisnis Indofood Agribisnis dan Distribusi};
  \node[mynode,below right=of imd] (iap) {Direktur Bisnis Indofood Agri Plantation};
  
  % Connectors
  \draw[->] (pres) -- (vpfin);
  \draw[->] (pres) -- (vpprod);
  \draw[->] (pres) -- (vpmar);
  
  \draw[->] (vpfin) -- (fd);
  \draw
