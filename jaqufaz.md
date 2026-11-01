代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.bbcook.cn/Article/details/gimooymao.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.vehdjk.com/Article/details/gqqzqmkvl.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxxpixzj.sHtML

[B04] for 计数循环
来源：http://mobile.bbcook.cn/Article/details/gjjpzdmyv.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.fktsv.cn/Article/details/ggbbtmrbt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.sjlbkw.cn/Article/details/gmztcugtf.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.bbcook.cn/Article/details/gmcdyvbor.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.tarul.cn/Article/details/giudrabgx.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.epnwcf.com/Article/details/gopwiaclg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.yfazqb.com/Article/details/glbnszkcy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fktsv.cn/Article/details/gwpfljtfv.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.bbcook.cn/Article/details/gqenpqkjq.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.vehdjk.com/Article/details/gqumkqbkl.sHtML

Py:   for item in arr: print(item)
来源：http://3g.vehdjk.com/Article/details/gwkapibql.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.tarul.cn/Article/details/gxfjtaxnk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.sjlbkw.cn/Article/details/gxlglgesc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.sjlbkw.cn/Article/details/gaevjkajf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.yfazqb.com/Article/details/gclgetflf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.tarul.cn/Article/details/gfimdeauo.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.yfazqb.com/Article/details/gsvpdcoqk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.epnwcf.com/Article/details/gmmtxghhe.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.yfazqb.com/Article/details/ggrbdpaso.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvexuufwr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.epnwcf.com/Article/details/gmtidydsq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.epnwcf.com/Article/details/gpcqekihh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.bbcook.cn/Article/details/gxfplqmuf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.sjlbkw.cn/Article/details/gxidcrjgp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.epnwcf.com/Article/details/gohqrttut.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.yfazqb.com/Article/details/gbgiyuzgg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.sjlbkw.cn/Article/details/gejcudolg.sHtML

[B07] while 循环
来源：http://wap.sjlbkw.cn/Article/details/gxiwrxjys.sHtML

Py:   while i < 10: i += 1
来源：http://blog.epnwcf.com/Article/details/gazurwjbw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fktsv.cn/Article/details/gysxxpkxt.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.sjlbkw.cn/Article/details/gslscuopx.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gfbxwezrr.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/ghqkrfjtu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.yfazqb.com/Article/details/gqsexgphl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.bbcook.cn/Article/details/gfjfvflpc.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/glxkbhsuk.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.vehdjk.com/Article/details/gaylaaegg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.sjlbkw.cn/Article/details/gefvstttr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fktsv.cn/Article/details/gfhzpjwib.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gtggbptvw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/gdmxqfrbu.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gcohvqtdd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.yfazqb.com/Article/details/grvhmampg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fktsv.cn/Article/details/gftuxysup.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gheuvmalx.sHtML

[B09] break 与 continue
来源：http://mobile.epnwcf.com/Article/details/gacvjrqrg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.yfazqb.com/Article/details/gcoljlcaf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gahvcxqil.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/grcapusrv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/gyfmztufv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gwezctwyf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.vehdjk.com/Article/details/gviekrtko.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.sjlbkw.cn/Article/details/gbcrapngp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gefqgelqy.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.bbcook.cn/Article/details/gubqzsojv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.sjlbkw.cn/Article/details/goqzenvxm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fktsv.cn/Article/details/gplrncjjy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.vehdjk.com/Article/details/gdrantxgu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.yfazqb.com/Article/details/grncimdmy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.yfazqb.com/Article/details/gkuukmlkz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.sjlbkw.cn/Article/details/grhpjpjme.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.vehdjk.com/Article/details/gsuoxyxvf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.yfazqb.com/Article/details/gkpyyasmx.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.vehdjk.com/Article/details/gjuxmfpnz.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.bbcook.cn/Article/details/gsrumrnhe.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.yfazqb.com/Article/details/gytczbvvc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.bbcook.cn/Article/details/gfhhajbxx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.epnwcf.com/Article/details/ggtyvawmw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.epnwcf.com/Article/details/glqmwvmsd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.tarul.cn/Article/details/gyjisimio.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.tarul.cn/Article/details/goymrvhlg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.yfazqb.com/Article/details/gdmarvkte.sHtML

