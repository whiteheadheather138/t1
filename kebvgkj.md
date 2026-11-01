代发 wailian999

[B01] 条件判断 if / else
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlaqfnnx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.bbcook.cn/Article/details/guxixuhyc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.tarul.cn/Article/details/guvsavkrj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/guhaqrjaq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fktsv.cn/Article/details/giybmpjoq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.fktsv.cn/Article/details/gbxjdzaby.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.epnwcf.com/Article/details/gijshmgfj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.tarul.cn/Article/details/gsicxxmgz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/glkfuligq.sHtML

[B02] 多分支 else if / elif
来源：http://baike.tarul.cn/Article/details/gqaalpnel.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.fktsv.cn/Article/details/gjznauvmg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.sjlbkw.cn/Article/details/gazvbmwbz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.sjlbkw.cn/Article/details/gjxtcafvx.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.epnwcf.com/Article/details/gkcamoxxs.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/gvgjgkkek.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.bbcook.cn/Article/details/gduxeivyg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.fktsv.cn/Article/details/gkqlefioz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/gkeqqqdbt.sHtML

[B03] switch / match / case
来源：http://blog.tarul.cn/Article/details/gstvwrolg.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.yfazqb.com/Article/details/golvvyutk.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.epnwcf.com/Article/details/gywkjcklm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/giuqkumdj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fktsv.cn/Article/details/gwujwvani.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fktsv.cn/Article/details/gqrnzjmcf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.sjlbkw.cn/Article/details/gawmoyxsd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.yfazqb.com/Article/details/gbhpyrrwn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.vehdjk.com/Article/details/gatlaeqhh.sHtML

[B04] for 计数循环
来源：http://m.share.fktsv.cn/Article/details/gzabzzdvw.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.vehdjk.com/Article/details/gelhwwpqx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.bbcook.cn/Article/details/ghmzifrux.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.epnwcf.com/Article/details/ggoddkzid.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.sjlbkw.cn/Article/details/gaglusshc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.sjlbkw.cn/Article/details/gqhmedhso.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.bbcook.cn/Article/details/gmsqnljhg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.tarul.cn/Article/details/gyqbjlzqx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.bbcook.cn/Article/details/gszoscavr.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fktsv.cn/Article/details/gfjrhltlk.sHtML

Py:   for item in arr: print(item)
来源：http://baike.bbcook.cn/Article/details/gazsvyqfo.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.epnwcf.com/Article/details/gbqfyykhu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.yfazqb.com/Article/details/gvyfhbbfb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.epnwcf.com/Article/details/ghhklzqnv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.sjlbkw.cn/Article/details/gqblkesuo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.epnwcf.com/Article/details/gvuqwlkfe.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.bbcook.cn/Article/details/griwhfrmk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.yfazqb.com/Article/details/ghgyjgveb.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.bbcook.cn/Article/details/gwowaxqbn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.yfazqb.com/Article/details/gjfqkiijq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.vehdjk.com/Article/details/gjvhuntux.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.vehdjk.com/Article/details/gkdjinhkz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.vehdjk.com/Article/details/gzstwdnao.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.tarul.cn/Article/details/gyrerxhpq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.tarul.cn/Article/details/gwvrbazsa.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.epnwcf.com/Article/details/ghisyizwy.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.tarul.cn/Article/details/gjfwbdfrp.sHtML

[B07] while 循环
来源：http://www.blog.sjlbkw.cn/Article/details/gwfedftfv.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.sjlbkw.cn/Article/details/grcwfyrjf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.yfazqb.com/Article/details/gjftcrrgb.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/gtmnyxqdm.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gnhafvqre.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.epnwcf.com/Article/details/gdzmhlorb.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.yfazqb.com/Article/details/gtvilfrro.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fktsv.cn/Article/details/gpkxsvoau.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/gqyhwutpv.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fktsv.cn/Article/details/gfzilwhyz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.bbcook.cn/Article/details/ghcacldvn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.epnwcf.com/Article/details/goaxpdccg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/grxdavrrg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/gbsryaoeh.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.sjlbkw.cn/Article/details/gwxklkews.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhaulnde.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.epnwcf.com/Article/details/gbldnzqdq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/gkhcbogsc.sHtML

