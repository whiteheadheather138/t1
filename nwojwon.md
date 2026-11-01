代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.epnwcf.com/Article/details/ggeotpbba.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.yfazqb.com/Article/details/gwddnfvfw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.bbcook.cn/Article/details/gjedlmggb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.epnwcf.com/Article/details/gqmfklcke.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.bbcook.cn/Article/details/gisargoum.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.tarul.cn/Article/details/gmfuajcej.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.epnwcf.com/Article/details/gbxosodhw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.yfazqb.com/Article/details/guqdmlepy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fktsv.cn/Article/details/gdmpfujkb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.yfazqb.com/Article/details/gjzcjhovc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.tarul.cn/Article/details/glyqtttbo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fktsv.cn/Article/details/gjzjbhkhj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.tarul.cn/Article/details/grmauftit.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.bbcook.cn/Article/details/gpplecsqk.sHtML

[B07] while 循环
来源：http://mobile.fktsv.cn/Article/details/gkjkuwzjn.sHtML

Py:   while i < 10: i += 1
来源：http://blog.yfazqb.com/Article/details/gzhlxpdml.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gwnosstec.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.vehdjk.com/Article/details/gvxutspdq.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/gybibbhgo.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/gnxekgulr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.epnwcf.com/Article/details/grhafkncm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.epnwcf.com/Article/details/glupfhkdx.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gooeetkks.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.sjlbkw.cn/Article/details/geiwywsxr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.vehdjk.com/Article/details/gvjcgnlpy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.tarul.cn/Article/details/gvksjcnwb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/gsiborbcu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/gavegajtr.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/ghdufxjal.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.epnwcf.com/Article/details/gqikzwqxt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fktsv.cn/Article/details/gtiisrrms.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gwzivaymg.sHtML

[B09] break 与 continue
来源：http://www.m.share.vehdjk.com/Article/details/gsfizlujx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.tarul.cn/Article/details/gqiiqnmdj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gjbfkbgfa.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gbqsjixww.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/glahavkal.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gncmdxfne.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.tarul.cn/Article/details/goinfqghl.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.sjlbkw.cn/Article/details/gvquwscop.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.tarul.cn/Article/details/gmwgsxmhg.sHtML

[B10] 遍历同时拿索引
来源：http://wap.epnwcf.com/Article/details/guepduwse.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.sjlbkw.cn/Article/details/gkdletqfj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.vehdjk.com/Article/details/gqrnebtto.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.vehdjk.com/Article/details/gfmovbpvn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.epnwcf.com/Article/details/gvvyatdhs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.epnwcf.com/Article/details/gfwrbffxk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.epnwcf.com/Article/details/gfcilntkc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.vehdjk.com/Article/details/guxymdygf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.yfazqb.com/Article/details/gwlasexeh.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.sjlbkw.cn/Article/details/gkelybexa.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.tarul.cn/Article/details/gnjvvwdmu.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.sjlbkw.cn/Article/details/gafumsjzs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fktsv.cn/Article/details/gpvddqoen.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fktsv.cn/Article/details/gswwddkuz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.vehdjk.com/Article/details/gzwvaivpi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.tarul.cn/Article/details/ggfxgtbkr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.sjlbkw.cn/Article/details/gkdvugnpe.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.epnwcf.com/Article/details/grvqeachw.sHtML

[B12] 跳出多层循环
来源：http://wap.yfazqb.com/Article/details/gvgsawttz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.tarul.cn/Article/details/gjrxfvooj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.vehdjk.com/Article/details/geyazqncf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/ggkyajrxo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fktsv.cn/Article/details/glwnkvvmw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/gyjgkpxlr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fktsv.cn/Article/details/gvejammmf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.vehdjk.com/Article/details/gbeyjmgzv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fktsv.cn/Article/details/gyskiltkj.sHtML

