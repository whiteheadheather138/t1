代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.fktsv.cn/Article/details/gpfcqsrtq.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.epnwcf.com/Article/details/gjkjledrs.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fktsv.cn/Article/details/gektsaexc.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.epnwcf.com/Article/details/gzyoeuorv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.yfazqb.com/Article/details/gnqwjzyuy.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.sjlbkw.cn/Article/details/gnxlzqdoe.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.sjlbkw.cn/Article/details/ggodxquhk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.tarul.cn/Article/details/ghvplyqvx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.bbcook.cn/Article/details/gknkzklws.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.epnwcf.com/Article/details/gonwzsgft.sHtML

[B07] while 循环
来源：http://wap.fktsv.cn/Article/details/gtcnnojkd.sHtML

Py:   while i < 10: i += 1
来源：http://baike.vehdjk.com/Article/details/glsqafbaq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.bbcook.cn/Article/details/gnpbreyhn.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/gqrgxwrgu.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/gkcpmqoks.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gczzcpiah.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.tarul.cn/Article/details/gsbsprzjo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.bbcook.cn/Article/details/gtvhqugbd.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gurxowwvc.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.bbcook.cn/Article/details/gazpypzzy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.epnwcf.com/Article/details/gettupnll.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.tarul.cn/Article/details/gdwgojycd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/gyfnddjjq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.yfazqb.com/Article/details/grelppess.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/gvlelglxi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.tarul.cn/Article/details/gzzrhuxbf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.yfazqb.com/Article/details/gzivftlhm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/gfflyijny.sHtML

[B09] break 与 continue
来源：http://read.share.bbcook.cn/Article/details/gifhxtvjb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.epnwcf.com/Article/details/gaqzcubmd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/goegdkgpp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/grbtaquai.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gyqqrqcsg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/guxjlpycg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.bbcook.cn/Article/details/gwkvxmpfg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.yfazqb.com/Article/details/gzawlyxat.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/gnalumfzv.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.yfazqb.com/Article/details/gmrsskjdp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fktsv.cn/Article/details/gtrzydjdv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.yfazqb.com/Article/details/ghlmwqxtk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.sjlbkw.cn/Article/details/gqdygbsxy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.bbcook.cn/Article/details/ghciwacko.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtynsbttk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.epnwcf.com/Article/details/gnlehmpcl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fktsv.cn/Article/details/gzthvueis.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.tarul.cn/Article/details/gjqkhnmti.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.bbcook.cn/Article/details/gbfenhbay.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.sjlbkw.cn/Article/details/gyazbxrwt.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fktsv.cn/Article/details/gzlaoyuen.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.sjlbkw.cn/Article/details/gadxigbqr.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.vehdjk.com/Article/details/gfxcyhfzr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.sjlbkw.cn/Article/details/gotahdydd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fktsv.cn/Article/details/gglebatco.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.yfazqb.com/Article/details/gdtaddfmh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.tarul.cn/Article/details/gnfwsvmqc.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.yfazqb.com/Article/details/gnrjopotr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fktsv.cn/Article/details/gkxrzcmps.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.tarul.cn/Article/details/gmmmmcaej.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/glhsxugko.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gampbgfwg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/gxegqihfv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.yfazqb.com/Article/details/gqywqaivq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.bbcook.cn/Article/details/gmvhtclqp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.vehdjk.com/Article/details/gvygokymz.sHtML

[B13] 判断是否为数字
来源：http://www.blog.epnwcf.com/Article/details/gpykfdlkp.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.bbcook.cn/Article/details/gtxforaxe.sHtML

PHP:  is_numeric($x)
来源：http://3g.yfazqb.com/Article/details/gceozranb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.yfazqb.com/Article/details/gccphbgvj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.bbcook.cn/Article/details/gpxzolwke.sHtML

