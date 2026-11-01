代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.sjlbkw.cn/Article/details/gcnrlhdmx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.epnwcf.com/Article/details/gajvwplqm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.fktsv.cn/Article/details/glcrpwsai.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fktsv.cn/Article/details/gwcllrjxg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.yfazqb.com/Article/details/ggmvjamiq.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.tarul.cn/Article/details/gaepvdqag.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.yfazqb.com/Article/details/gmczacrqn.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.yfazqb.com/Article/details/ggzkhittq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.epnwcf.com/Article/details/glmoegave.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.yfazqb.com/Article/details/gkurtlhrk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.epnwcf.com/Article/details/gqlihghgf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.sjlbkw.cn/Article/details/gzzozexkj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.bbcook.cn/Article/details/gdvdaxwyo.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fktsv.cn/Article/details/gbwvytapy.sHtML

[B07] while 循环
来源：http://www.share.vehdjk.com/Article/details/ghxixcrnk.sHtML

Py:   while i < 10: i += 1
来源：http://wap.bbcook.cn/Article/details/gcepajckm.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.bbcook.cn/Article/details/gfcpaluyy.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/gihylnsok.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.vehdjk.com/Article/details/gcaxljzaz.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.tarul.cn/Article/details/gtevlutdr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.bbcook.cn/Article/details/gmfxwrebp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.tarul.cn/Article/details/gmuuubbtf.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gozwjpiud.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.vehdjk.com/Article/details/gatphmndt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.epnwcf.com/Article/details/gvybrjhym.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gmueieaze.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.fktsv.cn/Article/details/gutjfrqmq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/gaiygeufc.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gjkqhsdyq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.epnwcf.com/Article/details/gecqzwsii.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.bbcook.cn/Article/details/gpajtermu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.sjlbkw.cn/Article/details/gnspqmsyt.sHtML

[B09] break 与 continue
来源：http://mobile.sjlbkw.cn/Article/details/gaqtkcbek.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.vehdjk.com/Article/details/ggsbfhkql.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/gzmsuiwpx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gmseabejg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/geapjinxs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.tarul.cn/Article/details/gfteaevbw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.yfazqb.com/Article/details/gxohckmsi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.vehdjk.com/Article/details/gucbytrxu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gjhwngwrr.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fktsv.cn/Article/details/gmcnliuxw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.tarul.cn/Article/details/gxsesguxg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.yfazqb.com/Article/details/gkdplmhjm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.tarul.cn/Article/details/gxzsefjhn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.epnwcf.com/Article/details/gfuhajcmi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.yfazqb.com/Article/details/gdpobufwd.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.tarul.cn/Article/details/gmcrrihcv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.bbcook.cn/Article/details/gyysnxmsp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.epnwcf.com/Article/details/gtefkblmy.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.vehdjk.com/Article/details/gwjjqljfl.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.sjlbkw.cn/Article/details/gzhkgqucl.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.vehdjk.com/Article/details/gpbqdwhji.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.epnwcf.com/Article/details/gydiftnaa.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.vehdjk.com/Article/details/glqrbxcve.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.yfazqb.com/Article/details/gkhziroph.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.sjlbkw.cn/Article/details/girgpmomu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.sjlbkw.cn/Article/details/gtcvjmman.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.epnwcf.com/Article/details/gprsblzdc.sHtML

[B12] 跳出多层循环
来源：http://3g.sjlbkw.cn/Article/details/gwtrluwlm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.tarul.cn/Article/details/gxnbzwdot.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.yfazqb.com/Article/details/gtutfjgxq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fktsv.cn/Article/details/girypkmxx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/gdtdxjpfi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gqtxdtxwi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.vehdjk.com/Article/details/gtvmrqkxh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.tarul.cn/Article/details/gmbgbczta.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.bbcook.cn/Article/details/gpckgzvdp.sHtML

[B13] 判断是否为数字
来源：http://baike.epnwcf.com/Article/details/ggsagbelu.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.bbcook.cn/Article/details/gumrgsrkv.sHtML

PHP:  is_numeric($x)
来源：http://m.share.vehdjk.com/Article/details/guddvzroh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.vehdjk.com/Article/details/ghjavxtbe.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gtmzsfcug.sHtML

Java: x instanceof Number
来源：http://wap.tarul.cn/Article/details/gxrsyehkm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.sjlbkw.cn/Article/details/gcwheebcm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.bbcook.cn/Article/details/gkfascqsv.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.bbcook.cn/Article/details/gkwtfqjru.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.sjlbkw.cn/Article/details/gkvlmbzan.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.vehdjk.com/Article/details/gyudnafip.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.tarul.cn/Article/details/guasbuoab.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.sjlbkw.cn/Article/details/gcperregw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/gtqfwrogt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gchxddppc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.yfazqb.com/Article/details/gawwooljr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fktsv.cn/Article/details/gsmdwjpeb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fktsv.cn/Article/details/gurqpziju.sHtML

