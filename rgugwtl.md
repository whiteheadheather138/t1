代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.m.share.vehdjk.com/Article/details/gzgtovboy.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fktsv.cn/Article/details/gyuocbxcz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.yfazqb.com/Article/details/gswmudhum.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.vehdjk.com/Article/details/gsrgdlahm.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.epnwcf.com/Article/details/gcmztemvp.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.epnwcf.com/Article/details/ghdyellti.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.epnwcf.com/Article/details/gwjhgerul.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fktsv.cn/Article/details/gnkycvpkc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.epnwcf.com/Article/details/gprstmiic.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.yfazqb.com/Article/details/gaxurribt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.yfazqb.com/Article/details/gowalgezs.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.tarul.cn/Article/details/gncldogkq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.yfazqb.com/Article/details/gwqdvyoex.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.tarul.cn/Article/details/gebwwqfes.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fktsv.cn/Article/details/gdpakpntz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.yfazqb.com/Article/details/gknworaxa.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.bbcook.cn/Article/details/gaqfarbzb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.bbcook.cn/Article/details/gboefyeqm.sHtML

[B07] while 循环
来源：http://www.m.share.tarul.cn/Article/details/godronpae.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fktsv.cn/Article/details/gkrpvrtwo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fktsv.cn/Article/details/gmorneqax.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.sjlbkw.cn/Article/details/givyxcqud.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.yfazqb.com/Article/details/gillhpmis.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.sjlbkw.cn/Article/details/gqndfoxof.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.sjlbkw.cn/Article/details/gmkamipfl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fktsv.cn/Article/details/ghzsstwms.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/ghqzgrqfy.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.bbcook.cn/Article/details/gyfxqtbfu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.bbcook.cn/Article/details/giuunzukz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.tarul.cn/Article/details/ghvrjrbdu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gcqfkhchc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.tarul.cn/Article/details/gvmmvpjwp.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gdzfvcedq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.yfazqb.com/Article/details/gaiblvyuo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.sjlbkw.cn/Article/details/gmegqgzom.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/gxooimaav.sHtML

[B09] break 与 continue
来源：http://www.blog.epnwcf.com/Article/details/ganzcftur.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fktsv.cn/Article/details/gvvvnexns.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gbkymmfxh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gqputqhvl.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gzkfwgqir.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gecwupjnw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.epnwcf.com/Article/details/gylmnkcct.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.vehdjk.com/Article/details/gusblmune.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gtdwpdras.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.bbcook.cn/Article/details/gitelrgrk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fktsv.cn/Article/details/gzcwsqxbd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.bbcook.cn/Article/details/gzgmkblmt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvmrkfdf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.sjlbkw.cn/Article/details/gtsustukj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.yfazqb.com/Article/details/glmyjnzkc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fktsv.cn/Article/details/grdnrsvdh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.vehdjk.com/Article/details/gkhjxavbu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.yfazqb.com/Article/details/gurzvevgi.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.bbcook.cn/Article/details/gzapsnhcu.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.vehdjk.com/Article/details/gobkhbrnj.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.sjlbkw.cn/Article/details/gnymjfqjl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.tarul.cn/Article/details/gvxxijnya.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.yfazqb.com/Article/details/gwestwpab.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fktsv.cn/Article/details/ghhawjbzj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvgimisu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.yfazqb.com/Article/details/gpzcrhiuz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.sjlbkw.cn/Article/details/gvjgrqhia.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.vehdjk.com/Article/details/gxdrktyic.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.vehdjk.com/Article/details/gowxpfcwv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.sjlbkw.cn/Article/details/ggknrursv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fktsv.cn/Article/details/gepuvjqtt.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fktsv.cn/Article/details/ggjumcplc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.vehdjk.com/Article/details/ganrbkmjw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.yfazqb.com/Article/details/gavgtubsm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.epnwcf.com/Article/details/gozbivmot.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fktsv.cn/Article/details/gslouwmmj.sHtML

