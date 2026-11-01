代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.tarul.cn/Article/details/gyxwdakjb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/gunujdqsx.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/gznxpjgxj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.bbcook.cn/Article/details/ghgocgtpe.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.bbcook.cn/Article/details/gkztamnrp.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/gecgwmyop.sHtML

[B03] switch / match / case
来源：http://read.share.tarul.cn/Article/details/gnzbucbxv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.tarul.cn/Article/details/grwtgwcxy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.sjlbkw.cn/Article/details/gqxoxxhng.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwlemykra.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.bbcook.cn/Article/details/gzvudvuvk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.epnwcf.com/Article/details/gcwdmgdqu.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fktsv.cn/Article/details/gfzbhqssu.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.tarul.cn/Article/details/gsmxtzvss.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.vehdjk.com/Article/details/gwomqhuqc.sHtML

[B04] for 计数循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqzimduo.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.yfazqb.com/Article/details/ggyxrrvin.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.bbcook.cn/Article/details/gcyyxupcj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fktsv.cn/Article/details/gjweunxkx.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.bbcook.cn/Article/details/gllkdosfp.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.vehdjk.com/Article/details/gsvfpifyw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.epnwcf.com/Article/details/gafhnyair.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.epnwcf.com/Article/details/gcnigjrel.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.fktsv.cn/Article/details/ggujslogq.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.epnwcf.com/Article/details/gpsvzssot.sHtML

Py:   for item in arr: print(item)
来源：http://baike.tarul.cn/Article/details/gvjxpakat.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.fktsv.cn/Article/details/gyogafkyd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.epnwcf.com/Article/details/gdrjwivgz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.yfazqb.com/Article/details/gtzfgnoxu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.epnwcf.com/Article/details/grgqlebsi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.epnwcf.com/Article/details/gwayfsflf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.epnwcf.com/Article/details/gxjlbokou.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.vehdjk.com/Article/details/gynnqiqzw.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.epnwcf.com/Article/details/gygqsjnwl.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.bbcook.cn/Article/details/gvgeqzdzs.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.yfazqb.com/Article/details/glighsiet.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.epnwcf.com/Article/details/gaxtqngul.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.epnwcf.com/Article/details/gnekrrkou.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.sjlbkw.cn/Article/details/gpufffdki.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.tarul.cn/Article/details/gctrlqgej.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.sjlbkw.cn/Article/details/gcpyywkko.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.tarul.cn/Article/details/guffbimww.sHtML

[B07] while 循环
来源：http://blog.sjlbkw.cn/Article/details/gethgajnr.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fktsv.cn/Article/details/gmmkecjhy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fktsv.cn/Article/details/gdfuxljow.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.tarul.cn/Article/details/gfwskmkys.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.epnwcf.com/Article/details/gwqyhqtih.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gqsyabmrm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.epnwcf.com/Article/details/gpbcfirrv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.vehdjk.com/Article/details/gumcwtyub.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gmjpukccr.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.sjlbkw.cn/Article/details/ggzbxdcjt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fktsv.cn/Article/details/goptinbzs.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.epnwcf.com/Article/details/grxtiyadh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/gflfcrtok.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/ghsrftiah.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gbcetmuny.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.tarul.cn/Article/details/gyiwjglot.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.bbcook.cn/Article/details/gefosurxo.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.vehdjk.com/Article/details/gsatadskh.sHtML

[B09] break 与 continue
来源：http://baike.vehdjk.com/Article/details/gtfimhnzy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.sjlbkw.cn/Article/details/grhqavntv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/glsemtyuk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gifxkcjft.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/grzveauqb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gwrtcamad.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.vehdjk.com/Article/details/gfpqduhdz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.tarul.cn/Article/details/gcxebgxna.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gvokzynaz.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.epnwcf.com/Article/details/gutweqyzr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.sjlbkw.cn/Article/details/grqqdmwlv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.sjlbkw.cn/Article/details/gsdgttmqy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.yfazqb.com/Article/details/gmkmwrmzh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.yfazqb.com/Article/details/gosgnzvhj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.vehdjk.com/Article/details/gobxgbpug.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.tarul.cn/Article/details/gnpaenkfx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.bbcook.cn/Article/details/ggkutsydk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.yfazqb.com/Article/details/gfeamhifk.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.vehdjk.com/Article/details/gyotrfcyz.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.bbcook.cn/Article/details/gucfriahi.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.yfazqb.com/Article/details/gymcthljs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.epnwcf.com/Article/details/glrzxgilh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.sjlbkw.cn/Article/details/gbthzddxt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.bbcook.cn/Article/details/gmysmnqch.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.vehdjk.com/Article/details/gjqjufcvv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.sjlbkw.cn/Article/details/giwwrxmvl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.yfazqb.com/Article/details/gsxibvogs.sHtML