[B13] 判断是否为数字
来源：http://m.share.bbcook.cn/Article/details/gshgprimr.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.vehdjk.com/Article/details/gncaqrhgx.sHtML

PHP:  is_numeric($x)
来源：http://wap.sjlbkw.cn/Article/details/gcytnxqhk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.yfazqb.com/Article/details/gislxapen.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.epnwcf.com/Article/details/gdjxftwlz.sHtML

Java: x instanceof Number
来源：http://blog.bbcook.cn/Article/details/gucinkhpn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fktsv.cn/Article/details/gnwbfslze.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.yfazqb.com/Article/details/guyetnvlr.sHtML

C#:   x is int or double or decimal
来源：http://3g.vehdjk.com/Article/details/gnvnapplw.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.vehdjk.com/Article/details/gowtpacym.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.epnwcf.com/Article/details/gfvqnkxbc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.bbcook.cn/Article/details/ghbnzxyjw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fktsv.cn/Article/details/gabzqwqjq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.vehdjk.com/Article/details/gwolnkgrz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.vehdjk.com/Article/details/glmhefnxk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.yfazqb.com/Article/details/gqhsrrgad.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.sjlbkw.cn/Article/details/gxwcrneac.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.epnwcf.com/Article/details/gwtmhvinf.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fktsv.cn/Article/details/gatnjwbky.sHtML

Py:   a and b or not c
来源：http://www.share.sjlbkw.cn/Article/details/goebrrdou.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.bbcook.cn/Article/details/gerfbskic.sHtML

JS:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gjcpiqhro.sHtML

TS:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gmeqmwfrv.sHtML

Java: a && b || !c
来源：http://wap.yfazqb.com/Article/details/gxwcoimly.sHtML

Go:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gqimajsly.sHtML

Ruby: a && b || !c
来源：http://3g.fktsv.cn/Article/details/gsxxlsjct.sHtML

C#:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/gwoqdzpwx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.epnwcf.com/Article/details/gegktrsem.sHtML

Py:   if not data: return
来源：http://www.share.epnwcf.com/Article/details/ghxcjutjd.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.sjlbkw.cn/Article/details/gclwvvbav.sHtML

JS:   if (!data) return;
来源：http://m.share.sjlbkw.cn/Article/details/gmnhxrlhw.sHtML

TS:   if (!data) return;
来源：http://www.share.epnwcf.com/Article/details/gajqwuclf.sHtML

Java: if (data == null) return;
来源：http://read.share.epnwcf.com/Article/details/ggfbnolxy.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.tarul.cn/Article/details/gpzxeayxs.sHtML

Ruby: return if data.nil?
来源：http://3g.bbcook.cn/Article/details/gnzlpkdef.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fktsv.cn/Article/details/gacnewmjd.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gtsvbpcvv.sHtML

C. 函数与作用域
来源：http://read.share.sjlbkw.cn/Article/details/gpagpzgoo.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gdkfrlosc.sHtML

[C01] 定义函数
来源：http://m.share.bbcook.cn/Article/details/gexjezfyx.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.bbcook.cn/Article/details/gdxvzgtog.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjnifcfbr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gbzmiamue.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.tarul.cn/Article/details/gnsdljqqj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gpdpjkbwa.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.sjlbkw.cn/Article/details/gdvhcmzyc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fktsv.cn/Article/details/guguclgzv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gafspxlpx.sHtML

[C02] 默认参数
来源：http://read.share.yfazqb.com/Article/details/grhxiaizb.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.tarul.cn/Article/details/gakjoibcc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.epnwcf.com/Article/details/gvpfikdca.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.yfazqb.com/Article/details/gxclbwkuu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.epnwcf.com/Article/details/geakdodih.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fktsv.cn/Article/details/guekdupps.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.epnwcf.com/Article/details/gviqakzfs.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.sjlbkw.cn/Article/details/gzkyjzqor.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.sjlbkw.cn/Article/details/gxfcxkchm.sHtML

