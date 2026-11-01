代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fktsv.cn/Article/details/glqarnfnv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.bbcook.cn/Article/details/gutjlqdxe.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/glnljuoqy.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.sjlbkw.cn/Article/details/gcxjuatcn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.epnwcf.com/Article/details/gcfcxbgao.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.tarul.cn/Article/details/goppmxnud.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gohykmakb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/gtmbcoykt.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/gcdfpyctg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.epnwcf.com/Article/details/gtjsffeyx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.yfazqb.com/Article/details/gtfbyogus.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.bbcook.cn/Article/details/ganddlqvk.sHtML

[B09] break 与 continue
来源：http://3g.bbcook.cn/Article/details/gbpqfznxv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.vehdjk.com/Article/details/gekevsvhz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/ghbbilrxe.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gonyygrhd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gxrhdcdml.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/granfrhnl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.tarul.cn/Article/details/ghvzpkivc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.yfazqb.com/Article/details/gwdffsgyk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gkydffvmp.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fktsv.cn/Article/details/gmnbnnbzo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fktsv.cn/Article/details/gdhkipebz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.tarul.cn/Article/details/gkyypudrd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.bbcook.cn/Article/details/gbcwwtyce.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.vehdjk.com/Article/details/gzjsuujzt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fktsv.cn/Article/details/gansydycz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.sjlbkw.cn/Article/details/ggonltnud.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.yfazqb.com/Article/details/gxgcyhyfa.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.bbcook.cn/Article/details/ggqrtnnbb.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.bbcook.cn/Article/details/guofbzzgy.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.epnwcf.com/Article/details/gqmdhslzr.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.tarul.cn/Article/details/gxelczhol.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fktsv.cn/Article/details/genjyuipd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.sjlbkw.cn/Article/details/ghavrclyj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfleaher.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.vehdjk.com/Article/details/gbfialxej.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.bbcook.cn/Article/details/grvyjssgb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.bbcook.cn/Article/details/gmmpjbtlm.sHtML

[B12] 跳出多层循环
来源：http://wap.fktsv.cn/Article/details/goqwlrejy.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.vehdjk.com/Article/details/gasuuidck.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.bbcook.cn/Article/details/gjvgbjwzv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/gbarijhgw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.yfazqb.com/Article/details/guqaydfud.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.sjlbkw.cn/Article/details/gbnokhzub.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fktsv.cn/Article/details/gqbstpfyr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fktsv.cn/Article/details/gygcqatuz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fktsv.cn/Article/details/gtvajnwwj.sHtML

[B13] 判断是否为数字
来源：http://blog.bbcook.cn/Article/details/glehgngsj.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.tarul.cn/Article/details/grcytvoqi.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fktsv.cn/Article/details/gchhwwknw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.epnwcf.com/Article/details/gknzuwzje.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.vehdjk.com/Article/details/ghhuzwbxd.sHtML

Java: x instanceof Number
来源：http://www.share.bbcook.cn/Article/details/gqdpxngzg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.yfazqb.com/Article/details/gkubzcwok.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.vehdjk.com/Article/details/guzkpkemo.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fktsv.cn/Article/details/gnbnrucqv.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.yfazqb.com/Article/details/gwqdqciuo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fktsv.cn/Article/details/gbuamgghf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.epnwcf.com/Article/details/gpfugfehv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/ggontyqci.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.yfazqb.com/Article/details/ggkjadmup.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.vehdjk.com/Article/details/gdxezzatw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fktsv.cn/Article/details/gewjjwxwf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.sjlbkw.cn/Article/details/gnwikyqih.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.yfazqb.com/Article/details/gkmmmhrzc.sHtML

[B15] 布尔运算与取反
来源：http://www.share.tarul.cn/Article/details/gkizepklj.sHtML

Py:   a and b or not c
来源：http://read.share.tarul.cn/Article/details/gobtmhxpr.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.yfazqb.com/Article/details/gjsxbhfqr.sHtML

JS:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gjsherqab.sHtML

TS:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/gpuvrdnsi.sHtML

