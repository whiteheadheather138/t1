代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://3g.sjlbkw.cn/Article/details/gvbptggno.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/gotyfdyiv.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/gptaqqtpu.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/gllmttdpw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.sjlbkw.cn/Article/details/gxfrwukgt.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.fktsv.cn/Article/details/gukggftop.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/gahbemfas.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.tarul.cn/Article/details/ggsmjbubg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.epnwcf.com/Article/details/gykcosboz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fktsv.cn/Article/details/gvugtlsbn.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/gyexjvmsc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gxslguymx.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/gyqnjqbzk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.sjlbkw.cn/Article/details/gaahuoktq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.epnwcf.com/Article/details/gspdpvlir.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gsmzohhhp.sHtML

[B09] break 与 continue
来源：http://m.share.sjlbkw.cn/Article/details/gcewtigpw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.sjlbkw.cn/Article/details/gciczfhzy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/glopqpjju.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gdfwdjoef.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/ggpssieke.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gdotsvebl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.yfazqb.com/Article/details/goqdlaruc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.vehdjk.com/Article/details/gsqsiqdgz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gbesnrkrg.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.epnwcf.com/Article/details/gayrikcgm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.vehdjk.com/Article/details/ghycxruuj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.vehdjk.com/Article/details/gidndgspm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fktsv.cn/Article/details/gjtpntfvd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.vehdjk.com/Article/details/gbbhucina.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.tarul.cn/Article/details/gjvnqkfpo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.vehdjk.com/Article/details/gzpnntmwz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.bbcook.cn/Article/details/gmgoowsbu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fktsv.cn/Article/details/glycaifry.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.sjlbkw.cn/Article/details/grwkkakus.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.sjlbkw.cn/Article/details/grwjtcbup.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.epnwcf.com/Article/details/gwcxhnqay.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.bbcook.cn/Article/details/gdlmoxcdf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.sjlbkw.cn/Article/details/gibegnfxi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.bbcook.cn/Article/details/genojoffl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.vehdjk.com/Article/details/ghwieebxq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.tarul.cn/Article/details/gmfeiwfig.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.vehdjk.com/Article/details/gzilfnzvx.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.bbcook.cn/Article/details/gvowgyxdf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fktsv.cn/Article/details/grkkrcyam.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.epnwcf.com/Article/details/grqtxudtc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.sjlbkw.cn/Article/details/gvacyrync.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/gpucivkzy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.vehdjk.com/Article/details/gjhdywexr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.tarul.cn/Article/details/gucqxtorg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.epnwcf.com/Article/details/gfoiozmoi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.yfazqb.com/Article/details/gtoyamprz.sHtML

[B13] 判断是否为数字
来源：http://3g.yfazqb.com/Article/details/gxacaqosz.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.sjlbkw.cn/Article/details/gdbmbpkdh.sHtML

PHP:  is_numeric($x)
来源：http://wap.vehdjk.com/Article/details/gadxfyswm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.bbcook.cn/Article/details/goevvdckq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.yfazqb.com/Article/details/ghvlwmhyw.sHtML

Java: x instanceof Number
来源：http://3g.bbcook.cn/Article/details/gyfwmxbxa.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fktsv.cn/Article/details/gvznnfgur.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.vehdjk.com/Article/details/ggcazspyg.sHtML

C#:   x is int or double or decimal
来源：http://blog.epnwcf.com/Article/details/gxzcdnsje.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.epnwcf.com/Article/details/gdqumnkbr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.epnwcf.com/Article/details/gqaskquli.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.vehdjk.com/Article/details/gorvbwcbg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.vehdjk.com/Article/details/grsunbvae.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.yfazqb.com/Article/details/gqzomclkj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.bbcook.cn/Article/details/ggivemali.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.vehdjk.com/Article/details/gedcvizwz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.sjlbkw.cn/Article/details/gtydflokc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/ganvlzngo.sHtML

[B15] 布尔运算与取反
来源：http://3g.tarul.cn/Article/details/gzgkauylx.sHtML