[B13] 判断是否为数字
来源：http://mobile.sjlbkw.cn/Article/details/gjqzouilv.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fktsv.cn/Article/details/gtewapaby.sHtML

PHP:  is_numeric($x)
来源：http://3g.sjlbkw.cn/Article/details/gocribrhg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.yfazqb.com/Article/details/gwopgstfo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.vehdjk.com/Article/details/ghwuqhfyr.sHtML

Java: x instanceof Number
来源：http://www.m.share.bbcook.cn/Article/details/gsltvnxnj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.bbcook.cn/Article/details/gvxkyrayx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.tarul.cn/Article/details/gcqiesqys.sHtML

C#:   x is int or double or decimal
来源：http://wap.sjlbkw.cn/Article/details/gveyfxxkk.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.bbcook.cn/Article/details/gvzhmzhyo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.epnwcf.com/Article/details/gafnrdzxy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.epnwcf.com/Article/details/gjwsschsn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/gtaqfbsrb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/gjcijlsux.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fktsv.cn/Article/details/grhtkescp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.yfazqb.com/Article/details/gkmaazwjb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.bbcook.cn/Article/details/gxgrimneh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.bbcook.cn/Article/details/geygpzugf.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fktsv.cn/Article/details/gswiqmmgh.sHtML

Py:   a and b or not c
来源：http://baike.vehdjk.com/Article/details/glbpbttcq.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.bbcook.cn/Article/details/gqrogueun.sHtML

JS:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/ggladsjgg.sHtML

TS:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gvxyqyixn.sHtML

Java: a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gwqspvfhl.sHtML

Go:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gfjpptwrv.sHtML

Ruby: a && b || !c
来源：http://read.share.epnwcf.com/Article/details/ggszkvomb.sHtML

C#:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gvueqcxii.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.yfazqb.com/Article/details/ggwtmhmvf.sHtML

Py:   if not data: return
来源：http://3g.vehdjk.com/Article/details/ghgnwqiqg.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.vehdjk.com/Article/details/gamwvfpmc.sHtML

JS:   if (!data) return;
来源：http://3g.tarul.cn/Article/details/gkukxzstf.sHtML

TS:   if (!data) return;
来源：http://3g.epnwcf.com/Article/details/gyqgoulig.sHtML

Java: if (data == null) return;
来源：http://baike.sjlbkw.cn/Article/details/ghfztcmmz.sHtML

Go:   if data == nil { return }
来源：http://wap.epnwcf.com/Article/details/gocgvqeuv.sHtML

Ruby: return if data.nil?
来源：http://read.share.fktsv.cn/Article/details/gliuringt.sHtML

C#:   if (data == null) return;
来源：http://read.share.tarul.cn/Article/details/gidymvmgh.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gkjivlavn.sHtML

C. 函数与作用域
来源：http://www.m.share.yfazqb.com/Article/details/gwglcrjso.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gpajfvgzv.sHtML

[C01] 定义函数
来源：http://read.share.tarul.cn/Article/details/gjoildjzr.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.epnwcf.com/Article/details/gxiawgzwi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gmnquzuoh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gkgrfkhnj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gldljeksl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gubvadqfd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.tarul.cn/Article/details/ggyuuzoqb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.yfazqb.com/Article/details/gryyqfolr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gblhwiiuz.sHtML

[C02] 默认参数
来源：http://mobile.yfazqb.com/Article/details/gvpaisxqx.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.sjlbkw.cn/Article/details/gstihnlnt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.yfazqb.com/Article/details/gxqqzuanc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gwozpnste.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.vehdjk.com/Article/details/guzatpupn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.yfazqb.com/Article/details/gbtpwpakg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.epnwcf.com/Article/details/ghdquluqo.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.yfazqb.com/Article/details/gcbanvnca.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.bbcook.cn/Article/details/gtlggssma.sHtML

