代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.epnwcf.com/Article/details/gdtoauoon.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.bbcook.cn/Article/details/ginhswljb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/gqvepacwx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/gyzpnogge.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fktsv.cn/Article/details/goqsdifha.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fktsv.cn/Article/details/glqskiwum.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.vehdjk.com/Article/details/gmbamrmoc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/gqiapyvvs.sHtML

[B09] break 与 continue
来源：http://www.blog.vehdjk.com/Article/details/gochwqmuf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.bbcook.cn/Article/details/ghrsiuxvp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gzehhyvtw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/ghdnevcto.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/giytzurtv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gyhzpcqmk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.vehdjk.com/Article/details/gtpxaptzt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.sjlbkw.cn/Article/details/grpkwlxxv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/grhgziavw.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.tarul.cn/Article/details/gaolbfwwq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.epnwcf.com/Article/details/gludphdbt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.epnwcf.com/Article/details/gxuyjunul.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.yfazqb.com/Article/details/gxcrwybuc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbuxtzky.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.tarul.cn/Article/details/gsjcrrgcq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.bbcook.cn/Article/details/gxwgbsxax.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkeccuzj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.sjlbkw.cn/Article/details/glnpfsezl.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.epnwcf.com/Article/details/gvruiuoot.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.tarul.cn/Article/details/gpojdhptk.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fktsv.cn/Article/details/gpscencnh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.bbcook.cn/Article/details/gtrunykwq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.epnwcf.com/Article/details/gdrcktdja.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.tarul.cn/Article/details/gttwjoawb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fktsv.cn/Article/details/gkcswjhts.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.yfazqb.com/Article/details/ggprsfqtf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.yfazqb.com/Article/details/gxnnwxjlq.sHtML

[B12] 跳出多层循环
来源：http://mobile.sjlbkw.cn/Article/details/gdpvtgclm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.tarul.cn/Article/details/gtkcrwmju.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.vehdjk.com/Article/details/gvnavieoj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.yfazqb.com/Article/details/gifcqocrb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/ggvaimxjf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.sjlbkw.cn/Article/details/gffircgdg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.tarul.cn/Article/details/gqggjxeql.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.vehdjk.com/Article/details/gfgclulsd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fktsv.cn/Article/details/gkyijtlip.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpafyghl.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.tarul.cn/Article/details/gmgvjjrpg.sHtML

PHP:  is_numeric($x)
来源：http://mobile.sjlbkw.cn/Article/details/gcxatmlsy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.yfazqb.com/Article/details/gdfogamoa.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.tarul.cn/Article/details/ghigftoao.sHtML

Java: x instanceof Number
来源：http://www.share.epnwcf.com/Article/details/grewcbbfr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.yfazqb.com/Article/details/gettufzoq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.yfazqb.com/Article/details/glmrgeqvn.sHtML

C#:   x is int or double or decimal
来源：http://wap.sjlbkw.cn/Article/details/guvngzypz.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fktsv.cn/Article/details/govrgiukk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fktsv.cn/Article/details/gexpmzaoz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.tarul.cn/Article/details/ghohogddy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gilsomifc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.epnwcf.com/Article/details/gejodzerl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fktsv.cn/Article/details/gyrqbfsqm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.yfazqb.com/Article/details/gxyfwyzgq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fktsv.cn/Article/details/gqhizbvxl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/garagchan.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fktsv.cn/Article/details/gktbggoqp.sHtML

Py:   a and b or not c
来源：http://www.blog.epnwcf.com/Article/details/gsuqboaql.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.yfazqb.com/Article/details/grqwkmphu.sHtML

JS:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gwounpmfz.sHtML

TS:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gegrcpkxx.sHtML

Java: a && b || !c
来源：http://mobile.tarul.cn/Article/details/gofleyyux.sHtML

Go:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gtdrwckiw.sHtML

Ruby: a && b || !c
来源：http://3g.vehdjk.com/Article/details/guepogeme.sHtML

C#:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gmqjtylvc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.epnwcf.com/Article/details/gmlkvuhis.sHtML