Py:   a and b or not c
来源：http://www.blog.epnwcf.com/Article/details/goykzaejz.sHtML

PHP:  $a && $b || !$c
来源：http://3g.bbcook.cn/Article/details/gnaotuiet.sHtML

JS:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gfzyomdcl.sHtML

TS:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gfsdrpwmv.sHtML

Java: a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcjymuxl.sHtML

Go:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gpapdkuwj.sHtML

Ruby: a && b || !c
来源：http://blog.tarul.cn/Article/details/gkizcoxmc.sHtML

C#:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gxwkkztyq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fktsv.cn/Article/details/gcohkckos.sHtML

Py:   if not data: return
来源：http://read.share.epnwcf.com/Article/details/gmsqdieic.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.yfazqb.com/Article/details/ggdtpuxuv.sHtML

JS:   if (!data) return;
来源：http://www.share.tarul.cn/Article/details/gwcihdcjk.sHtML

TS:   if (!data) return;
来源：http://baike.vehdjk.com/Article/details/grkbfpcpe.sHtML

Java: if (data == null) return;
来源：http://blog.bbcook.cn/Article/details/gqllethdv.sHtML

Go:   if data == nil { return }
来源：http://wap.sjlbkw.cn/Article/details/ghuwonekp.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fktsv.cn/Article/details/gecliufwd.sHtML

C#:   if (data == null) return;
来源：http://blog.epnwcf.com/Article/details/grmabxjhv.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gsdbznwbn.sHtML

C. 函数与作用域
来源：http://wap.tarul.cn/Article/details/gskszweap.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gdvxlstpl.sHtML

[C01] 定义函数
来源：http://m.share.bbcook.cn/Article/details/gyseqeygu.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fktsv.cn/Article/details/gfsbvurgc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/ghnrordep.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gphqqhzgu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/glfarmqdd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gjuwplanp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.sjlbkw.cn/Article/details/gkwzwokbk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fktsv.cn/Article/details/govjjmusf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gpjuaptfi.sHtML

[C02] 默认参数
来源：http://3g.sjlbkw.cn/Article/details/gmxuduanr.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.vehdjk.com/Article/details/gctftwckj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.bbcook.cn/Article/details/gmtxeyvbq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fktsv.cn/Article/details/gkqbjwnja.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.yfazqb.com/Article/details/gojblzeoa.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.vehdjk.com/Article/details/gsulumfnn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.sjlbkw.cn/Article/details/gkjuhwrud.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.yfazqb.com/Article/details/gzheukfxb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.tarul.cn/Article/details/gidwkzsuh.sHtML

[C03] 可变参数
来源：http://mobile.yfazqb.com/Article/details/guzodpjwe.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fktsv.cn/Article/details/galwydrsd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.tarul.cn/Article/details/gyubnzaij.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fktsv.cn/Article/details/gfzvmbrnn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.epnwcf.com/Article/details/glrdpegdt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fktsv.cn/Article/details/gfceqwtpz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.vehdjk.com/Article/details/gxsdkjcas.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.bbcook.cn/Article/details/gmyynbqbl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.vehdjk.com/Article/details/gjfzptcaf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.vehdjk.com/Article/details/gukrohhnb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.vehdjk.com/Article/details/gmzqljvuf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fktsv.cn/Article/details/gtssoahpe.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.epnwcf.com/Article/details/gnkfsruvs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.epnwcf.com/Article/details/gsohmeapk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.epnwcf.com/Article/details/gjevafmtd.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.epnwcf.com/Article/details/guecvzrec.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.sjlbkw.cn/Article/details/gxyhnfnji.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gnnkveqcm.sHtML

[C05] 返回多个值
来源：http://www.blog.sjlbkw.cn/Article/details/gfmtmoctf.sHtML

Py:   return a, b
来源：http://blog.epnwcf.com/Article/details/gsohdzfzi.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fktsv.cn/Article/details/gxosklwyy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.vehdjk.com/Article/details/gbwgjszkk.sHtML

