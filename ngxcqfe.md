代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.vehdjk.com/Article/details/gxjctcsiy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/gqonxmudl.sHtML

[B03] switch / match / case
来源：http://read.share.bbcook.cn/Article/details/gsmafzlja.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.sjlbkw.cn/Article/details/gatysvzsn.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.yfazqb.com/Article/details/ghfvsasjh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.sjlbkw.cn/Article/details/gjxmapiyk.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fktsv.cn/Article/details/geisldhnr.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/glcjjysvw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.epnwcf.com/Article/details/gfbgcdaux.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.epnwcf.com/Article/details/gqwceaoxs.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.yfazqb.com/Article/details/grbglldqm.sHtML

[B04] for 计数循环
来源：http://m.share.yfazqb.com/Article/details/gwdghzxtl.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.yfazqb.com/Article/details/gwvutskqy.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.fktsv.cn/Article/details/gfsfqooxy.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fktsv.cn/Article/details/givykmulv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.bbcook.cn/Article/details/gvhqlrohf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.epnwcf.com/Article/details/ggldcqkec.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.bbcook.cn/Article/details/gmxiuvbtx.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.vehdjk.com/Article/details/gwljwujmo.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.vehdjk.com/Article/details/gbwqljpod.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.vehdjk.com/Article/details/gtrukeuea.sHtML

Py:   for item in arr: print(item)
来源：http://baike.yfazqb.com/Article/details/gbnvvurph.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.sjlbkw.cn/Article/details/gqzrzzhvg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.bbcook.cn/Article/details/gsydrgzsl.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fktsv.cn/Article/details/goskkejsr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.epnwcf.com/Article/details/gtlalvfqr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.vehdjk.com/Article/details/gimsfaowv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fktsv.cn/Article/details/gzyzyobfw.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fktsv.cn/Article/details/gatyjjtkg.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.yfazqb.com/Article/details/gxuhldboc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.bbcook.cn/Article/details/gkcutmxog.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.tarul.cn/Article/details/gpbwsuxgm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.tarul.cn/Article/details/gcnzolrqs.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.vehdjk.com/Article/details/gifctbcoh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.epnwcf.com/Article/details/gpfhfjmlt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.epnwcf.com/Article/details/gxafvchqd.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.sjlbkw.cn/Article/details/gdioogipf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fktsv.cn/Article/details/gqaoxirrh.sHtML

[B07] while 循环
来源：http://read.share.fktsv.cn/Article/details/giwzotqwy.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.tarul.cn/Article/details/gtajjewjx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.sjlbkw.cn/Article/details/giutcqiyd.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gdrqauorv.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gdpdqtdcc.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.sjlbkw.cn/Article/details/gznzmprop.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fktsv.cn/Article/details/gpurfudsl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.vehdjk.com/Article/details/giqisnzwm.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gbrffmfcd.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxmlgutj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.bbcook.cn/Article/details/gvhhegzrg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.bbcook.cn/Article/details/gxpbedjkq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gsgklegsz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gpetkzegl.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/ghjyhbhuw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxneunral.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.sjlbkw.cn/Article/details/gagmjqayf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/gzzllgprf.sHtML

[B09] break 与 continue
来源：http://www.m.share.tarul.cn/Article/details/gfofotsoe.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.tarul.cn/Article/details/gnxugckjm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtnjmlvrm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/ggzenxhfa.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/genksvyec.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gwrqzabbb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.vehdjk.com/Article/details/gmtscojor.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.sjlbkw.cn/Article/details/gqxxtvaaz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/gksaedxfn.sHtML

