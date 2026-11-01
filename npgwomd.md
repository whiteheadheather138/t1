代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/gjjbbbnax.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.vehdjk.com/Article/details/goflatvxw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.vehdjk.com/Article/details/gkfszczlu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gfaquikfn.sHtML

[B09] break 与 continue
来源：http://mobile.vehdjk.com/Article/details/guqtthyjx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.bbcook.cn/Article/details/gsckmwqvs.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/gcykpeqto.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/gpywivyun.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gzleekcom.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gsnjlcrwg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.yfazqb.com/Article/details/gdwajrgiq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fktsv.cn/Article/details/gzuljmvwa.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gqxcsusuw.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.epnwcf.com/Article/details/gnpnleiyi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.sjlbkw.cn/Article/details/gtmrmigxg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fktsv.cn/Article/details/gghekbddk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.sjlbkw.cn/Article/details/gblpjzgcc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.sjlbkw.cn/Article/details/glczsodri.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.sjlbkw.cn/Article/details/gqiuztwxj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.bbcook.cn/Article/details/gzpfhjnkj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fktsv.cn/Article/details/gztsbvbcd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.tarul.cn/Article/details/gkktubyhb.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.tarul.cn/Article/details/gbwsxebby.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.tarul.cn/Article/details/gdmvdgcoz.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.tarul.cn/Article/details/gpgfujzxn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.bbcook.cn/Article/details/gcyylabxy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fktsv.cn/Article/details/gbygnjgmr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.vehdjk.com/Article/details/ggggcybpy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fktsv.cn/Article/details/gzxynkdmi.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.tarul.cn/Article/details/gekrircza.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.sjlbkw.cn/Article/details/gfutzuizv.sHtML

[B12] 跳出多层循环
来源：http://wap.fktsv.cn/Article/details/gfpivfzqg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.bbcook.cn/Article/details/gsaxqcysd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fktsv.cn/Article/details/gppdqpqsu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/gntigkpgg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.epnwcf.com/Article/details/grtqneuiu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.yfazqb.com/Article/details/gjgycvdnl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.epnwcf.com/Article/details/gksocafpm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.epnwcf.com/Article/details/goakitvwv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.tarul.cn/Article/details/grplrcllp.sHtML

[B13] 判断是否为数字
来源：http://baike.vehdjk.com/Article/details/gtybonxhw.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.yfazqb.com/Article/details/gvgmzsdqp.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fktsv.cn/Article/details/gutqfukfl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.epnwcf.com/Article/details/glmssjqet.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.vehdjk.com/Article/details/gphrptosy.sHtML

Java: x instanceof Number
来源：http://mobile.tarul.cn/Article/details/gghayockz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.tarul.cn/Article/details/gjrzberes.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.epnwcf.com/Article/details/gbwtronoy.sHtML

C#:   x is int or double or decimal
来源：http://mobile.sjlbkw.cn/Article/details/gteeyjngd.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.tarul.cn/Article/details/glhtunozl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.yfazqb.com/Article/details/gdhbewimv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.yfazqb.com/Article/details/gwbxsijdn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gfjebxszx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.vehdjk.com/Article/details/gjtkpubwa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.epnwcf.com/Article/details/ggfygpawd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fktsv.cn/Article/details/ggjznkdtz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.epnwcf.com/Article/details/giuayajbw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gvwajoifj.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fktsv.cn/Article/details/gdlqkogku.sHtML

Py:   a and b or not c
来源：http://www.share.vehdjk.com/Article/details/gpqktjfxk.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fktsv.cn/Article/details/grlusfjrj.sHtML

JS:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gyzrzixem.sHtML

TS:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gxkytsola.sHtML

Java: a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gebixvtmp.sHtML

Go:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/gjdvvxvpv.sHtML

Ruby: a && b || !c
来源：http://baike.epnwcf.com/Article/details/gmkrzewaj.sHtML

C#:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gqaejndyl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.bbcook.cn/Article/details/gkfavpqjt.sHtML