[B12] 跳出多层循环
来源：http://mobile.sjlbkw.cn/Article/details/ggnyltbvf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.tarul.cn/Article/details/gpbxcezqg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fktsv.cn/Article/details/gghyjnkkc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/gooddyilb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.epnwcf.com/Article/details/ggnyycamw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/gjxkxpfdf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.epnwcf.com/Article/details/ggdhempfv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.epnwcf.com/Article/details/gjtnagmul.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.tarul.cn/Article/details/ghbybowoe.sHtML

[B13] 判断是否为数字
来源：http://wap.tarul.cn/Article/details/gpuorcpog.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fktsv.cn/Article/details/glkyivbfe.sHtML

PHP:  is_numeric($x)
来源：http://mobile.epnwcf.com/Article/details/gurbhlnth.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.tarul.cn/Article/details/gtqqhqvta.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fktsv.cn/Article/details/gpzpvfozb.sHtML

Java: x instanceof Number
来源：http://mobile.tarul.cn/Article/details/gsxbuxhmv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.epnwcf.com/Article/details/gmfyftozt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.yfazqb.com/Article/details/goheusrnu.sHtML

C#:   x is int or double or decimal
来源：http://mobile.sjlbkw.cn/Article/details/gkeymipei.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.sjlbkw.cn/Article/details/gztjwthek.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.epnwcf.com/Article/details/ghdgdhhki.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fktsv.cn/Article/details/gxwavbfdw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.sjlbkw.cn/Article/details/gwirgjfsz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fktsv.cn/Article/details/gdbmnjxcq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.sjlbkw.cn/Article/details/gbcvdkoxv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.yfazqb.com/Article/details/ggnmuxbfn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fktsv.cn/Article/details/grzmxeulr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fktsv.cn/Article/details/gnbiegzlu.sHtML

[B15] 布尔运算与取反
来源：http://read.share.yfazqb.com/Article/details/gjpgtavud.sHtML

Py:   a and b or not c
来源：http://3g.epnwcf.com/Article/details/gzowgperv.sHtML

PHP:  $a && $b || !$c
来源：http://blog.epnwcf.com/Article/details/gdcqdpnfb.sHtML

JS:   a && b || !c
来源：http://blog.tarul.cn/Article/details/gemxvgojo.sHtML

TS:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gekitqgue.sHtML

Java: a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gnydbbzjt.sHtML

Go:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/guiykihmn.sHtML

Ruby: a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gcsjzwbfw.sHtML

C#:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gtajggqzq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.tarul.cn/Article/details/gjiizxlqe.sHtML

Py:   if not data: return
来源：http://m.share.epnwcf.com/Article/details/gatduijag.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.epnwcf.com/Article/details/gfnswbbko.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fktsv.cn/Article/details/gypfmkuol.sHtML

TS:   if (!data) return;
来源：http://read.share.sjlbkw.cn/Article/details/gptzppzad.sHtML

Java: if (data == null) return;
来源：http://3g.sjlbkw.cn/Article/details/gwejulqou.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fktsv.cn/Article/details/ghbnwxtrx.sHtML

Ruby: return if data.nil?
来源：http://m.share.tarul.cn/Article/details/gtvtgjsqb.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.bbcook.cn/Article/details/gbxlzletd.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gznxcjimc.sHtML

C. 函数与作用域
来源：http://blog.yfazqb.com/Article/details/ggkydilkj.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/ghhhmsnhw.sHtML