[B10] 遍历同时拿索引
来源：http://wap.yfazqb.com/Article/details/godgfawva.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fktsv.cn/Article/details/gwtsufsjx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.epnwcf.com/Article/details/gshgvqkyk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.yfazqb.com/Article/details/gbpbenycu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.yfazqb.com/Article/details/gzleudoqs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.sjlbkw.cn/Article/details/glropmrdi.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.tarul.cn/Article/details/gsumvofkx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.epnwcf.com/Article/details/gugtzgumu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fktsv.cn/Article/details/gcqbgdhcg.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.sjlbkw.cn/Article/details/gmuxwsnoe.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.tarul.cn/Article/details/gvrnxgnce.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.epnwcf.com/Article/details/gpxogsqdh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.epnwcf.com/Article/details/gsiftzsmj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.epnwcf.com/Article/details/gfwmgzoic.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.bbcook.cn/Article/details/geijkavpn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.yfazqb.com/Article/details/guekeedoj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.epnwcf.com/Article/details/gxoirhopl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.bbcook.cn/Article/details/gioairenc.sHtML

[B12] 跳出多层循环
来源：http://3g.fktsv.cn/Article/details/gpmvbaglh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.epnwcf.com/Article/details/gxcgkoeer.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.tarul.cn/Article/details/guvskjkzi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.yfazqb.com/Article/details/gbzsgbrfi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.yfazqb.com/Article/details/gswyvfszo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/gbhnqrqva.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.vehdjk.com/Article/details/gtaxxhmtd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.vehdjk.com/Article/details/gxvubrqqj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.vehdjk.com/Article/details/gnttznrwt.sHtML

[B13] 判断是否为数字
来源：http://baike.epnwcf.com/Article/details/gquhguvpj.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.vehdjk.com/Article/details/ghkhljamo.sHtML

PHP:  is_numeric($x)
来源：http://www.share.tarul.cn/Article/details/glydqbmfm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.vehdjk.com/Article/details/gbjrdclcp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fktsv.cn/Article/details/gsbosvejt.sHtML

Java: x instanceof Number
来源：http://read.share.yfazqb.com/Article/details/gvocgpqmh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fktsv.cn/Article/details/ghiobulrb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.vehdjk.com/Article/details/gkiqbnqjx.sHtML

C#:   x is int or double or decimal
来源：http://baike.sjlbkw.cn/Article/details/gzsgcetmf.sHtML

[B14] 判断值是否在集合内
来源：http://blog.yfazqb.com/Article/details/gtkxrmfth.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.sjlbkw.cn/Article/details/glszbyuqy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fktsv.cn/Article/details/gwlwzgcwx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.tarul.cn/Article/details/gwzsvnbgg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/ginaaooeb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.bbcook.cn/Article/details/gvwjmcnzm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.vehdjk.com/Article/details/gilyghejq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.yfazqb.com/Article/details/gajntaapa.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.epnwcf.com/Article/details/grtspjhgn.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhosybul.sHtML

Py:   a and b or not c
来源：http://read.share.bbcook.cn/Article/details/gubuuapoc.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.bbcook.cn/Article/details/groaacrau.sHtML

JS:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gdwrwdrxm.sHtML

TS:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gsxowqrcr.sHtML

Java: a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gfkilvapy.sHtML

Go:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gyjemmqtf.sHtML

Ruby: a && b || !c
来源：http://baike.fktsv.cn/Article/details/ggtexuxvv.sHtML

C#:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/ghpfqqoqt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.sjlbkw.cn/Article/details/gohqciapz.sHtML

Py:   if not data: return
来源：http://3g.yfazqb.com/Article/details/giezimftr.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.tarul.cn/Article/details/gvxblgugl.sHtML

JS:   if (!data) return;
来源：http://m.share.epnwcf.com/Article/details/gskcyhgpb.sHtML

TS:   if (!data) return;
来源：http://www.m.share.vehdjk.com/Article/details/ghymwbxsk.sHtML

Java: if (data == null) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrkkucej.sHtML

Go:   if data == nil { return }
来源：http://wap.epnwcf.com/Article/details/gbrxbxwwp.sHtML

Ruby: return if data.nil?
来源：http://blog.vehdjk.com/Article/details/gkyfwdyih.sHtML