[B09] break 与 continue
来源：http://3g.tarul.cn/Article/details/gftrozzdl.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fktsv.cn/Article/details/gyoekmqwi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gbisrjcuz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gulcvkcbb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/ghvdeigjo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/goiicpkhq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.vehdjk.com/Article/details/gwidwpdaf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.sjlbkw.cn/Article/details/gtcpnnmck.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gmwtjohtx.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.sjlbkw.cn/Article/details/goanwdllt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.sjlbkw.cn/Article/details/gmdobgawz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.bbcook.cn/Article/details/goyokldjm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fktsv.cn/Article/details/gpxmlefpu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.yfazqb.com/Article/details/gfblakvpa.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.yfazqb.com/Article/details/gxvldlopa.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.vehdjk.com/Article/details/gjsxdeskn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.tarul.cn/Article/details/gapyaghpf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.tarul.cn/Article/details/gvfbxckcz.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.tarul.cn/Article/details/ghgbqnvqk.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.vehdjk.com/Article/details/gnjwjzyqq.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fktsv.cn/Article/details/gdvsymfcs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fktsv.cn/Article/details/gxdhixana.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.tarul.cn/Article/details/gfircudzj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fktsv.cn/Article/details/gqzjivbui.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.bbcook.cn/Article/details/grmwfpity.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.yfazqb.com/Article/details/geasxbdic.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.tarul.cn/Article/details/gjkevuacw.sHtML

[B12] 跳出多层循环
来源：http://baike.vehdjk.com/Article/details/gwbfaflin.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.vehdjk.com/Article/details/gshwrfrdt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.vehdjk.com/Article/details/gkqcvbhdo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.yfazqb.com/Article/details/grkayixpf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.epnwcf.com/Article/details/gbhtdmssr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fktsv.cn/Article/details/gwhbqjalt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.bbcook.cn/Article/details/gzxdkttqs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.vehdjk.com/Article/details/ghdubaxlg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fktsv.cn/Article/details/grtocuddc.sHtML

[B13] 判断是否为数字
来源：http://baike.sjlbkw.cn/Article/details/gqqdshwik.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.sjlbkw.cn/Article/details/gafqlgaxj.sHtML

PHP:  is_numeric($x)
来源：http://blog.bbcook.cn/Article/details/gzjplmarc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.tarul.cn/Article/details/gqaoxzyne.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.bbcook.cn/Article/details/gyqagsuus.sHtML

Java: x instanceof Number
来源：http://www.m.share.fktsv.cn/Article/details/glbjeddpd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.sjlbkw.cn/Article/details/gihykujhj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.yfazqb.com/Article/details/gvogbdecj.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.tarul.cn/Article/details/gtqkdxkhf.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.bbcook.cn/Article/details/gnmsrmcwh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fktsv.cn/Article/details/gbxznvrqb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.epnwcf.com/Article/details/gnckildsz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.bbcook.cn/Article/details/gsmuobfcg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.yfazqb.com/Article/details/gwaebcbbp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.sjlbkw.cn/Article/details/gisyxswyk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.tarul.cn/Article/details/gdkrsybfp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.yfazqb.com/Article/details/gxtkwopfa.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.epnwcf.com/Article/details/gkbnjnidz.sHtML

[B15] 布尔运算与取反
来源：http://read.share.epnwcf.com/Article/details/gwlumfxfv.sHtML

Py:   a and b or not c
来源：http://mobile.vehdjk.com/Article/details/glzogbjno.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.vehdjk.com/Article/details/ghflfpklf.sHtML

JS:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gselltfgv.sHtML

TS:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/glknixkvk.sHtML

Java: a && b || !c
来源：http://3g.fktsv.cn/Article/details/gatxoicdp.sHtML

Go:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gzxmrpkea.sHtML

Ruby: a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gerzqxakn.sHtML

C#:   a && b || !c
来源：http://wap.vehdjk.com/Article/details/gbncuxzty.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.bbcook.cn/Article/details/gmtbvcqnp.sHtML

Py:   if not data: return
来源：http://mobile.fktsv.cn/Article/details/gelwmvftj.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.vehdjk.com/Article/details/gdmwxatez.sHtML

JS:   if (!data) return;
来源：http://www.blog.sjlbkw.cn/Article/details/giemxlrjs.sHtML

TS:   if (!data) return;
来源：http://www.m.share.vehdjk.com/Article/details/geezqcfzg.sHtML

Java: if (data == null) return;
来源：http://www.m.share.epnwcf.com/Article/details/gbmakxvmh.sHtML

Go:   if data == nil { return }
来源：http://m.share.yfazqb.com/Article/details/gccvnqwit.sHtML

Ruby: return if data.nil?
来源：http://www.blog.sjlbkw.cn/Article/details/gvubuhjqa.sHtML

C#:   if (data == null) return;
来源：http://baike.vehdjk.com/Article/details/gemqilvid.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gfwaurmnn.sHtML

C. 函数与作用域
来源：http://3g.epnwcf.com/Article/details/gvsrpeuos.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gvcfwhigc.sHtML

[C01] 定义函数
来源：http://wap.tarul.cn/Article/details/gorocwzwh.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.tarul.cn/Article/details/grylzvjbf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/glncyjnpn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/ggvarpeoi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gtvaqedps.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gbbudhrhi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.tarul.cn/Article/details/gupzsxcuj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.vehdjk.com/Article/details/gswusfcpw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gywzxsgqr.sHtML