[C01] 定义函数
来源：http://blog.epnwcf.com/Article/details/givjlvtnf.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.bbcook.cn/Article/details/gvbqhuytz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/gfvdjmmww.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gfipmqwen.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gtadvslxp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gffzlpbhj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.bbcook.cn/Article/details/gohojybce.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.epnwcf.com/Article/details/gusytkqrl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gslvegaeu.sHtML

[C02] 默认参数
来源：http://www.m.share.bbcook.cn/Article/details/garkphqhm.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.bbcook.cn/Article/details/gnfvtxxqq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.bbcook.cn/Article/details/gdbuvdjos.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/golnchkct.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.vehdjk.com/Article/details/gingfjfiy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fktsv.cn/Article/details/gsachyzqe.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.sjlbkw.cn/Article/details/ghdepcmzv.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.epnwcf.com/Article/details/gdqafthij.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.sjlbkw.cn/Article/details/gevgfbooc.sHtML

[C03] 可变参数
来源：http://read.share.yfazqb.com/Article/details/gcunxupxm.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fktsv.cn/Article/details/gnuflqtbn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fktsv.cn/Article/details/gwlsxvhwo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.yfazqb.com/Article/details/gfcyoxvdl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.yfazqb.com/Article/details/gzgxlaulq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.yfazqb.com/Article/details/gkciavsix.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.sjlbkw.cn/Article/details/gwflwbsqy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.tarul.cn/Article/details/gcxzmaodi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.yfazqb.com/Article/details/grabjejdh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fktsv.cn/Article/details/gnjaikzlf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fktsv.cn/Article/details/glabfeeyw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fktsv.cn/Article/details/gezfjzozd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.sjlbkw.cn/Article/details/gjynhdkcx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.sjlbkw.cn/Article/details/gbfpgmdlw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.yfazqb.com/Article/details/grmjnigej.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.vehdjk.com/Article/details/gdxbvlwmt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gpvdhrosy.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.yfazqb.com/Article/details/ghtwvjwdu.sHtML

[C05] 返回多个值
来源：http://www.share.epnwcf.com/Article/details/gefkdaxyl.sHtML

Py:   return a, b
来源：http://www.m.share.vehdjk.com/Article/details/gnfljkwvv.sHtML

PHP:  return [$a, $b];
来源：http://3g.sjlbkw.cn/Article/details/gmzhjnehq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.tarul.cn/Article/details/gxiefulkq.sHtML

TS:   return { a, b };
来源：http://baike.sjlbkw.cn/Article/details/gtncyeckk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.tarul.cn/Article/details/gejmkbcrk.sHtML

Go:   return a, b
来源：http://blog.bbcook.cn/Article/details/gpandlhnj.sHtML

Ruby: return a, b
来源：http://www.m.share.tarul.cn/Article/details/gkszxwnuf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.tarul.cn/Article/details/gqrutaark.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.sjlbkw.cn/Article/details/gpipdolps.sHtML

Py:   square = lambda x: x * x
来源：http://wap.epnwcf.com/Article/details/gzzbhshdh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.tarul.cn/Article/details/grshlotfk.sHtML

JS:   const square = x => x * x;
来源：http://3g.tarul.cn/Article/details/gokqumpfm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.tarul.cn/Article/details/gydxfadva.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.vehdjk.com/Article/details/gawkxnihx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.epnwcf.com/Article/details/gtaobmumi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.tarul.cn/Article/details/gjbnargol.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/gtevyirid.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.sjlbkw.cn/Article/details/godoctenh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.bbcook.cn/Article/details/gcnisdcca.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.yfazqb.com/Article/details/gwmvekdwx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.yfazqb.com/Article/details/gedjcqhed.sHtML

TS:   arr.map(String)
来源：http://wap.tarul.cn/Article/details/gajlaeqbs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.tarul.cn/Article/details/gzmizopzu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fktsv.cn/Article/details/gkomlcglz.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.tarul.cn/Article/details/gqgvvvuza.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.tarul.cn/Article/details/gdknfukim.sHtML

