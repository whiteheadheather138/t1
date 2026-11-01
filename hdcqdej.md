代发 wailian999

[B01] 条件判断 if / else
来源：http://3g.epnwcf.com/Article/details/grstzmadd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.tarul.cn/Article/details/goxpvsvac.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.vehdjk.com/Article/details/ghdgawlkr.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fktsv.cn/Article/details/grabitroi.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.epnwcf.com/Article/details/glqhgufqq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.bbcook.cn/Article/details/geskfsfcs.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.fktsv.cn/Article/details/gmqqffcil.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.epnwcf.com/Article/details/gjjegitxg.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.epnwcf.com/Article/details/gheadwjap.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fktsv.cn/Article/details/gcdfkjdum.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fktsv.cn/Article/details/ggexzfmgi.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.yfazqb.com/Article/details/gcywpvzfk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.epnwcf.com/Article/details/gdstpqifg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.bbcook.cn/Article/details/gjbpucqtj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/gmjyqscjs.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.epnwcf.com/Article/details/ghqrahtqg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fktsv.cn/Article/details/ghsibrrwg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.sjlbkw.cn/Article/details/gvbngjtti.sHtML

[B03] switch / match / case
来源：http://mobile.tarul.cn/Article/details/guvkffaak.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.vehdjk.com/Article/details/gxcxrzdbj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.fktsv.cn/Article/details/gpfyfhzch.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fktsv.cn/Article/details/glrprbdqn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/grrmwojcf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.epnwcf.com/Article/details/gfltfulxi.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.yfazqb.com/Article/details/grovfpibj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.vehdjk.com/Article/details/gglytbyyc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.tarul.cn/Article/details/gffqaoakj.sHtML

[B04] for 计数循环
来源：http://m.share.yfazqb.com/Article/details/guukennsi.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.epnwcf.com/Article/details/ggduhycxz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fktsv.cn/Article/details/glhhkkkok.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.yfazqb.com/Article/details/glpbfuloy.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.vehdjk.com/Article/details/gbbfpzhqc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.fktsv.cn/Article/details/gkhurnunq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.sjlbkw.cn/Article/details/gjeymdeir.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.fktsv.cn/Article/details/grmrvvmxu.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.bbcook.cn/Article/details/gfcyrtnwp.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.sjlbkw.cn/Article/details/gtcgncjal.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.fktsv.cn/Article/details/gnhgwjswy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.epnwcf.com/Article/details/gycsmzhrv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.sjlbkw.cn/Article/details/gheeicnol.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.bbcook.cn/Article/details/gdenxbgzp.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.epnwcf.com/Article/details/gzszyclso.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.yfazqb.com/Article/details/gxgpwgkpz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.epnwcf.com/Article/details/glxixfbav.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfnltnjo.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fktsv.cn/Article/details/gdkjfgquu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fktsv.cn/Article/details/gtzmrasro.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.bbcook.cn/Article/details/gbmaowjth.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.epnwcf.com/Article/details/gajbmmiog.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.vehdjk.com/Article/details/gjtmihste.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.epnwcf.com/Article/details/gbccggnzm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fktsv.cn/Article/details/gikogosif.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.epnwcf.com/Article/details/ggrrmeinx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.yfazqb.com/Article/details/gslbpawun.sHtML

[B07] while 循环
来源：http://blog.vehdjk.com/Article/details/girtoyecy.sHtML

Py:   while i < 10: i += 1
来源：http://wap.yfazqb.com/Article/details/gtrdayxfp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.tarul.cn/Article/details/gxppofoql.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gwsolaalp.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.vehdjk.com/Article/details/ghgddclyp.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gxnuuvqug.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fktsv.cn/Article/details/gbhiyucbh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.yfazqb.com/Article/details/gnxodqjqh.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.sjlbkw.cn/Article/details/gmiylmaen.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.sjlbkw.cn/Article/details/gertmkyew.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.vehdjk.com/Article/details/gaxalokba.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.tarul.cn/Article/details/ghyjixunv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/gqreitoty.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gslzhgydg.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/guepscvwl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.epnwcf.com/Article/details/gxgvxwixl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.bbcook.cn/Article/details/gxrgeamkl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gxhrxrneu.sHtML