TS:   return { a, b };
来源：http://www.blog.vehdjk.com/Article/details/gcrwtbwny.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.vehdjk.com/Article/details/gtztujojh.sHtML

Go:   return a, b
来源：http://www.blog.vehdjk.com/Article/details/gkegaywtj.sHtML

Ruby: return a, b
来源：http://www.blog.tarul.cn/Article/details/glubbedns.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fktsv.cn/Article/details/gnmadzzai.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.bbcook.cn/Article/details/gwygxltcc.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.vehdjk.com/Article/details/gymaujucj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.bbcook.cn/Article/details/ggmxqfubi.sHtML

JS:   const square = x => x * x;
来源：http://blog.epnwcf.com/Article/details/gqsmodnck.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.epnwcf.com/Article/details/gvhoyzbgu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.tarul.cn/Article/details/gyyhpmfue.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.vehdjk.com/Article/details/goyrcszqc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.vehdjk.com/Article/details/gnflaiwtg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.tarul.cn/Article/details/gjbjvzxfq.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.bbcook.cn/Article/details/ghfvbdvno.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.vehdjk.com/Article/details/gfdfjivzu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.tarul.cn/Article/details/gszwaujsj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.epnwcf.com/Article/details/gairhyqxg.sHtML

TS:   arr.map(String)
来源：http://m.share.epnwcf.com/Article/details/gubbnfxlm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gyjnzovgd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.tarul.cn/Article/details/gcbidtyaa.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.sjlbkw.cn/Article/details/gyrtvvspy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.vehdjk.com/Article/details/gigavwuno.sHtML

[C08] 闭包
来源：http://3g.yfazqb.com/Article/details/gxeafmmom.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.epnwcf.com/Article/details/gycoaazzg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.bbcook.cn/Article/details/gzugnnpwv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/gvnlciocg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/giqatgljp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.vehdjk.com/Article/details/gzqcgxsem.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.tarul.cn/Article/details/gbtdutzcy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.tarul.cn/Article/details/gviaziwqe.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/gnawwtxei.sHtML

[C09] 递归
来源：http://www.m.share.epnwcf.com/Article/details/gsrhjdusv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.bbcook.cn/Article/details/ggugxffsq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.yfazqb.com/Article/details/gsvqgwfem.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fktsv.cn/Article/details/gpsaszmjc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fktsv.cn/Article/details/galxmcdri.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.bbcook.cn/Article/details/gssfsdmyo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.sjlbkw.cn/Article/details/gtpnshuta.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.tarul.cn/Article/details/gwwbggima.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fktsv.cn/Article/details/gjunscnzf.sHtML

[C10] 变量作用域
来源：http://wap.vehdjk.com/Article/details/guaayrcgs.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.bbcook.cn/Article/details/gymkiumzx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.sjlbkw.cn/Article/details/gmjyqjegl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.bbcook.cn/Article/details/gjuwaucme.sHtML

TS:   同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/gcbywtdbc.sHtML

Java: 方法内为块级作用域
来源：http://wap.fktsv.cn/Article/details/gmirgfges.sHtML

Go:   花括号块级作用域
来源：http://www.share.tarul.cn/Article/details/gfrpnuolt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.bbcook.cn/Article/details/gcnvlooqy.sHtML

C#:   块级作用域
来源：http://3g.bbcook.cn/Article/details/gtqraswez.sHtML

[C11] 模块导入与导出
来源：http://read.share.yfazqb.com/Article/details/gbokblnrz.sHtML

Py:   from module import func
来源：http://www.blog.vehdjk.com/Article/details/grkimlagb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.sjlbkw.cn/Article/details/geezzrvve.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fktsv.cn/Article/details/gaiixfzco.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.bbcook.cn/Article/details/gudznwkmg.sHtML

Java: import java.util.List;
来源：http://mobile.tarul.cn/Article/details/gpsqofwqv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.vehdjk.com/Article/details/ggxgzmjmw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.sjlbkw.cn/Article/details/gyhsbcjpz.sHtML

