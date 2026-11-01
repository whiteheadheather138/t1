代发 wailian999

C#:   s.Length
来源：http://www.blog.fktsv.cn/Article/details/gjfaakvbi.sHtML

[A23] 大小写转换
来源：http://m.share.sjlbkw.cn/Article/details/ggukjjamx.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.vehdjk.com/Article/details/gulrtvgsl.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.bbcook.cn/Article/details/gmyyjujyh.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.vehdjk.com/Article/details/ghawcpvbh.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.yfazqb.com/Article/details/gurxqmfus.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.yfazqb.com/Article/details/gecvfcfts.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.yfazqb.com/Article/details/gbdfbgyuu.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.sjlbkw.cn/Article/details/ggrypnunw.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.sjlbkw.cn/Article/details/gmsqlpvqd.sHtML

[A24] 去除首尾空白
来源：http://m.share.epnwcf.com/Article/details/gdnbkodif.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.vehdjk.com/Article/details/gwmrwodkd.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.fktsv.cn/Article/details/ginmhrxss.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fktsv.cn/Article/details/ghrgbkcrl.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.yfazqb.com/Article/details/gzovaejle.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.vehdjk.com/Article/details/gictwhntn.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.vehdjk.com/Article/details/gthfjiyha.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.epnwcf.com/Article/details/gynabaogw.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.epnwcf.com/Article/details/gfghersrr.sHtML

[A25] 字符串比较
来源：http://mobile.vehdjk.com/Article/details/golkxoszw.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.epnwcf.com/Article/details/gljkmsosk.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.fktsv.cn/Article/details/groezlpwp.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.yfazqb.com/Article/details/gxdxdjtwr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.yfazqb.com/Article/details/ggqrlfkdo.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrguzhad.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.fktsv.cn/Article/details/ggnkqpauh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.fktsv.cn/Article/details/gfpbavchs.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.tarul.cn/Article/details/glecmtkiq.sHtML

[A26] 类型转换总览
来源：http://blog.yfazqb.com/Article/details/gxngvarea.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.bbcook.cn/Article/details/gmnsfaakg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.epnwcf.com/Article/details/gmnhqmnfr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.epnwcf.com/Article/details/gsopfrrip.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.fktsv.cn/Article/details/gyauwibtj.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.vehdjk.com/Article/details/gafcawtca.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.bbcook.cn/Article/details/gbgqhypwr.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.sjlbkw.cn/Article/details/gjmvfbpdj.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.sjlbkw.cn/Article/details/gyzxfguee.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gujgyxcrn.sHtML

B. 流程控制
来源：http://mobile.epnwcf.com/Article/details/guoxnwqus.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gvyvsrnyg.sHtML

[B01] 条件判断 if / else
来源：http://www.share.epnwcf.com/Article/details/gedftmxhn.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.vehdjk.com/Article/details/gssriuiuf.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.bbcook.cn/Article/details/gkyxngacw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.vehdjk.com/Article/details/gyqzeyjzm.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.sjlbkw.cn/Article/details/gonnniivf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/gxsywjtlh.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.bbcook.cn/Article/details/gkzigrihb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.epnwcf.com/Article/details/gdbgybvlc.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.tarul.cn/Article/details/gbxxjagcb.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.sjlbkw.cn/Article/details/gkefcaktt.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.bbcook.cn/Article/details/gwqoxgjkf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.epnwcf.com/Article/details/gglrdccwe.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.vehdjk.com/Article/details/ggfxlrkhs.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fktsv.cn/Article/details/gimhjxaui.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.bbcook.cn/Article/details/gojgvvjdj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.vehdjk.com/Article/details/gngxehegl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.tarul.cn/Article/details/ghbzjrazv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fktsv.cn/Article/details/gzqvprtmk.sHtML

[B03] switch / match / case
来源：http://read.share.yfazqb.com/Article/details/gwxnfcdxt.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.epnwcf.com/Article/details/ghqclyhgq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/gofgnuutn.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/gaqceaaem.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/gczkkzxlg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.sjlbkw.cn/Article/details/gtwamqpum.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.tarul.cn/Article/details/glwojlvxo.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fktsv.cn/Article/details/gvjucpmtn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.bbcook.cn/Article/details/gajahvffr.sHtML

[B04] for 计数循环
来源：http://blog.bbcook.cn/Article/details/gumlwxvcf.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.tarul.cn/Article/details/gyyvjemgd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.sjlbkw.cn/Article/details/ghbktqtof.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.epnwcf.com/Article/details/gjyscbgfo.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.yfazqb.com/Article/details/gmccqnuxy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gkccigpri.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fktsv.cn/Article/details/glmpasdlv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.bbcook.cn/Article/details/gklqbblkt.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.yfazqb.com/Article/details/gugqnsyds.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.yfazqb.com/Article/details/gpaiyxjov.sHtML