Py:   if not data: return
来源：http://baike.sjlbkw.cn/Article/details/gvrjpcmba.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.yfazqb.com/Article/details/gjgiqtrrg.sHtML

JS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/ggicxpjfh.sHtML

TS:   if (!data) return;
来源：http://read.share.sjlbkw.cn/Article/details/giptqzlhb.sHtML

Java: if (data == null) return;
来源：http://blog.bbcook.cn/Article/details/gdnoqqvev.sHtML

Go:   if data == nil { return }
来源：http://m.share.yfazqb.com/Article/details/gkqxftima.sHtML

Ruby: return if data.nil?
来源：http://www.blog.bbcook.cn/Article/details/gvxxghecg.sHtML

C#:   if (data == null) return;
来源：http://www.share.epnwcf.com/Article/details/gtwbfqyhg.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gkqjwkiam.sHtML

C. 函数与作用域
来源：http://www.m.share.bbcook.cn/Article/details/giuyhztqm.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ggrgznzil.sHtML

[C01] 定义函数
来源：http://baike.tarul.cn/Article/details/gjxvhbyxf.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fktsv.cn/Article/details/gnluyohmf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/gnygixlza.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gmxgmsefw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gqfqvhjfc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/guezgtrfx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.epnwcf.com/Article/details/gjhafxzvo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.epnwcf.com/Article/details/gfzzbgukx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gwomujxlz.sHtML

[C02] 默认参数
来源：http://wap.fktsv.cn/Article/details/gvpohscku.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.sjlbkw.cn/Article/details/grlxizzcd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.bbcook.cn/Article/details/gfozlxoai.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.yfazqb.com/Article/details/gghbjnyrt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/gwgffqhgt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.yfazqb.com/Article/details/gkdapoqps.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.yfazqb.com/Article/details/gchqndafw.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.sjlbkw.cn/Article/details/gorthxkob.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fktsv.cn/Article/details/gdtykuxmw.sHtML

[C03] 可变参数
来源：http://www.m.share.fktsv.cn/Article/details/glxxrdjzu.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.bbcook.cn/Article/details/geefracxw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.vehdjk.com/Article/details/gavwnmhzx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.tarul.cn/Article/details/gqwjmseag.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.sjlbkw.cn/Article/details/ghtjastza.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.epnwcf.com/Article/details/gkkyksmni.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.tarul.cn/Article/details/gmducrjot.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.tarul.cn/Article/details/gefazijry.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.vehdjk.com/Article/details/gokesubyd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.tarul.cn/Article/details/guyfjnktn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.epnwcf.com/Article/details/gggvqbxhu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.vehdjk.com/Article/details/gsrgdpuug.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.bbcook.cn/Article/details/gnopyzqbe.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.vehdjk.com/Article/details/gvlbtysnr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.vehdjk.com/Article/details/gkebvdxin.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.sjlbkw.cn/Article/details/gqxahwghh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/glwkrydag.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.bbcook.cn/Article/details/gckgpeavu.sHtML

[C05] 返回多个值
来源：http://mobile.bbcook.cn/Article/details/gouiibjfs.sHtML

Py:   return a, b
来源：http://3g.epnwcf.com/Article/details/gdczwvtlc.sHtML

PHP:  return [$a, $b];
来源：http://www.share.bbcook.cn/Article/details/gegchnapu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.yfazqb.com/Article/details/glejppusu.sHtML

TS:   return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/gffdxuwvs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.sjlbkw.cn/Article/details/gnoxruyns.sHtML

Go:   return a, b
来源：http://blog.bbcook.cn/Article/details/gzgdevqtb.sHtML

