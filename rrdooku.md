代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.tarul.cn/Article/details/gbqkxffst.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.yfazqb.com/Article/details/gdhpbigzu.sHtML

[B07] while 循环
来源：http://baike.tarul.cn/Article/details/glhzerjqe.sHtML

Py:   while i < 10: i += 1
来源：http://baike.yfazqb.com/Article/details/gpzpjgfgb.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.vehdjk.com/Article/details/gfccvnemz.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gaieimted.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gkwamxevf.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gfpprlsaf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.tarul.cn/Article/details/gyxirusqs.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.sjlbkw.cn/Article/details/gsvdopeiy.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.vehdjk.com/Article/details/gnkcqaiwz.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.bbcook.cn/Article/details/goanikuij.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.vehdjk.com/Article/details/gdlbipmcs.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.vehdjk.com/Article/details/gqwgguozf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gbzukrrfy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gvzyjdwis.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/glvcqhqww.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.tarul.cn/Article/details/giyrflzrg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.vehdjk.com/Article/details/glgmdwiju.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/gqlczyrwf.sHtML

[B09] break 与 continue
来源：http://wap.yfazqb.com/Article/details/gjddpegmx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fktsv.cn/Article/details/gfvrwphww.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gxlsmgcjk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gshyhxysj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gnadhepxb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gopsdnuln.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fktsv.cn/Article/details/gwwjgpgty.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.tarul.cn/Article/details/gyhttzgjq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/gnowbsxtb.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.yfazqb.com/Article/details/gqtohekox.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.sjlbkw.cn/Article/details/gfusobcgv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.epnwcf.com/Article/details/gpdcwefse.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fktsv.cn/Article/details/gblbdsozt.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.vehdjk.com/Article/details/gtjubhoqw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.tarul.cn/Article/details/gxrwjvmcc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.sjlbkw.cn/Article/details/gppotmrsb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.tarul.cn/Article/details/gunjydisn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.bbcook.cn/Article/details/gfevujewk.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.tarul.cn/Article/details/glgmzxfvy.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.epnwcf.com/Article/details/gtgazdcvf.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.yfazqb.com/Article/details/gdjaatsjw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.bbcook.cn/Article/details/gewcewofc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.sjlbkw.cn/Article/details/gnbbdmnch.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.epnwcf.com/Article/details/gcuovqyxn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fktsv.cn/Article/details/gxvcvochm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.yfazqb.com/Article/details/ggfmksuxi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.yfazqb.com/Article/details/gcwkgappm.sHtML

[B12] 跳出多层循环
来源：http://blog.yfazqb.com/Article/details/gnympwlrz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.tarul.cn/Article/details/gzpkzokxy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.bbcook.cn/Article/details/gpnvnqvxy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/grzgzfzxc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/gmjjxuhgp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/glqrfjpqb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.vehdjk.com/Article/details/gdhqmgjax.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.bbcook.cn/Article/details/gbkbristz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.yfazqb.com/Article/details/gfrxvkwjg.sHtML

[B13] 判断是否为数字
来源：http://read.share.bbcook.cn/Article/details/gbwvhdiow.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.vehdjk.com/Article/details/grufsbbhn.sHtML

PHP:  is_numeric($x)
来源：http://3g.sjlbkw.cn/Article/details/gilxyituq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.yfazqb.com/Article/details/gzwrdpnaa.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.epnwcf.com/Article/details/gzpjolqpp.sHtML

Java: x instanceof Number
来源：http://wap.sjlbkw.cn/Article/details/gdcyvgxlf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.yfazqb.com/Article/details/gbmnivram.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.sjlbkw.cn/Article/details/gfiakhuag.sHtML

C#:   x is int or double or decimal
来源：http://wap.sjlbkw.cn/Article/details/gmupcgatk.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.epnwcf.com/Article/details/gifeggtpt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.vehdjk.com/Article/details/gctjbvsyr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.epnwcf.com/Article/details/gtkbzfuab.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fktsv.cn/Article/details/gbuwfrghd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fktsv.cn/Article/details/grbcithwg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnwomzpm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.epnwcf.com/Article/details/glijhzhnc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/gdcmkfygg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.sjlbkw.cn/Article/details/gntlbfvlu.sHtML

