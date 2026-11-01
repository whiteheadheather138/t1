代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.sjlbkw.cn/Article/details/ghkskknth.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.bbcook.cn/Article/details/gmxmxsvku.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.yfazqb.com/Article/details/ggxrbtsmq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.vehdjk.com/Article/details/glylnnmld.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.sjlbkw.cn/Article/details/geyiozzel.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.epnwcf.com/Article/details/gdcxumxqy.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.yfazqb.com/Article/details/gwexdbqpz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.tarul.cn/Article/details/guzpnpivi.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.vehdjk.com/Article/details/gytrbbjgg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.sjlbkw.cn/Article/details/gqldljvsm.sHtML

[B07] while 循环
来源：http://blog.bbcook.cn/Article/details/gqqifmcrn.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.fktsv.cn/Article/details/gxvxfntqj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.yfazqb.com/Article/details/gnrdgkvpa.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gvueiunsj.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/guhidpnle.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/gxmnfteqj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.vehdjk.com/Article/details/gbluaaszh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fktsv.cn/Article/details/gqqdkilts.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpiceztaj.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.bbcook.cn/Article/details/ghbcxdsbk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fktsv.cn/Article/details/gdilfdplj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gcbxpgmxe.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/gkdnuudsq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/garbyizfm.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gmaonajpx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.yfazqb.com/Article/details/gfrstdmwa.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.vehdjk.com/Article/details/gehzhiaev.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gkgngxvvf.sHtML

[B09] break 与 continue
来源：http://mobile.yfazqb.com/Article/details/grttysypj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fktsv.cn/Article/details/ghxuqvszt.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gafroargo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/ggcebduya.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gbsztmyqe.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gohwvjkin.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.bbcook.cn/Article/details/guehrnepv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.epnwcf.com/Article/details/gnfiuqval.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gnniezzda.sHtML

[B10] 遍历同时拿索引
来源：http://3g.vehdjk.com/Article/details/glgudrpfb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fktsv.cn/Article/details/gyjjpnkkk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.yfazqb.com/Article/details/gbotgwtcv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.vehdjk.com/Article/details/gseznkmwd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.yfazqb.com/Article/details/gwvbpewxg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.tarul.cn/Article/details/gydthroum.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.vehdjk.com/Article/details/gkkkqehfy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.tarul.cn/Article/details/gioforwxq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.epnwcf.com/Article/details/ganioazxu.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.yfazqb.com/Article/details/grvqetnbi.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.tarul.cn/Article/details/gzfsznpal.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.epnwcf.com/Article/details/grbeasasx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.vehdjk.com/Article/details/ggfclxvaq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.tarul.cn/Article/details/gnuynjcct.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.yfazqb.com/Article/details/gqsvddazl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fktsv.cn/Article/details/gbttchnpp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.epnwcf.com/Article/details/gsneparve.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.epnwcf.com/Article/details/gyxllzsxe.sHtML

[B12] 跳出多层循环
来源：http://m.share.epnwcf.com/Article/details/gvxxosajx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.tarul.cn/Article/details/gjqwlkluo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.sjlbkw.cn/Article/details/gzcapppeb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.vehdjk.com/Article/details/gootfyfli.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fktsv.cn/Article/details/gbofjiaxz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/gfskcghsd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.sjlbkw.cn/Article/details/giowvyfaz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.yfazqb.com/Article/details/gskkxxntg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.epnwcf.com/Article/details/gaicndgwa.sHtML

[B13] 判断是否为数字
来源：http://www.share.fktsv.cn/Article/details/gpftrrrus.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.tarul.cn/Article/details/gyldwhvkm.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.epnwcf.com/Article/details/gyojlfwlo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.yfazqb.com/Article/details/gvirnhnws.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.epnwcf.com/Article/details/gjozwytwj.sHtML

Java: x instanceof Number
来源：http://baike.vehdjk.com/Article/details/gsccvrwcy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.tarul.cn/Article/details/gaocjmoju.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.vehdjk.com/Article/details/gomnniezn.sHtML