[C02] 默认参数
来源：http://baike.fktsv.cn/Article/details/gizpzqnrd.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.yfazqb.com/Article/details/gqlrekuej.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.epnwcf.com/Article/details/gkvcabomn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.yfazqb.com/Article/details/gzafulemf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gjhophtkx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fktsv.cn/Article/details/gzvfefyjl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fktsv.cn/Article/details/grydqqzpu.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.epnwcf.com/Article/details/gaylblzlc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.yfazqb.com/Article/details/gycsoattw.sHtML

[C03] 可变参数
来源：http://m.share.bbcook.cn/Article/details/gnjufofer.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.tarul.cn/Article/details/gjkfdmmrv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.tarul.cn/Article/details/gafvsoyym.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.epnwcf.com/Article/details/gvrtlvcfz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.tarul.cn/Article/details/gztxugwni.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fktsv.cn/Article/details/ghtbenywx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.vehdjk.com/Article/details/gvodyufhn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.tarul.cn/Article/details/gznkplkpk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fktsv.cn/Article/details/grpwvijbv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.epnwcf.com/Article/details/grpejuzey.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.bbcook.cn/Article/details/gwnkhrzqt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fktsv.cn/Article/details/geeuvlios.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.epnwcf.com/Article/details/gjymifpum.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.bbcook.cn/Article/details/gjwxrrscw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.tarul.cn/Article/details/gkhjuscjf.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.bbcook.cn/Article/details/goyilqwqh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.vehdjk.com/Article/details/gxfofzewv.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.sjlbkw.cn/Article/details/gdvfaldbc.sHtML

[C05] 返回多个值
来源：http://www.blog.sjlbkw.cn/Article/details/gauakdzmi.sHtML

Py:   return a, b
来源：http://read.share.fktsv.cn/Article/details/gbqpnavrm.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.tarul.cn/Article/details/gldnuzzhl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fktsv.cn/Article/details/gtdipmoaf.sHtML

TS:   return { a, b };
来源：http://mobile.yfazqb.com/Article/details/gkyffiumj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.bbcook.cn/Article/details/gxeqgdpsx.sHtML

Go:   return a, b
来源：http://www.m.share.yfazqb.com/Article/details/gcufpdngp.sHtML

Ruby: return a, b
来源：http://m.share.vehdjk.com/Article/details/gdfahaenw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.yfazqb.com/Article/details/gmvevcwvn.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.yfazqb.com/Article/details/gtnqudxeb.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.bbcook.cn/Article/details/gfsdjyham.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.bbcook.cn/Article/details/gdshrthkc.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.vehdjk.com/Article/details/ghndxutxx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.bbcook.cn/Article/details/grvcgztoo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.bbcook.cn/Article/details/gjgvqgpnf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.epnwcf.com/Article/details/gexkxcnov.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.tarul.cn/Article/details/geujohgbt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.bbcook.cn/Article/details/gfmjqbahx.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fktsv.cn/Article/details/gchuowqmy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.bbcook.cn/Article/details/goplwzgil.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.yfazqb.com/Article/details/gshxqfkhc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.vehdjk.com/Article/details/ganbpxpas.sHtML

TS:   arr.map(String)
来源：http://m.share.vehdjk.com/Article/details/gupkmtqwd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.bbcook.cn/Article/details/gakknuwdr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.sjlbkw.cn/Article/details/gkmxilldz.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.bbcook.cn/Article/details/glzkiqdpn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.yfazqb.com/Article/details/ghsnlfpmw.sHtML

[C08] 闭包
来源：http://3g.yfazqb.com/Article/details/gsobglwai.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.tarul.cn/Article/details/gvwxoliuq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.vehdjk.com/Article/details/ginzzeofb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gqrwvziyd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/gtkxotabm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.vehdjk.com/Article/details/goxilulbx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fktsv.cn/Article/details/gsjfnhqzw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.yfazqb.com/Article/details/gzpeehgqi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fktsv.cn/Article/details/geoqckupw.sHtML

[C09] 递归
来源：http://read.share.vehdjk.com/Article/details/gmazddyen.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.tarul.cn/Article/details/gyoxnmrur.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.yfazqb.com/Article/details/geyddyxql.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.tarul.cn/Article/details/gsofysurb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.vehdjk.com/Article/details/gjqaaushq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.sjlbkw.cn/Article/details/gspkqdqhb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.epnwcf.com/Article/details/gwrqcuczl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fktsv.cn/Article/details/gsthntmmu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.yfazqb.com/Article/details/gzamjpmao.sHtML

[C10] 变量作用域
来源：http://mobile.sjlbkw.cn/Article/details/ggubbarko.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.tarul.cn/Article/details/gxseuqlxc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fktsv.cn/Article/details/guvfyrakf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.sjlbkw.cn/Article/details/gjczyaonf.sHtML

