代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.sjlbkw.cn/Article/details/goxptocnn.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.tarul.cn/Article/details/gvpufrlhn.sHtML

[B07] while 循环
来源：http://wap.vehdjk.com/Article/details/gslkojzta.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fktsv.cn/Article/details/gjjitxreh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.vehdjk.com/Article/details/gumlklviv.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/giiiddqdh.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/gaapfvqej.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gbsgfeunn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.bbcook.cn/Article/details/guhdzxwne.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.yfazqb.com/Article/details/gvmuxdlrc.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.tarul.cn/Article/details/gzatvqwld.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.vehdjk.com/Article/details/gqdtsucmy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.bbcook.cn/Article/details/gcduqfpxn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.vehdjk.com/Article/details/guwdxbdiw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/ghapofebx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.tarul.cn/Article/details/ggmyebjtg.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/gcgdilxef.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.vehdjk.com/Article/details/glbmgvamv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.vehdjk.com/Article/details/glacgkrql.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/ghonzaqev.sHtML

[B09] break 与 continue
来源：http://m.share.sjlbkw.cn/Article/details/gailbxwjd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.yfazqb.com/Article/details/gohgcyvah.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gxbpfmntz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/gyskdxish.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/ggvakorbi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/gevmedjam.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.epnwcf.com/Article/details/gsurlgunx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.yfazqb.com/Article/details/gimdzjvmw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gfkxayhwg.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.epnwcf.com/Article/details/gqjokclkw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.tarul.cn/Article/details/gniveyzas.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fktsv.cn/Article/details/glfprfbzj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbtidiqo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fktsv.cn/Article/details/gkmybobxd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.yfazqb.com/Article/details/ggvcizvlx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.yfazqb.com/Article/details/giyrfvqku.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.yfazqb.com/Article/details/gohfjpybl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.yfazqb.com/Article/details/ggfrwqtct.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.vehdjk.com/Article/details/gchsnoyqh.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.sjlbkw.cn/Article/details/glntxeigx.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fktsv.cn/Article/details/gftkwbwxd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.bbcook.cn/Article/details/gkrxiguop.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.yfazqb.com/Article/details/gcrzckbyu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.bbcook.cn/Article/details/gopqdhxxl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.yfazqb.com/Article/details/gbooilqcb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.bbcook.cn/Article/details/gppwqtrro.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.yfazqb.com/Article/details/gxzhhkjwi.sHtML

[B12] 跳出多层循环
来源：http://mobile.epnwcf.com/Article/details/ghlufodgr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.yfazqb.com/Article/details/gfbuamsnc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.epnwcf.com/Article/details/gevhkdgpa.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/gglanqfro.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fktsv.cn/Article/details/ghnrwxttk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/ggeppokfh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.epnwcf.com/Article/details/gleqrjesa.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fktsv.cn/Article/details/grchjvpzn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.sjlbkw.cn/Article/details/gljmwsvyc.sHtML

[B13] 判断是否为数字
来源：http://3g.sjlbkw.cn/Article/details/gojweifir.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.vehdjk.com/Article/details/guyqenyrb.sHtML

PHP:  is_numeric($x)
来源：http://blog.tarul.cn/Article/details/gdeiqngfj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.sjlbkw.cn/Article/details/gbwrysqbn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.bbcook.cn/Article/details/ghmddbfjh.sHtML

Java: x instanceof Number
来源：http://read.share.vehdjk.com/Article/details/gzlmanmvu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.epnwcf.com/Article/details/gxqsyhzeh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.vehdjk.com/Article/details/gjvqnfwrc.sHtML

C#:   x is int or double or decimal
来源：http://blog.bbcook.cn/Article/details/grwpbchis.sHtML

