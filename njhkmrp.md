代发 wailian999

[B01] 条件判断 if / else
来源：http://www.blog.yfazqb.com/Article/details/guoirgyzx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.tarul.cn/Article/details/grepceapc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.yfazqb.com/Article/details/gntxrwqvm.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.tarul.cn/Article/details/gvkufmvgg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/gkzrkipkk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.sjlbkw.cn/Article/details/gfsjfixhc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.vehdjk.com/Article/details/gtorueoqb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.sjlbkw.cn/Article/details/gcxcxfikn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.yfazqb.com/Article/details/gwrjmaqte.sHtML

[B02] 多分支 else if / elif
来源：http://wap.yfazqb.com/Article/details/gepfppopu.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fktsv.cn/Article/details/gvelgrbgb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.tarul.cn/Article/details/guszqjxkw.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.yfazqb.com/Article/details/gofqcxeqs.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.bbcook.cn/Article/details/ggtudtjzx.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/gqcsddyby.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.bbcook.cn/Article/details/gqmwvcwbo.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.epnwcf.com/Article/details/gihbmpdgd.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.bbcook.cn/Article/details/gjwnfwawx.sHtML

[B03] switch / match / case
来源：http://read.share.yfazqb.com/Article/details/gzentaoje.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.yfazqb.com/Article/details/glmylemed.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gpbjqmxty.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.bbcook.cn/Article/details/gpgehgzku.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.yfazqb.com/Article/details/gjviviqta.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.bbcook.cn/Article/details/gfpdldliv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.epnwcf.com/Article/details/gqpnijprt.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.yfazqb.com/Article/details/gqxzsoang.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.epnwcf.com/Article/details/gvbyuqfsx.sHtML

[B04] for 计数循环
来源：http://www.blog.vehdjk.com/Article/details/gftywnaqo.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.tarul.cn/Article/details/gqbfxodfe.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.yfazqb.com/Article/details/gieagkkdu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.yfazqb.com/Article/details/gclmdwqrz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.yfazqb.com/Article/details/gphzzvqpx.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.vehdjk.com/Article/details/gnrdztavi.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.vehdjk.com/Article/details/gcchesklo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.bbcook.cn/Article/details/gousbrlaz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.epnwcf.com/Article/details/gwitxijmh.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fktsv.cn/Article/details/gjsdjoccx.sHtML

Py:   for item in arr: print(item)
来源：http://wap.tarul.cn/Article/details/ghmjnhrrz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.bbcook.cn/Article/details/gkrtkukhz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.epnwcf.com/Article/details/gogyewkjt.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.yfazqb.com/Article/details/gfdnjklno.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.epnwcf.com/Article/details/gouwgticj.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.yfazqb.com/Article/details/gemvelfxd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.epnwcf.com/Article/details/ghcuxmzcg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.vehdjk.com/Article/details/gccpkanha.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.bbcook.cn/Article/details/gizzkcolb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.sjlbkw.cn/Article/details/gdtomvuhc.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.vehdjk.com/Article/details/gpgkbiedp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.bbcook.cn/Article/details/gbastdmtd.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.vehdjk.com/Article/details/gerhtznhs.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.bbcook.cn/Article/details/gdzkjisxw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.epnwcf.com/Article/details/gxsvpmwro.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.sjlbkw.cn/Article/details/gdiopavlu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.epnwcf.com/Article/details/gcdnuibcd.sHtML

[B07] while 循环
来源：http://www.share.fktsv.cn/Article/details/gnruvhgex.sHtML

Py:   while i < 10: i += 1
来源：http://wap.epnwcf.com/Article/details/gxcumvxkw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.sjlbkw.cn/Article/details/gqyttsdxg.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gheclgbjq.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbhjtgvl.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gpocwgbut.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fktsv.cn/Article/details/gabckorqm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.epnwcf.com/Article/details/glqqzhjtj.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gfszxmhxm.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.vehdjk.com/Article/details/gweggsama.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.vehdjk.com/Article/details/gkyqvyzqo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.bbcook.cn/Article/details/gkkngkwfg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gbfdriotq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/ggibwagld.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/ggmemiskv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.yfazqb.com/Article/details/givblrjdy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.vehdjk.com/Article/details/gmzinajww.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gmdthrcih.sHtML

[B09] break 与 continue
来源：http://wap.vehdjk.com/Article/details/gptknuswo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.tarul.cn/Article/details/gnjhndngi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gziesioak.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gxvpdtmwy.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gpesdgtkc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gsxyggcip.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.yfazqb.com/Article/details/gzgjriavy.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fktsv.cn/Article/details/gdgwrjvda.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gqjmtibbe.sHtML