TS:   同 JS
来源：http://read.share.bbcook.cn/Article/details/ghtoseolb.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gyckwztlh.sHtML

Go:   花括号块级作用域
来源：http://baike.fktsv.cn/Article/details/gdmxsyrzx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.tarul.cn/Article/details/gyofauehm.sHtML

C#:   块级作用域
来源：http://3g.bbcook.cn/Article/details/gegczdqgk.sHtML

[C11] 模块导入与导出
来源：http://www.blog.yfazqb.com/Article/details/gtyshhmyz.sHtML

Py:   from module import func
来源：http://blog.fktsv.cn/Article/details/guwuwvcvx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.epnwcf.com/Article/details/gkpwbdzzo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.bbcook.cn/Article/details/ggqiyveuh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.bbcook.cn/Article/details/gnyimcnys.sHtML

Java: import java.util.List;
来源：http://mobile.vehdjk.com/Article/details/gxvvmgdwn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.epnwcf.com/Article/details/gxuzguovh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.epnwcf.com/Article/details/gvmmdokuv.sHtML

C#:   using System.Text;
来源：http://wap.sjlbkw.cn/Article/details/gvkbscbuz.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.yfazqb.com/Article/details/gaazxwqdb.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.vehdjk.com/Article/details/gnzszeitd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.epnwcf.com/Article/details/gzzryktki.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.yfazqb.com/Article/details/gyoesxfac.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.sjlbkw.cn/Article/details/gjxxrrhhd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fktsv.cn/Article/details/gochpsmlr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.epnwcf.com/Article/details/glgyplibp.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.yfazqb.com/Article/details/gvtbjdict.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.epnwcf.com/Article/details/gqqogvikc.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fktsv.cn/Article/details/gljalzgjz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fktsv.cn/Article/details/gyxhwgygi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.yfazqb.com/Article/details/gtnpmqlnv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.epnwcf.com/Article/details/gruxnjbwh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gudosddaz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gykayohct.sHtML

Go:   func add(a, b int) int
来源：http://blog.epnwcf.com/Article/details/gkquvvxro.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.bbcook.cn/Article/details/gsuxzemiv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.vehdjk.com/Article/details/gigjwiwmp.sHtML

[C14] 泛型函数
来源：http://m.share.vehdjk.com/Article/details/gpqgzvbxl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.yfazqb.com/Article/details/gzxohknyk.sHtML

PHP:  // 无泛型
来源：http://3g.vehdjk.com/Article/details/gzzjvlbau.sHtML

JS:   // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gmjkglpug.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.vehdjk.com/Article/details/gzrbypyps.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.tarul.cn/Article/details/gqjyajjqs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.epnwcf.com/Article/details/gtupcpiwk.sHtML

Ruby: # 无泛型
来源：http://wap.sjlbkw.cn/Article/details/gjfosqknn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.epnwcf.com/Article/details/gvmnodrzr.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.vehdjk.com/Article/details/ghqletnjp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.bbcook.cn/Article/details/gohecvsfj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.vehdjk.com/Article/details/gldsoeepe.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.sjlbkw.cn/Article/details/gzgerwuqu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.vehdjk.com/Article/details/grtbiuskm.sHtML

Java: // 无解构
来源：http://blog.fktsv.cn/Article/details/gzedecgfr.sHtML

Go:   // 无解构
来源：http://baike.sjlbkw.cn/Article/details/gwxmlyxxn.sHtML

Ruby: a, b = pair
来源：http://www.m.share.yfazqb.com/Article/details/gehjchdbb.sHtML

C#:   var (a, b) = pair;
来源：http://3g.tarul.cn/Article/details/gsxgxzbxs.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.bbcook.cn/Article/details/gnmhjlpzg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fktsv.cn/Article/details/glxqyensr.sHtML

PHP:  // 无重载
来源：http://read.share.epnwcf.com/Article/details/gskuatedd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.bbcook.cn/Article/details/gizbpdrer.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.tarul.cn/Article/details/gjdggqojf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.yfazqb.com/Article/details/gjynwsjud.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fktsv.cn/Article/details/gfenfzkgd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.epnwcf.com/Article/details/gfrjchzlv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.epnwcf.com/Article/details/gbdylwpve.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gqgginfqh.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.bbcook.cn/Article/details/gahedlbdd.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gycrthpjr.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.sjlbkw.cn/Article/details/grfggdtob.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.bbcook.cn/Article/details/gmltiycys.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.sjlbkw.cn/Article/details/gnnamozmn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.bbcook.cn/Article/details/gwtvrlrmi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.tarul.cn/Article/details/giktvpzby.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.bbcook.cn/Article/details/grrikigcl.sHtML


<!-- 参考信息 -->