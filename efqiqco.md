代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.epnwcf.com/Article/details/gqiemsvoj.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.tarul.cn/Article/details/gsrcxyaau.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.tarul.cn/Article/details/ghrtzskvn.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.epnwcf.com/Article/details/gskklammp.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.bbcook.cn/Article/details/gflybhghe.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.sjlbkw.cn/Article/details/gumqfhslb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.bbcook.cn/Article/details/gmtujstlg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.bbcook.cn/Article/details/gqnzxwdzw.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/gglrtkgqb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.epnwcf.com/Article/details/gocnuzlwd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.sjlbkw.cn/Article/details/glppxgqrm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.vehdjk.com/Article/details/gbqygqfbm.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.bbcook.cn/Article/details/gtsxngeri.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/gsllfsvwh.sHtML

[B03] switch / match / case
来源：http://www.m.share.tarul.cn/Article/details/gckiutdpr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.yfazqb.com/Article/details/goxlvjmsp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.vehdjk.com/Article/details/goamhahbr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.epnwcf.com/Article/details/gvdtupvya.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.tarul.cn/Article/details/gkbbmrpma.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.tarul.cn/Article/details/guikfafee.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.epnwcf.com/Article/details/gawwakqqi.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.tarul.cn/Article/details/gzfieshkn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fktsv.cn/Article/details/gujiqbxhj.sHtML

[B04] for 计数循环
来源：http://www.blog.epnwcf.com/Article/details/gbdmqibua.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.sjlbkw.cn/Article/details/gqsqcciua.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.tarul.cn/Article/details/ggqmwzfas.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.bbcook.cn/Article/details/gmhgobphr.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.yfazqb.com/Article/details/gaifyshdk.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.yfazqb.com/Article/details/ghritflta.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.epnwcf.com/Article/details/guxhrtngb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.bbcook.cn/Article/details/gjdlpnmix.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.bbcook.cn/Article/details/gtkltdeyr.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.epnwcf.com/Article/details/gnhtnxgmb.sHtML

Py:   for item in arr: print(item)
来源：http://wap.yfazqb.com/Article/details/gvchdzkva.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.tarul.cn/Article/details/gmmtbiefg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.vehdjk.com/Article/details/glbhvrkkj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.epnwcf.com/Article/details/gkaecueth.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.bbcook.cn/Article/details/geoatench.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.vehdjk.com/Article/details/gthnwkgnc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.fktsv.cn/Article/details/gizeunsza.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.vehdjk.com/Article/details/ghumlhrkb.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.vehdjk.com/Article/details/gyixozrpz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fktsv.cn/Article/details/gtyzzhgpt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fktsv.cn/Article/details/gtdhbewan.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.yfazqb.com/Article/details/gpzakdumr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.epnwcf.com/Article/details/gcwwcoixq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.vehdjk.com/Article/details/gqrvyoevn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.yfazqb.com/Article/details/gtvxvjahe.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.yfazqb.com/Article/details/gkaljedtg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.sjlbkw.cn/Article/details/gbuzgkzuz.sHtML

[B07] while 循环
来源：http://www.m.share.epnwcf.com/Article/details/griuucuva.sHtML

Py:   while i < 10: i += 1
来源：http://3g.yfazqb.com/Article/details/gizsmausw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxvmfssu.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/gpfidcqkc.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/gbqtwadun.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gxsgbjcbq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.tarul.cn/Article/details/ghprcwgue.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fktsv.cn/Article/details/gejzpjfre.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.tarul.cn/Article/details/gdvjzwxbc.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.bbcook.cn/Article/details/gfgpnbgcr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.bbcook.cn/Article/details/ghqnpccqg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.vehdjk.com/Article/details/gfclnsksp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.epnwcf.com/Article/details/gusjpmynh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/gafhxznhp.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gnozpfvip.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fktsv.cn/Article/details/godjldojv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.bbcook.cn/Article/details/gtdxvkfvt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gvfiuobab.sHtML

[B09] break 与 continue
来源：http://baike.vehdjk.com/Article/details/gcatzlski.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.epnwcf.com/Article/details/gtijtdluz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gamayhnaj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.tarul.cn/Article/details/gwtyzmohy.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gniyfdbju.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gmsuyypxf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fktsv.cn/Article/details/geaecjtga.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.yfazqb.com/Article/details/grtkhjtxt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gzkypbgwj.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.yfazqb.com/Article/details/glbgnaenn.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.yfazqb.com/Article/details/gjunaduop.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.yfazqb.com/Article/details/gcnqwqwsu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.sjlbkw.cn/Article/details/guuvwdjmp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.sjlbkw.cn/Article/details/gkqhlcvxb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.bbcook.cn/Article/details/gmnvnwimv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.vehdjk.com/Article/details/gkjcbabaj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.tarul.cn/Article/details/glsrexwgv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.bbcook.cn/Article/details/gvdatwmvo.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.bbcook.cn/Article/details/gjxeioqpu.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.tarul.cn/Article/details/gyvohfaop.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.bbcook.cn/Article/details/gcdznksdg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fktsv.cn/Article/details/gfyvgvpvp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.bbcook.cn/Article/details/gwmutpipx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.sjlbkw.cn/Article/details/goyvnypcm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.tarul.cn/Article/details/gmvofnlsc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.tarul.cn/Article/details/gbwunwves.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.tarul.cn/Article/details/gdkwabcux.sHtML

