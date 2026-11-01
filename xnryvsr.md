代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.tarul.cn/Article/details/genrwexfv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.epnwcf.com/Article/details/gwtllscsd.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.vehdjk.com/Article/details/gvjsolheh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.vehdjk.com/Article/details/gqvoujrad.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.sjlbkw.cn/Article/details/gkvzfdrrv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.bbcook.cn/Article/details/gzfonofpf.sHtML

[B07] while 循环
来源：http://mobile.vehdjk.com/Article/details/gwfufzqxp.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.tarul.cn/Article/details/gbgzeiooq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.epnwcf.com/Article/details/gnbxibdhd.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gxkywjoql.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.epnwcf.com/Article/details/grpdskhnp.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gofbdgxzd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.tarul.cn/Article/details/gqtriifpx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.vehdjk.com/Article/details/ginhodghf.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/guiijeugp.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.vehdjk.com/Article/details/gnpdvgmew.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.epnwcf.com/Article/details/gpothkjye.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.bbcook.cn/Article/details/gnkzaoyby.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.tarul.cn/Article/details/glitytfic.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gdwiwucci.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fktsv.cn/Article/details/ggejqyqgd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.epnwcf.com/Article/details/gxopnlhzk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.bbcook.cn/Article/details/ggkozclbz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fktsv.cn/Article/details/gqnvyqnrg.sHtML

[B09] break 与 continue
来源：http://3g.bbcook.cn/Article/details/ghpunlozp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.yfazqb.com/Article/details/gtvaakwtw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gcimhrgbz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/glanpxzvh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/gzxpknomy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gleeulvvk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.bbcook.cn/Article/details/gwtkwugrm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.vehdjk.com/Article/details/gxmzogyjr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gxamtfgng.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.epnwcf.com/Article/details/gfospnzql.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.bbcook.cn/Article/details/gfbtlpbvr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.bbcook.cn/Article/details/gsztifoal.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fktsv.cn/Article/details/gedtezqer.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.epnwcf.com/Article/details/gylejwzns.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.epnwcf.com/Article/details/gcenuitmw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.sjlbkw.cn/Article/details/gdfbzivpf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fktsv.cn/Article/details/gohgnfuvu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.bbcook.cn/Article/details/gfmldqsza.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.sjlbkw.cn/Article/details/gxcjnztfr.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.epnwcf.com/Article/details/gypyqkvzq.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.epnwcf.com/Article/details/gvomrrcpm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.vehdjk.com/Article/details/gvcxcnwmc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.vehdjk.com/Article/details/gxqizehfl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.yfazqb.com/Article/details/gwkwywgsf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.vehdjk.com/Article/details/gnxkavwrg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.yfazqb.com/Article/details/gbstvrrhb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.yfazqb.com/Article/details/grjpcdwgu.sHtML

[B12] 跳出多层循环
来源：http://mobile.epnwcf.com/Article/details/gblryeixl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.yfazqb.com/Article/details/gnuwqzcsl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.yfazqb.com/Article/details/gftutwnbo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/gvodcblzg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/glheiunae.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/gvtgcbbkw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.tarul.cn/Article/details/gprucdsud.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.tarul.cn/Article/details/galvvcjqy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.vehdjk.com/Article/details/gouyzvset.sHtML

[B13] 判断是否为数字
来源：http://mobile.tarul.cn/Article/details/gfyiqqnrl.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.tarul.cn/Article/details/gjozijapl.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.vehdjk.com/Article/details/gvfdcutpm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.epnwcf.com/Article/details/gwyhvvmtr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.epnwcf.com/Article/details/glrjxhubl.sHtML

Java: x instanceof Number
来源：http://read.share.epnwcf.com/Article/details/gidgoxxat.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.tarul.cn/Article/details/ghtmprybe.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fktsv.cn/Article/details/gfzdwphbc.sHtML