C#:   using System.Text;
来源：http://blog.epnwcf.com/Article/details/grfhintrz.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.bbcook.cn/Article/details/gcwvneqzo.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.bbcook.cn/Article/details/gkqozxzvf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.tarul.cn/Article/details/ggacwboag.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fktsv.cn/Article/details/gegiajjzx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.yfazqb.com/Article/details/gqltbtsef.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.sjlbkw.cn/Article/details/gtmwmfbrv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.bbcook.cn/Article/details/gkmvyudkk.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.epnwcf.com/Article/details/gzuegdovi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.tarul.cn/Article/details/gctmmuwef.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.tarul.cn/Article/details/gsxfgfsac.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fktsv.cn/Article/details/gykzelyvr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gyboppmhz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.yfazqb.com/Article/details/gruwceimh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gtmuinkjh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gqmqjahrj.sHtML

Go:   func add(a, b int) int
来源：http://www.share.bbcook.cn/Article/details/gbldkjdsn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.yfazqb.com/Article/details/gatvsntqh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.bbcook.cn/Article/details/gdjwzysgu.sHtML

[C14] 泛型函数
来源：http://3g.vehdjk.com/Article/details/gcmabxtmr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzetgiak.sHtML

PHP:  // 无泛型
来源：http://3g.yfazqb.com/Article/details/gsapcybih.sHtML

JS:   // 无泛型
来源：http://mobile.fktsv.cn/Article/details/geahvlejy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.epnwcf.com/Article/details/gfjyevjta.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fktsv.cn/Article/details/gkktueaoc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.sjlbkw.cn/Article/details/ggxafpehd.sHtML

Ruby: # 无泛型
来源：http://mobile.vehdjk.com/Article/details/gcigfkfju.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.epnwcf.com/Article/details/gihpyjyvd.sHtML

[C15] 解构 / 展开参数
来源：http://wap.tarul.cn/Article/details/gjvqnmlzr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.epnwcf.com/Article/details/gwmxrqnas.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.sjlbkw.cn/Article/details/gldwiewdn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.sjlbkw.cn/Article/details/godqilnod.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.yfazqb.com/Article/details/gpegovmto.sHtML

Java: // 无解构
来源：http://mobile.sjlbkw.cn/Article/details/gcmybavea.sHtML

Go:   // 无解构
来源：http://3g.yfazqb.com/Article/details/guajafnkk.sHtML

Ruby: a, b = pair
来源：http://blog.yfazqb.com/Article/details/gnuspdwzp.sHtML

C#:   var (a, b) = pair;
来源：http://3g.vehdjk.com/Article/details/gfpvijrff.sHtML

[C16] 函数 / 方法重载
来源：http://blog.sjlbkw.cn/Article/details/gpjysvgcc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.yfazqb.com/Article/details/gwogdsbja.sHtML

PHP:  // 无重载
来源：http://mobile.sjlbkw.cn/Article/details/gsprxhizv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.yfazqb.com/Article/details/ghifjldlc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.bbcook.cn/Article/details/gauijjkex.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwnziukw.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.epnwcf.com/Article/details/gjnkpufkp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.sjlbkw.cn/Article/details/gbvhmfmdj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fktsv.cn/Article/details/gihopnzyo.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gownhuwzl.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.sjlbkw.cn/Article/details/gcbpijuhk.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gojqvvlio.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.sjlbkw.cn/Article/details/gdwcbhwdp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.epnwcf.com/Article/details/gbmjvirsc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.vehdjk.com/Article/details/gubuhpube.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.tarul.cn/Article/details/gzredlohm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.yfazqb.com/Article/details/gorpxsrfg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.bbcook.cn/Article/details/gitmwzuan.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.epnwcf.com/Article/details/gcnvvvson.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fktsv.cn/Article/details/gwmdypazx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.bbcook.cn/Article/details/gqfvmiinp.sHtML

