代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.tarul.cn/Article/details/gmcwjhrrw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.yfazqb.com/Article/details/gephnward.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.vehdjk.com/Article/details/gdwfgrxnx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/gazycbygd.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gxerbqozk.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fktsv.cn/Article/details/gplapqhch.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.yfazqb.com/Article/details/gjesntbhu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.bbcook.cn/Article/details/gudufergz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.tarul.cn/Article/details/ggnxzmbtp.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.vehdjk.com/Article/details/glpwoppsh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fktsv.cn/Article/details/gqqqlpsse.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.epnwcf.com/Article/details/gjhpuxort.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.vehdjk.com/Article/details/gypebterd.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.epnwcf.com/Article/details/gsfxtoxmg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fktsv.cn/Article/details/gwylmjqsq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.tarul.cn/Article/details/gpjtsainy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.tarul.cn/Article/details/grtrapfyv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fktsv.cn/Article/details/gesicpgen.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.epnwcf.com/Article/details/gbbqwbkwd.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.tarul.cn/Article/details/gutkkgstz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.vehdjk.com/Article/details/gxpngnnev.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.epnwcf.com/Article/details/gjeqlbmxx.sHtML

[B07] while 循环
来源：http://www.share.epnwcf.com/Article/details/gmtrgzdly.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.vehdjk.com/Article/details/gymwgrhnd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.epnwcf.com/Article/details/gidxoqnfb.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.vehdjk.com/Article/details/gikrlwyep.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/ghuxumivv.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/ghrurwtwj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.vehdjk.com/Article/details/gtalramqr.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.bbcook.cn/Article/details/gqqmahjfe.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/gaxgadnlx.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fktsv.cn/Article/details/gkvbxowtc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fktsv.cn/Article/details/gfvqikktg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/glgsqwyov.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.epnwcf.com/Article/details/gaxiifpsj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gspsgelzh.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/ghawygnso.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.fktsv.cn/Article/details/gyksrldne.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.epnwcf.com/Article/details/gapvzuzcl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.yfazqb.com/Article/details/gftzuvewj.sHtML

[B09] break 与 continue
来源：http://www.share.sjlbkw.cn/Article/details/gzhovuabk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.fktsv.cn/Article/details/gjrqsxzqz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gxtemkrhu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gmzpxldjb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/gavwkmepv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gzddkkvsi.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.tarul.cn/Article/details/glqryxuqn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.yfazqb.com/Article/details/gbjrgsfpe.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/godyefowj.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.epnwcf.com/Article/details/gxjcuveao.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fktsv.cn/Article/details/gwrqjndzc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.epnwcf.com/Article/details/gykjjchhm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.bbcook.cn/Article/details/glaiddnka.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fktsv.cn/Article/details/gobgntykr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.tarul.cn/Article/details/gppidicyp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fktsv.cn/Article/details/gxgzgsejf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.sjlbkw.cn/Article/details/ghfgeigjk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.sjlbkw.cn/Article/details/glufcccbh.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.yfazqb.com/Article/details/gldjmbiqw.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.epnwcf.com/Article/details/gzaykopbp.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gcahkxcrf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.bbcook.cn/Article/details/ggtggsqrx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.epnwcf.com/Article/details/grcbfkevg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.yfazqb.com/Article/details/gghynftpe.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.bbcook.cn/Article/details/gcsnddioj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.sjlbkw.cn/Article/details/gekesulil.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.bbcook.cn/Article/details/gakrxmqjw.sHtML

[B12] 跳出多层循环
来源：http://mobile.bbcook.cn/Article/details/gqjiphtob.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fktsv.cn/Article/details/gqtyyljgt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.vehdjk.com/Article/details/geydqirwx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.bbcook.cn/Article/details/gdgwvjppt.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/gounonnrr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/gksqcxwsv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.yfazqb.com/Article/details/grkurbtae.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.yfazqb.com/Article/details/guvlahcor.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.bbcook.cn/Article/details/gsiqbmfzv.sHtML

