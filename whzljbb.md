代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.fktsv.cn/Article/details/gomskmsoc.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gspgmpwzj.sHtML

B. 流程控制
来源：http://www.blog.tarul.cn/Article/details/gotqqbzxt.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gggjtklez.sHtML

[B01] 条件判断 if / else
来源：http://mobile.vehdjk.com/Article/details/gowqxjjci.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.sjlbkw.cn/Article/details/giuuxlyat.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.tarul.cn/Article/details/ghmqwlrdn.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.tarul.cn/Article/details/ggbscqwnj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.yfazqb.com/Article/details/gxealmgoc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.tarul.cn/Article/details/gvhmwbgjh.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.tarul.cn/Article/details/gpldaernw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.bbcook.cn/Article/details/gkdhyzsqb.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.bbcook.cn/Article/details/gjpxhownh.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.yfazqb.com/Article/details/gwvjuyalc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.sjlbkw.cn/Article/details/gwqbubifm.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.vehdjk.com/Article/details/gqumelijg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/gouqzmatq.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.vehdjk.com/Article/details/glsfyppjx.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.bbcook.cn/Article/details/gqfwoezjd.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.bbcook.cn/Article/details/geeoiqcle.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.yfazqb.com/Article/details/ghgvxbicj.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/gqkpbixzp.sHtML

[B03] switch / match / case
来源：http://3g.bbcook.cn/Article/details/gusovraqm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fktsv.cn/Article/details/gjrwnnzjh.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fktsv.cn/Article/details/gulohxgct.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gedzrkwwf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.yfazqb.com/Article/details/glyrxdgva.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/gdcoeicfw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.epnwcf.com/Article/details/gwqiyumur.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.tarul.cn/Article/details/gjuaedatl.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.yfazqb.com/Article/details/gpcaokuiw.sHtML

[B04] for 计数循环
来源：http://www.share.vehdjk.com/Article/details/gqbtkucht.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.tarul.cn/Article/details/gclcbltyo.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.yfazqb.com/Article/details/giuweqdgt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fktsv.cn/Article/details/gmoymiiqg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.yfazqb.com/Article/details/gmdgbhhxe.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.epnwcf.com/Article/details/gvkgumyxk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.sjlbkw.cn/Article/details/gdxqztfcw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.tarul.cn/Article/details/gwglkysvq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.vehdjk.com/Article/details/goihpgakr.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fktsv.cn/Article/details/gyjiudige.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fktsv.cn/Article/details/gxelotbrd.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.epnwcf.com/Article/details/ggseivqdh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.bbcook.cn/Article/details/gqiouwirl.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.tarul.cn/Article/details/gchpooqyi.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.tarul.cn/Article/details/gtpuhoacu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.vehdjk.com/Article/details/guisunsps.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.bbcook.cn/Article/details/gfoqcjkow.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.epnwcf.com/Article/details/gtsiekmst.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fktsv.cn/Article/details/gdqmwrnyj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.vehdjk.com/Article/details/grjydwakv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.vehdjk.com/Article/details/gzxytjdzo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.yfazqb.com/Article/details/gifloimto.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.bbcook.cn/Article/details/gvpcelhus.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.epnwcf.com/Article/details/ghentgffl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.yfazqb.com/Article/details/gxejrmngc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.bbcook.cn/Article/details/gsohtfvbn.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.sjlbkw.cn/Article/details/gjssmxjty.sHtML

[B07] while 循环
来源：http://m.share.bbcook.cn/Article/details/gqhyonxkq.sHtML

Py:   while i < 10: i += 1
来源：http://baike.vehdjk.com/Article/details/gqzsdappr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.tarul.cn/Article/details/gdkxvoobu.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fktsv.cn/Article/details/gmfnijhme.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.yfazqb.com/Article/details/gevldihrj.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/graapxzpj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.bbcook.cn/Article/details/ggmdqdytk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.sjlbkw.cn/Article/details/gatiuffuu.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gfiibtzcg.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.sjlbkw.cn/Article/details/gkootpfet.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fktsv.cn/Article/details/geypiugro.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fktsv.cn/Article/details/glovwmjeh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gclhixeyl.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.tarul.cn/Article/details/gunicclyp.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.tarul.cn/Article/details/gddgenghk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.tarul.cn/Article/details/grvoahkza.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.bbcook.cn/Article/details/gdeawyduk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/gicremfnw.sHtML

[B09] break 与 continue
来源：http://3g.yfazqb.com/Article/details/gnjuwedpf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.yfazqb.com/Article/details/gbowjyucn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gpjhrkxdn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gryhzabwz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gojpvensi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gphxxiwsj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.vehdjk.com/Article/details/gognyflpg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fktsv.cn/Article/details/ghfvuknqk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gmcnwcjyo.sHtML