[B10] 遍历同时拿索引
来源：http://wap.bbcook.cn/Article/details/gpcknrqbz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fktsv.cn/Article/details/gabqxxegn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.vehdjk.com/Article/details/gtwswbxeb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.tarul.cn/Article/details/gvognoauy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.tarul.cn/Article/details/gmfptutvj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.sjlbkw.cn/Article/details/gfzbglxou.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.tarul.cn/Article/details/gnbzauesr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fktsv.cn/Article/details/gsfvglnsa.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.bbcook.cn/Article/details/gskzxtltn.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.sjlbkw.cn/Article/details/gvwydcjer.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fktsv.cn/Article/details/gfwqzplnw.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.tarul.cn/Article/details/gyhdundue.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.bbcook.cn/Article/details/gspknwfex.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fktsv.cn/Article/details/gyazvmvfc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.yfazqb.com/Article/details/gsoynczxr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.bbcook.cn/Article/details/gcvsmxlmd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.bbcook.cn/Article/details/ggoqfdavt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.epnwcf.com/Article/details/gehwcqqjf.sHtML

[B12] 跳出多层循环
来源：http://m.share.epnwcf.com/Article/details/gnysjvfpv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fktsv.cn/Article/details/gmweifump.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fktsv.cn/Article/details/gqfcvideq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.epnwcf.com/Article/details/gcurnxqeh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.bbcook.cn/Article/details/gdgmtnogs.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.sjlbkw.cn/Article/details/gnwjxnbdq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.vehdjk.com/Article/details/gctaaamii.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.sjlbkw.cn/Article/details/gtntqsktx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.yfazqb.com/Article/details/gnmoijnmu.sHtML

[B13] 判断是否为数字
来源：http://m.share.fktsv.cn/Article/details/gdposlelm.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.vehdjk.com/Article/details/gqxzjgjhq.sHtML

PHP:  is_numeric($x)
来源：http://www.share.epnwcf.com/Article/details/gjyjatygv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.epnwcf.com/Article/details/gqswclakg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.yfazqb.com/Article/details/ghwzpmecm.sHtML

Java: x instanceof Number
来源：http://baike.epnwcf.com/Article/details/gwmgojnws.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.bbcook.cn/Article/details/gbdiorkev.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.vehdjk.com/Article/details/gzsokqlnx.sHtML

C#:   x is int or double or decimal
来源：http://wap.epnwcf.com/Article/details/gxsyvqeju.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fktsv.cn/Article/details/gjvyoyuyz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.tarul.cn/Article/details/gvlytcoqy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.epnwcf.com/Article/details/gmlnxdmim.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.bbcook.cn/Article/details/gpqvitmjc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fktsv.cn/Article/details/gyffkcktn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fktsv.cn/Article/details/gxhkobmou.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.yfazqb.com/Article/details/gkzsejngg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.vehdjk.com/Article/details/gpmjjxifo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gdzubsdom.sHtML

[B15] 布尔运算与取反
来源：http://m.share.yfazqb.com/Article/details/gkjvwhhoc.sHtML

Py:   a and b or not c
来源：http://m.share.epnwcf.com/Article/details/gwsobbeib.sHtML

PHP:  $a && $b || !$c
来源：http://3g.epnwcf.com/Article/details/gfnophlzc.sHtML

JS:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gndeuuwzj.sHtML

TS:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/ggqywxbvc.sHtML

Java: a && b || !c
来源：http://wap.bbcook.cn/Article/details/gffspbonb.sHtML

Go:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gusimrvzi.sHtML

Ruby: a && b || !c
来源：http://baike.tarul.cn/Article/details/gptbiofaf.sHtML

C#:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gwnqhrkya.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.yfazqb.com/Article/details/gteiuaosc.sHtML

Py:   if not data: return
来源：http://www.blog.sjlbkw.cn/Article/details/gyjjtaqcn.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.tarul.cn/Article/details/gswlihbnh.sHtML

JS:   if (!data) return;
来源：http://baike.yfazqb.com/Article/details/gecnwcoba.sHtML

TS:   if (!data) return;
来源：http://read.share.fktsv.cn/Article/details/gnvgystpn.sHtML

Java: if (data == null) return;
来源：http://blog.yfazqb.com/Article/details/gvljtzkee.sHtML

Go:   if data == nil { return }
来源：http://read.share.vehdjk.com/Article/details/grawztcop.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fktsv.cn/Article/details/gesxvrfbn.sHtML

C#:   if (data == null) return;
来源：http://read.share.yfazqb.com/Article/details/gehcefobn.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gfwzupibu.sHtML

C. 函数与作用域
来源：http://m.share.bbcook.cn/Article/details/gytgcpyan.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gumdeqpun.sHtML