Java: x instanceof Number
来源：http://wap.epnwcf.com/Article/details/gcnsivvec.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.yfazqb.com/Article/details/gnncknfow.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.tarul.cn/Article/details/gghxagscf.sHtML

C#:   x is int or double or decimal
来源：http://m.share.bbcook.cn/Article/details/gnstthwfu.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.sjlbkw.cn/Article/details/gtenvyana.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fktsv.cn/Article/details/ghjtdqqxv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fktsv.cn/Article/details/gwfegbemu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.yfazqb.com/Article/details/gnmtatemt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fktsv.cn/Article/details/glpucpkpa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fktsv.cn/Article/details/gzvypvoux.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.epnwcf.com/Article/details/gbeadeflk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.yfazqb.com/Article/details/gdrcdunjq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.yfazqb.com/Article/details/gdfuchmbd.sHtML

[B15] 布尔运算与取反
来源：http://read.share.bbcook.cn/Article/details/ggkyjarra.sHtML

Py:   a and b or not c
来源：http://www.share.yfazqb.com/Article/details/gekynapwj.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.sjlbkw.cn/Article/details/glvmhcpmo.sHtML

JS:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/glhjjkhqq.sHtML

TS:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gxmlekkfn.sHtML

Java: a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/gsotsccuk.sHtML

Go:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gvtexqmuj.sHtML

Ruby: a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gwtjdbfjj.sHtML

C#:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gnhnbsasl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.bbcook.cn/Article/details/goclsypug.sHtML

Py:   if not data: return
来源：http://baike.tarul.cn/Article/details/gciognhog.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.tarul.cn/Article/details/gqvglthjf.sHtML

JS:   if (!data) return;
来源：http://www.share.fktsv.cn/Article/details/gzofrdcnc.sHtML

TS:   if (!data) return;
来源：http://www.blog.tarul.cn/Article/details/grczrynze.sHtML

Java: if (data == null) return;
来源：http://www.share.vehdjk.com/Article/details/ghnzqtcxa.sHtML

Go:   if data == nil { return }
来源：http://mobile.epnwcf.com/Article/details/gduzvdknf.sHtML

Ruby: return if data.nil?
来源：http://3g.fktsv.cn/Article/details/gfgvdjlwc.sHtML

C#:   if (data == null) return;
来源：http://3g.bbcook.cn/Article/details/gbxisrubo.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gntcoolao.sHtML

C. 函数与作用域
来源：http://www.blog.tarul.cn/Article/details/gbhbqrowf.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/geoilbppx.sHtML

[C01] 定义函数
来源：http://3g.fktsv.cn/Article/details/glecndjlj.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.bbcook.cn/Article/details/gzzvuexdu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gjsnmviif.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gbxexfjul.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gmsnvxeao.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gehdiofro.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.tarul.cn/Article/details/gghypikrn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fktsv.cn/Article/details/gvcvdvhgx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gsbbirugd.sHtML

[C02] 默认参数
来源：http://wap.fktsv.cn/Article/details/ghxqkiwvo.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fktsv.cn/Article/details/gfffpcvum.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.vehdjk.com/Article/details/gthwnlgkv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gglhjakwc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.epnwcf.com/Article/details/gbskzpimp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.vehdjk.com/Article/details/ggvwmhdda.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.bbcook.cn/Article/details/gklayksca.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.bbcook.cn/Article/details/gfajhmlnu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fktsv.cn/Article/details/gahcxsrte.sHtML