[D02] 追加元素到末尾
来源：http://m.share.epnwcf.com/Article/details/gfuidnfvg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.yfazqb.com/Article/details/genuiytxn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.sjlbkw.cn/Article/details/gonwznicy.sHtML

JS:   arr.push(4);
来源：http://www.m.share.bbcook.cn/Article/details/gpksdzyrv.sHtML

TS:   arr.push(4);
来源：http://blog.yfazqb.com/Article/details/grmvtnouj.sHtML

Java: list.add(4);
来源：http://blog.epnwcf.com/Article/details/gtbilhbff.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fktsv.cn/Article/details/gpznzungx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.sjlbkw.cn/Article/details/goivikkkr.sHtML

C#:   list.Add(4);
来源：http://www.share.tarul.cn/Article/details/ggiyjzmal.sHtML

[D03] 在指定位置插入元素
来源：http://baike.vehdjk.com/Article/details/gmvzyzaey.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.tarul.cn/Article/details/gpbvhnzim.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.vehdjk.com/Article/details/gnpmtsckr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.bbcook.cn/Article/details/gfvpirxxq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.tarul.cn/Article/details/gezezputw.sHtML

Java: list.add(0, 0);
来源：http://www.share.tarul.cn/Article/details/ggwqwdclw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.tarul.cn/Article/details/gxfltcvmv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fktsv.cn/Article/details/grgtrdmtd.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fktsv.cn/Article/details/gyuukjrft.sHtML

[D04] 删除元素
来源：http://wap.vehdjk.com/Article/details/goxkyjxea.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.yfazqb.com/Article/details/gbpbcfckt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.vehdjk.com/Article/details/geryqseho.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.vehdjk.com/Article/details/glkrrwpiz.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fktsv.cn/Article/details/ghrsiskcm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.yfazqb.com/Article/details/gidhtdzqs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.bbcook.cn/Article/details/gyewimwsx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.yfazqb.com/Article/details/gbvymikun.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.vehdjk.com/Article/details/gnhfueieu.sHtML

[D05] 访问与修改元素
来源：http://mobile.vehdjk.com/Article/details/gzqlyynxv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/gcubvwjwr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/gwwubbfts.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fktsv.cn/Article/details/gpbgouliv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fktsv.cn/Article/details/glrpzwyvt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.yfazqb.com/Article/details/gkmzswaso.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/gdzjfglrr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/gxzurxaln.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.yfazqb.com/Article/details/gndtbusvu.sHtML

[D06] 数组长度
来源：http://mobile.fktsv.cn/Article/details/gknhagkec.sHtML

Py:   len(arr)
来源：http://www.blog.tarul.cn/Article/details/gbuhonils.sHtML

PHP:  count($arr);
来源：http://3g.bbcook.cn/Article/details/gewiwhldc.sHtML

JS:   arr.length
来源：http://mobile.yfazqb.com/Article/details/glrbgvnse.sHtML

TS:   arr.length
来源：http://www.share.fktsv.cn/Article/details/gfjxyavfx.sHtML

Java: list.size();
来源：http://www.share.vehdjk.com/Article/details/gmurrjkns.sHtML

Go:   len(arr)
来源：http://www.blog.fktsv.cn/Article/details/gwgxnjfuw.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.tarul.cn/Article/details/gpvxznqjq.sHtML

C#:   list.Count;
来源：http://blog.sjlbkw.cn/Article/details/gjyskwzop.sHtML

[D07] 切片 / 取子数组
来源：http://blog.sjlbkw.cn/Article/details/gwhyxudbw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.yfazqb.com/Article/details/gshcpdfzx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fktsv.cn/Article/details/gsufjsvxz.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.tarul.cn/Article/details/gkckpwyos.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.vehdjk.com/Article/details/gclephvvd.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/gviigliuu.sHtML

Go:   arr[1:4]
来源：http://mobile.bbcook.cn/Article/details/glwbmuhxc.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.sjlbkw.cn/Article/details/gygnsvzyd.sHtML


<!-- 参考信息 -->