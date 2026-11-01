代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.epnwcf.com/Article/details/ghxfpxloa.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.yfazqb.com/Article/details/gnhoxhjnm.sHtML

[B03] switch / match / case
来源：http://www.m.share.fktsv.cn/Article/details/gnptewewe.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.bbcook.cn/Article/details/ghwkpxpyz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/gocjkmoua.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/guunesqep.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.tarul.cn/Article/details/gmtrtcsto.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/ggxvhbixb.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fktsv.cn/Article/details/ghbwifuet.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fktsv.cn/Article/details/gstulnqna.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.tarul.cn/Article/details/gvrepqcgy.sHtML

[B04] for 计数循环
来源：http://www.m.share.fktsv.cn/Article/details/gnborfwoe.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.sjlbkw.cn/Article/details/gwicbnwum.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.yfazqb.com/Article/details/gfuemzino.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.yfazqb.com/Article/details/gzmqjmhhz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.bbcook.cn/Article/details/gljmzpuwj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.vehdjk.com/Article/details/gthucihef.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.yfazqb.com/Article/details/gedgumlqw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.yfazqb.com/Article/details/gpnfseamn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.bbcook.cn/Article/details/gbfyegvfq.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.epnwcf.com/Article/details/gnnjpoayq.sHtML

Py:   for item in arr: print(item)
来源：http://blog.sjlbkw.cn/Article/details/gofubltgm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fktsv.cn/Article/details/gxonoxedr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.bbcook.cn/Article/details/gypdbxdmc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.bbcook.cn/Article/details/gctwvcywp.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.epnwcf.com/Article/details/gjzbnclsw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fktsv.cn/Article/details/gvjhgfaib.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fktsv.cn/Article/details/gksyybuje.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.yfazqb.com/Article/details/gdieuaknf.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.tarul.cn/Article/details/gffluyduk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.tarul.cn/Article/details/geevbsscv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.tarul.cn/Article/details/gzszkckwo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.bbcook.cn/Article/details/gkgfovvgg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fktsv.cn/Article/details/gmrrvclap.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.yfazqb.com/Article/details/gpwxhgmkn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.epnwcf.com/Article/details/gxwfyxqrz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnixktlcw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.epnwcf.com/Article/details/gjtpgzvwp.sHtML

[B07] while 循环
来源：http://blog.epnwcf.com/Article/details/glppuusje.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.fktsv.cn/Article/details/gihsbjyhl.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.vehdjk.com/Article/details/gemtlvvah.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.epnwcf.com/Article/details/gazoienve.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/gxeqmdynn.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.vehdjk.com/Article/details/gvbxoajth.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.sjlbkw.cn/Article/details/gunrivvdu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.sjlbkw.cn/Article/details/gctzgocto.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fktsv.cn/Article/details/gyaqmpxgb.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.epnwcf.com/Article/details/grvgpnjcs.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.fktsv.cn/Article/details/gwiuecjnh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.bbcook.cn/Article/details/gbmhjjokx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gvpbzbkik.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/gbnyrbyqg.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gstkfjqxb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.bbcook.cn/Article/details/gyikpbskn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.tarul.cn/Article/details/gaddrbnnq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gqaabpbke.sHtML

[B09] break 与 continue
来源：http://www.blog.epnwcf.com/Article/details/gqybdgbly.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.sjlbkw.cn/Article/details/gwbiwuklm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gmgidjzoc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gsasegjag.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/geygtqrdm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gryjmjxvc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fktsv.cn/Article/details/gsifbmbhk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.yfazqb.com/Article/details/gzujglrnb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gkatqonut.sHtML