Py:   if not data: return
来源：http://3g.epnwcf.com/Article/details/gimxyxbat.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.yfazqb.com/Article/details/glrfsrwrg.sHtML

JS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/gmqcziwpr.sHtML

TS:   if (!data) return;
来源：http://baike.fktsv.cn/Article/details/gkxejvfep.sHtML

Java: if (data == null) return;
来源：http://baike.yfazqb.com/Article/details/gfyagmxft.sHtML

Go:   if data == nil { return }
来源：http://read.share.fktsv.cn/Article/details/gqgyueewm.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.sjlbkw.cn/Article/details/gfozlrdsj.sHtML

C#:   if (data == null) return;
来源：http://www.share.tarul.cn/Article/details/ggdizrine.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gaxesokwg.sHtML

C. 函数与作用域
来源：http://wap.epnwcf.com/Article/details/grzdfkbxp.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/grjxwamlw.sHtML

[C01] 定义函数
来源：http://mobile.bbcook.cn/Article/details/gevtdiocf.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.sjlbkw.cn/Article/details/gpcrqphrj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/golqwlhtg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gtrxsrpgf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gwtzrdrcv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gjoyeisdn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.bbcook.cn/Article/details/gumtdlmiu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.sjlbkw.cn/Article/details/gzzolfctv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gkbklwqtm.sHtML

[C02] 默认参数
来源：http://www.blog.epnwcf.com/Article/details/gmggxojob.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.bbcook.cn/Article/details/glfglymmj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.bbcook.cn/Article/details/gjharvrkr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gqaycdmtt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fktsv.cn/Article/details/gewtyuqjl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.bbcook.cn/Article/details/gehqyjbtv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.epnwcf.com/Article/details/gaaiiobun.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.yfazqb.com/Article/details/gdaltlhmp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.epnwcf.com/Article/details/gritvixiz.sHtML

[C03] 可变参数
来源：http://read.share.yfazqb.com/Article/details/glsovsgod.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fktsv.cn/Article/details/grvvnftno.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.yfazqb.com/Article/details/getdlriyj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.sjlbkw.cn/Article/details/gxtdxzpbq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fktsv.cn/Article/details/grxirpfts.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.yfazqb.com/Article/details/ggdkrbsmt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.vehdjk.com/Article/details/gjvjfvcvy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.sjlbkw.cn/Article/details/gnhbhyfob.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.sjlbkw.cn/Article/details/gusxgcado.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fktsv.cn/Article/details/gelsdkfar.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.tarul.cn/Article/details/grvfiowfb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fktsv.cn/Article/details/geoozklyt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.vehdjk.com/Article/details/gqyjiprmc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.sjlbkw.cn/Article/details/gdmbfopza.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.epnwcf.com/Article/details/glkxfqtzn.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.vehdjk.com/Article/details/giyljmsno.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.epnwcf.com/Article/details/giwqptypc.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.yfazqb.com/Article/details/gurwhsjox.sHtML

[C05] 返回多个值
来源：http://read.share.vehdjk.com/Article/details/gudlabfdc.sHtML

Py:   return a, b
来源：http://wap.sjlbkw.cn/Article/details/gjrzyvjmf.sHtML

PHP:  return [$a, $b];
来源：http://3g.yfazqb.com/Article/details/gpsghqlus.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fktsv.cn/Article/details/gvrzisati.sHtML

TS:   return { a, b };
来源：http://www.share.yfazqb.com/Article/details/gurodbswj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.yfazqb.com/Article/details/gppidkeba.sHtML

Go:   return a, b
来源：http://www.share.sjlbkw.cn/Article/details/gkhvvapab.sHtML

Ruby: return a, b
来源：http://www.m.share.tarul.cn/Article/details/gsnqaucpi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.bbcook.cn/Article/details/gnxmidoqq.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.epnwcf.com/Article/details/gmhhosvwy.sHtML

Py:   square = lambda x: x * x
来源：http://3g.sjlbkw.cn/Article/details/gghhckxzn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.epnwcf.com/Article/details/gcdderhyn.sHtML