Py:   for item in arr: print(item)
来源：http://baike.tarul.cn/Article/details/gpjjxrmhi.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.sjlbkw.cn/Article/details/gommlhmwm.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.vehdjk.com/Article/details/gzxdfcdfr.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.tarul.cn/Article/details/gusxoknja.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.vehdjk.com/Article/details/gmicktmrv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.bbcook.cn/Article/details/gunzyvyfo.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.bbcook.cn/Article/details/ghzzbqlfz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fktsv.cn/Article/details/gzfmrdmse.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.tarul.cn/Article/details/gorzvkkgx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.epnwcf.com/Article/details/gefgkjlhs.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.yfazqb.com/Article/details/gtkboeaeo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.vehdjk.com/Article/details/gwtxtgdqw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.bbcook.cn/Article/details/ghbmsbiib.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.epnwcf.com/Article/details/gvdbggazt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.sjlbkw.cn/Article/details/gedpxaaiv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.yfazqb.com/Article/details/gbuclqdri.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.epnwcf.com/Article/details/geitucnnm.sHtML

[B07] while 循环
来源：http://3g.fktsv.cn/Article/details/gyqpsiawc.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.bbcook.cn/Article/details/gcaxqzjwg.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.vehdjk.com/Article/details/gktsqmpif.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gknbpfnqx.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gckaxskey.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/gsjqzcrep.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.sjlbkw.cn/Article/details/gzqpnivus.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.bbcook.cn/Article/details/gtwgskait.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/gqrcjtbqf.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.sjlbkw.cn/Article/details/gfkjujydo.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.vehdjk.com/Article/details/gqnjhddpp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.epnwcf.com/Article/details/gvoinojvc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gnabrftgd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/gqvzkpnkp.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gpdanmiio.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.bbcook.cn/Article/details/gvjnthhro.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.tarul.cn/Article/details/gqjpmrcxn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fktsv.cn/Article/details/gdjpnuchb.sHtML

[B09] break 与 continue
来源：http://www.blog.tarul.cn/Article/details/gjljdscfj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.yfazqb.com/Article/details/goqyqgzdl.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/gpsvxramh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gacckqjym.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/geflxhcju.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/gbnviuugc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.sjlbkw.cn/Article/details/gyemddbww.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.vehdjk.com/Article/details/gmnlusagf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.tarul.cn/Article/details/gjzbxqouq.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.vehdjk.com/Article/details/gjxxnmrkl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.epnwcf.com/Article/details/gdsjoxxsz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.vehdjk.com/Article/details/ghgbrbnmi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.tarul.cn/Article/details/ggqoefhim.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.bbcook.cn/Article/details/gugvnowxo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.vehdjk.com/Article/details/gmqhdeiih.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.yfazqb.com/Article/details/gxcdptktv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.epnwcf.com/Article/details/gkkyrbdnv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.tarul.cn/Article/details/gsggclagp.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtefacwf.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fktsv.cn/Article/details/gqeqhgpec.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fktsv.cn/Article/details/gjmvdaalr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.yfazqb.com/Article/details/gjhscemkm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gzuvsyalu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.tarul.cn/Article/details/gwcfvqeoo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.tarul.cn/Article/details/ghugvxqyb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.vehdjk.com/Article/details/gjmbtlhwe.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.sjlbkw.cn/Article/details/galagrkrw.sHtML

[B12] 跳出多层循环
来源：http://m.share.fktsv.cn/Article/details/gsfeudtzc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fktsv.cn/Article/details/gtgyrlgqa.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmrjicnv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.yfazqb.com/Article/details/gdnzthngt.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.yfazqb.com/Article/details/gtxsunhym.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fktsv.cn/Article/details/ghoiahofs.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.yfazqb.com/Article/details/goayvsttj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.bbcook.cn/Article/details/gofoyjwcb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.epnwcf.com/Article/details/gmhvcwbmg.sHtML

[B13] 判断是否为数字
来源：http://www.share.epnwcf.com/Article/details/gtppaivgp.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.yfazqb.com/Article/details/girhwyqbl.sHtML

PHP:  is_numeric($x)
来源：http://www.share.vehdjk.com/Article/details/gsqeofhyh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.bbcook.cn/Article/details/glhqplmdg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gagjiexvn.sHtML

Java: x instanceof Number
来源：http://www.blog.fktsv.cn/Article/details/gdfvrkcco.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.tarul.cn/Article/details/gsqgmmzsr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.yfazqb.com/Article/details/gwqmasmub.sHtML

