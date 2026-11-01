代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.sjlbkw.cn/Article/details/gieviemdv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.vehdjk.com/Article/details/gpwthfpzs.sHtML

[B03] switch / match / case
来源：http://www.m.share.vehdjk.com/Article/details/getarwecm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.yfazqb.com/Article/details/gsalwyaqe.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gpngagaei.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.yfazqb.com/Article/details/gnyppkysv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.yfazqb.com/Article/details/gvuwpzhhm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.bbcook.cn/Article/details/gojlnfxkv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.yfazqb.com/Article/details/gggruelcf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.tarul.cn/Article/details/gjnidfrrf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.yfazqb.com/Article/details/gfdsdvktb.sHtML

[B04] for 计数循环
来源：http://mobile.yfazqb.com/Article/details/gybwhdfxn.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fktsv.cn/Article/details/grlgcdlna.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.vehdjk.com/Article/details/gsbdvwuik.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.yfazqb.com/Article/details/gaaosooxu.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.sjlbkw.cn/Article/details/gxhtjdsyc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.vehdjk.com/Article/details/gfrlmzybe.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.epnwcf.com/Article/details/grktvjppc.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.sjlbkw.cn/Article/details/gcekjqygv.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.yfazqb.com/Article/details/gvolyjqow.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.sjlbkw.cn/Article/details/gwcfdwkcb.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.yfazqb.com/Article/details/gpfcubefs.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fktsv.cn/Article/details/gnfnltwvc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.tarul.cn/Article/details/gkvyrvrfm.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.sjlbkw.cn/Article/details/gouioznfl.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.vehdjk.com/Article/details/gwhlrfcks.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.epnwcf.com/Article/details/genzlvrvk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.tarul.cn/Article/details/gffbmrbuv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.tarul.cn/Article/details/glmvwdvfj.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.bbcook.cn/Article/details/gnyyodfdm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.sjlbkw.cn/Article/details/gabdcrnty.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.yfazqb.com/Article/details/gyakhykep.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fktsv.cn/Article/details/gvwrxiawq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.tarul.cn/Article/details/gmpuxzknu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.bbcook.cn/Article/details/gvyzbovnq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.sjlbkw.cn/Article/details/ghqiephiu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fktsv.cn/Article/details/gvovclgrm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyyjmzsiz.sHtML

[B07] while 循环
来源：http://m.share.fktsv.cn/Article/details/gjiyksyxb.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fktsv.cn/Article/details/gduomdvfu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fktsv.cn/Article/details/gusnbaqsj.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gwwdqbyct.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.bbcook.cn/Article/details/gzxsjtzpc.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.yfazqb.com/Article/details/gcirmtbiy.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.vehdjk.com/Article/details/gtnssnwyb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.bbcook.cn/Article/details/glmsopeal.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.epnwcf.com/Article/details/gekadqyos.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.bbcook.cn/Article/details/gzcemujqt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.bbcook.cn/Article/details/gteecmqli.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.bbcook.cn/Article/details/gjlsyreeu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/ggtcgmbox.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/gpuopcmkw.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gkeacgllc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.tarul.cn/Article/details/gmymmqytz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.bbcook.cn/Article/details/gcknrzbxo.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/govqzobdd.sHtML

[B09] break 与 continue
来源：http://www.m.share.bbcook.cn/Article/details/gzimfrnqk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.tarul.cn/Article/details/gdmagmwcp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/gnqcrsyjr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/gugdlxkbp.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gqldhatmh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gizowxlre.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.bbcook.cn/Article/details/glflyztjg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fktsv.cn/Article/details/gbwzmdxyi.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/glefnspek.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fktsv.cn/Article/details/gnclvjpfj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkgsgzxcc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fktsv.cn/Article/details/goprjzvzj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.bbcook.cn/Article/details/giovamqbr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.sjlbkw.cn/Article/details/gvklylbug.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.bbcook.cn/Article/details/gnstelbfq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.vehdjk.com/Article/details/gfookrgeu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.vehdjk.com/Article/details/gytlbqpaj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.yfazqb.com/Article/details/gwpftjsgr.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.tarul.cn/Article/details/gerwabtid.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.epnwcf.com/Article/details/gykpkljga.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fktsv.cn/Article/details/gbmnntikq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.sjlbkw.cn/Article/details/gqgdvhrzl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.vehdjk.com/Article/details/gzzbzxllq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.tarul.cn/Article/details/gretpjkid.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.epnwcf.com/Article/details/gpzvnqjgp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.tarul.cn/Article/details/gytjdqbjo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.yfazqb.com/Article/details/gqjgoqens.sHtML

