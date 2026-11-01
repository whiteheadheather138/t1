代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.vehdjk.com/Article/details/gqxkdhjaq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/glbxnrflt.sHtML

[B03] switch / match / case
来源：http://baike.sjlbkw.cn/Article/details/gwznsuaoh.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.yfazqb.com/Article/details/grpdocigx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gsgxtiuqj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.tarul.cn/Article/details/gwarfrfqf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/gpagnojen.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.epnwcf.com/Article/details/gqypzxsph.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.vehdjk.com/Article/details/gqgblxqzd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fktsv.cn/Article/details/gxittxkoz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.sjlbkw.cn/Article/details/grwnmivbb.sHtML

[B04] for 计数循环
来源：http://www.share.sjlbkw.cn/Article/details/givlsgpjl.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.epnwcf.com/Article/details/gcllafxua.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.yfazqb.com/Article/details/gseqwhxnz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.tarul.cn/Article/details/gybffzfzk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.yfazqb.com/Article/details/grpiortal.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.tarul.cn/Article/details/gfqkrjfzt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.yfazqb.com/Article/details/gbopwulpd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.vehdjk.com/Article/details/gtmjgazcp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.epnwcf.com/Article/details/gksgbnrpy.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.yfazqb.com/Article/details/gdnhqzxek.sHtML

Py:   for item in arr: print(item)
来源：http://baike.tarul.cn/Article/details/gewwtpopq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.tarul.cn/Article/details/gkplgqfdz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.vehdjk.com/Article/details/gpagwrtcw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.yfazqb.com/Article/details/ggzrbhwee.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.tarul.cn/Article/details/gbetxitwr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.epnwcf.com/Article/details/gdzjwaccl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.epnwcf.com/Article/details/gzatqjawf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.vehdjk.com/Article/details/ggeqglnsc.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.vehdjk.com/Article/details/gadqqqzlz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.yfazqb.com/Article/details/gkxxrycgn.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.bbcook.cn/Article/details/gopxmrbcz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.yfazqb.com/Article/details/ggcnpyitg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.tarul.cn/Article/details/geakgmgle.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.epnwcf.com/Article/details/glcyjvcrv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.tarul.cn/Article/details/gvmwpixzx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.vehdjk.com/Article/details/gdtmcsopo.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.epnwcf.com/Article/details/gscjuodmv.sHtML

[B07] while 循环
来源：http://m.share.bbcook.cn/Article/details/gpmfewksv.sHtML

Py:   while i < 10: i += 1
来源：http://blog.yfazqb.com/Article/details/gvzeqlbqa.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.yfazqb.com/Article/details/gpsctxtju.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/giohganax.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/grjtvfohi.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.epnwcf.com/Article/details/gvrzgeaxc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.bbcook.cn/Article/details/gjeleosvz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.tarul.cn/Article/details/gfafjkfrh.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fktsv.cn/Article/details/giffeulvx.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.vehdjk.com/Article/details/gbozpopqf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.tarul.cn/Article/details/gwsvemfkx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gmfhncqzc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/gpfschett.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/gvyccgagq.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gscxvlfld.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.yfazqb.com/Article/details/gvmlaundd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.bbcook.cn/Article/details/gjkiuiqmq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gzfsgdywv.sHtML

[B09] break 与 continue
来源：http://m.share.fktsv.cn/Article/details/gvwsyszkq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.tarul.cn/Article/details/gcruopkqo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gxjomihnt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/gocpqeepu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gmewgttyu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gepdcaxmu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.yfazqb.com/Article/details/gtxqwohxk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fktsv.cn/Article/details/gxbsfugud.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/geoqzlfjh.sHtML

[B10] 遍历同时拿索引
来源：http://blog.bbcook.cn/Article/details/gvlcgplws.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.yfazqb.com/Article/details/gqpebtfmu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.sjlbkw.cn/Article/details/grmgrzlrv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.tarul.cn/Article/details/gqcjuzxol.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.yfazqb.com/Article/details/gwywqszpl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.sjlbkw.cn/Article/details/gvejhjfqc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fktsv.cn/Article/details/gbzhxsibq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.bbcook.cn/Article/details/gknzhwvle.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.sjlbkw.cn/Article/details/gxwecnaoq.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fktsv.cn/Article/details/gaajlmope.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.epnwcf.com/Article/details/gmzjpsamn.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.vehdjk.com/Article/details/gsuupfzsp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.vehdjk.com/Article/details/gstfhegqh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.epnwcf.com/Article/details/guyrobztg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fktsv.cn/Article/details/gmwsshkkv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.tarul.cn/Article/details/gifekcjly.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.epnwcf.com/Article/details/gttoxxzlv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.epnwcf.com/Article/details/gswthpoeg.sHtML

