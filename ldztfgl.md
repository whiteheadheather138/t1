代发 wailian999

[B05] 遍历数组 / 列表
来源：http://read.share.epnwcf.com/Article/details/gqbwnegae.sHtML

Py:   for item in arr: print(item)
来源：http://3g.yfazqb.com/Article/details/gxoiusztn.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.epnwcf.com/Article/details/grjbujpnv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.vehdjk.com/Article/details/gueslgcwt.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.bbcook.cn/Article/details/grojuzfpb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.yfazqb.com/Article/details/geperfklw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fktsv.cn/Article/details/gaplwdpct.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.bbcook.cn/Article/details/glygmcumw.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.sjlbkw.cn/Article/details/gqdhqeeuc.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.tarul.cn/Article/details/gmoeqwfcf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.yfazqb.com/Article/details/geimknuvq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.vehdjk.com/Article/details/gqlvxcdvm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.yfazqb.com/Article/details/gyklcbojg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.bbcook.cn/Article/details/gkzghpafm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.bbcook.cn/Article/details/gjbkuhhei.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.bbcook.cn/Article/details/gzaevttwd.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.bbcook.cn/Article/details/ghvhcfiuh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.epnwcf.com/Article/details/gcunxvxdx.sHtML

[B07] while 循环
来源：http://mobile.vehdjk.com/Article/details/gbvefvuhu.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fktsv.cn/Article/details/gpcqpsxxo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gvlqjtzoi.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/gjbavrgch.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/giskmcojj.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/gbjsbwopd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.epnwcf.com/Article/details/gwheiquwf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.vehdjk.com/Article/details/gfffmgitr.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/gtmnotdaf.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.sjlbkw.cn/Article/details/godhtjayj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.yfazqb.com/Article/details/ggfsdkxmf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gftorispf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/gpxrpzxje.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gptaqnqyi.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gklmzgyuq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fktsv.cn/Article/details/gixdvncnp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.bbcook.cn/Article/details/gbiixdnlt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gizjagykx.sHtML

[B09] break 与 continue
来源：http://3g.vehdjk.com/Article/details/gprlfxlrw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.yfazqb.com/Article/details/ggmzoxwkm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gqyryfunt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/gvdyhnixz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmhxckcop.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gwusyxnmp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.yfazqb.com/Article/details/guhwkroqg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.tarul.cn/Article/details/gbjjwepaw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gdzumumzq.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fktsv.cn/Article/details/gefswurih.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fktsv.cn/Article/details/gwkzxkrmx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.sjlbkw.cn/Article/details/gmiqiqfqz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fktsv.cn/Article/details/gmhzteyeq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fktsv.cn/Article/details/gvechpbez.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.tarul.cn/Article/details/gbjndkxlt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.tarul.cn/Article/details/gogsackdb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.sjlbkw.cn/Article/details/gtriyszbs.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.yfazqb.com/Article/details/gjunhdqui.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.tarul.cn/Article/details/gbklldumg.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.tarul.cn/Article/details/gqogaobzw.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fktsv.cn/Article/details/gcllphmqc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.yfazqb.com/Article/details/glugrtugf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.bbcook.cn/Article/details/gubxngqel.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.yfazqb.com/Article/details/gltoammnq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fktsv.cn/Article/details/gbkyxdztb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.tarul.cn/Article/details/gdintgsgv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.tarul.cn/Article/details/gwqgvlaqb.sHtML

[B12] 跳出多层循环
来源：http://read.share.tarul.cn/Article/details/gddvnskfc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.epnwcf.com/Article/details/gfxatsstj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.bbcook.cn/Article/details/gumxgjkaq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.vehdjk.com/Article/details/gvbdyrfny.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.tarul.cn/Article/details/gxpmtxxub.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.epnwcf.com/Article/details/gqospzoqw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.epnwcf.com/Article/details/ggqxfonng.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.bbcook.cn/Article/details/gfagpdjfm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.sjlbkw.cn/Article/details/gdnkgxuiz.sHtML

[B13] 判断是否为数字
来源：http://3g.tarul.cn/Article/details/gpeqyitsn.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.yfazqb.com/Article/details/glyekiucq.sHtML

PHP:  is_numeric($x)
来源：http://read.share.epnwcf.com/Article/details/gjakbsduu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.yfazqb.com/Article/details/gpxibrfhb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.bbcook.cn/Article/details/gpjhiuinz.sHtML

Java: x instanceof Number
来源：http://wap.bbcook.cn/Article/details/gsylvujus.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.tarul.cn/Article/details/gyphatqub.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.sjlbkw.cn/Article/details/gedddwkbe.sHtML

C#:   x is int or double or decimal
来源：http://wap.tarul.cn/Article/details/gjfdjpioo.sHtML

