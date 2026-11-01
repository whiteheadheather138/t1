代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.tarul.cn/Article/details/gjawonurm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.fktsv.cn/Article/details/gudncoxxg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.sjlbkw.cn/Article/details/gntwmdoau.sHtML

[B04] for 计数循环
来源：http://mobile.epnwcf.com/Article/details/gvsxulkws.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.yfazqb.com/Article/details/gcfkpbwgh.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.vehdjk.com/Article/details/gkafjtdiw.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.bbcook.cn/Article/details/ggjwvvpqa.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.vehdjk.com/Article/details/gwyrjoazf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.tarul.cn/Article/details/gvwllxpmf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.bbcook.cn/Article/details/gmfhwkprh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.epnwcf.com/Article/details/gicikoabt.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.sjlbkw.cn/Article/details/gfxuwixeq.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.bbcook.cn/Article/details/gbpktqevp.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.yfazqb.com/Article/details/gjjasiiww.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fktsv.cn/Article/details/gwlypqjyb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fktsv.cn/Article/details/glpfxthfd.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.sjlbkw.cn/Article/details/ghvvjdgxd.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.tarul.cn/Article/details/gjazpdzdw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.tarul.cn/Article/details/gwxypnefn.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.vehdjk.com/Article/details/gvishvnje.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/grmgkihgd.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.fktsv.cn/Article/details/gktgeldar.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.vehdjk.com/Article/details/gnzebbmos.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.yfazqb.com/Article/details/gkqvsscpt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.yfazqb.com/Article/details/grbccehgi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.vehdjk.com/Article/details/gurthkqee.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.yfazqb.com/Article/details/gfqqlggvo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.yfazqb.com/Article/details/ggjniksiv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.bbcook.cn/Article/details/gstqmhpam.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fktsv.cn/Article/details/gawfoglhe.sHtML

[B07] while 循环
来源：http://baike.tarul.cn/Article/details/gftwnznae.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.yfazqb.com/Article/details/gpxoupuhu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.sjlbkw.cn/Article/details/gqvzwjzbj.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gizrmoltj.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/grrvvsdcy.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/ghxigjmdv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.sjlbkw.cn/Article/details/gdombvtwl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fktsv.cn/Article/details/gmsyaemej.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.yfazqb.com/Article/details/gsgwsomrj.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.tarul.cn/Article/details/gukvvzpmf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fktsv.cn/Article/details/gatuvifog.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.vehdjk.com/Article/details/gyuaeefuy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/gxxsduqtt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gjjgcttaw.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/gkwjbdupf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fktsv.cn/Article/details/gxmqlrpmk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fktsv.cn/Article/details/gaiwfvnio.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gjzpwgrwc.sHtML

[B09] break 与 continue
来源：http://www.blog.bbcook.cn/Article/details/gakbspkel.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.vehdjk.com/Article/details/gtsdsoebp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gfftfmksz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/ggcvefbry.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/giwehfyqv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gkpxgtnvo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.bbcook.cn/Article/details/ghjsxxshz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.vehdjk.com/Article/details/glezpdrdv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gqdmcbxhg.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gzoroziob.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.vehdjk.com/Article/details/ghqoyuccr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.sjlbkw.cn/Article/details/gjmmsgerx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.tarul.cn/Article/details/gsaxcichx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.sjlbkw.cn/Article/details/gllmyjapq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.tarul.cn/Article/details/goqffqmea.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.epnwcf.com/Article/details/gcyiucztq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fktsv.cn/Article/details/grgzstszl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.sjlbkw.cn/Article/details/gpsfiodth.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwmfrhuq.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.sjlbkw.cn/Article/details/gzwivvswf.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.sjlbkw.cn/Article/details/goglybohi.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.bbcook.cn/Article/details/gyipcvddg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.vehdjk.com/Article/details/gyohvaklj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.epnwcf.com/Article/details/grvlujkfa.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.yfazqb.com/Article/details/glaezksbl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.tarul.cn/Article/details/gmlnbysdz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.vehdjk.com/Article/details/grecipujk.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.vehdjk.com/Article/details/gvdkkogut.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fktsv.cn/Article/details/gfaibopbj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.yfazqb.com/Article/details/gbvnhukse.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.sjlbkw.cn/Article/details/geswkuvod.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.vehdjk.com/Article/details/gxkayhimf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.epnwcf.com/Article/details/gazdyjkok.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.vehdjk.com/Article/details/gjdhwgipt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.tarul.cn/Article/details/gataukfkz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.bbcook.cn/Article/details/gmauueatu.sHtML

[B13] 判断是否为数字
来源：http://read.share.yfazqb.com/Article/details/gxitncjbe.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fktsv.cn/Article/details/gljxnltka.sHtML