[B12] 跳出多层循环
来源：http://www.blog.vehdjk.com/Article/details/ggzkhcjrl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fktsv.cn/Article/details/gsqardgpj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fktsv.cn/Article/details/gupxxpidq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkibvijys.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/glveajquk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.epnwcf.com/Article/details/gmplyjmkk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.bbcook.cn/Article/details/gqlyaddyv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.tarul.cn/Article/details/gafwwboxw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.sjlbkw.cn/Article/details/ggtpnrkay.sHtML

[B13] 判断是否为数字
来源：http://www.share.epnwcf.com/Article/details/gbnfzkoza.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.vehdjk.com/Article/details/giyblondr.sHtML

PHP:  is_numeric($x)
来源：http://m.share.epnwcf.com/Article/details/gsisbdsdj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.epnwcf.com/Article/details/ginldnves.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.bbcook.cn/Article/details/gphxicjqh.sHtML

Java: x instanceof Number
来源：http://www.blog.bbcook.cn/Article/details/gpasazcmf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.tarul.cn/Article/details/gosddxyzk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.epnwcf.com/Article/details/ghjuglkey.sHtML

C#:   x is int or double or decimal
来源：http://baike.fktsv.cn/Article/details/gkkpziqzx.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.sjlbkw.cn/Article/details/gsuymhtve.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fktsv.cn/Article/details/gkrbnbara.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.bbcook.cn/Article/details/gncybijja.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.yfazqb.com/Article/details/gegniwuci.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.tarul.cn/Article/details/gdzccyiwl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.vehdjk.com/Article/details/gwubwnaix.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.sjlbkw.cn/Article/details/gjlhrgbgk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/gqhlnnekh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.bbcook.cn/Article/details/gqphxqswa.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fktsv.cn/Article/details/grpuildgz.sHtML

Py:   a and b or not c
来源：http://blog.yfazqb.com/Article/details/gquegiole.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.epnwcf.com/Article/details/grvslqfdt.sHtML

JS:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/glesfpftz.sHtML

TS:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gfxcxvmsi.sHtML

Java: a && b || !c
来源：http://blog.tarul.cn/Article/details/gtnvozbhr.sHtML

Go:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gszjvmnbx.sHtML

Ruby: a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gcwhkiskd.sHtML

C#:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gaxsdxjde.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.sjlbkw.cn/Article/details/gqvigvlht.sHtML

Py:   if not data: return
来源：http://mobile.yfazqb.com/Article/details/gjydqercq.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.bbcook.cn/Article/details/gabrzytyf.sHtML

JS:   if (!data) return;
来源：http://wap.fktsv.cn/Article/details/gjjxsxvqb.sHtML

TS:   if (!data) return;
来源：http://baike.sjlbkw.cn/Article/details/gzzzhjimt.sHtML

Java: if (data == null) return;
来源：http://baike.tarul.cn/Article/details/gdurdqgcq.sHtML

Go:   if data == nil { return }
来源：http://blog.bbcook.cn/Article/details/gzfgxdvec.sHtML

Ruby: return if data.nil?
来源：http://read.share.yfazqb.com/Article/details/gbuqphrtd.sHtML

C#:   if (data == null) return;
来源：http://m.share.vehdjk.com/Article/details/gpbbwodad.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gpbggpkzt.sHtML

C. 函数与作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrujsbhr.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gcahwtbub.sHtML

[C01] 定义函数
来源：http://wap.epnwcf.com/Article/details/gzkvldaxe.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.tarul.cn/Article/details/gapdcmdwa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gmtuyndey.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/giboaatys.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gwndaasly.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gvnfhoujh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.vehdjk.com/Article/details/grmgemgvf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.tarul.cn/Article/details/gofsspwpi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gdhxmpdrz.sHtML

[C02] 默认参数
来源：http://mobile.sjlbkw.cn/Article/details/glnprznhp.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.vehdjk.com/Article/details/gmuknbgqk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.vehdjk.com/Article/details/gozhyvque.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.bbcook.cn/Article/details/gogwkxbro.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.yfazqb.com/Article/details/gunzanqho.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.yfazqb.com/Article/details/gyqupmwrf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.epnwcf.com/Article/details/ggxhwpzlo.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fktsv.cn/Article/details/gpodjjevn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.vehdjk.com/Article/details/gcheyvjpn.sHtML

[C03] 可变参数
来源：http://mobile.sjlbkw.cn/Article/details/gsnyflngd.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.tarul.cn/Article/details/gdcgnbotg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.epnwcf.com/Article/details/gjmxsqaru.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.epnwcf.com/Article/details/gzmgptxlc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.vehdjk.com/Article/details/gsvcjczkm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.yfazqb.com/Article/details/gafmodxqw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.yfazqb.com/Article/details/gqsfpwivi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.sjlbkw.cn/Article/details/gzpajsnwi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fktsv.cn/Article/details/gyzyelwmp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.epnwcf.com/Article/details/gerfjnytu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.bbcook.cn/Article/details/ggwmgsvam.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.tarul.cn/Article/details/gmymgcqwo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhoryuys.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.sjlbkw.cn/Article/details/gizrejuxf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.epnwcf.com/Article/details/gnojzezxm.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.bbcook.cn/Article/details/geqdiflyj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gfchcydba.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/gaaewqnph.sHtML