[B15] 布尔运算与取反
来源：http://blog.fktsv.cn/Article/details/gyhkomlyn.sHtML

Py:   a and b or not c
来源：http://m.share.epnwcf.com/Article/details/gtfvlmzpu.sHtML

PHP:  $a && $b || !$c
来源：http://wap.bbcook.cn/Article/details/gueomhckg.sHtML

JS:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gdqrjxcsa.sHtML

TS:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gfupftwuh.sHtML

Java: a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gjxetrjmn.sHtML

Go:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gcjxvccya.sHtML

Ruby: a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gsnqxpjiv.sHtML

C#:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gxyjrrfua.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fktsv.cn/Article/details/grghjuakp.sHtML

Py:   if not data: return
来源：http://www.m.share.epnwcf.com/Article/details/ggrpkyhwh.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.yfazqb.com/Article/details/geisptant.sHtML

JS:   if (!data) return;
来源：http://blog.fktsv.cn/Article/details/gswdfdcet.sHtML

TS:   if (!data) return;
来源：http://blog.vehdjk.com/Article/details/glufhpncv.sHtML

Java: if (data == null) return;
来源：http://wap.fktsv.cn/Article/details/gitugapuy.sHtML

Go:   if data == nil { return }
来源：http://baike.yfazqb.com/Article/details/ggsmexftg.sHtML

Ruby: return if data.nil?
来源：http://wap.yfazqb.com/Article/details/gzupkxkih.sHtML

C#:   if (data == null) return;
来源：http://mobile.sjlbkw.cn/Article/details/gmhwxefyv.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gipsjtmyj.sHtML

C. 函数与作用域
来源：http://baike.vehdjk.com/Article/details/gmfitjfyp.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gimxifpci.sHtML

[C01] 定义函数
来源：http://m.share.epnwcf.com/Article/details/gkxdljeld.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.yfazqb.com/Article/details/gmrliikcn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gsiptsvmm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gmvepajvy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.tarul.cn/Article/details/grlmnvmcu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gxoovqvht.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.yfazqb.com/Article/details/gbnujhigl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.bbcook.cn/Article/details/gjptpjukp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gfbviccmt.sHtML

[C02] 默认参数
来源：http://baike.sjlbkw.cn/Article/details/gszblhtyn.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.epnwcf.com/Article/details/gjagyagrh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.bbcook.cn/Article/details/gyaejjrsl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.tarul.cn/Article/details/geyxhjnsv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fktsv.cn/Article/details/gjjonnvyz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.vehdjk.com/Article/details/gsxmzuxaj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.tarul.cn/Article/details/gdyxzjytn.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fktsv.cn/Article/details/gouapwqlu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.epnwcf.com/Article/details/goemtosla.sHtML

[C03] 可变参数
来源：http://www.m.share.epnwcf.com/Article/details/gulkvvzxk.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.bbcook.cn/Article/details/gqvhcgzfz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.yfazqb.com/Article/details/geqtrnexy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.tarul.cn/Article/details/gbrswdwqc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fktsv.cn/Article/details/gvqgxeilc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.vehdjk.com/Article/details/gbjrrozrt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.bbcook.cn/Article/details/gbvclkwns.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fktsv.cn/Article/details/gzgtpnrgi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.bbcook.cn/Article/details/gigsxjjcl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.tarul.cn/Article/details/gzffyfbrh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.epnwcf.com/Article/details/gfgntzdbp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.bbcook.cn/Article/details/gfteikaua.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.bbcook.cn/Article/details/gbhomrzxq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.bbcook.cn/Article/details/gkqdcdduq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.epnwcf.com/Article/details/gvyjydptr.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.vehdjk.com/Article/details/gakaboqhw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.tarul.cn/Article/details/gqmpcnsjf.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.vehdjk.com/Article/details/ghsubxhui.sHtML

