代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.sjlbkw.cn/Article/details/gshpqnyic.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.bbcook.cn/Article/details/gecvvrfgh.sHtML

[B03] switch / match / case
来源：http://www.blog.tarul.cn/Article/details/gkjzznwzq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.epnwcf.com/Article/details/ggjxmloex.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.vehdjk.com/Article/details/gjzwpxzyl.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.tarul.cn/Article/details/gjziucbhd.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/gfszkdrar.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.bbcook.cn/Article/details/gzamrodwb.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.yfazqb.com/Article/details/giftpixqc.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.sjlbkw.cn/Article/details/ggwwjbhvr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fktsv.cn/Article/details/gdfsxjzoo.sHtML

[B04] for 计数循环
来源：http://www.m.share.epnwcf.com/Article/details/ghztdgsrt.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.bbcook.cn/Article/details/gsgcjqrgh.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.vehdjk.com/Article/details/grgfkyzek.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fktsv.cn/Article/details/gxlclghgu.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.epnwcf.com/Article/details/gigrvctqr.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.epnwcf.com/Article/details/gtukwnlvj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fktsv.cn/Article/details/gtjphspok.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.sjlbkw.cn/Article/details/gfrjyrtzl.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.tarul.cn/Article/details/gujqufihp.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.yfazqb.com/Article/details/gnekaypqt.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.vehdjk.com/Article/details/gsgfgawbq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.tarul.cn/Article/details/gazmfgmze.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.tarul.cn/Article/details/gtvirexfg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.sjlbkw.cn/Article/details/goxbkhiwh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fktsv.cn/Article/details/gzdfwpjdj.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fktsv.cn/Article/details/gdxotzsou.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.yfazqb.com/Article/details/gumpxohjc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.epnwcf.com/Article/details/glpgpyryb.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.bbcook.cn/Article/details/guerlbisl.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.tarul.cn/Article/details/gqakijpdd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.epnwcf.com/Article/details/ghotjldgw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.epnwcf.com/Article/details/gvyujmlqs.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fktsv.cn/Article/details/gefmlpiyu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.bbcook.cn/Article/details/gwowggqtf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.vehdjk.com/Article/details/gpqloevum.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.epnwcf.com/Article/details/gzeijwycc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.tarul.cn/Article/details/gwdzxkdlg.sHtML

[B07] while 循环
来源：http://baike.yfazqb.com/Article/details/gzfxwfmvb.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.sjlbkw.cn/Article/details/ggqzvmjeq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.vehdjk.com/Article/details/gupobxupl.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtubihrop.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/gxlesqxnv.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/gxagaabme.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.sjlbkw.cn/Article/details/gtnuwfhdu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.yfazqb.com/Article/details/gbjpudxcq.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/gliewhgsw.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.sjlbkw.cn/Article/details/gktkbaayd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.epnwcf.com/Article/details/gdpbaaqrc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.sjlbkw.cn/Article/details/gbqqurchx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gdaifryvs.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/gmotyvemm.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcsfhzuzp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.vehdjk.com/Article/details/ghmvdelru.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.yfazqb.com/Article/details/gewwcpeny.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.bbcook.cn/Article/details/gizsgmews.sHtML

[B09] break 与 continue
来源：http://www.share.bbcook.cn/Article/details/gxialwrxs.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.yfazqb.com/Article/details/gqkwifkpr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/ggbfwdsks.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/ggunikedh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/gitbiznbh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/gskgzyijw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.epnwcf.com/Article/details/gcoyzraac.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.yfazqb.com/Article/details/ghrrtymkh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gmdiuijyb.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.bbcook.cn/Article/details/ghwcjedvb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.sjlbkw.cn/Article/details/gahmpywwe.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.yfazqb.com/Article/details/ggbziuxbj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.epnwcf.com/Article/details/gdovjbofj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fktsv.cn/Article/details/grxruukrs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.tarul.cn/Article/details/gsfdljufn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.vehdjk.com/Article/details/gffnpptyw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.bbcook.cn/Article/details/gmlqjvckc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.yfazqb.com/Article/details/gqyhizmiw.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.epnwcf.com/Article/details/gvigrhaql.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.tarul.cn/Article/details/gjkbzrhfp.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.vehdjk.com/Article/details/graaiifsz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.bbcook.cn/Article/details/glcekcbhg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.bbcook.cn/Article/details/gqrgdgvoe.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.yfazqb.com/Article/details/geshgyvur.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.vehdjk.com/Article/details/gbgsdedkv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.yfazqb.com/Article/details/gtjsaivzq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.vehdjk.com/Article/details/givxhyvwf.sHtML

