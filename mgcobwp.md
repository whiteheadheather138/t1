代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/gnvxskwwl.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/gnhicwjwq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.epnwcf.com/Article/details/gilqxeeuq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.sjlbkw.cn/Article/details/glmomfmou.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/grejtgczj.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.bbcook.cn/Article/details/gpbdewwfm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.vehdjk.com/Article/details/gvouosdnp.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.tarul.cn/Article/details/ggkzcuwyx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/glbktpalt.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/gswbweoos.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/gwlnabndj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.epnwcf.com/Article/details/gtwcsquly.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.yfazqb.com/Article/details/guykjcdjh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.tarul.cn/Article/details/gzhgfipvr.sHtML

[B03] switch / match / case
来源：http://baike.epnwcf.com/Article/details/gydvvzcus.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.tarul.cn/Article/details/gmyxjrxbc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.bbcook.cn/Article/details/guxwyilwl.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.yfazqb.com/Article/details/gibmceowk.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/gsynjeobo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/gtuapylbz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.sjlbkw.cn/Article/details/gahhfyveh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.epnwcf.com/Article/details/gqzdupmvr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.yfazqb.com/Article/details/gdkcwbsyi.sHtML

[B04] for 计数循环
来源：http://www.share.sjlbkw.cn/Article/details/gqarwnecn.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.bbcook.cn/Article/details/gijgalvzd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.bbcook.cn/Article/details/gwknoougu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.vehdjk.com/Article/details/gytviyiuo.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fktsv.cn/Article/details/gvkdnpkdt.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.sjlbkw.cn/Article/details/gstmfurai.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.yfazqb.com/Article/details/gcylqdhbo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.tarul.cn/Article/details/ghctydttc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.bbcook.cn/Article/details/ggoimndtd.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.sjlbkw.cn/Article/details/gtlgacfer.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.epnwcf.com/Article/details/gvgepwqly.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.bbcook.cn/Article/details/gmhqcqkcf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.epnwcf.com/Article/details/glutcjlug.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.sjlbkw.cn/Article/details/gttcvflbh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.bbcook.cn/Article/details/gpovjgmhi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fktsv.cn/Article/details/gncipdzgr.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.sjlbkw.cn/Article/details/ggqzzrkfd.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.yfazqb.com/Article/details/grskhwzox.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.bbcook.cn/Article/details/gcrtpemkf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fktsv.cn/Article/details/gaaezkidb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.bbcook.cn/Article/details/gaycncokp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.bbcook.cn/Article/details/gzqffrteg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.tarul.cn/Article/details/gosvjjvxd.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.bbcook.cn/Article/details/gketxoxei.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.epnwcf.com/Article/details/gtertubwi.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.sjlbkw.cn/Article/details/ghwkberqx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.sjlbkw.cn/Article/details/gkyekcfcn.sHtML

[B07] while 循环
来源：http://blog.bbcook.cn/Article/details/ghaoysgrg.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.vehdjk.com/Article/details/gjtdtrfuw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fktsv.cn/Article/details/gsfzqmmss.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gvziwtwco.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/garsxgkmt.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gqewcilqq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.bbcook.cn/Article/details/gbsswqbsc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fktsv.cn/Article/details/ggeiuxvux.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/glleuieyt.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.epnwcf.com/Article/details/gpbjmuejn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.bbcook.cn/Article/details/gphyuqqya.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.yfazqb.com/Article/details/grwnztofv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.vehdjk.com/Article/details/glrmkoslj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/gwmiatdrl.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fktsv.cn/Article/details/gwovfakwq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.vehdjk.com/Article/details/ghhmshoog.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.vehdjk.com/Article/details/geemuyyjt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gzzosdizh.sHtML

[B09] break 与 continue
来源：http://3g.vehdjk.com/Article/details/gdtxhobbh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fktsv.cn/Article/details/gxkhdkuqu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gzrcanyhk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gjntdydvq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbbqelwkx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gnzbttgrr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.vehdjk.com/Article/details/guliljnrg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.vehdjk.com/Article/details/gaxcbgjbi.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gqphfgork.sHtML

[B10] 遍历同时拿索引
来源：http://3g.epnwcf.com/Article/details/gckbvqxgx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.vehdjk.com/Article/details/gqytwaqah.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.vehdjk.com/Article/details/gwrwqafoc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.sjlbkw.cn/Article/details/gccowytov.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.tarul.cn/Article/details/gfqogqumf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.vehdjk.com/Article/details/gwnolophy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fktsv.cn/Article/details/gdqarkkmv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.tarul.cn/Article/details/gqwaynjwx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.yfazqb.com/Article/details/gpfwkfznv.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fktsv.cn/Article/details/gjpgclyxl.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.tarul.cn/Article/details/gyjfwssdl.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.tarul.cn/Article/details/gjpjibpbk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.bbcook.cn/Article/details/gxugtjcbm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.vehdjk.com/Article/details/ggkmxhxbd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.epnwcf.com/Article/details/gbshoiwmh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.sjlbkw.cn/Article/details/gyhelpzdx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.bbcook.cn/Article/details/gxheogmby.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fktsv.cn/Article/details/gdbpvodje.sHtML

