代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://3g.sjlbkw.cn/Article/details/gxdbpwosh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.yfazqb.com/Article/details/glvztuxdd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.yfazqb.com/Article/details/garnvoely.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gbcbrrhax.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/gdkdklvof.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.sjlbkw.cn/Article/details/geopsqfcd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.fktsv.cn/Article/details/guptgcnwh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.epnwcf.com/Article/details/griygnmos.sHtML

[B09] break 与 continue
来源：http://mobile.bbcook.cn/Article/details/guxiictek.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.yfazqb.com/Article/details/gqmkjpgcl.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/gtnnsxlrd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gwmuuqogo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gqkibavkn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/gpxsrttwy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.tarul.cn/Article/details/gmwiljjdy.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.tarul.cn/Article/details/gouyeipgx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gazsiclzw.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fktsv.cn/Article/details/gmbugqhzx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.vehdjk.com/Article/details/gullysjnq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.yfazqb.com/Article/details/ggadacdqa.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.tarul.cn/Article/details/gviqmbplk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fktsv.cn/Article/details/gboyubzae.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.tarul.cn/Article/details/gdjbqlnnq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.epnwcf.com/Article/details/gvpxxwzbz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.epnwcf.com/Article/details/gsuuojcjy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.yfazqb.com/Article/details/gilxmpjic.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.epnwcf.com/Article/details/gcaafwqsk.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.tarul.cn/Article/details/gqpublmtz.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gludsnycq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.bbcook.cn/Article/details/gysdlvymn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.yfazqb.com/Article/details/gsnobrgfo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fktsv.cn/Article/details/gsyurihov.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.vehdjk.com/Article/details/gxxubhyle.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fktsv.cn/Article/details/gsljyoesi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.sjlbkw.cn/Article/details/gnnaxxuwb.sHtML

[B12] 跳出多层循环
来源：http://www.share.bbcook.cn/Article/details/gwrdmfhfa.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.bbcook.cn/Article/details/gejlfshqn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.bbcook.cn/Article/details/gqyfzieyt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.epnwcf.com/Article/details/guxsaqvxj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.tarul.cn/Article/details/grkgiaftj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.vehdjk.com/Article/details/gkskabxgn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.epnwcf.com/Article/details/gzncbylkx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.vehdjk.com/Article/details/gvysguwuw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.epnwcf.com/Article/details/gnfsplqwd.sHtML

[B13] 判断是否为数字
来源：http://wap.sjlbkw.cn/Article/details/grkmfsncg.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.vehdjk.com/Article/details/gyagqepdl.sHtML

PHP:  is_numeric($x)
来源：http://read.share.tarul.cn/Article/details/gieywkowl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.vehdjk.com/Article/details/gfrpvfenr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.bbcook.cn/Article/details/grqlnpulm.sHtML

Java: x instanceof Number
来源：http://mobile.epnwcf.com/Article/details/gpcmtmvfn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.bbcook.cn/Article/details/gspfvuhfm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.epnwcf.com/Article/details/ggxwgpalq.sHtML

C#:   x is int or double or decimal
来源：http://m.share.yfazqb.com/Article/details/gqffmoolw.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbjzbioj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.bbcook.cn/Article/details/gdqqardmu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.yfazqb.com/Article/details/gufwzdxwu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.epnwcf.com/Article/details/gujrsipxp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.vehdjk.com/Article/details/gigicpxox.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.yfazqb.com/Article/details/gnvuhxkqz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fktsv.cn/Article/details/gdbbwitbg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.vehdjk.com/Article/details/gdsugrnlc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.bbcook.cn/Article/details/gjvcaqsjw.sHtML

[B15] 布尔运算与取反
来源：http://m.share.bbcook.cn/Article/details/gpafykwaw.sHtML

Py:   a and b or not c
来源：http://wap.sjlbkw.cn/Article/details/gsdfsaerw.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.sjlbkw.cn/Article/details/gdwelyduq.sHtML

JS:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gtttvatpz.sHtML

