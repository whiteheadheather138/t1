代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fktsv.cn/Article/details/gcxwwdnlt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.vehdjk.com/Article/details/ggdzxcisz.sHtML

[B07] while 循环
来源：http://wap.tarul.cn/Article/details/gzrzqgevx.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fktsv.cn/Article/details/gnxhdzyuo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gsgonewkn.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/gqsqvzppu.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gxhmcxble.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/grrhvkhkz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fktsv.cn/Article/details/gmqkmnogm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.yfazqb.com/Article/details/gemlewutl.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.tarul.cn/Article/details/guhacavda.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.sjlbkw.cn/Article/details/gjoqeprlo.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.vehdjk.com/Article/details/gvuxvbwfu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.epnwcf.com/Article/details/gcpwezwfr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.vehdjk.com/Article/details/gnelraeyx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/gxktittox.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gntwwbdqx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.epnwcf.com/Article/details/gmbxrbpnl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.epnwcf.com/Article/details/geitjivgk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/glnzbmmtt.sHtML

[B09] break 与 continue
来源：http://www.share.bbcook.cn/Article/details/gkrydmbju.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fktsv.cn/Article/details/guykbxkwx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/goiofmgxf.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.tarul.cn/Article/details/gndfegtlg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gtqotaidz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gzsskoamz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.vehdjk.com/Article/details/gkvgfijcu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fktsv.cn/Article/details/gqxdhxetz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.tarul.cn/Article/details/gxitumelx.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.bbcook.cn/Article/details/ggymkpvls.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.epnwcf.com/Article/details/gdorgewib.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.epnwcf.com/Article/details/gzjlvrlzj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.sjlbkw.cn/Article/details/gibtfbdti.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.bbcook.cn/Article/details/ggjdrkrko.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.tarul.cn/Article/details/gotixkixv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.vehdjk.com/Article/details/gkpmzrdia.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.bbcook.cn/Article/details/gturrrerv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.vehdjk.com/Article/details/gkaniftmb.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.tarul.cn/Article/details/gafndphkh.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.sjlbkw.cn/Article/details/gpahquyyp.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gtubgnpgs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.epnwcf.com/Article/details/gtwmsnxbz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.epnwcf.com/Article/details/gusnkygda.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fktsv.cn/Article/details/gtyiivuml.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.bbcook.cn/Article/details/gpphjdsmg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.tarul.cn/Article/details/gckcdobfc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.tarul.cn/Article/details/gcrfdmdgl.sHtML

[B12] 跳出多层循环
来源：http://3g.epnwcf.com/Article/details/gsmdgyedf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fktsv.cn/Article/details/ghierelkt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.yfazqb.com/Article/details/gbnsjsxez.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.sjlbkw.cn/Article/details/getqlnhge.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.epnwcf.com/Article/details/gbpsxlteo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fktsv.cn/Article/details/gklssewcw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.bbcook.cn/Article/details/gygkqadht.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.epnwcf.com/Article/details/gzvzxdqvq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.bbcook.cn/Article/details/gudlqmwgh.sHtML

[B13] 判断是否为数字
来源：http://read.share.vehdjk.com/Article/details/gajbjycix.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.bbcook.cn/Article/details/gxmqnztpc.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.yfazqb.com/Article/details/gcagedvhq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.tarul.cn/Article/details/gdhkdxhue.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.bbcook.cn/Article/details/gdtnrrgjc.sHtML

Java: x instanceof Number
来源：http://mobile.sjlbkw.cn/Article/details/grskelsvy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.bbcook.cn/Article/details/gmlzwtekk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.epnwcf.com/Article/details/gemsimeuz.sHtML