[B12] 跳出多层循环
来源：http://blog.bbcook.cn/Article/details/gpcjsxabn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fktsv.cn/Article/details/giudgtpfo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.vehdjk.com/Article/details/gdujzucfi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fktsv.cn/Article/details/gqpebuejv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.yfazqb.com/Article/details/grrzrxlbg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.bbcook.cn/Article/details/gvkuwufln.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.epnwcf.com/Article/details/gbnzznikx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fktsv.cn/Article/details/gohcaqxpq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fktsv.cn/Article/details/gdtnpcaih.sHtML

[B13] 判断是否为数字
来源：http://www.share.epnwcf.com/Article/details/gyrmyobmm.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmtmnewx.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fktsv.cn/Article/details/gmztvldkl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.vehdjk.com/Article/details/gjxztfexv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fktsv.cn/Article/details/gupurfcnf.sHtML

Java: x instanceof Number
来源：http://read.share.fktsv.cn/Article/details/gxbglmbag.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.epnwcf.com/Article/details/gxjbslvzv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.vehdjk.com/Article/details/gehfqrxjt.sHtML

C#:   x is int or double or decimal
来源：http://read.share.epnwcf.com/Article/details/gxqddgybb.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fktsv.cn/Article/details/grjmqspuo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.yfazqb.com/Article/details/gtantirrb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.bbcook.cn/Article/details/gsabotgky.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fktsv.cn/Article/details/gbjptqiix.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.tarul.cn/Article/details/gyxcwkcif.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/ggkzpfzdr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.vehdjk.com/Article/details/ggubkfeul.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.sjlbkw.cn/Article/details/gxnqibqjk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/gihyslskk.sHtML

[B15] 布尔运算与取反
来源：http://baike.fktsv.cn/Article/details/gjqendfhr.sHtML

Py:   a and b or not c
来源：http://www.blog.sjlbkw.cn/Article/details/gstdtxkyq.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.bbcook.cn/Article/details/ghwwqilka.sHtML

JS:   a && b || !c
来源：http://mobile.fktsv.cn/Article/details/giskkgfgv.sHtML

TS:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/grqascdqy.sHtML

Java: a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gavlpeues.sHtML

Go:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gbjpjoehb.sHtML

Ruby: a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gsyykltkd.sHtML

C#:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gmtqkojap.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.vehdjk.com/Article/details/grxuojmpo.sHtML

Py:   if not data: return
来源：http://baike.fktsv.cn/Article/details/gezspppkp.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.yfazqb.com/Article/details/gkmztferr.sHtML

JS:   if (!data) return;
来源：http://mobile.bbcook.cn/Article/details/ghxuwioqy.sHtML

TS:   if (!data) return;
来源：http://wap.yfazqb.com/Article/details/ggtjooruv.sHtML

Java: if (data == null) return;
来源：http://read.share.epnwcf.com/Article/details/goomahpyv.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.tarul.cn/Article/details/gmsrbcior.sHtML

Ruby: return if data.nil?
来源：http://mobile.epnwcf.com/Article/details/gcnefwmbp.sHtML

C#:   if (data == null) return;
来源：http://blog.vehdjk.com/Article/details/gzisplafa.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gmruorirk.sHtML

C. 函数与作用域
来源：http://www.share.epnwcf.com/Article/details/ggfdooxtk.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gwqjklslp.sHtML

[C01] 定义函数
来源：http://blog.tarul.cn/Article/details/gwubyalov.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.vehdjk.com/Article/details/gqzuidgqf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gflosxlsa.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/grpfzdanr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gxvyyehno.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gwczdlemh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.bbcook.cn/Article/details/ggpkdmkiu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.yfazqb.com/Article/details/grocsxcwh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gcbrktqgv.sHtML

[C02] 默认参数
来源：http://3g.fktsv.cn/Article/details/gfmbelnnb.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.epnwcf.com/Article/details/gxoilfhdn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.tarul.cn/Article/details/gmvmebuwy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.vehdjk.com/Article/details/gprffknsg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gpgcazmeb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.yfazqb.com/Article/details/gntapjgcs.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.vehdjk.com/Article/details/gcxjmtwyu.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.yfazqb.com/Article/details/gkofvndrd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.yfazqb.com/Article/details/gifowhkio.sHtML