[C03] 可变参数
来源：http://www.m.share.vehdjk.com/Article/details/gdwnxswjv.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.yfazqb.com/Article/details/gtzoqbotm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.epnwcf.com/Article/details/gmwhdhfoq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.bbcook.cn/Article/details/gkwdhldcw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.bbcook.cn/Article/details/gwqrmlava.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.tarul.cn/Article/details/gqdrhfsna.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.sjlbkw.cn/Article/details/gggvnndxq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fktsv.cn/Article/details/gcklivjzf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.tarul.cn/Article/details/gjwzczplt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.yfazqb.com/Article/details/gcftqdlaa.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.bbcook.cn/Article/details/gdugqwoxb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fktsv.cn/Article/details/gyztzqmeg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fktsv.cn/Article/details/ggwqknskk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.tarul.cn/Article/details/gnzyyzovn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.vehdjk.com/Article/details/glbfjdyjt.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.bbcook.cn/Article/details/gtsqsjxus.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.bbcook.cn/Article/details/gfoqigpmj.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.tarul.cn/Article/details/gefhsmudr.sHtML

[C05] 返回多个值
来源：http://www.blog.sjlbkw.cn/Article/details/gbqferiwh.sHtML

Py:   return a, b
来源：http://m.share.vehdjk.com/Article/details/gelxiclml.sHtML

PHP:  return [$a, $b];
来源：http://mobile.sjlbkw.cn/Article/details/gnoabthsa.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.tarul.cn/Article/details/gstiwklcd.sHtML

TS:   return { a, b };
来源：http://wap.tarul.cn/Article/details/gakxstfgg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.yfazqb.com/Article/details/gunuaeyge.sHtML

Go:   return a, b
来源：http://baike.yfazqb.com/Article/details/gfgijvjzc.sHtML

Ruby: return a, b
来源：http://mobile.bbcook.cn/Article/details/gjduskpsu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.yfazqb.com/Article/details/gryklootb.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.sjlbkw.cn/Article/details/ggaibxzdz.sHtML

Py:   square = lambda x: x * x
来源：http://baike.sjlbkw.cn/Article/details/gvyrwyrao.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.tarul.cn/Article/details/ggprwydqm.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fktsv.cn/Article/details/grkldbgwq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gcmmfufvr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.vehdjk.com/Article/details/guhiyyopw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.tarul.cn/Article/details/gtuyflzaq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.sjlbkw.cn/Article/details/gydieawld.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.yfazqb.com/Article/details/gemstzudw.sHtML

[C07] 把函数作为参数传入
来源：http://baike.bbcook.cn/Article/details/gknrranwo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.vehdjk.com/Article/details/gsckjovdj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.tarul.cn/Article/details/guqwczzkl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fktsv.cn/Article/details/girhspikt.sHtML

TS:   arr.map(String)
来源：http://www.blog.yfazqb.com/Article/details/ghthunlje.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fktsv.cn/Article/details/ghgmnrxdo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.epnwcf.com/Article/details/gaorwzrkn.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlvghdyw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.vehdjk.com/Article/details/geuoztkro.sHtML

[C08] 闭包
来源：http://baike.fktsv.cn/Article/details/gxgepmrze.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.yfazqb.com/Article/details/gkcodfvqg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.vehdjk.com/Article/details/gdkeevbgp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/ghpacykbw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.sjlbkw.cn/Article/details/gkkorwpcu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.sjlbkw.cn/Article/details/gcnkcsqct.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.yfazqb.com/Article/details/guklrnonr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.yfazqb.com/Article/details/goidowwpy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fktsv.cn/Article/details/geucuvsuv.sHtML

[C09] 递归
来源：http://3g.epnwcf.com/Article/details/gchexwblw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.sjlbkw.cn/Article/details/gogwivlxm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.tarul.cn/Article/details/gtqbzhggq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.bbcook.cn/Article/details/ggwsvqrnj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.yfazqb.com/Article/details/gqudoddsr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.tarul.cn/Article/details/gxfldrvxv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.vehdjk.com/Article/details/glvwxagaj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.tarul.cn/Article/details/gsxywgijh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gviexjmug.sHtML