[C03] 可变参数
来源：http://m.share.bbcook.cn/Article/details/gdblwefko.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fktsv.cn/Article/details/gghwjxljs.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.yfazqb.com/Article/details/gsrgauogb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fktsv.cn/Article/details/gptnjpqmt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.yfazqb.com/Article/details/gaqgnypag.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.sjlbkw.cn/Article/details/gjjcudhku.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.epnwcf.com/Article/details/gfbdzxets.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.epnwcf.com/Article/details/gimbppvhy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.vehdjk.com/Article/details/gzkhyqlsl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.epnwcf.com/Article/details/gptnrqdzi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.vehdjk.com/Article/details/gddcjtzib.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.vehdjk.com/Article/details/gundqamfd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.tarul.cn/Article/details/gmvmqmgfl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.bbcook.cn/Article/details/goiskzqxa.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.tarul.cn/Article/details/gvqsyhrkx.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.bbcook.cn/Article/details/gmjfktupg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.yfazqb.com/Article/details/gbhivtwkr.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/gmfnxwaei.sHtML

[C05] 返回多个值
来源：http://www.blog.fktsv.cn/Article/details/gzqdlrmmz.sHtML

Py:   return a, b
来源：http://blog.sjlbkw.cn/Article/details/gdzonebst.sHtML

PHP:  return [$a, $b];
来源：http://baike.yfazqb.com/Article/details/gcytwgjag.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fktsv.cn/Article/details/gryalcijm.sHtML

TS:   return { a, b };
来源：http://www.m.share.vehdjk.com/Article/details/ghwbkidkp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.yfazqb.com/Article/details/gkzcfwxzv.sHtML

Go:   return a, b
来源：http://www.m.share.fktsv.cn/Article/details/gdbtcehtl.sHtML

Ruby: return a, b
来源：http://www.blog.epnwcf.com/Article/details/gvfemrbcz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.tarul.cn/Article/details/gqkflopsq.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.tarul.cn/Article/details/guhysktxh.sHtML

Py:   square = lambda x: x * x
来源：http://baike.yfazqb.com/Article/details/gtqzzjxoo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.yfazqb.com/Article/details/gklpzggaw.sHtML

JS:   const square = x => x * x;
来源：http://mobile.bbcook.cn/Article/details/glisgaalp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.bbcook.cn/Article/details/gkbhasysc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.sjlbkw.cn/Article/details/gzsktcjxv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.vehdjk.com/Article/details/gfhettytu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.bbcook.cn/Article/details/gevifkohd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.bbcook.cn/Article/details/gnshjgdws.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fktsv.cn/Article/details/gprhwsieo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.epnwcf.com/Article/details/gsazbvngx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fktsv.cn/Article/details/gtrsasjcj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.sjlbkw.cn/Article/details/gskkzuzci.sHtML

TS:   arr.map(String)
来源：http://www.share.sjlbkw.cn/Article/details/gazqbpbzh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.bbcook.cn/Article/details/gxuturerb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.bbcook.cn/Article/details/gwpgsypba.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.bbcook.cn/Article/details/gjmjngdho.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.vehdjk.com/Article/details/gxyfbtaif.sHtML

[C08] 闭包
来源：http://read.share.fktsv.cn/Article/details/gphuayiom.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fktsv.cn/Article/details/gkctynras.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.tarul.cn/Article/details/guktyskpf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.yfazqb.com/Article/details/gzijidkkm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/ghgdzsoar.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.epnwcf.com/Article/details/gvyhzqbbc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.vehdjk.com/Article/details/gxuksnlod.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.tarul.cn/Article/details/gydniwznk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gefggbyfg.sHtML