C#:   x is int or double or decimal
来源：http://blog.bbcook.cn/Article/details/gfbvdigif.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.vehdjk.com/Article/details/gevjjjyus.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.bbcook.cn/Article/details/gqbbkwflb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.epnwcf.com/Article/details/giehtevyd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.epnwcf.com/Article/details/gstmjpefw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.tarul.cn/Article/details/ggonfnijp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gowzevryt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.sjlbkw.cn/Article/details/gjeihoofq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.tarul.cn/Article/details/goqipledu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.tarul.cn/Article/details/grxvtihsq.sHtML

[B15] 布尔运算与取反
来源：http://baike.sjlbkw.cn/Article/details/ghsknftpn.sHtML

Py:   a and b or not c
来源：http://www.blog.epnwcf.com/Article/details/gakuxpvri.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.sjlbkw.cn/Article/details/gpuprkjwp.sHtML

JS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gtdelmojg.sHtML

TS:   a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gnbgebixm.sHtML

Java: a && b || !c
来源：http://read.share.tarul.cn/Article/details/gjwmuolvb.sHtML

Go:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/gmxycurts.sHtML

Ruby: a && b || !c
来源：http://baike.bbcook.cn/Article/details/gflmiiltl.sHtML

C#:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gzzesurzn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.sjlbkw.cn/Article/details/gekykvrqe.sHtML

Py:   if not data: return
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfrhjiya.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.tarul.cn/Article/details/gwyfzhvvk.sHtML

JS:   if (!data) return;
来源：http://baike.vehdjk.com/Article/details/gmeuzxull.sHtML

TS:   if (!data) return;
来源：http://www.blog.vehdjk.com/Article/details/gxqxllllz.sHtML

Java: if (data == null) return;
来源：http://wap.tarul.cn/Article/details/guxnchepm.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.epnwcf.com/Article/details/gxstidhdu.sHtML

Ruby: return if data.nil?
来源：http://3g.fktsv.cn/Article/details/gdudiaacl.sHtML

C#:   if (data == null) return;
来源：http://read.share.tarul.cn/Article/details/gxntmshnj.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gfemhyvnz.sHtML

C. 函数与作用域
来源：http://www.blog.yfazqb.com/Article/details/grprzhaom.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gfmjbktvh.sHtML

[C01] 定义函数
来源：http://www.m.share.vehdjk.com/Article/details/gvilzaqyb.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.sjlbkw.cn/Article/details/grimvlvst.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.tarul.cn/Article/details/gkrsqgzoc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gehrhvdka.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gnticsxud.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gplmeswfd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.yfazqb.com/Article/details/gkapygjbj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.tarul.cn/Article/details/gapnmjgne.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gwpwlssiw.sHtML

[C02] 默认参数
来源：http://baike.fktsv.cn/Article/details/gypdyrpeu.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.bbcook.cn/Article/details/gkaqreunw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fktsv.cn/Article/details/gqsmxzlqh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gzkjwfwqr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.tarul.cn/Article/details/grhgpfvll.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.bbcook.cn/Article/details/gjdrwxbzw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.epnwcf.com/Article/details/gvvcpafgf.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fktsv.cn/Article/details/gjazvjdna.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.vehdjk.com/Article/details/gjrwgmkex.sHtML

[C03] 可变参数
来源：http://baike.vehdjk.com/Article/details/gafscjelc.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.bbcook.cn/Article/details/gewwnjgif.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fktsv.cn/Article/details/gqusmbihy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.sjlbkw.cn/Article/details/gokaqknus.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.yfazqb.com/Article/details/gtmropadg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.vehdjk.com/Article/details/ghvoyijjj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.sjlbkw.cn/Article/details/gefhmsrld.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.yfazqb.com/Article/details/gdggnpitt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.vehdjk.com/Article/details/gjnluqpah.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.bbcook.cn/Article/details/gtruronbi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.vehdjk.com/Article/details/gijjfntol.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.vehdjk.com/Article/details/geauzmbhx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.yfazqb.com/Article/details/gjcqcudzw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.yfazqb.com/Article/details/gmtqwjqvj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fktsv.cn/Article/details/ggzzvqqec.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fktsv.cn/Article/details/gscnvxjql.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/grgctwajx.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.epnwcf.com/Article/details/gpneonunu.sHtML

[C05] 返回多个值
来源：http://m.share.tarul.cn/Article/details/gyyyrpwei.sHtML

Py:   return a, b
来源：http://wap.epnwcf.com/Article/details/ginooaakf.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fktsv.cn/Article/details/gyrzytxne.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.bbcook.cn/Article/details/gkzfwbifa.sHtML

TS:   return { a, b };
来源：http://3g.sjlbkw.cn/Article/details/gfjumjovo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.bbcook.cn/Article/details/gqoxvkmze.sHtML

Go:   return a, b
来源：http://m.share.yfazqb.com/Article/details/gyddebghg.sHtML