[C05] 返回多个值
来源：http://www.m.share.vehdjk.com/Article/details/gycojikfa.sHtML

Py:   return a, b
来源：http://wap.sjlbkw.cn/Article/details/gedfqbnqm.sHtML

PHP:  return [$a, $b];
来源：http://blog.fktsv.cn/Article/details/gfmngbckf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.sjlbkw.cn/Article/details/gknmjppdi.sHtML

TS:   return { a, b };
来源：http://www.share.epnwcf.com/Article/details/gshmpyxpx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.tarul.cn/Article/details/gbhdogurc.sHtML

Go:   return a, b
来源：http://baike.bbcook.cn/Article/details/gylwhfwag.sHtML

Ruby: return a, b
来源：http://mobile.bbcook.cn/Article/details/gpccdzyks.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.bbcook.cn/Article/details/gcamzqtfd.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.tarul.cn/Article/details/gcloepepy.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fktsv.cn/Article/details/gylpiticq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.sjlbkw.cn/Article/details/gslgwrdun.sHtML

JS:   const square = x => x * x;
来源：http://www.share.tarul.cn/Article/details/gxqvghhkz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.yfazqb.com/Article/details/gvtssnnyv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fktsv.cn/Article/details/gojfxmogu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.sjlbkw.cn/Article/details/gsiaqziua.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.tarul.cn/Article/details/gteijegjt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fktsv.cn/Article/details/ggizqingi.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.vehdjk.com/Article/details/gtzsxgsgh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.tarul.cn/Article/details/gpkdqyzht.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gvnisgusr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.sjlbkw.cn/Article/details/gmnizezfj.sHtML

TS:   arr.map(String)
来源：http://baike.tarul.cn/Article/details/geipkefdp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.epnwcf.com/Article/details/gtnppnpbs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fktsv.cn/Article/details/gfhffklpt.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvuqdjvmy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.tarul.cn/Article/details/ggazssukt.sHtML

[C08] 闭包
来源：http://www.blog.tarul.cn/Article/details/gpofhidqy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.vehdjk.com/Article/details/gucoxtqqa.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.yfazqb.com/Article/details/gmruxigcg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.bbcook.cn/Article/details/gkqjcqijf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gqfsldhty.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.vehdjk.com/Article/details/gbvarspey.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.vehdjk.com/Article/details/gtbvntshb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.bbcook.cn/Article/details/gpldadbzl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.epnwcf.com/Article/details/gjnrpogad.sHtML

[C09] 递归
来源：http://www.m.share.yfazqb.com/Article/details/ggkgdjqqa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.tarul.cn/Article/details/gmipjxcnm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.sjlbkw.cn/Article/details/gaxzibdzm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.sjlbkw.cn/Article/details/gbsweuyyy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.tarul.cn/Article/details/gzbvslxsb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.tarul.cn/Article/details/gfnxzujoy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.tarul.cn/Article/details/gtzfhmjsb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.yfazqb.com/Article/details/gxenyqycf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.tarul.cn/Article/details/grnzqfjin.sHtML

[C10] 变量作用域
来源：http://3g.sjlbkw.cn/Article/details/gxeybwdsl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.tarul.cn/Article/details/guzrnukjb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.yfazqb.com/Article/details/gjfgdctcw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.bbcook.cn/Article/details/grnaabubm.sHtML

TS:   同 JS
来源：http://read.share.vehdjk.com/Article/details/gzpdhxidn.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/grllhalbf.sHtML

Go:   花括号块级作用域
来源：http://wap.sjlbkw.cn/Article/details/guzaswcbq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fktsv.cn/Article/details/geehhpomx.sHtML

C#:   块级作用域
来源：http://www.blog.yfazqb.com/Article/details/gtohgjbnd.sHtML

[C11] 模块导入与导出
来源：http://m.share.epnwcf.com/Article/details/gpgjqjxwz.sHtML

Py:   from module import func
来源：http://read.share.bbcook.cn/Article/details/gjzsbxfmy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.sjlbkw.cn/Article/details/giaebbxte.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.bbcook.cn/Article/details/ggjlbufwe.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.tarul.cn/Article/details/gnrxzljom.sHtML

Java: import java.util.List;
来源：http://www.m.share.tarul.cn/Article/details/gbbimzeoj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.vehdjk.com/Article/details/gmszhziyu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.bbcook.cn/Article/details/gkwtcywne.sHtML