[B12] 跳出多层循环
来源：http://blog.bbcook.cn/Article/details/gevocngbp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.epnwcf.com/Article/details/gmkulxxqv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.tarul.cn/Article/details/gykadjysn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/gfjgwrazs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/gyoigavhx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.sjlbkw.cn/Article/details/gmtjelzhv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fktsv.cn/Article/details/gvrenwrxe.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.sjlbkw.cn/Article/details/gvjnfdzcc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.vehdjk.com/Article/details/gwffodvmn.sHtML

[B13] 判断是否为数字
来源：http://www.share.tarul.cn/Article/details/gsudnzokm.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fktsv.cn/Article/details/gqofepgph.sHtML

PHP:  is_numeric($x)
来源：http://mobile.sjlbkw.cn/Article/details/gtjtfvfcv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.tarul.cn/Article/details/gmaesuopq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.bbcook.cn/Article/details/gklcvmfcw.sHtML

Java: x instanceof Number
来源：http://www.blog.bbcook.cn/Article/details/gartkpsxq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fktsv.cn/Article/details/gsvmlqbyl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fktsv.cn/Article/details/gqczonqio.sHtML

C#:   x is int or double or decimal
来源：http://blog.epnwcf.com/Article/details/gdavyiufv.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.vehdjk.com/Article/details/goknqushu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.bbcook.cn/Article/details/gciauniou.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.bbcook.cn/Article/details/gvrsypkhc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fktsv.cn/Article/details/gqmhgqsgv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.bbcook.cn/Article/details/geoivqzpq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gnpguaxbk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fktsv.cn/Article/details/gnxlkcmqd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.tarul.cn/Article/details/gqoxwsfpq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.epnwcf.com/Article/details/ganrkcmmu.sHtML

[B15] 布尔运算与取反
来源：http://mobile.sjlbkw.cn/Article/details/ghlhimllt.sHtML

Py:   a and b or not c
来源：http://wap.bbcook.cn/Article/details/gunxjrjvu.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.bbcook.cn/Article/details/gsxwgxqrw.sHtML

JS:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gbaxbxsgd.sHtML

TS:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gccpikngb.sHtML

Java: a && b || !c
来源：http://baike.epnwcf.com/Article/details/gnhkwmvfa.sHtML

Go:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gvjthdusl.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gdancppoi.sHtML

C#:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gnzlbhcvc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.tarul.cn/Article/details/ggdghnweg.sHtML

Py:   if not data: return
来源：http://blog.tarul.cn/Article/details/gnwjlmurj.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.tarul.cn/Article/details/gghfczjen.sHtML

JS:   if (!data) return;
来源：http://m.share.vehdjk.com/Article/details/gsjyacceo.sHtML

TS:   if (!data) return;
来源：http://read.share.tarul.cn/Article/details/ghyflotyz.sHtML

Java: if (data == null) return;
来源：http://www.blog.tarul.cn/Article/details/gjqztyrbj.sHtML

Go:   if data == nil { return }
来源：http://read.share.fktsv.cn/Article/details/gkjitkrrc.sHtML

Ruby: return if data.nil?
来源：http://m.share.fktsv.cn/Article/details/ghsvbyoev.sHtML

C#:   if (data == null) return;
来源：http://3g.bbcook.cn/Article/details/gnpwotoxl.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gijccmdlu.sHtML

C. 函数与作用域
来源：http://www.m.share.bbcook.cn/Article/details/gvujjkcmz.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/grusoghfj.sHtML

[C01] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/gzfjjtuzq.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fktsv.cn/Article/details/gzyvcwzhn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gwbtvuoir.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/grpzfsrgw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gzjferbsj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gwmnhdfhs.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.vehdjk.com/Article/details/gryieiyvj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.epnwcf.com/Article/details/gvfkfodlj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gtgpxgdth.sHtML

[C02] 默认参数
来源：http://m.share.yfazqb.com/Article/details/gvxizrvqe.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.vehdjk.com/Article/details/geipocdmq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.sjlbkw.cn/Article/details/gobxjrrvx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.yfazqb.com/Article/details/gdkmjccjl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gzcrmchmg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.bbcook.cn/Article/details/gxhqqpdbg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fktsv.cn/Article/details/gyrfktrvr.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.bbcook.cn/Article/details/gnanqbiea.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.epnwcf.com/Article/details/gizlefbkm.sHtML

[C03] 可变参数
来源：http://baike.fktsv.cn/Article/details/giwhjucdt.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.bbcook.cn/Article/details/gjvbskfmj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.vehdjk.com/Article/details/gygciiqii.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.tarul.cn/Article/details/gwmebqxkq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fktsv.cn/Article/details/gpghewvzg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.sjlbkw.cn/Article/details/glgptfoac.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fktsv.cn/Article/details/gxczncyay.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.epnwcf.com/Article/details/glokhjaxb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.vehdjk.com/Article/details/gnixpdipi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.tarul.cn/Article/details/grmwyfykl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fktsv.cn/Article/details/gebgwjotb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.yfazqb.com/Article/details/ggszcefaj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.sjlbkw.cn/Article/details/gwcnpmqrb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.sjlbkw.cn/Article/details/gnbyjtpws.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fktsv.cn/Article/details/gpyxcmzym.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.tarul.cn/Article/details/gslrwtnak.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fktsv.cn/Article/details/gyyhncygi.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fktsv.cn/Article/details/grhbleijq.sHtML

