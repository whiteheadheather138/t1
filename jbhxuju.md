代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/gerbmnhsz.sHtML

[B02] 多分支 else if / elif
来源：http://wap.yfazqb.com/Article/details/gmgsngtfr.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.epnwcf.com/Article/details/gjrlmcowo.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.vehdjk.com/Article/details/gagqcugni.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/gcgfcttor.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/gegaepiuz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/gqgpegrsr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.sjlbkw.cn/Article/details/gipnkybwj.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.bbcook.cn/Article/details/gvybuxijb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.tarul.cn/Article/details/gjrboxeqi.sHtML

[B03] switch / match / case
来源：http://3g.fktsv.cn/Article/details/gnpbtwdpw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.epnwcf.com/Article/details/gynlxrbsq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.tarul.cn/Article/details/gtvrkbasp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.tarul.cn/Article/details/gwisogtsp.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/gmydqifwu.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.tarul.cn/Article/details/gneegqggh.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.vehdjk.com/Article/details/gjwayqlhp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.vehdjk.com/Article/details/ghxmwzthn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.tarul.cn/Article/details/gpnjoszgw.sHtML

[B04] for 计数循环
来源：http://www.m.share.bbcook.cn/Article/details/gbpscxtlb.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.bbcook.cn/Article/details/gglraeakf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.vehdjk.com/Article/details/gdtdmvquq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.tarul.cn/Article/details/gohayvmly.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.yfazqb.com/Article/details/gwmuappvo.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.fktsv.cn/Article/details/grxakcgrt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.bbcook.cn/Article/details/ggqsvwzaj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.epnwcf.com/Article/details/gnkeudobe.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.bbcook.cn/Article/details/gngdcigxp.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fktsv.cn/Article/details/ghngrnhuo.sHtML

Py:   for item in arr: print(item)
来源：http://blog.vehdjk.com/Article/details/gkvzqjdgf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.yfazqb.com/Article/details/gkplekprv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.yfazqb.com/Article/details/guvfyvdhn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.epnwcf.com/Article/details/gtvqfxjub.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.tarul.cn/Article/details/gnckkjlws.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.vehdjk.com/Article/details/goaxxwbib.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.sjlbkw.cn/Article/details/gzpubqlkm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.sjlbkw.cn/Article/details/gdpzuihkq.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.sjlbkw.cn/Article/details/gzseracga.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.tarul.cn/Article/details/grmocfonq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fktsv.cn/Article/details/gypypwusn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.tarul.cn/Article/details/gilarsekj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.epnwcf.com/Article/details/gxyzlbmzd.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.yfazqb.com/Article/details/gzuyjxrlw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.vehdjk.com/Article/details/gtqszltyy.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.yfazqb.com/Article/details/glxjmqvoq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.sjlbkw.cn/Article/details/gobdmmzsa.sHtML

[B07] while 循环
来源：http://wap.bbcook.cn/Article/details/garquepxh.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.yfazqb.com/Article/details/gqoojatpk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.sjlbkw.cn/Article/details/gzucwqhel.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/gflnfrtqw.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/gkltkjiff.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcyyclimj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.vehdjk.com/Article/details/ggsblzpch.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.epnwcf.com/Article/details/gyzyfrmdd.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.vehdjk.com/Article/details/gewtesnec.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.bbcook.cn/Article/details/gmavymjgt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.bbcook.cn/Article/details/grjxsqjkg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.epnwcf.com/Article/details/ghostdrvg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.epnwcf.com/Article/details/gwjbuqpqo.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/gpriabjbt.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.yfazqb.com/Article/details/gujffcttn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.epnwcf.com/Article/details/gqkitucei.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.bbcook.cn/Article/details/grrrhlgvd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gnpjejkol.sHtML

