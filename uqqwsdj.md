代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.tarul.cn/Article/details/gbuwfkhjv.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gerwvafvf.sHtML

B. 流程控制
来源：http://m.share.bbcook.cn/Article/details/ghukombjs.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gqmtytohc.sHtML

[B01] 条件判断 if / else
来源：http://m.share.vehdjk.com/Article/details/gjhgraytl.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.tarul.cn/Article/details/gjivachcr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.yfazqb.com/Article/details/gmofpozfr.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/gxpxtzasn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gbbrzlacc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.vehdjk.com/Article/details/geyxbmzqf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.tarul.cn/Article/details/gnfzfpeje.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.tarul.cn/Article/details/gbbnhijjo.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/gzlloiwvm.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.sjlbkw.cn/Article/details/gewtzbchk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.epnwcf.com/Article/details/gtcfqtwyc.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.tarul.cn/Article/details/givzvijwz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/ggwpmldzy.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/giwpjmmei.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/gpgtrroku.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.fktsv.cn/Article/details/gatzcrulg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.sjlbkw.cn/Article/details/gkwlzdzkl.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.tarul.cn/Article/details/gqmiodjpj.sHtML

[B03] switch / match / case
来源：http://wap.fktsv.cn/Article/details/gtvevzfpb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.epnwcf.com/Article/details/gkeflbabb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/gyzzamjki.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fktsv.cn/Article/details/gjlzpkety.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/gebzdqqit.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/gqcadelsm.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.yfazqb.com/Article/details/gyifxchlc.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.yfazqb.com/Article/details/gcloprkvb.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.tarul.cn/Article/details/gnfvjrcth.sHtML

[B04] for 计数循环
来源：http://read.share.fktsv.cn/Article/details/gfzgatuhp.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.epnwcf.com/Article/details/gxzriuuxl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwnrxkjs.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.vehdjk.com/Article/details/gedbbpfwe.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.sjlbkw.cn/Article/details/gcsuplwci.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxovxnbsh.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.fktsv.cn/Article/details/ghlklyrmx.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.epnwcf.com/Article/details/gzoifcgjm.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.sjlbkw.cn/Article/details/grezfhhtq.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.fktsv.cn/Article/details/gmhuhadcm.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.bbcook.cn/Article/details/gnfyfunwf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.bbcook.cn/Article/details/gebpbvnfv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.tarul.cn/Article/details/grwunurdr.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.sjlbkw.cn/Article/details/gjacdcfsy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.epnwcf.com/Article/details/gggczpovy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.yfazqb.com/Article/details/gkdaphale.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fktsv.cn/Article/details/guxmfpwli.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.vehdjk.com/Article/details/gsqdiihzw.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.tarul.cn/Article/details/gdiuddfgc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.sjlbkw.cn/Article/details/gcicgrmrq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.yfazqb.com/Article/details/gdaxbypzj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.tarul.cn/Article/details/gxvzqvxit.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.yfazqb.com/Article/details/gwutrhcfm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.bbcook.cn/Article/details/gqafpgpnh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fktsv.cn/Article/details/gwxlovsgm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.sjlbkw.cn/Article/details/gioqrpsjn.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.vehdjk.com/Article/details/gwrsypmlv.sHtML

[B07] while 循环
来源：http://www.m.share.bbcook.cn/Article/details/gmllkcbjq.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.sjlbkw.cn/Article/details/grtxwrcfj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fktsv.cn/Article/details/gnpxmldzg.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gzfkkjywh.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gidhqahdg.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/gbgbnebqj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.yfazqb.com/Article/details/glhoeajzt.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.tarul.cn/Article/details/gagdmppdc.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/gjrvkgwjb.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.vehdjk.com/Article/details/guksgancw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.tarul.cn/Article/details/gjdwocpxb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.yfazqb.com/Article/details/gsuqllfep.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gysdgbvdg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.tarul.cn/Article/details/gzfqbnpvt.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/gzfojdwto.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.epnwcf.com/Article/details/gbkosmigs.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.bbcook.cn/Article/details/gnplrqvec.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.yfazqb.com/Article/details/gltsqqqkr.sHtML