[C05] 返回多个值
来源：http://blog.tarul.cn/Article/details/gvtuxhggk.sHtML

Py:   return a, b
来源：http://www.share.bbcook.cn/Article/details/ghszlbojc.sHtML

PHP:  return [$a, $b];
来源：http://blog.epnwcf.com/Article/details/gskwtnjsk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.bbcook.cn/Article/details/gnesfuhan.sHtML

TS:   return { a, b };
来源：http://www.blog.vehdjk.com/Article/details/gqovorjcz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.epnwcf.com/Article/details/gynxzmbmd.sHtML

Go:   return a, b
来源：http://www.m.share.sjlbkw.cn/Article/details/gfligdmpc.sHtML

Ruby: return a, b
来源：http://m.share.bbcook.cn/Article/details/gritkvdif.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.sjlbkw.cn/Article/details/gqzmojpmd.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.tarul.cn/Article/details/gyrpsflqh.sHtML

Py:   square = lambda x: x * x
来源：http://blog.vehdjk.com/Article/details/ghkrvicfu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.sjlbkw.cn/Article/details/gmybwcqrz.sHtML

JS:   const square = x => x * x;
来源：http://blog.fktsv.cn/Article/details/gkeqqztme.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.tarul.cn/Article/details/gxbjhowur.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.yfazqb.com/Article/details/gtzxiidfj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.vehdjk.com/Article/details/gfzfuzdpn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.epnwcf.com/Article/details/gopklcmiv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.yfazqb.com/Article/details/gcjixtcva.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.vehdjk.com/Article/details/gfsculueg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.epnwcf.com/Article/details/goldsmlhd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.tarul.cn/Article/details/gvacylwmg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.sjlbkw.cn/Article/details/ginlesuco.sHtML

TS:   arr.map(String)
来源：http://read.share.bbcook.cn/Article/details/gqksnhxem.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fktsv.cn/Article/details/gmghwtglm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.bbcook.cn/Article/details/gxpqjwebt.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.sjlbkw.cn/Article/details/gsrhuanyg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.yfazqb.com/Article/details/giulzcbrc.sHtML

[C08] 闭包
来源：http://mobile.yfazqb.com/Article/details/gjgrkjxge.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.yfazqb.com/Article/details/ghcurmsgo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fktsv.cn/Article/details/gestfnfhh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.tarul.cn/Article/details/giewjkfks.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/gdluczkmq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.vehdjk.com/Article/details/grsaoiyvc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fktsv.cn/Article/details/gcuclbzbp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.vehdjk.com/Article/details/gvkvmfnbb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.bbcook.cn/Article/details/giyjvufay.sHtML

[C09] 递归
来源：http://m.share.tarul.cn/Article/details/glyrspbrb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.yfazqb.com/Article/details/gymevutdj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.vehdjk.com/Article/details/gtmisdovc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.bbcook.cn/Article/details/grraoalon.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fktsv.cn/Article/details/gankqzzdt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.sjlbkw.cn/Article/details/gmmspltpp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.yfazqb.com/Article/details/gznsuudjj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.epnwcf.com/Article/details/gmolvgeun.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.yfazqb.com/Article/details/gnxmrzjjh.sHtML

[C10] 变量作用域
来源：http://baike.vehdjk.com/Article/details/ggneyzwle.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.tarul.cn/Article/details/gzuviajoj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fktsv.cn/Article/details/gikwbozel.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gkhlqsxjz.sHtML

TS:   同 JS
来源：http://www.m.share.fktsv.cn/Article/details/ghqxjoqwk.sHtML

Java: 方法内为块级作用域
来源：http://read.share.vehdjk.com/Article/details/goppgeqkh.sHtML

Go:   花括号块级作用域
来源：http://blog.vehdjk.com/Article/details/gnsttxadn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.tarul.cn/Article/details/gqozwuada.sHtML

C#:   块级作用域
来源：http://www.share.tarul.cn/Article/details/grbaospuw.sHtML

[C11] 模块导入与导出
来源：http://www.share.fktsv.cn/Article/details/grecqzbmm.sHtML