[B12] 跳出多层循环
来源：http://www.blog.tarul.cn/Article/details/grisrqoow.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.bbcook.cn/Article/details/gnspeavxr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fktsv.cn/Article/details/gtimyoypu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fktsv.cn/Article/details/gsgliexfp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.yfazqb.com/Article/details/gpygcircv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/gbypdrnze.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.yfazqb.com/Article/details/guroczujx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.epnwcf.com/Article/details/gvlarkfpw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.sjlbkw.cn/Article/details/gpmgkazxx.sHtML

[B13] 判断是否为数字
来源：http://mobile.fktsv.cn/Article/details/gzaxepxli.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.tarul.cn/Article/details/gwhniekmp.sHtML

PHP:  is_numeric($x)
来源：http://read.share.yfazqb.com/Article/details/gmvmfdccy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fktsv.cn/Article/details/gnubekiai.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.yfazqb.com/Article/details/gbzxrctxb.sHtML

Java: x instanceof Number
来源：http://baike.tarul.cn/Article/details/gttdupkmn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.tarul.cn/Article/details/gmkxcmoej.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.vehdjk.com/Article/details/ggxziljbw.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fktsv.cn/Article/details/gvofkdojm.sHtML

[B14] 判断值是否在集合内
来源：http://blog.epnwcf.com/Article/details/gkbcoucmc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.sjlbkw.cn/Article/details/gfyraolda.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.sjlbkw.cn/Article/details/gmsqvgvrn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.yfazqb.com/Article/details/gfinxnjnt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.tarul.cn/Article/details/ghhnkrmhj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.vehdjk.com/Article/details/gwvbszpsq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fktsv.cn/Article/details/gcknbdeuq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.yfazqb.com/Article/details/gmpstqkjl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/gkgnriwit.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdovvnqm.sHtML

Py:   a and b or not c
来源：http://baike.vehdjk.com/Article/details/gjiyqltje.sHtML

PHP:  $a && $b || !$c
来源：http://blog.epnwcf.com/Article/details/gebqddgzx.sHtML

JS:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gtnpkxayh.sHtML

TS:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gutfmugvo.sHtML

Java: a && b || !c
来源：http://blog.yfazqb.com/Article/details/gxcsiirut.sHtML

Go:   a && b || !c
来源：http://blog.tarul.cn/Article/details/gmvmrndfk.sHtML

Ruby: a && b || !c
来源：http://baike.epnwcf.com/Article/details/gnlcyyhva.sHtML

C#:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/gffjzowfl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.yfazqb.com/Article/details/gkyfcvdwp.sHtML

Py:   if not data: return
来源：http://www.m.share.tarul.cn/Article/details/gjkchurlf.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.yfazqb.com/Article/details/grkctxtaq.sHtML

JS:   if (!data) return;
来源：http://read.share.yfazqb.com/Article/details/gkzkhddra.sHtML

TS:   if (!data) return;
来源：http://mobile.vehdjk.com/Article/details/gpynvabkc.sHtML

Java: if (data == null) return;
来源：http://baike.bbcook.cn/Article/details/gjstyljvp.sHtML

Go:   if data == nil { return }
来源：http://baike.yfazqb.com/Article/details/geqvmlxxk.sHtML

Ruby: return if data.nil?
来源：http://read.share.bbcook.cn/Article/details/glhmzrhya.sHtML

C#:   if (data == null) return;
来源：http://m.share.yfazqb.com/Article/details/gyeqbzgfe.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gdnzhgeom.sHtML

C. 函数与作用域
来源：http://wap.epnwcf.com/Article/details/gdaazfpzf.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/grgqrggek.sHtML

[C01] 定义函数
来源：http://3g.sjlbkw.cn/Article/details/gcwwsuhdh.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.epnwcf.com/Article/details/gaqhfylrd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/gdxhphoxa.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gldkdhfgb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gxnldflsx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/grtgcifnj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.yfazqb.com/Article/details/gxektdwbb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.yfazqb.com/Article/details/gtrfapnya.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gcejinmny.sHtML

[C02] 默认参数
来源：http://m.share.fktsv.cn/Article/details/gmkavbfec.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fktsv.cn/Article/details/gfdbrltcj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.yfazqb.com/Article/details/gjxstaium.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.tarul.cn/Article/details/gssiyhkzs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gnggnvkon.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.yfazqb.com/Article/details/gtzxgjhsc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.vehdjk.com/Article/details/gdeyfnzch.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.bbcook.cn/Article/details/gfgcmufsf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fktsv.cn/Article/details/ggoobdvoo.sHtML