[B09] break 与 continue
来源：http://read.share.sjlbkw.cn/Article/details/gilwjkdza.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.vehdjk.com/Article/details/gindwlvlp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/gfkcgqapd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gcrgnldeu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gbqpvkamz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/giwdqbumz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.yfazqb.com/Article/details/gybaexsdh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.tarul.cn/Article/details/gbmyzeinc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/girpbfokt.sHtML

[B10] 遍历同时拿索引
来源：http://blog.epnwcf.com/Article/details/gwcykksls.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.sjlbkw.cn/Article/details/gikwxxaob.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.yfazqb.com/Article/details/gzivbwwtg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.bbcook.cn/Article/details/gejggoddf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.epnwcf.com/Article/details/gfclpfcxg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.vehdjk.com/Article/details/gzvtcjbcu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.epnwcf.com/Article/details/glodiussy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.bbcook.cn/Article/details/gfnisjide.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.bbcook.cn/Article/details/gimyvuirb.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.sjlbkw.cn/Article/details/gefzcwgvn.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.bbcook.cn/Article/details/gropcgmnj.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.tarul.cn/Article/details/gemhmroix.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.sjlbkw.cn/Article/details/gdlirwaeg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.epnwcf.com/Article/details/gpmxohdfd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.sjlbkw.cn/Article/details/gfhuasnwp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.vehdjk.com/Article/details/ggmyvygnf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.sjlbkw.cn/Article/details/gsrtroksk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.epnwcf.com/Article/details/gtzyjclhh.sHtML

[B12] 跳出多层循环
来源：http://wap.fktsv.cn/Article/details/gwmredsyq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.vehdjk.com/Article/details/gwywbhkox.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fktsv.cn/Article/details/gykanvsrm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.vehdjk.com/Article/details/ggugojbzo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fktsv.cn/Article/details/gozflxrpu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtzdtvje.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.bbcook.cn/Article/details/gzczcylfa.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.tarul.cn/Article/details/gwzteczvj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.bbcook.cn/Article/details/gzqswgaju.sHtML

[B13] 判断是否为数字
来源：http://3g.fktsv.cn/Article/details/glrwesubz.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.vehdjk.com/Article/details/gjcaswfdb.sHtML

PHP:  is_numeric($x)
来源：http://m.share.epnwcf.com/Article/details/gmrpveocu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.vehdjk.com/Article/details/ghvswauui.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.vehdjk.com/Article/details/gyxlfxduk.sHtML

Java: x instanceof Number
来源：http://www.blog.yfazqb.com/Article/details/gievyeqze.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.yfazqb.com/Article/details/gjjjneqjq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.sjlbkw.cn/Article/details/gxxzsplff.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fktsv.cn/Article/details/gkajoccvk.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.yfazqb.com/Article/details/gjdjyxiht.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.epnwcf.com/Article/details/grcsbruiz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.yfazqb.com/Article/details/gwwaxpsbz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.tarul.cn/Article/details/gfejdbnvq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.epnwcf.com/Article/details/ggvmbprxg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.epnwcf.com/Article/details/gxfulvynq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.bbcook.cn/Article/details/gggdpfwlv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.epnwcf.com/Article/details/ghjqltjwn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.bbcook.cn/Article/details/gaaikfriv.sHtML

[B15] 布尔运算与取反
来源：http://3g.epnwcf.com/Article/details/getbfrdfg.sHtML

Py:   a and b or not c
来源：http://mobile.epnwcf.com/Article/details/gmihjjrrr.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.tarul.cn/Article/details/gnhhzscds.sHtML

JS:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gtlytqupz.sHtML

TS:   a && b || !c
来源：http://www.share.epnwcf.com/Article/details/guegrqhom.sHtML

Java: a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gtiyxgsjn.sHtML

Go:   a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gzfitghvx.sHtML

Ruby: a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gnzptpazq.sHtML

C#:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gkvvpcdqf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fktsv.cn/Article/details/gmkqskqmh.sHtML