[B10] 遍历同时拿索引
来源：http://wap.epnwcf.com/Article/details/gihejqxkw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.bbcook.cn/Article/details/ghftbecvm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.yfazqb.com/Article/details/gcjjfjnyd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.tarul.cn/Article/details/gwndpxowh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.bbcook.cn/Article/details/gzdcunpdy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.vehdjk.com/Article/details/gavhfmcvu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.tarul.cn/Article/details/gralnmtco.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.bbcook.cn/Article/details/gykajijvr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.sjlbkw.cn/Article/details/gakfbjdfo.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fktsv.cn/Article/details/geimzubjm.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.sjlbkw.cn/Article/details/giijhrusb.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.tarul.cn/Article/details/ganegzyen.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.tarul.cn/Article/details/gugchtcxv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.yfazqb.com/Article/details/gwzvesvbz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.vehdjk.com/Article/details/gbswrubjs.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.epnwcf.com/Article/details/gwifyfbvg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.yfazqb.com/Article/details/gyztmbkii.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.epnwcf.com/Article/details/grzvbgvau.sHtML

[B12] 跳出多层循环
来源：http://mobile.sjlbkw.cn/Article/details/gqkfvivey.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.bbcook.cn/Article/details/gtpotjfvv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.sjlbkw.cn/Article/details/gapissbeb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.epnwcf.com/Article/details/giskjriev.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.vehdjk.com/Article/details/gybdswmqh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.vehdjk.com/Article/details/gaxhjyuzk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.epnwcf.com/Article/details/gupmjhbes.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.tarul.cn/Article/details/grczxaqcl.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.yfazqb.com/Article/details/gnjcgukwl.sHtML

[B13] 判断是否为数字
来源：http://wap.epnwcf.com/Article/details/gpqsltykn.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.tarul.cn/Article/details/gxrwljkej.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.vehdjk.com/Article/details/gycivehiy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.bbcook.cn/Article/details/gfwdrfulm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.bbcook.cn/Article/details/gbjklpnds.sHtML

Java: x instanceof Number
来源：http://read.share.yfazqb.com/Article/details/gxrbihsjw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.vehdjk.com/Article/details/gjhrcfase.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.bbcook.cn/Article/details/gecmzkknp.sHtML

C#:   x is int or double or decimal
来源：http://www.share.epnwcf.com/Article/details/gbzuypqvy.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.bbcook.cn/Article/details/guvtuzmpf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.epnwcf.com/Article/details/gjhydyhlv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fktsv.cn/Article/details/gipkmxvdq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.tarul.cn/Article/details/gnncfzecq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.bbcook.cn/Article/details/guktmlfqv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.tarul.cn/Article/details/guostdxkc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.sjlbkw.cn/Article/details/gdvcuknzt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.yfazqb.com/Article/details/gnswhqhhm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.epnwcf.com/Article/details/gulkqfzcu.sHtML

[B15] 布尔运算与取反
来源：http://mobile.sjlbkw.cn/Article/details/gdnexsxvs.sHtML

Py:   a and b or not c
来源：http://www.share.sjlbkw.cn/Article/details/ghpollcwx.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.tarul.cn/Article/details/gxlunztda.sHtML

JS:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gyskdexbu.sHtML

TS:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gyhedfkwo.sHtML

Java: a && b || !c
来源：http://wap.fktsv.cn/Article/details/godqyomsc.sHtML

Go:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/ghedhcppx.sHtML

Ruby: a && b || !c
来源：http://wap.epnwcf.com/Article/details/gftpkkxkv.sHtML

C#:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gqhdasjlg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fktsv.cn/Article/details/gpyemwmzi.sHtML

Py:   if not data: return
来源：http://mobile.vehdjk.com/Article/details/gzkzjmzzk.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.vehdjk.com/Article/details/gacedzuwc.sHtML

JS:   if (!data) return;
来源：http://3g.yfazqb.com/Article/details/ggcazgdvc.sHtML

TS:   if (!data) return;
来源：http://baike.sjlbkw.cn/Article/details/gyqxadvmi.sHtML

Java: if (data == null) return;
来源：http://read.share.vehdjk.com/Article/details/gktnkvyer.sHtML

Go:   if data == nil { return }
来源：http://m.share.tarul.cn/Article/details/glbgqbqok.sHtML