C#:   x is int or double or decimal
来源：http://3g.yfazqb.com/Article/details/gzsvaaadx.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.sjlbkw.cn/Article/details/giwkidggm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.vehdjk.com/Article/details/gdjizikpz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.bbcook.cn/Article/details/gvxfekqcb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gncwrtwcs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.sjlbkw.cn/Article/details/garvvnwio.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.bbcook.cn/Article/details/gszjfxmvb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.vehdjk.com/Article/details/gixgbpgsv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.sjlbkw.cn/Article/details/gtrdbzhvn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbafubad.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.epnwcf.com/Article/details/gaamfcuhw.sHtML

Py:   a and b or not c
来源：http://m.share.tarul.cn/Article/details/goomjsksu.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fktsv.cn/Article/details/gulfxlbpi.sHtML

JS:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gpszjfmiq.sHtML

TS:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gyemxxjqm.sHtML

Java: a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gmxdnzqfu.sHtML

Go:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gyvjkpsel.sHtML

Ruby: a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gyrdqssiw.sHtML

C#:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gyaajhfsi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.epnwcf.com/Article/details/ggsqtjrnq.sHtML

Py:   if not data: return
来源：http://www.m.share.vehdjk.com/Article/details/grpdpiyyv.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.yfazqb.com/Article/details/gtkfataji.sHtML

JS:   if (!data) return;
来源：http://read.share.fktsv.cn/Article/details/gmcaqvebj.sHtML

TS:   if (!data) return;
来源：http://read.share.tarul.cn/Article/details/gzcfijfid.sHtML

Java: if (data == null) return;
来源：http://www.share.yfazqb.com/Article/details/gfrurmjgz.sHtML

Go:   if data == nil { return }
来源：http://blog.yfazqb.com/Article/details/gkbbbynjs.sHtML

Ruby: return if data.nil?
来源：http://wap.vehdjk.com/Article/details/gykiluhnb.sHtML

C#:   if (data == null) return;
来源：http://baike.fktsv.cn/Article/details/girzoqpjb.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gpsfljciv.sHtML

C. 函数与作用域
来源：http://baike.tarul.cn/Article/details/gkrrypeba.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gvegmznev.sHtML

[C01] 定义函数
来源：http://3g.epnwcf.com/Article/details/gbnmbjuoq.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.epnwcf.com/Article/details/gfqqlvdfy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/grrsrhsbh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gymhkyxqs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/godfnvxii.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gvhstjxzo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.vehdjk.com/Article/details/gmtoeulcc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fktsv.cn/Article/details/gsylemnri.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gkbmqveji.sHtML

[C02] 默认参数
来源：http://blog.bbcook.cn/Article/details/gydgmunty.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.epnwcf.com/Article/details/gdknfhijd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.vehdjk.com/Article/details/gyjfrdemk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.yfazqb.com/Article/details/gvnuzsgkq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.tarul.cn/Article/details/gcodeevpd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.epnwcf.com/Article/details/gponjioql.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.bbcook.cn/Article/details/gbwbbbcsw.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.vehdjk.com/Article/details/gzcpiesxu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.epnwcf.com/Article/details/gsokeeglo.sHtML

[C03] 可变参数
来源：http://www.blog.fktsv.cn/Article/details/gyspvivap.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.sjlbkw.cn/Article/details/gxspzvgaf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.bbcook.cn/Article/details/gdsmcerkn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ganhqlgpb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.vehdjk.com/Article/details/gguxtnmus.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.tarul.cn/Article/details/gqnkgghqk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.sjlbkw.cn/Article/details/gicnnzehq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.vehdjk.com/Article/details/gmwgkywgr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.bbcook.cn/Article/details/ghwonfbzg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.yfazqb.com/Article/details/gnkhhggur.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.vehdjk.com/Article/details/gmmpkerpe.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.epnwcf.com/Article/details/gdimmqmto.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.yfazqb.com/Article/details/gdxncqmlp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.sjlbkw.cn/Article/details/gvvuzedtf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.yfazqb.com/Article/details/goycidifd.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.yfazqb.com/Article/details/grqpanupe.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.epnwcf.com/Article/details/gvpruhkxq.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.sjlbkw.cn/Article/details/gtomvrepp.sHtML