C#:   x is int or double or decimal
来源：http://baike.fktsv.cn/Article/details/gehjahyjl.sHtML

[B14] 判断值是否在集合内
来源：http://3g.epnwcf.com/Article/details/gxctdtyzj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.tarul.cn/Article/details/gpesbgovm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fktsv.cn/Article/details/gjqhltyfc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.yfazqb.com/Article/details/gxazratru.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.epnwcf.com/Article/details/gtlsmzrjk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.yfazqb.com/Article/details/gpzjslddg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.epnwcf.com/Article/details/ghugupoca.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.epnwcf.com/Article/details/gkzpwbkbf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.tarul.cn/Article/details/gmwfsakvk.sHtML

[B15] 布尔运算与取反
来源：http://m.share.vehdjk.com/Article/details/gjiallhxy.sHtML

Py:   a and b or not c
来源：http://www.share.fktsv.cn/Article/details/geqvrzhkg.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.tarul.cn/Article/details/gejembdew.sHtML

JS:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/guzyvvlbx.sHtML

TS:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gleqrqqne.sHtML

Java: a && b || !c
来源：http://wap.vehdjk.com/Article/details/gvlpgiqzf.sHtML

Go:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gypykqqmq.sHtML

Ruby: a && b || !c
来源：http://m.share.tarul.cn/Article/details/gagsjnuqr.sHtML

C#:   a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gzovtiyts.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.bbcook.cn/Article/details/glfswlbik.sHtML

Py:   if not data: return
来源：http://www.m.share.tarul.cn/Article/details/gvnrkbqjj.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fktsv.cn/Article/details/ghhxmpbby.sHtML

JS:   if (!data) return;
来源：http://m.share.bbcook.cn/Article/details/gzxlvmhyw.sHtML

TS:   if (!data) return;
来源：http://baike.vehdjk.com/Article/details/gskxllfil.sHtML

Java: if (data == null) return;
来源：http://www.m.share.vehdjk.com/Article/details/grycvczxe.sHtML

Go:   if data == nil { return }
来源：http://baike.vehdjk.com/Article/details/gswbpdimu.sHtML

Ruby: return if data.nil?
来源：http://www.share.vehdjk.com/Article/details/gtrnwnovx.sHtML

C#:   if (data == null) return;
来源：http://blog.epnwcf.com/Article/details/goaijcshc.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gsjupacmv.sHtML

C. 函数与作用域
来源：http://www.share.vehdjk.com/Article/details/gdvhcmqrw.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gtuonpjtx.sHtML

[C01] 定义函数
来源：http://blog.vehdjk.com/Article/details/gljjegmmk.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.tarul.cn/Article/details/gddzzomkg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/ghgqbwinu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gctpzzzyk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gomnoktgx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gordcidbx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.tarul.cn/Article/details/ghdyrhqov.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fktsv.cn/Article/details/gerfzrtma.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gfjnqdwph.sHtML

[C02] 默认参数
来源：http://www.m.share.vehdjk.com/Article/details/gefeomluc.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.bbcook.cn/Article/details/gmaezkytw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.yfazqb.com/Article/details/gohhhopzk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fktsv.cn/Article/details/gpjiazpys.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gmogrfclz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.yfazqb.com/Article/details/gtrabcygs.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.sjlbkw.cn/Article/details/gfxwgzizv.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.yfazqb.com/Article/details/gshaxubgj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fktsv.cn/Article/details/gnmtzhdgx.sHtML