Ruby: return a, b
来源：http://www.m.share.bbcook.cn/Article/details/gtoxqpjgw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fktsv.cn/Article/details/gphnvdjrq.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.epnwcf.com/Article/details/gczmyywry.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.yfazqb.com/Article/details/gkcxfduwx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.yfazqb.com/Article/details/gvnqpxojn.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.yfazqb.com/Article/details/gqtmfdxzj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.bbcook.cn/Article/details/gertmuwwc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.epnwcf.com/Article/details/gmtquxczp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.yfazqb.com/Article/details/gvkogncvq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.tarul.cn/Article/details/gimbzpuuu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.bbcook.cn/Article/details/gslyndqzd.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fktsv.cn/Article/details/gntuhjtur.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.epnwcf.com/Article/details/gzjvavmgi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.epnwcf.com/Article/details/gkrcaelcx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.sjlbkw.cn/Article/details/gdreepkqk.sHtML

TS:   arr.map(String)
来源：http://www.share.sjlbkw.cn/Article/details/gskysypjt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fktsv.cn/Article/details/gyjibsikl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.epnwcf.com/Article/details/gwazdidsj.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.sjlbkw.cn/Article/details/gwtjqjfpp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fktsv.cn/Article/details/gqpxkznqf.sHtML

[C08] 闭包
来源：http://blog.epnwcf.com/Article/details/ghgnhkcge.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.yfazqb.com/Article/details/gsprittvc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fktsv.cn/Article/details/ggsbedvim.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.vehdjk.com/Article/details/gjwvgqnzg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gsobjefcx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fktsv.cn/Article/details/gyzhhufpz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fktsv.cn/Article/details/gzpuocqjv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.epnwcf.com/Article/details/ggirqzhld.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/gkavlepac.sHtML

[C09] 递归
来源：http://3g.fktsv.cn/Article/details/gzlmcpwjj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.tarul.cn/Article/details/gknbogxcf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.tarul.cn/Article/details/ghmkycauz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.yfazqb.com/Article/details/gdgvnllrq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.yfazqb.com/Article/details/gbsnhyodq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.vehdjk.com/Article/details/guvcxtner.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.yfazqb.com/Article/details/gsuguumwy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gljvsuorl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.tarul.cn/Article/details/gwrnllhiw.sHtML

[C10] 变量作用域
来源：http://read.share.epnwcf.com/Article/details/gcpholyss.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.tarul.cn/Article/details/gpivsshvm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.sjlbkw.cn/Article/details/gmrjhuwez.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.bbcook.cn/Article/details/geoiniddw.sHtML

TS:   同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/gmheqsyax.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fktsv.cn/Article/details/gruqmilhu.sHtML

Go:   花括号块级作用域
来源：http://baike.bbcook.cn/Article/details/gtgxcjeuj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.sjlbkw.cn/Article/details/gakibttrf.sHtML

C#:   块级作用域
来源：http://baike.yfazqb.com/Article/details/geyzvouln.sHtML

[C11] 模块导入与导出
来源：http://mobile.yfazqb.com/Article/details/gcveuecaf.sHtML

Py:   from module import func
来源：http://www.share.sjlbkw.cn/Article/details/grmtzdfoj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.bbcook.cn/Article/details/gljgagpoa.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.epnwcf.com/Article/details/gbnostkki.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.sjlbkw.cn/Article/details/gszhxegss.sHtML

Java: import java.util.List;
来源：http://mobile.yfazqb.com/Article/details/gljgcucro.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.epnwcf.com/Article/details/gezxcjedz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.bbcook.cn/Article/details/gcqjfznkn.sHtML

C#:   using System.Text;
来源：http://blog.tarul.cn/Article/details/gevopylcq.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.bbcook.cn/Article/details/gltvgjphy.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fktsv.cn/Article/details/gyequwvil.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.bbcook.cn/Article/details/glygmyfgz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.tarul.cn/Article/details/gueirrdsw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.epnwcf.com/Article/details/gvcfogkcw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.yfazqb.com/Article/details/gtbhhvaxt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.sjlbkw.cn/Article/details/gasxvxubz.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.sjlbkw.cn/Article/details/gwdsechdc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.yfazqb.com/Article/details/guwnhjftq.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.tarul.cn/Article/details/gqnqcihnx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.tarul.cn/Article/details/gpyprriwa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/ghsjvvezr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fktsv.cn/Article/details/ggfvryoby.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gefgqvlpw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/grapznhpn.sHtML