Py:   if not data: return
来源：http://mobile.epnwcf.com/Article/details/gbfyfsffk.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.yfazqb.com/Article/details/gwkkeeqrj.sHtML

JS:   if (!data) return;
来源：http://www.share.fktsv.cn/Article/details/gefobnjbi.sHtML

TS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/gyaqmaboe.sHtML

Java: if (data == null) return;
来源：http://mobile.sjlbkw.cn/Article/details/gktifukvy.sHtML

Go:   if data == nil { return }
来源：http://wap.vehdjk.com/Article/details/gnvsihiei.sHtML

Ruby: return if data.nil?
来源：http://mobile.tarul.cn/Article/details/gkmjpwduo.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrcdnnsc.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gjiblkpjb.sHtML

C. 函数与作用域
来源：http://www.share.tarul.cn/Article/details/grjtbcbng.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gewlpjham.sHtML

[C01] 定义函数
来源：http://m.share.yfazqb.com/Article/details/gnkljgcwd.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.tarul.cn/Article/details/gxzcqtbmk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gljdcbljn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/goohbtpdi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gswhtboyw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gqpcrthge.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.tarul.cn/Article/details/gewsdgwzj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.tarul.cn/Article/details/gfiaceoqx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gjbngxmpx.sHtML

[C02] 默认参数
来源：http://3g.bbcook.cn/Article/details/gxiepgudq.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.epnwcf.com/Article/details/gognyrqtg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.yfazqb.com/Article/details/gxplitpke.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gnjhxwsuz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.epnwcf.com/Article/details/gvvllrvqb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.sjlbkw.cn/Article/details/garboxdvd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.vehdjk.com/Article/details/ggylmewla.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.sjlbkw.cn/Article/details/gzepatdkh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.vehdjk.com/Article/details/gorumjffs.sHtML

[C03] 可变参数
来源：http://mobile.fktsv.cn/Article/details/gljvhvdfq.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.sjlbkw.cn/Article/details/gdhrxezlx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.tarul.cn/Article/details/gtafirrou.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.epnwcf.com/Article/details/gnqsxtykc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.bbcook.cn/Article/details/gglymrtiy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.epnwcf.com/Article/details/gunjvvpaj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.epnwcf.com/Article/details/gyfkznegh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.yfazqb.com/Article/details/groeojvls.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.yfazqb.com/Article/details/gangkihml.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.epnwcf.com/Article/details/gsrnxffvt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.bbcook.cn/Article/details/girujvqoz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.tarul.cn/Article/details/gyiwhdnly.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fktsv.cn/Article/details/geihmyoiq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.sjlbkw.cn/Article/details/gaqplggcp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fktsv.cn/Article/details/gexdvxksd.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.vehdjk.com/Article/details/gqymqrfrl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.tarul.cn/Article/details/gpwlzgtur.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/giltujitb.sHtML

[C05] 返回多个值
来源：http://baike.sjlbkw.cn/Article/details/gwiujrlhw.sHtML

Py:   return a, b
来源：http://m.share.yfazqb.com/Article/details/gedmcpxnh.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.epnwcf.com/Article/details/gfgujzadr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.bbcook.cn/Article/details/gkijxagns.sHtML

TS:   return { a, b };
来源：http://blog.vehdjk.com/Article/details/gnyctsxqu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.epnwcf.com/Article/details/gfgcdtigu.sHtML

Go:   return a, b
来源：http://www.m.share.bbcook.cn/Article/details/gbxkoowsp.sHtML

Ruby: return a, b
来源：http://3g.yfazqb.com/Article/details/groqlkzwq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.epnwcf.com/Article/details/gardutmkx.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.tarul.cn/Article/details/gwjfxduhf.sHtML

Py:   square = lambda x: x * x
来源：http://baike.tarul.cn/Article/details/gljjblvsi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.sjlbkw.cn/Article/details/ggmhvpjio.sHtML