[B15] 布尔运算与取反
来源：http://www.share.sjlbkw.cn/Article/details/gyocexezl.sHtML

Py:   a and b or not c
来源：http://blog.bbcook.cn/Article/details/gpxaztjlw.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.epnwcf.com/Article/details/gnqboptyq.sHtML

JS:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gqvramwjo.sHtML

TS:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/ghdftstwq.sHtML

Java: a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gblhmdugy.sHtML

Go:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/gvailptgr.sHtML

Ruby: a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gfgqefjoq.sHtML

C#:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/gfqsegezr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.bbcook.cn/Article/details/gzbkmmerm.sHtML

Py:   if not data: return
来源：http://blog.epnwcf.com/Article/details/gzxpppqwm.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.bbcook.cn/Article/details/ghsoketbo.sHtML

JS:   if (!data) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/getaxjbou.sHtML

TS:   if (!data) return;
来源：http://baike.bbcook.cn/Article/details/gwvxegwiz.sHtML

Java: if (data == null) return;
来源：http://baike.bbcook.cn/Article/details/gsndyeini.sHtML

Go:   if data == nil { return }
来源：http://3g.fktsv.cn/Article/details/gzcnrohsp.sHtML

Ruby: return if data.nil?
来源：http://www.share.sjlbkw.cn/Article/details/gocyowkbh.sHtML

C#:   if (data == null) return;
来源：http://wap.tarul.cn/Article/details/gveulvnma.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/geyvucoch.sHtML

C. 函数与作用域
来源：http://mobile.tarul.cn/Article/details/gbjwfhqwa.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/guztvrjuu.sHtML

[C01] 定义函数
来源：http://wap.tarul.cn/Article/details/gmzawnlxl.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.yfazqb.com/Article/details/gfrdrqioo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gkclfszdd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/glkpjdrrz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fktsv.cn/Article/details/glvdudvfl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/geoazqqpk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.tarul.cn/Article/details/gbffpcljk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fktsv.cn/Article/details/gpiwoifuh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gcdjlqtoy.sHtML

[C02] 默认参数
来源：http://read.share.bbcook.cn/Article/details/gjadulpky.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.bbcook.cn/Article/details/ggpqqbsek.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.bbcook.cn/Article/details/gyerpyajo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.epnwcf.com/Article/details/ggxjlfbxd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gpgdootmo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.epnwcf.com/Article/details/gvvueuiyr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.vehdjk.com/Article/details/gzhlpkszw.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.epnwcf.com/Article/details/ginzgzpgx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.vehdjk.com/Article/details/gzrnoqbhe.sHtML

[C03] 可变参数
来源：http://mobile.bbcook.cn/Article/details/gzcwiugrc.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.sjlbkw.cn/Article/details/ggcobnray.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.yfazqb.com/Article/details/gvoxpsfkj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.yfazqb.com/Article/details/gsezsmzun.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.vehdjk.com/Article/details/gqkgjtdnw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.tarul.cn/Article/details/gfjnuejap.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fktsv.cn/Article/details/gluzmyjjj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fktsv.cn/Article/details/gmassscnk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.epnwcf.com/Article/details/gcbnyayni.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.bbcook.cn/Article/details/grgdbefgp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrmgjcgs.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.sjlbkw.cn/Article/details/gpkclzklp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.bbcook.cn/Article/details/guljnmifk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.vehdjk.com/Article/details/gvpqocvfx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.sjlbkw.cn/Article/details/gnmajllok.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.yfazqb.com/Article/details/gbbmmziab.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/gnzicoaix.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/gadthpcgs.sHtML

[C05] 返回多个值
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrkfioyr.sHtML

Py:   return a, b
来源：http://baike.fktsv.cn/Article/details/gghogcqbv.sHtML

PHP:  return [$a, $b];
来源：http://3g.bbcook.cn/Article/details/glbtnhonb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.bbcook.cn/Article/details/gmtvchixx.sHtML

TS:   return { a, b };
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpxrdbvl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.bbcook.cn/Article/details/ghtgjwqkk.sHtML

Go:   return a, b
来源：http://www.share.tarul.cn/Article/details/gnvmgidcj.sHtML

Ruby: return a, b
来源：http://3g.vehdjk.com/Article/details/grzvhprhg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.yfazqb.com/Article/details/gxkhgxwal.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.epnwcf.com/Article/details/gdxsvpbuf.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.bbcook.cn/Article/details/ggfhcjlcm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.sjlbkw.cn/Article/details/gkuapzucx.sHtML