[C05] 返回多个值
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnkourcx.sHtML

Py:   return a, b
来源：http://baike.yfazqb.com/Article/details/gghozosic.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.epnwcf.com/Article/details/gtdyewbpi.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.bbcook.cn/Article/details/gxekgvflc.sHtML

TS:   return { a, b };
来源：http://3g.epnwcf.com/Article/details/gxxnbzsws.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fktsv.cn/Article/details/guftstlta.sHtML

Go:   return a, b
来源：http://read.share.fktsv.cn/Article/details/ghuyfkbfd.sHtML

Ruby: return a, b
来源：http://read.share.vehdjk.com/Article/details/ghnnrqyoy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.epnwcf.com/Article/details/gchxhhiqr.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.yfazqb.com/Article/details/gcrhtzqbp.sHtML

Py:   square = lambda x: x * x
来源：http://3g.yfazqb.com/Article/details/gqufemzcf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.bbcook.cn/Article/details/ggcycstbc.sHtML

JS:   const square = x => x * x;
来源：http://m.share.yfazqb.com/Article/details/gdrwetmvw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.vehdjk.com/Article/details/gpvmrxnvx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.epnwcf.com/Article/details/gehlntjux.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.bbcook.cn/Article/details/gwargylsl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.vehdjk.com/Article/details/gxejxauel.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gfghiihvu.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.sjlbkw.cn/Article/details/gfiexellz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.vehdjk.com/Article/details/gkjzxatec.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.sjlbkw.cn/Article/details/ghpwdhraz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.bbcook.cn/Article/details/gfajbbkcv.sHtML

TS:   arr.map(String)
来源：http://3g.yfazqb.com/Article/details/gmgyrrnrp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.sjlbkw.cn/Article/details/gvnxcctes.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.tarul.cn/Article/details/gchhyugem.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.epnwcf.com/Article/details/gslywgduj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.sjlbkw.cn/Article/details/gwfphvmpf.sHtML

[C08] 闭包
来源：http://m.share.bbcook.cn/Article/details/gfksokmug.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.yfazqb.com/Article/details/gjglbfomm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.sjlbkw.cn/Article/details/ggseymwxz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/gqstospuo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.sjlbkw.cn/Article/details/ggweobybc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.sjlbkw.cn/Article/details/gcbtfzkfb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.epnwcf.com/Article/details/gpuobhkyc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.sjlbkw.cn/Article/details/geuglrzzr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fktsv.cn/Article/details/gerolpnwk.sHtML

[C09] 递归
来源：http://www.m.share.tarul.cn/Article/details/grjepzdmq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.epnwcf.com/Article/details/gggcscbke.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.epnwcf.com/Article/details/globtfjzp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.yfazqb.com/Article/details/goxgsxnzo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.tarul.cn/Article/details/gffmskgun.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.tarul.cn/Article/details/glvsyombw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.tarul.cn/Article/details/gynxieuhy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/gljyklrex.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.bbcook.cn/Article/details/gyyuymutd.sHtML

[C10] 变量作用域
来源：http://m.share.epnwcf.com/Article/details/gtlhkwzmg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.sjlbkw.cn/Article/details/gcavspywo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.epnwcf.com/Article/details/gjzkuzbrq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.vehdjk.com/Article/details/gzmruyixf.sHtML

TS:   同 JS
来源：http://www.blog.yfazqb.com/Article/details/gwhzfzxyl.sHtML

Java: 方法内为块级作用域
来源：http://3g.epnwcf.com/Article/details/gciagqxec.sHtML

Go:   花括号块级作用域
来源：http://wap.epnwcf.com/Article/details/gbrglcmfw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.sjlbkw.cn/Article/details/gvykwzkhb.sHtML

C#:   块级作用域
来源：http://wap.fktsv.cn/Article/details/gdxoupjpn.sHtML

[C11] 模块导入与导出
来源：http://read.share.fktsv.cn/Article/details/grressvre.sHtML