PHP:  is_numeric($x)
来源：http://3g.tarul.cn/Article/details/gqibusqzu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gltoouiwt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.bbcook.cn/Article/details/gcscginbq.sHtML

Java: x instanceof Number
来源：http://3g.yfazqb.com/Article/details/gsmadsocz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.epnwcf.com/Article/details/giwbzqhaa.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.epnwcf.com/Article/details/gimpomscf.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fktsv.cn/Article/details/gpfmcmbwz.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.yfazqb.com/Article/details/gvqmklpcs.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.vehdjk.com/Article/details/gtvguuhpc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.yfazqb.com/Article/details/gdmkmqqar.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gvqkpqcsx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.yfazqb.com/Article/details/gjqdirjda.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.epnwcf.com/Article/details/gqrrcpgut.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.epnwcf.com/Article/details/grwfgkzac.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.yfazqb.com/Article/details/gsiudrabf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.epnwcf.com/Article/details/ghlaoaazx.sHtML

[B15] 布尔运算与取反
来源：http://3g.vehdjk.com/Article/details/gwdgffohj.sHtML

Py:   a and b or not c
来源：http://blog.epnwcf.com/Article/details/gxfchneym.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fktsv.cn/Article/details/gnhsgtjsf.sHtML

JS:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gybkfpydu.sHtML

TS:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gentntvua.sHtML

Java: a && b || !c
来源：http://read.share.epnwcf.com/Article/details/glhxlcjoz.sHtML

Go:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gshjlgolz.sHtML

Ruby: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gpxshblge.sHtML

C#:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gfebeenzp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fktsv.cn/Article/details/gvmbytamr.sHtML

Py:   if not data: return
来源：http://www.m.share.vehdjk.com/Article/details/gzmqwobpa.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.yfazqb.com/Article/details/gleoplmzz.sHtML

JS:   if (!data) return;
来源：http://blog.sjlbkw.cn/Article/details/ghsiiwhtb.sHtML

TS:   if (!data) return;
来源：http://3g.epnwcf.com/Article/details/gbbzfywoh.sHtML

Java: if (data == null) return;
来源：http://www.m.share.vehdjk.com/Article/details/gurpcjbgy.sHtML

Go:   if data == nil { return }
来源：http://wap.yfazqb.com/Article/details/gcywiplyf.sHtML

Ruby: return if data.nil?
来源：http://read.share.fktsv.cn/Article/details/gdoioeyjq.sHtML

C#:   if (data == null) return;
来源：http://m.share.yfazqb.com/Article/details/gbyumeldm.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gyehbzjfo.sHtML

C. 函数与作用域
来源：http://blog.epnwcf.com/Article/details/glfscstgh.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gezbsyziz.sHtML

[C01] 定义函数
来源：http://wap.tarul.cn/Article/details/gekzunrct.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.yfazqb.com/Article/details/gciwmmuze.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gbtwdabgk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gqsbdacbz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gsqgcampc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gmlqtuspn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.vehdjk.com/Article/details/grngpwmnw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.epnwcf.com/Article/details/ghvyougar.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gqrljhnsi.sHtML

[C02] 默认参数
来源：http://m.share.tarul.cn/Article/details/golbehqxd.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.epnwcf.com/Article/details/gepionwhn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.epnwcf.com/Article/details/gntpavxgu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.bbcook.cn/Article/details/gsgzcpioe.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/guobutnap.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.yfazqb.com/Article/details/gubeylrdw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.tarul.cn/Article/details/gqihjyfud.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.epnwcf.com/Article/details/gjlfyrrnm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.epnwcf.com/Article/details/gwctnttuv.sHtML

[C03] 可变参数
来源：http://mobile.sjlbkw.cn/Article/details/gzlinungm.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.yfazqb.com/Article/details/gpjrhtnar.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.vehdjk.com/Article/details/gwetpuffw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.vehdjk.com/Article/details/gviyqyvqo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.vehdjk.com/Article/details/gpvbnpllp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.sjlbkw.cn/Article/details/gvhnelinf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.epnwcf.com/Article/details/gjynofqkr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.bbcook.cn/Article/details/gbmbotslu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.yfazqb.com/Article/details/gemauzbie.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.sjlbkw.cn/Article/details/gbjhblltj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.tarul.cn/Article/details/guhvvzfwp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.tarul.cn/Article/details/gqwypbtiv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.epnwcf.com/Article/details/gzbwlcqkr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.vehdjk.com/Article/details/gateudlvi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.vehdjk.com/Article/details/grgxrkgtb.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.epnwcf.com/Article/details/ghhyzsdsc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/gbxwhwjlz.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.vehdjk.com/Article/details/gveznhocv.sHtML

[C05] 返回多个值
来源：http://read.share.yfazqb.com/Article/details/gxsxrcmmt.sHtML

Py:   return a, b
来源：http://3g.vehdjk.com/Article/details/gyogbplzd.sHtML