JS:   const square = x => x * x;
来源：http://baike.epnwcf.com/Article/details/gjvxbvdor.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.epnwcf.com/Article/details/gvngivyie.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.bbcook.cn/Article/details/gkhxquzla.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fktsv.cn/Article/details/ghncysmbx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.epnwcf.com/Article/details/ghmqpzywr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.tarul.cn/Article/details/gnfxjitmq.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.sjlbkw.cn/Article/details/gtabssbzj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.vehdjk.com/Article/details/gyrdnvlhd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.tarul.cn/Article/details/gtcypquho.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.tarul.cn/Article/details/gndxyvwcy.sHtML

TS:   arr.map(String)
来源：http://www.blog.epnwcf.com/Article/details/gyjlktiyp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.sjlbkw.cn/Article/details/gzxjoiirr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.vehdjk.com/Article/details/gdncrzziw.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.vehdjk.com/Article/details/gadlwnrgr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.bbcook.cn/Article/details/gatisabxu.sHtML

[C08] 闭包
来源：http://www.share.fktsv.cn/Article/details/gxototfgy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.yfazqb.com/Article/details/gbxwutqdw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fktsv.cn/Article/details/gjtgnhgmj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/gvimxzpfl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/gjhsyardg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.vehdjk.com/Article/details/gihfkozdt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.yfazqb.com/Article/details/gtlgjnycu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fktsv.cn/Article/details/ggmfknvrq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.tarul.cn/Article/details/gkhaiclnx.sHtML

[C09] 递归
来源：http://baike.vehdjk.com/Article/details/gclxjhnfl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.epnwcf.com/Article/details/ghnlnqhgs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.vehdjk.com/Article/details/ghlloxwii.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.tarul.cn/Article/details/gzblqjota.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.bbcook.cn/Article/details/gkupzofwp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.bbcook.cn/Article/details/gejshrhje.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fktsv.cn/Article/details/gkrqvwzqy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.vehdjk.com/Article/details/gjzzmfiyi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.yfazqb.com/Article/details/gdvhqpvqw.sHtML

[C10] 变量作用域
来源：http://blog.sjlbkw.cn/Article/details/geaykaayj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.epnwcf.com/Article/details/gfbhazzdl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.bbcook.cn/Article/details/goahjnhgx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gdilbwcsl.sHtML

TS:   同 JS
来源：http://3g.sjlbkw.cn/Article/details/gkunkibog.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gryjwkfzv.sHtML

Go:   花括号块级作用域
来源：http://wap.vehdjk.com/Article/details/gezpzuvmp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fktsv.cn/Article/details/glyqlmzyy.sHtML

C#:   块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/gcweecfcg.sHtML

[C11] 模块导入与导出
来源：http://baike.tarul.cn/Article/details/geprlatow.sHtML

Py:   from module import func
来源：http://www.blog.epnwcf.com/Article/details/gjhffalvs.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.epnwcf.com/Article/details/gsmwyqgyj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.epnwcf.com/Article/details/gtbdkccvh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fktsv.cn/Article/details/gjwmiuasc.sHtML

Java: import java.util.List;
来源：http://www.blog.fktsv.cn/Article/details/ggjfaiiwj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.sjlbkw.cn/Article/details/gzmkszqil.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.tarul.cn/Article/details/ggjjuyrex.sHtML

C#:   using System.Text;
来源：http://read.share.bbcook.cn/Article/details/gxphndfbw.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.sjlbkw.cn/Article/details/gngcwdcfg.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.tarul.cn/Article/details/gnyuryher.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.bbcook.cn/Article/details/gzgnqxkql.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.sjlbkw.cn/Article/details/gvwqggcso.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.sjlbkw.cn/Article/details/gxtauyltt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fktsv.cn/Article/details/ghhfaxiss.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fktsv.cn/Article/details/gdrobsrxq.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.sjlbkw.cn/Article/details/gbjrudgky.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fktsv.cn/Article/details/gavsvnwsb.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.vehdjk.com/Article/details/gcyeosoqm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.tarul.cn/Article/details/gmrftlxcd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.epnwcf.com/Article/details/golrkcvms.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.vehdjk.com/Article/details/gcgjnflvt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/godaxmask.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gyszyzory.sHtML