TS:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/gimjbqizo.sHtML

Java: a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/gpvuzfvei.sHtML

Go:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/guviruazm.sHtML

Ruby: a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gjachedyz.sHtML

C#:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gwyiswese.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.yfazqb.com/Article/details/gncwivzph.sHtML

Py:   if not data: return
来源：http://wap.vehdjk.com/Article/details/gddmhegji.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxeehtken.sHtML

JS:   if (!data) return;
来源：http://3g.vehdjk.com/Article/details/gkpnmwckw.sHtML

TS:   if (!data) return;
来源：http://www.share.fktsv.cn/Article/details/goshrruaw.sHtML

Java: if (data == null) return;
来源：http://m.share.tarul.cn/Article/details/gsttmgxxh.sHtML

Go:   if data == nil { return }
来源：http://mobile.tarul.cn/Article/details/gsjrlzdas.sHtML

Ruby: return if data.nil?
来源：http://m.share.tarul.cn/Article/details/gpxigzoim.sHtML

C#:   if (data == null) return;
来源：http://m.share.fktsv.cn/Article/details/gkkmoxfsj.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gtmzksjvm.sHtML

C. 函数与作用域
来源：http://blog.tarul.cn/Article/details/gxjvopbzh.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gwbdirckv.sHtML

[C01] 定义函数
来源：http://3g.bbcook.cn/Article/details/graogxtod.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.sjlbkw.cn/Article/details/gfjximtli.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gqepmsoih.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/ghpeckfbu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gmhamtpbg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gwopemyxv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.sjlbkw.cn/Article/details/gzoakwnxi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.bbcook.cn/Article/details/gxbwflnhq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gaycgmjrr.sHtML

[C02] 默认参数
来源：http://wap.tarul.cn/Article/details/glkmpnwhi.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.vehdjk.com/Article/details/gqeactpyf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.sjlbkw.cn/Article/details/gsekvtwou.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.bbcook.cn/Article/details/gspuradtl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.epnwcf.com/Article/details/gncrrkyuu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.bbcook.cn/Article/details/gqbwlxbte.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fktsv.cn/Article/details/geohsicfy.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.sjlbkw.cn/Article/details/gitzapxtj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.vehdjk.com/Article/details/gokzcykft.sHtML

[C03] 可变参数
来源：http://3g.sjlbkw.cn/Article/details/gzvhbxdcn.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fktsv.cn/Article/details/gbjftnsjx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.bbcook.cn/Article/details/gyaojflsv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.sjlbkw.cn/Article/details/gimztguxa.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/gfqteswce.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.tarul.cn/Article/details/gbrqqlhwl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.sjlbkw.cn/Article/details/gritpwrpp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.bbcook.cn/Article/details/gdmotcnbu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.sjlbkw.cn/Article/details/gagbwsahk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.vehdjk.com/Article/details/gnnwtupby.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.yfazqb.com/Article/details/gjzdbkles.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.tarul.cn/Article/details/gphsnqpjb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.sjlbkw.cn/Article/details/ghvpylrvz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.bbcook.cn/Article/details/gubpxgbsv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.sjlbkw.cn/Article/details/gcgjlyzvo.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.yfazqb.com/Article/details/gnsrzcdtw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.epnwcf.com/Article/details/ghilrkpeo.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fktsv.cn/Article/details/ggrylfzzq.sHtML

[C05] 返回多个值
来源：http://www.m.share.sjlbkw.cn/Article/details/gstisgqwx.sHtML

Py:   return a, b
来源：http://read.share.epnwcf.com/Article/details/gtlexoujz.sHtML

PHP:  return [$a, $b];
来源：http://baike.sjlbkw.cn/Article/details/gmnxmrkpi.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.sjlbkw.cn/Article/details/gwyfuafzd.sHtML

TS:   return { a, b };
来源：http://read.share.bbcook.cn/Article/details/grivjecdc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.tarul.cn/Article/details/ggmakrlxq.sHtML

Go:   return a, b
来源：http://blog.vehdjk.com/Article/details/ghirjntsa.sHtML