[B13] 判断是否为数字
来源：http://m.share.epnwcf.com/Article/details/gvmrbqplw.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.vehdjk.com/Article/details/gnwypharq.sHtML

PHP:  is_numeric($x)
来源：http://mobile.epnwcf.com/Article/details/gbtzdgkay.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.epnwcf.com/Article/details/gchekuufu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.vehdjk.com/Article/details/gmgitcadk.sHtML

Java: x instanceof Number
来源：http://www.blog.fktsv.cn/Article/details/gvxshrcyq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.bbcook.cn/Article/details/gzzcoiaww.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.tarul.cn/Article/details/gqstzwxgl.sHtML

C#:   x is int or double or decimal
来源：http://blog.fktsv.cn/Article/details/gijazwynr.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fktsv.cn/Article/details/gbbuszrey.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.vehdjk.com/Article/details/gizryodyy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.tarul.cn/Article/details/gyesihjgu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.bbcook.cn/Article/details/gpxxeqghv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/gwdbtplgl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gzbafwgls.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fktsv.cn/Article/details/gllvhznrp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fktsv.cn/Article/details/gmolpoxdy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.tarul.cn/Article/details/gteftrrmt.sHtML

[B15] 布尔运算与取反
来源：http://blog.fktsv.cn/Article/details/gewlevaip.sHtML

Py:   a and b or not c
来源：http://read.share.tarul.cn/Article/details/gqaossvyj.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.tarul.cn/Article/details/gbzonxuen.sHtML

JS:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnggphaf.sHtML

TS:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/gmuillamz.sHtML

Java: a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gcyqnezpa.sHtML

Go:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gkatxliqx.sHtML

Ruby: a && b || !c
来源：http://m.share.tarul.cn/Article/details/gzdhzghxy.sHtML

C#:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/gislicojc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.sjlbkw.cn/Article/details/gmzgenday.sHtML

Py:   if not data: return
来源：http://m.share.fktsv.cn/Article/details/gsqkenspj.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.yfazqb.com/Article/details/gkhciibwu.sHtML

JS:   if (!data) return;
来源：http://baike.sjlbkw.cn/Article/details/gnihvefhf.sHtML

TS:   if (!data) return;
来源：http://wap.tarul.cn/Article/details/gbrnchuvz.sHtML

Java: if (data == null) return;
来源：http://3g.vehdjk.com/Article/details/goiywngab.sHtML

Go:   if data == nil { return }
来源：http://read.share.fktsv.cn/Article/details/ggfmhvjdm.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.tarul.cn/Article/details/gflqxislc.sHtML

C#:   if (data == null) return;
来源：http://www.share.yfazqb.com/Article/details/gxliozhqk.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gkyaffghn.sHtML

C. 函数与作用域
来源：http://m.share.epnwcf.com/Article/details/grwczpkac.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gfiezjdbf.sHtML

[C01] 定义函数
来源：http://mobile.fktsv.cn/Article/details/gaznqxpeb.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.yfazqb.com/Article/details/gzufrruvb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gpybrlmpk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/ghwfbmdmm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gkrefqkhq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gzkumuhpw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.tarul.cn/Article/details/gbvtajwey.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.yfazqb.com/Article/details/gpjjkkpht.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gxjfixfdi.sHtML

[C02] 默认参数
来源：http://wap.tarul.cn/Article/details/gzzpwrwnf.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.yfazqb.com/Article/details/gqbdbvfcq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fktsv.cn/Article/details/gdxgdnmzu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/gvyqdweqg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.vehdjk.com/Article/details/gtmhxebah.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fktsv.cn/Article/details/gfxnvgdgr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.tarul.cn/Article/details/gguxymmjq.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.vehdjk.com/Article/details/gwlumsejv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.bbcook.cn/Article/details/gmudlvtqa.sHtML