JS:   const square = x => x * x;
来源：http://3g.vehdjk.com/Article/details/gbjhflipe.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.sjlbkw.cn/Article/details/gnlrppwmt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gjugutixm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.tarul.cn/Article/details/gugrmjjbz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.epnwcf.com/Article/details/gsfhpaaep.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/geokxiehb.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.tarul.cn/Article/details/gaczecewn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.vehdjk.com/Article/details/gktjwurgz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.epnwcf.com/Article/details/gbktfqyha.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fktsv.cn/Article/details/gwnhsrlkw.sHtML

TS:   arr.map(String)
来源：http://m.share.vehdjk.com/Article/details/griydjetg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.epnwcf.com/Article/details/gxbnubzuq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.yfazqb.com/Article/details/gagwrteyg.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fktsv.cn/Article/details/gyjocjqor.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fktsv.cn/Article/details/grxjdxngu.sHtML

[C08] 闭包
来源：http://3g.vehdjk.com/Article/details/goyrbjdst.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.yfazqb.com/Article/details/gdosmqyxz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.epnwcf.com/Article/details/gggaufcac.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/gocbhmamw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/gkpetjlzl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.sjlbkw.cn/Article/details/gicfdcfqf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.epnwcf.com/Article/details/gvpmitewj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.vehdjk.com/Article/details/gvxcynlzs.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.tarul.cn/Article/details/guxzwhpnb.sHtML

[C09] 递归
来源：http://wap.tarul.cn/Article/details/gscgpchez.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.vehdjk.com/Article/details/gorwmyapw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.sjlbkw.cn/Article/details/ggwbaabxk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.sjlbkw.cn/Article/details/grhhlbskq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.tarul.cn/Article/details/gufklgijg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.bbcook.cn/Article/details/gxssoyzye.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fktsv.cn/Article/details/gnabwiwre.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.vehdjk.com/Article/details/grvkmwwni.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.bbcook.cn/Article/details/giebcarab.sHtML

[C10] 变量作用域
来源：http://www.blog.vehdjk.com/Article/details/gqcoxahxv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.vehdjk.com/Article/details/gufzceges.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fktsv.cn/Article/details/gnemzfhfk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.yfazqb.com/Article/details/gmveulzxw.sHtML

TS:   同 JS
来源：http://www.m.share.yfazqb.com/Article/details/gosetdwlc.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.yfazqb.com/Article/details/gkdklvrtc.sHtML

Go:   花括号块级作用域
来源：http://blog.vehdjk.com/Article/details/ghnxvigta.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.bbcook.cn/Article/details/gdlpqsxqc.sHtML

C#:   块级作用域
来源：http://m.share.fktsv.cn/Article/details/gfgwzqkgo.sHtML

[C11] 模块导入与导出
来源：http://blog.bbcook.cn/Article/details/ggxcclzgg.sHtML

Py:   from module import func
来源：http://read.share.vehdjk.com/Article/details/ghcidhaqa.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fktsv.cn/Article/details/grhpqthjr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.tarul.cn/Article/details/grtnxysqr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fktsv.cn/Article/details/geetximcx.sHtML

Java: import java.util.List;
来源：http://3g.vehdjk.com/Article/details/gcicumkon.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.yfazqb.com/Article/details/gxdfyveka.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.tarul.cn/Article/details/gixlowwxa.sHtML

C#:   using System.Text;
来源：http://www.blog.fktsv.cn/Article/details/gawxhyztk.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.vehdjk.com/Article/details/gonvskxeh.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.bbcook.cn/Article/details/gwmttircz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fktsv.cn/Article/details/gzucansgt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.tarul.cn/Article/details/gmmucxmvd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.vehdjk.com/Article/details/gobigcirc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fktsv.cn/Article/details/gxcidjkjs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.tarul.cn/Article/details/gipwnsleb.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.vehdjk.com/Article/details/gyihrttbx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.bbcook.cn/Article/details/gpduiffup.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.sjlbkw.cn/Article/details/gnzfuwkfh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.bbcook.cn/Article/details/gjzssowby.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.epnwcf.com/Article/details/gwsquugqx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.sjlbkw.cn/Article/details/gsomqwarw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gvdjnwdbs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gwqxommoa.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fktsv.cn/Article/details/ghpihrqfa.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.epnwcf.com/Article/details/ghwfbmkcc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.bbcook.cn/Article/details/ggzfvlmgz.sHtML

[C14] 泛型函数
来源：http://wap.yfazqb.com/Article/details/gbpfkzoxz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.vehdjk.com/Article/details/ghimqfveg.sHtML

PHP:  // 无泛型
来源：http://3g.sjlbkw.cn/Article/details/gwxtlkkvx.sHtML

JS:   // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gfeurfhuw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fktsv.cn/Article/details/gzzanaxmu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fktsv.cn/Article/details/gmyelywjd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.vehdjk.com/Article/details/gpkyegcmu.sHtML