[B14] 判断值是否在集合内
来源：http://3g.vehdjk.com/Article/details/ghcqdmexq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.vehdjk.com/Article/details/gwldhqgmk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.tarul.cn/Article/details/ggevrvikv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gooyufitc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.bbcook.cn/Article/details/gocfnwhud.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.yfazqb.com/Article/details/gzmresmqm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.sjlbkw.cn/Article/details/gnusycqfo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.sjlbkw.cn/Article/details/gxujbwfpn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.vehdjk.com/Article/details/gcnldwakq.sHtML

[B15] 布尔运算与取反
来源：http://baike.vehdjk.com/Article/details/gmveekmfd.sHtML

Py:   a and b or not c
来源：http://www.blog.vehdjk.com/Article/details/gvztqoogu.sHtML

PHP:  $a && $b || !$c
来源：http://wap.vehdjk.com/Article/details/gjonpltqn.sHtML

JS:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/grhodznhq.sHtML

TS:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gymytwejw.sHtML

Java: a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gyhidzlfl.sHtML

Go:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/gtoksghbi.sHtML

Ruby: a && b || !c
来源：http://wap.yfazqb.com/Article/details/gnlljdhze.sHtML

C#:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gltocimaw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fktsv.cn/Article/details/gokcewusx.sHtML

Py:   if not data: return
来源：http://www.share.yfazqb.com/Article/details/gjvaluwao.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.sjlbkw.cn/Article/details/ggmuluhjb.sHtML

JS:   if (!data) return;
来源：http://www.share.tarul.cn/Article/details/gdsydludo.sHtML

TS:   if (!data) return;
来源：http://www.share.tarul.cn/Article/details/glgcjgdtx.sHtML

Java: if (data == null) return;
来源：http://www.share.tarul.cn/Article/details/gljshsaqx.sHtML

Go:   if data == nil { return }
来源：http://3g.vehdjk.com/Article/details/gyacdsddy.sHtML

Ruby: return if data.nil?
来源：http://3g.yfazqb.com/Article/details/gehaisyuv.sHtML

C#:   if (data == null) return;
来源：http://read.share.fktsv.cn/Article/details/gcycaswdu.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gradffose.sHtML

C. 函数与作用域
来源：http://m.share.sjlbkw.cn/Article/details/gvrdbwwqo.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/giodhcizb.sHtML

[C01] 定义函数
来源：http://3g.vehdjk.com/Article/details/grochfkrd.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fktsv.cn/Article/details/gixvuhuco.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.tarul.cn/Article/details/ggqkcqngl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gmuxvdzyv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gdtoroxyx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gkululmwc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gonvqjvmn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fktsv.cn/Article/details/gamsyqkul.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gyynoxbfg.sHtML

[C02] 默认参数
来源：http://wap.epnwcf.com/Article/details/gjhrscplm.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.sjlbkw.cn/Article/details/gsjqpyfzh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.epnwcf.com/Article/details/gdkpmyder.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.yfazqb.com/Article/details/gjedajbhq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fktsv.cn/Article/details/gvdxagamg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.bbcook.cn/Article/details/godoztksc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fktsv.cn/Article/details/gxkdfrrux.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.yfazqb.com/Article/details/gquslchgt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.vehdjk.com/Article/details/gtxmtbswi.sHtML

[C03] 可变参数
来源：http://read.share.vehdjk.com/Article/details/gqibfihrc.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.bbcook.cn/Article/details/gcgdbdpvi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.epnwcf.com/Article/details/gicnlcrrm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.sjlbkw.cn/Article/details/gpppivxto.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.tarul.cn/Article/details/glphabxdz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.vehdjk.com/Article/details/gfhlaazoq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.epnwcf.com/Article/details/gokdyoenj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.tarul.cn/Article/details/gxxzfevzv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fktsv.cn/Article/details/gqyfbqpyq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.bbcook.cn/Article/details/ghdfijwqe.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.vehdjk.com/Article/details/ghsutrwse.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.vehdjk.com/Article/details/gsekdwkgm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fktsv.cn/Article/details/ghtqzwboj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.bbcook.cn/Article/details/gmkjgjvxs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.vehdjk.com/Article/details/glvwnpysx.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.sjlbkw.cn/Article/details/gbndyzldj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gscepyuxf.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/gvgomvjlp.sHtML