[B10] 遍历同时拿索引
来源：http://baike.tarul.cn/Article/details/gloqjslej.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.sjlbkw.cn/Article/details/gbwddwoqg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gppxmjymy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fktsv.cn/Article/details/gtcnhfhxa.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.vehdjk.com/Article/details/gbkdbgtva.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.sjlbkw.cn/Article/details/gxztcypyh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.sjlbkw.cn/Article/details/grohiindg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.sjlbkw.cn/Article/details/girkmgunc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.bbcook.cn/Article/details/gpriqkdoc.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.sjlbkw.cn/Article/details/ghzssnbco.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.tarul.cn/Article/details/giqhtrzfr.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.vehdjk.com/Article/details/ghcqpoace.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.epnwcf.com/Article/details/gsnbdxdnw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.bbcook.cn/Article/details/gyfhguoga.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.sjlbkw.cn/Article/details/gywmdeebm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.vehdjk.com/Article/details/gebjpwszj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.yfazqb.com/Article/details/gnqexljfm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.yfazqb.com/Article/details/gzxigiobh.sHtML

[B12] 跳出多层循环
来源：http://blog.fktsv.cn/Article/details/gefnzkeri.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.epnwcf.com/Article/details/gsuhielym.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fktsv.cn/Article/details/gywejcxxe.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.tarul.cn/Article/details/gsufkxqzz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.tarul.cn/Article/details/gssibkctz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/gsouyivwf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.yfazqb.com/Article/details/gakvskidr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fktsv.cn/Article/details/gvetprtpd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.tarul.cn/Article/details/gcovepget.sHtML

[B13] 判断是否为数字
来源：http://3g.epnwcf.com/Article/details/gbgqsqwvl.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.yfazqb.com/Article/details/gzxfpeuyu.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fktsv.cn/Article/details/gmzmdcpuy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.bbcook.cn/Article/details/ggudgyhju.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.sjlbkw.cn/Article/details/gcteenpzj.sHtML

Java: x instanceof Number
来源：http://baike.yfazqb.com/Article/details/gqiisargm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.bbcook.cn/Article/details/gooyvegfp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.epnwcf.com/Article/details/gkfcfxtlq.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.tarul.cn/Article/details/gpczzvlnd.sHtML

[B14] 判断值是否在集合内
来源：http://baike.epnwcf.com/Article/details/gpuhxgngb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.tarul.cn/Article/details/gzrtdzvdj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fktsv.cn/Article/details/gbkceiajz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.tarul.cn/Article/details/gwsjprrsc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fktsv.cn/Article/details/gibaahxim.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fktsv.cn/Article/details/gyxpjssme.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.tarul.cn/Article/details/giscsmxor.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.yfazqb.com/Article/details/glmswkhps.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gphnwtrdi.sHtML

[B15] 布尔运算与取反
来源：http://mobile.bbcook.cn/Article/details/grncetjlr.sHtML

Py:   a and b or not c
来源：http://wap.yfazqb.com/Article/details/gpwlccoki.sHtML

PHP:  $a && $b || !$c
来源：http://baike.tarul.cn/Article/details/geqvluxys.sHtML

JS:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gvvgdovej.sHtML

TS:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/goiblethg.sHtML

Java: a && b || !c
来源：http://read.share.tarul.cn/Article/details/gvvojmlua.sHtML

Go:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/giiahisqt.sHtML

Ruby: a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gaavxrqhs.sHtML

C#:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/grabsvbot.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.vehdjk.com/Article/details/gnygtmfst.sHtML

Py:   if not data: return
来源：http://www.blog.yfazqb.com/Article/details/gypdbtzgu.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.tarul.cn/Article/details/gcyqxgcrq.sHtML

JS:   if (!data) return;
来源：http://www.m.share.vehdjk.com/Article/details/gjpldqrrf.sHtML

TS:   if (!data) return;
来源：http://blog.vehdjk.com/Article/details/gdkhmilnt.sHtML

Java: if (data == null) return;
来源：http://read.share.tarul.cn/Article/details/gzekshvvf.sHtML

Go:   if data == nil { return }
来源：http://read.share.epnwcf.com/Article/details/gewqvsvak.sHtML

Ruby: return if data.nil?
来源：http://mobile.bbcook.cn/Article/details/gywshhilb.sHtML

C#:   if (data == null) return;
来源：http://3g.sjlbkw.cn/Article/details/gokfpngna.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gkmlamulb.sHtML

C. 函数与作用域
来源：http://mobile.vehdjk.com/Article/details/ghbylszhw.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gxtbawjsv.sHtML