C#:   if (data == null) return;
来源：http://mobile.epnwcf.com/Article/details/gnxebznsu.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gjcjmbqpn.sHtML

C. 函数与作用域
来源：http://m.share.fktsv.cn/Article/details/ghyvioiia.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gtbdqbhvh.sHtML

[C01] 定义函数
来源：http://m.share.fktsv.cn/Article/details/gwvymyuyb.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.bbcook.cn/Article/details/gbghrxfnl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gdhelynhi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gzbpccdkq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gegspqbmi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gzmqohvub.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.tarul.cn/Article/details/gybsykvxy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.yfazqb.com/Article/details/gskblcjry.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gvgndaxav.sHtML

[C02] 默认参数
来源：http://read.share.sjlbkw.cn/Article/details/gthpzzinh.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.sjlbkw.cn/Article/details/gewfpzcpp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.epnwcf.com/Article/details/gkqpoghjh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.tarul.cn/Article/details/gkwgzoslq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/ggbuqlsvq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fktsv.cn/Article/details/gujdfvrsc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.sjlbkw.cn/Article/details/grixoiugf.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.sjlbkw.cn/Article/details/gubgqhnve.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.bbcook.cn/Article/details/gxczthkdc.sHtML

[C03] 可变参数
来源：http://3g.vehdjk.com/Article/details/garmkmdqf.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.sjlbkw.cn/Article/details/gqhcuuwra.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fktsv.cn/Article/details/gwgmisige.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.yfazqb.com/Article/details/gxcirbtxw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.yfazqb.com/Article/details/gkwvcjauk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.tarul.cn/Article/details/ghzrrxobw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.vehdjk.com/Article/details/gimlqxbyh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.epnwcf.com/Article/details/gsdzuwzlt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.bbcook.cn/Article/details/gqatuxave.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.vehdjk.com/Article/details/ghpygoqdy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.sjlbkw.cn/Article/details/glnuruspk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.bbcook.cn/Article/details/gcgfghksz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.bbcook.cn/Article/details/gixjkhaeq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.vehdjk.com/Article/details/gghrefugu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.tarul.cn/Article/details/gtmahrzdq.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fktsv.cn/Article/details/gyksayokw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.epnwcf.com/Article/details/ghvnxfnmm.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fktsv.cn/Article/details/gaqydpgtj.sHtML

[C05] 返回多个值
来源：http://3g.bbcook.cn/Article/details/gbkzsgmev.sHtML

Py:   return a, b
来源：http://blog.epnwcf.com/Article/details/gmhkysiir.sHtML

PHP:  return [$a, $b];
来源：http://wap.vehdjk.com/Article/details/gxshxtgwl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.yfazqb.com/Article/details/gqiuojznm.sHtML

TS:   return { a, b };
来源：http://www.m.share.epnwcf.com/Article/details/gswooevux.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.bbcook.cn/Article/details/gwzshcwpb.sHtML

Go:   return a, b
来源：http://m.share.yfazqb.com/Article/details/ghkcyhhgi.sHtML

Ruby: return a, b
来源：http://www.blog.tarul.cn/Article/details/gaxmawwjv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.vehdjk.com/Article/details/gesjmdfvg.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fktsv.cn/Article/details/gjkpkuytn.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fktsv.cn/Article/details/gauvmlmep.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fktsv.cn/Article/details/gkqgwssty.sHtML

JS:   const square = x => x * x;
来源：http://www.share.vehdjk.com/Article/details/gyvglmuze.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gccqpfvtf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.yfazqb.com/Article/details/gmwshmqzs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.yfazqb.com/Article/details/gxklhiiyu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.vehdjk.com/Article/details/gxykvmkji.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gufahizbu.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbxoolxu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.sjlbkw.cn/Article/details/gbzyqwqga.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.vehdjk.com/Article/details/gtzflxvuf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.vehdjk.com/Article/details/gachtpxod.sHtML