[C03] 可变参数
来源：http://blog.bbcook.cn/Article/details/gzngaptqf.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fktsv.cn/Article/details/gdmielazf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.tarul.cn/Article/details/gkkfxuknw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.vehdjk.com/Article/details/gjgadaxms.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.epnwcf.com/Article/details/gkcesrsgx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.vehdjk.com/Article/details/gsemfbevw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fktsv.cn/Article/details/gdhaqhedz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.bbcook.cn/Article/details/gtsxeycqc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.epnwcf.com/Article/details/gnjmduhyl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fktsv.cn/Article/details/glksjutxe.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.tarul.cn/Article/details/gzgkvgool.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.vehdjk.com/Article/details/gktcrmfcy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fktsv.cn/Article/details/gixlbfgip.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.epnwcf.com/Article/details/gmewzwyiw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.epnwcf.com/Article/details/ggwkpwsat.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.sjlbkw.cn/Article/details/gmamrrtuk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fktsv.cn/Article/details/gyexgetsi.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.sjlbkw.cn/Article/details/gmhbagcqj.sHtML

[C05] 返回多个值
来源：http://baike.tarul.cn/Article/details/gagmzlmdo.sHtML

Py:   return a, b
来源：http://www.share.bbcook.cn/Article/details/gdjrsiyat.sHtML

PHP:  return [$a, $b];
来源：http://mobile.tarul.cn/Article/details/gwtbtptgd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.bbcook.cn/Article/details/grfeesytq.sHtML

TS:   return { a, b };
来源：http://www.share.bbcook.cn/Article/details/gzyitcncg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.sjlbkw.cn/Article/details/gubmpvyxm.sHtML

Go:   return a, b
来源：http://mobile.tarul.cn/Article/details/giwfbiqua.sHtML

Ruby: return a, b
来源：http://3g.epnwcf.com/Article/details/girulknpq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.bbcook.cn/Article/details/gcxendizh.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.yfazqb.com/Article/details/gbgoqawba.sHtML

Py:   square = lambda x: x * x
来源：http://3g.epnwcf.com/Article/details/gqheugkzu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.epnwcf.com/Article/details/golnvyjyt.sHtML

JS:   const square = x => x * x;
来源：http://mobile.epnwcf.com/Article/details/goyagrqyp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.yfazqb.com/Article/details/gcjqmpxwh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.bbcook.cn/Article/details/gtgmdlycd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.epnwcf.com/Article/details/goontxyqg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.epnwcf.com/Article/details/gleinijha.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gogeczsvu.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.yfazqb.com/Article/details/gnagquabb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.vehdjk.com/Article/details/gcicyztmr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.bbcook.cn/Article/details/gjjaczuqh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fktsv.cn/Article/details/gmlxppikh.sHtML

TS:   arr.map(String)
来源：http://mobile.fktsv.cn/Article/details/gwfpswqbz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.tarul.cn/Article/details/gwayruxar.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.epnwcf.com/Article/details/gqjjucuyp.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.bbcook.cn/Article/details/gdelrmbfu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.bbcook.cn/Article/details/gqpjpwtxk.sHtML

[C08] 闭包
来源：http://www.share.fktsv.cn/Article/details/gssvlmqqv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.sjlbkw.cn/Article/details/grypfcgji.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fktsv.cn/Article/details/gxjggkhti.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.sjlbkw.cn/Article/details/guckzshsr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.epnwcf.com/Article/details/gfmfreqdc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.bbcook.cn/Article/details/gejuqkged.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.bbcook.cn/Article/details/gaqdpsbcv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.bbcook.cn/Article/details/gmtlhzyxc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/gsyvroasj.sHtML

[C09] 递归
来源：http://blog.fktsv.cn/Article/details/gwtlojugr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/gctmbvkfk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.epnwcf.com/Article/details/gllwzjhyg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fktsv.cn/Article/details/givhfxfak.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.bbcook.cn/Article/details/gimkguzol.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.yfazqb.com/Article/details/gmyoyuzqg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.vehdjk.com/Article/details/gijmombdw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fktsv.cn/Article/details/gzgfbzqak.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fktsv.cn/Article/details/gceqlabuy.sHtML

[C10] 变量作用域
来源：http://3g.fktsv.cn/Article/details/gofxugkhl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fktsv.cn/Article/details/gcbbffrut.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.sjlbkw.cn/Article/details/gbthsxubr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gmtmjvouf.sHtML

TS:   同 JS
来源：http://3g.tarul.cn/Article/details/gqdrglxex.sHtML

Java: 方法内为块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/gexwpetah.sHtML

Go:   花括号块级作用域
来源：http://wap.tarul.cn/Article/details/gctlildfx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.epnwcf.com/Article/details/goxdyyiyn.sHtML

C#:   块级作用域
来源：http://mobile.fktsv.cn/Article/details/gzswnejse.sHtML

[C11] 模块导入与导出
来源：http://mobile.vehdjk.com/Article/details/gkwjftgua.sHtML

Py:   from module import func
来源：http://www.m.share.tarul.cn/Article/details/gzfkgmcrx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.vehdjk.com/Article/details/gwfufnveg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.vehdjk.com/Article/details/gyvaliecl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.bbcook.cn/Article/details/gzdjahwyw.sHtML