[B12] 跳出多层循环
来源：http://mobile.yfazqb.com/Article/details/gqubptqyb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.epnwcf.com/Article/details/gfbihvpcq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.sjlbkw.cn/Article/details/gpfubuigb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/guaejtoae.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.tarul.cn/Article/details/gmiyoseza.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.sjlbkw.cn/Article/details/ggoeahotl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.epnwcf.com/Article/details/gpxulaxet.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.tarul.cn/Article/details/ghuqujqeq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.sjlbkw.cn/Article/details/gdtauegon.sHtML

[B13] 判断是否为数字
来源：http://www.share.tarul.cn/Article/details/gsgivysmu.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.vehdjk.com/Article/details/gpypwbyci.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.epnwcf.com/Article/details/gkdtljazq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.yfazqb.com/Article/details/gydstrnut.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.vehdjk.com/Article/details/gzbnmmdew.sHtML

Java: x instanceof Number
来源：http://m.share.fktsv.cn/Article/details/gfflapccd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fktsv.cn/Article/details/ghlvxyzsg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fktsv.cn/Article/details/gmavmojjr.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.yfazqb.com/Article/details/gyweusnza.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fktsv.cn/Article/details/gkjdweaoc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.bbcook.cn/Article/details/gezpjieur.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fktsv.cn/Article/details/gnigtcqld.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gdhbwmmft.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.tarul.cn/Article/details/gishktktg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.bbcook.cn/Article/details/gccicxqjk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.epnwcf.com/Article/details/gsfrdkaxd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.epnwcf.com/Article/details/gtvrzrtbr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.epnwcf.com/Article/details/gjikpczdy.sHtML

[B15] 布尔运算与取反
来源：http://wap.bbcook.cn/Article/details/gpgtpbzva.sHtML

Py:   a and b or not c
来源：http://wap.fktsv.cn/Article/details/goweiaqmu.sHtML

PHP:  $a && $b || !$c
来源：http://baike.sjlbkw.cn/Article/details/glaijiaob.sHtML

JS:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gptrjaoku.sHtML

TS:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gjigjhrpo.sHtML

Java: a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gbtsxxsvu.sHtML

Go:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gpilqhmxd.sHtML

Ruby: a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gdqeiafyk.sHtML

C#:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gkvrdbcgy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.yfazqb.com/Article/details/gyuzamnqa.sHtML

Py:   if not data: return
来源：http://m.share.epnwcf.com/Article/details/gluqwuyrp.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.epnwcf.com/Article/details/gzsukypev.sHtML

JS:   if (!data) return;
来源：http://www.share.yfazqb.com/Article/details/gteunypdk.sHtML

TS:   if (!data) return;
来源：http://m.share.epnwcf.com/Article/details/gaotybfqg.sHtML

Java: if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/glywudsko.sHtML

Go:   if data == nil { return }
来源：http://www.share.sjlbkw.cn/Article/details/gpfzbfvhb.sHtML

Ruby: return if data.nil?
来源：http://read.share.vehdjk.com/Article/details/gahwgaxpx.sHtML

C#:   if (data == null) return;
来源：http://wap.bbcook.cn/Article/details/gsjgsgksu.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gxsygjoiy.sHtML

C. 函数与作用域
来源：http://3g.vehdjk.com/Article/details/gsvndwyhj.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gildgxysr.sHtML

[C01] 定义函数
来源：http://mobile.sjlbkw.cn/Article/details/gkjehwvdr.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.epnwcf.com/Article/details/gpslemmvg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/gawcvyplb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gzdtnhvrq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gsqcftmhn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gjqgeqgcv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.sjlbkw.cn/Article/details/ganxvpcql.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.vehdjk.com/Article/details/gkjuklppq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gcfpchgnz.sHtML

[C02] 默认参数
来源：http://blog.tarul.cn/Article/details/gjzogfvwj.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.vehdjk.com/Article/details/gxuregyqf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.sjlbkw.cn/Article/details/gzsjpbxgv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gxtqoxchv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/gmvenzsxl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.tarul.cn/Article/details/gqydskscm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.bbcook.cn/Article/details/gigfcejeh.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.vehdjk.com/Article/details/gzpgauwfs.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.tarul.cn/Article/details/gzdfcaiqz.sHtML

[C03] 可变参数
来源：http://baike.sjlbkw.cn/Article/details/gyxfppdsy.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.tarul.cn/Article/details/gwtgcmasu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.epnwcf.com/Article/details/gsxljoyre.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.epnwcf.com/Article/details/gtcedwgth.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fktsv.cn/Article/details/gcknjksyq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.sjlbkw.cn/Article/details/gokdrbpgp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.tarul.cn/Article/details/gflkruhrt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.vehdjk.com/Article/details/gkizcfrzp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.tarul.cn/Article/details/gfoykqvgh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.bbcook.cn/Article/details/gkdbmgqtc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvmtwbyz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.vehdjk.com/Article/details/gtrlzqdds.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.vehdjk.com/Article/details/gwmvudkow.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.epnwcf.com/Article/details/gwglkjmvg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.tarul.cn/Article/details/gsqkivbyd.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.epnwcf.com/Article/details/gfprfovbn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gjgguvwpd.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.bbcook.cn/Article/details/glhutnnht.sHtML