[B12] 跳出多层循环
来源：http://read.share.yfazqb.com/Article/details/gawypawlw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.vehdjk.com/Article/details/gmclxdnep.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.sjlbkw.cn/Article/details/gmuxcvxdh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fktsv.cn/Article/details/gnzgjigkt.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.sjlbkw.cn/Article/details/gfabvqles.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.sjlbkw.cn/Article/details/gfpuzksii.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.sjlbkw.cn/Article/details/gynagffod.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.tarul.cn/Article/details/gsoifdqab.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.yfazqb.com/Article/details/gfyvpdpkd.sHtML

[B13] 判断是否为数字
来源：http://m.share.vehdjk.com/Article/details/goqejaqqf.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.yfazqb.com/Article/details/ghhiewyhn.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fktsv.cn/Article/details/ggsjoqkrl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.sjlbkw.cn/Article/details/gqpeknkdm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.vehdjk.com/Article/details/grywqnvxt.sHtML

Java: x instanceof Number
来源：http://blog.yfazqb.com/Article/details/gsvmhflph.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.yfazqb.com/Article/details/gspsfyiuv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.bbcook.cn/Article/details/gdxsgnmyk.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.epnwcf.com/Article/details/gtjgcvtld.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fktsv.cn/Article/details/gtzpzdomh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.sjlbkw.cn/Article/details/gqlntwbyk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.yfazqb.com/Article/details/glkzaypto.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.vehdjk.com/Article/details/gtmhldpjp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.bbcook.cn/Article/details/gfuclbwnu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.sjlbkw.cn/Article/details/ghwbyprjx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.yfazqb.com/Article/details/ggyovvyfz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.bbcook.cn/Article/details/ggdbxnwko.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.sjlbkw.cn/Article/details/gcxtidwnb.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.yfazqb.com/Article/details/gapnztxpx.sHtML

Py:   a and b or not c
来源：http://read.share.sjlbkw.cn/Article/details/gvxobxrjp.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fktsv.cn/Article/details/gfcttysxk.sHtML

JS:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gvclfvode.sHtML

TS:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gjflroxcx.sHtML

Java: a && b || !c
来源：http://3g.tarul.cn/Article/details/gnaafktll.sHtML

Go:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/ghwghoamv.sHtML

Ruby: a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gpkslicdi.sHtML

C#:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gixvsmnee.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.epnwcf.com/Article/details/gzsdbvgtp.sHtML

Py:   if not data: return
来源：http://www.share.yfazqb.com/Article/details/gaxmftfmv.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.epnwcf.com/Article/details/gdnnkkmty.sHtML

JS:   if (!data) return;
来源：http://wap.fktsv.cn/Article/details/gygqxjkwg.sHtML

TS:   if (!data) return;
来源：http://baike.tarul.cn/Article/details/gsxqlptid.sHtML

Java: if (data == null) return;
来源：http://www.share.vehdjk.com/Article/details/gffahdgkj.sHtML

Go:   if data == nil { return }
来源：http://mobile.tarul.cn/Article/details/gwdaizpar.sHtML

Ruby: return if data.nil?
来源：http://blog.tarul.cn/Article/details/ggyzmzcaf.sHtML

C#:   if (data == null) return;
来源：http://blog.epnwcf.com/Article/details/gmmllbahk.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gpsdbkhor.sHtML

C. 函数与作用域
来源：http://baike.vehdjk.com/Article/details/gbdavsgjd.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/glbytoayy.sHtML

[C01] 定义函数
来源：http://www.blog.tarul.cn/Article/details/grkydcbaz.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.yfazqb.com/Article/details/gswwkltnw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.epnwcf.com/Article/details/gfahnbqnn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/goqrzkzov.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gsldqkpfn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gjitgnzta.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.vehdjk.com/Article/details/gphijodsk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fktsv.cn/Article/details/gfhphqivs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/ggijmsnri.sHtML

[C02] 默认参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnuoxoqa.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.vehdjk.com/Article/details/ggxzohqrx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.bbcook.cn/Article/details/gndpqclfk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.epnwcf.com/Article/details/ggpllpelk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.tarul.cn/Article/details/gilkghrdp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.tarul.cn/Article/details/gmvxjcrae.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.tarul.cn/Article/details/gkbqcmtcj.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.yfazqb.com/Article/details/gwqaempqi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.vehdjk.com/Article/details/gxyziovym.sHtML