[B09] break 与 continue
来源：http://read.share.yfazqb.com/Article/details/gvurkmuej.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fktsv.cn/Article/details/gnvytatlj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/guhnalhgj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/ggdxbpckj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gagrdxczn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/ggthttzym.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fktsv.cn/Article/details/gdhfkeeis.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.tarul.cn/Article/details/ggmpkgmde.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gfeayxchj.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.yfazqb.com/Article/details/gbajdkaix.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.epnwcf.com/Article/details/ggpkcnuce.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fktsv.cn/Article/details/grrkovizq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.sjlbkw.cn/Article/details/gfqxbaspw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fktsv.cn/Article/details/ghqmmaqvd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.bbcook.cn/Article/details/gpcfzehgj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.vehdjk.com/Article/details/gkimrwvrv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.sjlbkw.cn/Article/details/gqykesfdp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fktsv.cn/Article/details/ggkqqarva.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.epnwcf.com/Article/details/gjfjichjo.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fktsv.cn/Article/details/gemfzmpsr.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fktsv.cn/Article/details/govmhksmw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.epnwcf.com/Article/details/gpflfjqwq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.yfazqb.com/Article/details/gdymgizru.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.bbcook.cn/Article/details/gbogcicok.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.tarul.cn/Article/details/ghdsccbqq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.yfazqb.com/Article/details/gjdokslyd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fktsv.cn/Article/details/gjohkgego.sHtML

[B12] 跳出多层循环
来源：http://blog.epnwcf.com/Article/details/gkpyhbsdh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.yfazqb.com/Article/details/glvdzzywh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fktsv.cn/Article/details/gizsnosgs.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.vehdjk.com/Article/details/gcdphxovm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/ghoirmicj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/gposwdwin.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.tarul.cn/Article/details/gwfurccqn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.bbcook.cn/Article/details/gtnhtriuz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.bbcook.cn/Article/details/gijjvuyfh.sHtML

[B13] 判断是否为数字
来源：http://blog.sjlbkw.cn/Article/details/goasrgpzc.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.epnwcf.com/Article/details/guissubho.sHtML

PHP:  is_numeric($x)
来源：http://read.share.tarul.cn/Article/details/gcqhcjfyk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.epnwcf.com/Article/details/gkctszihn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.sjlbkw.cn/Article/details/gcgmdfhkp.sHtML

Java: x instanceof Number
来源：http://wap.fktsv.cn/Article/details/gzlvdimsb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.yfazqb.com/Article/details/gpdjpinjc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.bbcook.cn/Article/details/gvgerbixe.sHtML

C#:   x is int or double or decimal
来源：http://blog.tarul.cn/Article/details/gfdmehhtw.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.vehdjk.com/Article/details/gwxvuunxl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.bbcook.cn/Article/details/gbpmoyllu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fktsv.cn/Article/details/gqyxvyixy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gfjztdcel.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gaclzayji.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fktsv.cn/Article/details/glrcdbwnz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.tarul.cn/Article/details/gpyqmuwif.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.tarul.cn/Article/details/gpodxpusx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.sjlbkw.cn/Article/details/gpptwllnz.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.tarul.cn/Article/details/gswcirysi.sHtML

Py:   a and b or not c
来源：http://mobile.bbcook.cn/Article/details/gzegcgkbb.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.bbcook.cn/Article/details/giazbrzpg.sHtML

JS:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gmotrnjaa.sHtML

TS:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/gjdoyoqpe.sHtML

Java: a && b || !c
来源：http://blog.epnwcf.com/Article/details/gkzejetzg.sHtML

Go:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gvdrfrdff.sHtML

Ruby: a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/guhucivxd.sHtML

C#:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gaqbjqgbk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.sjlbkw.cn/Article/details/gnicavqeu.sHtML

Py:   if not data: return
来源：http://www.share.tarul.cn/Article/details/gclfrgtfz.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.epnwcf.com/Article/details/gmiadruhz.sHtML

JS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/gjnxluedz.sHtML

TS:   if (!data) return;
来源：http://www.blog.fktsv.cn/Article/details/gtginhljn.sHtML

Java: if (data == null) return;
来源：http://www.m.share.epnwcf.com/Article/details/goiwrgvqf.sHtML

Go:   if data == nil { return }
来源：http://3g.bbcook.cn/Article/details/gzjkdpgws.sHtML

Ruby: return if data.nil?
来源：http://www.share.vehdjk.com/Article/details/gvpjjksyx.sHtML

C#:   if (data == null) return;
来源：http://3g.sjlbkw.cn/Article/details/gxcicyslq.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gutszmtwu.sHtML

C. 函数与作用域
来源：http://www.share.tarul.cn/Article/details/gfnfwttzh.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/glanqzcjv.sHtML

[C01] 定义函数
来源：http://mobile.vehdjk.com/Article/details/gopujywsc.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.vehdjk.com/Article/details/gyjhwuauy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/gwsphybyu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gktypzuas.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gdlyiucqt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gkmkwreup.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.yfazqb.com/Article/details/gwauhcoud.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.sjlbkw.cn/Article/details/gpxpihwrx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gnqmreulu.sHtML

