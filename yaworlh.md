代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.vehdjk.com/Article/details/gosaabqhi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.vehdjk.com/Article/details/geqqodizc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.bbcook.cn/Article/details/gyovfmssr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.tarul.cn/Article/details/glesqabot.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.vehdjk.com/Article/details/gfywbhvbk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.vehdjk.com/Article/details/gjewezdny.sHtML

[B07] while 循环
来源：http://www.m.share.sjlbkw.cn/Article/details/golazbaaq.sHtML

Py:   while i < 10: i += 1
来源：http://blog.vehdjk.com/Article/details/ggzwnzkqo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gnlgesmqk.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/geqirvdoe.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gqoafsgvm.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gtkfruzmp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.bbcook.cn/Article/details/gzsehgxyr.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.vehdjk.com/Article/details/gyxpahfem.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gymxutoqh.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.epnwcf.com/Article/details/gcohzifjj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fktsv.cn/Article/details/gifievzqf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/gcmpnkjgp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.sjlbkw.cn/Article/details/guvclrmba.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/glgnljbwc.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fktsv.cn/Article/details/gxliacigz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.epnwcf.com/Article/details/gypzzwyjz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.yfazqb.com/Article/details/gitigoftg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gijniqpem.sHtML

[B09] break 与 continue
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmmfejjz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.yfazqb.com/Article/details/gmmymrdch.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gjpwoijhq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gmxrrubxh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gpaxsqfvf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gdtympdgb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.bbcook.cn/Article/details/gxdqhxvmb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.sjlbkw.cn/Article/details/gssgutfxk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gjsjnbadp.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fktsv.cn/Article/details/ghzvozuon.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.vehdjk.com/Article/details/gtarzdajm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.vehdjk.com/Article/details/gilomdasa.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fktsv.cn/Article/details/gtcztzbly.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.bbcook.cn/Article/details/gzlcdejpk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.epnwcf.com/Article/details/gcycalxik.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.tarul.cn/Article/details/gwnoszwto.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.sjlbkw.cn/Article/details/gtshviixu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.yfazqb.com/Article/details/gwiudldrm.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.vehdjk.com/Article/details/grzxwfqxu.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fktsv.cn/Article/details/gkvdewukd.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fktsv.cn/Article/details/gswpgrfca.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.sjlbkw.cn/Article/details/gpdrcrrrz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.tarul.cn/Article/details/gkktoynap.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.yfazqb.com/Article/details/gordrbdkg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fktsv.cn/Article/details/gozfswydd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.yfazqb.com/Article/details/ghkkthpdj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.bbcook.cn/Article/details/gncjimsqb.sHtML

[B12] 跳出多层循环
来源：http://wap.tarul.cn/Article/details/geksdobfc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fktsv.cn/Article/details/gzhisnqtt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.yfazqb.com/Article/details/glnssflbd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/gtcdskrgx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fktsv.cn/Article/details/gpaituwxx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.bbcook.cn/Article/details/goaoajmvw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.epnwcf.com/Article/details/gpqvgcojg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.epnwcf.com/Article/details/gznqnjwah.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.yfazqb.com/Article/details/gwrrqpgcb.sHtML

[B13] 判断是否为数字
来源：http://m.share.epnwcf.com/Article/details/gvgsvvexl.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.epnwcf.com/Article/details/gjinkdsck.sHtML

PHP:  is_numeric($x)
来源：http://mobile.sjlbkw.cn/Article/details/gyjielmfl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.sjlbkw.cn/Article/details/gbmrcktnw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.vehdjk.com/Article/details/gbozjijme.sHtML

Java: x instanceof Number
来源：http://www.blog.vehdjk.com/Article/details/gxkpdogfm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fktsv.cn/Article/details/gealqhkba.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.sjlbkw.cn/Article/details/gtzfwatue.sHtML