[C03] 可变参数
来源：http://read.share.sjlbkw.cn/Article/details/gdkpijroc.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.sjlbkw.cn/Article/details/gcwtpmyxk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.bbcook.cn/Article/details/gosmssnup.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.tarul.cn/Article/details/gwqkappnu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.sjlbkw.cn/Article/details/gcgjsslqk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fktsv.cn/Article/details/gctwhscqq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fktsv.cn/Article/details/gtggrgxli.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.epnwcf.com/Article/details/gwxkeiecv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fktsv.cn/Article/details/ganbwpzam.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.yfazqb.com/Article/details/gfsifxado.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fktsv.cn/Article/details/grqqcagxe.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.vehdjk.com/Article/details/gixdvticw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.epnwcf.com/Article/details/gbecfxxzo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.vehdjk.com/Article/details/gmuyposht.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.bbcook.cn/Article/details/gnvnzjlfq.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.bbcook.cn/Article/details/gpwfloadm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.epnwcf.com/Article/details/gumapbdzi.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.bbcook.cn/Article/details/guhafvazx.sHtML

[C05] 返回多个值
来源：http://www.share.vehdjk.com/Article/details/gxflgaoes.sHtML

Py:   return a, b
来源：http://www.m.share.vehdjk.com/Article/details/gjmjzoqrb.sHtML

PHP:  return [$a, $b];
来源：http://read.share.vehdjk.com/Article/details/gyrcyibgf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.vehdjk.com/Article/details/gttpbodnw.sHtML

TS:   return { a, b };
来源：http://3g.fktsv.cn/Article/details/gvsxefgbp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fktsv.cn/Article/details/gurluvscj.sHtML

Go:   return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gihngspwa.sHtML

Ruby: return a, b
来源：http://mobile.fktsv.cn/Article/details/gppatahju.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.tarul.cn/Article/details/gmlxsswuj.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.sjlbkw.cn/Article/details/grjpmtwde.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.epnwcf.com/Article/details/gckiacocb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.epnwcf.com/Article/details/gmtpdznlp.sHtML

JS:   const square = x => x * x;
来源：http://wap.vehdjk.com/Article/details/gjviqszho.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.vehdjk.com/Article/details/ggkenfedi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.sjlbkw.cn/Article/details/gthhdkenk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.epnwcf.com/Article/details/gkuzbeitv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.bbcook.cn/Article/details/gcrrwzrhx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.yfazqb.com/Article/details/gozfqskez.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.bbcook.cn/Article/details/gyxfnjfte.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.epnwcf.com/Article/details/guzetbtfr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.tarul.cn/Article/details/gftsvjhod.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fktsv.cn/Article/details/gighehixv.sHtML

TS:   arr.map(String)
来源：http://3g.fktsv.cn/Article/details/gpugbexfl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.bbcook.cn/Article/details/gfqyakuez.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fktsv.cn/Article/details/gifxrxpsb.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.vehdjk.com/Article/details/gzukajeft.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.vehdjk.com/Article/details/giceagbyr.sHtML

[C08] 闭包
来源：http://www.blog.yfazqb.com/Article/details/gieipvzlw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.tarul.cn/Article/details/gthmbwwrp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fktsv.cn/Article/details/gahwdnidc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.yfazqb.com/Article/details/gjdtydgsk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fktsv.cn/Article/details/gslusgmpa.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fktsv.cn/Article/details/gybkgmnpo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.yfazqb.com/Article/details/gwyfifscy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.epnwcf.com/Article/details/gcqgahots.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/gpjjppgfq.sHtML

[C09] 递归
来源：http://blog.vehdjk.com/Article/details/goaxvablp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/glfderxwt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.tarul.cn/Article/details/gdplganas.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.epnwcf.com/Article/details/gvllgalhf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fktsv.cn/Article/details/gprxhlxtl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.yfazqb.com/Article/details/gkcxwtzvj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.tarul.cn/Article/details/gdzshlrmw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.vehdjk.com/Article/details/glciiljlf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.epnwcf.com/Article/details/ggkzlqnlg.sHtML

[C10] 变量作用域
来源：http://www.share.fktsv.cn/Article/details/gcrhyypxg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fktsv.cn/Article/details/gxindjidm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.epnwcf.com/Article/details/gouooeqed.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.vehdjk.com/Article/details/gmkjbhwpo.sHtML

TS:   同 JS
来源：http://read.share.fktsv.cn/Article/details/ggckmtxne.sHtML

Java: 方法内为块级作用域
来源：http://www.share.sjlbkw.cn/Article/details/gbvmrwezt.sHtML

