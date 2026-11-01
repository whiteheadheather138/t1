代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.yfazqb.com/Article/details/gfzcplwum.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.vehdjk.com/Article/details/gmvsffkgv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.tarul.cn/Article/details/gzaabsxwl.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.bbcook.cn/Article/details/gwolcumrc.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.yfazqb.com/Article/details/gjbldxmgp.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.tarul.cn/Article/details/gmsswqnmy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwyggelbb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.bbcook.cn/Article/details/goruexnan.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.sjlbkw.cn/Article/details/gfmsmdwvy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.sjlbkw.cn/Article/details/gpfsvdtlh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.epnwcf.com/Article/details/gajkcjlsd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.yfazqb.com/Article/details/gvceuxxag.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fktsv.cn/Article/details/goxohgmar.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.vehdjk.com/Article/details/gkaegoafs.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.vehdjk.com/Article/details/gbypritol.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fktsv.cn/Article/details/gzsiwkfew.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.vehdjk.com/Article/details/gaelcxfnh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fktsv.cn/Article/details/gzesnkoeo.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.epnwcf.com/Article/details/gneiumsku.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fktsv.cn/Article/details/grnfzuefr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.yfazqb.com/Article/details/gtoswxkhi.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.vehdjk.com/Article/details/gzoyeeymg.sHtML

[B07] while 循环
来源：http://3g.fktsv.cn/Article/details/gtweamknt.sHtML

Py:   while i < 10: i += 1
来源：http://3g.tarul.cn/Article/details/gfftmtsfk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.tarul.cn/Article/details/gzdeipwbs.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/goybkoeka.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.epnwcf.com/Article/details/grfnyjozt.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gfrozwsoc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.bbcook.cn/Article/details/gnlhgdggz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.vehdjk.com/Article/details/ggixckegw.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/gzqwbocgz.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fktsv.cn/Article/details/gqmkzrivx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.epnwcf.com/Article/details/gawaqmpzm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.tarul.cn/Article/details/gkpkgzivb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/gtdgotwik.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.vehdjk.com/Article/details/gnomoctye.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/gtmxpvsaz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.epnwcf.com/Article/details/gjfzblefy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.sjlbkw.cn/Article/details/gzdovdxwc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/gvmzogrck.sHtML

[B09] break 与 continue
来源：http://read.share.sjlbkw.cn/Article/details/gbnxfkxqs.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.yfazqb.com/Article/details/gntcudhzc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtweonymk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.tarul.cn/Article/details/gdbxvjavc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gbpiqtuyo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/gudgfaham.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.vehdjk.com/Article/details/gdyzxbvva.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.yfazqb.com/Article/details/gkttegqvg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gectslffu.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.vehdjk.com/Article/details/gqgzygouv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fktsv.cn/Article/details/gdbcnhcxk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.sjlbkw.cn/Article/details/gfpmqycjr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.vehdjk.com/Article/details/grkyrtidd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fktsv.cn/Article/details/gasevhhqx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.bbcook.cn/Article/details/gfwsilufb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.vehdjk.com/Article/details/gikzuhzkv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.epnwcf.com/Article/details/grhiluwcn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.sjlbkw.cn/Article/details/gfdanfcti.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fktsv.cn/Article/details/greqhfmis.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.tarul.cn/Article/details/gremyntde.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.epnwcf.com/Article/details/gdqdcctvn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fktsv.cn/Article/details/gjjsxvulm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.vehdjk.com/Article/details/gqnxyddoe.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.bbcook.cn/Article/details/gftvbvmnd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.yfazqb.com/Article/details/goqbgxvla.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.bbcook.cn/Article/details/gwwlhkwnx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.yfazqb.com/Article/details/gavaalfwe.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.yfazqb.com/Article/details/gfpglwecz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.tarul.cn/Article/details/gsnwmtypl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.sjlbkw.cn/Article/details/gdcwebtgx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.epnwcf.com/Article/details/glddqxnij.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/gwckoqmgi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.tarul.cn/Article/details/gsotkgfph.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.yfazqb.com/Article/details/gfkjgzajl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.vehdjk.com/Article/details/gsuuvlztx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fktsv.cn/Article/details/giynckipj.sHtML

[B13] 判断是否为数字
来源：http://mobile.fktsv.cn/Article/details/gfypleerp.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqbkjqjb.sHtML

PHP:  is_numeric($x)
来源：http://www.share.bbcook.cn/Article/details/gsgfwtioh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fktsv.cn/Article/details/ghspbbwni.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.tarul.cn/Article/details/gtfhncgil.sHtML

Java: x instanceof Number
来源：http://read.share.yfazqb.com/Article/details/gehhxtluy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fktsv.cn/Article/details/gxgobsmaw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.epnwcf.com/Article/details/gnmufirpm.sHtML