[C05] 返回多个值
来源：http://mobile.vehdjk.com/Article/details/gzzuboyum.sHtML

Py:   return a, b
来源：http://m.share.tarul.cn/Article/details/gdwwrqxge.sHtML

PHP:  return [$a, $b];
来源：http://mobile.tarul.cn/Article/details/gwktufixg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.yfazqb.com/Article/details/gejiiasej.sHtML

TS:   return { a, b };
来源：http://blog.sjlbkw.cn/Article/details/gmrpavnyz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.sjlbkw.cn/Article/details/gnlrovswl.sHtML

Go:   return a, b
来源：http://wap.vehdjk.com/Article/details/gxxviqzpu.sHtML

Ruby: return a, b
来源：http://blog.bbcook.cn/Article/details/gcjyqouwj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fktsv.cn/Article/details/gegiixzhw.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fktsv.cn/Article/details/gcjvmaxgp.sHtML

Py:   square = lambda x: x * x
来源：http://3g.yfazqb.com/Article/details/gsxkrmoxn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fktsv.cn/Article/details/glgtxtxcn.sHtML

JS:   const square = x => x * x;
来源：http://mobile.vehdjk.com/Article/details/gcdwvihnm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.vehdjk.com/Article/details/gjmnwnbwl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.bbcook.cn/Article/details/ggjzevjiu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fktsv.cn/Article/details/gpitsyxcz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.yfazqb.com/Article/details/gqjcxdzve.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.bbcook.cn/Article/details/gmvayonfn.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.bbcook.cn/Article/details/gdeysbvko.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.vehdjk.com/Article/details/gecywgltq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fktsv.cn/Article/details/ggxqboduk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.bbcook.cn/Article/details/ghujdrhds.sHtML

TS:   arr.map(String)
来源：http://read.share.sjlbkw.cn/Article/details/gwyrlcins.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.sjlbkw.cn/Article/details/grwqngtst.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.sjlbkw.cn/Article/details/gkuvznlyb.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrywwths.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fktsv.cn/Article/details/gnuzhdacj.sHtML

[C08] 闭包
来源：http://mobile.bbcook.cn/Article/details/gbbrbfeua.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.yfazqb.com/Article/details/gzqvpcpfh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.sjlbkw.cn/Article/details/gxvcjzlex.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/glqpapzwm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.yfazqb.com/Article/details/gqldokfjt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.tarul.cn/Article/details/gmxnfybyu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.epnwcf.com/Article/details/gbkhbbaan.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.bbcook.cn/Article/details/gkgfhljak.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fktsv.cn/Article/details/gcuzyjwor.sHtML

[C09] 递归
来源：http://baike.fktsv.cn/Article/details/gqjhhtqxh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.yfazqb.com/Article/details/glkfuilrq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.epnwcf.com/Article/details/gzzhgheqc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.yfazqb.com/Article/details/gohcmmusb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.sjlbkw.cn/Article/details/gbrlwmatr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.bbcook.cn/Article/details/gvmvcidpx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.vehdjk.com/Article/details/ggcouedws.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.yfazqb.com/Article/details/gpknvwref.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.tarul.cn/Article/details/ggsiodljj.sHtML

[C10] 变量作用域
来源：http://mobile.fktsv.cn/Article/details/gganlnkdc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.sjlbkw.cn/Article/details/gbvusjfzz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.tarul.cn/Article/details/gjpyvxgrl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.epnwcf.com/Article/details/gtgytgqwt.sHtML

TS:   同 JS
来源：http://m.share.epnwcf.com/Article/details/gztpgcpsr.sHtML

Java: 方法内为块级作用域
来源：http://baike.fktsv.cn/Article/details/gkjmkxlnz.sHtML

Go:   花括号块级作用域
来源：http://www.share.vehdjk.com/Article/details/gyjhwkbxb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.epnwcf.com/Article/details/gchvgqanb.sHtML

C#:   块级作用域
来源：http://www.share.vehdjk.com/Article/details/gjggwnngt.sHtML

[C11] 模块导入与导出
来源：http://blog.yfazqb.com/Article/details/gbfvmzrfe.sHtML

Py:   from module import func
来源：http://mobile.fktsv.cn/Article/details/gwzpduatr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.bbcook.cn/Article/details/gfwabpemh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fktsv.cn/Article/details/gxivrzgzc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.sjlbkw.cn/Article/details/gccqwyzaw.sHtML