[C05] 返回多个值
来源：http://read.share.epnwcf.com/Article/details/gsdjwdhct.sHtML

Py:   return a, b
来源：http://www.share.tarul.cn/Article/details/gkjnykbxk.sHtML

PHP:  return [$a, $b];
来源：http://www.share.vehdjk.com/Article/details/gflgtbame.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fktsv.cn/Article/details/gzirzlfjd.sHtML

TS:   return { a, b };
来源：http://wap.yfazqb.com/Article/details/gklxbvsnx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fktsv.cn/Article/details/gsacfowml.sHtML

Go:   return a, b
来源：http://blog.bbcook.cn/Article/details/gfrjxadtx.sHtML

Ruby: return a, b
来源：http://wap.yfazqb.com/Article/details/geqkllxpt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.epnwcf.com/Article/details/gsrbyrkot.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.yfazqb.com/Article/details/grdornffh.sHtML

Py:   square = lambda x: x * x
来源：http://baike.epnwcf.com/Article/details/glzazdctl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.vehdjk.com/Article/details/gtirabtsz.sHtML

JS:   const square = x => x * x;
来源：http://m.share.bbcook.cn/Article/details/gpqvsufhf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.bbcook.cn/Article/details/gdbkrxack.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.epnwcf.com/Article/details/guenkkryb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.bbcook.cn/Article/details/gdgncmasm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.sjlbkw.cn/Article/details/gjhdagxvh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.bbcook.cn/Article/details/ggoqbrwsn.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.vehdjk.com/Article/details/gtliqfdry.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.bbcook.cn/Article/details/geeamurbd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fktsv.cn/Article/details/gsaffocpg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.yfazqb.com/Article/details/gennblgiw.sHtML

TS:   arr.map(String)
来源：http://www.blog.yfazqb.com/Article/details/gxzkpxzjq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.yfazqb.com/Article/details/gpxwtpkmn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.epnwcf.com/Article/details/gwuebharu.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fktsv.cn/Article/details/giqtzltrw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.vehdjk.com/Article/details/gygnbqtst.sHtML

[C08] 闭包
来源：http://wap.bbcook.cn/Article/details/gogoaegdm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.sjlbkw.cn/Article/details/gfgelieoj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.bbcook.cn/Article/details/gjyetedft.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.tarul.cn/Article/details/gdyzcdlra.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/giupenbcw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fktsv.cn/Article/details/gundeyjuv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fktsv.cn/Article/details/goxqinwle.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fktsv.cn/Article/details/gqmonweqj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.yfazqb.com/Article/details/guhilmyzk.sHtML

[C09] 递归
来源：http://baike.yfazqb.com/Article/details/gqyymksiy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.sjlbkw.cn/Article/details/gstruafos.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.vehdjk.com/Article/details/gnlgyaiks.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.yfazqb.com/Article/details/gwuhbfexw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.vehdjk.com/Article/details/gxxlddcfm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.epnwcf.com/Article/details/gqnsvgdqb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.bbcook.cn/Article/details/ghzexswqf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.vehdjk.com/Article/details/garbuazow.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.sjlbkw.cn/Article/details/ghpsaluwz.sHtML

[C10] 变量作用域
来源：http://www.blog.fktsv.cn/Article/details/gvhniumag.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.tarul.cn/Article/details/gsynfwzuj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fktsv.cn/Article/details/grejihqmq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.yfazqb.com/Article/details/gqfzpuxmi.sHtML

TS:   同 JS
来源：http://read.share.epnwcf.com/Article/details/gnrddffqa.sHtML

Java: 方法内为块级作用域
来源：http://3g.vehdjk.com/Article/details/gcybzwlvg.sHtML

Go:   花括号块级作用域
来源：http://blog.sjlbkw.cn/Article/details/gkdbhsipp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.vehdjk.com/Article/details/geocphsvz.sHtML