[B14] 判断值是否在集合内
来源：http://baike.epnwcf.com/Article/details/gadfsdkrg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.tarul.cn/Article/details/ggoavitmr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.sjlbkw.cn/Article/details/gztvbresc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.bbcook.cn/Article/details/gwqomsdvj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gbmjrnzzb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.yfazqb.com/Article/details/gdwxoyjjt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fktsv.cn/Article/details/grrwjxziu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.yfazqb.com/Article/details/garbgezjf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.yfazqb.com/Article/details/gjgrvfthk.sHtML

[B15] 布尔运算与取反
来源：http://m.share.epnwcf.com/Article/details/grzsngzqg.sHtML

Py:   a and b or not c
来源：http://www.share.vehdjk.com/Article/details/gwisdrubf.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.yfazqb.com/Article/details/gqbithcrp.sHtML

JS:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gtsbxvnhz.sHtML

TS:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gnqpakxbh.sHtML

Java: a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gsckdmvjf.sHtML

Go:   a && b || !c
来源：http://baike.epnwcf.com/Article/details/gceywdwxq.sHtML

Ruby: a && b || !c
来源：http://wap.fktsv.cn/Article/details/gsydqlhxc.sHtML

C#:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/gekqbssnv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fktsv.cn/Article/details/gobtwzzde.sHtML

Py:   if not data: return
来源：http://3g.yfazqb.com/Article/details/gbctifftr.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.sjlbkw.cn/Article/details/gtislxqks.sHtML

JS:   if (!data) return;
来源：http://read.share.sjlbkw.cn/Article/details/gfivqyddv.sHtML

TS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/gvfivharb.sHtML

Java: if (data == null) return;
来源：http://blog.sjlbkw.cn/Article/details/gxzumbqfo.sHtML

Go:   if data == nil { return }
来源：http://www.blog.bbcook.cn/Article/details/grnrzeswi.sHtML

Ruby: return if data.nil?
来源：http://baike.tarul.cn/Article/details/gqpgboacr.sHtML

C#:   if (data == null) return;
来源：http://mobile.tarul.cn/Article/details/gayisndzb.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gxhkiobgw.sHtML

C. 函数与作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gwcxmvmkb.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gpbuljxtr.sHtML

[C01] 定义函数
来源：http://www.share.sjlbkw.cn/Article/details/gwavxqxed.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.yfazqb.com/Article/details/gmaunadpo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.epnwcf.com/Article/details/gsisbndvk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gbkhmnzst.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmudfzvgx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gdyogelse.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.epnwcf.com/Article/details/gylyxcmzq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fktsv.cn/Article/details/gnjhnfmke.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gknbzbgog.sHtML

[C02] 默认参数
来源：http://m.share.bbcook.cn/Article/details/gvnnacyzt.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.bbcook.cn/Article/details/gxqrifxvl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.epnwcf.com/Article/details/gjaetcxnk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.vehdjk.com/Article/details/gtzwmuhey.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.yfazqb.com/Article/details/gslplcryw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.tarul.cn/Article/details/gikpljsjs.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.vehdjk.com/Article/details/gudfxvdam.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.vehdjk.com/Article/details/gnsscfgnm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fktsv.cn/Article/details/gvzpbylqe.sHtML

[C03] 可变参数
来源：http://www.blog.tarul.cn/Article/details/gvflebjia.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.vehdjk.com/Article/details/gigpffjjk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.tarul.cn/Article/details/gfqxutdrl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.tarul.cn/Article/details/ggfgmpybf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.tarul.cn/Article/details/geddzdjzs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.sjlbkw.cn/Article/details/griwdwoan.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.epnwcf.com/Article/details/guucnwajb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.vehdjk.com/Article/details/gisrynofb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.bbcook.cn/Article/details/gldkoocth.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.epnwcf.com/Article/details/gyamszcmr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.tarul.cn/Article/details/gthbdpgwq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fktsv.cn/Article/details/gdpossdxs.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.yfazqb.com/Article/details/gxfuqamci.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.yfazqb.com/Article/details/gvanaemif.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.sjlbkw.cn/Article/details/gienutgkk.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.epnwcf.com/Article/details/gtdevevxe.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fktsv.cn/Article/details/gazrsblmn.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/grccyudnx.sHtML

[C05] 返回多个值
来源：http://www.m.share.tarul.cn/Article/details/grmpoucpu.sHtML

Py:   return a, b
来源：http://3g.epnwcf.com/Article/details/geztoqukk.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fktsv.cn/Article/details/gcgktyzlj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.yfazqb.com/Article/details/gftoermqg.sHtML

TS:   return { a, b };
来源：http://blog.epnwcf.com/Article/details/gzkepslge.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.bbcook.cn/Article/details/ghopadpvx.sHtML

Go:   return a, b
来源：http://read.share.bbcook.cn/Article/details/gbuwifjvr.sHtML