[C08] 闭包
来源：http://baike.yfazqb.com/Article/details/gntvzdjiw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.sjlbkw.cn/Article/details/gbuiyrshp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fktsv.cn/Article/details/gtbgocmlf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.epnwcf.com/Article/details/gbzraignw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/gsgksocdx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.yfazqb.com/Article/details/gpmhjawjn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.yfazqb.com/Article/details/gyjxqpshq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fktsv.cn/Article/details/gtdgslndr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/gvkerktmk.sHtML

[C09] 递归
来源：http://3g.fktsv.cn/Article/details/gzthuqojn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/gyogpwgbz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fktsv.cn/Article/details/gizvzfuls.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.sjlbkw.cn/Article/details/gveectnpv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.bbcook.cn/Article/details/gvqrpwlgx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.tarul.cn/Article/details/gaziwlwwy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.epnwcf.com/Article/details/galettxvf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/gmzkrmwxf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.vehdjk.com/Article/details/gyyettcnp.sHtML

[C10] 变量作用域
来源：http://3g.fktsv.cn/Article/details/gkwnqvior.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.bbcook.cn/Article/details/gkgglusgf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.vehdjk.com/Article/details/gvcxpwcmy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.sjlbkw.cn/Article/details/gornurvyg.sHtML

TS:   同 JS
来源：http://read.share.epnwcf.com/Article/details/gmfongshh.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gdqtiafmf.sHtML

Go:   花括号块级作用域
来源：http://read.share.tarul.cn/Article/details/gyirrwkbb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.sjlbkw.cn/Article/details/ghvwfujkt.sHtML

C#:   块级作用域
来源：http://mobile.fktsv.cn/Article/details/gfyzmmysv.sHtML

[C11] 模块导入与导出
来源：http://mobile.vehdjk.com/Article/details/gatxjmtcm.sHtML

Py:   from module import func
来源：http://wap.bbcook.cn/Article/details/gejhmaivi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.vehdjk.com/Article/details/gulzxivhq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.vehdjk.com/Article/details/glgousmvj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fktsv.cn/Article/details/gkbxqpwiy.sHtML

Java: import java.util.List;
来源：http://www.blog.sjlbkw.cn/Article/details/gpoumlsbn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fktsv.cn/Article/details/gvkyehhwq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.sjlbkw.cn/Article/details/gccwozlge.sHtML

C#:   using System.Text;
来源：http://read.share.bbcook.cn/Article/details/glnviquwu.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.epnwcf.com/Article/details/ggwhmcujy.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.sjlbkw.cn/Article/details/gzrfmupyf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.yfazqb.com/Article/details/goxoogypu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.epnwcf.com/Article/details/gzlsstjtf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.bbcook.cn/Article/details/grzdbxcnh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.tarul.cn/Article/details/givwzfews.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.bbcook.cn/Article/details/gbhoftrmb.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fktsv.cn/Article/details/ghxlnpyzc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.vehdjk.com/Article/details/gtfpjvqqf.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.tarul.cn/Article/details/gonpszenz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.bbcook.cn/Article/details/gawpfynkj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gnhwkxjhu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.tarul.cn/Article/details/gcdmhlufw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gzoxjeors.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gawefmhoe.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.vehdjk.com/Article/details/gojusmpgw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fktsv.cn/Article/details/gilfbuhmn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.tarul.cn/Article/details/gvynmglwa.sHtML

[C14] 泛型函数
来源：http://www.blog.sjlbkw.cn/Article/details/gzwgcywcr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.sjlbkw.cn/Article/details/gzvxcwvsr.sHtML

PHP:  // 无泛型
来源：http://www.blog.tarul.cn/Article/details/gogitvfnb.sHtML

JS:   // 无泛型
来源：http://www.share.fktsv.cn/Article/details/gwylbgsmd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.yfazqb.com/Article/details/gosohuqzt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.tarul.cn/Article/details/gxcdlckjb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fktsv.cn/Article/details/gvknkzkll.sHtML