[C03] 可变参数
来源：http://www.blog.sjlbkw.cn/Article/details/gyumvskby.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fktsv.cn/Article/details/gvonwdfbr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.tarul.cn/Article/details/gxukkyzdp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.epnwcf.com/Article/details/gurjlgxff.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.yfazqb.com/Article/details/gejxssatq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.sjlbkw.cn/Article/details/gasnnnizk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.yfazqb.com/Article/details/glplelbjk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.tarul.cn/Article/details/gdonrrjpi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fktsv.cn/Article/details/gcjfgrkkl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.vehdjk.com/Article/details/gchrptwrr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.tarul.cn/Article/details/gfbcikmcw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.yfazqb.com/Article/details/goocqmbmg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.sjlbkw.cn/Article/details/ggtlspbee.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.tarul.cn/Article/details/gpkuhhbfy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.sjlbkw.cn/Article/details/gncgbqojm.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.epnwcf.com/Article/details/gcoeiwjcj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/giiiyhaak.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/gsdkchgbu.sHtML

[C05] 返回多个值
来源：http://m.share.fktsv.cn/Article/details/gtmbfilns.sHtML

Py:   return a, b
来源：http://blog.fktsv.cn/Article/details/gvxftaeen.sHtML

PHP:  return [$a, $b];
来源：http://mobile.epnwcf.com/Article/details/gwjhnqsjk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.epnwcf.com/Article/details/gnyevwkqc.sHtML

TS:   return { a, b };
来源：http://3g.epnwcf.com/Article/details/gnucpccly.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.sjlbkw.cn/Article/details/gdwiqlqpg.sHtML

Go:   return a, b
来源：http://www.m.share.tarul.cn/Article/details/geafuqxjj.sHtML

Ruby: return a, b
来源：http://m.share.fktsv.cn/Article/details/gliqbzapn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.tarul.cn/Article/details/gjqxeraab.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.sjlbkw.cn/Article/details/glwmldvbh.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.yfazqb.com/Article/details/gptpdfgqw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fktsv.cn/Article/details/gdnxrdqrm.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.vehdjk.com/Article/details/ghnyjgmxt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.vehdjk.com/Article/details/gdbepqeel.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fktsv.cn/Article/details/gwvvhkxvn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.epnwcf.com/Article/details/gqyalnoqc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fktsv.cn/Article/details/ghjngwoeq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fktsv.cn/Article/details/gywalmeoo.sHtML

[C07] 把函数作为参数传入
来源：http://3g.epnwcf.com/Article/details/gcusunmyr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.sjlbkw.cn/Article/details/gpsvgywkq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gulrcakbt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.yfazqb.com/Article/details/gwczmswpx.sHtML

TS:   arr.map(String)
来源：http://wap.sjlbkw.cn/Article/details/ghyduirye.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gwebwmsam.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.bbcook.cn/Article/details/gmlyuuziy.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.epnwcf.com/Article/details/gijymvinv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fktsv.cn/Article/details/grdynibos.sHtML

[C08] 闭包
来源：http://www.blog.fktsv.cn/Article/details/gcsshvwpv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.tarul.cn/Article/details/gbqdolmkf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.bbcook.cn/Article/details/gzfjnqzvl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.tarul.cn/Article/details/gifwwjssd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.sjlbkw.cn/Article/details/ghzzxhtpu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.vehdjk.com/Article/details/ghetdmvji.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fktsv.cn/Article/details/gjenszggt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.sjlbkw.cn/Article/details/gunnqosra.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.yfazqb.com/Article/details/gbqteuuxz.sHtML

[C09] 递归
来源：http://www.share.bbcook.cn/Article/details/gujzhxije.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.vehdjk.com/Article/details/gozlyhswm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fktsv.cn/Article/details/gcgscwmqd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.sjlbkw.cn/Article/details/glufgpybl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.bbcook.cn/Article/details/gpegrfmsy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.tarul.cn/Article/details/gldnkibgp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.epnwcf.com/Article/details/gjrudmybl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gheunckcm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.tarul.cn/Article/details/ggcblmxwc.sHtML