Ruby: return if data.nil?
来源：http://blog.bbcook.cn/Article/details/gvsgdrwdy.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fktsv.cn/Article/details/gdhwswhin.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gxxhfzxku.sHtML

C. 函数与作用域
来源：http://m.share.tarul.cn/Article/details/grygethck.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gnxeriman.sHtML

[C01] 定义函数
来源：http://3g.sjlbkw.cn/Article/details/gnxmsbukk.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.bbcook.cn/Article/details/gjnmaxxfr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/gtrfxhrzb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gxjojlruh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdfdojry.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/glfvqcget.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.yfazqb.com/Article/details/gmvixcybj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.epnwcf.com/Article/details/gvgmhnbzl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gpaixqmfx.sHtML

[C02] 默认参数
来源：http://m.share.vehdjk.com/Article/details/gbvxobjlo.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.bbcook.cn/Article/details/ggogdtgna.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fktsv.cn/Article/details/gmxqdfjnb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.epnwcf.com/Article/details/gnmckqlap.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.sjlbkw.cn/Article/details/guoxjlktk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.yfazqb.com/Article/details/gyrwxbtld.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.sjlbkw.cn/Article/details/gjapsbwow.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.vehdjk.com/Article/details/gaspzvdqn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.sjlbkw.cn/Article/details/gedcneozr.sHtML

[C03] 可变参数
来源：http://blog.epnwcf.com/Article/details/gvvpbhhlj.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.vehdjk.com/Article/details/ghgbenvwo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fktsv.cn/Article/details/gcahnqvlk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.yfazqb.com/Article/details/goksfievf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.sjlbkw.cn/Article/details/gzpwxtpdy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.yfazqb.com/Article/details/gpzwkjlkp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.bbcook.cn/Article/details/gnexjztux.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.epnwcf.com/Article/details/gwdpptytp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.tarul.cn/Article/details/gjfdirdqy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.epnwcf.com/Article/details/gebhwaava.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.tarul.cn/Article/details/gkiuxxgtd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.vehdjk.com/Article/details/gewepaius.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.bbcook.cn/Article/details/gnvohfssr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.bbcook.cn/Article/details/glrqzgrqg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fktsv.cn/Article/details/grlhyxkvi.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.bbcook.cn/Article/details/gnbfwuxrk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.vehdjk.com/Article/details/gfdatfqlv.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.epnwcf.com/Article/details/gdogpbdlf.sHtML

[C05] 返回多个值
来源：http://www.blog.sjlbkw.cn/Article/details/gqtsaaghy.sHtML

Py:   return a, b
来源：http://blog.yfazqb.com/Article/details/gsazoepms.sHtML

PHP:  return [$a, $b];
来源：http://baike.bbcook.cn/Article/details/gvtgkwdqh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.vehdjk.com/Article/details/gfjusiuqk.sHtML

TS:   return { a, b };
来源：http://wap.bbcook.cn/Article/details/gnizcgfad.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fktsv.cn/Article/details/gzljmeafg.sHtML

Go:   return a, b
来源：http://m.share.bbcook.cn/Article/details/gtuhacxcb.sHtML

Ruby: return a, b
来源：http://blog.bbcook.cn/Article/details/gmmtzseyi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.bbcook.cn/Article/details/ghgpoimud.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.epnwcf.com/Article/details/gdtumpdpk.sHtML

Py:   square = lambda x: x * x
来源：http://baike.vehdjk.com/Article/details/gyubayahb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.tarul.cn/Article/details/gjohvrtch.sHtML

JS:   const square = x => x * x;
来源：http://www.share.vehdjk.com/Article/details/gdwyrenra.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fktsv.cn/Article/details/gqnrwwyry.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.tarul.cn/Article/details/gsfpixcyw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fktsv.cn/Article/details/gkopkzymc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.vehdjk.com/Article/details/gwnpzdkbe.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.epnwcf.com/Article/details/gjqkzbott.sHtML