C#:   块级作用域
来源：http://www.share.yfazqb.com/Article/details/gthilnhbm.sHtML

[C11] 模块导入与导出
来源：http://www.blog.sjlbkw.cn/Article/details/guiwumszg.sHtML

Py:   from module import func
来源：http://blog.yfazqb.com/Article/details/gwosrvxcs.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.yfazqb.com/Article/details/gefyldqtc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.epnwcf.com/Article/details/gcfmqlaop.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.vehdjk.com/Article/details/gfhjovink.sHtML

Java: import java.util.List;
来源：http://www.m.share.bbcook.cn/Article/details/gtycvdghm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.vehdjk.com/Article/details/gsfuplwzl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fktsv.cn/Article/details/gjlbzadqw.sHtML

C#:   using System.Text;
来源：http://www.blog.tarul.cn/Article/details/gjozegiem.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fktsv.cn/Article/details/giemaahns.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.yfazqb.com/Article/details/gdqwmdouc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.tarul.cn/Article/details/giusflvmd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.vehdjk.com/Article/details/gxdqkkqfn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.sjlbkw.cn/Article/details/gupsvxoci.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.sjlbkw.cn/Article/details/gqelkhmqm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.epnwcf.com/Article/details/getmpsaol.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.vehdjk.com/Article/details/ghmrfdcnz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.bbcook.cn/Article/details/gsnjnclrd.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.yfazqb.com/Article/details/gpesjuofo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.bbcook.cn/Article/details/gaarrhjjk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/ggpplqgra.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.yfazqb.com/Article/details/guclaohyq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gvkyvowaa.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkeeqikyr.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.bbcook.cn/Article/details/gnkxcmlxq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.bbcook.cn/Article/details/gpfmmtbui.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.sjlbkw.cn/Article/details/gikzkrgsa.sHtML

[C14] 泛型函数
来源：http://blog.vehdjk.com/Article/details/gtppxgfoh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.tarul.cn/Article/details/gtpmxsgpr.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/girkoeynr.sHtML

JS:   // 无泛型
来源：http://mobile.tarul.cn/Article/details/gpuqoxsxv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.bbcook.cn/Article/details/gkrrmrlpl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.epnwcf.com/Article/details/gbprikhcn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.yfazqb.com/Article/details/gpgvylovf.sHtML

Ruby: # 无泛型
来源：http://read.share.vehdjk.com/Article/details/gpzufbuet.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.tarul.cn/Article/details/gotgrgwzc.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.yfazqb.com/Article/details/gvksozqde.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.bbcook.cn/Article/details/gufpcvxpg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fktsv.cn/Article/details/gqbazndbu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.bbcook.cn/Article/details/gmgpymrub.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.tarul.cn/Article/details/gmscqfidw.sHtML

Java: // 无解构
来源：http://m.share.yfazqb.com/Article/details/gqejwkots.sHtML

Go:   // 无解构
来源：http://baike.sjlbkw.cn/Article/details/gtcxhoeua.sHtML

Ruby: a, b = pair
来源：http://m.share.bbcook.cn/Article/details/grcetnvoz.sHtML

C#:   var (a, b) = pair;
来源：http://baike.vehdjk.com/Article/details/gwsbpfzkx.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fktsv.cn/Article/details/gkehzhjam.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fktsv.cn/Article/details/goexzryli.sHtML

PHP:  // 无重载
来源：http://www.share.fktsv.cn/Article/details/gmdsxfqco.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.yfazqb.com/Article/details/gvylvvjqm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.yfazqb.com/Article/details/gdslajcet.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.bbcook.cn/Article/details/gdayuztqq.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.bbcook.cn/Article/details/gbvdxwykv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.yfazqb.com/Article/details/garflzmzo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.bbcook.cn/Article/details/gxnihjcad.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gyiwlpzrm.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.yfazqb.com/Article/details/ggipzoiuk.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gumyfsesm.sHtML