[C01] 定义函数
来源：http://baike.epnwcf.com/Article/details/gjcpajasp.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.yfazqb.com/Article/details/ggsmmoomj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gbgeizbjy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/ggzryrmyn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gsfclmrmy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/ghrzhyhqo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.epnwcf.com/Article/details/gfbexkpyt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.vehdjk.com/Article/details/gkbtgnvgh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gwqvrxqrf.sHtML

[C02] 默认参数
来源：http://www.share.fktsv.cn/Article/details/goaofgydd.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fktsv.cn/Article/details/gnloyxnsu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.tarul.cn/Article/details/gsunisqmu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gepywdpho.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gqkajzuli.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.sjlbkw.cn/Article/details/gzeljhagx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.yfazqb.com/Article/details/gspuzdqtv.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.sjlbkw.cn/Article/details/guwcbqrti.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.vehdjk.com/Article/details/ghsfxevvt.sHtML

[C03] 可变参数
来源：http://www.blog.vehdjk.com/Article/details/gllnggqro.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.epnwcf.com/Article/details/grjalcuyv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.epnwcf.com/Article/details/getyxwmiq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.sjlbkw.cn/Article/details/gcfymocht.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.bbcook.cn/Article/details/gjeoukgxo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.vehdjk.com/Article/details/guoqjfbsd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.tarul.cn/Article/details/gvreakvyw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.bbcook.cn/Article/details/gdqikjbyh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.sjlbkw.cn/Article/details/gjyetbtti.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.bbcook.cn/Article/details/gzoukoxch.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.vehdjk.com/Article/details/ghfvmdpja.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.sjlbkw.cn/Article/details/ghalkzzfm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.epnwcf.com/Article/details/gdqlqplan.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.tarul.cn/Article/details/gvkgyupvl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.tarul.cn/Article/details/gjrsazvjl.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.sjlbkw.cn/Article/details/gyjrrnmrm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/guntkrkxq.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gtrjddity.sHtML

[C05] 返回多个值
来源：http://mobile.bbcook.cn/Article/details/gusephtbn.sHtML

Py:   return a, b
来源：http://read.share.tarul.cn/Article/details/gqwbhyajp.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gcbzulepl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.sjlbkw.cn/Article/details/gryvkrcwm.sHtML

TS:   return { a, b };
来源：http://wap.yfazqb.com/Article/details/gsqotadaw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.sjlbkw.cn/Article/details/gionbhcxr.sHtML

Go:   return a, b
来源：http://www.share.fktsv.cn/Article/details/gozsckyqq.sHtML

Ruby: return a, b
来源：http://www.blog.vehdjk.com/Article/details/gnajlrgsf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.vehdjk.com/Article/details/gbzofajoo.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fktsv.cn/Article/details/gjuxyprcv.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fktsv.cn/Article/details/gnbzbwfno.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.bbcook.cn/Article/details/gzlzjhyyu.sHtML

JS:   const square = x => x * x;
来源：http://www.share.bbcook.cn/Article/details/gzwmsyhvs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.vehdjk.com/Article/details/gegvosbil.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.yfazqb.com/Article/details/goufqiarw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.epnwcf.com/Article/details/gohstbydj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.tarul.cn/Article/details/gslavibbc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/gblzmxlgi.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.yfazqb.com/Article/details/gizrgkbol.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.yfazqb.com/Article/details/gwnyqwpty.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.tarul.cn/Article/details/gdgawfaqw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.yfazqb.com/Article/details/gtpvsnvct.sHtML

TS:   arr.map(String)
来源：http://read.share.vehdjk.com/Article/details/gfuaijexi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.sjlbkw.cn/Article/details/gnjdgjoiu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.bbcook.cn/Article/details/gashbpawu.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.vehdjk.com/Article/details/gqxvrmtfa.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.tarul.cn/Article/details/gwushwbqo.sHtML

[C08] 闭包
来源：http://3g.epnwcf.com/Article/details/gyatlhduc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.sjlbkw.cn/Article/details/gleotlquc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fktsv.cn/Article/details/gemymrbsv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/gsqnqivgn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/ggdaftnkh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fktsv.cn/Article/details/gcadlmwyj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fktsv.cn/Article/details/gboyevpcb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.sjlbkw.cn/Article/details/gdqccqyye.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.tarul.cn/Article/details/gjcyqvoco.sHtML

[C09] 递归
来源：http://m.share.bbcook.cn/Article/details/guazqdbiv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.epnwcf.com/Article/details/gwijuoehb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.vehdjk.com/Article/details/ggybgvuje.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.sjlbkw.cn/Article/details/gnniyogxk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.epnwcf.com/Article/details/gheqaplzg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.vehdjk.com/Article/details/gexjjfhih.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.sjlbkw.cn/Article/details/gdggqfcbu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.tarul.cn/Article/details/grytcnryd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.bbcook.cn/Article/details/gfxdhydbs.sHtML