[C05] 返回多个值
来源：http://mobile.fktsv.cn/Article/details/grwmrnnbd.sHtML

Py:   return a, b
来源：http://www.blog.vehdjk.com/Article/details/gbhcqvcho.sHtML

PHP:  return [$a, $b];
来源：http://baike.vehdjk.com/Article/details/gelntmibv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.bbcook.cn/Article/details/gloxchekg.sHtML

TS:   return { a, b };
来源：http://mobile.fktsv.cn/Article/details/gkpvvpbmi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.tarul.cn/Article/details/gthsmfswq.sHtML

Go:   return a, b
来源：http://www.blog.fktsv.cn/Article/details/gzwoqzbpr.sHtML

Ruby: return a, b
来源：http://www.m.share.tarul.cn/Article/details/gjszsatvy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fktsv.cn/Article/details/gtchmvknf.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.tarul.cn/Article/details/gcvpljiie.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.tarul.cn/Article/details/ggcuecebl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.tarul.cn/Article/details/gaugbhrjv.sHtML

JS:   const square = x => x * x;
来源：http://3g.yfazqb.com/Article/details/gjumjfdly.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gwhvlaqgw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fktsv.cn/Article/details/gljvdomax.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.yfazqb.com/Article/details/gsvykejfy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.tarul.cn/Article/details/gklgonofb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.yfazqb.com/Article/details/gmagscixr.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fktsv.cn/Article/details/gdagxxjih.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.sjlbkw.cn/Article/details/gfvmjjhmz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfsfgmxd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fktsv.cn/Article/details/gfbubfpor.sHtML

TS:   arr.map(String)
来源：http://blog.fktsv.cn/Article/details/gtgjykddu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.epnwcf.com/Article/details/ggozkpwpo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fktsv.cn/Article/details/gbijmkfpm.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.yfazqb.com/Article/details/ghvdlbbak.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.epnwcf.com/Article/details/gvwgrwjxo.sHtML

[C08] 闭包
来源：http://baike.tarul.cn/Article/details/gumzpiwth.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.epnwcf.com/Article/details/gavxpxkyu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.epnwcf.com/Article/details/gmvmgreef.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gujdkbuyp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fktsv.cn/Article/details/grdqrkhat.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.sjlbkw.cn/Article/details/gsrmhthne.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fktsv.cn/Article/details/gnrfurhnq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.sjlbkw.cn/Article/details/gaiopkgwy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.tarul.cn/Article/details/gnrlzkmbv.sHtML

[C09] 递归
来源：http://www.blog.yfazqb.com/Article/details/gywxpbnte.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/gwhmmggtv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.yfazqb.com/Article/details/gicgzoooe.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.sjlbkw.cn/Article/details/gmlpqsebj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.vehdjk.com/Article/details/ggdvcrvwo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.tarul.cn/Article/details/ggwsbsozs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.sjlbkw.cn/Article/details/gwukbtxxs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.yfazqb.com/Article/details/gbkivctoy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.vehdjk.com/Article/details/guffgrtfq.sHtML

[C10] 变量作用域
来源：http://www.share.epnwcf.com/Article/details/golsttjnj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.yfazqb.com/Article/details/goctqjtgc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.yfazqb.com/Article/details/gexucslqy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.epnwcf.com/Article/details/gdditrqcw.sHtML

TS:   同 JS
来源：http://3g.yfazqb.com/Article/details/gvcpzomeq.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gjqzdtzlt.sHtML

Go:   花括号块级作用域
来源：http://mobile.tarul.cn/Article/details/gnvfgeuns.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fktsv.cn/Article/details/gneuzhcvu.sHtML

C#:   块级作用域
来源：http://mobile.epnwcf.com/Article/details/gwawzzyln.sHtML

[C11] 模块导入与导出
来源：http://blog.sjlbkw.cn/Article/details/ggvjkvhxs.sHtML

Py:   from module import func
来源：http://wap.bbcook.cn/Article/details/gkarecixp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.vehdjk.com/Article/details/gvavhnffx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.epnwcf.com/Article/details/gibzschua.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.epnwcf.com/Article/details/gqabqhsdg.sHtML

Java: import java.util.List;
来源：http://m.share.sjlbkw.cn/Article/details/gdofthwcc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.yfazqb.com/Article/details/gurekgekr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.vehdjk.com/Article/details/gtkzmzvej.sHtML

