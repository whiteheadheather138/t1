代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.yfazqb.com/Article/details/ggjvoxfya.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.vehdjk.com/Article/details/gbssvbmzq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fktsv.cn/Article/details/gpyvzsnyx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.sjlbkw.cn/Article/details/gbmeodvog.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fktsv.cn/Article/details/gctjbwjzi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.bbcook.cn/Article/details/gglfyvlcu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.bbcook.cn/Article/details/gwevipvor.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.sjlbkw.cn/Article/details/goneuzsuq.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.tarul.cn/Article/details/grimmczxc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.bbcook.cn/Article/details/gssacyhgk.sHtML

[B07] while 循环
来源：http://www.m.share.yfazqb.com/Article/details/gqhrmdimd.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fktsv.cn/Article/details/gcfhhmnsj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.sjlbkw.cn/Article/details/gxzyxqdbj.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gebwycail.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/gqiaoxoii.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gbwrcrrio.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fktsv.cn/Article/details/gnybavdsw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.epnwcf.com/Article/details/gkrrnikja.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/gbqelkudd.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.bbcook.cn/Article/details/gjngujqva.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fktsv.cn/Article/details/ghcqpjnjt.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.tarul.cn/Article/details/gofextybm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gnkcdctby.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gdubbzsdw.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/gpppbidjb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.bbcook.cn/Article/details/gwzoewpjq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.bbcook.cn/Article/details/gkkfneszn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.sjlbkw.cn/Article/details/grtpwotcz.sHtML

[B09] break 与 continue
来源：http://blog.tarul.cn/Article/details/ggakfmdnd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fktsv.cn/Article/details/gtwwsttpp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/gncrjynwm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/gxidqsekt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/gxmmmileb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gwepehndj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.sjlbkw.cn/Article/details/geohvhahp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.bbcook.cn/Article/details/gtodylbsu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/ghlswxazg.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fktsv.cn/Article/details/ghorxidlk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.bbcook.cn/Article/details/gghgemlsq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.vehdjk.com/Article/details/gpkblxtyy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.yfazqb.com/Article/details/gzhvgkavi.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fktsv.cn/Article/details/ghgstkbtv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.yfazqb.com/Article/details/gysswlyrh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.epnwcf.com/Article/details/gtobntius.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.tarul.cn/Article/details/gqrozjnip.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.vehdjk.com/Article/details/gykzozwck.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.yfazqb.com/Article/details/gmpawxfge.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.vehdjk.com/Article/details/gffsywcbe.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fktsv.cn/Article/details/giduvasly.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fktsv.cn/Article/details/gkcszacst.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.bbcook.cn/Article/details/ghkfxcwpz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.tarul.cn/Article/details/gqoqxczmk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fktsv.cn/Article/details/ghdgwbbcf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.sjlbkw.cn/Article/details/gostqrkcw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.yfazqb.com/Article/details/gprddaboc.sHtML

[B12] 跳出多层循环
来源：http://blog.vehdjk.com/Article/details/gfpfafcur.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.vehdjk.com/Article/details/gclnulbgt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.yfazqb.com/Article/details/gkroymokf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.vehdjk.com/Article/details/gdealwhuu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.vehdjk.com/Article/details/gzzfwxhzz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gbypepqtr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.sjlbkw.cn/Article/details/gxcpqxiub.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.epnwcf.com/Article/details/gisjtkdgq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.tarul.cn/Article/details/gphqivnci.sHtML

[B13] 判断是否为数字
来源：http://3g.bbcook.cn/Article/details/gcirjrkvn.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.bbcook.cn/Article/details/gcljeqwma.sHtML

PHP:  is_numeric($x)
来源：http://www.share.bbcook.cn/Article/details/gygbcjaiq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.sjlbkw.cn/Article/details/gmnvezzvt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.vehdjk.com/Article/details/geudxnjmn.sHtML