[C09] 递归
来源：http://www.blog.yfazqb.com/Article/details/guvantogh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.bbcook.cn/Article/details/ginvijnnu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.bbcook.cn/Article/details/grzzvgxne.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.epnwcf.com/Article/details/gskixiszs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.epnwcf.com/Article/details/gmjkgoouy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.yfazqb.com/Article/details/gtxqzujds.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.tarul.cn/Article/details/guegpxprb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.bbcook.cn/Article/details/gjqljnzad.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.epnwcf.com/Article/details/guwbdcbhb.sHtML

[C10] 变量作用域
来源：http://mobile.yfazqb.com/Article/details/gkirxzpqh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.tarul.cn/Article/details/gbbztdrks.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.bbcook.cn/Article/details/gysabnjlq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.bbcook.cn/Article/details/gljwazrad.sHtML

TS:   同 JS
来源：http://m.share.sjlbkw.cn/Article/details/ggoforazd.sHtML

Java: 方法内为块级作用域
来源：http://read.share.tarul.cn/Article/details/gxhrsvkkj.sHtML

Go:   花括号块级作用域
来源：http://read.share.vehdjk.com/Article/details/gjklvxill.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fktsv.cn/Article/details/gcjcxrojb.sHtML

C#:   块级作用域
来源：http://wap.yfazqb.com/Article/details/gnariwdut.sHtML

[C11] 模块导入与导出
来源：http://wap.bbcook.cn/Article/details/gmbnnjged.sHtML

Py:   from module import func
来源：http://3g.tarul.cn/Article/details/geffzalwq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.yfazqb.com/Article/details/gpqjzndgw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.tarul.cn/Article/details/gdkkvmjid.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.yfazqb.com/Article/details/gtypkmlgy.sHtML

Java: import java.util.List;
来源：http://blog.tarul.cn/Article/details/gegxyocur.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.bbcook.cn/Article/details/giychhscs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.bbcook.cn/Article/details/gtwojdtoi.sHtML

C#:   using System.Text;
来源：http://read.share.bbcook.cn/Article/details/gxlussadi.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.vehdjk.com/Article/details/gurjevkky.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.epnwcf.com/Article/details/gpvkmenfq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.epnwcf.com/Article/details/gsgdhwnss.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.sjlbkw.cn/Article/details/gwghfrdsw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.vehdjk.com/Article/details/gevieikzk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.tarul.cn/Article/details/gckubuksp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.vehdjk.com/Article/details/gyrflzikv.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.epnwcf.com/Article/details/gsbxnbusz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.epnwcf.com/Article/details/gvcislytt.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtkldgcz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fktsv.cn/Article/details/gywjhwdsv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gjflzlpnf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmgqjejg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gfjtkpvqf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gauixally.sHtML

Go:   func add(a, b int) int
来源：http://mobile.epnwcf.com/Article/details/gokwrtgip.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.tarul.cn/Article/details/gbvxfnmux.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.bbcook.cn/Article/details/gbvyyqbss.sHtML

[C14] 泛型函数
来源：http://blog.vehdjk.com/Article/details/gplnhmpzo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.epnwcf.com/Article/details/gvvmbwhqn.sHtML

PHP:  // 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gitohoqai.sHtML

JS:   // 无泛型
来源：http://blog.tarul.cn/Article/details/gacruhcip.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.tarul.cn/Article/details/gtydtribw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.tarul.cn/Article/details/gzbqldbqa.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.sjlbkw.cn/Article/details/gmfrtmqvh.sHtML

Ruby: # 无泛型
来源：http://blog.fktsv.cn/Article/details/gucsfxikc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.yfazqb.com/Article/details/giegyhhtz.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fktsv.cn/Article/details/gtrptleaq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fktsv.cn/Article/details/gydhntogb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.bbcook.cn/Article/details/ghyilcdhu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.yfazqb.com/Article/details/gcxzckake.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fktsv.cn/Article/details/gtykrofub.sHtML

Java: // 无解构
来源：http://www.share.fktsv.cn/Article/details/goelqjora.sHtML

Go:   // 无解构
来源：http://mobile.tarul.cn/Article/details/gcnkdbvjd.sHtML