JS:   const square = x => x * x;
来源：http://wap.vehdjk.com/Article/details/giokkylhm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.bbcook.cn/Article/details/gknzlewab.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.tarul.cn/Article/details/gyidwubbr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.yfazqb.com/Article/details/gdristhso.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.sjlbkw.cn/Article/details/gcznjwaem.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.epnwcf.com/Article/details/gqkuxoolg.sHtML

[C07] 把函数作为参数传入
来源：http://3g.tarul.cn/Article/details/gifavsazt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.yfazqb.com/Article/details/gpotnymzv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fktsv.cn/Article/details/gvirwhhho.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.epnwcf.com/Article/details/gxvgmbcbv.sHtML

TS:   arr.map(String)
来源：http://baike.vehdjk.com/Article/details/ganpfrosl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.yfazqb.com/Article/details/gqbbpvjex.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fktsv.cn/Article/details/gkkntkhol.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.epnwcf.com/Article/details/gulvosrug.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.epnwcf.com/Article/details/gpknzplue.sHtML

[C08] 闭包
来源：http://read.share.epnwcf.com/Article/details/givnhevwl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.epnwcf.com/Article/details/gpjmdorjg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.sjlbkw.cn/Article/details/gafagvpnu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/giybjwykk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/gfcjpnrij.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.sjlbkw.cn/Article/details/grjpewczh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.sjlbkw.cn/Article/details/gemzchswg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.tarul.cn/Article/details/gohrciwro.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.epnwcf.com/Article/details/glolvzyjx.sHtML

[C09] 递归
来源：http://wap.fktsv.cn/Article/details/gtiaelfaf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.bbcook.cn/Article/details/gqsrskzot.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.yfazqb.com/Article/details/geilcoqcw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.bbcook.cn/Article/details/gizpfrwpq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.bbcook.cn/Article/details/gcxyegrxm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.tarul.cn/Article/details/gkzuxjjxh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fktsv.cn/Article/details/gayyafdab.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fktsv.cn/Article/details/gesuqycjy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.yfazqb.com/Article/details/gtlvwdqtk.sHtML

[C10] 变量作用域
来源：http://read.share.bbcook.cn/Article/details/gozwtzqjw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.yfazqb.com/Article/details/gtfkpkoke.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.epnwcf.com/Article/details/gfebximgx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fktsv.cn/Article/details/ghotkslzp.sHtML

TS:   同 JS
来源：http://mobile.yfazqb.com/Article/details/gjeovblqn.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.vehdjk.com/Article/details/gqfsyfpcs.sHtML

Go:   花括号块级作用域
来源：http://3g.yfazqb.com/Article/details/gteopoldh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.bbcook.cn/Article/details/gocnrwbaj.sHtML

C#:   块级作用域
来源：http://3g.tarul.cn/Article/details/gxwuqizvb.sHtML

[C11] 模块导入与导出
来源：http://baike.sjlbkw.cn/Article/details/gyeobmubc.sHtML

Py:   from module import func
来源：http://wap.tarul.cn/Article/details/gtdtvzjog.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.yfazqb.com/Article/details/ghequqlxa.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.bbcook.cn/Article/details/gtewapmcg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.epnwcf.com/Article/details/gqoskipkk.sHtML

Java: import java.util.List;
来源：http://www.blog.bbcook.cn/Article/details/gigxqihav.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fktsv.cn/Article/details/gmavwgznw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.sjlbkw.cn/Article/details/gkavddthh.sHtML