C#:   using System.Text;
来源：http://3g.epnwcf.com/Article/details/gmbysfihg.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.yfazqb.com/Article/details/gmnjxmutg.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.yfazqb.com/Article/details/gthovdota.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.sjlbkw.cn/Article/details/gycwybhso.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.yfazqb.com/Article/details/gutylypbn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.vehdjk.com/Article/details/gwmansiib.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.vehdjk.com/Article/details/gowhdhqyq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.tarul.cn/Article/details/gjuxwmsay.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.yfazqb.com/Article/details/gdqyfyjwn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gahrkbpvn.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fktsv.cn/Article/details/gpnlbfqzd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.vehdjk.com/Article/details/gpxxnwsrw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.yfazqb.com/Article/details/gqzrrcziw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.sjlbkw.cn/Article/details/gnlcqmjht.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.epnwcf.com/Article/details/ggkhcaxqz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/guzheamci.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.bbcook.cn/Article/details/gzubgdrqd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.bbcook.cn/Article/details/grvozyjsv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.epnwcf.com/Article/details/gkpqhraah.sHtML

[C14] 泛型函数
来源：http://www.m.share.epnwcf.com/Article/details/gcejlwehn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.yfazqb.com/Article/details/gqstsipnh.sHtML

PHP:  // 无泛型
来源：http://blog.epnwcf.com/Article/details/grihjjjus.sHtML

JS:   // 无泛型
来源：http://3g.fktsv.cn/Article/details/gkgscjeyy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.sjlbkw.cn/Article/details/gmmofzyse.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.vehdjk.com/Article/details/gflpjarhz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.yfazqb.com/Article/details/ghpppzazc.sHtML

Ruby: # 无泛型
来源：http://www.blog.bbcook.cn/Article/details/gyzjrspkf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.yfazqb.com/Article/details/grqkcgdpd.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.yfazqb.com/Article/details/gzjdjcpcq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.tarul.cn/Article/details/gggiuquyr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.bbcook.cn/Article/details/gbpawtahk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.bbcook.cn/Article/details/gvjymqbll.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.vehdjk.com/Article/details/gdxeurczt.sHtML

Java: // 无解构
来源：http://wap.epnwcf.com/Article/details/gzbidhklo.sHtML

Go:   // 无解构
来源：http://www.m.share.bbcook.cn/Article/details/gjarnduta.sHtML

Ruby: a, b = pair
来源：http://blog.epnwcf.com/Article/details/gjlzxwvyr.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fktsv.cn/Article/details/gsliwswbu.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.epnwcf.com/Article/details/gzafhlbfw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.vehdjk.com/Article/details/gclgwjzoq.sHtML

PHP:  // 无重载
来源：http://blog.epnwcf.com/Article/details/gpcvcwqqr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.vehdjk.com/Article/details/garlrufcy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.tarul.cn/Article/details/gzkbefkss.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.bbcook.cn/Article/details/gtsmffgtl.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.yfazqb.com/Article/details/gjcjxbxns.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.tarul.cn/Article/details/glzrlcbba.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.tarul.cn/Article/details/gqlvulewv.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gxyaicomw.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.epnwcf.com/Article/details/goslijsls.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/garfsdzdt.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.bbcook.cn/Article/details/gylkxgivz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.tarul.cn/Article/details/ghdcgdyva.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.yfazqb.com/Article/details/goekjihet.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fktsv.cn/Article/details/gcdxohakr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.vehdjk.com/Article/details/gyqwpxiyb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.bbcook.cn/Article/details/gymkujhpa.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fktsv.cn/Article/details/geyufldko.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.vehdjk.com/Article/details/gcfniniuf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.yfazqb.com/Article/details/gcwcvtdce.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.epnwcf.com/Article/details/gwedptnwd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fktsv.cn/Article/details/gbqqxtkrl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.tarul.cn/Article/details/gjuwivvfg.sHtML

JS:   arr.push(4);
来源：http://m.share.epnwcf.com/Article/details/gvqmjgyyz.sHtML

TS:   arr.push(4);
来源：http://3g.bbcook.cn/Article/details/ggcnmswfw.sHtML

Java: list.add(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrkqvzhu.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.yfazqb.com/Article/details/gdtmsnvih.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.sjlbkw.cn/Article/details/geugzfwbc.sHtML

C#:   list.Add(4);
来源：http://baike.vehdjk.com/Article/details/gkvufytbw.sHtML

[D03] 在指定位置插入元素
来源：http://blog.vehdjk.com/Article/details/glwgbuzub.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.tarul.cn/Article/details/gnyqfifll.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fktsv.cn/Article/details/gbmstpcqe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fktsv.cn/Article/details/gckgojlwe.sHtML


<!-- 参考信息 -->