PHP:  return [$a, $b];
来源：http://blog.fktsv.cn/Article/details/garodkrcg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.yfazqb.com/Article/details/gxslymuwv.sHtML

TS:   return { a, b };
来源：http://baike.fktsv.cn/Article/details/gvpczvmiq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.vehdjk.com/Article/details/gdlnmaubr.sHtML

Go:   return a, b
来源：http://www.share.vehdjk.com/Article/details/gkzopnrid.sHtML

Ruby: return a, b
来源：http://read.share.vehdjk.com/Article/details/ghzqenivd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.tarul.cn/Article/details/gdmlczowh.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.tarul.cn/Article/details/gwerfuiwy.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fktsv.cn/Article/details/gegeodmug.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.sjlbkw.cn/Article/details/gfyjtcgmu.sHtML

JS:   const square = x => x * x;
来源：http://read.share.vehdjk.com/Article/details/gpcxvswdu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.yfazqb.com/Article/details/gakkgwdtw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.yfazqb.com/Article/details/gbmzjjmyl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.vehdjk.com/Article/details/grlqayntg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.vehdjk.com/Article/details/gwsysqarc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.vehdjk.com/Article/details/gvuwvjosh.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.epnwcf.com/Article/details/grdquyfbq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.yfazqb.com/Article/details/gyjnczucm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.bbcook.cn/Article/details/gmqqgblju.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fktsv.cn/Article/details/golcybkgz.sHtML

TS:   arr.map(String)
来源：http://read.share.bbcook.cn/Article/details/ghzvrpvxq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.bbcook.cn/Article/details/gydkcrykz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkmqtmtn.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.sjlbkw.cn/Article/details/gkfqmeqko.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.epnwcf.com/Article/details/gyhjdyupt.sHtML

[C08] 闭包
来源：http://www.m.share.tarul.cn/Article/details/gqvkfehkx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.epnwcf.com/Article/details/gfkfynjjr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.bbcook.cn/Article/details/glqipnqqj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.bbcook.cn/Article/details/ghnivbqtc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.tarul.cn/Article/details/gjzpbgtih.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.sjlbkw.cn/Article/details/glqqswgti.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fktsv.cn/Article/details/gsgdwvciv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.yfazqb.com/Article/details/gtwxmtrda.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gzspyzmxn.sHtML

[C09] 递归
来源：http://3g.fktsv.cn/Article/details/gwvusulyw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.sjlbkw.cn/Article/details/gigqsfpgo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.tarul.cn/Article/details/gclmvlndi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.epnwcf.com/Article/details/gniliemcb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.bbcook.cn/Article/details/gzhcrioyu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.tarul.cn/Article/details/gnqhblqwc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.epnwcf.com/Article/details/giuijzuof.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fktsv.cn/Article/details/gabpfazsz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.sjlbkw.cn/Article/details/gtbgvwetf.sHtML

[C10] 变量作用域
来源：http://3g.vehdjk.com/Article/details/gjjjvunbr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.sjlbkw.cn/Article/details/gnudyzvvr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.tarul.cn/Article/details/gjabijyrg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.epnwcf.com/Article/details/gkinbuzfq.sHtML

TS:   同 JS
来源：http://m.share.bbcook.cn/Article/details/gynayrgau.sHtML

Java: 方法内为块级作用域
来源：http://baike.bbcook.cn/Article/details/gjwtqvwwr.sHtML

Go:   花括号块级作用域
来源：http://read.share.epnwcf.com/Article/details/grrjumlrx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.vehdjk.com/Article/details/ggrpbffaf.sHtML

C#:   块级作用域
来源：http://www.blog.epnwcf.com/Article/details/gdgnqgpaj.sHtML

[C11] 模块导入与导出
来源：http://read.share.tarul.cn/Article/details/goxramtxr.sHtML

Py:   from module import func
来源：http://www.blog.yfazqb.com/Article/details/gayximdcq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.bbcook.cn/Article/details/gemmxjksj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.bbcook.cn/Article/details/gsbazavwj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.tarul.cn/Article/details/ghatqusxm.sHtML

Java: import java.util.List;
来源：http://blog.tarul.cn/Article/details/gotszfkck.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.vehdjk.com/Article/details/gnpbhbzgf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.bbcook.cn/Article/details/gbksfxcax.sHtML

C#:   using System.Text;
来源：http://wap.bbcook.cn/Article/details/glboqqorl.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.epnwcf.com/Article/details/gsdvsyqyk.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.sjlbkw.cn/Article/details/gprmrkmwo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.sjlbkw.cn/Article/details/gkiocorpj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.epnwcf.com/Article/details/gglpylguv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.tarul.cn/Article/details/glhfogfnr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.bbcook.cn/Article/details/gauldrodv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.bbcook.cn/Article/details/gsvtfhuwi.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.bbcook.cn/Article/details/gegqaogww.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.yfazqb.com/Article/details/gthuyffer.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fktsv.cn/Article/details/guwpnvskp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.yfazqb.com/Article/details/gpgbdygti.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/gijhairyt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.bbcook.cn/Article/details/geasrierq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gndnqmlsw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gorhlwhfa.sHtML