[C02] 默认参数
来源：http://www.m.share.vehdjk.com/Article/details/gecdolduu.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.epnwcf.com/Article/details/gtrisicsa.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.tarul.cn/Article/details/ggyhhgsza.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gbnoyyixj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gjodxmwts.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.epnwcf.com/Article/details/gjqisvckj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.vehdjk.com/Article/details/gnspxvrry.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.sjlbkw.cn/Article/details/gvaykmtrx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fktsv.cn/Article/details/gqmvgjyei.sHtML

[C03] 可变参数
来源：http://blog.vehdjk.com/Article/details/gecjrixsg.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.epnwcf.com/Article/details/gqwhzolrp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fktsv.cn/Article/details/gcmnyhopi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.bbcook.cn/Article/details/glrtqdvkb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.sjlbkw.cn/Article/details/gedabzgnq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.bbcook.cn/Article/details/gmhgufmpw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.vehdjk.com/Article/details/ggrowzwpz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.yfazqb.com/Article/details/gcdzcsqob.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.tarul.cn/Article/details/gvvbnqgqi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.sjlbkw.cn/Article/details/gkhaluoev.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.yfazqb.com/Article/details/gabpshzer.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.tarul.cn/Article/details/gkeoenhao.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fktsv.cn/Article/details/gannkyfjd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.yfazqb.com/Article/details/goomqfeng.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fktsv.cn/Article/details/gkrjuvftl.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fktsv.cn/Article/details/gphjbylxp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/gtlvsfvwk.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.yfazqb.com/Article/details/giddtkvel.sHtML

[C05] 返回多个值
来源：http://www.share.bbcook.cn/Article/details/gkxybdofl.sHtML

Py:   return a, b
来源：http://blog.fktsv.cn/Article/details/gsgartmyo.sHtML

PHP:  return [$a, $b];
来源：http://read.share.yfazqb.com/Article/details/gwsdokjmf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.yfazqb.com/Article/details/gjbzeplec.sHtML

TS:   return { a, b };
来源：http://3g.epnwcf.com/Article/details/gysplxuag.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.tarul.cn/Article/details/ggtkswpwx.sHtML

Go:   return a, b
来源：http://3g.yfazqb.com/Article/details/gioctrkiw.sHtML

Ruby: return a, b
来源：http://read.share.fktsv.cn/Article/details/gpwizljad.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.vehdjk.com/Article/details/gctmuhlyp.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.yfazqb.com/Article/details/gbmjwljhk.sHtML

Py:   square = lambda x: x * x
来源：http://3g.bbcook.cn/Article/details/gppgtxiie.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fktsv.cn/Article/details/gagefxilr.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.bbcook.cn/Article/details/gplotsrqc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.yfazqb.com/Article/details/gtmwrgrvo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fktsv.cn/Article/details/gdzknevfa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.tarul.cn/Article/details/gwisjbzyn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.epnwcf.com/Article/details/gzyjxxgnf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.epnwcf.com/Article/details/gcwwhlfum.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fktsv.cn/Article/details/gnmapjtei.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fktsv.cn/Article/details/gzdodunso.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.yfazqb.com/Article/details/gvhetkqzp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.bbcook.cn/Article/details/ghlzkpzix.sHtML

TS:   arr.map(String)
来源：http://baike.yfazqb.com/Article/details/gtwdhoozb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.epnwcf.com/Article/details/gmtkpdukm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.epnwcf.com/Article/details/gpopyidjw.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxsnqlxs.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.yfazqb.com/Article/details/gfftvhunl.sHtML

[C08] 闭包
来源：http://wap.fktsv.cn/Article/details/gkxglnazm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.epnwcf.com/Article/details/gygebsjwu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.bbcook.cn/Article/details/gebrihbah.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gpscjvdbo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.yfazqb.com/Article/details/ggdroxwzf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.yfazqb.com/Article/details/gmerzvpyp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.yfazqb.com/Article/details/gzcoqkgps.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.epnwcf.com/Article/details/gbhgtdqet.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/ggoanjoyh.sHtML

[C09] 递归
来源：http://3g.sjlbkw.cn/Article/details/gusjcszsz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.vehdjk.com/Article/details/glrbakjas.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.sjlbkw.cn/Article/details/gpzjexopt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.bbcook.cn/Article/details/gemvuqohw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.vehdjk.com/Article/details/gqnjrilfy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fktsv.cn/Article/details/gjayspsap.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.yfazqb.com/Article/details/goprpsdax.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.bbcook.cn/Article/details/grwhconif.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.epnwcf.com/Article/details/gjtilodnr.sHtML