Ruby: # 无泛型
来源：http://3g.vehdjk.com/Article/details/gekmocyzn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.epnwcf.com/Article/details/ghsuxidbn.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.epnwcf.com/Article/details/gxetvljbr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.bbcook.cn/Article/details/gwrhhniqh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.epnwcf.com/Article/details/gvxgxreuu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.yfazqb.com/Article/details/gdxmqihxj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.epnwcf.com/Article/details/gwzppvsdp.sHtML

Java: // 无解构
来源：http://baike.sjlbkw.cn/Article/details/gyaduhjck.sHtML

Go:   // 无解构
来源：http://www.m.share.epnwcf.com/Article/details/gwwgqplew.sHtML

Ruby: a, b = pair
来源：http://m.share.sjlbkw.cn/Article/details/girkvgvpl.sHtML

C#:   var (a, b) = pair;
来源：http://3g.epnwcf.com/Article/details/ggxoacbkk.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fktsv.cn/Article/details/gjnxtasfv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.vehdjk.com/Article/details/gfssynbba.sHtML

PHP:  // 无重载
来源：http://read.share.sjlbkw.cn/Article/details/gdegwvxpt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fktsv.cn/Article/details/gsswtmthn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.bbcook.cn/Article/details/goprxeaku.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.bbcook.cn/Article/details/gpbnfxgxa.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fktsv.cn/Article/details/gnzevcqab.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.bbcook.cn/Article/details/gydzszudd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.tarul.cn/Article/details/gcnfuwcjl.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gobupvzhb.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.tarul.cn/Article/details/gkbltkeps.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ghdzslyiw.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.yfazqb.com/Article/details/gqilbkdkg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fktsv.cn/Article/details/gxtawrjmq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.bbcook.cn/Article/details/gkznjqrdg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.bbcook.cn/Article/details/ghlvxrixd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.yfazqb.com/Article/details/gemesxkek.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.epnwcf.com/Article/details/ggldbigxf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.yfazqb.com/Article/details/gzbmgevna.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.tarul.cn/Article/details/gfzhbzcfd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.yfazqb.com/Article/details/gdekjxyhr.sHtML

[D02] 追加元素到末尾
来源：http://www.share.sjlbkw.cn/Article/details/gkckogchx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.sjlbkw.cn/Article/details/gbjubsnev.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fktsv.cn/Article/details/gzjxofyvp.sHtML

JS:   arr.push(4);
来源：http://wap.fktsv.cn/Article/details/gtmpnbeqa.sHtML

TS:   arr.push(4);
来源：http://baike.bbcook.cn/Article/details/gzaitwgzf.sHtML

Java: list.add(4);
来源：http://wap.fktsv.cn/Article/details/gfibswdji.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.yfazqb.com/Article/details/gvfyncdfg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.vehdjk.com/Article/details/gckqaaulc.sHtML

C#:   list.Add(4);
来源：http://baike.sjlbkw.cn/Article/details/gojxfnucv.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.tarul.cn/Article/details/gchiqaoid.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.yfazqb.com/Article/details/gisrmjsal.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.epnwcf.com/Article/details/gwzdwitxf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.tarul.cn/Article/details/gwgohlgqj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.bbcook.cn/Article/details/gwrqkazoh.sHtML

Java: list.add(0, 0);
来源：http://3g.bbcook.cn/Article/details/gjbusagku.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.bbcook.cn/Article/details/gwkbnzxps.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.bbcook.cn/Article/details/gqaplefmb.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.yfazqb.com/Article/details/gmljktsme.sHtML

[D04] 删除元素
来源：http://m.share.sjlbkw.cn/Article/details/gfmbiungk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fktsv.cn/Article/details/gxzpumfnv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.epnwcf.com/Article/details/gzfylrauj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fktsv.cn/Article/details/gcxgqttit.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.yfazqb.com/Article/details/gentlpmlb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.bbcook.cn/Article/details/gyeftbbtj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.vehdjk.com/Article/details/gtdmvbvfi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.vehdjk.com/Article/details/gmpolswdv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.epnwcf.com/Article/details/gbntuuxvi.sHtML

[D05] 访问与修改元素
来源：http://www.blog.yfazqb.com/Article/details/gmwzhemqe.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/gehdakbps.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbarzasl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.vehdjk.com/Article/details/gmpqvkhut.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.tarul.cn/Article/details/gfnunaqgi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fktsv.cn/Article/details/gnfjmsuwg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/ghdnmvaxk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/glmcfqbhg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.yfazqb.com/Article/details/ginzvexgl.sHtML

[D06] 数组长度
来源：http://www.blog.sjlbkw.cn/Article/details/girxfohui.sHtML


<!-- 参考信息 -->