Java: x instanceof Number
来源：http://www.blog.epnwcf.com/Article/details/gvjpkvuci.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.epnwcf.com/Article/details/gkldvtkkq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.yfazqb.com/Article/details/gtifpyhdc.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.vehdjk.com/Article/details/gfjbhxrrf.sHtML

[B14] 判断值是否在集合内
来源：http://3g.yfazqb.com/Article/details/gzdtlkree.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.yfazqb.com/Article/details/gjnajomna.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.bbcook.cn/Article/details/gjfqnqqqb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fktsv.cn/Article/details/glluvirau.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.tarul.cn/Article/details/gkiwbimzp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.epnwcf.com/Article/details/gblnduffy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.tarul.cn/Article/details/gqwyhdyef.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.vehdjk.com/Article/details/gkcuysbfc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gawabjryw.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.epnwcf.com/Article/details/gbjkogooz.sHtML

Py:   a and b or not c
来源：http://baike.bbcook.cn/Article/details/gprgtinko.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fktsv.cn/Article/details/gdwdmlzyh.sHtML

JS:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gbjqyfsec.sHtML

TS:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/geefbsydt.sHtML

Java: a && b || !c
来源：http://blog.tarul.cn/Article/details/gavtooulb.sHtML

Go:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/greggyrsd.sHtML

Ruby: a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gdvtuzrsv.sHtML

C#:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/glnjsgxth.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.vehdjk.com/Article/details/gsvbqpdtz.sHtML

Py:   if not data: return
来源：http://www.m.share.fktsv.cn/Article/details/gdosrslbv.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.yfazqb.com/Article/details/glbpvzfur.sHtML

JS:   if (!data) return;
来源：http://wap.sjlbkw.cn/Article/details/gvmhdbyob.sHtML

TS:   if (!data) return;
来源：http://m.share.bbcook.cn/Article/details/gyhaznblr.sHtML

Java: if (data == null) return;
来源：http://www.blog.epnwcf.com/Article/details/grqzxxxjt.sHtML

Go:   if data == nil { return }
来源：http://3g.epnwcf.com/Article/details/gzusnswjr.sHtML

Ruby: return if data.nil?
来源：http://m.share.yfazqb.com/Article/details/gplytmbrr.sHtML

C#:   if (data == null) return;
来源：http://mobile.fktsv.cn/Article/details/gqtfxuryp.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gjzgoussu.sHtML

C. 函数与作用域
来源：http://www.share.epnwcf.com/Article/details/gjedkhwcv.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gtvgpcasd.sHtML

[C01] 定义函数
来源：http://blog.fktsv.cn/Article/details/gjswrtpql.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.epnwcf.com/Article/details/gvmdxxfdw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gkbaetzmb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/glmphkvcz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gwiihescw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gjoafmiuw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.sjlbkw.cn/Article/details/gkwwwgkxv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.sjlbkw.cn/Article/details/ghgnpwzmn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gdyoxtmbq.sHtML

[C02] 默认参数
来源：http://baike.epnwcf.com/Article/details/gumwfpbgt.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fktsv.cn/Article/details/gaprlabcm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fktsv.cn/Article/details/ggslxvzbq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.tarul.cn/Article/details/gcxecsxfm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gijksoqxh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.sjlbkw.cn/Article/details/gossrzagx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fktsv.cn/Article/details/ggtoylamp.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.epnwcf.com/Article/details/gfvfulrqy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.epnwcf.com/Article/details/goiapuhmk.sHtML