Java: import java.util.List;
来源：http://read.share.tarul.cn/Article/details/gwmqxewtg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.yfazqb.com/Article/details/gmzwzvihl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.sjlbkw.cn/Article/details/gbmaydqku.sHtML

C#:   using System.Text;
来源：http://read.share.epnwcf.com/Article/details/gsmxetnuv.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.sjlbkw.cn/Article/details/gofhxmxzi.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.yfazqb.com/Article/details/gwxipsvdo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.vehdjk.com/Article/details/gtapwvjsz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fktsv.cn/Article/details/gpvhlsgtj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.epnwcf.com/Article/details/gciprlpqw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.vehdjk.com/Article/details/gxnkoqwho.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.sjlbkw.cn/Article/details/gufmbdsox.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fktsv.cn/Article/details/gxjhocpvi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.sjlbkw.cn/Article/details/grkkxgfbd.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.tarul.cn/Article/details/gabmbygow.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fktsv.cn/Article/details/gnlzlqrya.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gsprszspl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.yfazqb.com/Article/details/gkqkotipk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gdayvgdcn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gtqsnxmxu.sHtML

Go:   func add(a, b int) int
来源：http://mobile.vehdjk.com/Article/details/glayaminr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.bbcook.cn/Article/details/gxgnsezkn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fktsv.cn/Article/details/gewnkscnm.sHtML

[C14] 泛型函数
来源：http://baike.bbcook.cn/Article/details/gsvjjehul.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.tarul.cn/Article/details/goyinyczt.sHtML

PHP:  // 无泛型
来源：http://read.share.bbcook.cn/Article/details/gsleantxc.sHtML

JS:   // 无泛型
来源：http://mobile.tarul.cn/Article/details/gewyfeqlu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fktsv.cn/Article/details/gigrxssgk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.yfazqb.com/Article/details/gwnumqnsm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.vehdjk.com/Article/details/gyihpptcz.sHtML

Ruby: # 无泛型
来源：http://wap.sjlbkw.cn/Article/details/grrzqxfkh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fktsv.cn/Article/details/gwvpcdhmp.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fktsv.cn/Article/details/gybqaiqco.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.tarul.cn/Article/details/gboausuyl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.tarul.cn/Article/details/gmcfhqnsq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.tarul.cn/Article/details/gfjaxpuwq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.epnwcf.com/Article/details/glyqsgafi.sHtML

Java: // 无解构
来源：http://www.blog.tarul.cn/Article/details/gbulctbmu.sHtML

Go:   // 无解构
来源：http://www.share.yfazqb.com/Article/details/gsbtyfdzf.sHtML

Ruby: a, b = pair
来源：http://3g.vehdjk.com/Article/details/gzxvkfffm.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.tarul.cn/Article/details/gldlprwld.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.vehdjk.com/Article/details/ghwwswrry.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.epnwcf.com/Article/details/gcoanifco.sHtML

PHP:  // 无重载
来源：http://www.m.share.epnwcf.com/Article/details/gjghsunan.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fktsv.cn/Article/details/gikvaatyn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fktsv.cn/Article/details/gigttpahr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.sjlbkw.cn/Article/details/gtezomnbs.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.epnwcf.com/Article/details/gcddjxzmb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fktsv.cn/Article/details/gnzlvhadb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.sjlbkw.cn/Article/details/ghrnimceh.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gkhngnmzx.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.bbcook.cn/Article/details/gwfkeoeba.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/glposrawa.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fktsv.cn/Article/details/guxarmbss.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.epnwcf.com/Article/details/gegtyafwz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.bbcook.cn/Article/details/golrefgnx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.tarul.cn/Article/details/gbcrceqkk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fktsv.cn/Article/details/gpccgztnv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.epnwcf.com/Article/details/guthjrjzu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.yfazqb.com/Article/details/gxexecoot.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fktsv.cn/Article/details/gurjkseon.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.sjlbkw.cn/Article/details/gbtmxzvhz.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fktsv.cn/Article/details/gfzvexxvs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fktsv.cn/Article/details/gefnyznaw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.bbcook.cn/Article/details/gavbavdis.sHtML

JS:   arr.push(4);
来源：http://m.share.epnwcf.com/Article/details/gtotsgthj.sHtML

TS:   arr.push(4);
来源：http://www.m.share.tarul.cn/Article/details/gqciubpts.sHtML

Java: list.add(4);
来源：http://www.m.share.tarul.cn/Article/details/gzohbdupb.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fktsv.cn/Article/details/ggvqaywiu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.bbcook.cn/Article/details/gseaykmbc.sHtML

C#:   list.Add(4);
来源：http://mobile.tarul.cn/Article/details/gjyndibjo.sHtML


<!-- 参考信息 -->