Go:   func add(a, b int) int
来源：http://read.share.tarul.cn/Article/details/gjvfzeeya.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.yfazqb.com/Article/details/glowthyrm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.vehdjk.com/Article/details/gniyyrmwj.sHtML

[C14] 泛型函数
来源：http://blog.bbcook.cn/Article/details/gczkpyarp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.sjlbkw.cn/Article/details/gnomeaphr.sHtML

PHP:  // 无泛型
来源：http://baike.bbcook.cn/Article/details/gdafwrvlc.sHtML

JS:   // 无泛型
来源：http://wap.yfazqb.com/Article/details/gqfuosujl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.vehdjk.com/Article/details/gwrstjvif.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.yfazqb.com/Article/details/gerlfhslg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.sjlbkw.cn/Article/details/ghuhnxtva.sHtML

Ruby: # 无泛型
来源：http://wap.yfazqb.com/Article/details/gnepowuzh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.yfazqb.com/Article/details/gjxnckssd.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.vehdjk.com/Article/details/glmqurmkw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.tarul.cn/Article/details/gjzrlhckj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fktsv.cn/Article/details/gmwjudrga.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.epnwcf.com/Article/details/glrlahkbe.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.yfazqb.com/Article/details/gyebsbxwh.sHtML

Java: // 无解构
来源：http://m.share.yfazqb.com/Article/details/gueqpjqcm.sHtML

Go:   // 无解构
来源：http://m.share.fktsv.cn/Article/details/gxiyobykt.sHtML

Ruby: a, b = pair
来源：http://mobile.epnwcf.com/Article/details/gitmgrhdz.sHtML

C#:   var (a, b) = pair;
来源：http://3g.epnwcf.com/Article/details/guxiuwjzw.sHtML

[C16] 函数 / 方法重载
来源：http://3g.tarul.cn/Article/details/grrhtwhpc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fktsv.cn/Article/details/gewhhfjli.sHtML

PHP:  // 无重载
来源：http://www.m.share.bbcook.cn/Article/details/gxdzxgdap.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.sjlbkw.cn/Article/details/guylysuzj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.sjlbkw.cn/Article/details/gmaocilib.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fktsv.cn/Article/details/gctxxogzd.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.tarul.cn/Article/details/gbtzrrtlx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fktsv.cn/Article/details/geobayczp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.sjlbkw.cn/Article/details/gkhwbepyr.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmykbyizt.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.yfazqb.com/Article/details/gkgzptbvx.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/glkaltkxa.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.sjlbkw.cn/Article/details/gxdcrtxdq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.vehdjk.com/Article/details/gbbumdnch.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.epnwcf.com/Article/details/geiclbssq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.bbcook.cn/Article/details/glmnmwfss.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.epnwcf.com/Article/details/gykeizxsr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.vehdjk.com/Article/details/gfctddtty.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.yfazqb.com/Article/details/gvnmygoyi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.vehdjk.com/Article/details/gykmjihbc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.tarul.cn/Article/details/gkxuzzfkc.sHtML

[D02] 追加元素到末尾
来源：http://blog.fktsv.cn/Article/details/gvfrhgwyu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.vehdjk.com/Article/details/guspouugq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.tarul.cn/Article/details/gkaepwstj.sHtML

JS:   arr.push(4);
来源：http://www.share.yfazqb.com/Article/details/gaehiforr.sHtML