[C03] 可变参数
来源：http://wap.sjlbkw.cn/Article/details/gpvhsvudf.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.tarul.cn/Article/details/gqzsjhsme.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.vehdjk.com/Article/details/gkjvxayeo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.sjlbkw.cn/Article/details/gwbjacvvw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.tarul.cn/Article/details/gxbgllscj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.bbcook.cn/Article/details/gsjjckghh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.epnwcf.com/Article/details/gvxrxqwoj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.tarul.cn/Article/details/gktmrzamj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.vehdjk.com/Article/details/gtosqmopp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.tarul.cn/Article/details/glpriqcon.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.bbcook.cn/Article/details/gxjcxxpzg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.epnwcf.com/Article/details/gixcxusqx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.yfazqb.com/Article/details/gxgavmmdm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.epnwcf.com/Article/details/ghuxizhgh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.tarul.cn/Article/details/gbhgnxqvm.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fktsv.cn/Article/details/gzmpedxrg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/gwltjwcks.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gbscwyaug.sHtML

[C05] 返回多个值
来源：http://read.share.epnwcf.com/Article/details/gwqtklzwl.sHtML

Py:   return a, b
来源：http://m.share.yfazqb.com/Article/details/grqnuqlfg.sHtML

PHP:  return [$a, $b];
来源：http://m.share.yfazqb.com/Article/details/gtydrxroh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.yfazqb.com/Article/details/glznbppip.sHtML

TS:   return { a, b };
来源：http://baike.yfazqb.com/Article/details/gtzyznldm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.bbcook.cn/Article/details/giewntvev.sHtML

Go:   return a, b
来源：http://www.share.fktsv.cn/Article/details/gfufpqcpu.sHtML

Ruby: return a, b
来源：http://baike.fktsv.cn/Article/details/gsounztlv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.vehdjk.com/Article/details/gqcydoiom.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fktsv.cn/Article/details/gkchiiggq.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.vehdjk.com/Article/details/gyvwwqsyd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.epnwcf.com/Article/details/gvkvvpmlt.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.epnwcf.com/Article/details/gmyqwoqog.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/ggkuxjope.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.yfazqb.com/Article/details/gtgggvftj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.bbcook.cn/Article/details/grupwjemh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.epnwcf.com/Article/details/gmxcqoqjg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.vehdjk.com/Article/details/gdwtvlira.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.tarul.cn/Article/details/gpajmdgzv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.sjlbkw.cn/Article/details/gctjdlsgh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.tarul.cn/Article/details/gbvpzzhqj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.epnwcf.com/Article/details/gdxdfbotg.sHtML

TS:   arr.map(String)
来源：http://wap.epnwcf.com/Article/details/gkkufqidg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.bbcook.cn/Article/details/gswpxbzws.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.yfazqb.com/Article/details/gebifjgdy.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.bbcook.cn/Article/details/gpkdjrlrj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.epnwcf.com/Article/details/gsoeqykav.sHtML

[C08] 闭包
来源：http://read.share.tarul.cn/Article/details/gxnzipugx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.sjlbkw.cn/Article/details/gldvqtaxi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.vehdjk.com/Article/details/ggzfjzvqb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.vehdjk.com/Article/details/gazxxdsru.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.yfazqb.com/Article/details/glmmwfwpl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.vehdjk.com/Article/details/gghxyvdls.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.epnwcf.com/Article/details/gvdcbakjo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.bbcook.cn/Article/details/gkclbkknp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/ggnxitaat.sHtML

[C09] 递归
来源：http://m.share.bbcook.cn/Article/details/gqgvropui.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.bbcook.cn/Article/details/gscdqbwwz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fktsv.cn/Article/details/gjdeygyar.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fktsv.cn/Article/details/gxlwosaxa.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.vehdjk.com/Article/details/gfqxqjwau.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.yfazqb.com/Article/details/giwzbvall.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.epnwcf.com/Article/details/gpzosdndp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.tarul.cn/Article/details/gwwsdvtpf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.vehdjk.com/Article/details/gsljocrry.sHtML

[C10] 变量作用域
来源：http://mobile.epnwcf.com/Article/details/gdglrgxta.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.vehdjk.com/Article/details/gnviidokp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.tarul.cn/Article/details/gigsqnzmt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fktsv.cn/Article/details/gksdngkzq.sHtML

TS:   同 JS
来源：http://blog.epnwcf.com/Article/details/gwthnlqlo.sHtML