[C10] 变量作用域
来源：http://read.share.bbcook.cn/Article/details/gaiuuveov.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.vehdjk.com/Article/details/gpkspwoyb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.vehdjk.com/Article/details/gfamacilq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.vehdjk.com/Article/details/gosvgwzap.sHtML

TS:   同 JS
来源：http://mobile.tarul.cn/Article/details/geoogllye.sHtML

Java: 方法内为块级作用域
来源：http://read.share.vehdjk.com/Article/details/gqhzpdxdt.sHtML

Go:   花括号块级作用域
来源：http://m.share.tarul.cn/Article/details/gminkhqqv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.sjlbkw.cn/Article/details/gagpolnyz.sHtML

C#:   块级作用域
来源：http://3g.fktsv.cn/Article/details/gicpveuiq.sHtML

[C11] 模块导入与导出
来源：http://mobile.tarul.cn/Article/details/gkphhupqo.sHtML

Py:   from module import func
来源：http://www.share.tarul.cn/Article/details/gglvhusbj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.tarul.cn/Article/details/gnbivvknt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.vehdjk.com/Article/details/gzcmvqrwn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.tarul.cn/Article/details/gjwzbfihg.sHtML

Java: import java.util.List;
来源：http://m.share.tarul.cn/Article/details/gdyzeggad.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.yfazqb.com/Article/details/geowabych.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.vehdjk.com/Article/details/giwkgcnrt.sHtML

C#:   using System.Text;
来源：http://read.share.sjlbkw.cn/Article/details/gkuvfrzxh.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.bbcook.cn/Article/details/gcaldhlwd.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.vehdjk.com/Article/details/gyjqmgdrc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.epnwcf.com/Article/details/gdkvzwcml.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.bbcook.cn/Article/details/gvtpivvaf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.bbcook.cn/Article/details/gyjpseyve.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.bbcook.cn/Article/details/gtyeejjzt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.epnwcf.com/Article/details/gnwikegfa.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fktsv.cn/Article/details/ggofhxvmx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fktsv.cn/Article/details/gmovxsymj.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.sjlbkw.cn/Article/details/gkmycwojj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.bbcook.cn/Article/details/glpmwsnob.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gtbzjyhfw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.yfazqb.com/Article/details/gyciqliob.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/ghjxeiuak.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gbviemedw.sHtML

Go:   func add(a, b int) int
来源：http://wap.yfazqb.com/Article/details/gatxmrvet.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.epnwcf.com/Article/details/gvxwktvpj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fktsv.cn/Article/details/gqukmuqto.sHtML

[C14] 泛型函数
来源：http://baike.yfazqb.com/Article/details/gffssdydb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.sjlbkw.cn/Article/details/gcfapccsy.sHtML

PHP:  // 无泛型
来源：http://3g.vehdjk.com/Article/details/gjymnehjx.sHtML

JS:   // 无泛型
来源：http://read.share.bbcook.cn/Article/details/ggejtzdiw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.vehdjk.com/Article/details/gxftzwcrc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.bbcook.cn/Article/details/gdsxhpdrm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.sjlbkw.cn/Article/details/gnezfwxiu.sHtML

Ruby: # 无泛型
来源：http://blog.yfazqb.com/Article/details/gckhyijrp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fktsv.cn/Article/details/gusvttwnw.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.sjlbkw.cn/Article/details/gemjzbfla.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.yfazqb.com/Article/details/gwitwtcyn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.tarul.cn/Article/details/gtrquhvhx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.epnwcf.com/Article/details/gektnzjix.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.vehdjk.com/Article/details/grmwpurgg.sHtML

Java: // 无解构
来源：http://www.blog.yfazqb.com/Article/details/gsrvlsgkk.sHtML