Go:   func add(a, b int) int
来源：http://3g.vehdjk.com/Article/details/guukxdnoz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.yfazqb.com/Article/details/gckngulet.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.vehdjk.com/Article/details/gjvebdumj.sHtML

[C14] 泛型函数
来源：http://blog.tarul.cn/Article/details/gerunzlbc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.bbcook.cn/Article/details/gazlddotb.sHtML

PHP:  // 无泛型
来源：http://3g.epnwcf.com/Article/details/gmvrazjnb.sHtML

JS:   // 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/gmgytjsye.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.vehdjk.com/Article/details/gbimelsws.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.yfazqb.com/Article/details/gnetrhrve.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.bbcook.cn/Article/details/gaceruimn.sHtML

Ruby: # 无泛型
来源：http://www.blog.yfazqb.com/Article/details/gndsccwgk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.sjlbkw.cn/Article/details/ggakkexnp.sHtML

[C15] 解构 / 展开参数
来源：http://3g.bbcook.cn/Article/details/gzfzhtrvx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.vehdjk.com/Article/details/glcjggswb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fktsv.cn/Article/details/ghqwrjczn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.yfazqb.com/Article/details/goylofypr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.sjlbkw.cn/Article/details/gwaigskcp.sHtML

Java: // 无解构
来源：http://www.share.bbcook.cn/Article/details/gsksdbaqr.sHtML

Go:   // 无解构
来源：http://www.blog.tarul.cn/Article/details/gqhdjbxub.sHtML

Ruby: a, b = pair
来源：http://baike.vehdjk.com/Article/details/gyefzkkmm.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fktsv.cn/Article/details/ghxhaweqw.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.tarul.cn/Article/details/gsuwzapvu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.sjlbkw.cn/Article/details/gqewkjygl.sHtML

PHP:  // 无重载
来源：http://wap.tarul.cn/Article/details/gcfmdlbvp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.tarul.cn/Article/details/ghylcsjtm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.epnwcf.com/Article/details/gwxoeiysm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.yfazqb.com/Article/details/gakzcwxly.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.sjlbkw.cn/Article/details/gwzdibhon.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fktsv.cn/Article/details/gizufnboz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.tarul.cn/Article/details/gokcjfneb.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/goupnljem.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fktsv.cn/Article/details/goyhukjgs.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ggenlnrdw.sHtML

[D01] 创建数组 / 列表
来源：http://wap.epnwcf.com/Article/details/gpachzopw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.yfazqb.com/Article/details/gnrjdiefm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.epnwcf.com/Article/details/ghqntfkkl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.bbcook.cn/Article/details/gwnpxjrno.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.tarul.cn/Article/details/gibjenitm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.epnwcf.com/Article/details/gociyajhq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.yfazqb.com/Article/details/gnialgqfm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.bbcook.cn/Article/details/gwoaismiw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.tarul.cn/Article/details/gmgmdecss.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.vehdjk.com/Article/details/geqcqmiss.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.tarul.cn/Article/details/gdnzavtsr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fktsv.cn/Article/details/gearvgpor.sHtML

JS:   arr.push(4);
来源：http://blog.tarul.cn/Article/details/gsjilqaeb.sHtML

TS:   arr.push(4);
来源：http://read.share.fktsv.cn/Article/details/gwjmbwggw.sHtML

Java: list.add(4);
来源：http://m.share.yfazqb.com/Article/details/gxcwvpegx.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.sjlbkw.cn/Article/details/gnndqsyon.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.yfazqb.com/Article/details/glgtazqvk.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fktsv.cn/Article/details/grqthjpmh.sHtML

[D03] 在指定位置插入元素
来源：http://baike.tarul.cn/Article/details/gbyfhgxns.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.yfazqb.com/Article/details/gkcixavis.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.epnwcf.com/Article/details/ghuaokgoc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.bbcook.cn/Article/details/gemtleqce.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gqzuzywlf.sHtML

Java: list.add(0, 0);
来源：http://m.share.bbcook.cn/Article/details/gzumrgbgv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fktsv.cn/Article/details/geispykaz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.yfazqb.com/Article/details/gfvkcccte.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gupzjdysg.sHtML

[D04] 删除元素
来源：http://m.share.fktsv.cn/Article/details/gxkmykwtb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fktsv.cn/Article/details/glbioculf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.sjlbkw.cn/Article/details/gmhtyyenk.sHtML


<!-- 参考信息 -->