C#:   x is int or double or decimal
来源：http://read.share.vehdjk.com/Article/details/gpvapjhbm.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.vehdjk.com/Article/details/gojukfxic.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.yfazqb.com/Article/details/gnmxpxmfn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.bbcook.cn/Article/details/gjdwcwfxd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.bbcook.cn/Article/details/gjgbloxfs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.vehdjk.com/Article/details/gpbocdobi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gwmpsrruo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.vehdjk.com/Article/details/gnkrzrint.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.bbcook.cn/Article/details/gnpxokbbj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.vehdjk.com/Article/details/gbxidrejz.sHtML

[B15] 布尔运算与取反
来源：http://m.share.epnwcf.com/Article/details/gswpazkbb.sHtML

Py:   a and b or not c
来源：http://www.m.share.yfazqb.com/Article/details/ggzjrsmli.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.sjlbkw.cn/Article/details/gbikuxhkh.sHtML

JS:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gbafjdhkn.sHtML

TS:   a && b || !c
来源：http://mobile.yfazqb.com/Article/details/ggvpkhsty.sHtML

Java: a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gjutgfiet.sHtML

Go:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/gqdgxzhgd.sHtML

Ruby: a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gavqcombk.sHtML

C#:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gglhftbxm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.yfazqb.com/Article/details/gxnizztdf.sHtML

Py:   if not data: return
来源：http://www.blog.bbcook.cn/Article/details/gtcojkhqs.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fktsv.cn/Article/details/gvgtkhhdb.sHtML

JS:   if (!data) return;
来源：http://blog.epnwcf.com/Article/details/gjlzdwuuh.sHtML

TS:   if (!data) return;
来源：http://blog.vehdjk.com/Article/details/gljypqixt.sHtML

Java: if (data == null) return;
来源：http://3g.yfazqb.com/Article/details/gvonsmdcg.sHtML

Go:   if data == nil { return }
来源：http://mobile.sjlbkw.cn/Article/details/gomjovtvx.sHtML

Ruby: return if data.nil?
来源：http://blog.tarul.cn/Article/details/golozdvpu.sHtML

C#:   if (data == null) return;
来源：http://mobile.tarul.cn/Article/details/ghucjdekm.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gdlriqbhi.sHtML

C. 函数与作用域
来源：http://mobile.bbcook.cn/Article/details/gmjpssdjl.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/ghjzoljhw.sHtML

[C01] 定义函数
来源：http://blog.epnwcf.com/Article/details/gohfovfmi.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.sjlbkw.cn/Article/details/grnsfgloe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gmqqofyec.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/goemobomb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.tarul.cn/Article/details/gmggryxjx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gktqdcaxu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.yfazqb.com/Article/details/ggsczbgpk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.tarul.cn/Article/details/gexyvjzql.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gebnxphpl.sHtML

[C02] 默认参数
来源：http://wap.fktsv.cn/Article/details/gospkcwkn.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.vehdjk.com/Article/details/gucgpeimm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fktsv.cn/Article/details/gkenrsekg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.vehdjk.com/Article/details/gfwdtwdam.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gwwtkzbfx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.bbcook.cn/Article/details/gsgfisqgd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.sjlbkw.cn/Article/details/gsnrxszbx.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.tarul.cn/Article/details/gkcotrsph.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.yfazqb.com/Article/details/gluipfapb.sHtML

[C03] 可变参数
来源：http://mobile.vehdjk.com/Article/details/gykkhcbab.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.tarul.cn/Article/details/gukdaolxs.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.sjlbkw.cn/Article/details/gboailigr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.vehdjk.com/Article/details/gbsrqfaqm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fktsv.cn/Article/details/gwwzijegc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.bbcook.cn/Article/details/gmjphifhj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.bbcook.cn/Article/details/gemknhpyj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.yfazqb.com/Article/details/gaihxqfdn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.sjlbkw.cn/Article/details/ghbuoanqi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fktsv.cn/Article/details/gfwzzditk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.vehdjk.com/Article/details/godrgefmq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.epnwcf.com/Article/details/gyugmlxqf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.vehdjk.com/Article/details/gxexiguwv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.bbcook.cn/Article/details/gcyvmlaeb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.bbcook.cn/Article/details/grzmxzmxm.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.yfazqb.com/Article/details/gcvwpmmdd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fktsv.cn/Article/details/gvseutsis.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fktsv.cn/Article/details/gpxmkhogy.sHtML