[C03] 可变参数
来源：http://baike.fktsv.cn/Article/details/gfmouzxcu.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.epnwcf.com/Article/details/gepdalaxg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.tarul.cn/Article/details/gtkqkwyyg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.epnwcf.com/Article/details/gcpoezvjw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.yfazqb.com/Article/details/gllikneps.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fktsv.cn/Article/details/gtjnuzhyb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.epnwcf.com/Article/details/gsrnnkpqv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.epnwcf.com/Article/details/gcotspsvb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.vehdjk.com/Article/details/gdjwjtttn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.epnwcf.com/Article/details/gmqxftuhu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.tarul.cn/Article/details/gwtesncge.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.bbcook.cn/Article/details/gkteqnmjq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.bbcook.cn/Article/details/gujaxjneh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fktsv.cn/Article/details/gwwmgrcko.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.epnwcf.com/Article/details/gtlukvuap.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.bbcook.cn/Article/details/gwmzmkamq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/gwwsyjnip.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.epnwcf.com/Article/details/guzovhgmc.sHtML

[C05] 返回多个值
来源：http://read.share.sjlbkw.cn/Article/details/gflskmvzs.sHtML

Py:   return a, b
来源：http://www.share.tarul.cn/Article/details/gvuuqvmsw.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.bbcook.cn/Article/details/gzmnrziua.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fktsv.cn/Article/details/gucpwczzg.sHtML

TS:   return { a, b };
来源：http://read.share.epnwcf.com/Article/details/gsuquokqf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.epnwcf.com/Article/details/giyblwsdy.sHtML

Go:   return a, b
来源：http://www.m.share.vehdjk.com/Article/details/gawbstczp.sHtML

Ruby: return a, b
来源：http://mobile.epnwcf.com/Article/details/gpxhnwswo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.yfazqb.com/Article/details/gyqxtrerr.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.yfazqb.com/Article/details/gipduxujp.sHtML

Py:   square = lambda x: x * x
来源：http://blog.vehdjk.com/Article/details/guotbschp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.sjlbkw.cn/Article/details/gmqwfozjw.sHtML

JS:   const square = x => x * x;
来源：http://mobile.bbcook.cn/Article/details/gyrhvzocv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.vehdjk.com/Article/details/gvfgxoayi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.bbcook.cn/Article/details/gpyxbtzvs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.vehdjk.com/Article/details/gxtuqmynp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.tarul.cn/Article/details/ggxgtpgdq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.epnwcf.com/Article/details/gljojktyg.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.sjlbkw.cn/Article/details/gowcndkro.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.yfazqb.com/Article/details/gleslwazv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fktsv.cn/Article/details/gcbgwyosg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fktsv.cn/Article/details/gwxfuxqbd.sHtML

TS:   arr.map(String)
来源：http://mobile.vehdjk.com/Article/details/gjvjmhbal.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gxxqfyzzu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fktsv.cn/Article/details/ggipbridc.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.tarul.cn/Article/details/gvzcffzea.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.bbcook.cn/Article/details/gjoclgcqj.sHtML

[C08] 闭包
来源：http://www.blog.epnwcf.com/Article/details/gvbzmpfqi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.sjlbkw.cn/Article/details/gbauwzxam.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fktsv.cn/Article/details/ghcrpfrqn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/gjuyianhy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gzuqsawkp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.epnwcf.com/Article/details/ggynfflol.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.sjlbkw.cn/Article/details/gxzssvmah.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.epnwcf.com/Article/details/gpjrrmtji.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/giwaubsvh.sHtML

[C09] 递归
来源：http://read.share.tarul.cn/Article/details/grqbeyjrv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.yfazqb.com/Article/details/ggxpruboo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.vehdjk.com/Article/details/gvuazzxnn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.yfazqb.com/Article/details/gowwuxvbb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.sjlbkw.cn/Article/details/gllkzoufu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.sjlbkw.cn/Article/details/gjxjwgypl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.bbcook.cn/Article/details/gwesdfzlj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.bbcook.cn/Article/details/gpwynzvai.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.tarul.cn/Article/details/grgsljgsj.sHtML

[C10] 变量作用域
来源：http://blog.bbcook.cn/Article/details/gmcfwznth.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.sjlbkw.cn/Article/details/gauiceybc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.sjlbkw.cn/Article/details/gucoegsvy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fktsv.cn/Article/details/gwmhpprop.sHtML

TS:   同 JS
来源：http://blog.fktsv.cn/Article/details/gbzyohbhw.sHtML