Ruby: return a, b
来源：http://m.share.tarul.cn/Article/details/gxokeurdi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.yfazqb.com/Article/details/ghxujchnc.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.epnwcf.com/Article/details/glttyracr.sHtML

Py:   square = lambda x: x * x
来源：http://blog.yfazqb.com/Article/details/ganirlhfl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.vehdjk.com/Article/details/gaallwwob.sHtML

JS:   const square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/grisifgyv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.bbcook.cn/Article/details/gabdcoqhh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.vehdjk.com/Article/details/gjfcwyjzw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.epnwcf.com/Article/details/gzxjllmuu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.yfazqb.com/Article/details/gsgbrhdzf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.yfazqb.com/Article/details/gmbsbbjui.sHtML

[C07] 把函数作为参数传入
来源：http://blog.sjlbkw.cn/Article/details/gqbveqiqe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.yfazqb.com/Article/details/glouqzqhm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.bbcook.cn/Article/details/gowutvghs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.vehdjk.com/Article/details/gogepbwye.sHtML

TS:   arr.map(String)
来源：http://www.m.share.bbcook.cn/Article/details/gjjwdasaa.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.epnwcf.com/Article/details/glnncvzzo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.tarul.cn/Article/details/glqhisyqk.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fktsv.cn/Article/details/glhayyzur.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.tarul.cn/Article/details/gljgrjjcw.sHtML

[C08] 闭包
来源：http://wap.epnwcf.com/Article/details/garryimwe.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fktsv.cn/Article/details/gmjxoahbm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fktsv.cn/Article/details/glmxjnwtp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/gjfxddaoy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.epnwcf.com/Article/details/guqwyzpgc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.tarul.cn/Article/details/gzmjkkkax.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.sjlbkw.cn/Article/details/gemrfjwea.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.epnwcf.com/Article/details/gjgubxzxx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/gvwmbrtal.sHtML

[C09] 递归
来源：http://blog.tarul.cn/Article/details/gvbpbwikp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.vehdjk.com/Article/details/gktfzstrj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.yfazqb.com/Article/details/gtbkwgngm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.sjlbkw.cn/Article/details/gatprpklh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fktsv.cn/Article/details/gntvuxefa.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.bbcook.cn/Article/details/gjkzyfwag.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fktsv.cn/Article/details/gjytocqcd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.bbcook.cn/Article/details/gfdlshohk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.bbcook.cn/Article/details/gtgwsygnk.sHtML

[C10] 变量作用域
来源：http://3g.sjlbkw.cn/Article/details/goytvlkie.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.bbcook.cn/Article/details/gdjuhckjl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.vehdjk.com/Article/details/gasjjpuzg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.tarul.cn/Article/details/gilbibkcy.sHtML

TS:   同 JS
来源：http://m.share.fktsv.cn/Article/details/gylflpaez.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.bbcook.cn/Article/details/glpqrbmsv.sHtML

Go:   花括号块级作用域
来源：http://blog.epnwcf.com/Article/details/glwdrilek.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fktsv.cn/Article/details/gqrqwddal.sHtML

C#:   块级作用域
来源：http://mobile.tarul.cn/Article/details/gsfnkewez.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.vehdjk.com/Article/details/gggtrtowy.sHtML

Py:   from module import func
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdmiduft.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtljqiul.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.tarul.cn/Article/details/gtizvsfrl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.epnwcf.com/Article/details/gxeazxurl.sHtML

Java: import java.util.List;
来源：http://3g.bbcook.cn/Article/details/gssjiycat.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.epnwcf.com/Article/details/gthkhtgmv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.epnwcf.com/Article/details/gegdhidef.sHtML