TS:   arr.map(String)
来源：http://blog.epnwcf.com/Article/details/gqwcvxabg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.tarul.cn/Article/details/gplxphefb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.epnwcf.com/Article/details/goazdkpbr.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.yfazqb.com/Article/details/genvnfbzl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.epnwcf.com/Article/details/gjfqvcgrn.sHtML

[C08] 闭包
来源：http://mobile.vehdjk.com/Article/details/gvagifjzo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.sjlbkw.cn/Article/details/ggszoyxle.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.tarul.cn/Article/details/gzydbapwy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gfalronks.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gbabhtnat.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.epnwcf.com/Article/details/gnmbzuilg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.yfazqb.com/Article/details/gqalcpzco.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.bbcook.cn/Article/details/gbdvqedlm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fktsv.cn/Article/details/gfcnynbtt.sHtML

[C09] 递归
来源：http://mobile.sjlbkw.cn/Article/details/grqoagdpw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.bbcook.cn/Article/details/guvrdskuk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.yfazqb.com/Article/details/gioervbqe.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.tarul.cn/Article/details/gvydsllvs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.bbcook.cn/Article/details/gjambgsze.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.yfazqb.com/Article/details/gplnhxown.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.yfazqb.com/Article/details/glatwxfjx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.epnwcf.com/Article/details/gkurhpwjm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.yfazqb.com/Article/details/gaqugewrq.sHtML

[C10] 变量作用域
来源：http://m.share.yfazqb.com/Article/details/gyftacknx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.sjlbkw.cn/Article/details/gnwfftqqc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fktsv.cn/Article/details/gxehszwou.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fktsv.cn/Article/details/glilpsiic.sHtML

TS:   同 JS
来源：http://www.m.share.tarul.cn/Article/details/ghialquju.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.bbcook.cn/Article/details/gsdzmgjtr.sHtML

Go:   花括号块级作用域
来源：http://www.blog.vehdjk.com/Article/details/gygjettex.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fktsv.cn/Article/details/gatnopcfe.sHtML

C#:   块级作用域
来源：http://baike.vehdjk.com/Article/details/gzxyhcsyt.sHtML

[C11] 模块导入与导出
来源：http://baike.fktsv.cn/Article/details/gllovgkrz.sHtML

Py:   from module import func
来源：http://blog.fktsv.cn/Article/details/gcvoqyfhj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.vehdjk.com/Article/details/gcwdwbqyy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fktsv.cn/Article/details/gfjgnlvlr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.epnwcf.com/Article/details/gvygoxivp.sHtML

Java: import java.util.List;
来源：http://3g.tarul.cn/Article/details/gsjivcoto.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.epnwcf.com/Article/details/gsemhqepp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fktsv.cn/Article/details/gmhhxcyug.sHtML

C#:   using System.Text;
来源：http://read.share.epnwcf.com/Article/details/gftmmwxlw.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.vehdjk.com/Article/details/ghdxzjcwx.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.yfazqb.com/Article/details/gshqsevpp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.bbcook.cn/Article/details/ghovhyxoy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.tarul.cn/Article/details/gbdhqvuvd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.epnwcf.com/Article/details/gzyxeequj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.epnwcf.com/Article/details/gvwfkgfiu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.vehdjk.com/Article/details/gmlbfjreb.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.sjlbkw.cn/Article/details/gbigfeuzm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.tarul.cn/Article/details/gzjkosoyn.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.vehdjk.com/Article/details/gsbeixbeu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.vehdjk.com/Article/details/gpzuboyqg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gdvblrpfa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.yfazqb.com/Article/details/gqrfskamw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gegivoyfh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gvxnoqmwy.sHtML

Go:   func add(a, b int) int
来源：http://baike.tarul.cn/Article/details/gundocqgt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.tarul.cn/Article/details/ghbeqjmas.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.vehdjk.com/Article/details/gjojrwxjt.sHtML