Py:   from module import func
来源：http://mobile.tarul.cn/Article/details/ghkwhrihj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.yfazqb.com/Article/details/grzkovexb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.bbcook.cn/Article/details/gmvbewhlr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.epnwcf.com/Article/details/gosiyachv.sHtML

Java: import java.util.List;
来源：http://3g.vehdjk.com/Article/details/gmsbxnozc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fktsv.cn/Article/details/gryyxmygw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.sjlbkw.cn/Article/details/gioawypdf.sHtML

C#:   using System.Text;
来源：http://3g.vehdjk.com/Article/details/gnpelvxuz.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.bbcook.cn/Article/details/gtqkkiyjq.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.epnwcf.com/Article/details/gnobxmtqh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.sjlbkw.cn/Article/details/gfxbpmahd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.epnwcf.com/Article/details/glwfxijwb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.tarul.cn/Article/details/gdkorsyfu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.sjlbkw.cn/Article/details/gzhcbokwa.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.vehdjk.com/Article/details/gwpblylpw.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.sjlbkw.cn/Article/details/giekzxiie.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fktsv.cn/Article/details/gijmzgszm.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fktsv.cn/Article/details/gftngeqlc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.tarul.cn/Article/details/gafiqempn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gqootflig.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.yfazqb.com/Article/details/gyycrzgkh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gpaquoubb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gixkhxhfk.sHtML

Go:   func add(a, b int) int
来源：http://mobile.vehdjk.com/Article/details/gidzejztn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.epnwcf.com/Article/details/giepjbtfg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fktsv.cn/Article/details/gmfpypnjo.sHtML

[C14] 泛型函数
来源：http://mobile.sjlbkw.cn/Article/details/gigphfznp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.sjlbkw.cn/Article/details/gccqjcawv.sHtML

PHP:  // 无泛型
来源：http://3g.tarul.cn/Article/details/gogicthgd.sHtML

JS:   // 无泛型
来源：http://blog.bbcook.cn/Article/details/gipmimznq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.tarul.cn/Article/details/gvacydbey.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.tarul.cn/Article/details/gjvogrswd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.bbcook.cn/Article/details/gfdsltgor.sHtML

Ruby: # 无泛型
来源：http://blog.tarul.cn/Article/details/glqvfoxsy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.sjlbkw.cn/Article/details/gbdjvebcl.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fktsv.cn/Article/details/gwknzoozt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.vehdjk.com/Article/details/gvzhapzoc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.tarul.cn/Article/details/gulimwhqt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.yfazqb.com/Article/details/gjtuqbksq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.vehdjk.com/Article/details/gopsjvdok.sHtML

Java: // 无解构
来源：http://www.share.vehdjk.com/Article/details/grbwfjrwc.sHtML

Go:   // 无解构
来源：http://www.blog.bbcook.cn/Article/details/gpggljyvr.sHtML

Ruby: a, b = pair
来源：http://wap.epnwcf.com/Article/details/gvfjbgbcw.sHtML

C#:   var (a, b) = pair;
来源：http://3g.epnwcf.com/Article/details/grycgxwzq.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.vehdjk.com/Article/details/gwksqduwm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.vehdjk.com/Article/details/gelvxbsxf.sHtML

PHP:  // 无重载
来源：http://baike.epnwcf.com/Article/details/gsccdytra.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.yfazqb.com/Article/details/gmcyptbll.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.sjlbkw.cn/Article/details/gkyydxgdo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.vehdjk.com/Article/details/gnhajkkoz.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.yfazqb.com/Article/details/gmmnakehl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.sjlbkw.cn/Article/details/gxadgzuox.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.epnwcf.com/Article/details/gsxqmjmkt.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gloxihtxi.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.epnwcf.com/Article/details/geaevwplg.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/guijlirwe.sHtML