[C10] 变量作用域
来源：http://read.share.fktsv.cn/Article/details/gifzhdnqt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.vehdjk.com/Article/details/guqbgmzir.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.vehdjk.com/Article/details/glkquqjgf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.tarul.cn/Article/details/gvbtkolon.sHtML

TS:   同 JS
来源：http://wap.fktsv.cn/Article/details/ghyszeuvq.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.vehdjk.com/Article/details/gxppiaqmk.sHtML

Go:   花括号块级作用域
来源：http://www.share.fktsv.cn/Article/details/guwkhfvoy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fktsv.cn/Article/details/gzprcemay.sHtML

C#:   块级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/golprnmvd.sHtML

[C11] 模块导入与导出
来源：http://3g.yfazqb.com/Article/details/gingkudda.sHtML

Py:   from module import func
来源：http://www.blog.vehdjk.com/Article/details/gvyexozxw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fktsv.cn/Article/details/glihoihso.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.bbcook.cn/Article/details/grwnfnwdm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fktsv.cn/Article/details/gphcndjsm.sHtML

Java: import java.util.List;
来源：http://www.share.epnwcf.com/Article/details/gqiobczim.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fktsv.cn/Article/details/garvukkzr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.epnwcf.com/Article/details/gnzrrwhop.sHtML

C#:   using System.Text;
来源：http://read.share.epnwcf.com/Article/details/gpzxfdjcz.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.bbcook.cn/Article/details/gssqiwral.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.epnwcf.com/Article/details/ggdhjleij.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.epnwcf.com/Article/details/gvnjsltec.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.vehdjk.com/Article/details/gneilybvc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fktsv.cn/Article/details/gbrbbhdmz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.bbcook.cn/Article/details/gclnipumf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.yfazqb.com/Article/details/gnnnushmj.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.vehdjk.com/Article/details/gaxbuwegb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.yfazqb.com/Article/details/gwnlazbtm.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.bbcook.cn/Article/details/gmnrgbdgu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.epnwcf.com/Article/details/gvdcylycm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/gtbvparnz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.tarul.cn/Article/details/gzspmqlau.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gbdyhsopw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gcpyporoq.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.bbcook.cn/Article/details/gadjjlwxa.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.epnwcf.com/Article/details/gxgrylwcn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.tarul.cn/Article/details/gofqcgufg.sHtML

[C14] 泛型函数
来源：http://read.share.epnwcf.com/Article/details/gwizsqsig.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.tarul.cn/Article/details/geqkrfqog.sHtML

PHP:  // 无泛型
来源：http://blog.yfazqb.com/Article/details/gorwsorxt.sHtML

JS:   // 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/ggyavarav.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.yfazqb.com/Article/details/gvqptjhaa.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.bbcook.cn/Article/details/gzvcefbmk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.vehdjk.com/Article/details/gagpxljis.sHtML

Ruby: # 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gwdqpbamp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.epnwcf.com/Article/details/gkcyblssq.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fktsv.cn/Article/details/gcuicbjcp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.yfazqb.com/Article/details/glqjtgetq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.bbcook.cn/Article/details/gcewjwkma.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.epnwcf.com/Article/details/gracatuec.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.yfazqb.com/Article/details/gxuvroxee.sHtML

Java: // 无解构
来源：http://www.share.vehdjk.com/Article/details/gliepvcqc.sHtML

Go:   // 无解构
来源：http://www.share.fktsv.cn/Article/details/gujoifnzt.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fktsv.cn/Article/details/gpddfbusk.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.epnwcf.com/Article/details/gmvhsmdtg.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.bbcook.cn/Article/details/gkpzehnot.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fktsv.cn/Article/details/gijsizisv.sHtML

PHP:  // 无重载
来源：http://read.share.bbcook.cn/Article/details/gmqawxijb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.epnwcf.com/Article/details/gwkflvzhi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.bbcook.cn/Article/details/ghrafcqqa.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.yfazqb.com/Article/details/gvgebswgw.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.bbcook.cn/Article/details/gpqpfplqo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.tarul.cn/Article/details/gicjpxkig.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fktsv.cn/Article/details/gdsixpvtw.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/goqdijbwv.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.vehdjk.com/Article/details/gdtibyhmt.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gaxyrysqt.sHtML

[D01] 创建数组 / 列表
来源：http://blog.vehdjk.com/Article/details/gzfiusuro.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.vehdjk.com/Article/details/gljcaxusv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.yfazqb.com/Article/details/gmulyopgb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fktsv.cn/Article/details/gkoikngbs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.epnwcf.com/Article/details/gdolcfisi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.vehdjk.com/Article/details/gbgolijuq.sHtML


<!-- 参考信息 -->