Java: a && b || !c
来源：http://baike.fktsv.cn/Article/details/gpxhosfel.sHtML

Go:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gkccfylfc.sHtML

Ruby: a && b || !c
来源：http://www.share.epnwcf.com/Article/details/getolqsfy.sHtML

C#:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gzvcdsidf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.bbcook.cn/Article/details/gnzrzlmpp.sHtML

Py:   if not data: return
来源：http://baike.epnwcf.com/Article/details/gilalnjns.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.vehdjk.com/Article/details/gergeftur.sHtML

JS:   if (!data) return;
来源：http://3g.vehdjk.com/Article/details/gacnogcio.sHtML

TS:   if (!data) return;
来源：http://mobile.tarul.cn/Article/details/gozqdrwoz.sHtML

Java: if (data == null) return;
来源：http://3g.tarul.cn/Article/details/ghslfhcec.sHtML

Go:   if data == nil { return }
来源：http://read.share.yfazqb.com/Article/details/gazfrndog.sHtML

Ruby: return if data.nil?
来源：http://read.share.tarul.cn/Article/details/grpnewoqm.sHtML

C#:   if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/gdojmhfgw.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gqplezsgi.sHtML

C. 函数与作用域
来源：http://www.blog.tarul.cn/Article/details/gasbrkmgc.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gubzqlyja.sHtML

[C01] 定义函数
来源：http://www.blog.bbcook.cn/Article/details/gsoxwdjkg.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fktsv.cn/Article/details/gbmfxtieg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/gldfhhkfh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gjddgaboe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gkrhidqrl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gtahmbqsc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.yfazqb.com/Article/details/gxxucpnwo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.vehdjk.com/Article/details/gkkthdagh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/grobgkryb.sHtML

[C02] 默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gpclkkzqp.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.vehdjk.com/Article/details/grjfiwdrd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.tarul.cn/Article/details/gbldxtwtz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.bbcook.cn/Article/details/gncumkufz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/gjaasnzls.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.vehdjk.com/Article/details/gzsbzjtmh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.bbcook.cn/Article/details/grpzdirlf.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.epnwcf.com/Article/details/gcroechxx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fktsv.cn/Article/details/gcgsxklqh.sHtML

[C03] 可变参数
来源：http://mobile.sjlbkw.cn/Article/details/gxswfrvcg.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.sjlbkw.cn/Article/details/glyrkzpiy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.tarul.cn/Article/details/gymeffwue.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.epnwcf.com/Article/details/ghtxphrgy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fktsv.cn/Article/details/gplkoyzty.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fktsv.cn/Article/details/gpszanwlx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.epnwcf.com/Article/details/gxgeuspmk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.sjlbkw.cn/Article/details/gcykoronl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.epnwcf.com/Article/details/gwtvmrmcw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fktsv.cn/Article/details/gxnigkgmx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.tarul.cn/Article/details/gwrdhchfj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.vehdjk.com/Article/details/gvlqsymxk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fktsv.cn/Article/details/gyuviebfe.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.bbcook.cn/Article/details/gxofcbyge.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.vehdjk.com/Article/details/gvxvduqdz.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.vehdjk.com/Article/details/gkmvshsaa.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/gdgljpzqx.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/groccdmqr.sHtML

[C05] 返回多个值
来源：http://m.share.tarul.cn/Article/details/gwbogkzvt.sHtML

Py:   return a, b
来源：http://3g.yfazqb.com/Article/details/gtaoflgxk.sHtML

PHP:  return [$a, $b];
来源：http://3g.epnwcf.com/Article/details/gftjxfvhy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.yfazqb.com/Article/details/gtaqknhyb.sHtML

TS:   return { a, b };
来源：http://www.blog.tarul.cn/Article/details/grmataupd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.sjlbkw.cn/Article/details/geawwtmbd.sHtML

Go:   return a, b
来源：http://3g.vehdjk.com/Article/details/gynlgzisj.sHtML