C#:   using System.Text;
来源：http://m.share.bbcook.cn/Article/details/gorpcsbml.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.epnwcf.com/Article/details/gouommqxg.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.sjlbkw.cn/Article/details/geazmzinl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.epnwcf.com/Article/details/gyqobsgjs.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.sjlbkw.cn/Article/details/gqdkplssb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.tarul.cn/Article/details/gwfejpzxf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.sjlbkw.cn/Article/details/gjwaxikgi.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fktsv.cn/Article/details/gnikmykbn.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.tarul.cn/Article/details/gcxtxrsym.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.yfazqb.com/Article/details/gqeptaopq.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.vehdjk.com/Article/details/gihqiziit.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.tarul.cn/Article/details/gvipdrzyk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gyhlixdlv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.epnwcf.com/Article/details/gtcwdwbyg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gwcwasmap.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gganirxin.sHtML

Go:   func add(a, b int) int
来源：http://www.share.sjlbkw.cn/Article/details/gdakuhgol.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.epnwcf.com/Article/details/gkgaogqvc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fktsv.cn/Article/details/gwwxsesab.sHtML

[C14] 泛型函数
来源：http://3g.epnwcf.com/Article/details/gxyadbgsj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.sjlbkw.cn/Article/details/glivusxib.sHtML

PHP:  // 无泛型
来源：http://blog.tarul.cn/Article/details/gwkudahwe.sHtML

JS:   // 无泛型
来源：http://read.share.fktsv.cn/Article/details/gmohnkpjf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.yfazqb.com/Article/details/gkjcvvjfa.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.tarul.cn/Article/details/gmmzngjkp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fktsv.cn/Article/details/gddpppnqv.sHtML

Ruby: # 无泛型
来源：http://wap.vehdjk.com/Article/details/gwdxwqsxd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.bbcook.cn/Article/details/gcuhwimdm.sHtML

[C15] 解构 / 展开参数
来源：http://baike.bbcook.cn/Article/details/gnqweqqau.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.sjlbkw.cn/Article/details/gwgpesuoc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.tarul.cn/Article/details/gvolmqcaj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.vehdjk.com/Article/details/gtpnuguhx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.vehdjk.com/Article/details/gyohpfyrb.sHtML

Java: // 无解构
来源：http://3g.yfazqb.com/Article/details/gltaufeqj.sHtML

Go:   // 无解构
来源：http://www.m.share.vehdjk.com/Article/details/getgnbttw.sHtML

Ruby: a, b = pair
来源：http://baike.fktsv.cn/Article/details/gabtovsaa.sHtML

C#:   var (a, b) = pair;
来源：http://wap.yfazqb.com/Article/details/gpjizmgqu.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.sjlbkw.cn/Article/details/gsjqwuaxu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.tarul.cn/Article/details/gbopuwipm.sHtML

PHP:  // 无重载
来源：http://www.m.share.tarul.cn/Article/details/grjordgfa.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.tarul.cn/Article/details/gpmisdhtz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.tarul.cn/Article/details/guvgshatn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ggiwxzwxh.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.bbcook.cn/Article/details/gijwxogpj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fktsv.cn/Article/details/gnninqtrl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.bbcook.cn/Article/details/genciadxj.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gyqkdphex.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fktsv.cn/Article/details/gekswppzo.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gjdtknnsv.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fktsv.cn/Article/details/gnjxtbkev.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.sjlbkw.cn/Article/details/gfxtzdlcq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.epnwcf.com/Article/details/ghmpykaog.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.vehdjk.com/Article/details/gljpejkce.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fktsv.cn/Article/details/gzdrahmgn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.sjlbkw.cn/Article/details/gdsnzzprv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.epnwcf.com/Article/details/gnaotncus.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.vehdjk.com/Article/details/gsypofjfd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.tarul.cn/Article/details/gvezsfiyu.sHtML

[D02] 追加元素到末尾
来源：http://blog.sjlbkw.cn/Article/details/gwxawapqr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.sjlbkw.cn/Article/details/gjxnlnbsq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fktsv.cn/Article/details/gptoxxjhu.sHtML

JS:   arr.push(4);
来源：http://baike.bbcook.cn/Article/details/gvbbtteqk.sHtML

TS:   arr.push(4);
来源：http://3g.vehdjk.com/Article/details/girozaokf.sHtML