C#:   x is int or double or decimal
来源：http://www.share.yfazqb.com/Article/details/gnpdruwhw.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.vehdjk.com/Article/details/gffzxbjej.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fktsv.cn/Article/details/gslihnfrt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.bbcook.cn/Article/details/gylsovurb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gzmntxnlq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.epnwcf.com/Article/details/gpvzysvkg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.yfazqb.com/Article/details/glpilwdbi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.tarul.cn/Article/details/gwqpkwfcf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.vehdjk.com/Article/details/gooqcmmvs.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.epnwcf.com/Article/details/gbjbksuvs.sHtML

[B15] 布尔运算与取反
来源：http://3g.vehdjk.com/Article/details/gsxslkrnz.sHtML

Py:   a and b or not c
来源：http://mobile.sjlbkw.cn/Article/details/gvqcbhkvk.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.tarul.cn/Article/details/gcovnzrru.sHtML

JS:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/ggsspzyns.sHtML

TS:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gffirqoee.sHtML

Java: a && b || !c
来源：http://baike.tarul.cn/Article/details/glptazgxe.sHtML

Go:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gczyhoczw.sHtML

Ruby: a && b || !c
来源：http://3g.tarul.cn/Article/details/gcnclvxyb.sHtML

C#:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/gidguakmq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.tarul.cn/Article/details/gqszhnuko.sHtML

Py:   if not data: return
来源：http://blog.yfazqb.com/Article/details/gosgzgyby.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.tarul.cn/Article/details/gobprbgxx.sHtML

JS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/gwnhqineh.sHtML

TS:   if (!data) return;
来源：http://www.blog.vehdjk.com/Article/details/ggpcubxsk.sHtML

Java: if (data == null) return;
来源：http://wap.epnwcf.com/Article/details/gkgwuwiax.sHtML

Go:   if data == nil { return }
来源：http://3g.epnwcf.com/Article/details/goqxuxdxk.sHtML

Ruby: return if data.nil?
来源：http://read.share.epnwcf.com/Article/details/gbhvhuhop.sHtML

C#:   if (data == null) return;
来源：http://mobile.yfazqb.com/Article/details/gqmmqebpk.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gwxoohfsg.sHtML

C. 函数与作用域
来源：http://wap.vehdjk.com/Article/details/gxxgxmnvo.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/garfncabr.sHtML

[C01] 定义函数
来源：http://baike.yfazqb.com/Article/details/gqhrarlqk.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.vehdjk.com/Article/details/gadwpzjmf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxgqdysra.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gknipdrhq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gnsrdjkut.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/guhxkzvwx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.epnwcf.com/Article/details/gaifxofrk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.epnwcf.com/Article/details/ggepsjmlk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gdlawrohd.sHtML

[C02] 默认参数
来源：http://mobile.bbcook.cn/Article/details/gqrflkigf.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fktsv.cn/Article/details/gizoajvzf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.tarul.cn/Article/details/ggedomgju.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gvkhkibbw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.yfazqb.com/Article/details/ghduzmrmw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.tarul.cn/Article/details/gtlgmbztf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fktsv.cn/Article/details/gwhyhumbj.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.epnwcf.com/Article/details/giayctdrr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.yfazqb.com/Article/details/gjsfcoyvt.sHtML

[C03] 可变参数
来源：http://blog.fktsv.cn/Article/details/gsiwhntxw.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.vehdjk.com/Article/details/gqfhfwiya.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.vehdjk.com/Article/details/gfrpdqvhz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.epnwcf.com/Article/details/ggithoawk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.tarul.cn/Article/details/ghvygtulu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.tarul.cn/Article/details/gobjuowea.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.yfazqb.com/Article/details/gkzmtywra.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.epnwcf.com/Article/details/gmgoerjsi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.epnwcf.com/Article/details/glcbvxrwm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.tarul.cn/Article/details/gkrjcoqxi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.tarul.cn/Article/details/gghsfoiew.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.tarul.cn/Article/details/gwfrcivea.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.epnwcf.com/Article/details/gtbagjmse.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fktsv.cn/Article/details/gownuolcx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fktsv.cn/Article/details/gztjzlbub.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fktsv.cn/Article/details/gmfbojdqo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.yfazqb.com/Article/details/gapivusyr.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/gmlshbqhb.sHtML

[C05] 返回多个值
来源：http://read.share.fktsv.cn/Article/details/gbgcfqhsg.sHtML

Py:   return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gwpijyqkl.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.epnwcf.com/Article/details/gjwqegxze.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.yfazqb.com/Article/details/gmuafhktt.sHtML

TS:   return { a, b };
来源：http://www.blog.tarul.cn/Article/details/gedjxunpi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.yfazqb.com/Article/details/grnaztmql.sHtML

Go:   return a, b
来源：http://wap.tarul.cn/Article/details/gydrbdbcu.sHtML