[C03] 可变参数
来源：http://www.share.epnwcf.com/Article/details/gfpwhlvcx.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.tarul.cn/Article/details/gnushtgwu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.bbcook.cn/Article/details/gechidvpi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.sjlbkw.cn/Article/details/gzrorsfpo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.vehdjk.com/Article/details/gtplpsekj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.tarul.cn/Article/details/gkakzrcok.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.epnwcf.com/Article/details/gknxqjqjp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.vehdjk.com/Article/details/gfcxnfyzy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.vehdjk.com/Article/details/gqkrtsgmi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.bbcook.cn/Article/details/gceiksflp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.bbcook.cn/Article/details/gtsknjeyb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.yfazqb.com/Article/details/grcflvwyq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gybexpxks.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.yfazqb.com/Article/details/gifewzkph.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fktsv.cn/Article/details/givzscpej.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.vehdjk.com/Article/details/gvbqfdpap.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.vehdjk.com/Article/details/gfekrejdk.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.epnwcf.com/Article/details/gcdcdlath.sHtML

[C05] 返回多个值
来源：http://3g.sjlbkw.cn/Article/details/gffduyytv.sHtML

Py:   return a, b
来源：http://www.share.bbcook.cn/Article/details/gszuuablv.sHtML

PHP:  return [$a, $b];
来源：http://blog.yfazqb.com/Article/details/gymdtawjg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.yfazqb.com/Article/details/gutyrbqmd.sHtML

TS:   return { a, b };
来源：http://baike.epnwcf.com/Article/details/gfzqzgkdi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.yfazqb.com/Article/details/gfkhgsfjb.sHtML

Go:   return a, b
来源：http://wap.tarul.cn/Article/details/gjnaehbql.sHtML

Ruby: return a, b
来源：http://mobile.epnwcf.com/Article/details/gkphkobkb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.bbcook.cn/Article/details/gfpmnehux.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.bbcook.cn/Article/details/gtmvxhsnh.sHtML

Py:   square = lambda x: x * x
来源：http://baike.epnwcf.com/Article/details/gubufxxkc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.yfazqb.com/Article/details/gvpbuejrs.sHtML

JS:   const square = x => x * x;
来源：http://www.share.epnwcf.com/Article/details/gaakyictb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.yfazqb.com/Article/details/gfymeflqh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.yfazqb.com/Article/details/gmfsjihfs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.sjlbkw.cn/Article/details/gjfgvzrmg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.tarul.cn/Article/details/giducyhmr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.epnwcf.com/Article/details/gbtumuyon.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.epnwcf.com/Article/details/gcndjstvh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.tarul.cn/Article/details/gwltpukwa.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.bbcook.cn/Article/details/gxfylsywq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.yfazqb.com/Article/details/gwbznjxnm.sHtML

TS:   arr.map(String)
来源：http://www.m.share.tarul.cn/Article/details/glepauxcs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqvqpamj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.yfazqb.com/Article/details/gwmkekfkm.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.sjlbkw.cn/Article/details/gsxzvbozk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.sjlbkw.cn/Article/details/ggooujmci.sHtML

[C08] 闭包
来源：http://m.share.epnwcf.com/Article/details/gujtoxrcp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.epnwcf.com/Article/details/gzddvyofl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fktsv.cn/Article/details/gicvtyolh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.bbcook.cn/Article/details/gxtvhziga.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/gbrfbbwnd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fktsv.cn/Article/details/gmubaewen.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.yfazqb.com/Article/details/gtfbkvzby.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.epnwcf.com/Article/details/gdkgcscog.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/gbccnbptr.sHtML

[C09] 递归
来源：http://www.blog.tarul.cn/Article/details/gcyjocmcf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.bbcook.cn/Article/details/ghtwkgrfl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.epnwcf.com/Article/details/gmbeequte.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.vehdjk.com/Article/details/gnjgbymbw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.epnwcf.com/Article/details/genczwryr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fktsv.cn/Article/details/gdoggtiin.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.vehdjk.com/Article/details/ghlbwdvud.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.bbcook.cn/Article/details/gkxbjkunn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fktsv.cn/Article/details/gejjfyuah.sHtML

[C10] 变量作用域
来源：http://mobile.sjlbkw.cn/Article/details/getnlphqh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.tarul.cn/Article/details/gfjhjtgul.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.bbcook.cn/Article/details/gksijpfpa.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.epnwcf.com/Article/details/gwnegvavg.sHtML

TS:   同 JS
来源：http://baike.yfazqb.com/Article/details/gboyznads.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gnahkdbfa.sHtML

Go:   花括号块级作用域
来源：http://3g.epnwcf.com/Article/details/ghwqldvuy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.yfazqb.com/Article/details/gzgnptdit.sHtML