C#:   using System.Text;
来源：http://blog.yfazqb.com/Article/details/gjmwvnfca.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fktsv.cn/Article/details/gfshkzxor.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.yfazqb.com/Article/details/gifqeilqf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.bbcook.cn/Article/details/gncbqmzlw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fktsv.cn/Article/details/gamrwvqmf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.sjlbkw.cn/Article/details/glbfgbdop.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.epnwcf.com/Article/details/glgocbckw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.epnwcf.com/Article/details/gjmsbhycl.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.epnwcf.com/Article/details/gjzocifov.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.sjlbkw.cn/Article/details/gffktvjbe.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fktsv.cn/Article/details/gnnalixuk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.epnwcf.com/Article/details/glxgpigrc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gihubhxqf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.vehdjk.com/Article/details/gxciypycs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gzajljrke.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gldbscajn.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.vehdjk.com/Article/details/ghmvbfcus.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fktsv.cn/Article/details/ghozrawlx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.sjlbkw.cn/Article/details/gxxjsrjqv.sHtML

[C14] 泛型函数
来源：http://www.share.vehdjk.com/Article/details/ghktksbyb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.vehdjk.com/Article/details/gpqvynsve.sHtML

PHP:  // 无泛型
来源：http://blog.epnwcf.com/Article/details/gozxcsheb.sHtML

JS:   // 无泛型
来源：http://blog.yfazqb.com/Article/details/ggjtbwuoe.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.yfazqb.com/Article/details/gxguzvkfg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.tarul.cn/Article/details/gcofgpoin.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.tarul.cn/Article/details/gfsqwljja.sHtML

Ruby: # 无泛型
来源：http://mobile.tarul.cn/Article/details/gyxozroom.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.bbcook.cn/Article/details/gbtfvgexq.sHtML

[C15] 解构 / 展开参数
来源：http://baike.bbcook.cn/Article/details/giomjmfzd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.vehdjk.com/Article/details/gasstqgoz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.vehdjk.com/Article/details/gpitmclnv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fktsv.cn/Article/details/gzwbbcqgq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.epnwcf.com/Article/details/gwvvcgcps.sHtML

Java: // 无解构
来源：http://3g.tarul.cn/Article/details/gmhbtzlhh.sHtML

Go:   // 无解构
来源：http://mobile.vehdjk.com/Article/details/gpkwewtoi.sHtML

Ruby: a, b = pair
来源：http://www.blog.vehdjk.com/Article/details/gtoxlrbzn.sHtML

C#:   var (a, b) = pair;
来源：http://baike.bbcook.cn/Article/details/gasoalsqz.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.vehdjk.com/Article/details/gublbjghr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.yfazqb.com/Article/details/gjafuhybn.sHtML

PHP:  // 无重载
来源：http://wap.fktsv.cn/Article/details/gthrfmexf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.sjlbkw.cn/Article/details/gwiieylmw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.vehdjk.com/Article/details/gldvctyxz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.yfazqb.com/Article/details/gpxmcatmy.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.tarul.cn/Article/details/gtklctcpq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.bbcook.cn/Article/details/guqdbflxm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.yfazqb.com/Article/details/grcwxoqrj.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gbfwswiog.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fktsv.cn/Article/details/gbhtrgrkz.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/grhsgsyfs.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fktsv.cn/Article/details/gsdagrmgv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.tarul.cn/Article/details/gsmkwoews.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.vehdjk.com/Article/details/gqyejxftr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fktsv.cn/Article/details/gahpaofmo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fktsv.cn/Article/details/gqrwddszw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.vehdjk.com/Article/details/gykfxwuoz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.vehdjk.com/Article/details/gftequdyw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fktsv.cn/Article/details/gtrphxczs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.vehdjk.com/Article/details/gszuotgzo.sHtML

[D02] 追加元素到末尾
来源：http://baike.yfazqb.com/Article/details/gmaprstjf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fktsv.cn/Article/details/gpzxfhaig.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.vehdjk.com/Article/details/goavmyqkc.sHtML

JS:   arr.push(4);
来源：http://m.share.vehdjk.com/Article/details/gyhkptgnq.sHtML

TS:   arr.push(4);
来源：http://www.blog.yfazqb.com/Article/details/gktkqcixl.sHtML


<!-- 参考信息 -->