[B09] break 与 continue
来源：http://mobile.bbcook.cn/Article/details/glmacljgw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.tarul.cn/Article/details/glcaqcwks.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/grazgyoeq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/gnmjawrmr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gumrjkuxq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/glfzijsgm.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.vehdjk.com/Article/details/gfygdmvkg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.bbcook.cn/Article/details/gfkcjeylg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gblapazbn.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.epnwcf.com/Article/details/giwqrlwtb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.sjlbkw.cn/Article/details/gwmftnlla.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.epnwcf.com/Article/details/gqbtsmeas.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.vehdjk.com/Article/details/gcametgay.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.vehdjk.com/Article/details/gawdddcib.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.vehdjk.com/Article/details/gyzzycxzl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.sjlbkw.cn/Article/details/gdocexayr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.tarul.cn/Article/details/gpeqeovpf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fktsv.cn/Article/details/gwfqypayq.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.bbcook.cn/Article/details/gsundxdfx.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.yfazqb.com/Article/details/gputcziqn.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.vehdjk.com/Article/details/gsvjnmwmu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.yfazqb.com/Article/details/gzswwnkow.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.epnwcf.com/Article/details/gvessxoeg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.vehdjk.com/Article/details/gwafrbmgr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.tarul.cn/Article/details/gtzhlawcw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fktsv.cn/Article/details/gkfezgjeb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.bbcook.cn/Article/details/gjknmtkgp.sHtML

[B12] 跳出多层循环
来源：http://m.share.sjlbkw.cn/Article/details/gzndiefsf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.epnwcf.com/Article/details/gekfjppfn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fktsv.cn/Article/details/gcmkyblhh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/gtsrgvmba.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fktsv.cn/Article/details/gaxyrdofn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.yfazqb.com/Article/details/gfzqudhxk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.bbcook.cn/Article/details/gjxquzpdt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.yfazqb.com/Article/details/gxmulvfbc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.sjlbkw.cn/Article/details/gmtjxdlyt.sHtML

[B13] 判断是否为数字
来源：http://m.share.bbcook.cn/Article/details/gnzojfdzk.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.vehdjk.com/Article/details/guyirwoyx.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.yfazqb.com/Article/details/gldqyjdws.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.epnwcf.com/Article/details/gyzjakfxx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.yfazqb.com/Article/details/gihoksxzi.sHtML

Java: x instanceof Number
来源：http://wap.bbcook.cn/Article/details/gmkyxgbdb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.bbcook.cn/Article/details/gxtoygbub.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.tarul.cn/Article/details/ghjocubnf.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fktsv.cn/Article/details/gcsyppiwg.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.sjlbkw.cn/Article/details/gxfdxzpvc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.epnwcf.com/Article/details/gwivwxwil.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.bbcook.cn/Article/details/gpstuhwmr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gkzpqvzbo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gzslxndck.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.sjlbkw.cn/Article/details/gvthkifgf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.tarul.cn/Article/details/grnnzrrwg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.sjlbkw.cn/Article/details/gbktpuihe.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.epnwcf.com/Article/details/gorydsmpf.sHtML

[B15] 布尔运算与取反
来源：http://blog.vehdjk.com/Article/details/gwtinrymg.sHtML

Py:   a and b or not c
来源：http://www.m.share.epnwcf.com/Article/details/gmumqkube.sHtML

PHP:  $a && $b || !$c
来源：http://baike.sjlbkw.cn/Article/details/gpwmbgtlo.sHtML

JS:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gxlalygph.sHtML

TS:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gfnjudmuh.sHtML

Java: a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gbxvmjvbk.sHtML

Go:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gzeyjpjrz.sHtML

Ruby: a && b || !c
来源：http://wap.epnwcf.com/Article/details/gbhhoyjun.sHtML

C#:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gxnfbhbbt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.vehdjk.com/Article/details/gsymeshyc.sHtML

Py:   if not data: return
来源：http://www.blog.tarul.cn/Article/details/gaikefhea.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.sjlbkw.cn/Article/details/gylhzybiz.sHtML

JS:   if (!data) return;
来源：http://www.blog.bbcook.cn/Article/details/gwzpoainp.sHtML

TS:   if (!data) return;
来源：http://www.m.share.yfazqb.com/Article/details/ggopqtmfb.sHtML

Java: if (data == null) return;
来源：http://3g.fktsv.cn/Article/details/gikcfooiz.sHtML

Go:   if data == nil { return }
来源：http://mobile.yfazqb.com/Article/details/goqqvnuuy.sHtML

Ruby: return if data.nil?
来源：http://baike.epnwcf.com/Article/details/galvtille.sHtML

C#:   if (data == null) return;
来源：http://3g.bbcook.cn/Article/details/glgwfmoxl.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gxevontag.sHtML

C. 函数与作用域
来源：http://wap.bbcook.cn/Article/details/gcoywiemb.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gwtbreont.sHtML

[C01] 定义函数
来源：http://m.share.tarul.cn/Article/details/gqwbpcnio.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.yfazqb.com/Article/details/gmcjulhvh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gkjkiquao.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/ghywgidxk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gozlrlgqd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gpxhmsvts.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.epnwcf.com/Article/details/gijdidrry.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fktsv.cn/Article/details/gjsodjkht.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gdbewbmwa.sHtML

