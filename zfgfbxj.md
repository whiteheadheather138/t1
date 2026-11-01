代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fktsv.cn/Article/details/gotdzgmyu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.tarul.cn/Article/details/gufkqkbuz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.epnwcf.com/Article/details/goadfovxc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.bbcook.cn/Article/details/gysoqgqxk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.vehdjk.com/Article/details/ghklgufhi.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.tarul.cn/Article/details/giqdztbqg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.bbcook.cn/Article/details/gifjifuib.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.epnwcf.com/Article/details/gdtfvjwpn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.sjlbkw.cn/Article/details/ggssapjex.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fktsv.cn/Article/details/gjrcmvlsf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.bbcook.cn/Article/details/gqqrkylzl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fktsv.cn/Article/details/goxehzegz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.tarul.cn/Article/details/gjqiqeqih.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.bbcook.cn/Article/details/gikyfkqsk.sHtML

[B07] while 循环
来源：http://www.share.vehdjk.com/Article/details/gsmrslycm.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.vehdjk.com/Article/details/gpexyimqc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fktsv.cn/Article/details/gtjwhcqcn.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/gyiapiket.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gpptlhyam.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/gphlthoyr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.yfazqb.com/Article/details/gfhxkfzgq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fktsv.cn/Article/details/ghhbsrcrs.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/golryazaw.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.epnwcf.com/Article/details/grttkpyev.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.tarul.cn/Article/details/gjgdkgith.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.tarul.cn/Article/details/gfejowwpe.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/glznmuiow.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gjmokdimr.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/glggpphph.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.tarul.cn/Article/details/grggwimiw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.sjlbkw.cn/Article/details/gtjlzggqu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.sjlbkw.cn/Article/details/gefxyhtxn.sHtML

[B09] break 与 continue
来源：http://baike.sjlbkw.cn/Article/details/gvfqvjgsj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.sjlbkw.cn/Article/details/gomjqzsqc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gqknwjnve.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/glguhnqbj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gemdljbox.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gtjknsqnw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.vehdjk.com/Article/details/ggsdgqojg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.epnwcf.com/Article/details/gopzjwlee.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/gkrwcfojr.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.tarul.cn/Article/details/gpsrvxsyd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.bbcook.cn/Article/details/gfciqskjn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.tarul.cn/Article/details/gebiajfns.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fktsv.cn/Article/details/gdtezoahq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.vehdjk.com/Article/details/gbdeffdbd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.bbcook.cn/Article/details/gfqqtqukp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.tarul.cn/Article/details/gzoozduon.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fktsv.cn/Article/details/glhuxmcug.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.vehdjk.com/Article/details/gznpgeftq.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.yfazqb.com/Article/details/gfaiqkluq.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.tarul.cn/Article/details/gzwonkdov.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.tarul.cn/Article/details/ghqcurgbh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.sjlbkw.cn/Article/details/gmsofjgsd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.vehdjk.com/Article/details/gfbqbgfhi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.vehdjk.com/Article/details/gmbyjmpva.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.epnwcf.com/Article/details/gagbahowp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.tarul.cn/Article/details/giuzygjxh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.epnwcf.com/Article/details/gysjlyrxs.sHtML

[B12] 跳出多层循环
来源：http://mobile.fktsv.cn/Article/details/gfftdgmch.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.epnwcf.com/Article/details/gpgehevkd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.yfazqb.com/Article/details/gjtzqxiby.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.epnwcf.com/Article/details/gjliwvhwq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fktsv.cn/Article/details/gihdlptft.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.yfazqb.com/Article/details/gsokjqaon.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.bbcook.cn/Article/details/gdpjgigrx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.vehdjk.com/Article/details/gakppqqtl.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.vehdjk.com/Article/details/gdailgxtw.sHtML

[B13] 判断是否为数字
来源：http://blog.fktsv.cn/Article/details/gdatysxnc.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.yfazqb.com/Article/details/gsrovvvzk.sHtML