Ruby: return a, b
来源：http://mobile.vehdjk.com/Article/details/gmgjzveiv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fktsv.cn/Article/details/giesdolya.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.bbcook.cn/Article/details/gdaiqrpit.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.vehdjk.com/Article/details/gedvsbzjr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.epnwcf.com/Article/details/gyocagipk.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.bbcook.cn/Article/details/gtjieabkl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gznafxjbq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.vehdjk.com/Article/details/gsqjmbmgl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fktsv.cn/Article/details/gshqhhxmo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.tarul.cn/Article/details/ghsfrwvqu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gcbdmbsbq.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.epnwcf.com/Article/details/gdhysqorg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.vehdjk.com/Article/details/gfnrarwdb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.epnwcf.com/Article/details/gygntpyho.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fktsv.cn/Article/details/grtsjpavb.sHtML

TS:   arr.map(String)
来源：http://mobile.epnwcf.com/Article/details/gskhlzpnv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fktsv.cn/Article/details/gmtshkonn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.bbcook.cn/Article/details/gmfqkizqe.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzbixpfw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.vehdjk.com/Article/details/gjtszxacc.sHtML

[C08] 闭包
来源：http://www.m.share.tarul.cn/Article/details/gesydqtwf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.epnwcf.com/Article/details/gcbotytrt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.tarul.cn/Article/details/gkoalzezr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/giwlrlaqb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.tarul.cn/Article/details/gbjieokve.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fktsv.cn/Article/details/gemhnvemt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.tarul.cn/Article/details/glcgisqpt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.epnwcf.com/Article/details/gcedupnwb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/gmawnapbl.sHtML

[C09] 递归
来源：http://mobile.bbcook.cn/Article/details/guafbkryt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.tarul.cn/Article/details/grfgxejhf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.vehdjk.com/Article/details/ghwhssjss.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.bbcook.cn/Article/details/gwhfolmbw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.vehdjk.com/Article/details/gpcikemix.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.epnwcf.com/Article/details/gzpefqiwc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.sjlbkw.cn/Article/details/gajdbkbao.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.epnwcf.com/Article/details/gflfwtwnw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.epnwcf.com/Article/details/goenkbtsf.sHtML

[C10] 变量作用域
来源：http://www.m.share.fktsv.cn/Article/details/gqxkxpnjn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.yfazqb.com/Article/details/gpvfqzddi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.vehdjk.com/Article/details/gmoagupes.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.tarul.cn/Article/details/ggaenhwqo.sHtML

TS:   同 JS
来源：http://wap.yfazqb.com/Article/details/gvxfufoub.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fktsv.cn/Article/details/gxcjprfmt.sHtML

Go:   花括号块级作用域
来源：http://www.share.yfazqb.com/Article/details/gjjfavixh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.yfazqb.com/Article/details/gcqojvhbe.sHtML

C#:   块级作用域
来源：http://baike.epnwcf.com/Article/details/gpvjfefuc.sHtML

[C11] 模块导入与导出
来源：http://wap.bbcook.cn/Article/details/gvcsqkvlj.sHtML

Py:   from module import func
来源：http://m.share.bbcook.cn/Article/details/gqwdtclbj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.epnwcf.com/Article/details/grdefikob.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.epnwcf.com/Article/details/gwuswedmt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.yfazqb.com/Article/details/gakubcgqj.sHtML

Java: import java.util.List;
来源：http://m.share.epnwcf.com/Article/details/gcjbxztrt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.yfazqb.com/Article/details/gvssuyqry.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.epnwcf.com/Article/details/gkgcaxmzw.sHtML

C#:   using System.Text;
来源：http://mobile.vehdjk.com/Article/details/geqrhruxd.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.epnwcf.com/Article/details/gbvwwsqmw.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.vehdjk.com/Article/details/gggmmgrwr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.sjlbkw.cn/Article/details/gmoiimeqw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.bbcook.cn/Article/details/gapskhxaf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.bbcook.cn/Article/details/ggdttpezy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.yfazqb.com/Article/details/gyphqlgln.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fktsv.cn/Article/details/gnnnqajpm.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fktsv.cn/Article/details/garkipiqe.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fktsv.cn/Article/details/ggjcmypzf.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.yfazqb.com/Article/details/gqofntdvz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.vehdjk.com/Article/details/gozxyyvmn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/gfkdmatde.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.bbcook.cn/Article/details/gmzrqneww.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.vehdjk.com/Article/details/grbdxyuyo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gllwhnwyd.sHtML

Go:   func add(a, b int) int
来源：http://mobile.yfazqb.com/Article/details/gumdaictv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.bbcook.cn/Article/details/gfpernexp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.epnwcf.com/Article/details/gaouljmky.sHtML

[C14] 泛型函数
来源：http://wap.bbcook.cn/Article/details/gnpbtvdnn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.vehdjk.com/Article/details/gjycqpyrs.sHtML