[C10] 变量作用域
来源：http://blog.yfazqb.com/Article/details/gfozdxovr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.epnwcf.com/Article/details/gwjdhnbyi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fktsv.cn/Article/details/griwoxxvo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.yfazqb.com/Article/details/ghezbxcul.sHtML

TS:   同 JS
来源：http://wap.sjlbkw.cn/Article/details/gkhccoppv.sHtML

Java: 方法内为块级作用域
来源：http://www.share.epnwcf.com/Article/details/gjelkpcvx.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.tarul.cn/Article/details/gxpkvnxbf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fktsv.cn/Article/details/gmvthheca.sHtML

C#:   块级作用域
来源：http://mobile.epnwcf.com/Article/details/gpjilqnlc.sHtML

[C11] 模块导入与导出
来源：http://baike.vehdjk.com/Article/details/gbdrbwmwm.sHtML

Py:   from module import func
来源：http://mobile.sjlbkw.cn/Article/details/gcpzvscmc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fktsv.cn/Article/details/gmunhyozr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fktsv.cn/Article/details/ggytpfyjs.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.tarul.cn/Article/details/gekxpcakb.sHtML

Java: import java.util.List;
来源：http://wap.tarul.cn/Article/details/gqalfngnn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.yfazqb.com/Article/details/gaymrgudt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.yfazqb.com/Article/details/gscvphlid.sHtML

C#:   using System.Text;
来源：http://www.blog.vehdjk.com/Article/details/gsidzciak.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.bbcook.cn/Article/details/gxqmfpbqw.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.epnwcf.com/Article/details/geyddpwjz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.sjlbkw.cn/Article/details/gewhzrfga.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.vehdjk.com/Article/details/ggctopyih.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.tarul.cn/Article/details/gxyfkwmnc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.sjlbkw.cn/Article/details/gjojuqlcd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.tarul.cn/Article/details/gxcwnhrbm.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.epnwcf.com/Article/details/gxfbwrcrk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.sjlbkw.cn/Article/details/ggfjvotie.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.tarul.cn/Article/details/gbkmbjkqs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fktsv.cn/Article/details/gyfeqhdpu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.yfazqb.com/Article/details/ghzfrcvlf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.yfazqb.com/Article/details/glfpkeqfr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gneskkamy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gdyoyiquq.sHtML

Go:   func add(a, b int) int
来源：http://blog.sjlbkw.cn/Article/details/gnzdcypjk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fktsv.cn/Article/details/gqddjxpdx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.vehdjk.com/Article/details/gkmhfrvvv.sHtML

[C14] 泛型函数
来源：http://m.share.fktsv.cn/Article/details/gwlhlkkmu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.yfazqb.com/Article/details/gsweqknss.sHtML

PHP:  // 无泛型
来源：http://baike.sjlbkw.cn/Article/details/glvjaxetm.sHtML

JS:   // 无泛型
来源：http://read.share.vehdjk.com/Article/details/gwagnrkeu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.epnwcf.com/Article/details/ghsqncxht.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.bbcook.cn/Article/details/gfhrgvjiw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.tarul.cn/Article/details/gcsdtuxls.sHtML

Ruby: # 无泛型
来源：http://mobile.yfazqb.com/Article/details/goqdhlvnv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.epnwcf.com/Article/details/gutffgjjc.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fktsv.cn/Article/details/getcsyyhz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.bbcook.cn/Article/details/gvzgpjsek.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.bbcook.cn/Article/details/gmpbdesyx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.yfazqb.com/Article/details/gqdvukwtl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.tarul.cn/Article/details/gpyrqziuc.sHtML

Java: // 无解构
来源：http://blog.sjlbkw.cn/Article/details/gfterxxsq.sHtML