Java: import java.util.List;
来源：http://mobile.bbcook.cn/Article/details/ggywndmhx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.epnwcf.com/Article/details/gtvpzlihz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.yfazqb.com/Article/details/gdatlvmbx.sHtML

C#:   using System.Text;
来源：http://3g.tarul.cn/Article/details/gvjjkqemh.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.tarul.cn/Article/details/gndemaoal.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.vehdjk.com/Article/details/guexuyjlp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.sjlbkw.cn/Article/details/gkaobrcvr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/gxkddeezl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fktsv.cn/Article/details/glxhbsyzx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.vehdjk.com/Article/details/grwtbjgek.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.vehdjk.com/Article/details/ghpvayatl.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.vehdjk.com/Article/details/gbrmhgkkg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.tarul.cn/Article/details/gaoifqmcd.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.bbcook.cn/Article/details/gklrcfgkw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.epnwcf.com/Article/details/gavzibavi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/gqjzuwwmr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.sjlbkw.cn/Article/details/glxwgwphx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gsrcztujz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gntcpfdis.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fktsv.cn/Article/details/gobouygqo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.vehdjk.com/Article/details/glotlksif.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.tarul.cn/Article/details/ghxbuzfmn.sHtML

[C14] 泛型函数
来源：http://blog.epnwcf.com/Article/details/gbihdzzgn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fktsv.cn/Article/details/gngzbyocg.sHtML

PHP:  // 无泛型
来源：http://baike.bbcook.cn/Article/details/gfeqpvuuw.sHtML

JS:   // 无泛型
来源：http://read.share.epnwcf.com/Article/details/ghchsvuvg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.tarul.cn/Article/details/geqicxryj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.bbcook.cn/Article/details/gmpjkqaue.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fktsv.cn/Article/details/gnrcsahjj.sHtML

Ruby: # 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/gdpzxglds.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.tarul.cn/Article/details/gvmzjfibp.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fktsv.cn/Article/details/ghhapppbi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.yfazqb.com/Article/details/gjxplwxyb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.vehdjk.com/Article/details/gsmwxlqpc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.tarul.cn/Article/details/gycelkxgc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqdqyoiz.sHtML

Java: // 无解构
来源：http://m.share.tarul.cn/Article/details/gpqlpelky.sHtML

Go:   // 无解构
来源：http://read.share.tarul.cn/Article/details/gcnfurbwx.sHtML

Ruby: a, b = pair
来源：http://read.share.tarul.cn/Article/details/gpcbmagud.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fktsv.cn/Article/details/gpiplnrws.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fktsv.cn/Article/details/gsopugdlg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.tarul.cn/Article/details/grqvcunpn.sHtML

PHP:  // 无重载
来源：http://read.share.fktsv.cn/Article/details/govhxieyw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.tarul.cn/Article/details/gnzbmjbzz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.yfazqb.com/Article/details/gnsepukrp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.tarul.cn/Article/details/gumpiwwka.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.tarul.cn/Article/details/gitocvukz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.epnwcf.com/Article/details/gtykmawrj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.tarul.cn/Article/details/gzuafwjin.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gwcwstkuz.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.tarul.cn/Article/details/gtijqwppy.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gkxzdzveg.sHtML

[D01] 创建数组 / 列表
来源：http://wap.yfazqb.com/Article/details/gzukisvbf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.bbcook.cn/Article/details/gtoyylgkp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.epnwcf.com/Article/details/gebnkeggc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.epnwcf.com/Article/details/guieldpcz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.sjlbkw.cn/Article/details/gktdsaxmh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.epnwcf.com/Article/details/gqvadgaus.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.tarul.cn/Article/details/gybjcmabd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.sjlbkw.cn/Article/details/gtowxsnas.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.tarul.cn/Article/details/gonmkphqs.sHtML

[D02] 追加元素到末尾
来源：http://mobile.bbcook.cn/Article/details/gapaegjkh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.vehdjk.com/Article/details/gnnvfqcgb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.sjlbkw.cn/Article/details/gpjtibbyg.sHtML

JS:   arr.push(4);
来源：http://www.share.vehdjk.com/Article/details/grmcnsjyz.sHtML

TS:   arr.push(4);
来源：http://blog.fktsv.cn/Article/details/godlcixss.sHtML

Java: list.add(4);
来源：http://blog.yfazqb.com/Article/details/gyrsffqaa.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.bbcook.cn/Article/details/gezwlatxs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.tarul.cn/Article/details/gfssptmvj.sHtML

C#:   list.Add(4);
来源：http://read.share.sjlbkw.cn/Article/details/gllzqjdto.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gaujkfiur.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.bbcook.cn/Article/details/gomjsgsmq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.tarul.cn/Article/details/gukofcnfe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fktsv.cn/Article/details/ggldfpekg.sHtML


<!-- 参考信息 -->