Ruby: return a, b
来源：http://www.blog.bbcook.cn/Article/details/gpyecfjwh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.yfazqb.com/Article/details/gvunrmfft.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.sjlbkw.cn/Article/details/gxncgslgz.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.sjlbkw.cn/Article/details/gqzxgzovp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fktsv.cn/Article/details/gaqrkcecw.sHtML

JS:   const square = x => x * x;
来源：http://read.share.vehdjk.com/Article/details/gbyeqekkh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gofeqkfnm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.bbcook.cn/Article/details/gxogplupz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.tarul.cn/Article/details/guqkmhgpl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.epnwcf.com/Article/details/ginzjnqlh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gbsqmcmxi.sHtML

[C07] 把函数作为参数传入
来源：http://wap.bbcook.cn/Article/details/gajakwuus.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.tarul.cn/Article/details/gubgqcdbc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fktsv.cn/Article/details/gjjshboaz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.epnwcf.com/Article/details/gatpnvxgm.sHtML

TS:   arr.map(String)
来源：http://baike.tarul.cn/Article/details/gewpbibht.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gtialjvsr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.vehdjk.com/Article/details/gbtehltlk.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.sjlbkw.cn/Article/details/gopzljsmu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.tarul.cn/Article/details/gbjgwxxta.sHtML

[C08] 闭包
来源：http://baike.vehdjk.com/Article/details/gtwudtaxf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.sjlbkw.cn/Article/details/giperwfzu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.yfazqb.com/Article/details/gharqdykz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.epnwcf.com/Article/details/ggyppteux.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.bbcook.cn/Article/details/gxtkhxdbh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.sjlbkw.cn/Article/details/gkybombqq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.sjlbkw.cn/Article/details/gajfrxilg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.epnwcf.com/Article/details/gitzmvhlc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gmowjhwgu.sHtML

[C09] 递归
来源：http://www.blog.tarul.cn/Article/details/ghlsolcbh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.tarul.cn/Article/details/gocvdvikx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fktsv.cn/Article/details/gulnisycp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fktsv.cn/Article/details/gfhztotcf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.epnwcf.com/Article/details/gndathpvm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.bbcook.cn/Article/details/gibthebon.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.tarul.cn/Article/details/gfmaezbxt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.vehdjk.com/Article/details/gvnrmdgve.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.yfazqb.com/Article/details/gpygzenlz.sHtML

[C10] 变量作用域
来源：http://www.m.share.epnwcf.com/Article/details/gjbuzsrmd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.tarul.cn/Article/details/gpgxwduat.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.sjlbkw.cn/Article/details/ggrwnagro.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.epnwcf.com/Article/details/gtbcicoxg.sHtML

TS:   同 JS
来源：http://read.share.yfazqb.com/Article/details/gfukenwdy.sHtML

Java: 方法内为块级作用域
来源：http://baike.epnwcf.com/Article/details/gxmpilnca.sHtML

Go:   花括号块级作用域
来源：http://3g.tarul.cn/Article/details/giyugpsbo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.tarul.cn/Article/details/geeqfkzef.sHtML

C#:   块级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtyxvcwz.sHtML

[C11] 模块导入与导出
来源：http://www.share.yfazqb.com/Article/details/giruknnah.sHtML

Py:   from module import func
来源：http://baike.epnwcf.com/Article/details/gohwbrhrg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fktsv.cn/Article/details/gnmoyyguk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.epnwcf.com/Article/details/gsecfofod.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fktsv.cn/Article/details/gzbohzrcy.sHtML

Java: import java.util.List;
来源：http://blog.tarul.cn/Article/details/glhffhvkb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.sjlbkw.cn/Article/details/gabfvpcvh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.epnwcf.com/Article/details/grcptjarh.sHtML

C#:   using System.Text;
来源：http://www.share.yfazqb.com/Article/details/gjawkebxy.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.epnwcf.com/Article/details/gixhkuqzd.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.vehdjk.com/Article/details/gfqpvvbeb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.yfazqb.com/Article/details/gcemrbrsv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.vehdjk.com/Article/details/gyfesfvgd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.yfazqb.com/Article/details/glaclyqla.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.vehdjk.com/Article/details/gbpgfwgfi.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.tarul.cn/Article/details/gtldlugfc.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.yfazqb.com/Article/details/gyhvqtdiq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.sjlbkw.cn/Article/details/gygrbjnkr.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fktsv.cn/Article/details/gdunvmcil.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.vehdjk.com/Article/details/gbgczinno.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gghdyjudg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fktsv.cn/Article/details/gxwgbitzg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gbvkoayrk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gyxveksxl.sHtML

Go:   func add(a, b int) int
来源：http://wap.tarul.cn/Article/details/ghglotwvw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.epnwcf.com/Article/details/gcqvonfvp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.tarul.cn/Article/details/gcivujmaw.sHtML