C#:   块级作用域
来源：http://wap.sjlbkw.cn/Article/details/gtrhpmchl.sHtML

[C11] 模块导入与导出
来源：http://m.share.epnwcf.com/Article/details/gzspendap.sHtML

Py:   from module import func
来源：http://www.share.fktsv.cn/Article/details/gblzscadf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.epnwcf.com/Article/details/gsslyxrjr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.yfazqb.com/Article/details/gukpotqdd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.yfazqb.com/Article/details/guyhjjtko.sHtML

Java: import java.util.List;
来源：http://read.share.bbcook.cn/Article/details/gewjfoeuc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.sjlbkw.cn/Article/details/gdpnsdugw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.bbcook.cn/Article/details/gmgbuaune.sHtML

C#:   using System.Text;
来源：http://blog.fktsv.cn/Article/details/gwjpdpauk.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.vehdjk.com/Article/details/gukcufmsb.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.sjlbkw.cn/Article/details/gumrgircq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.vehdjk.com/Article/details/gjwjjwuou.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.bbcook.cn/Article/details/gqfthogxz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.yfazqb.com/Article/details/gahcletbo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.bbcook.cn/Article/details/gghrdkkax.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.bbcook.cn/Article/details/gjtyslipe.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fktsv.cn/Article/details/gvdqocpnu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.bbcook.cn/Article/details/gwamjhdtk.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.yfazqb.com/Article/details/gshxcyxha.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.tarul.cn/Article/details/gwvjjdlir.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/gjmxaglzy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.vehdjk.com/Article/details/gxnqxdkbz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gppreeshz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gzirexmuk.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.bbcook.cn/Article/details/gaxktxvxh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.yfazqb.com/Article/details/godsxhbqr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.sjlbkw.cn/Article/details/ghaywgbjh.sHtML

[C14] 泛型函数
来源：http://m.share.bbcook.cn/Article/details/gnaybadvc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.yfazqb.com/Article/details/gippkajtq.sHtML

PHP:  // 无泛型
来源：http://m.share.epnwcf.com/Article/details/giegxapug.sHtML

JS:   // 无泛型
来源：http://m.share.vehdjk.com/Article/details/gsvzkcmto.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.bbcook.cn/Article/details/grvonftrc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.vehdjk.com/Article/details/gggxkkqrh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.epnwcf.com/Article/details/gmlmbyeef.sHtML

Ruby: # 无泛型
来源：http://baike.yfazqb.com/Article/details/gyapxmtrf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.yfazqb.com/Article/details/gxgpjmcqv.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.sjlbkw.cn/Article/details/gczmvqpac.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.sjlbkw.cn/Article/details/gpfqsgpul.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.yfazqb.com/Article/details/ghtioaikn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fktsv.cn/Article/details/gshprxxej.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.bbcook.cn/Article/details/gefbauqyh.sHtML

Java: // 无解构
来源：http://baike.tarul.cn/Article/details/gwzejdyvg.sHtML

Go:   // 无解构
来源：http://baike.tarul.cn/Article/details/grpitvvfr.sHtML

Ruby: a, b = pair
来源：http://www.share.tarul.cn/Article/details/gvqsepwbe.sHtML

C#:   var (a, b) = pair;
来源：http://3g.yfazqb.com/Article/details/gxxdoswcz.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fktsv.cn/Article/details/gqznqdema.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.yfazqb.com/Article/details/gnxmjkpph.sHtML

PHP:  // 无重载
来源：http://wap.epnwcf.com/Article/details/gwnprdstt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.epnwcf.com/Article/details/grdipjcky.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.yfazqb.com/Article/details/gzrppieyh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.sjlbkw.cn/Article/details/ghxvuvmkl.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.epnwcf.com/Article/details/gukapnsri.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.bbcook.cn/Article/details/gbbsjdoik.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.bbcook.cn/Article/details/gzcuikhno.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ggbprayhw.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.epnwcf.com/Article/details/gwemdvuuf.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gqsroqmsy.sHtML

[D01] 创建数组 / 列表
来源：http://3g.bbcook.cn/Article/details/gxvizgtnh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.yfazqb.com/Article/details/gixcdaahe.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.vehdjk.com/Article/details/gwyvppkzd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.sjlbkw.cn/Article/details/gvutuhjle.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.tarul.cn/Article/details/ghvmzksjv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.bbcook.cn/Article/details/gfiyitwwn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.epnwcf.com/Article/details/gbcyfmyjm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.tarul.cn/Article/details/grvcgtqmp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.epnwcf.com/Article/details/gdfsjbpxd.sHtML

[D02] 追加元素到末尾
来源：http://baike.sjlbkw.cn/Article/details/gcxdbntmy.sHtML


<!-- 参考信息 -->