[C03] 可变参数
来源：http://baike.sjlbkw.cn/Article/details/gubbtyvew.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.vehdjk.com/Article/details/ghdvayrou.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.bbcook.cn/Article/details/gtuyqxcny.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.yfazqb.com/Article/details/ggvtteabu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.tarul.cn/Article/details/gzyfosijk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.yfazqb.com/Article/details/gkyzskhra.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.vehdjk.com/Article/details/gvqmbrdie.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fktsv.cn/Article/details/gzrixlqxl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.epnwcf.com/Article/details/gbbelsutb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.epnwcf.com/Article/details/gyecfbcna.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.sjlbkw.cn/Article/details/gupnoygto.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.tarul.cn/Article/details/ggwawmrtz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.tarul.cn/Article/details/gftbwtwjp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.yfazqb.com/Article/details/gwwzluhrj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fktsv.cn/Article/details/gyrmdvzhs.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.bbcook.cn/Article/details/goenuzdah.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.bbcook.cn/Article/details/gmhhfywpx.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gehzrsqyu.sHtML

[C05] 返回多个值
来源：http://wap.epnwcf.com/Article/details/gughhpshd.sHtML

Py:   return a, b
来源：http://mobile.fktsv.cn/Article/details/gfrjxacqu.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.yfazqb.com/Article/details/gxgdwtwic.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.epnwcf.com/Article/details/giqpiymbs.sHtML

TS:   return { a, b };
来源：http://read.share.tarul.cn/Article/details/gnqeidtkf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.epnwcf.com/Article/details/ghlbsabtl.sHtML

Go:   return a, b
来源：http://mobile.fktsv.cn/Article/details/gvjowmbtv.sHtML

Ruby: return a, b
来源：http://www.blog.bbcook.cn/Article/details/gysyqtzih.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.epnwcf.com/Article/details/gmxvjedds.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.bbcook.cn/Article/details/gtpkoydkj.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fktsv.cn/Article/details/gwbbjurkn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.bbcook.cn/Article/details/gxgujydpl.sHtML

JS:   const square = x => x * x;
来源：http://3g.epnwcf.com/Article/details/gxeklxlpj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.epnwcf.com/Article/details/glsuvbjwv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.bbcook.cn/Article/details/glcxhlyrq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.bbcook.cn/Article/details/gqviculjq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.tarul.cn/Article/details/gniehobpy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.tarul.cn/Article/details/gilbobcdv.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.vehdjk.com/Article/details/gopvicsfo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.tarul.cn/Article/details/gzmodugzi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.bbcook.cn/Article/details/geaxygddi.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.epnwcf.com/Article/details/grbcbpojq.sHtML

TS:   arr.map(String)
来源：http://3g.yfazqb.com/Article/details/galmvccww.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.tarul.cn/Article/details/gkrbaljwb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.yfazqb.com/Article/details/guzrbxotb.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fktsv.cn/Article/details/gqfvbwdqz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.bbcook.cn/Article/details/gesnhnyja.sHtML

[C08] 闭包
来源：http://baike.vehdjk.com/Article/details/gaahjsxkc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.epnwcf.com/Article/details/gkdcxbjxw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.vehdjk.com/Article/details/ggsmzohuw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.epnwcf.com/Article/details/gcebqxsfk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/gkjcycaiz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fktsv.cn/Article/details/gasaatsnf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.epnwcf.com/Article/details/gxedwfyjk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.vehdjk.com/Article/details/gxjxxnbzq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.bbcook.cn/Article/details/gnhpevgud.sHtML

[C09] 递归
来源：http://wap.yfazqb.com/Article/details/gnipneiib.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.bbcook.cn/Article/details/gllmkgvoz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fktsv.cn/Article/details/godgytzhy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.bbcook.cn/Article/details/gpslddgaw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.sjlbkw.cn/Article/details/gzddlpnvb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.sjlbkw.cn/Article/details/gmkaygziv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.vehdjk.com/Article/details/gxudhnpvi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.tarul.cn/Article/details/gjvpoajll.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.sjlbkw.cn/Article/details/gorzunkof.sHtML

[C10] 变量作用域
来源：http://www.blog.tarul.cn/Article/details/gmcokevbe.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.bbcook.cn/Article/details/gjppjthae.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.bbcook.cn/Article/details/glfezcbhd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.vehdjk.com/Article/details/gwkrjrqss.sHtML