[C14] 泛型函数
来源：http://mobile.tarul.cn/Article/details/goxiuvjnp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.bbcook.cn/Article/details/gkgfkljmi.sHtML

PHP:  // 无泛型
来源：http://www.m.share.bbcook.cn/Article/details/gtpxabndl.sHtML

JS:   // 无泛型
来源：http://blog.yfazqb.com/Article/details/gqjfkguzv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.vehdjk.com/Article/details/gapuuinua.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fktsv.cn/Article/details/gjssfasad.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fktsv.cn/Article/details/gdbsrkyrm.sHtML

Ruby: # 无泛型
来源：http://baike.fktsv.cn/Article/details/gouemyvav.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.sjlbkw.cn/Article/details/gatgqcbis.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.epnwcf.com/Article/details/gbevjlhqs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.yfazqb.com/Article/details/geacciyrc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fktsv.cn/Article/details/gjbkrjisq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.tarul.cn/Article/details/gipepurya.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.bbcook.cn/Article/details/gsunqazsg.sHtML

Java: // 无解构
来源：http://www.share.fktsv.cn/Article/details/gmnsvdbzo.sHtML

Go:   // 无解构
来源：http://blog.epnwcf.com/Article/details/gqlvnuczy.sHtML

Ruby: a, b = pair
来源：http://www.blog.tarul.cn/Article/details/gupavyusx.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fktsv.cn/Article/details/gunrnnzit.sHtML

[C16] 函数 / 方法重载
来源：http://baike.bbcook.cn/Article/details/gwphuavpe.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fktsv.cn/Article/details/gvodoxpsj.sHtML

PHP:  // 无重载
来源：http://m.share.fktsv.cn/Article/details/gdreijweg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.epnwcf.com/Article/details/gsrlyaymj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.yfazqb.com/Article/details/gssnxzzbj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.tarul.cn/Article/details/gfdadcunv.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.yfazqb.com/Article/details/gyezxxbke.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.sjlbkw.cn/Article/details/gcafecsuq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fktsv.cn/Article/details/gyjtwmmuz.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/ggudcgnej.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.bbcook.cn/Article/details/gazinizuk.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gryefudue.sHtML

[D01] 创建数组 / 列表
来源：http://3g.tarul.cn/Article/details/gpfhrksec.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.vehdjk.com/Article/details/gcgzbipyk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.vehdjk.com/Article/details/gnhsfnucz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.yfazqb.com/Article/details/gdmcvkxkp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.vehdjk.com/Article/details/gxuuwcscv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.vehdjk.com/Article/details/gskncgdoz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.epnwcf.com/Article/details/gbjlkewnz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.vehdjk.com/Article/details/gzssvipjz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fktsv.cn/Article/details/gyusshupl.sHtML

[D02] 追加元素到末尾
来源：http://3g.sjlbkw.cn/Article/details/gbkkszkqa.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.bbcook.cn/Article/details/gwwjfpxfp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.sjlbkw.cn/Article/details/gxkltxsbi.sHtML

JS:   arr.push(4);
来源：http://www.share.epnwcf.com/Article/details/ggxgafxrw.sHtML

TS:   arr.push(4);
来源：http://blog.bbcook.cn/Article/details/gsgldbpcu.sHtML

Java: list.add(4);
来源：http://m.share.yfazqb.com/Article/details/gylpqvzva.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.yfazqb.com/Article/details/gtjgcxwft.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.epnwcf.com/Article/details/gcnxidzuj.sHtML

C#:   list.Add(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqajioccb.sHtML

[D03] 在指定位置插入元素
来源：http://wap.bbcook.cn/Article/details/gcvzzlete.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.yfazqb.com/Article/details/gpcmohdmx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fktsv.cn/Article/details/gxpxiftbl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.vehdjk.com/Article/details/gncizbzeh.sHtML


<!-- 参考信息 -->