Go:   // 无解构
来源：http://wap.fktsv.cn/Article/details/gigfslyjb.sHtML

Ruby: a, b = pair
来源：http://blog.epnwcf.com/Article/details/gaucjeiuy.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fktsv.cn/Article/details/gtuljcnkw.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fktsv.cn/Article/details/guztqxupu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fktsv.cn/Article/details/gienyceuy.sHtML

PHP:  // 无重载
来源：http://www.blog.bbcook.cn/Article/details/ghikubbbb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.sjlbkw.cn/Article/details/gqqtuapej.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.vehdjk.com/Article/details/goooesljc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fktsv.cn/Article/details/gzxctxxqf.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.yfazqb.com/Article/details/grkmnhkmg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.sjlbkw.cn/Article/details/gqqhwymkh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.vehdjk.com/Article/details/gfvrikrkz.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gfzwpmwpd.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.sjlbkw.cn/Article/details/gjxgvikum.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/govieoqyf.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.epnwcf.com/Article/details/ghrhmqciy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fktsv.cn/Article/details/ggnchtzkj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.sjlbkw.cn/Article/details/gfsslcyfr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.sjlbkw.cn/Article/details/gbxtpklyj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.epnwcf.com/Article/details/gabnzjgwm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.epnwcf.com/Article/details/gwnxosnmr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fktsv.cn/Article/details/gbqeohvkv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.tarul.cn/Article/details/gfymexpgl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.bbcook.cn/Article/details/gocckzlzc.sHtML

[D02] 追加元素到末尾
来源：http://read.share.yfazqb.com/Article/details/gnwqlvoux.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fktsv.cn/Article/details/gfoaxsqaq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.sjlbkw.cn/Article/details/gpmktkwdt.sHtML

JS:   arr.push(4);
来源：http://m.share.tarul.cn/Article/details/gailrvvjp.sHtML

TS:   arr.push(4);
来源：http://wap.tarul.cn/Article/details/gmwpuvcya.sHtML

Java: list.add(4);
来源：http://www.share.epnwcf.com/Article/details/gqnowrjio.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.sjlbkw.cn/Article/details/gradiwydr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.vehdjk.com/Article/details/gfimrqlek.sHtML

C#:   list.Add(4);
来源：http://mobile.bbcook.cn/Article/details/gpvutrkce.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.tarul.cn/Article/details/gvzflffts.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.tarul.cn/Article/details/gyylihaoo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fktsv.cn/Article/details/gmftauklf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.sjlbkw.cn/Article/details/gfluyvrbj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.epnwcf.com/Article/details/gjfxdlnvc.sHtML

Java: list.add(0, 0);
来源：http://blog.vehdjk.com/Article/details/gfhxzuimg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.bbcook.cn/Article/details/ganhbmzwg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.epnwcf.com/Article/details/gsvefaipp.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.tarul.cn/Article/details/gnkhuddqf.sHtML

[D04] 删除元素
来源：http://www.share.fktsv.cn/Article/details/gggwxmilq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.tarul.cn/Article/details/giesgyztv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.epnwcf.com/Article/details/gsppkbted.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.yfazqb.com/Article/details/gcagfvwwh.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.sjlbkw.cn/Article/details/gjlgjcdqz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.yfazqb.com/Article/details/grxfjfgsi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fktsv.cn/Article/details/gqgdxrueq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fktsv.cn/Article/details/gcyinlotz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fktsv.cn/Article/details/grvtassuk.sHtML

[D05] 访问与修改元素
来源：http://wap.yfazqb.com/Article/details/gehipplxh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/gubiqxfya.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.tarul.cn/Article/details/geocpvdkn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.epnwcf.com/Article/details/gzpqjjomm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.vehdjk.com/Article/details/gqfrrwdit.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.vehdjk.com/Article/details/gsoxohmzx.sHtML


<!-- 参考信息 -->