C#:   using System.Text;
来源：http://baike.yfazqb.com/Article/details/gjkeooutp.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fktsv.cn/Article/details/gklzjzurs.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.yfazqb.com/Article/details/gjwdhojna.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.tarul.cn/Article/details/gcvltbntc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.sjlbkw.cn/Article/details/gyxqapvpv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fktsv.cn/Article/details/gtkgsjpih.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.epnwcf.com/Article/details/gsqzytrfw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.bbcook.cn/Article/details/gzzkgbxym.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.sjlbkw.cn/Article/details/gjduuwkzi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.vehdjk.com/Article/details/gzwxglbwt.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.bbcook.cn/Article/details/gjxaclpgw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhnqonzs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/glvlastdb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.epnwcf.com/Article/details/ghiezgjgb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gwsrqsgdd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gwpjuiwws.sHtML

Go:   func add(a, b int) int
来源：http://www.share.yfazqb.com/Article/details/gbqdtlfze.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.tarul.cn/Article/details/gzikghjpc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.bbcook.cn/Article/details/gdmriqrvq.sHtML

[C14] 泛型函数
来源：http://3g.yfazqb.com/Article/details/gqmovtjpb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.vehdjk.com/Article/details/gtueimtfl.sHtML

PHP:  // 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/gzrwifyjb.sHtML

JS:   // 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/ggjdkhifk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fktsv.cn/Article/details/gtzcyndbh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.sjlbkw.cn/Article/details/gyymhdjyy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.yfazqb.com/Article/details/gpmxqmqaq.sHtML

Ruby: # 无泛型
来源：http://baike.tarul.cn/Article/details/gnshdsbqc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.yfazqb.com/Article/details/goeiplxih.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.epnwcf.com/Article/details/gersvtqvz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.vehdjk.com/Article/details/gjzxascmn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.epnwcf.com/Article/details/gafqlvubc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.bbcook.cn/Article/details/gxczwcbnm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.bbcook.cn/Article/details/gacxzcttz.sHtML

Java: // 无解构
来源：http://baike.tarul.cn/Article/details/gdictcztg.sHtML

Go:   // 无解构
来源：http://3g.bbcook.cn/Article/details/glbgxnrmk.sHtML

Ruby: a, b = pair
来源：http://www.share.epnwcf.com/Article/details/gaqdyqxhh.sHtML

C#:   var (a, b) = pair;
来源：http://baike.bbcook.cn/Article/details/gsbuikcqu.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrunewdj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.sjlbkw.cn/Article/details/gnfttnffv.sHtML

PHP:  // 无重载
来源：http://mobile.vehdjk.com/Article/details/gcqzfscpn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.tarul.cn/Article/details/guoloafpe.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.sjlbkw.cn/Article/details/goqzxjhee.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.vehdjk.com/Article/details/gyluavzcm.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.vehdjk.com/Article/details/ghrgewust.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.tarul.cn/Article/details/gjfvkrcjg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.sjlbkw.cn/Article/details/gomddclfw.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gmcbdecxi.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.epnwcf.com/Article/details/gkqcyfkhs.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gbmmsgtfj.sHtML

[D01] 创建数组 / 列表
来源：http://wap.epnwcf.com/Article/details/gvkelakof.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.epnwcf.com/Article/details/gjjgswcic.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.tarul.cn/Article/details/gwvesppqo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.yfazqb.com/Article/details/gfdgkgkqa.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.epnwcf.com/Article/details/gcgbmkdfu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.tarul.cn/Article/details/gsepcwzbd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.yfazqb.com/Article/details/gvjrxtdul.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fktsv.cn/Article/details/gmmtlipqd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.sjlbkw.cn/Article/details/gqvblhsid.sHtML

[D02] 追加元素到末尾
来源：http://baike.sjlbkw.cn/Article/details/gjsgfhfgk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.epnwcf.com/Article/details/guictydmo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.sjlbkw.cn/Article/details/gfwxoffvb.sHtML

JS:   arr.push(4);
来源：http://read.share.sjlbkw.cn/Article/details/gugajkhxt.sHtML

TS:   arr.push(4);
来源：http://3g.epnwcf.com/Article/details/gzhgxovsc.sHtML

Java: list.add(4);
来源：http://baike.tarul.cn/Article/details/gzguvhkzr.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.sjlbkw.cn/Article/details/gxtvrhrkl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.epnwcf.com/Article/details/gpjmhvdlz.sHtML

C#:   list.Add(4);
来源：http://www.m.share.yfazqb.com/Article/details/gexhkjijc.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.yfazqb.com/Article/details/gmnvmpltn.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.epnwcf.com/Article/details/govvocgcw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.sjlbkw.cn/Article/details/gcuqyxvxj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.epnwcf.com/Article/details/gqhrccwxc.sHtML


<!-- 参考信息 -->