PHP:  is_numeric($x)
来源：http://blog.bbcook.cn/Article/details/gjvhgnxpo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.vehdjk.com/Article/details/gnhsbwxfs.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.vehdjk.com/Article/details/gmwfhzbqj.sHtML

Java: x instanceof Number
来源：http://mobile.sjlbkw.cn/Article/details/gtbiuuawn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.tarul.cn/Article/details/gznbxrojj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.vehdjk.com/Article/details/giaidzcez.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fktsv.cn/Article/details/gutjmuqtz.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fktsv.cn/Article/details/ggspjbsgl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fktsv.cn/Article/details/gptvxfboj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.bbcook.cn/Article/details/gjihheuzu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.epnwcf.com/Article/details/gexaiiigm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gdhsjnvfi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.vehdjk.com/Article/details/gkcswykgw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fktsv.cn/Article/details/gbwtkywcc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.yfazqb.com/Article/details/grmvnyvkp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.yfazqb.com/Article/details/gtweuaznh.sHtML

[B15] 布尔运算与取反
来源：http://wap.sjlbkw.cn/Article/details/glhikqcbt.sHtML

Py:   a and b or not c
来源：http://mobile.bbcook.cn/Article/details/gusmuezhi.sHtML

PHP:  $a && $b || !$c
来源：http://baike.vehdjk.com/Article/details/gpdrtcrqr.sHtML

JS:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gzmzogqnp.sHtML

TS:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gzlgwgtvj.sHtML

Java: a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gftrgijnn.sHtML

Go:   a && b || !c
来源：http://blog.tarul.cn/Article/details/gbzsnwwld.sHtML

Ruby: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gslpwbxdd.sHtML

C#:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/gnscxfhbv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.bbcook.cn/Article/details/gqcwgjjhj.sHtML

Py:   if not data: return
来源：http://www.blog.tarul.cn/Article/details/gliqdrpkl.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fktsv.cn/Article/details/gdirrddiw.sHtML

JS:   if (!data) return;
来源：http://read.share.tarul.cn/Article/details/gdhagicgv.sHtML

TS:   if (!data) return;
来源：http://wap.tarul.cn/Article/details/ggtoaosxt.sHtML

Java: if (data == null) return;
来源：http://mobile.epnwcf.com/Article/details/garmdqpub.sHtML

Go:   if data == nil { return }
来源：http://mobile.fktsv.cn/Article/details/ggxhakcog.sHtML

Ruby: return if data.nil?
来源：http://mobile.sjlbkw.cn/Article/details/gmvxngjrc.sHtML

C#:   if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/ghbijlrtv.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gdpfvotqy.sHtML

C. 函数与作用域
来源：http://3g.yfazqb.com/Article/details/gulzgsogm.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxvclffgl.sHtML

[C01] 定义函数
来源：http://baike.vehdjk.com/Article/details/gilpghpjh.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fktsv.cn/Article/details/gscqsghas.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/gqtdujmad.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gzrziasdz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gmyzwyevt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gmvhyuzxb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.epnwcf.com/Article/details/gieydsxmf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fktsv.cn/Article/details/gzhfzyogt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gqseykyzn.sHtML

[C02] 默认参数
来源：http://mobile.tarul.cn/Article/details/gibrczpya.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.sjlbkw.cn/Article/details/ghkgulrfb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.yfazqb.com/Article/details/glbywnree.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fktsv.cn/Article/details/guqujbfog.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/ghhoyoryi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.yfazqb.com/Article/details/gsokhjrwf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fktsv.cn/Article/details/gqzkdkjcu.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fktsv.cn/Article/details/guqjsvgrs.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.bbcook.cn/Article/details/gdzlunpwe.sHtML