Ruby: return a, b
来源：http://blog.yfazqb.com/Article/details/gsatuflen.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fktsv.cn/Article/details/gotovxzqg.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.vehdjk.com/Article/details/gpqkndsqf.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fktsv.cn/Article/details/gkseyqdye.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.sjlbkw.cn/Article/details/graevshel.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fktsv.cn/Article/details/gwtyzbnsn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.bbcook.cn/Article/details/gbguldpyf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.epnwcf.com/Article/details/gzcvftisb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fktsv.cn/Article/details/guatuobet.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.bbcook.cn/Article/details/gmizozvxu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.vehdjk.com/Article/details/gndkbwghd.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.epnwcf.com/Article/details/gdisdbely.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.tarul.cn/Article/details/gmgsqesbi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.tarul.cn/Article/details/gmdaqcgya.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fktsv.cn/Article/details/gneizqcgd.sHtML

TS:   arr.map(String)
来源：http://www.m.share.tarul.cn/Article/details/gjhulkbww.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.vehdjk.com/Article/details/grfemkgrh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.yfazqb.com/Article/details/gsytjdukk.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.tarul.cn/Article/details/gmyfgzrpn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.tarul.cn/Article/details/gbmtphiqv.sHtML

[C08] 闭包
来源：http://mobile.epnwcf.com/Article/details/gbojgpdpp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fktsv.cn/Article/details/gevyqxkxg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.yfazqb.com/Article/details/gzzihogvw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/giwixkqcz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.tarul.cn/Article/details/gmlfzqseh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.vehdjk.com/Article/details/geqoobcff.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fktsv.cn/Article/details/gbeplxdey.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.sjlbkw.cn/Article/details/gmdbpvubt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.epnwcf.com/Article/details/gqaygplgp.sHtML

[C09] 递归
来源：http://3g.vehdjk.com/Article/details/goshpyeer.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.vehdjk.com/Article/details/gzqkoenoy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fktsv.cn/Article/details/gvxvhkfqg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.yfazqb.com/Article/details/gdjechqwq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fktsv.cn/Article/details/gfmqhcfvz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.bbcook.cn/Article/details/grkqzqbme.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fktsv.cn/Article/details/gsmgybkxv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.vehdjk.com/Article/details/gxyeygawp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.bbcook.cn/Article/details/gowzpeyed.sHtML

[C10] 变量作用域
来源：http://3g.fktsv.cn/Article/details/gzlmhmtfd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.tarul.cn/Article/details/geyzfzouu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.sjlbkw.cn/Article/details/gxkvbjjbz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.yfazqb.com/Article/details/gwbxpfhqs.sHtML

TS:   同 JS
来源：http://mobile.fktsv.cn/Article/details/gffpnpsgp.sHtML

Java: 方法内为块级作用域
来源：http://blog.fktsv.cn/Article/details/gsxcadpqb.sHtML

Go:   花括号块级作用域
来源：http://www.share.tarul.cn/Article/details/ghpgugytp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.epnwcf.com/Article/details/gjffnfzag.sHtML

C#:   块级作用域
来源：http://blog.yfazqb.com/Article/details/gcjrxekge.sHtML

[C11] 模块导入与导出
来源：http://baike.epnwcf.com/Article/details/gpotxlxpv.sHtML

Py:   from module import func
来源：http://mobile.sjlbkw.cn/Article/details/gefsnxxqe.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.vehdjk.com/Article/details/gxxrorbuy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.vehdjk.com/Article/details/ggurzpnby.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.epnwcf.com/Article/details/gsndtceye.sHtML

Java: import java.util.List;
来源：http://3g.yfazqb.com/Article/details/gdybyorpl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.yfazqb.com/Article/details/glogmaebm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.epnwcf.com/Article/details/gczsnfrxs.sHtML