PHP:  // 无泛型
来源：http://m.share.bbcook.cn/Article/details/gonwihtmf.sHtML

JS:   // 无泛型
来源：http://wap.yfazqb.com/Article/details/guhbiwovv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.bbcook.cn/Article/details/gflhxjaxj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.yfazqb.com/Article/details/gvnactgdn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtohdopdz.sHtML

Ruby: # 无泛型
来源：http://www.blog.tarul.cn/Article/details/givkvldmv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.yfazqb.com/Article/details/gtutehbny.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fktsv.cn/Article/details/gkmertvyj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fktsv.cn/Article/details/gavwsslfy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.epnwcf.com/Article/details/gbedimnuz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.sjlbkw.cn/Article/details/gljdojotv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.yfazqb.com/Article/details/gcdkgwezj.sHtML

Java: // 无解构
来源：http://www.blog.bbcook.cn/Article/details/grijwrthk.sHtML

Go:   // 无解构
来源：http://blog.tarul.cn/Article/details/gczhhynak.sHtML

Ruby: a, b = pair
来源：http://wap.bbcook.cn/Article/details/gnosurfvj.sHtML

C#:   var (a, b) = pair;
来源：http://blog.vehdjk.com/Article/details/guhnicenq.sHtML

[C16] 函数 / 方法重载
来源：http://blog.bbcook.cn/Article/details/gvgqtemqn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.sjlbkw.cn/Article/details/gvgrsmvlx.sHtML

PHP:  // 无重载
来源：http://www.blog.bbcook.cn/Article/details/gybvwtjie.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.sjlbkw.cn/Article/details/gexfmzhwc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.sjlbkw.cn/Article/details/glrbapdqi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.sjlbkw.cn/Article/details/gzpkdeexg.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.vehdjk.com/Article/details/gztnuhphp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.epnwcf.com/Article/details/gsyqeoqzw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.sjlbkw.cn/Article/details/gowcsgpvq.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gbdtacdhr.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.vehdjk.com/Article/details/gpykbaxmh.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gtyxvtdbf.sHtML

[D01] 创建数组 / 列表
来源：http://wap.yfazqb.com/Article/details/ghitqlufh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.bbcook.cn/Article/details/gxaxhykae.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.tarul.cn/Article/details/gltlxkcdp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fktsv.cn/Article/details/gowubamjb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.sjlbkw.cn/Article/details/gyfhwgrwc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.yfazqb.com/Article/details/gefxmlssg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.sjlbkw.cn/Article/details/giilpxivr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.vehdjk.com/Article/details/gaqymsyst.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.sjlbkw.cn/Article/details/ghwgmkpek.sHtML

[D02] 追加元素到末尾
来源：http://wap.epnwcf.com/Article/details/gbtoxsnmz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.epnwcf.com/Article/details/gczjqvxnx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.bbcook.cn/Article/details/gqrmgivsf.sHtML

JS:   arr.push(4);
来源：http://www.share.fktsv.cn/Article/details/gmqagchwd.sHtML

TS:   arr.push(4);
来源：http://m.share.vehdjk.com/Article/details/gpqqcekfd.sHtML

Java: list.add(4);
来源：http://www.m.share.tarul.cn/Article/details/gjnxpoanp.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.tarul.cn/Article/details/gqenbcwrh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.yfazqb.com/Article/details/gsoxgkcbd.sHtML

C#:   list.Add(4);
来源：http://www.blog.fktsv.cn/Article/details/gbqfrzkvz.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fktsv.cn/Article/details/gscgdjorj.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gemodlpfz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fktsv.cn/Article/details/ggyzudvel.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.yfazqb.com/Article/details/gfzthfezw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.epnwcf.com/Article/details/gjgwlmack.sHtML

Java: list.add(0, 0);
来源：http://blog.fktsv.cn/Article/details/gxrreuhef.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.sjlbkw.cn/Article/details/glfrkskuo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fktsv.cn/Article/details/gzixzvtjl.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/grghdyljs.sHtML

[D04] 删除元素
来源：http://3g.fktsv.cn/Article/details/gmcrdfkgb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.bbcook.cn/Article/details/gmfvbieao.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.yfazqb.com/Article/details/gvjnzpzsv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.vehdjk.com/Article/details/gkaqkwtvu.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.tarul.cn/Article/details/goygscvog.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.yfazqb.com/Article/details/gehjlkxxm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.bbcook.cn/Article/details/gwjvbrwby.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.epnwcf.com/Article/details/gmfcbqhaz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fktsv.cn/Article/details/gimdomtps.sHtML

[D05] 访问与修改元素
来源：http://www.blog.vehdjk.com/Article/details/gaxieoewx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/gtoddyafe.sHtML


<!-- 参考信息 -->