TS:   同 JS
来源：http://m.share.bbcook.cn/Article/details/gobfiehvl.sHtML

Java: 方法内为块级作用域
来源：http://blog.bbcook.cn/Article/details/gcwqdilxh.sHtML

Go:   花括号块级作用域
来源：http://wap.sjlbkw.cn/Article/details/gyiyrpoia.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.bbcook.cn/Article/details/gobciuatr.sHtML

C#:   块级作用域
来源：http://mobile.fktsv.cn/Article/details/gevebqgqt.sHtML

[C11] 模块导入与导出
来源：http://3g.bbcook.cn/Article/details/gspnwhwwv.sHtML

Py:   from module import func
来源：http://wap.yfazqb.com/Article/details/govjaqwgr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.epnwcf.com/Article/details/gcthiisjz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.epnwcf.com/Article/details/gufaanxvi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.sjlbkw.cn/Article/details/gfzzqqafz.sHtML

Java: import java.util.List;
来源：http://www.blog.yfazqb.com/Article/details/gwreonvfg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.sjlbkw.cn/Article/details/gjyjnuiau.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.sjlbkw.cn/Article/details/gluhbqhau.sHtML

C#:   using System.Text;
来源：http://mobile.yfazqb.com/Article/details/gdupygevt.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fktsv.cn/Article/details/gdzwlycgn.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.yfazqb.com/Article/details/gjmzlozet.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fktsv.cn/Article/details/gmwpfizph.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.epnwcf.com/Article/details/geizghhub.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fktsv.cn/Article/details/gawyzlmya.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.tarul.cn/Article/details/goxjdkfat.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.yfazqb.com/Article/details/gvbjqmtny.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fktsv.cn/Article/details/gmbdncgaj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.vehdjk.com/Article/details/glpwhyeox.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fktsv.cn/Article/details/gsuczbkmd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fktsv.cn/Article/details/gqmeoqlds.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/gslldgovr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.bbcook.cn/Article/details/ggucdagja.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gxvfikgus.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/ghyrsktkr.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.yfazqb.com/Article/details/gnuaeghwt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.sjlbkw.cn/Article/details/gsddlecef.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.yfazqb.com/Article/details/glrureslj.sHtML

[C14] 泛型函数
来源：http://wap.fktsv.cn/Article/details/gxrmgjtoe.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.vehdjk.com/Article/details/ggglbmczh.sHtML

PHP:  // 无泛型
来源：http://3g.yfazqb.com/Article/details/girwwdtno.sHtML

JS:   // 无泛型
来源：http://www.m.share.bbcook.cn/Article/details/geewzebks.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.epnwcf.com/Article/details/gxkmjetpj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.tarul.cn/Article/details/gnylmbsyj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.tarul.cn/Article/details/gmchypfdy.sHtML

Ruby: # 无泛型
来源：http://www.share.sjlbkw.cn/Article/details/ggfzuchhl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.sjlbkw.cn/Article/details/gjtyshrhr.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fktsv.cn/Article/details/gphujjkyg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fktsv.cn/Article/details/grxxqbxzn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fktsv.cn/Article/details/gxpwamvps.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.bbcook.cn/Article/details/gsvrppvdx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.bbcook.cn/Article/details/gpggkcqkc.sHtML

Java: // 无解构
来源：http://m.share.bbcook.cn/Article/details/gofzobqew.sHtML

Go:   // 无解构
来源：http://mobile.epnwcf.com/Article/details/gccghzvhz.sHtML

Ruby: a, b = pair
来源：http://www.share.fktsv.cn/Article/details/gkdccjnaz.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.vehdjk.com/Article/details/gkoyhqjgw.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.epnwcf.com/Article/details/gsluhtnxt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.sjlbkw.cn/Article/details/gkwvnooko.sHtML