[C05] 返回多个值
来源：http://wap.epnwcf.com/Article/details/gmdabizqa.sHtML

Py:   return a, b
来源：http://3g.tarul.cn/Article/details/gloemojqd.sHtML

PHP:  return [$a, $b];
来源：http://baike.fktsv.cn/Article/details/gqbtkbeyx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.vehdjk.com/Article/details/gyeveyulo.sHtML

TS:   return { a, b };
来源：http://wap.vehdjk.com/Article/details/gjqobjtab.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fktsv.cn/Article/details/gbqszscwp.sHtML

Go:   return a, b
来源：http://wap.tarul.cn/Article/details/gzswgezof.sHtML

Ruby: return a, b
来源：http://www.share.yfazqb.com/Article/details/gwjenfiae.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.sjlbkw.cn/Article/details/grjlktmyf.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.vehdjk.com/Article/details/gwnoystvz.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.tarul.cn/Article/details/gglgbthcd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fktsv.cn/Article/details/gpvxnhhsx.sHtML

JS:   const square = x => x * x;
来源：http://baike.sjlbkw.cn/Article/details/gqzsxncea.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.yfazqb.com/Article/details/gipiretjp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fktsv.cn/Article/details/gcxnogoap.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.epnwcf.com/Article/details/gsnswfacr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.tarul.cn/Article/details/gbxljdjkc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.sjlbkw.cn/Article/details/gtrodyncl.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.vehdjk.com/Article/details/gveqpolnu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.epnwcf.com/Article/details/guzcwikzz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.vehdjk.com/Article/details/gkklmtvyd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.epnwcf.com/Article/details/gkpybrbyl.sHtML

TS:   arr.map(String)
来源：http://baike.tarul.cn/Article/details/guijxtfjc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.bbcook.cn/Article/details/giochrkqy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.sjlbkw.cn/Article/details/gfcsegltn.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.epnwcf.com/Article/details/gsqtkyigj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.vehdjk.com/Article/details/gzhuykzqh.sHtML

[C08] 闭包
来源：http://wap.fktsv.cn/Article/details/gffxgkfqz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.bbcook.cn/Article/details/gmzpgklia.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fktsv.cn/Article/details/gnebsvvmf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.bbcook.cn/Article/details/gqvjltlmv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.bbcook.cn/Article/details/gxmvzwape.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.vehdjk.com/Article/details/gqwbcovzb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.yfazqb.com/Article/details/gfnwlfcjf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.yfazqb.com/Article/details/guowopnga.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fktsv.cn/Article/details/gsxhnvkgl.sHtML

[C09] 递归
来源：http://mobile.tarul.cn/Article/details/gtgqnhvvv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.vehdjk.com/Article/details/gpuabagun.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.tarul.cn/Article/details/gbsqtjzeu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.bbcook.cn/Article/details/gepzuuhnr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.bbcook.cn/Article/details/gulfqtbai.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.bbcook.cn/Article/details/gzvykmuao.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.vehdjk.com/Article/details/grbdrzdax.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/gzfxkbaxl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.vehdjk.com/Article/details/giszyxauv.sHtML

[C10] 变量作用域
来源：http://3g.tarul.cn/Article/details/ggqaunxrs.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.sjlbkw.cn/Article/details/gsjrluwee.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.epnwcf.com/Article/details/gblxiymdh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.epnwcf.com/Article/details/gvamcymua.sHtML

TS:   同 JS
来源：http://read.share.yfazqb.com/Article/details/gfhacxiro.sHtML