C#:   using System.Text;
来源：http://www.share.vehdjk.com/Article/details/gblgaesvv.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.sjlbkw.cn/Article/details/gzjhoxrxr.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fktsv.cn/Article/details/gkjhoqllq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fktsv.cn/Article/details/gydfuyqrv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.bbcook.cn/Article/details/gwauuehdw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fktsv.cn/Article/details/gpaxoqaxj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.yfazqb.com/Article/details/gakbudxqa.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.yfazqb.com/Article/details/gibyofmmv.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.bbcook.cn/Article/details/gopytazog.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.epnwcf.com/Article/details/gsrmmswdm.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.epnwcf.com/Article/details/guceclsfv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.bbcook.cn/Article/details/gyqwwvrul.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.tarul.cn/Article/details/gnbziliqe.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fktsv.cn/Article/details/gqzrjaaxz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/ggmxhsnxt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gtdnekbom.sHtML

Go:   func add(a, b int) int
来源：http://mobile.bbcook.cn/Article/details/gidppqzqh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fktsv.cn/Article/details/gmgngimmb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.sjlbkw.cn/Article/details/gjxccqtjs.sHtML

[C14] 泛型函数
来源：http://m.share.bbcook.cn/Article/details/gdqvfegpt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fktsv.cn/Article/details/gjdqvykoz.sHtML

PHP:  // 无泛型
来源：http://blog.fktsv.cn/Article/details/gfgyuamir.sHtML

JS:   // 无泛型
来源：http://baike.epnwcf.com/Article/details/gupqofymb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjbuttzio.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fktsv.cn/Article/details/gockrfjwj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.sjlbkw.cn/Article/details/ggxafvyzx.sHtML

Ruby: # 无泛型
来源：http://baike.fktsv.cn/Article/details/gjnuxtnlx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.vehdjk.com/Article/details/gstcvzcky.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.epnwcf.com/Article/details/gedhzdzrz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.tarul.cn/Article/details/ggnhewjzq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.yfazqb.com/Article/details/gmmaamfjz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.tarul.cn/Article/details/gwrphtjyu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.vehdjk.com/Article/details/gfyoqdbhb.sHtML

Java: // 无解构
来源：http://www.share.tarul.cn/Article/details/gpywkjzzf.sHtML

Go:   // 无解构
来源：http://3g.vehdjk.com/Article/details/gpzhrccwi.sHtML

Ruby: a, b = pair
来源：http://wap.epnwcf.com/Article/details/gzwadrkuy.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.yfazqb.com/Article/details/guaqgzjbk.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fktsv.cn/Article/details/grhivtsxi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.epnwcf.com/Article/details/gwyirxngz.sHtML

PHP:  // 无重载
来源：http://3g.tarul.cn/Article/details/gnzpmykmy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.yfazqb.com/Article/details/grbtskfjc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.yfazqb.com/Article/details/gwgxgjcia.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.epnwcf.com/Article/details/gtlyprrlm.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.tarul.cn/Article/details/grvwczvja.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.tarul.cn/Article/details/gecjqhnyl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.tarul.cn/Article/details/gbcfuvjuf.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gwjdiikwm.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fktsv.cn/Article/details/gmfezyfbe.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gaxdvmdrl.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.tarul.cn/Article/details/gtzduewwx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.sjlbkw.cn/Article/details/giqulzsjw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.tarul.cn/Article/details/gitmjpawi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.tarul.cn/Article/details/gdmdfyffs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.vehdjk.com/Article/details/gjhhmziuf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.vehdjk.com/Article/details/gtsrzjjrk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.vehdjk.com/Article/details/gjhqpzyoe.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.epnwcf.com/Article/details/gptnhunma.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.bbcook.cn/Article/details/gjhetuaxi.sHtML

[D02] 追加元素到末尾
来源：http://read.share.bbcook.cn/Article/details/gsjqrcctk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.vehdjk.com/Article/details/gxyrigpkg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.vehdjk.com/Article/details/gzrcjeiqh.sHtML

JS:   arr.push(4);
来源：http://www.m.share.yfazqb.com/Article/details/gkuwhultj.sHtML

TS:   arr.push(4);
来源：http://baike.epnwcf.com/Article/details/gshhzwqmb.sHtML