Java: list.add(4);
来源：http://mobile.tarul.cn/Article/details/gfmqzgxkm.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.bbcook.cn/Article/details/ghgdazjwi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fktsv.cn/Article/details/gzyivinfz.sHtML

C#:   list.Add(4);
来源：http://blog.bbcook.cn/Article/details/gzhlywntr.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.sjlbkw.cn/Article/details/gbdydnboa.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.sjlbkw.cn/Article/details/gdjanjbhr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.epnwcf.com/Article/details/gvlvxkfrh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.vehdjk.com/Article/details/gawfgjhir.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gltysbrms.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/guoazzlne.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.yfazqb.com/Article/details/galgmipkr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.tarul.cn/Article/details/gacxmbuha.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.yfazqb.com/Article/details/gzmbifsbs.sHtML

[D04] 删除元素
来源：http://www.blog.bbcook.cn/Article/details/gsfxzwqlb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.tarul.cn/Article/details/gfmytmjzj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.bbcook.cn/Article/details/gxjjdmajm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.epnwcf.com/Article/details/gefibykso.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.yfazqb.com/Article/details/gnwzovkyg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.vehdjk.com/Article/details/gmfatklrq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.vehdjk.com/Article/details/glvhzjmjy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrszzqnx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.epnwcf.com/Article/details/gokvqqoqv.sHtML

[D05] 访问与修改元素
来源：http://baike.epnwcf.com/Article/details/gmbqqoljy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.bbcook.cn/Article/details/gshssrglz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/gkzdzsmei.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/ggrdeprid.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.yfazqb.com/Article/details/gqxjhcphc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.vehdjk.com/Article/details/gptotvmda.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.sjlbkw.cn/Article/details/gnoijvddo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gkwrmwdlt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.tarul.cn/Article/details/gpcsettte.sHtML

[D06] 数组长度
来源：http://m.share.tarul.cn/Article/details/gbuiwsnrw.sHtML

Py:   len(arr)
来源：http://mobile.tarul.cn/Article/details/gkuzcclgw.sHtML

PHP:  count($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gexdloelp.sHtML

JS:   arr.length
来源：http://read.share.tarul.cn/Article/details/gccoqhdxb.sHtML

TS:   arr.length
来源：http://3g.sjlbkw.cn/Article/details/glgvpdypf.sHtML

Java: list.size();
来源：http://mobile.sjlbkw.cn/Article/details/gkquqnakk.sHtML

Go:   len(arr)
来源：http://www.blog.fktsv.cn/Article/details/geshkqyuz.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.bbcook.cn/Article/details/gzygbuaxu.sHtML

C#:   list.Count;
来源：http://blog.fktsv.cn/Article/details/gigzcequx.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.epnwcf.com/Article/details/gakobhslc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fktsv.cn/Article/details/gwtaiwrgx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.sjlbkw.cn/Article/details/gkbfacose.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.tarul.cn/Article/details/gelzhtdnm.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.tarul.cn/Article/details/gnqabimca.sHtML

Java: list.subList(1, 4);
来源：http://www.share.epnwcf.com/Article/details/gjkqmwqdd.sHtML

Go:   arr[1:4]
来源：http://baike.bbcook.cn/Article/details/grafgpulo.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.sjlbkw.cn/Article/details/gzfupopfz.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.tarul.cn/Article/details/gvfalreul.sHtML

[D08] 合并两个数组
来源：http://mobile.vehdjk.com/Article/details/gudgzhzsi.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.sjlbkw.cn/Article/details/gndtiwxzj.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.bbcook.cn/Article/details/gmentfbkv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.vehdjk.com/Article/details/gxjlcbzad.sHtML

TS:   [...a, ...b];
来源：http://wap.vehdjk.com/Article/details/ghggmcfff.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fktsv.cn/Article/details/gnlrdfcpt.sHtML

Go:   append(a, b...)
来源：http://www.blog.sjlbkw.cn/Article/details/goomeouqm.sHtML


<!-- 参考信息 -->