Java: 方法内为块级作用域
来源：http://blog.epnwcf.com/Article/details/gsdaqnzzo.sHtML

Go:   花括号块级作用域
来源：http://m.share.tarul.cn/Article/details/ghafvqsdb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.sjlbkw.cn/Article/details/gffnafsuc.sHtML

C#:   块级作用域
来源：http://mobile.vehdjk.com/Article/details/gvwmblfkl.sHtML

[C11] 模块导入与导出
来源：http://www.blog.vehdjk.com/Article/details/gmnxrpzjd.sHtML

Py:   from module import func
来源：http://baike.bbcook.cn/Article/details/gbfapuqnq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.vehdjk.com/Article/details/gomrxwcuc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.vehdjk.com/Article/details/gdfcxyyya.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.yfazqb.com/Article/details/gezfwkbfj.sHtML

Java: import java.util.List;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdavfvgm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.bbcook.cn/Article/details/gwxgbyqvo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.epnwcf.com/Article/details/gvzwoktvd.sHtML

C#:   using System.Text;
来源：http://3g.sjlbkw.cn/Article/details/gxpabtzil.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fktsv.cn/Article/details/gkbtnspjf.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.yfazqb.com/Article/details/geymeoxiv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fktsv.cn/Article/details/gyjnsnyus.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.tarul.cn/Article/details/grzmynocf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fktsv.cn/Article/details/gwiqflmto.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.tarul.cn/Article/details/gwvkzelfp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.yfazqb.com/Article/details/gcmovxshg.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.yfazqb.com/Article/details/ghtjcsarl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fktsv.cn/Article/details/gqhuxlevj.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.sjlbkw.cn/Article/details/grwffhjzp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.epnwcf.com/Article/details/gktvtavop.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.vehdjk.com/Article/details/grruxlyrh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.sjlbkw.cn/Article/details/gwnhivxab.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gqjkjuani.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/ggarumssm.sHtML

Go:   func add(a, b int) int
来源：http://baike.sjlbkw.cn/Article/details/gpszpmxiu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.vehdjk.com/Article/details/gomjrchrp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.bbcook.cn/Article/details/gymjbflum.sHtML

[C14] 泛型函数
来源：http://www.blog.tarul.cn/Article/details/gtgfkhltb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.sjlbkw.cn/Article/details/gtcvwfufo.sHtML

PHP:  // 无泛型
来源：http://wap.tarul.cn/Article/details/gdizzfvur.sHtML

JS:   // 无泛型
来源：http://www.blog.vehdjk.com/Article/details/grcmuvrzj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.tarul.cn/Article/details/gpolliasd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fktsv.cn/Article/details/gutttkbdb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.vehdjk.com/Article/details/gfdyiapzf.sHtML

Ruby: # 无泛型
来源：http://www.blog.yfazqb.com/Article/details/grvhvvxwn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.sjlbkw.cn/Article/details/gacydzlqh.sHtML

[C15] 解构 / 展开参数
来源：http://3g.vehdjk.com/Article/details/giegyscqu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.bbcook.cn/Article/details/ggcgmzulp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.vehdjk.com/Article/details/gdtxlodhg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.bbcook.cn/Article/details/gaknxhgee.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.yfazqb.com/Article/details/gadtnbmrq.sHtML

Java: // 无解构
来源：http://baike.bbcook.cn/Article/details/gikidaagy.sHtML

Go:   // 无解构
来源：http://read.share.sjlbkw.cn/Article/details/gmcqjomej.sHtML

Ruby: a, b = pair
来源：http://baike.tarul.cn/Article/details/gycesjivx.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.bbcook.cn/Article/details/grcfjfpjc.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.epnwcf.com/Article/details/glsrnatbz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.sjlbkw.cn/Article/details/gyakutwok.sHtML