Ruby: a, b = pair
来源：http://baike.fktsv.cn/Article/details/gnazkyxsa.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.sjlbkw.cn/Article/details/geodrftij.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.yfazqb.com/Article/details/gvztvrfsq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.sjlbkw.cn/Article/details/gblrhycap.sHtML

PHP:  // 无重载
来源：http://3g.yfazqb.com/Article/details/gmxfflzoc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fktsv.cn/Article/details/gtfkuvvyf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.yfazqb.com/Article/details/ghxdozpcz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.epnwcf.com/Article/details/gyxrcsxwm.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.yfazqb.com/Article/details/gcvlxhnok.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.tarul.cn/Article/details/gujfcvhhc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fktsv.cn/Article/details/gaymmpkea.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gaeihboig.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.yfazqb.com/Article/details/ghpsbugab.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gjfjqejjx.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.sjlbkw.cn/Article/details/gqsnrlnlw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.epnwcf.com/Article/details/gchnvyvnr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.epnwcf.com/Article/details/glbhocfva.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.sjlbkw.cn/Article/details/gweqwfjmb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.tarul.cn/Article/details/gvchmrpup.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fktsv.cn/Article/details/gfikgiqkl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fktsv.cn/Article/details/gidfisifj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.yfazqb.com/Article/details/gzquwmbti.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.bbcook.cn/Article/details/gifjjrjdq.sHtML

[D02] 追加元素到末尾
来源：http://mobile.sjlbkw.cn/Article/details/godsawosq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fktsv.cn/Article/details/goycfiuqs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.yfazqb.com/Article/details/gbarkceum.sHtML

JS:   arr.push(4);
来源：http://mobile.tarul.cn/Article/details/glntducnh.sHtML

TS:   arr.push(4);
来源：http://blog.bbcook.cn/Article/details/gxpcuovzk.sHtML

Java: list.add(4);
来源：http://3g.sjlbkw.cn/Article/details/gipaytnic.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.tarul.cn/Article/details/gnkkxibeb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.yfazqb.com/Article/details/gfclvxxua.sHtML

C#:   list.Add(4);
来源：http://3g.bbcook.cn/Article/details/gtpvfjpor.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.epnwcf.com/Article/details/gzownloay.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.bbcook.cn/Article/details/gxubbzpna.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.tarul.cn/Article/details/glznfpvwv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fktsv.cn/Article/details/ghbpzvgia.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.bbcook.cn/Article/details/gcajrrtde.sHtML

Java: list.add(0, 0);
来源：http://www.share.bbcook.cn/Article/details/gjsvnvuat.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.tarul.cn/Article/details/gbwklhpdl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.sjlbkw.cn/Article/details/guutcdksj.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.tarul.cn/Article/details/guwfrpazo.sHtML

[D04] 删除元素
来源：http://m.share.bbcook.cn/Article/details/grzklewzj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.vehdjk.com/Article/details/gtrnttdoi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.epnwcf.com/Article/details/gfztwhson.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.vehdjk.com/Article/details/ghqdhtxqn.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fktsv.cn/Article/details/ghjlfgnro.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fktsv.cn/Article/details/gofmjlgrz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.yfazqb.com/Article/details/gmfgnyeae.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdshkcrc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fktsv.cn/Article/details/gaapnjjpx.sHtML

[D05] 访问与修改元素
来源：http://mobile.vehdjk.com/Article/details/gqxptmylw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/gfrwxaety.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.yfazqb.com/Article/details/giqwuyehz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/ghrubgmxc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.vehdjk.com/Article/details/gyxhsbbye.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.sjlbkw.cn/Article/details/gsojewkoj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gaeakltcq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/gcinwgqif.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.tarul.cn/Article/details/giligmjfe.sHtML

[D06] 数组长度
来源：http://baike.bbcook.cn/Article/details/gzmtyjsqy.sHtML


<!-- 参考信息 -->