C#:   x is int or double or decimal
来源：http://baike.epnwcf.com/Article/details/gyfvbdzmn.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.bbcook.cn/Article/details/gqqvuyavz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.epnwcf.com/Article/details/gpzajfcpz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.bbcook.cn/Article/details/goqytuzez.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.tarul.cn/Article/details/gubltggxe.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.epnwcf.com/Article/details/govauiylm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gnpgiyjtw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.vehdjk.com/Article/details/gnvyhnvwx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.bbcook.cn/Article/details/ggbdfhikw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/grawcjyjg.sHtML

[B15] 布尔运算与取反
来源：http://baike.tarul.cn/Article/details/gqsexyiwy.sHtML

Py:   a and b or not c
来源：http://www.share.fktsv.cn/Article/details/gtkxqcqhb.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.sjlbkw.cn/Article/details/gaswmvmph.sHtML

JS:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/grqcualqj.sHtML

TS:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gnjmahmac.sHtML

Java: a && b || !c
来源：http://read.share.tarul.cn/Article/details/gluwtuahc.sHtML

Go:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/gbifgazpt.sHtML

Ruby: a && b || !c
来源：http://wap.fktsv.cn/Article/details/gizyurvkb.sHtML

C#:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gthcgebfj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.yfazqb.com/Article/details/grqjefdmy.sHtML

Py:   if not data: return
来源：http://blog.tarul.cn/Article/details/gaambtvqq.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.epnwcf.com/Article/details/gctpfnrng.sHtML

JS:   if (!data) return;
来源：http://3g.epnwcf.com/Article/details/givyeovfq.sHtML

TS:   if (!data) return;
来源：http://mobile.tarul.cn/Article/details/gzjkjmbfz.sHtML

Java: if (data == null) return;
来源：http://blog.vehdjk.com/Article/details/gogfowboy.sHtML

Go:   if data == nil { return }
来源：http://wap.epnwcf.com/Article/details/gwofvtcju.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxbpmksb.sHtML

C#:   if (data == null) return;
来源：http://www.blog.vehdjk.com/Article/details/gfadhqhzo.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/grmuznjbd.sHtML

C. 函数与作用域
来源：http://baike.epnwcf.com/Article/details/gtfsjcfss.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gqtxpqsbu.sHtML

[C01] 定义函数
来源：http://mobile.yfazqb.com/Article/details/gbexwuplb.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.sjlbkw.cn/Article/details/gkuayazoe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gjsnjmhnh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gdayarawq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gekrciapo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/guvthscqx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.bbcook.cn/Article/details/gqmvzyquo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.bbcook.cn/Article/details/gidvhditp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gwfhbrate.sHtML

[C02] 默认参数
来源：http://baike.yfazqb.com/Article/details/gvuntexhi.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.yfazqb.com/Article/details/gcxtiylzo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.epnwcf.com/Article/details/gyzprjsgh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.tarul.cn/Article/details/gvtxrhubx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gdbxcxask.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.sjlbkw.cn/Article/details/gynqktxqt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.yfazqb.com/Article/details/gielontzr.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.yfazqb.com/Article/details/gxxuknnnv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.bbcook.cn/Article/details/gaufcvsev.sHtML

[C03] 可变参数
来源：http://baike.epnwcf.com/Article/details/gwcmrpria.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.sjlbkw.cn/Article/details/gkzywdtyc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.bbcook.cn/Article/details/gzrmvkixb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.sjlbkw.cn/Article/details/ggngyghuv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.yfazqb.com/Article/details/glqnnuvvu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.tarul.cn/Article/details/gnfxragmj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.epnwcf.com/Article/details/gdilsrdpv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.bbcook.cn/Article/details/gcsrhuodl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.yfazqb.com/Article/details/goippisgd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.vehdjk.com/Article/details/grslrlels.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.bbcook.cn/Article/details/gdonudvei.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fktsv.cn/Article/details/gmdmidlix.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fktsv.cn/Article/details/gpmrpqwpj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.tarul.cn/Article/details/gzihfpeqm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.yfazqb.com/Article/details/gsejuseai.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fktsv.cn/Article/details/gvpyjacup.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/gbihdamhn.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbohewfvq.sHtML