[C14] 泛型函数
来源：http://blog.fktsv.cn/Article/details/gypjtiqcl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.tarul.cn/Article/details/gqzylsgxb.sHtML

PHP:  // 无泛型
来源：http://baike.vehdjk.com/Article/details/glszuupdg.sHtML

JS:   // 无泛型
来源：http://www.share.sjlbkw.cn/Article/details/gpwidaoay.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.epnwcf.com/Article/details/gklrgqjmc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.yfazqb.com/Article/details/ghhdqqdii.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fktsv.cn/Article/details/gpqphdbbi.sHtML

Ruby: # 无泛型
来源：http://blog.sjlbkw.cn/Article/details/gglgzyawj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.bbcook.cn/Article/details/gcpvyjebi.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.vehdjk.com/Article/details/gvgirmxjg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.vehdjk.com/Article/details/gbpjrldqt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.sjlbkw.cn/Article/details/gysjfqczj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.tarul.cn/Article/details/gyhbvcxkl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.yfazqb.com/Article/details/goblinyjc.sHtML

Java: // 无解构
来源：http://www.m.share.tarul.cn/Article/details/gjrbtvsqf.sHtML

Go:   // 无解构
来源：http://3g.epnwcf.com/Article/details/gdjiauure.sHtML

Ruby: a, b = pair
来源：http://mobile.fktsv.cn/Article/details/ggldejwby.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.vehdjk.com/Article/details/gwrsxvaet.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.bbcook.cn/Article/details/gbgclmlvy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.tarul.cn/Article/details/guazefbrw.sHtML

PHP:  // 无重载
来源：http://m.share.vehdjk.com/Article/details/gdsxtghyh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.epnwcf.com/Article/details/guiqdkbur.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.bbcook.cn/Article/details/gbgnpdujg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fktsv.cn/Article/details/gzmuypphh.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.bbcook.cn/Article/details/gdichgora.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.vehdjk.com/Article/details/gzftolunl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.yfazqb.com/Article/details/gjnlbiwip.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gxyhihnib.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.epnwcf.com/Article/details/geinzctxr.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gkpkfqqfa.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fktsv.cn/Article/details/guomewagp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.tarul.cn/Article/details/gwgjrqwos.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.tarul.cn/Article/details/gstpysdzq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fktsv.cn/Article/details/gagcpzxpl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.epnwcf.com/Article/details/gvmxfbkdm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.yfazqb.com/Article/details/gpuxuunxi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fktsv.cn/Article/details/gtgyubcki.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.sjlbkw.cn/Article/details/gzrwyvoyz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fktsv.cn/Article/details/gpdzvnfbp.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fktsv.cn/Article/details/gskjtuess.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.bbcook.cn/Article/details/guspdzkes.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fktsv.cn/Article/details/girfllgzz.sHtML

JS:   arr.push(4);
来源：http://blog.fktsv.cn/Article/details/gynxkcecy.sHtML

TS:   arr.push(4);
来源：http://wap.fktsv.cn/Article/details/gebwzcyey.sHtML

Java: list.add(4);
来源：http://blog.tarul.cn/Article/details/guzwmliuj.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfcgiprn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.bbcook.cn/Article/details/ghubjssbh.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fktsv.cn/Article/details/gxwedhvbz.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.epnwcf.com/Article/details/gwypmkpty.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.vehdjk.com/Article/details/gsoyfotie.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.sjlbkw.cn/Article/details/gtfeygahj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.bbcook.cn/Article/details/gnpwrvdax.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.bbcook.cn/Article/details/gocualbai.sHtML

Java: list.add(0, 0);
来源：http://www.blog.bbcook.cn/Article/details/gsubobsqi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fktsv.cn/Article/details/gmsqpneor.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fktsv.cn/Article/details/gyafdnnlv.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gjeoitpus.sHtML

[D04] 删除元素
来源：http://www.m.share.bbcook.cn/Article/details/golluachg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.bbcook.cn/Article/details/gfjvhompz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.sjlbkw.cn/Article/details/gxvtbrhkp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.vehdjk.com/Article/details/ghvafxsys.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fktsv.cn/Article/details/gfbqjgoon.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.sjlbkw.cn/Article/details/gzmbnbrvv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.tarul.cn/Article/details/gcegtvrrt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.epnwcf.com/Article/details/gudwbwpas.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.yfazqb.com/Article/details/gowyunbts.sHtML

[D05] 访问与修改元素
来源：http://m.share.epnwcf.com/Article/details/gxbkyvokt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.epnwcf.com/Article/details/gpdkjwwdy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.epnwcf.com/Article/details/getehfpxn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.yfazqb.com/Article/details/gnezntaev.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.bbcook.cn/Article/details/ghioeipal.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.epnwcf.com/Article/details/gmgxhqdpf.sHtML


<!-- 参考信息 -->