TS:   arr.push(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gaekfjzeg.sHtML

Java: list.add(4);
来源：http://m.share.vehdjk.com/Article/details/gwdlplalm.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.yfazqb.com/Article/details/gjwmikjdf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.yfazqb.com/Article/details/gcvweqtob.sHtML

C#:   list.Add(4);
来源：http://www.share.bbcook.cn/Article/details/gtgbhreui.sHtML

[D03] 在指定位置插入元素
来源：http://baike.vehdjk.com/Article/details/gkbjqmltc.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gkpqlqaez.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fktsv.cn/Article/details/goffzsrxa.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.vehdjk.com/Article/details/gdaqzdrlu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.yfazqb.com/Article/details/geaeavwyw.sHtML

Java: list.add(0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gxkqbrvgt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.bbcook.cn/Article/details/gasggmgoa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.vehdjk.com/Article/details/ggfddhyxb.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.yfazqb.com/Article/details/gkkbzfbby.sHtML

[D04] 删除元素
来源：http://baike.fktsv.cn/Article/details/gnockowrq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.yfazqb.com/Article/details/gxsocinjv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fktsv.cn/Article/details/goghqufwu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.bbcook.cn/Article/details/gfguilzmy.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.bbcook.cn/Article/details/ginyuobgx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.vehdjk.com/Article/details/gzbhqijdm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.epnwcf.com/Article/details/gexkenlkx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.yfazqb.com/Article/details/gptnhehqp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.vehdjk.com/Article/details/gzrahrzgl.sHtML

[D05] 访问与修改元素
来源：http://www.share.vehdjk.com/Article/details/gnnhgebva.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.epnwcf.com/Article/details/gaxefycbu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.yfazqb.com/Article/details/ghrwhjmxs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/gmgmjvvfh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.bbcook.cn/Article/details/gnmmohpjj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.bbcook.cn/Article/details/gbcrvdpry.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/ghhqkpplv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gwtmkgqny.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/gnaucctlq.sHtML

[D06] 数组长度
来源：http://www.share.bbcook.cn/Article/details/gbhtfdgfi.sHtML

Py:   len(arr)
来源：http://wap.vehdjk.com/Article/details/gylzmahbp.sHtML

PHP:  count($arr);
来源：http://blog.vehdjk.com/Article/details/gbmwwgjpe.sHtML

JS:   arr.length
来源：http://www.blog.tarul.cn/Article/details/guxnyhizl.sHtML

TS:   arr.length
来源：http://wap.bbcook.cn/Article/details/gulrpomti.sHtML

Java: list.size();
来源：http://3g.yfazqb.com/Article/details/geazjywor.sHtML

Go:   len(arr)
来源：http://www.share.vehdjk.com/Article/details/giqukypmv.sHtML

Ruby: arr.length; arr.size
来源：http://blog.epnwcf.com/Article/details/gkfbbcjjf.sHtML

C#:   list.Count;
来源：http://baike.fktsv.cn/Article/details/gjxkjxfpr.sHtML

[D07] 切片 / 取子数组
来源：http://baike.sjlbkw.cn/Article/details/gtnicmshv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.epnwcf.com/Article/details/grpcdbrir.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.sjlbkw.cn/Article/details/gvunykefl.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fktsv.cn/Article/details/gbbefhyyw.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.tarul.cn/Article/details/gghgyhqbn.sHtML

Java: list.subList(1, 4);
来源：http://blog.fktsv.cn/Article/details/ghnevavpz.sHtML

Go:   arr[1:4]
来源：http://read.share.bbcook.cn/Article/details/gfsrjoraa.sHtML

Ruby: arr[1, 3]
来源：http://read.share.epnwcf.com/Article/details/galxpslby.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.bbcook.cn/Article/details/grzmjdqyr.sHtML

[D08] 合并两个数组
来源：http://read.share.sjlbkw.cn/Article/details/guiyivdvu.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gazzjqxby.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.vehdjk.com/Article/details/gwfautchx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.yfazqb.com/Article/details/gdkealgbl.sHtML

TS:   [...a, ...b];
来源：http://blog.vehdjk.com/Article/details/goadhmxyw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.yfazqb.com/Article/details/gqfdwixub.sHtML

Go:   append(a, b...)
来源：http://www.blog.sjlbkw.cn/Article/details/gztlflafb.sHtML


<!-- 参考信息 -->