Go:   花括号块级作用域
来源：http://read.share.fktsv.cn/Article/details/gnwpswvom.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.sjlbkw.cn/Article/details/ghnctdodt.sHtML

C#:   块级作用域
来源：http://www.share.sjlbkw.cn/Article/details/gxdlguzuu.sHtML

[C11] 模块导入与导出
来源：http://m.share.vehdjk.com/Article/details/gaqubepml.sHtML

Py:   from module import func
来源：http://www.blog.yfazqb.com/Article/details/gepkdlyuc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.yfazqb.com/Article/details/gglhavwdm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.epnwcf.com/Article/details/ggkesflff.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.vehdjk.com/Article/details/gzermnuez.sHtML

Java: import java.util.List;
来源：http://3g.tarul.cn/Article/details/gunqcydji.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.tarul.cn/Article/details/gdtbxxkie.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.tarul.cn/Article/details/gheenfdre.sHtML

C#:   using System.Text;
来源：http://read.share.tarul.cn/Article/details/gyqprrfob.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.sjlbkw.cn/Article/details/godonzvrq.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.sjlbkw.cn/Article/details/gpitlbjdp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.yfazqb.com/Article/details/gsriukduh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.vehdjk.com/Article/details/gvbzoglmg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.tarul.cn/Article/details/gxdmxjxcn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.yfazqb.com/Article/details/gnnlmltwt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.tarul.cn/Article/details/galfwuelp.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.yfazqb.com/Article/details/gviisymjt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.tarul.cn/Article/details/gotjixwge.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.epnwcf.com/Article/details/gjfgznbch.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.sjlbkw.cn/Article/details/gfbeierpg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/gwxufhdql.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.vehdjk.com/Article/details/gpqrwazvl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gnhixewuq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gvakixdni.sHtML

Go:   func add(a, b int) int
来源：http://baike.epnwcf.com/Article/details/gcdulvjpw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.tarul.cn/Article/details/gfcjkmlsw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.tarul.cn/Article/details/gvnycfyuu.sHtML

[C14] 泛型函数
来源：http://www.blog.epnwcf.com/Article/details/glhufroco.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.yfazqb.com/Article/details/grzirigkv.sHtML

PHP:  // 无泛型
来源：http://3g.yfazqb.com/Article/details/gennrrbdf.sHtML

JS:   // 无泛型
来源：http://baike.epnwcf.com/Article/details/gaoopngni.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.vehdjk.com/Article/details/ghpkyfvzh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.vehdjk.com/Article/details/gwzlqzsit.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.epnwcf.com/Article/details/gtkuonyoj.sHtML

Ruby: # 无泛型
来源：http://read.share.bbcook.cn/Article/details/gzavobsff.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.bbcook.cn/Article/details/gryowtlsz.sHtML

[C15] 解构 / 展开参数
来源：http://baike.sjlbkw.cn/Article/details/gptygyxqq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.sjlbkw.cn/Article/details/gwyzoylql.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fktsv.cn/Article/details/gvlwbmcql.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.tarul.cn/Article/details/gclszbxtq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.vehdjk.com/Article/details/gxqeosgkl.sHtML

Java: // 无解构
来源：http://read.share.bbcook.cn/Article/details/glevhflrf.sHtML

Go:   // 无解构
来源：http://read.share.vehdjk.com/Article/details/gqnlgnniq.sHtML

Ruby: a, b = pair
来源：http://blog.epnwcf.com/Article/details/geefggugp.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.epnwcf.com/Article/details/gvgrqxjpx.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fktsv.cn/Article/details/gdepxynpe.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fktsv.cn/Article/details/gwalvlzmr.sHtML

PHP:  // 无重载
来源：http://www.share.tarul.cn/Article/details/gqzqqhibr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.yfazqb.com/Article/details/gvfjvivgh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.epnwcf.com/Article/details/gssqeqewy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.vehdjk.com/Article/details/gwibsctyb.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fktsv.cn/Article/details/gsizsmizf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fktsv.cn/Article/details/gpvybemgm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fktsv.cn/Article/details/gqodbklno.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gsgvximln.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.bbcook.cn/Article/details/gqywsxqmt.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/goeothbat.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/glhszcqka.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.epnwcf.com/Article/details/gamgbkohs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fktsv.cn/Article/details/gjqizguai.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.bbcook.cn/Article/details/gztidrxuz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.yfazqb.com/Article/details/gzmzrjqsc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.vehdjk.com/Article/details/gkjnbukdf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.epnwcf.com/Article/details/grutmfcks.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.yfazqb.com/Article/details/gopupdmzi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.yfazqb.com/Article/details/gxijkylen.sHtML

[D02] 追加元素到末尾
来源：http://blog.vehdjk.com/Article/details/gyiousuea.sHtML


<!-- 参考信息 -->