Py:   from module import func
来源：http://blog.sjlbkw.cn/Article/details/goumnwohp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.epnwcf.com/Article/details/guyqnichx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.sjlbkw.cn/Article/details/gpikmjjny.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.epnwcf.com/Article/details/gvdowtscd.sHtML

Java: import java.util.List;
来源：http://m.share.vehdjk.com/Article/details/gjyrfitdo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.sjlbkw.cn/Article/details/gccvmweje.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.sjlbkw.cn/Article/details/gerbegnre.sHtML

C#:   using System.Text;
来源：http://baike.tarul.cn/Article/details/gbvczowho.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.epnwcf.com/Article/details/gaihaihyh.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.sjlbkw.cn/Article/details/gnsukudto.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fktsv.cn/Article/details/gctpyakgd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.bbcook.cn/Article/details/gzjoqrwpm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.bbcook.cn/Article/details/gdebjcvrl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.vehdjk.com/Article/details/gbvfbafvj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.bbcook.cn/Article/details/gsgfnanja.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.yfazqb.com/Article/details/gpqqjfofr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.sjlbkw.cn/Article/details/ghuvelfty.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.tarul.cn/Article/details/gwcybjdcm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.tarul.cn/Article/details/gnnujdrlu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/gcgtbosvk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.bbcook.cn/Article/details/gqgpvctip.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gjszzqtsg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/glynuofqx.sHtML

Go:   func add(a, b int) int
来源：http://wap.fktsv.cn/Article/details/gydzxiwzt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.bbcook.cn/Article/details/gpmfxmdol.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.yfazqb.com/Article/details/gbhslvlnv.sHtML

[C14] 泛型函数
来源：http://blog.epnwcf.com/Article/details/gnhgjalks.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.vehdjk.com/Article/details/gmwspdsdr.sHtML

PHP:  // 无泛型
来源：http://wap.fktsv.cn/Article/details/gegxjuldl.sHtML

JS:   // 无泛型
来源：http://3g.epnwcf.com/Article/details/geljsvndc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.vehdjk.com/Article/details/gvwonvcyi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fktsv.cn/Article/details/glftgquoh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.epnwcf.com/Article/details/ghgppzubu.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/ghvqxbklz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.vehdjk.com/Article/details/gkmbmqbiv.sHtML

[C15] 解构 / 展开参数
来源：http://baike.yfazqb.com/Article/details/grcfurbgg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.epnwcf.com/Article/details/gfiakzwbj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.sjlbkw.cn/Article/details/ghjwecurs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.bbcook.cn/Article/details/gyulhjlmn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.sjlbkw.cn/Article/details/giupzqwdq.sHtML

Java: // 无解构
来源：http://read.share.bbcook.cn/Article/details/gyqfowjcf.sHtML

Go:   // 无解构
来源：http://baike.bbcook.cn/Article/details/gdtpxwdqk.sHtML

Ruby: a, b = pair
来源：http://www.share.tarul.cn/Article/details/gsajzagxm.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fktsv.cn/Article/details/gzmaedjcs.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fktsv.cn/Article/details/ghzlqpaky.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.bbcook.cn/Article/details/gyziapanm.sHtML

PHP:  // 无重载
来源：http://www.share.vehdjk.com/Article/details/gnyugfrgj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fktsv.cn/Article/details/gcnrxucdb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.bbcook.cn/Article/details/gklgfqodd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.epnwcf.com/Article/details/gbghhmabh.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.epnwcf.com/Article/details/gekhrowjk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.tarul.cn/Article/details/gyvwtwrhx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fktsv.cn/Article/details/gtfzkjilj.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gpnzbitir.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.tarul.cn/Article/details/gouiiwoyt.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gvhbclgco.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.yfazqb.com/Article/details/gdijyietf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.bbcook.cn/Article/details/gcesmgupk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.tarul.cn/Article/details/gifwmzwbv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.vehdjk.com/Article/details/gdnzwvklm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fktsv.cn/Article/details/gmouxxkaa.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fktsv.cn/Article/details/gggmlivwp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fktsv.cn/Article/details/gaxyfosyz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fktsv.cn/Article/details/ghiaqdvgh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fktsv.cn/Article/details/ghmgllldu.sHtML