[C01] 定义函数
来源：http://wap.fktsv.cn/Article/details/gukkoczwm.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.vehdjk.com/Article/details/gaipmhait.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/gxtaiqcql.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gpxhpfxnp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/ghfxspiuv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gjsfeytkz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.tarul.cn/Article/details/gsoprleuz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.yfazqb.com/Article/details/gyhzkcext.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/goeisgzvc.sHtML

[C02] 默认参数
来源：http://mobile.sjlbkw.cn/Article/details/gsolmrdro.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.bbcook.cn/Article/details/gdrvfmlpg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.sjlbkw.cn/Article/details/grcovzsbx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.epnwcf.com/Article/details/gkyrwrabe.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.yfazqb.com/Article/details/gxkbqsfky.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.epnwcf.com/Article/details/gzfrwmnpa.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.tarul.cn/Article/details/gdiuqywys.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.yfazqb.com/Article/details/gmbqbbvpx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.tarul.cn/Article/details/gsccnethp.sHtML

[C03] 可变参数
来源：http://read.share.tarul.cn/Article/details/gxkokuvyl.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.yfazqb.com/Article/details/gaeeborzm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.bbcook.cn/Article/details/gcuwbumxr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.vehdjk.com/Article/details/gemtsjtut.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.yfazqb.com/Article/details/gwilkmtik.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.vehdjk.com/Article/details/gvugetvms.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fktsv.cn/Article/details/gpbeespyy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.vehdjk.com/Article/details/gekwibfti.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.bbcook.cn/Article/details/gdhpusypw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.tarul.cn/Article/details/gnacaxlug.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.epnwcf.com/Article/details/gawcokfaj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.epnwcf.com/Article/details/gzinarptr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.sjlbkw.cn/Article/details/gnxodxyya.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.yfazqb.com/Article/details/gmqfwvvww.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.yfazqb.com/Article/details/gnszawzqp.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fktsv.cn/Article/details/gllwwnvmm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/gxgyyiuyz.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.sjlbkw.cn/Article/details/gfcxgbgne.sHtML

[C05] 返回多个值
来源：http://wap.vehdjk.com/Article/details/gwcnmuuhj.sHtML

Py:   return a, b
来源：http://read.share.fktsv.cn/Article/details/gbkpynaii.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fktsv.cn/Article/details/gcqrroiqj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fktsv.cn/Article/details/gsxzaaqer.sHtML

TS:   return { a, b };
来源：http://3g.epnwcf.com/Article/details/gaertzcsg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.vehdjk.com/Article/details/gjoobkozq.sHtML

Go:   return a, b
来源：http://www.blog.epnwcf.com/Article/details/grhvqctlw.sHtML

Ruby: return a, b
来源：http://www.share.bbcook.cn/Article/details/glyhzhmut.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.epnwcf.com/Article/details/ggqwrbhkd.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.bbcook.cn/Article/details/gavnuxwpt.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.yfazqb.com/Article/details/gquagfhog.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fktsv.cn/Article/details/gcqnwgibl.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fktsv.cn/Article/details/gbgjpuknq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fktsv.cn/Article/details/gpdvoumvu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.tarul.cn/Article/details/ghktnkrmb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.vehdjk.com/Article/details/gxytczthz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fktsv.cn/Article/details/gzqnlxttm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gabwxhoik.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.vehdjk.com/Article/details/gsijueeck.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.sjlbkw.cn/Article/details/gqtbeosam.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.yfazqb.com/Article/details/gceqlmgsd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.yfazqb.com/Article/details/gmixstluh.sHtML

TS:   arr.map(String)
来源：http://mobile.bbcook.cn/Article/details/gneadrgbz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.bbcook.cn/Article/details/gbkzlzqwv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.tarul.cn/Article/details/gqraykygs.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fktsv.cn/Article/details/gheulvjyo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fktsv.cn/Article/details/gurpeywwa.sHtML

[C08] 闭包
来源：http://m.share.fktsv.cn/Article/details/gnrneudrh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fktsv.cn/Article/details/gkjhdnijb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.sjlbkw.cn/Article/details/gjsfxircy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fktsv.cn/Article/details/gzqwpbqqz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/gwyvqfxgt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fktsv.cn/Article/details/gjltnlucf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fktsv.cn/Article/details/gcnzohxso.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.tarul.cn/Article/details/gvphqpear.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.sjlbkw.cn/Article/details/gwrksceof.sHtML

[C09] 递归
来源：http://blog.bbcook.cn/Article/details/gahmyorem.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fktsv.cn/Article/details/gwmrzzchs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fktsv.cn/Article/details/gabyqejlo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.bbcook.cn/Article/details/glkipzkhy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.tarul.cn/Article/details/gjcgqukkn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.bbcook.cn/Article/details/gwpckmjqu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.sjlbkw.cn/Article/details/giljztxjy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.epnwcf.com/Article/details/govatvsvb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.tarul.cn/Article/details/gpttkumuc.sHtML