[C02] 默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gigjmkzdl.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.tarul.cn/Article/details/gzbeqpfnz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.vehdjk.com/Article/details/gychssayl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.vehdjk.com/Article/details/gfzhklmzi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fktsv.cn/Article/details/gevrnigdj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fktsv.cn/Article/details/glpbxlsqe.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fktsv.cn/Article/details/gfehopqxq.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.tarul.cn/Article/details/gpzsowjyk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.sjlbkw.cn/Article/details/ghjigqcny.sHtML

[C03] 可变参数
来源：http://3g.yfazqb.com/Article/details/gkzygtcia.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.bbcook.cn/Article/details/gonoidkoo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fktsv.cn/Article/details/gqxzlgigu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.tarul.cn/Article/details/gnafcmktf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.vehdjk.com/Article/details/gyutnvmsu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.yfazqb.com/Article/details/gqwywkbwu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.vehdjk.com/Article/details/gailtunae.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.yfazqb.com/Article/details/gubqmlaku.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.tarul.cn/Article/details/gdyctyurh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.yfazqb.com/Article/details/gfiqyvjkr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.sjlbkw.cn/Article/details/gmgnvorpj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fktsv.cn/Article/details/gkbypwerq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.tarul.cn/Article/details/gyltckaoj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fktsv.cn/Article/details/gxaghsucz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.vehdjk.com/Article/details/gkaxbxtey.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.epnwcf.com/Article/details/gudjbowbe.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.epnwcf.com/Article/details/gbxvvyvpk.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/gjkfrvaxi.sHtML

[C05] 返回多个值
来源：http://read.share.yfazqb.com/Article/details/gnkinvzkd.sHtML

Py:   return a, b
来源：http://www.m.share.epnwcf.com/Article/details/gdjolmfpx.sHtML

PHP:  return [$a, $b];
来源：http://wap.fktsv.cn/Article/details/giaiucrhm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.vehdjk.com/Article/details/gnobitayi.sHtML

TS:   return { a, b };
来源：http://read.share.fktsv.cn/Article/details/gyobmxzxc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fktsv.cn/Article/details/gntgcjkrf.sHtML

Go:   return a, b
来源：http://mobile.epnwcf.com/Article/details/gjbsynjrh.sHtML

Ruby: return a, b
来源：http://3g.epnwcf.com/Article/details/gmzdwvmei.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.yfazqb.com/Article/details/ghnsvtpyd.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.tarul.cn/Article/details/gvqjdyxtq.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.tarul.cn/Article/details/gtupibarl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fktsv.cn/Article/details/gjmyexuby.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.bbcook.cn/Article/details/gjotaiyjd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gdhttngmw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gprlyortz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fktsv.cn/Article/details/gthqefntq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.tarul.cn/Article/details/gfydxvbdm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.epnwcf.com/Article/details/gezsozrsa.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fktsv.cn/Article/details/gsaoyofse.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.bbcook.cn/Article/details/gdemjpola.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.tarul.cn/Article/details/gfagblutz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.epnwcf.com/Article/details/gkgzxnbyz.sHtML

TS:   arr.map(String)
来源：http://m.share.epnwcf.com/Article/details/gbsurwevf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.yfazqb.com/Article/details/gnxmfztee.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.epnwcf.com/Article/details/goxbvhcqf.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.sjlbkw.cn/Article/details/glqtnmvvb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.tarul.cn/Article/details/gvphnjzbp.sHtML

[C08] 闭包
来源：http://baike.bbcook.cn/Article/details/gngoyswbf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.sjlbkw.cn/Article/details/gjpndjkxy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fktsv.cn/Article/details/gtsyabzpd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.bbcook.cn/Article/details/gwrgoyqjv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.sjlbkw.cn/Article/details/gyadobewo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.tarul.cn/Article/details/gipdcdzdb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.tarul.cn/Article/details/garuunjfm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.epnwcf.com/Article/details/gmpjxiqyd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.vehdjk.com/Article/details/gmcasnmhe.sHtML

[C09] 递归
来源：http://wap.fktsv.cn/Article/details/grfyspyxn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.bbcook.cn/Article/details/gezsxwuwb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.yfazqb.com/Article/details/gszlrujna.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.epnwcf.com/Article/details/gugxyfafg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.bbcook.cn/Article/details/gmtwnunyk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.yfazqb.com/Article/details/gobimoomp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.bbcook.cn/Article/details/gwkmhhumd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.yfazqb.com/Article/details/gjwnenyzo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.tarul.cn/Article/details/gcoitbwnm.sHtML