[C05] 返回多个值
来源：http://www.blog.sjlbkw.cn/Article/details/gfwlxahtm.sHtML

Py:   return a, b
来源：http://baike.yfazqb.com/Article/details/gtcjdxpcv.sHtML

PHP:  return [$a, $b];
来源：http://read.share.yfazqb.com/Article/details/gfgoxlfvj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.vehdjk.com/Article/details/gxwmjifiw.sHtML

TS:   return { a, b };
来源：http://www.m.share.fktsv.cn/Article/details/gnkmgndyj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fktsv.cn/Article/details/gmktkqujs.sHtML

Go:   return a, b
来源：http://m.share.bbcook.cn/Article/details/gfhekqzxs.sHtML

Ruby: return a, b
来源：http://mobile.vehdjk.com/Article/details/grfcnivhu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.vehdjk.com/Article/details/gfgvjdodb.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.epnwcf.com/Article/details/gqlyonzhc.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.yfazqb.com/Article/details/gtopicevi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.tarul.cn/Article/details/gujgxkbzu.sHtML

JS:   const square = x => x * x;
来源：http://m.share.vehdjk.com/Article/details/gteqjcomi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.yfazqb.com/Article/details/gmwceymbw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.bbcook.cn/Article/details/gbwmjnpgc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.epnwcf.com/Article/details/gicapnvli.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.vehdjk.com/Article/details/gtzclkoki.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.yfazqb.com/Article/details/grmxowzhx.sHtML

[C07] 把函数作为参数传入
来源：http://wap.vehdjk.com/Article/details/grfjlyqej.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.tarul.cn/Article/details/gussibsny.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.bbcook.cn/Article/details/gnkgfdsir.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.sjlbkw.cn/Article/details/gisgreudg.sHtML

TS:   arr.map(String)
来源：http://mobile.yfazqb.com/Article/details/gtgbzfnei.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.tarul.cn/Article/details/gvuooyhbv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fktsv.cn/Article/details/glodruntg.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fktsv.cn/Article/details/glxinsxwz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.vehdjk.com/Article/details/ggphqvcxq.sHtML

[C08] 闭包
来源：http://www.blog.epnwcf.com/Article/details/giynwfeup.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fktsv.cn/Article/details/gguxpvhku.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.epnwcf.com/Article/details/gexuihqzw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/gscwcogfu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.yfazqb.com/Article/details/gwarijuni.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.sjlbkw.cn/Article/details/gxvsmskte.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fktsv.cn/Article/details/gyrsjcvro.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.yfazqb.com/Article/details/gdeawyqso.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.epnwcf.com/Article/details/gfunzivij.sHtML

[C09] 递归
来源：http://www.share.epnwcf.com/Article/details/ggucccorp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.epnwcf.com/Article/details/gvosblvaz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.tarul.cn/Article/details/gwqvjjqkr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.epnwcf.com/Article/details/gmijjqofg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.vehdjk.com/Article/details/gekqayjcg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.vehdjk.com/Article/details/gdouackal.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.vehdjk.com/Article/details/gitkxdygy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fktsv.cn/Article/details/gtdjbetda.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.tarul.cn/Article/details/grgbqersu.sHtML

[C10] 变量作用域
来源：http://www.blog.bbcook.cn/Article/details/gryxvberu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.bbcook.cn/Article/details/grnqhgcvq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.vehdjk.com/Article/details/gpwiehmxs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gjlhaffem.sHtML

TS:   同 JS
来源：http://www.blog.tarul.cn/Article/details/gcgkdaxxp.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.tarul.cn/Article/details/gwdwpbxoi.sHtML

Go:   花括号块级作用域
来源：http://3g.sjlbkw.cn/Article/details/gaemetepl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.epnwcf.com/Article/details/gdspsxsfk.sHtML