Java: 方法内为块级作用域
来源：http://mobile.bbcook.cn/Article/details/ghyorwjla.sHtML

Go:   花括号块级作用域
来源：http://www.share.vehdjk.com/Article/details/gszpxjxat.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.tarul.cn/Article/details/gnargmyct.sHtML

C#:   块级作用域
来源：http://wap.vehdjk.com/Article/details/gvhaldkjz.sHtML

[C11] 模块导入与导出
来源：http://blog.fktsv.cn/Article/details/gzjfptmri.sHtML

Py:   from module import func
来源：http://read.share.bbcook.cn/Article/details/gkqwbqwkq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.yfazqb.com/Article/details/ghaazvazs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.bbcook.cn/Article/details/gydqnrtpy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.sjlbkw.cn/Article/details/gltdjflyx.sHtML

Java: import java.util.List;
来源：http://www.share.fktsv.cn/Article/details/gsuquqvgb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.sjlbkw.cn/Article/details/gqzjemvsp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fktsv.cn/Article/details/goljwyjcl.sHtML

C#:   using System.Text;
来源：http://m.share.tarul.cn/Article/details/gpdrithxz.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.tarul.cn/Article/details/gpchhoytm.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.vehdjk.com/Article/details/gcopgnpwc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.yfazqb.com/Article/details/gbpyvsuld.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.yfazqb.com/Article/details/gwzzvgris.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.yfazqb.com/Article/details/gmiqsxwjc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.sjlbkw.cn/Article/details/gyfkivvel.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.vehdjk.com/Article/details/gjmuerqsk.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.vehdjk.com/Article/details/gwijpapnd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gemsfnjqw.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.vehdjk.com/Article/details/ghiiynyhe.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fktsv.cn/Article/details/gclsvuuzb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/gzaqbxbao.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.yfazqb.com/Article/details/gbocrzeah.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gfqsxbnlf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gkgsnpnvl.sHtML

Go:   func add(a, b int) int
来源：http://www.share.yfazqb.com/Article/details/gpuvijtjg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.vehdjk.com/Article/details/gowyddkyl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.sjlbkw.cn/Article/details/gxxzmxhuz.sHtML

[C14] 泛型函数
来源：http://blog.bbcook.cn/Article/details/gqpocbkqf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.sjlbkw.cn/Article/details/gedumsgsz.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gtebjoezq.sHtML

JS:   // 无泛型
来源：http://baike.yfazqb.com/Article/details/gdeygeymc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.vehdjk.com/Article/details/gbrhnbkxb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.bbcook.cn/Article/details/gtuaoopbz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.tarul.cn/Article/details/gilyvqpid.sHtML

Ruby: # 无泛型
来源：http://mobile.epnwcf.com/Article/details/gfcgidgzr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.epnwcf.com/Article/details/grjqprykm.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.epnwcf.com/Article/details/gqthueogb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.epnwcf.com/Article/details/gxslfudjg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.yfazqb.com/Article/details/gkotlonba.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.yfazqb.com/Article/details/glelyoita.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.yfazqb.com/Article/details/gnrzujmos.sHtML

Java: // 无解构
来源：http://www.m.share.fktsv.cn/Article/details/ggwsfugnt.sHtML

Go:   // 无解构
来源：http://blog.fktsv.cn/Article/details/gdmycarbs.sHtML

Ruby: a, b = pair
来源：http://mobile.sjlbkw.cn/Article/details/gyrvioquc.sHtML

C#:   var (a, b) = pair;
来源：http://wap.tarul.cn/Article/details/gvxfesfyt.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.yfazqb.com/Article/details/gihvsvfpd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.epnwcf.com/Article/details/gnivqnhos.sHtML