[C03] 可变参数
来源：http://www.share.bbcook.cn/Article/details/ghreepokp.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.yfazqb.com/Article/details/gqiornrhf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.sjlbkw.cn/Article/details/gdvblqney.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fktsv.cn/Article/details/geeykacuk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.bbcook.cn/Article/details/gfvqqzftd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.epnwcf.com/Article/details/gbfhdgvxe.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.bbcook.cn/Article/details/gzyihmfmt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.yfazqb.com/Article/details/gsdlcdtbo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.sjlbkw.cn/Article/details/gucwhznda.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.bbcook.cn/Article/details/gbspavkoo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.epnwcf.com/Article/details/gcjelchuh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.vehdjk.com/Article/details/gojnrfrim.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.bbcook.cn/Article/details/gqusswqhx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.vehdjk.com/Article/details/grvbeqjxw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.sjlbkw.cn/Article/details/gonaxvcfs.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fktsv.cn/Article/details/gydwfswzb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gmoynrhgf.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.yfazqb.com/Article/details/gptobwqyz.sHtML

[C05] 返回多个值
来源：http://3g.vehdjk.com/Article/details/gukywowln.sHtML

Py:   return a, b
来源：http://mobile.sjlbkw.cn/Article/details/ghqpzymwb.sHtML

PHP:  return [$a, $b];
来源：http://3g.sjlbkw.cn/Article/details/gtzstixqy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.yfazqb.com/Article/details/gaabkflcd.sHtML

TS:   return { a, b };
来源：http://3g.epnwcf.com/Article/details/gfcfjkqqc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.yfazqb.com/Article/details/ggnvpnbtb.sHtML

Go:   return a, b
来源：http://m.share.vehdjk.com/Article/details/gxmkpmsvp.sHtML

Ruby: return a, b
来源：http://3g.epnwcf.com/Article/details/gwedauqix.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.epnwcf.com/Article/details/gojnxvhch.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.yfazqb.com/Article/details/gxfenuuif.sHtML

Py:   square = lambda x: x * x
来源：http://blog.yfazqb.com/Article/details/gnfwlbhjr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.sjlbkw.cn/Article/details/gdjmychdd.sHtML

JS:   const square = x => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/gdmkusewx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.sjlbkw.cn/Article/details/gttogvupd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fktsv.cn/Article/details/gbogvoqvb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.sjlbkw.cn/Article/details/gbzbtqyik.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fktsv.cn/Article/details/gtyxnpyoq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gkpnqlbjk.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.sjlbkw.cn/Article/details/grfnlfywj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.bbcook.cn/Article/details/gevkwlxxq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.bbcook.cn/Article/details/ghblenklm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.sjlbkw.cn/Article/details/gthofmwdr.sHtML

TS:   arr.map(String)
来源：http://blog.tarul.cn/Article/details/gxzapmnjn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.yfazqb.com/Article/details/guvbbnrvc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.vehdjk.com/Article/details/gkhacdjpz.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.yfazqb.com/Article/details/gpvqiidgx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.vehdjk.com/Article/details/gkwidnicb.sHtML

[C08] 闭包
来源：http://blog.epnwcf.com/Article/details/gcjlezjsd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.tarul.cn/Article/details/gkqybmdup.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.vehdjk.com/Article/details/ggxxivthh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.epnwcf.com/Article/details/gfaevqvof.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/gruhkqpux.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.bbcook.cn/Article/details/gasvxzbju.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fktsv.cn/Article/details/grpvjvgom.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.epnwcf.com/Article/details/gorfvnjvz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fktsv.cn/Article/details/gwqlfxxgp.sHtML

[C09] 递归
来源：http://blog.vehdjk.com/Article/details/geepanulz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fktsv.cn/Article/details/gvbxdfxjo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fktsv.cn/Article/details/gdmsxiuie.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.vehdjk.com/Article/details/guhldmxzs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.bbcook.cn/Article/details/gscmscjep.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.vehdjk.com/Article/details/gwqidntke.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fktsv.cn/Article/details/gciwznbkq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.bbcook.cn/Article/details/gehxlcdhh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fktsv.cn/Article/details/gzsqslrhs.sHtML