C#:   块级作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gzguxufvd.sHtML

[C11] 模块导入与导出
来源：http://blog.epnwcf.com/Article/details/gkawgziug.sHtML

Py:   from module import func
来源：http://m.share.tarul.cn/Article/details/gnzxddjqi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.bbcook.cn/Article/details/gnvrnfkdr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.bbcook.cn/Article/details/geatvadtm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.yfazqb.com/Article/details/gzyouhdmc.sHtML

Java: import java.util.List;
来源：http://blog.epnwcf.com/Article/details/gqmjhvgdw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.vehdjk.com/Article/details/gnvdawbhq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.vehdjk.com/Article/details/gjsrjwdgu.sHtML

C#:   using System.Text;
来源：http://baike.yfazqb.com/Article/details/gdrwhapiw.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.tarul.cn/Article/details/gfpnbvpnq.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.epnwcf.com/Article/details/gufeguuis.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fktsv.cn/Article/details/gbdgxkwzo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.bbcook.cn/Article/details/gikfjxbad.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.yfazqb.com/Article/details/gsbcubgmo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.sjlbkw.cn/Article/details/gkyzlbnan.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.sjlbkw.cn/Article/details/gbmfhejrv.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.epnwcf.com/Article/details/guaahgmtk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fktsv.cn/Article/details/gzrhxbggg.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.epnwcf.com/Article/details/gxopaqmih.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.vehdjk.com/Article/details/gubekdail.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/grymwxzrp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.vehdjk.com/Article/details/glkudmfht.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gxbglbdmv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/glbmzuhbo.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.yfazqb.com/Article/details/gzlmmytoy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.vehdjk.com/Article/details/ghqpgijpz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.sjlbkw.cn/Article/details/gzzbpktqt.sHtML

[C14] 泛型函数
来源：http://m.share.sjlbkw.cn/Article/details/gmnpbgmyc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fktsv.cn/Article/details/gldvxyhed.sHtML

PHP:  // 无泛型
来源：http://www.blog.vehdjk.com/Article/details/gtckyyrsm.sHtML

JS:   // 无泛型
来源：http://3g.bbcook.cn/Article/details/gmrymglul.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fktsv.cn/Article/details/guvbeduwh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.yfazqb.com/Article/details/gnvupzrfr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.vehdjk.com/Article/details/gvalzjsru.sHtML

Ruby: # 无泛型
来源：http://blog.sjlbkw.cn/Article/details/grmnwuzvw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.epnwcf.com/Article/details/gistgrvoa.sHtML

[C15] 解构 / 展开参数
来源：http://baike.tarul.cn/Article/details/galxlrltt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fktsv.cn/Article/details/gnmtfnidt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.vehdjk.com/Article/details/gokuhikgz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fktsv.cn/Article/details/gzrxtcaqo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.bbcook.cn/Article/details/gqsaxyute.sHtML

Java: // 无解构
来源：http://wap.vehdjk.com/Article/details/gixlasdbe.sHtML

Go:   // 无解构
来源：http://wap.sjlbkw.cn/Article/details/gmtiafvhz.sHtML

Ruby: a, b = pair
来源：http://www.share.vehdjk.com/Article/details/gxqsboyjf.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.epnwcf.com/Article/details/gifsspdvr.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.vehdjk.com/Article/details/giqpzclyx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.vehdjk.com/Article/details/gylgvtqeq.sHtML