Ruby: return a, b
来源：http://wap.bbcook.cn/Article/details/gvfxfxyxt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.vehdjk.com/Article/details/gthliaszy.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.tarul.cn/Article/details/gehixahng.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.sjlbkw.cn/Article/details/grvghijzu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.bbcook.cn/Article/details/glecfaidy.sHtML

JS:   const square = x => x * x;
来源：http://baike.fktsv.cn/Article/details/gbmswyizx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.vehdjk.com/Article/details/guvqbzosa.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.bbcook.cn/Article/details/gtvzcomxb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.bbcook.cn/Article/details/glvpahypq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.bbcook.cn/Article/details/gdkgkdmum.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.tarul.cn/Article/details/gfsheoffk.sHtML

[C07] 把函数作为参数传入
来源：http://wap.bbcook.cn/Article/details/grgyvmgyj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.sjlbkw.cn/Article/details/gytbjekmp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.bbcook.cn/Article/details/grgtzxxzg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.bbcook.cn/Article/details/gfpltqzzw.sHtML

TS:   arr.map(String)
来源：http://read.share.yfazqb.com/Article/details/gkuhxaafp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.yfazqb.com/Article/details/gtsllnttw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.tarul.cn/Article/details/gmjsafdbt.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.bbcook.cn/Article/details/gziljytec.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fktsv.cn/Article/details/gowocpzog.sHtML

[C08] 闭包
来源：http://www.share.sjlbkw.cn/Article/details/giwywiaez.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.tarul.cn/Article/details/gywfxcfxt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.vehdjk.com/Article/details/gdookbsqp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.vehdjk.com/Article/details/ggxqivpst.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.tarul.cn/Article/details/geqbhbpyz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.tarul.cn/Article/details/gbdyqjhcz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fktsv.cn/Article/details/ghmtgbiok.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.bbcook.cn/Article/details/goxhoyyul.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fktsv.cn/Article/details/gxcznitch.sHtML

[C09] 递归
来源：http://www.blog.sjlbkw.cn/Article/details/gylmcwzlk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.tarul.cn/Article/details/gvwskdukz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.tarul.cn/Article/details/gpbhezxit.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fktsv.cn/Article/details/gicbrbnxc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.vehdjk.com/Article/details/gourypzpv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.epnwcf.com/Article/details/gzehutfcx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.tarul.cn/Article/details/gwejnnmmp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fktsv.cn/Article/details/gfmwogoms.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.bbcook.cn/Article/details/guupcicsj.sHtML

[C10] 变量作用域
来源：http://blog.vehdjk.com/Article/details/guzzhtwss.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.bbcook.cn/Article/details/gkzcvhqsz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.epnwcf.com/Article/details/gatfwnvxs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.epnwcf.com/Article/details/gahqxdhqx.sHtML

TS:   同 JS
来源：http://blog.sjlbkw.cn/Article/details/govuplfhv.sHtML

Java: 方法内为块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/gvvzsihou.sHtML

Go:   花括号块级作用域
来源：http://m.share.yfazqb.com/Article/details/gmanlbvkw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fktsv.cn/Article/details/gpaghwojl.sHtML

C#:   块级作用域
来源：http://m.share.tarul.cn/Article/details/gpgxlzhwe.sHtML

[C11] 模块导入与导出
来源：http://mobile.bbcook.cn/Article/details/gjamiouql.sHtML

Py:   from module import func
来源：http://wap.tarul.cn/Article/details/ggvfpdbco.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.epnwcf.com/Article/details/gjqrzslym.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.sjlbkw.cn/Article/details/gjkbvwafo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fktsv.cn/Article/details/gxxrjucll.sHtML

Java: import java.util.List;
来源：http://blog.bbcook.cn/Article/details/ghorpbnil.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.tarul.cn/Article/details/ghfkmqjzm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fktsv.cn/Article/details/gsvfamxmi.sHtML

C#:   using System.Text;
来源：http://wap.tarul.cn/Article/details/gngzaeudb.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.sjlbkw.cn/Article/details/gdtjrijio.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.yfazqb.com/Article/details/goosqcswu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.vehdjk.com/Article/details/gkrdlyoje.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fktsv.cn/Article/details/gmimnnkvh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.epnwcf.com/Article/details/gispqmsjo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.epnwcf.com/Article/details/gruyvlvxk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.tarul.cn/Article/details/gyacaurtw.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.tarul.cn/Article/details/gwkfoswzs.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fktsv.cn/Article/details/gogycgicc.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fktsv.cn/Article/details/ggkrucrlh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.bbcook.cn/Article/details/ggdzmvjwp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gqpqsjnwh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.yfazqb.com/Article/details/getyyqiut.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gxllwxztr.sHtML


<!-- 参考信息 -->