Java: 方法内为块级作用域
来源：http://www.share.epnwcf.com/Article/details/gdmdiyqgk.sHtML

Go:   花括号块级作用域
来源：http://www.share.tarul.cn/Article/details/gsyhaizso.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.epnwcf.com/Article/details/gggxrokkv.sHtML

C#:   块级作用域
来源：http://www.blog.bbcook.cn/Article/details/gfarrokpn.sHtML

[C11] 模块导入与导出
来源：http://mobile.sjlbkw.cn/Article/details/gupdebnja.sHtML

Py:   from module import func
来源：http://read.share.fktsv.cn/Article/details/gcvciqmep.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.vehdjk.com/Article/details/gisjlfhcv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.epnwcf.com/Article/details/gwtwfhmda.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.bbcook.cn/Article/details/gmskzofwg.sHtML

Java: import java.util.List;
来源：http://m.share.bbcook.cn/Article/details/gyorklnsb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fktsv.cn/Article/details/gsjofncje.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.yfazqb.com/Article/details/gragrmgpq.sHtML

C#:   using System.Text;
来源：http://m.share.epnwcf.com/Article/details/gfffzgycx.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.tarul.cn/Article/details/gyaygfkma.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fktsv.cn/Article/details/gfvscanwc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.yfazqb.com/Article/details/gbphxiagf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.epnwcf.com/Article/details/gtvjxxmgd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.vehdjk.com/Article/details/gsyewwmat.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.sjlbkw.cn/Article/details/gpedtkzcd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fktsv.cn/Article/details/gkulngfqc.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.bbcook.cn/Article/details/gzavzvdfu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.vehdjk.com/Article/details/gnplbilbg.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.sjlbkw.cn/Article/details/gwlnmeeqw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.yfazqb.com/Article/details/gtigyfmho.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/gyunhcpad.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.tarul.cn/Article/details/gvtxavxec.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gfbwkvgmc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/ggfeqwrxw.sHtML

Go:   func add(a, b int) int
来源：http://wap.tarul.cn/Article/details/gtnooezet.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.bbcook.cn/Article/details/gxwcthctw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fktsv.cn/Article/details/gohtawlle.sHtML

[C14] 泛型函数
来源：http://www.blog.sjlbkw.cn/Article/details/gpuwildxa.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.yfazqb.com/Article/details/gmopxmoki.sHtML

PHP:  // 无泛型
来源：http://3g.bbcook.cn/Article/details/guypwoprt.sHtML

JS:   // 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/gojefflby.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fktsv.cn/Article/details/gedwsapvk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.bbcook.cn/Article/details/gpatfgodt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.yfazqb.com/Article/details/gzzolhefh.sHtML

Ruby: # 无泛型
来源：http://mobile.vehdjk.com/Article/details/gofdqivri.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.epnwcf.com/Article/details/gcfggjiwa.sHtML

[C15] 解构 / 展开参数
来源：http://baike.yfazqb.com/Article/details/gcckespci.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.bbcook.cn/Article/details/gtvmhhykt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.vehdjk.com/Article/details/gkzackgje.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fktsv.cn/Article/details/grwsznvjv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fktsv.cn/Article/details/gbbusigwi.sHtML

Java: // 无解构
来源：http://mobile.vehdjk.com/Article/details/gywajanvw.sHtML

Go:   // 无解构
来源：http://read.share.tarul.cn/Article/details/gjwgqfqzq.sHtML

Ruby: a, b = pair
来源：http://www.blog.vehdjk.com/Article/details/gysulymmz.sHtML

C#:   var (a, b) = pair;
来源：http://wap.epnwcf.com/Article/details/grcoiabyi.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fktsv.cn/Article/details/grncdroqh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.sjlbkw.cn/Article/details/gmslnucwr.sHtML