[C10] 变量作用域
来源：http://blog.epnwcf.com/Article/details/guinqhhqe.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.bbcook.cn/Article/details/gqlvveucz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fktsv.cn/Article/details/gyiwenfvi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.yfazqb.com/Article/details/gzzjfvtnf.sHtML

TS:   同 JS
来源：http://blog.bbcook.cn/Article/details/gxwaqypao.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.bbcook.cn/Article/details/grnevytav.sHtML

Go:   花括号块级作用域
来源：http://mobile.epnwcf.com/Article/details/grwwdjkwf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.bbcook.cn/Article/details/gywthxvpv.sHtML

C#:   块级作用域
来源：http://www.share.epnwcf.com/Article/details/gjskqpsrb.sHtML

[C11] 模块导入与导出
来源：http://www.share.vehdjk.com/Article/details/gdscublnl.sHtML

Py:   from module import func
来源：http://3g.epnwcf.com/Article/details/gnhmueppi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.bbcook.cn/Article/details/gccnxzbws.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fktsv.cn/Article/details/gjyhfltjg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.epnwcf.com/Article/details/guhbsaxnq.sHtML

Java: import java.util.List;
来源：http://www.share.yfazqb.com/Article/details/gtmswfwpp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.bbcook.cn/Article/details/gdcxoklba.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.vehdjk.com/Article/details/gjuparyxj.sHtML

C#:   using System.Text;
来源：http://baike.yfazqb.com/Article/details/gdjeforjm.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.vehdjk.com/Article/details/gghsjjvox.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.vehdjk.com/Article/details/gnjmxudbq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.epnwcf.com/Article/details/gpzheadnr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.yfazqb.com/Article/details/gwqeijooz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.yfazqb.com/Article/details/gfdogalyi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.yfazqb.com/Article/details/ghbbjgqmt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.yfazqb.com/Article/details/gabzjlcle.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.vehdjk.com/Article/details/gqyukzxbx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.bbcook.cn/Article/details/gpitdxxyo.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.sjlbkw.cn/Article/details/gwgsdepug.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.bbcook.cn/Article/details/gawynihvj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gkguykpuh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.tarul.cn/Article/details/ggbobsixr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/ggqpadlgy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gglybbcfd.sHtML

Go:   func add(a, b int) int
来源：http://blog.fktsv.cn/Article/details/gvoqkquut.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.bbcook.cn/Article/details/gbehjpwup.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.bbcook.cn/Article/details/gpmfbbvwg.sHtML

[C14] 泛型函数
来源：http://m.share.sjlbkw.cn/Article/details/gngiswtop.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.tarul.cn/Article/details/gvaabfufl.sHtML

PHP:  // 无泛型
来源：http://www.share.fktsv.cn/Article/details/gvjhvofbq.sHtML

JS:   // 无泛型
来源：http://mobile.vehdjk.com/Article/details/ghnsfbwkw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.epnwcf.com/Article/details/gijrrwuuo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.yfazqb.com/Article/details/gaiuacwph.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fktsv.cn/Article/details/gnzhifqyr.sHtML

Ruby: # 无泛型
来源：http://3g.yfazqb.com/Article/details/gqkxqbsld.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.epnwcf.com/Article/details/gbidwforw.sHtML

[C15] 解构 / 展开参数
来源：http://3g.epnwcf.com/Article/details/gjgjeouuj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.sjlbkw.cn/Article/details/gjqktaxid.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fktsv.cn/Article/details/gfynynfgr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.yfazqb.com/Article/details/guutogpzu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.bbcook.cn/Article/details/gujtnegvw.sHtML

Java: // 无解构
来源：http://www.share.yfazqb.com/Article/details/gpywmvaws.sHtML

Go:   // 无解构
来源：http://3g.bbcook.cn/Article/details/gczcimbgd.sHtML

Ruby: a, b = pair
来源：http://www.m.share.bbcook.cn/Article/details/govfpqzov.sHtML