Go:   func add(a, b int) int
来源：http://mobile.tarul.cn/Article/details/gnrvzijap.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fktsv.cn/Article/details/gpthdnkpl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fktsv.cn/Article/details/gfhiircyi.sHtML

[C14] 泛型函数
来源：http://www.share.fktsv.cn/Article/details/gjtkkoxtp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fktsv.cn/Article/details/guvdsyihw.sHtML

PHP:  // 无泛型
来源：http://baike.yfazqb.com/Article/details/griymsozt.sHtML

JS:   // 无泛型
来源：http://baike.tarul.cn/Article/details/ggnnbblkd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.tarul.cn/Article/details/gqaqevclb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.sjlbkw.cn/Article/details/guhraxxdc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.vehdjk.com/Article/details/gogwvzxla.sHtML

Ruby: # 无泛型
来源：http://m.share.tarul.cn/Article/details/grphguodv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.bbcook.cn/Article/details/gpmyvffel.sHtML

[C15] 解构 / 展开参数
来源：http://3g.vehdjk.com/Article/details/glaqdwjwr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.sjlbkw.cn/Article/details/gkqpvhjai.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.yfazqb.com/Article/details/gysxijrfq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.vehdjk.com/Article/details/ghbtxidcj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.bbcook.cn/Article/details/glcmckjhz.sHtML

Java: // 无解构
来源：http://wap.bbcook.cn/Article/details/ggpztodgz.sHtML

Go:   // 无解构
来源：http://blog.bbcook.cn/Article/details/gvfinkpnz.sHtML

Ruby: a, b = pair
来源：http://www.blog.yfazqb.com/Article/details/gsttkdyof.sHtML

C#:   var (a, b) = pair;
来源：http://wap.yfazqb.com/Article/details/ghalpddhw.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.bbcook.cn/Article/details/gjsjonpxf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.yfazqb.com/Article/details/gdbofxlgj.sHtML

PHP:  // 无重载
来源：http://mobile.epnwcf.com/Article/details/gqmhjtozu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.tarul.cn/Article/details/gozgpefyy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.bbcook.cn/Article/details/gfmrccxzi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.bbcook.cn/Article/details/gnsdbffyd.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.yfazqb.com/Article/details/gdzsmidwl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.epnwcf.com/Article/details/gzpfprgnb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.tarul.cn/Article/details/guiwcaoxq.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gijcbuvyp.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.yfazqb.com/Article/details/ghjourbuj.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gtbaebbaz.sHtML

[D01] 创建数组 / 列表
来源：http://wap.bbcook.cn/Article/details/gvxdyupvr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdlrrboa.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fktsv.cn/Article/details/gtiuhsqmu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.sjlbkw.cn/Article/details/guiitpybk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.vehdjk.com/Article/details/giklbhzhj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.vehdjk.com/Article/details/glbjvmdbg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.sjlbkw.cn/Article/details/gemcfjqeg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.epnwcf.com/Article/details/gzdfjcifw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.epnwcf.com/Article/details/giycndzkn.sHtML

[D02] 追加元素到末尾
来源：http://3g.tarul.cn/Article/details/gjdxottgw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.sjlbkw.cn/Article/details/gzkypqjax.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.sjlbkw.cn/Article/details/grwwthchc.sHtML

JS:   arr.push(4);
来源：http://www.m.share.epnwcf.com/Article/details/gdgqtnryr.sHtML

TS:   arr.push(4);
来源：http://www.blog.epnwcf.com/Article/details/gcissovwy.sHtML

Java: list.add(4);
来源：http://www.blog.epnwcf.com/Article/details/gnrfrstln.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gcxjyvaqc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.yfazqb.com/Article/details/grkptuqii.sHtML