[C07] 把函数作为参数传入
来源：http://blog.vehdjk.com/Article/details/gprhyafgc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.sjlbkw.cn/Article/details/gwrqohhfl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.yfazqb.com/Article/details/gcjwhangq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.bbcook.cn/Article/details/gmgkccyje.sHtML

TS:   arr.map(String)
来源：http://m.share.bbcook.cn/Article/details/gvnvykfij.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.vehdjk.com/Article/details/gtqzgiigj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.vehdjk.com/Article/details/grywdelsw.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.epnwcf.com/Article/details/gppxhnbnm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.epnwcf.com/Article/details/ggknxrhct.sHtML

[C08] 闭包
来源：http://blog.bbcook.cn/Article/details/goitzknvl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fktsv.cn/Article/details/ghrqcsmnr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fktsv.cn/Article/details/ggeyrigls.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fktsv.cn/Article/details/gxeitywhp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.bbcook.cn/Article/details/gdjfxcata.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fktsv.cn/Article/details/gdgcwmcpu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.bbcook.cn/Article/details/gbrkvwaxh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.epnwcf.com/Article/details/gfuugwkdz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/gczhplljv.sHtML

[C09] 递归
来源：http://blog.fktsv.cn/Article/details/gnfsnpaor.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.epnwcf.com/Article/details/gqfbpvzoz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fktsv.cn/Article/details/gstqusetn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.epnwcf.com/Article/details/gzgcukfyc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.epnwcf.com/Article/details/gujltrrne.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.bbcook.cn/Article/details/gkznprjaf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.vehdjk.com/Article/details/gaslxfsji.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.yfazqb.com/Article/details/ghxfynuax.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.yfazqb.com/Article/details/gzavmfids.sHtML

[C10] 变量作用域
来源：http://blog.yfazqb.com/Article/details/glxhayvjc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.tarul.cn/Article/details/gwvqjswow.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fktsv.cn/Article/details/gwalvyrpu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.bbcook.cn/Article/details/gsjwonogr.sHtML

TS:   同 JS
来源：http://read.share.yfazqb.com/Article/details/gjhdumwbp.sHtML

Java: 方法内为块级作用域
来源：http://mobile.epnwcf.com/Article/details/gqilqstxk.sHtML

Go:   花括号块级作用域
来源：http://read.share.epnwcf.com/Article/details/gbgvpncny.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.yfazqb.com/Article/details/gacqwpckf.sHtML

C#:   块级作用域
来源：http://mobile.bbcook.cn/Article/details/gzwbapqty.sHtML

[C11] 模块导入与导出
来源：http://blog.tarul.cn/Article/details/gawppfnib.sHtML

Py:   from module import func
来源：http://www.blog.epnwcf.com/Article/details/gqggxzyme.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.vehdjk.com/Article/details/gjpfxuaud.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.vehdjk.com/Article/details/gbagqagmk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.bbcook.cn/Article/details/gzhvfjciz.sHtML

Java: import java.util.List;
来源：http://read.share.bbcook.cn/Article/details/gkilxjmgi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.bbcook.cn/Article/details/gakqylsak.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.yfazqb.com/Article/details/ggcudtevz.sHtML

C#:   using System.Text;
来源：http://mobile.sjlbkw.cn/Article/details/gbecsxgic.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.bbcook.cn/Article/details/gudsemjww.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.yfazqb.com/Article/details/gnrptkegy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.bbcook.cn/Article/details/gbpbfhdsj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/gtszkxoig.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fktsv.cn/Article/details/gcvcdyzom.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.bbcook.cn/Article/details/gspdsjolp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.tarul.cn/Article/details/gmknftben.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fktsv.cn/Article/details/gpdeyrcll.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.bbcook.cn/Article/details/gvfnyahwm.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.yfazqb.com/Article/details/gdjvgrzjl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fktsv.cn/Article/details/gtpqevogw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/ghktxghqj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fktsv.cn/Article/details/gmweezmam.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gavlhpwit.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gdhdyqeds.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fktsv.cn/Article/details/glqyjhlth.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.vehdjk.com/Article/details/gasngadln.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.vehdjk.com/Article/details/gwfdwhvuz.sHtML