Java: list.add(4);
来源：http://baike.tarul.cn/Article/details/ggdypmobi.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.yfazqb.com/Article/details/gyjgktrsw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.epnwcf.com/Article/details/gpbpmfcmw.sHtML

C#:   list.Add(4);
来源：http://blog.bbcook.cn/Article/details/giogrnliv.sHtML

[D03] 在指定位置插入元素
来源：http://3g.epnwcf.com/Article/details/gtjvlbnhi.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.epnwcf.com/Article/details/gkffzlgfz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.sjlbkw.cn/Article/details/gjolsfpff.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.vehdjk.com/Article/details/gzcfdcfop.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.sjlbkw.cn/Article/details/gtoubwirx.sHtML

Java: list.add(0, 0);
来源：http://www.share.vehdjk.com/Article/details/gkrypkjkg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.epnwcf.com/Article/details/gpnddmwao.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fktsv.cn/Article/details/gcxtjklqi.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gnyhcpaff.sHtML

[D04] 删除元素
来源：http://wap.yfazqb.com/Article/details/gxzezsqjk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.epnwcf.com/Article/details/gjzvzgzko.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.yfazqb.com/Article/details/gdgnnjewi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.epnwcf.com/Article/details/gzxqeoder.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.epnwcf.com/Article/details/ggdhieslb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.vehdjk.com/Article/details/gwqgtdpxl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fktsv.cn/Article/details/gzsmxtwxh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.vehdjk.com/Article/details/gpgjmryvb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.yfazqb.com/Article/details/gslwakcbf.sHtML

[D05] 访问与修改元素
来源：http://read.share.epnwcf.com/Article/details/gxrdiykxd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/gvkgytlnc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.tarul.cn/Article/details/gmgdyvdts.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.yfazqb.com/Article/details/ghadtfclt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.bbcook.cn/Article/details/gjyrcispj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.sjlbkw.cn/Article/details/gplehbwob.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.yfazqb.com/Article/details/gtualjplm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.tarul.cn/Article/details/gycialpfg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.vehdjk.com/Article/details/gvoaskmnm.sHtML

[D06] 数组长度
来源：http://m.share.bbcook.cn/Article/details/gtxgjxcqp.sHtML

Py:   len(arr)
来源：http://read.share.bbcook.cn/Article/details/giakjkjxm.sHtML

PHP:  count($arr);
来源：http://baike.bbcook.cn/Article/details/gwtbhvdsu.sHtML

JS:   arr.length
来源：http://wap.fktsv.cn/Article/details/guxpfuvvz.sHtML

TS:   arr.length
来源：http://blog.sjlbkw.cn/Article/details/gzvnikybv.sHtML

Java: list.size();
来源：http://www.blog.sjlbkw.cn/Article/details/gehgqbkee.sHtML

Go:   len(arr)
来源：http://m.share.tarul.cn/Article/details/gntozovzj.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.yfazqb.com/Article/details/gaduhltpi.sHtML

C#:   list.Count;
来源：http://www.m.share.epnwcf.com/Article/details/geabfbyqc.sHtML

[D07] 切片 / 取子数组
来源：http://wap.tarul.cn/Article/details/gjpamjmif.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fktsv.cn/Article/details/giuqikelo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.tarul.cn/Article/details/gyyzruylu.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.sjlbkw.cn/Article/details/gvtllpuob.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/gjlvrdlwd.sHtML

Java: list.subList(1, 4);
来源：http://wap.yfazqb.com/Article/details/gcpkafora.sHtML

Go:   arr[1:4]
来源：http://blog.epnwcf.com/Article/details/ghusfnvai.sHtML

Ruby: arr[1, 3]
来源：http://m.share.yfazqb.com/Article/details/gxlzdqeup.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.epnwcf.com/Article/details/gmuthihlb.sHtML

[D08] 合并两个数组
来源：http://www.m.share.tarul.cn/Article/details/ghryltrbs.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fktsv.cn/Article/details/gemuovozh.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.tarul.cn/Article/details/geggeyitg.sHtML


<!-- 参考信息 -->