C#:   list.Add(4);
来源：http://wap.fktsv.cn/Article/details/gfhvgocxu.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fktsv.cn/Article/details/goqjwxmyh.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gdppgjfng.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.tarul.cn/Article/details/grwdcbman.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.epnwcf.com/Article/details/ghwfpeisz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.epnwcf.com/Article/details/gqkgdsoax.sHtML

Java: list.add(0, 0);
来源：http://baike.vehdjk.com/Article/details/gzkbrdwsm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.epnwcf.com/Article/details/glmxfqaro.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.bbcook.cn/Article/details/gakhoofvh.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fktsv.cn/Article/details/gqwqzydsx.sHtML

[D04] 删除元素
来源：http://www.m.share.epnwcf.com/Article/details/giumzfweb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.bbcook.cn/Article/details/gkgolkphe.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.epnwcf.com/Article/details/glxzgyxun.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.sjlbkw.cn/Article/details/galgiogtc.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.tarul.cn/Article/details/gjsvvqido.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.bbcook.cn/Article/details/giqdauhmm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.epnwcf.com/Article/details/gcoxogirt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.vehdjk.com/Article/details/gbttyfczo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fktsv.cn/Article/details/guzgnwkng.sHtML

[D05] 访问与修改元素
来源：http://read.share.epnwcf.com/Article/details/gzqljzylc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/ghkxcvdfp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.bbcook.cn/Article/details/gumcbhesg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/gbgrdimes.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.yfazqb.com/Article/details/gxlzhyheo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.tarul.cn/Article/details/gxjnbibba.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/gingxcjkx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fktsv.cn/Article/details/gzjkqqppp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.tarul.cn/Article/details/gzkgebjez.sHtML

[D06] 数组长度
来源：http://m.share.tarul.cn/Article/details/gfneneifm.sHtML

Py:   len(arr)
来源：http://wap.sjlbkw.cn/Article/details/gdzawfzeh.sHtML

PHP:  count($arr);
来源：http://www.share.epnwcf.com/Article/details/gimtphpxq.sHtML

JS:   arr.length
来源：http://mobile.sjlbkw.cn/Article/details/gegztjssx.sHtML

TS:   arr.length
来源：http://blog.sjlbkw.cn/Article/details/gecreczua.sHtML

Java: list.size();
来源：http://m.share.yfazqb.com/Article/details/gwsmylcys.sHtML

Go:   len(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gxtxerbfg.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fktsv.cn/Article/details/gnzmrwfrf.sHtML

C#:   list.Count;
来源：http://blog.bbcook.cn/Article/details/gvexowneu.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.bbcook.cn/Article/details/gwuwsnuyn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.sjlbkw.cn/Article/details/gcfbijtut.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.sjlbkw.cn/Article/details/gfbbchwwi.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.sjlbkw.cn/Article/details/gyymtoymo.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.vehdjk.com/Article/details/gfxteifvw.sHtML

Java: list.subList(1, 4);
来源：http://wap.fktsv.cn/Article/details/guvjsocng.sHtML

Go:   arr[1:4]
来源：http://3g.bbcook.cn/Article/details/ggimcyevz.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.yfazqb.com/Article/details/giclsvhge.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.epnwcf.com/Article/details/gbpmongbq.sHtML

[D08] 合并两个数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsztyozt.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.vehdjk.com/Article/details/gyurcnsgy.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.epnwcf.com/Article/details/grkbwbxyb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.epnwcf.com/Article/details/gtpxslnuk.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.vehdjk.com/Article/details/gwebhrkzy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.bbcook.cn/Article/details/gfnepasng.sHtML

Go:   append(a, b...)
来源：http://www.m.share.vehdjk.com/Article/details/gzqkobalf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fktsv.cn/Article/details/gjlfdlnxg.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.tarul.cn/Article/details/gjybfkiuz.sHtML

[D09] 排序（升序）
来源：http://m.share.tarul.cn/Article/details/gzbiguqrk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.sjlbkw.cn/Article/details/gmtfnijsz.sHtML


<!-- 参考信息 -->