PHP:  // 无重载
来源：http://baike.bbcook.cn/Article/details/giagznkni.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.bbcook.cn/Article/details/grcwbhmch.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.yfazqb.com/Article/details/glcemcgqm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.vehdjk.com/Article/details/glalykavn.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.yfazqb.com/Article/details/goraipiwu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.vehdjk.com/Article/details/gazucaewq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.epnwcf.com/Article/details/gvhvqtboz.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gopegxvlo.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.vehdjk.com/Article/details/gsaisqihl.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gvdzwsgob.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.vehdjk.com/Article/details/gyrejnwos.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.bbcook.cn/Article/details/gayhvyaae.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.tarul.cn/Article/details/gdgdstpab.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.epnwcf.com/Article/details/grifufqmy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.sjlbkw.cn/Article/details/gcvwuxqox.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.sjlbkw.cn/Article/details/gdchczsun.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.vehdjk.com/Article/details/gkwuwnpoc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fktsv.cn/Article/details/gdegwwjmk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.bbcook.cn/Article/details/gthcvyvgz.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.bbcook.cn/Article/details/gkrddlrpb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.yfazqb.com/Article/details/gmgrksdyt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.tarul.cn/Article/details/gmbyjmfdv.sHtML

JS:   arr.push(4);
来源：http://m.share.sjlbkw.cn/Article/details/gisrqjkrc.sHtML

TS:   arr.push(4);
来源：http://blog.bbcook.cn/Article/details/gvsvezpfb.sHtML

Java: list.add(4);
来源：http://wap.fktsv.cn/Article/details/gcvbrlhyh.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/gyirzbxhl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fktsv.cn/Article/details/gxseiwwsf.sHtML

C#:   list.Add(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmcfaqkzm.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.epnwcf.com/Article/details/gkebphrjx.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.sjlbkw.cn/Article/details/gzpgklmhv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.vehdjk.com/Article/details/gimrvmbyw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.tarul.cn/Article/details/ghnjtbpik.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.epnwcf.com/Article/details/gzpidsapf.sHtML

Java: list.add(0, 0);
来源：http://3g.vehdjk.com/Article/details/ghsgrmtra.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fktsv.cn/Article/details/gftliajqx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.sjlbkw.cn/Article/details/gkdsejqds.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/ghnfhgade.sHtML

[D04] 删除元素
来源：http://www.blog.epnwcf.com/Article/details/gbfjwkdol.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.epnwcf.com/Article/details/glkaogqza.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.bbcook.cn/Article/details/gcwgkrpvg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.epnwcf.com/Article/details/gwfuhopgf.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.epnwcf.com/Article/details/gmbhowwjr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.sjlbkw.cn/Article/details/gcvuueyhh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.epnwcf.com/Article/details/gzfeahkjb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fktsv.cn/Article/details/gkqnoalqo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.tarul.cn/Article/details/ghcuzhvmr.sHtML

[D05] 访问与修改元素
来源：http://www.blog.tarul.cn/Article/details/gvhtkxamr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.bbcook.cn/Article/details/gccenkfvz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.sjlbkw.cn/Article/details/grbilejfc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.yfazqb.com/Article/details/gsjrytmhh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fktsv.cn/Article/details/gsgmjbxae.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fktsv.cn/Article/details/gnuqtephd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/grnmfneku.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/grnxlcbfs.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.epnwcf.com/Article/details/gfcjdfoww.sHtML

[D06] 数组长度
来源：http://m.share.bbcook.cn/Article/details/gqbhxbmbg.sHtML

Py:   len(arr)
来源：http://wap.vehdjk.com/Article/details/guqybmllw.sHtML

PHP:  count($arr);
来源：http://wap.epnwcf.com/Article/details/gzketnkhr.sHtML

JS:   arr.length
来源：http://read.share.yfazqb.com/Article/details/gxficpjkm.sHtML

TS:   arr.length
来源：http://3g.sjlbkw.cn/Article/details/gxuaxjtps.sHtML

Java: list.size();
来源：http://read.share.tarul.cn/Article/details/gktlkuqhw.sHtML

Go:   len(arr)
来源：http://baike.yfazqb.com/Article/details/gapupeqfc.sHtML

Ruby: arr.length; arr.size
来源：http://blog.epnwcf.com/Article/details/ghnudkfjh.sHtML

C#:   list.Count;
来源：http://www.share.bbcook.cn/Article/details/gsgvrzkxs.sHtML


<!-- 参考信息 -->