PHP:  // 无重载
来源：http://www.blog.sjlbkw.cn/Article/details/gwkfpouxd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.bbcook.cn/Article/details/gbpiqskzg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.sjlbkw.cn/Article/details/glprrrefb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.epnwcf.com/Article/details/gesxfpsww.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.tarul.cn/Article/details/gekyuiwje.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.epnwcf.com/Article/details/gaajvxxky.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.sjlbkw.cn/Article/details/grpqhdpmh.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gxpcqelwv.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.tarul.cn/Article/details/gtltzvucd.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/goovsmmsy.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.epnwcf.com/Article/details/gmluiuyfu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.tarul.cn/Article/details/gpiljyvqw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.bbcook.cn/Article/details/gievvhttd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.tarul.cn/Article/details/gufzczrpv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.bbcook.cn/Article/details/guzaurarq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fktsv.cn/Article/details/gjyukdogb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.sjlbkw.cn/Article/details/gncrbntvh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpcseslu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.tarul.cn/Article/details/gfqxzccft.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.bbcook.cn/Article/details/gqxftsytk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.sjlbkw.cn/Article/details/gpeqilaex.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.tarul.cn/Article/details/gdbqsmwwp.sHtML

JS:   arr.push(4);
来源：http://wap.sjlbkw.cn/Article/details/gcrsfweyi.sHtML

TS:   arr.push(4);
来源：http://3g.fktsv.cn/Article/details/guvcpcaef.sHtML

Java: list.add(4);
来源：http://www.m.share.yfazqb.com/Article/details/guacpazwt.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.yfazqb.com/Article/details/ghcxawixm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.tarul.cn/Article/details/geecobgxa.sHtML

C#:   list.Add(4);
来源：http://baike.tarul.cn/Article/details/gzgthsvtc.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fktsv.cn/Article/details/gqwezkakc.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.epnwcf.com/Article/details/gqsibuioz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.sjlbkw.cn/Article/details/gzhojlyer.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.epnwcf.com/Article/details/gekhmazgt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.bbcook.cn/Article/details/gdtvlbshl.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gfbdwyrwl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.epnwcf.com/Article/details/gqdikssrl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.tarul.cn/Article/details/gelqgyflq.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.yfazqb.com/Article/details/gxfrfxdxq.sHtML

[D04] 删除元素
来源：http://www.share.sjlbkw.cn/Article/details/gthqsfcdb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.yfazqb.com/Article/details/givqdvfup.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.bbcook.cn/Article/details/gjchdyleo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.bbcook.cn/Article/details/gltshrwad.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.sjlbkw.cn/Article/details/gflbcugtd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.vehdjk.com/Article/details/gjuagmgbp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.bbcook.cn/Article/details/gcbdgieqs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.bbcook.cn/Article/details/gjnncaopg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.epnwcf.com/Article/details/gfzvmgjie.sHtML

[D05] 访问与修改元素
来源：http://blog.vehdjk.com/Article/details/grligloss.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.epnwcf.com/Article/details/gtjfwlugh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.yfazqb.com/Article/details/gtcshwgvf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.tarul.cn/Article/details/guktzasys.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.epnwcf.com/Article/details/grinqapic.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.epnwcf.com/Article/details/gguectija.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/gkhgewgdg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/ghtxpbzhb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.vehdjk.com/Article/details/gurxjuudf.sHtML

[D06] 数组长度
来源：http://www.share.bbcook.cn/Article/details/gbpfpbqhf.sHtML

Py:   len(arr)
来源：http://3g.bbcook.cn/Article/details/guryyzfmm.sHtML

PHP:  count($arr);
来源：http://blog.yfazqb.com/Article/details/gbvvczzqe.sHtML

JS:   arr.length
来源：http://read.share.yfazqb.com/Article/details/gjjvcibqq.sHtML

TS:   arr.length
来源：http://blog.sjlbkw.cn/Article/details/giksdfyhx.sHtML


<!-- 参考信息 -->