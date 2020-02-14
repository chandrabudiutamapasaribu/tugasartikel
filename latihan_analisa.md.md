---


---

<p>Profil Saya:</p>
<blockquote>
<p><a href="https://github.com/chandrabudiutamapasaribu">chandrabudiutamapasaribu</a></p>
</blockquote>
<h1 id="perbedaan-antara-class-component-dan-functional-component">Perbedaan antara Class Component dan Functional Component</h1>
<blockquote>
<p>class componen</p>
</blockquote>
<pre class=" language-js"><code class="prism  language-js"><span class="token keyword">class</span> <span class="token class-name">Nama</span> <span class="token keyword">extends</span> <span class="token class-name">Component</span> <span class="token punctuation">{</span>
  <span class="token function">render</span><span class="token punctuation">(</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
    <span class="token keyword">return</span> <span class="token punctuation">(</span>
      <span class="token operator">&lt;</span>div className<span class="token operator">=</span><span class="token string">"test"</span><span class="token operator">&gt;</span>
        <span class="token operator">&lt;</span>p className<span class="token operator">=</span><span class="token string">"initext"</span><span class="token operator">&gt;</span>Header<span class="token operator">&lt;</span><span class="token operator">/</span>p<span class="token operator">&gt;</span>
      <span class="token operator">&lt;</span><span class="token operator">/</span>div<span class="token operator">&gt;</span>
    <span class="token punctuation">)</span><span class="token punctuation">;</span>
  <span class="token punctuation">}</span>
<span class="token punctuation">}</span>

<span class="token keyword">export</span> <span class="token keyword">default</span> Nama<span class="token punctuation">;</span>
</code></pre>
<blockquote>
<p>funtional componen</p>
</blockquote>
<pre><code>
const Nama = () =&gt; {
  return (
    &lt;div className="test"&gt;
      &lt;p className="initext"&gt;Header&lt;/p&gt;
    &lt;/div&gt;
  );
};

export default Nama;
</code></pre>
<ul>
<li>class componen memliki state,sedangan functional component hanya mengoper props saja</li>
<li>mampu biasa digunakan mengolah data,sedangan functional biasa digunakan untuk  keperluan UI nya saja.</li>
<li>functional componen tidak memilii constructor</li>
</ul>
<h1 id="perbedaan-antara-state-dan-props">Perbedaan antara State dan Props</h1>
<ul>
<li>state tidak dapat diakses oleh komponen lain</li>
<li>pada class componen,state merupakan private data,sedangkan props adalah properti,dan paramater jika di functional component.</li>
<li>props lebih dinamis karena dapat di panggil dan diedit di manapun,sedangkan state harus di edit didalam komponen itu sendiri.</li>
</ul>
<h1 id="perbedaan-antara-virtual-dom-dan-real-dom">Perbedaan antara Virtual DOM dan Real DOM</h1>
<p>DOM adalah singkatan dari Document Object Model,dengan DOM kita mampu mengedit,menghapus,dan mengakses dokument /tag pada html.Perbedaan antara Real DOM dengan Virtual Dom terletak pada ke efisienanya,karena Real DOM tidak dianjurkan untuk aplikasi skala besar,karena akan membutuhkan waktu untuk mengedit  beberapa tag/document pada DOM secara langsung.Sedangkan Virtual DOM dibuat dengan membuat abstraksi DOM dalam bentuk virtual</p>