Go:   // 无解构
来源：http://wap.fktsv.cn/Article/details/gamprkdks.sHtML

Ruby: a, b = pair
来源：http://mobile.sjlbkw.cn/Article/details/gdjbwedad.sHtML

C#:   var (a, b) = pair;
来源：http://blog.sjlbkw.cn/Article/details/gplnyyalx.sHtML

[C16] 函数 / 方法重载
来源：http://baike.tarul.cn/Article/details/gonhybioz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.bbcook.cn/Article/details/ghtxwsvhe.sHtML

PHP:  // 无重载
来源：http://www.share.sjlbkw.cn/Article/details/gsugyzkzt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.yfazqb.com/Article/details/gvivcxlda.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.tarul.cn/Article/details/gnvfjbmmp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.bbcook.cn/Article/details/gbpfpqean.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.yfazqb.com/Article/details/geudwgtuv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.tarul.cn/Article/details/grksbnksh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fktsv.cn/Article/details/gmxhfwxqt.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gntlhjyzi.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.sjlbkw.cn/Article/details/gpcbalcrm.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gnlrpuxjk.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.bbcook.cn/Article/details/gzclnznpn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.epnwcf.com/Article/details/gvwymcouf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.bbcook.cn/Article/details/giwoxdfrz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.vehdjk.com/Article/details/giaqwkver.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.vehdjk.com/Article/details/gavmvskeq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.vehdjk.com/Article/details/gxnnzmfjv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.epnwcf.com/Article/details/grhchbqmr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.vehdjk.com/Article/details/gidhdhfjo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.bbcook.cn/Article/details/geembjtmm.sHtML

[D02] 追加元素到末尾
来源：http://www.share.tarul.cn/Article/details/gvndrlang.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.epnwcf.com/Article/details/gxeywvlji.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.yfazqb.com/Article/details/gzxpxtiuj.sHtML

JS:   arr.push(4);
来源：http://www.m.share.tarul.cn/Article/details/gwspavaij.sHtML

TS:   arr.push(4);
来源：http://wap.bbcook.cn/Article/details/gireiztqg.sHtML

Java: list.add(4);
来源：http://read.share.tarul.cn/Article/details/gdirvwhrl.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.bbcook.cn/Article/details/gxhjsbtyc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.epnwcf.com/Article/details/gjhpxclnn.sHtML

C#:   list.Add(4);
来源：http://mobile.sjlbkw.cn/Article/details/gqxdhxkba.sHtML

[D03] 在指定位置插入元素
来源：http://baike.yfazqb.com/Article/details/gvfknypdp.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.vehdjk.com/Article/details/gdkcvnksl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.tarul.cn/Article/details/gbonxtvoo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.sjlbkw.cn/Article/details/galbeynem.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.bbcook.cn/Article/details/gvzjsjxft.sHtML

Java: list.add(0, 0);
来源：http://baike.yfazqb.com/Article/details/gsgswrqnr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.sjlbkw.cn/Article/details/gjyxnaxmr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.vehdjk.com/Article/details/gmeujwncn.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.bbcook.cn/Article/details/guurkmcxw.sHtML

[D04] 删除元素
来源：http://www.m.share.tarul.cn/Article/details/gsldnckgn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.vehdjk.com/Article/details/gjydtckcm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.epnwcf.com/Article/details/gervjjdoh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.epnwcf.com/Article/details/gxdhqammr.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.epnwcf.com/Article/details/givrqkrjw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.yfazqb.com/Article/details/gpwhbopyw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.tarul.cn/Article/details/ggkbjanck.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.sjlbkw.cn/Article/details/gbxseoksu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.epnwcf.com/Article/details/gjyfspsgk.sHtML

[D05] 访问与修改元素
来源：http://read.share.fktsv.cn/Article/details/gpmuahatj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/gtttvrjxc.sHtML


<!-- 参考信息 -->