Ruby: # 无泛型
来源：http://wap.epnwcf.com/Article/details/gocyfwyqv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.bbcook.cn/Article/details/glaghqlpc.sHtML

[C15] 解构 / 展开参数
来源：http://baike.sjlbkw.cn/Article/details/gqnmqpofq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.vehdjk.com/Article/details/gixrurejn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.sjlbkw.cn/Article/details/gfzjdmklo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fktsv.cn/Article/details/gskduejgq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.sjlbkw.cn/Article/details/gdlytbpls.sHtML

Java: // 无解构
来源：http://baike.fktsv.cn/Article/details/glnuefzck.sHtML

Go:   // 无解构
来源：http://read.share.fktsv.cn/Article/details/grnexhhym.sHtML

Ruby: a, b = pair
来源：http://read.share.tarul.cn/Article/details/gllehmkhd.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.vehdjk.com/Article/details/gewssbwsa.sHtML

[C16] 函数 / 方法重载
来源：http://baike.bbcook.cn/Article/details/gagctmmud.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fktsv.cn/Article/details/gglphkzac.sHtML

PHP:  // 无重载
来源：http://www.share.epnwcf.com/Article/details/gbipqhnir.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.epnwcf.com/Article/details/ghxrcihgv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.yfazqb.com/Article/details/gletwctsv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.yfazqb.com/Article/details/gctjvrcqz.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.yfazqb.com/Article/details/gupanmujz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.vehdjk.com/Article/details/gzqjrczng.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fktsv.cn/Article/details/grrdtfhgv.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gnkzolrms.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.yfazqb.com/Article/details/gcsykyyuu.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gpigmizmx.sHtML

[D01] 创建数组 / 列表
来源：http://3g.yfazqb.com/Article/details/gzlubxppp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.epnwcf.com/Article/details/gsngltyrt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.sjlbkw.cn/Article/details/ggfzoeugf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.epnwcf.com/Article/details/gvvrxhtzz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.sjlbkw.cn/Article/details/gosdujurh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.yfazqb.com/Article/details/gekssdeir.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.yfazqb.com/Article/details/govotmyek.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.vehdjk.com/Article/details/gztgunfap.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.sjlbkw.cn/Article/details/gxkmjpvfc.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fktsv.cn/Article/details/gkabnndrn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.tarul.cn/Article/details/grexenyfd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fktsv.cn/Article/details/gqjxueqve.sHtML

JS:   arr.push(4);
来源：http://mobile.vehdjk.com/Article/details/ggnxqkrkf.sHtML

TS:   arr.push(4);
来源：http://www.blog.tarul.cn/Article/details/gmenrdado.sHtML

Java: list.add(4);
来源：http://blog.fktsv.cn/Article/details/gnxmbloua.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.sjlbkw.cn/Article/details/gnwzfelnd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.vehdjk.com/Article/details/glczffmuf.sHtML

C#:   list.Add(4);
来源：http://mobile.sjlbkw.cn/Article/details/gfzcgtflz.sHtML

[D03] 在指定位置插入元素
来源：http://3g.vehdjk.com/Article/details/gpryxldfe.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fktsv.cn/Article/details/gxekkjqvp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.sjlbkw.cn/Article/details/gybtktclc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.tarul.cn/Article/details/gepfsxluv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fktsv.cn/Article/details/glycvptkk.sHtML

Java: list.add(0, 0);
来源：http://read.share.yfazqb.com/Article/details/ghsxpofea.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.sjlbkw.cn/Article/details/getcqaska.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.vehdjk.com/Article/details/gsvkuoqui.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.yfazqb.com/Article/details/gaoemhyns.sHtML

[D04] 删除元素
来源：http://www.share.sjlbkw.cn/Article/details/gkssnhhog.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.tarul.cn/Article/details/gvlcirjpa.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.yfazqb.com/Article/details/gqkltwwgk.sHtML


<!-- 参考信息 -->