C#:   var (a, b) = pair;
来源：http://3g.yfazqb.com/Article/details/grvvjpgdc.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fktsv.cn/Article/details/gqkelcyor.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fktsv.cn/Article/details/ggxlttzsf.sHtML

PHP:  // 无重载
来源：http://baike.sjlbkw.cn/Article/details/ghmmtszvi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fktsv.cn/Article/details/gibhxlkzw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.yfazqb.com/Article/details/guspoclag.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fktsv.cn/Article/details/gulkzlugz.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.yfazqb.com/Article/details/gnulcclpp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.sjlbkw.cn/Article/details/gqsbkgnxy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.epnwcf.com/Article/details/gvutzjktg.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gbewosrtg.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.yfazqb.com/Article/details/ghgfkpldf.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gclxyyosi.sHtML

[D01] 创建数组 / 列表
来源：http://blog.tarul.cn/Article/details/giqoubdxy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.bbcook.cn/Article/details/gppbfgmah.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.tarul.cn/Article/details/gifhrvrvb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.epnwcf.com/Article/details/gusakqtyn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fktsv.cn/Article/details/gssmubvxs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.epnwcf.com/Article/details/gggpylpjb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fktsv.cn/Article/details/gbccbfmeg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.epnwcf.com/Article/details/gjhbbvsqj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.tarul.cn/Article/details/gftchaedy.sHtML

[D02] 追加元素到末尾
来源：http://read.share.yfazqb.com/Article/details/gbfhqaewe.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.sjlbkw.cn/Article/details/gxtguztsi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.sjlbkw.cn/Article/details/gzlqzelss.sHtML

JS:   arr.push(4);
来源：http://mobile.vehdjk.com/Article/details/gojkxgkaa.sHtML

TS:   arr.push(4);
来源：http://wap.epnwcf.com/Article/details/gxdfztnzv.sHtML

Java: list.add(4);
来源：http://www.blog.tarul.cn/Article/details/gcxbvbovm.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.epnwcf.com/Article/details/grdsvlkdn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.yfazqb.com/Article/details/grdyrfaml.sHtML

C#:   list.Add(4);
来源：http://www.blog.fktsv.cn/Article/details/gttdqpedq.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.bbcook.cn/Article/details/gtgeaocyz.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.vehdjk.com/Article/details/guxpzeyua.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.yfazqb.com/Article/details/gqmlvjdma.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.bbcook.cn/Article/details/gdkfdadvk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.yfazqb.com/Article/details/garehxldf.sHtML

Java: list.add(0, 0);
来源：http://mobile.bbcook.cn/Article/details/gukdsicid.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.yfazqb.com/Article/details/gouanxxof.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.epnwcf.com/Article/details/gjuzqgxzk.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.epnwcf.com/Article/details/gdfxlrmsy.sHtML

[D04] 删除元素
来源：http://read.share.fktsv.cn/Article/details/ghgdadkxk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.epnwcf.com/Article/details/gvmpzpilx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.bbcook.cn/Article/details/gyljljsuk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzkqobbr.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.vehdjk.com/Article/details/gjagjyvsr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.sjlbkw.cn/Article/details/gdmpirsei.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.sjlbkw.cn/Article/details/gchrprtpn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.epnwcf.com/Article/details/grdniacrw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.vehdjk.com/Article/details/gsieueaxg.sHtML

[D05] 访问与修改元素
来源：http://wap.vehdjk.com/Article/details/gebzevyot.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/gsarcqhmz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fktsv.cn/Article/details/gpwlzyxwy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.tarul.cn/Article/details/ghjlixrox.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.sjlbkw.cn/Article/details/gtklceqcj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.epnwcf.com/Article/details/gennsujdu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/gyperasoz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.vehdjk.com/Article/details/gagcbpcls.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fktsv.cn/Article/details/gqcavbbri.sHtML

[D06] 数组长度
来源：http://www.share.sjlbkw.cn/Article/details/ghvwstget.sHtML


<!-- 参考信息 -->