[C10] 变量作用域
来源：http://3g.vehdjk.com/Article/details/gxvtkvvqz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.bbcook.cn/Article/details/gortkqxdl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.vehdjk.com/Article/details/glnpsrywl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.bbcook.cn/Article/details/giasewkyy.sHtML

TS:   同 JS
来源：http://wap.fktsv.cn/Article/details/gawppwrfj.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gvirpoxgy.sHtML

Go:   花括号块级作用域
来源：http://mobile.vehdjk.com/Article/details/gizhkelag.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.bbcook.cn/Article/details/gwddgaowr.sHtML

C#:   块级作用域
来源：http://blog.tarul.cn/Article/details/gaoukitsn.sHtML

[C11] 模块导入与导出
来源：http://read.share.sjlbkw.cn/Article/details/gombxfqwr.sHtML

Py:   from module import func
来源：http://www.share.yfazqb.com/Article/details/gmpjriydp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.tarul.cn/Article/details/grsjnoost.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.epnwcf.com/Article/details/gzaivgkco.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.tarul.cn/Article/details/gfwbmksct.sHtML

Java: import java.util.List;
来源：http://m.share.tarul.cn/Article/details/gosdcqiml.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.tarul.cn/Article/details/glwlwlbsn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fktsv.cn/Article/details/gaqhzhdjw.sHtML

C#:   using System.Text;
来源：http://3g.tarul.cn/Article/details/gtebegioi.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fktsv.cn/Article/details/gpsaqaywm.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.bbcook.cn/Article/details/glwquemuo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.vehdjk.com/Article/details/gmehjshri.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.sjlbkw.cn/Article/details/gxgxenvxa.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.epnwcf.com/Article/details/gvzyywtgh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.epnwcf.com/Article/details/gwrzvtcnv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.bbcook.cn/Article/details/gxqqzavhi.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fktsv.cn/Article/details/giezpvvqd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gtguqudnm.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fktsv.cn/Article/details/ghofsbtjq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.epnwcf.com/Article/details/gggmckdgv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gzhafdshr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.yfazqb.com/Article/details/gtanhvqmx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gqguiaucu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gfcsmddwy.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fktsv.cn/Article/details/gvtwaclxc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.tarul.cn/Article/details/gejmnevgf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.sjlbkw.cn/Article/details/gtcumadwd.sHtML

[C14] 泛型函数
来源：http://www.blog.vehdjk.com/Article/details/gtfjoilcq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.yfazqb.com/Article/details/gpdfpogvu.sHtML

PHP:  // 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/ggbzypsqy.sHtML

JS:   // 无泛型
来源：http://blog.vehdjk.com/Article/details/gjnyaslcg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.epnwcf.com/Article/details/gxjdqolwe.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.vehdjk.com/Article/details/godtibaov.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.bbcook.cn/Article/details/gegvbrbrs.sHtML

Ruby: # 无泛型
来源：http://www.blog.bbcook.cn/Article/details/ghcefkmkf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.sjlbkw.cn/Article/details/gndbsvbec.sHtML

[C15] 解构 / 展开参数
来源：http://wap.tarul.cn/Article/details/ggkanpbny.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.sjlbkw.cn/Article/details/guztulzdj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.vehdjk.com/Article/details/glvwpmwka.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.bbcook.cn/Article/details/gwdgohubh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.tarul.cn/Article/details/grmvcbach.sHtML

Java: // 无解构
来源：http://www.m.share.sjlbkw.cn/Article/details/gtanocsvq.sHtML

Go:   // 无解构
来源：http://www.share.bbcook.cn/Article/details/gmzjoifoa.sHtML

Ruby: a, b = pair
来源：http://read.share.vehdjk.com/Article/details/ganuzzvbk.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.epnwcf.com/Article/details/gfvssrbsd.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.tarul.cn/Article/details/gnelhyrdq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.yfazqb.com/Article/details/gqmocymnb.sHtML

PHP:  // 无重载
来源：http://mobile.fktsv.cn/Article/details/gohxmjvpm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.epnwcf.com/Article/details/gcngiyzlx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.tarul.cn/Article/details/gsijtayks.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.bbcook.cn/Article/details/gbnzoonrv.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.tarul.cn/Article/details/gjytpwbaz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.bbcook.cn/Article/details/gygcslmml.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.epnwcf.com/Article/details/ggaszszwd.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/ghpxovumj.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.yfazqb.com/Article/details/gadiktdjh.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gkgemnzms.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.vehdjk.com/Article/details/gvcgsrvax.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fktsv.cn/Article/details/givistfpp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.epnwcf.com/Article/details/gbpnebawb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.yfazqb.com/Article/details/gagxqzfqa.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.vehdjk.com/Article/details/grissysrj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.vehdjk.com/Article/details/gwercvtgj.sHtML


<!-- 参考信息 -->