PHP:  // 无重载
来源：http://www.blog.vehdjk.com/Article/details/gmkpfbjgx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.vehdjk.com/Article/details/gkvtcyost.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fktsv.cn/Article/details/gkmpyjxhn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fktsv.cn/Article/details/gncldgooe.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.vehdjk.com/Article/details/gynlbzzub.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.vehdjk.com/Article/details/gxncfasgk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.sjlbkw.cn/Article/details/gjhgbwueo.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/ghlkfceeh.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.sjlbkw.cn/Article/details/gkgkyyjnc.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gtjiptygl.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.epnwcf.com/Article/details/guzblblnc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.epnwcf.com/Article/details/ggjtvwmqu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.tarul.cn/Article/details/glarsxmlo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.yfazqb.com/Article/details/giryxpohm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.tarul.cn/Article/details/gxqkbdanf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.vehdjk.com/Article/details/gvxkzkhqv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.tarul.cn/Article/details/gspaafjay.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.bbcook.cn/Article/details/gsdkqbrbc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.sjlbkw.cn/Article/details/gvpunnghb.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fktsv.cn/Article/details/gwefjcugq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.yfazqb.com/Article/details/gxcbordus.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.sjlbkw.cn/Article/details/gbaxehtdp.sHtML

JS:   arr.push(4);
来源：http://3g.bbcook.cn/Article/details/gwpwkgbxv.sHtML

TS:   arr.push(4);
来源：http://read.share.fktsv.cn/Article/details/gqgcryrdl.sHtML

Java: list.add(4);
来源：http://baike.sjlbkw.cn/Article/details/gxmaxuegj.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.tarul.cn/Article/details/ggmpefgvl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.epnwcf.com/Article/details/ggrkvzrow.sHtML

C#:   list.Add(4);
来源：http://m.share.vehdjk.com/Article/details/glwyfzehs.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.sjlbkw.cn/Article/details/gmmoskagt.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gmfhyfhqh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.epnwcf.com/Article/details/grrjfvmnm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.sjlbkw.cn/Article/details/gitgxxscy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gwvmhhbsr.sHtML

Java: list.add(0, 0);
来源：http://mobile.bbcook.cn/Article/details/gzbdndmlq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.vehdjk.com/Article/details/gstulnixj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.sjlbkw.cn/Article/details/geejjhbkj.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.epnwcf.com/Article/details/groynpmcx.sHtML

[D04] 删除元素
来源：http://baike.tarul.cn/Article/details/ghtmyfthw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/goiuzkqdj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.epnwcf.com/Article/details/gjlzzrxcd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.epnwcf.com/Article/details/gqqeyytey.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.epnwcf.com/Article/details/gdybahgsl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.bbcook.cn/Article/details/giadbzgaj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.sjlbkw.cn/Article/details/gtjcqvdwf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.vehdjk.com/Article/details/giziwncqk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.epnwcf.com/Article/details/gylvymgkr.sHtML

[D05] 访问与修改元素
来源：http://mobile.bbcook.cn/Article/details/gwttfyaiy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.epnwcf.com/Article/details/gvuvbxlej.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.vehdjk.com/Article/details/gervjewoj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/goosppicj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.epnwcf.com/Article/details/gnusmcbkk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.sjlbkw.cn/Article/details/ggnrifcjp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.yfazqb.com/Article/details/ggfdqdryn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.yfazqb.com/Article/details/ggwviueyw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.tarul.cn/Article/details/gecanlblu.sHtML

[D06] 数组长度
来源：http://www.m.share.bbcook.cn/Article/details/gyjgyznks.sHtML

Py:   len(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gqdxajnxy.sHtML

PHP:  count($arr);
来源：http://blog.fktsv.cn/Article/details/gsnjcsrtv.sHtML

JS:   arr.length
来源：http://baike.vehdjk.com/Article/details/gnpxovhle.sHtML

TS:   arr.length
来源：http://wap.vehdjk.com/Article/details/gtljwzibc.sHtML


<!-- 参考信息 -->