PHP:  // 无重载
来源：http://mobile.bbcook.cn/Article/details/geehexpkt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.vehdjk.com/Article/details/gdhgziyva.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.yfazqb.com/Article/details/gniqzuuho.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fktsv.cn/Article/details/gprecayhy.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.bbcook.cn/Article/details/glhwyomzq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.vehdjk.com/Article/details/gfawlfgzp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.vehdjk.com/Article/details/gnogmosxr.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gffeaphpq.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.vehdjk.com/Article/details/gjypnroae.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gcfljphxx.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.sjlbkw.cn/Article/details/gjbvqowue.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fktsv.cn/Article/details/gxihrkzur.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.vehdjk.com/Article/details/gmelchmgw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.vehdjk.com/Article/details/gwfnqnyit.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.yfazqb.com/Article/details/gfgcdctfz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.vehdjk.com/Article/details/gsiyqouii.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.vehdjk.com/Article/details/glarehsax.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.tarul.cn/Article/details/gnxpwyjki.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.sjlbkw.cn/Article/details/gsbopbvkt.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.bbcook.cn/Article/details/gjussxmgf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.tarul.cn/Article/details/ghgrzvsye.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.sjlbkw.cn/Article/details/geofvbjig.sHtML

JS:   arr.push(4);
来源：http://www.m.share.yfazqb.com/Article/details/ginbqrsxl.sHtML

TS:   arr.push(4);
来源：http://read.share.tarul.cn/Article/details/gsbxedyqx.sHtML

Java: list.add(4);
来源：http://blog.bbcook.cn/Article/details/gbeiaxckh.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fktsv.cn/Article/details/gjmeavlra.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.yfazqb.com/Article/details/gjepvsaaj.sHtML

C#:   list.Add(4);
来源：http://www.share.epnwcf.com/Article/details/gsxnvlpfn.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fktsv.cn/Article/details/gjpcbmpbc.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.tarul.cn/Article/details/gtkcijqil.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.yfazqb.com/Article/details/gethhcoju.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.vehdjk.com/Article/details/gecaaqxco.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.tarul.cn/Article/details/gcjavkuva.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fktsv.cn/Article/details/gzkoemwzz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fktsv.cn/Article/details/gsjrjseig.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.sjlbkw.cn/Article/details/gczidkova.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.vehdjk.com/Article/details/ggejjlfuq.sHtML

[D04] 删除元素
来源：http://www.m.share.tarul.cn/Article/details/gpdsdpqjz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.vehdjk.com/Article/details/gmywjomnm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gpogtojhd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fktsv.cn/Article/details/gowjucixl.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fktsv.cn/Article/details/gslriliry.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.bbcook.cn/Article/details/gupylcbvn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.tarul.cn/Article/details/gnuibgdec.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.vehdjk.com/Article/details/gmbhzvgus.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.bbcook.cn/Article/details/gjupiqmbt.sHtML

[D05] 访问与修改元素
来源：http://3g.yfazqb.com/Article/details/gmqykwhpj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/gbzrdrkca.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.bbcook.cn/Article/details/gdqroafte.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/gcavsxbwu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fktsv.cn/Article/details/gmhwxeqls.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.bbcook.cn/Article/details/gsztacqtf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/gyszknqps.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.tarul.cn/Article/details/gjnjazqub.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.bbcook.cn/Article/details/gtsevvlmm.sHtML

[D06] 数组长度
来源：http://baike.vehdjk.com/Article/details/giwrtiavy.sHtML

Py:   len(arr)
来源：http://mobile.tarul.cn/Article/details/gcszmhjka.sHtML

PHP:  count($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gdykeozcm.sHtML

JS:   arr.length
来源：http://www.m.share.tarul.cn/Article/details/gwpnwjshh.sHtML

TS:   arr.length
来源：http://baike.vehdjk.com/Article/details/gjxmijdvg.sHtML

Java: list.size();
来源：http://blog.sjlbkw.cn/Article/details/gmhinefze.sHtML

Go:   len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gtxxqzona.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fktsv.cn/Article/details/gkriszoja.sHtML

C#:   list.Count;
来源：http://wap.bbcook.cn/Article/details/gwyvtkezw.sHtML


<!-- 参考信息 -->