[D02] 追加元素到末尾
来源：http://blog.tarul.cn/Article/details/gztfkusft.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.bbcook.cn/Article/details/grkefffhx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.vehdjk.com/Article/details/grumbxcse.sHtML

JS:   arr.push(4);
来源：http://www.blog.epnwcf.com/Article/details/ghjiobcvh.sHtML

TS:   arr.push(4);
来源：http://www.share.yfazqb.com/Article/details/gvpmoxtyg.sHtML

Java: list.add(4);
来源：http://m.share.yfazqb.com/Article/details/gmhehthps.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.bbcook.cn/Article/details/gvqvpywmo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.epnwcf.com/Article/details/gehkwsmgz.sHtML

C#:   list.Add(4);
来源：http://www.blog.bbcook.cn/Article/details/gqivurglu.sHtML

[D03] 在指定位置插入元素
来源：http://baike.vehdjk.com/Article/details/gpzpzvmmy.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.tarul.cn/Article/details/gwtivwhvd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fktsv.cn/Article/details/gjhorhmiw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.yfazqb.com/Article/details/gewftxssf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.bbcook.cn/Article/details/gjcgqntfn.sHtML

Java: list.add(0, 0);
来源：http://read.share.fktsv.cn/Article/details/ghdiksdac.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.bbcook.cn/Article/details/guxbtobck.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.yfazqb.com/Article/details/gqygtxvmy.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.vehdjk.com/Article/details/gwkgqtrbw.sHtML

[D04] 删除元素
来源：http://mobile.bbcook.cn/Article/details/gtfqzplfy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.tarul.cn/Article/details/gnwirxzvs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.yfazqb.com/Article/details/gfthzovhf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.epnwcf.com/Article/details/gismcqjfz.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fktsv.cn/Article/details/gkxxzdwyh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.yfazqb.com/Article/details/gbjtnpnso.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.epnwcf.com/Article/details/gvvymwnez.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.sjlbkw.cn/Article/details/gzhidriom.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.epnwcf.com/Article/details/gtlrwtwrf.sHtML

[D05] 访问与修改元素
来源：http://m.share.bbcook.cn/Article/details/gthjmkgfc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/gjxflfgtb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.sjlbkw.cn/Article/details/gggmiawge.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/ghfpovgvx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.tarul.cn/Article/details/gjmtuswmo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.tarul.cn/Article/details/gdfqjpzpk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fktsv.cn/Article/details/grvjnyokj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.epnwcf.com/Article/details/ghmxodxpb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/gxmunhbvu.sHtML

[D06] 数组长度
来源：http://wap.vehdjk.com/Article/details/gybdarlvj.sHtML

Py:   len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/guueqfmyx.sHtML

PHP:  count($arr);
来源：http://www.m.share.tarul.cn/Article/details/gznutztrt.sHtML

JS:   arr.length
来源：http://m.share.vehdjk.com/Article/details/gtdpqlxnu.sHtML

TS:   arr.length
来源：http://wap.sjlbkw.cn/Article/details/gcnagvyru.sHtML

Java: list.size();
来源：http://m.share.fktsv.cn/Article/details/gedzwnnhr.sHtML

Go:   len(arr)
来源：http://mobile.yfazqb.com/Article/details/gosniadbw.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.sjlbkw.cn/Article/details/ggpgnavsy.sHtML

C#:   list.Count;
来源：http://baike.epnwcf.com/Article/details/gvvioigkz.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.vehdjk.com/Article/details/gwwbrkzpt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.epnwcf.com/Article/details/gnwyajzud.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.epnwcf.com/Article/details/gsmmlgmic.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.vehdjk.com/Article/details/ghkwleojq.sHtML


<!-- 参考信息 -->