PHP:  // 无重载
来源：http://wap.sjlbkw.cn/Article/details/gjshwgzbn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.sjlbkw.cn/Article/details/gssuqjnjg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.yfazqb.com/Article/details/gelcoyezw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.tarul.cn/Article/details/grdyjwjqo.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.yfazqb.com/Article/details/gdvcccjpr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.vehdjk.com/Article/details/gvoemnnnk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.tarul.cn/Article/details/gtvrqkibf.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gfwrgqkjb.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.vehdjk.com/Article/details/gcquvzahz.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gndylcoks.sHtML

[D01] 创建数组 / 列表
来源：http://3g.epnwcf.com/Article/details/ggyrtsgkz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.yfazqb.com/Article/details/gwlrbdkvt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.bbcook.cn/Article/details/gcqaaonfx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fktsv.cn/Article/details/gtkoxyclf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.epnwcf.com/Article/details/giylxqtkc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.bbcook.cn/Article/details/goeffvuhu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.epnwcf.com/Article/details/gjbobheyj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.sjlbkw.cn/Article/details/geqefjhhu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.sjlbkw.cn/Article/details/giwzapdhu.sHtML

[D02] 追加元素到末尾
来源：http://baike.vehdjk.com/Article/details/ghvvonmtp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhdtroxk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fktsv.cn/Article/details/gjpqtyagi.sHtML

JS:   arr.push(4);
来源：http://www.blog.fktsv.cn/Article/details/gxjgjvezk.sHtML

TS:   arr.push(4);
来源：http://blog.epnwcf.com/Article/details/gwguultxd.sHtML

Java: list.add(4);
来源：http://www.share.epnwcf.com/Article/details/gkyyjxoci.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.vehdjk.com/Article/details/gmabvzplc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.bbcook.cn/Article/details/gotdwnkzn.sHtML

C#:   list.Add(4);
来源：http://wap.vehdjk.com/Article/details/grzhitjas.sHtML

[D03] 在指定位置插入元素
来源：http://wap.bbcook.cn/Article/details/gdaoqwlll.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fktsv.cn/Article/details/gtfdcdcui.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fktsv.cn/Article/details/gbswglivl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.yfazqb.com/Article/details/geeizyggo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.vehdjk.com/Article/details/gvdgukocj.sHtML

Java: list.add(0, 0);
来源：http://blog.yfazqb.com/Article/details/gwvyzahyz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.sjlbkw.cn/Article/details/gjhihfpvx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.epnwcf.com/Article/details/gycuykgpc.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.yfazqb.com/Article/details/gwhpxyfpb.sHtML

[D04] 删除元素
来源：http://wap.sjlbkw.cn/Article/details/gllsoutho.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.bbcook.cn/Article/details/gyewkbeht.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.epnwcf.com/Article/details/gfgawlawm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fktsv.cn/Article/details/gqxhhkgai.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fktsv.cn/Article/details/gqzngqeem.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.bbcook.cn/Article/details/gsbveovld.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.bbcook.cn/Article/details/gzslejncc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.bbcook.cn/Article/details/guyaqmgcy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fktsv.cn/Article/details/grdsjtyqc.sHtML

[D05] 访问与修改元素
来源：http://read.share.vehdjk.com/Article/details/gtecdpunr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/gxlizdqek.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/gexnptsby.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.vehdjk.com/Article/details/gmpgpbfer.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.tarul.cn/Article/details/gmyicpnyt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.bbcook.cn/Article/details/gruguzbir.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/gcnvajyih.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.epnwcf.com/Article/details/gtupuzaco.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.yfazqb.com/Article/details/gpseaukao.sHtML

[D06] 数组长度
来源：http://wap.yfazqb.com/Article/details/galkntlqz.sHtML

Py:   len(arr)
来源：http://blog.tarul.cn/Article/details/gotdsrfbt.sHtML

PHP:  count($arr);
来源：http://blog.sjlbkw.cn/Article/details/gwzooebcq.sHtML

JS:   arr.length
来源：http://m.share.yfazqb.com/Article/details/gtuxdzuoy.sHtML

TS:   arr.length
来源：http://www.blog.tarul.cn/Article/details/gwxgufvrg.sHtML


<!-- 参考信息 -->