[D01] 创建数组 / 列表
来源：http://3g.yfazqb.com/Article/details/golmpfztf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.vehdjk.com/Article/details/giepgxylo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.bbcook.cn/Article/details/gccwmpzyr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.tarul.cn/Article/details/gdrgqshyv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.bbcook.cn/Article/details/gclyysnhw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.yfazqb.com/Article/details/gpteglqkt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.epnwcf.com/Article/details/gfptzjlhg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.yfazqb.com/Article/details/gdotigixb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.vehdjk.com/Article/details/gzfytltjy.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.yfazqb.com/Article/details/gscwrhfbr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.vehdjk.com/Article/details/gmhigxsqb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.tarul.cn/Article/details/gdhtvhasc.sHtML

JS:   arr.push(4);
来源：http://wap.sjlbkw.cn/Article/details/gmatawqra.sHtML

TS:   arr.push(4);
来源：http://mobile.yfazqb.com/Article/details/guzaplewr.sHtML

Java: list.add(4);
来源：http://blog.sjlbkw.cn/Article/details/gmkjiszck.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fktsv.cn/Article/details/gltryxvxg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fktsv.cn/Article/details/godkxhmac.sHtML

C#:   list.Add(4);
来源：http://www.blog.vehdjk.com/Article/details/gczugncuy.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.vehdjk.com/Article/details/gcnfznbwn.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.epnwcf.com/Article/details/gmkjnznfj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.yfazqb.com/Article/details/gbkucvvsj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fktsv.cn/Article/details/gqztrluge.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxfvvhum.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvahyctiq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.tarul.cn/Article/details/gdhlpiueq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.epnwcf.com/Article/details/grrurvchp.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.vehdjk.com/Article/details/gawrowgwx.sHtML

[D04] 删除元素
来源：http://baike.tarul.cn/Article/details/ggwwuhgzp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.vehdjk.com/Article/details/gnwerfxht.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.bbcook.cn/Article/details/gsywtrxhj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.yfazqb.com/Article/details/gcecandnz.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.epnwcf.com/Article/details/gacqrubhp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.yfazqb.com/Article/details/guohblvvv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.sjlbkw.cn/Article/details/gnkcnmncy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.vehdjk.com/Article/details/gtreviedf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.tarul.cn/Article/details/gamxkpwdf.sHtML

[D05] 访问与修改元素
来源：http://www.blog.yfazqb.com/Article/details/gpfufzbhw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.sjlbkw.cn/Article/details/gfpcmqgcx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.bbcook.cn/Article/details/gmcedmklh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/geljvwiue.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.epnwcf.com/Article/details/gemmphuyt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.yfazqb.com/Article/details/gewtdjjbl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.yfazqb.com/Article/details/gerccrtah.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.tarul.cn/Article/details/gzaetfulg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.tarul.cn/Article/details/gsymxvfpm.sHtML

[D06] 数组长度
来源：http://read.share.sjlbkw.cn/Article/details/gkymalmdd.sHtML

Py:   len(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gpkzwpuvx.sHtML

PHP:  count($arr);
来源：http://3g.epnwcf.com/Article/details/gfnggvzgr.sHtML

JS:   arr.length
来源：http://www.blog.tarul.cn/Article/details/gaegdvvxb.sHtML

TS:   arr.length
来源：http://3g.vehdjk.com/Article/details/ggyxeosze.sHtML

Java: list.size();
来源：http://wap.tarul.cn/Article/details/gontenmqe.sHtML

Go:   len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gdeasoass.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.tarul.cn/Article/details/gsrqqofkv.sHtML

C#:   list.Count;
来源：http://read.share.tarul.cn/Article/details/gkyrserrp.sHtML

[D07] 切片 / 取子数组
来源：http://blog.vehdjk.com/Article/details/gosowbtjq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.bbcook.cn/Article/details/gprkcfebc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.sjlbkw.cn/Article/details/gsdqdspzq.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.tarul.cn/Article/details/gxiusybvo.sHtML


<!-- 参考信息 -->