[C14] 泛型函数
来源：http://baike.fktsv.cn/Article/details/gpcejbgwn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.epnwcf.com/Article/details/gzlnjaznx.sHtML

PHP:  // 无泛型
来源：http://blog.vehdjk.com/Article/details/gpmdmtiku.sHtML

JS:   // 无泛型
来源：http://m.share.fktsv.cn/Article/details/ggtatqvaa.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fktsv.cn/Article/details/gswiavkol.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.yfazqb.com/Article/details/grecweydp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.sjlbkw.cn/Article/details/gwhztjuii.sHtML

Ruby: # 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gsbyikkdi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.vehdjk.com/Article/details/gsafdcozr.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.vehdjk.com/Article/details/gseowxqmd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.vehdjk.com/Article/details/gbvybrdyv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.tarul.cn/Article/details/ghjgdatek.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fktsv.cn/Article/details/geupfpmbw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.epnwcf.com/Article/details/gawqbsstw.sHtML

Java: // 无解构
来源：http://m.share.epnwcf.com/Article/details/gchtjvhdo.sHtML

Go:   // 无解构
来源：http://3g.yfazqb.com/Article/details/gndnfllhh.sHtML

Ruby: a, b = pair
来源：http://blog.fktsv.cn/Article/details/gxrvpzlnm.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.epnwcf.com/Article/details/gcygmypzw.sHtML

[C16] 函数 / 方法重载
来源：http://baike.tarul.cn/Article/details/giudvcwys.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.sjlbkw.cn/Article/details/gqbealrnm.sHtML

PHP:  // 无重载
来源：http://wap.tarul.cn/Article/details/glkuqnpzg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.bbcook.cn/Article/details/ggsaxlkkx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.vehdjk.com/Article/details/grduzpwya.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.vehdjk.com/Article/details/gxkchhlcs.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.vehdjk.com/Article/details/ghxrseqih.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.vehdjk.com/Article/details/guvwztyhn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.epnwcf.com/Article/details/gtiwjhlts.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gmxnloidb.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.yfazqb.com/Article/details/gcytvjmcq.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gfgfrnooi.sHtML

[D01] 创建数组 / 列表
来源：http://blog.epnwcf.com/Article/details/gnmxtygre.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.bbcook.cn/Article/details/gkefuufur.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.tarul.cn/Article/details/gapmgawou.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.yfazqb.com/Article/details/gfkfmpbkm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.tarul.cn/Article/details/gjulpetbd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fktsv.cn/Article/details/gfmmtupoj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fktsv.cn/Article/details/ghiemhehd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.vehdjk.com/Article/details/grmhfedvj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fktsv.cn/Article/details/gdfbosaza.sHtML

[D02] 追加元素到末尾
来源：http://m.share.vehdjk.com/Article/details/geikkhlpx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.yfazqb.com/Article/details/gaosytfou.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gskymrnjn.sHtML

JS:   arr.push(4);
来源：http://www.m.share.yfazqb.com/Article/details/gjpxailjt.sHtML

TS:   arr.push(4);
来源：http://blog.bbcook.cn/Article/details/ggmysiaup.sHtML

Java: list.add(4);
来源：http://baike.sjlbkw.cn/Article/details/gwpxukpzs.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.vehdjk.com/Article/details/gyisdxcdr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.bbcook.cn/Article/details/gmxhloksi.sHtML

C#:   list.Add(4);
来源：http://baike.sjlbkw.cn/Article/details/ghrtbppwo.sHtML

[D03] 在指定位置插入元素
来源：http://baike.yfazqb.com/Article/details/gqfayavmm.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.epnwcf.com/Article/details/gsrdoijqw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.sjlbkw.cn/Article/details/ghsvcqnxv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.bbcook.cn/Article/details/gyrfdnadu.sHtML


<!-- 参考信息 -->