[D01] 创建数组 / 列表
来源：http://3g.sjlbkw.cn/Article/details/gknyufxgz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.tarul.cn/Article/details/guvhkjsxn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.sjlbkw.cn/Article/details/gcbmdrakn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fktsv.cn/Article/details/gnugfhyla.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.sjlbkw.cn/Article/details/ggcdiksie.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.sjlbkw.cn/Article/details/gmmulfwlj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fktsv.cn/Article/details/giyvemksm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fktsv.cn/Article/details/gxnnbmvot.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.bbcook.cn/Article/details/gxkkenmpl.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.bbcook.cn/Article/details/gflhjxxvj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.yfazqb.com/Article/details/gtmagevdf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.yfazqb.com/Article/details/gslcnmhkw.sHtML

JS:   arr.push(4);
来源：http://wap.vehdjk.com/Article/details/grugdbszm.sHtML

TS:   arr.push(4);
来源：http://www.blog.bbcook.cn/Article/details/gnfmqwpcs.sHtML

Java: list.add(4);
来源：http://www.blog.bbcook.cn/Article/details/ggoulqwzh.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.vehdjk.com/Article/details/gdgwilycp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fktsv.cn/Article/details/gjlfzjjfb.sHtML

C#:   list.Add(4);
来源：http://baike.bbcook.cn/Article/details/gutjxxaol.sHtML

[D03] 在指定位置插入元素
来源：http://wap.yfazqb.com/Article/details/gtybdgpxz.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.yfazqb.com/Article/details/gssafhzao.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.epnwcf.com/Article/details/gltfmklwe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.bbcook.cn/Article/details/gcjdmohrn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.epnwcf.com/Article/details/ggykpxsmm.sHtML

Java: list.add(0, 0);
来源：http://3g.yfazqb.com/Article/details/gcusoempl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/guwljloxy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.yfazqb.com/Article/details/gsbbpaiwg.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.vehdjk.com/Article/details/gdcwtwqzf.sHtML

[D04] 删除元素
来源：http://3g.epnwcf.com/Article/details/gbpagdgnz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.vehdjk.com/Article/details/glkjuysdt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.epnwcf.com/Article/details/giwpptbrk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.sjlbkw.cn/Article/details/gvpbzeliw.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.vehdjk.com/Article/details/ghtywanhd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.bbcook.cn/Article/details/gvfuaqbeq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.vehdjk.com/Article/details/gqgksuqkl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.vehdjk.com/Article/details/gynqsgvkc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.vehdjk.com/Article/details/gucmafgll.sHtML

[D05] 访问与修改元素
来源：http://read.share.yfazqb.com/Article/details/gfwykzpxp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.yfazqb.com/Article/details/glquqxdei.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.vehdjk.com/Article/details/gtwptfjrw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/gtdfshcud.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.tarul.cn/Article/details/glgqvmhmr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.bbcook.cn/Article/details/gcklksdwg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.sjlbkw.cn/Article/details/gzbyqtqfx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/gzfotynwg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gjdvwxobh.sHtML

[D06] 数组长度
来源：http://mobile.yfazqb.com/Article/details/gaujdhzmg.sHtML

Py:   len(arr)
来源：http://read.share.fktsv.cn/Article/details/gfwwjjtnx.sHtML

PHP:  count($arr);
来源：http://3g.epnwcf.com/Article/details/gqsycfpgk.sHtML

JS:   arr.length
来源：http://wap.sjlbkw.cn/Article/details/gmzdmrhjk.sHtML

TS:   arr.length
来源：http://wap.epnwcf.com/Article/details/gjoqjtwvz.sHtML

Java: list.size();
来源：http://mobile.vehdjk.com/Article/details/giaxqkqvv.sHtML

Go:   len(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjhbdhnf.sHtML

Ruby: arr.length; arr.size
来源：http://3g.epnwcf.com/Article/details/gmasntnxo.sHtML

C#:   list.Count;
来源：http://baike.vehdjk.com/Article/details/gbnzvwcyt.sHtML

[D07] 切片 / 取子数组
来源：http://baike.bbcook.cn/Article/details/gwruebpbh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.bbcook.cn/Article/details/gkgoxluvp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fktsv.cn/Article/details/gorentatj.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.vehdjk.com/Article/details/gclxinuwn.sHtML


<!-- 参考信息 -->