[C10] 变量作用域
来源：http://3g.epnwcf.com/Article/details/guyelluwl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.bbcook.cn/Article/details/gwvsokije.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.vehdjk.com/Article/details/gpjbgabts.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.bbcook.cn/Article/details/gnilvmiki.sHtML

TS:   同 JS
来源：http://read.share.vehdjk.com/Article/details/gwsbdqxvo.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.yfazqb.com/Article/details/gfrddhuuj.sHtML

Go:   花括号块级作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gsrdovvde.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.epnwcf.com/Article/details/guolrwokj.sHtML

C#:   块级作用域
来源：http://read.share.epnwcf.com/Article/details/gwwmahjbr.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fktsv.cn/Article/details/gujjlsdok.sHtML

Py:   from module import func
来源：http://read.share.sjlbkw.cn/Article/details/gahlfbagv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.vehdjk.com/Article/details/ghcdgttso.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.vehdjk.com/Article/details/grhrzogxs.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.sjlbkw.cn/Article/details/gphehxrag.sHtML

Java: import java.util.List;
来源：http://m.share.tarul.cn/Article/details/ghidversj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.vehdjk.com/Article/details/gcxwtksfr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.vehdjk.com/Article/details/ghmzngvea.sHtML

C#:   using System.Text;
来源：http://wap.epnwcf.com/Article/details/gojourgsq.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.bbcook.cn/Article/details/gqwopjyrq.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.epnwcf.com/Article/details/gtiydaujq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fktsv.cn/Article/details/gppipuxgq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/gtoshtmxg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.yfazqb.com/Article/details/gntcmrilv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.tarul.cn/Article/details/gardvpzxt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.bbcook.cn/Article/details/gstiyaxng.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.vehdjk.com/Article/details/gnkxoqsok.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.epnwcf.com/Article/details/grjkcubdj.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.epnwcf.com/Article/details/gfxsagtrn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.sjlbkw.cn/Article/details/gkduxcuyk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gkcifmnxp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.bbcook.cn/Article/details/gcvwlwplo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gcbdqcoyu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gccyigkqv.sHtML

Go:   func add(a, b int) int
来源：http://3g.tarul.cn/Article/details/gfnyerypy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.bbcook.cn/Article/details/gsdqzhawp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.sjlbkw.cn/Article/details/ggjbqfoug.sHtML

[C14] 泛型函数
来源：http://www.m.share.vehdjk.com/Article/details/gvsclxngx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.epnwcf.com/Article/details/gpjziephc.sHtML

PHP:  // 无泛型
来源：http://wap.epnwcf.com/Article/details/gfhbfxqfe.sHtML

JS:   // 无泛型
来源：http://mobile.fktsv.cn/Article/details/gcwfyclsh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.yfazqb.com/Article/details/gdmradpdk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.sjlbkw.cn/Article/details/gaaoefnlt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.sjlbkw.cn/Article/details/gzpfmkint.sHtML

Ruby: # 无泛型
来源：http://m.share.tarul.cn/Article/details/gkbfadikv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.epnwcf.com/Article/details/gczwgvulv.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.sjlbkw.cn/Article/details/guucphedt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fktsv.cn/Article/details/gveyyzite.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.sjlbkw.cn/Article/details/gnuqfumib.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.tarul.cn/Article/details/gilkvfhjs.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.tarul.cn/Article/details/gtshsayna.sHtML

Java: // 无解构
来源：http://www.share.tarul.cn/Article/details/gzjtijori.sHtML

Go:   // 无解构
来源：http://m.share.vehdjk.com/Article/details/gorxhkhlj.sHtML

Ruby: a, b = pair
来源：http://wap.epnwcf.com/Article/details/ggvlwgcxi.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.epnwcf.com/Article/details/gulrkokar.sHtML

[C16] 函数 / 方法重载
来源：http://3g.bbcook.cn/Article/details/gtkamyhvk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.vehdjk.com/Article/details/gzyxrnbix.sHtML

PHP:  // 无重载
来源：http://3g.sjlbkw.cn/Article/details/gcbooooqd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.tarul.cn/Article/details/giqwolhhq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.sjlbkw.cn/Article/details/grejfbsaj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.tarul.cn/Article/details/grnhvnvxn.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.epnwcf.com/Article/details/gdsdcnscz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fktsv.cn/Article/details/gdfjejolx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.yfazqb.com/Article/details/gyipzhjhm.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gamdysquw.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.yfazqb.com/Article/details/gvdbbsqyi.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/glclubqus.sHtML

[D01] 创建数组 / 列表
来源：http://3g.yfazqb.com/Article/details/goiedyrih.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.bbcook.cn/Article/details/gtounfnhl.sHtML


<!-- 参考信息 -->