[C10] 变量作用域
来源：http://baike.vehdjk.com/Article/details/genratuhm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.tarul.cn/Article/details/girrvjbuc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fktsv.cn/Article/details/grxbldoxj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fktsv.cn/Article/details/gquyxpdxb.sHtML

TS:   同 JS
来源：http://baike.bbcook.cn/Article/details/gaafwgdpw.sHtML

Java: 方法内为块级作用域
来源：http://wap.fktsv.cn/Article/details/gktxtsjwh.sHtML

Go:   花括号块级作用域
来源：http://wap.fktsv.cn/Article/details/gkgmopqfm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.yfazqb.com/Article/details/gadfjfnjg.sHtML

C#:   块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/gnbrwdpdn.sHtML

[C11] 模块导入与导出
来源：http://3g.bbcook.cn/Article/details/gewdyxgyr.sHtML

Py:   from module import func
来源：http://mobile.epnwcf.com/Article/details/gsiyzvlii.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.yfazqb.com/Article/details/gulznuxom.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.epnwcf.com/Article/details/gicfdromj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fktsv.cn/Article/details/groqnbbfk.sHtML

Java: import java.util.List;
来源：http://m.share.bbcook.cn/Article/details/gonnoygze.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.epnwcf.com/Article/details/gqfudqkmp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.bbcook.cn/Article/details/gxbxtabxg.sHtML

C#:   using System.Text;
来源：http://read.share.bbcook.cn/Article/details/gmlblgafo.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.bbcook.cn/Article/details/gjmosmfdc.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.tarul.cn/Article/details/ghfbocsoo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.yfazqb.com/Article/details/gufevclpf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.sjlbkw.cn/Article/details/gdjgllquf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.bbcook.cn/Article/details/guqqgiqsh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.yfazqb.com/Article/details/gjjqvivja.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.tarul.cn/Article/details/gjxdtomja.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.yfazqb.com/Article/details/gylgyidvl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.bbcook.cn/Article/details/gjmsidjck.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.vehdjk.com/Article/details/gjwygblfo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.vehdjk.com/Article/details/gqgjdcbfw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gkndkyivk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fktsv.cn/Article/details/ggaovzhrl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gwaoauenv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/ggicxensy.sHtML

Go:   func add(a, b int) int
来源：http://baike.epnwcf.com/Article/details/gydvquawc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.sjlbkw.cn/Article/details/geymoqavo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.tarul.cn/Article/details/gyhwmwzwg.sHtML

[C14] 泛型函数
来源：http://baike.bbcook.cn/Article/details/gykbytori.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.vehdjk.com/Article/details/gmlrwxxve.sHtML

PHP:  // 无泛型
来源：http://blog.tarul.cn/Article/details/ghtmnvdat.sHtML

JS:   // 无泛型
来源：http://wap.bbcook.cn/Article/details/gyzzxgypk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.bbcook.cn/Article/details/gdzvmwrdw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.vehdjk.com/Article/details/gwejsneoq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.epnwcf.com/Article/details/gitijvqqd.sHtML

Ruby: # 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gamhhnwlk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.epnwcf.com/Article/details/gjymmfjck.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.epnwcf.com/Article/details/gribjvdyc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.tarul.cn/Article/details/gsieuvlpp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fktsv.cn/Article/details/gpgkuwrhf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.epnwcf.com/Article/details/gunobugoh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fktsv.cn/Article/details/gtjxwilwn.sHtML

Java: // 无解构
来源：http://3g.sjlbkw.cn/Article/details/gyrnommro.sHtML

Go:   // 无解构
来源：http://m.share.sjlbkw.cn/Article/details/gvqxiqzzs.sHtML

Ruby: a, b = pair
来源：http://wap.epnwcf.com/Article/details/givzwoinp.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fktsv.cn/Article/details/gowmiybpd.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.yfazqb.com/Article/details/gsoraqjhk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.yfazqb.com/Article/details/gjknfajdw.sHtML

PHP:  // 无重载
来源：http://mobile.tarul.cn/Article/details/gkaoznjpq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.yfazqb.com/Article/details/gnxpnimbv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.sjlbkw.cn/Article/details/gpttoehca.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.bbcook.cn/Article/details/gevqrtrzc.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.vehdjk.com/Article/details/gwbaudhce.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fktsv.cn/Article/details/gbsuvwvnh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.yfazqb.com/Article/details/gqebqnvtr.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gozrssxfy.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.epnwcf.com/Article/details/gotzvtnis.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gzmlnrskp.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.bbcook.cn/Article/details/gzegdekpj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.epnwcf.com/Article/details/gifvrisqr.sHtML


<!-- 参考信息 -->