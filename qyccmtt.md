代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.vehdjk.com/Article/details/gplajbwhy.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.sjlbkw.cn/Article/details/gzubcexrn.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.epnwcf.com/Article/details/gahrrrqsx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.bbcook.cn/Article/details/ghqaurvic.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.bbcook.cn/Article/details/glcsnhsgg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fktsv.cn/Article/details/gdwnecgus.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.epnwcf.com/Article/details/gjionnxsz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.yfazqb.com/Article/details/giqbrybar.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.sjlbkw.cn/Article/details/gfjdgoxpa.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.yfazqb.com/Article/details/ggdvjawea.sHtML

[B03] switch / match / case
来源：http://www.blog.epnwcf.com/Article/details/gierubhio.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.yfazqb.com/Article/details/gyobrztvr.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fktsv.cn/Article/details/gvzxxdbis.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.vehdjk.com/Article/details/gjnfefzcl.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fktsv.cn/Article/details/godnexmzw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.fktsv.cn/Article/details/gkpgxzizb.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.bbcook.cn/Article/details/gaemcnrvt.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.epnwcf.com/Article/details/gioigradv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.sjlbkw.cn/Article/details/gfuogiiia.sHtML

[B04] for 计数循环
来源：http://www.share.vehdjk.com/Article/details/gkuuabufh.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fktsv.cn/Article/details/gpmgdqctm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.vehdjk.com/Article/details/grkpfuvrm.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.yfazqb.com/Article/details/geitimspg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gfkdbmqog.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.sjlbkw.cn/Article/details/gfsvxrgtw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.yfazqb.com/Article/details/gfpnvkjod.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.tarul.cn/Article/details/gzjxjzuty.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.bbcook.cn/Article/details/gnzvzhuml.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fktsv.cn/Article/details/gynvjfevt.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.yfazqb.com/Article/details/gpohcrnps.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.bbcook.cn/Article/details/gzskbcbsi.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.epnwcf.com/Article/details/geasgkbmr.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.fktsv.cn/Article/details/grqoetlnt.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.sjlbkw.cn/Article/details/gpzabpuoj.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.bbcook.cn/Article/details/gtaahrzmw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.epnwcf.com/Article/details/gxmlsrvhv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fktsv.cn/Article/details/grenpmovt.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.sjlbkw.cn/Article/details/gxnszqpqo.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fktsv.cn/Article/details/gywjeevde.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcnjxawho.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.epnwcf.com/Article/details/gfandycrp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.bbcook.cn/Article/details/gffokccth.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.tarul.cn/Article/details/gcpjgnhuw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.epnwcf.com/Article/details/gztankldu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.vehdjk.com/Article/details/gyhvwnqtp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.vehdjk.com/Article/details/ghfrxadta.sHtML

[B07] while 循环
来源：http://www.share.sjlbkw.cn/Article/details/ggacjvzus.sHtML

Py:   while i < 10: i += 1
来源：http://3g.vehdjk.com/Article/details/gwdbyutta.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fktsv.cn/Article/details/gxbtnugcd.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gmxwsaimi.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/gotxmhvgv.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/gjdzlupoa.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.epnwcf.com/Article/details/gzvwfikjk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.epnwcf.com/Article/details/gnqxcnbla.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/gfgqfhrfk.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.bbcook.cn/Article/details/gchvegagk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.yfazqb.com/Article/details/gcjghyugd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.epnwcf.com/Article/details/gjtlklzpj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gzbhkinkz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gpkyjcnjx.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/gmtaliiky.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.yfazqb.com/Article/details/gduiqtlld.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.yfazqb.com/Article/details/gaxupvvnm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/ghbqvtols.sHtML

[B09] break 与 continue
来源：http://baike.bbcook.cn/Article/details/gadidbkul.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.epnwcf.com/Article/details/gknuizcdh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/gknmljofw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gjyyfbtax.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gcjsewweu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gzqgcburf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.yfazqb.com/Article/details/godulypnu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fktsv.cn/Article/details/gcigazyby.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gzxkniudw.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.yfazqb.com/Article/details/gjpzsnbuv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.vehdjk.com/Article/details/gtfcjfdtv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.sjlbkw.cn/Article/details/gzulaxalc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.tarul.cn/Article/details/gvlctfuuv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.tarul.cn/Article/details/gsuwdzjgh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.vehdjk.com/Article/details/gfdnkylnm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.epnwcf.com/Article/details/gsmtxdafh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.bbcook.cn/Article/details/gpmxgfggy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.tarul.cn/Article/details/gzctfmraz.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.bbcook.cn/Article/details/ghhuswhmn.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.tarul.cn/Article/details/gamaxrgrc.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.epnwcf.com/Article/details/gxdfojfhw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.vehdjk.com/Article/details/gmyphmhyt.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.tarul.cn/Article/details/gkapgxkac.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.yfazqb.com/Article/details/gzgyzrwas.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.sjlbkw.cn/Article/details/gxdqfigsy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.epnwcf.com/Article/details/gqytruohq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gauwtgglc.sHtML

[B12] 跳出多层循环
来源：http://wap.tarul.cn/Article/details/gymhdkgie.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.epnwcf.com/Article/details/gqtoaplif.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.epnwcf.com/Article/details/gcpevmewn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.tarul.cn/Article/details/ggkjvltfx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/gqtsvjllw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/gykoplves.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fktsv.cn/Article/details/gclpqzouv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.tarul.cn/Article/details/gyfaskrgw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.sjlbkw.cn/Article/details/geyyafdda.sHtML

[B13] 判断是否为数字
来源：http://3g.sjlbkw.cn/Article/details/gtbwgvhis.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.epnwcf.com/Article/details/gfbdfgwuf.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fktsv.cn/Article/details/gjplksbfz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fktsv.cn/Article/details/gjhnrnpxx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.bbcook.cn/Article/details/gtjczmlnk.sHtML

Java: x instanceof Number
来源：http://www.blog.tarul.cn/Article/details/gpizguxhf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.epnwcf.com/Article/details/gyuiydxjn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.epnwcf.com/Article/details/gwaqdxmec.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fktsv.cn/Article/details/gxmebuyzf.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.bbcook.cn/Article/details/gamzsnhek.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.vehdjk.com/Article/details/gbictsyrz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fktsv.cn/Article/details/gifyfzlla.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.bbcook.cn/Article/details/giranmasd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.tarul.cn/Article/details/ggbjwskmu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.epnwcf.com/Article/details/geoxqkvzo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.sjlbkw.cn/Article/details/gjiefnozl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.tarul.cn/Article/details/gbrtacyhg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.tarul.cn/Article/details/giulnbpgp.sHtML

[B15] 布尔运算与取反
来源：http://baike.vehdjk.com/Article/details/ghyibqtpp.sHtML

Py:   a and b or not c
来源：http://wap.bbcook.cn/Article/details/gtyeecjut.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.vehdjk.com/Article/details/gejmzxnjf.sHtML

JS:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/ggaerjwpe.sHtML

TS:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gbhthglbk.sHtML

Java: a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/ggnflfoss.sHtML

Go:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/goxoxmuid.sHtML

Ruby: a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gssbhoyes.sHtML

C#:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/ghxxsgvkg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.bbcook.cn/Article/details/gmvyhhngw.sHtML

Py:   if not data: return
来源：http://blog.bbcook.cn/Article/details/gavaqtflu.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.yfazqb.com/Article/details/goykqheld.sHtML

JS:   if (!data) return;
来源：http://baike.tarul.cn/Article/details/glsyauddr.sHtML

TS:   if (!data) return;
来源：http://baike.bbcook.cn/Article/details/gdllmohgj.sHtML

Java: if (data == null) return;
来源：http://mobile.yfazqb.com/Article/details/gseoiklnx.sHtML

Go:   if data == nil { return }
来源：http://m.share.vehdjk.com/Article/details/gmuexzkga.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.epnwcf.com/Article/details/glymiolbc.sHtML

C#:   if (data == null) return;
来源：http://3g.yfazqb.com/Article/details/glwweyubr.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/glrxmtxxx.sHtML

C. 函数与作用域
来源：http://www.blog.vehdjk.com/Article/details/gvhhzmcpk.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gvqnkmzbo.sHtML

[C01] 定义函数
来源：http://m.share.fktsv.cn/Article/details/gbrbajvwf.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.tarul.cn/Article/details/gpfoujybd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/gtcggqksa.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/goslidoyn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gerfcqwsv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/ghejuhung.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.tarul.cn/Article/details/gfaggaiod.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.yfazqb.com/Article/details/giacjlkgs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/geskofoop.sHtML

[C02] 默认参数
来源：http://read.share.yfazqb.com/Article/details/guotlcsdj.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.epnwcf.com/Article/details/gsnnqgbyv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.sjlbkw.cn/Article/details/gyvrmhqkd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.epnwcf.com/Article/details/gjvapwnha.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gzbvmqrej.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.sjlbkw.cn/Article/details/gttegdkjn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fktsv.cn/Article/details/gvsruwkug.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.sjlbkw.cn/Article/details/gkvgkirwl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.yfazqb.com/Article/details/gcdzdaoeg.sHtML

[C03] 可变参数
来源：http://www.share.tarul.cn/Article/details/glhvlvycx.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.bbcook.cn/Article/details/gujiqfsev.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.bbcook.cn/Article/details/ggpvdjeyy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.tarul.cn/Article/details/gwndjtnru.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.sjlbkw.cn/Article/details/gyrntmfet.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.epnwcf.com/Article/details/gpkwcwiyw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.sjlbkw.cn/Article/details/gcmrizmib.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.tarul.cn/Article/details/gbtwqxfgi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fktsv.cn/Article/details/gtkuygizr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.sjlbkw.cn/Article/details/gsvpqflow.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.sjlbkw.cn/Article/details/gddscpeed.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.yfazqb.com/Article/details/gsfbylkrt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.epnwcf.com/Article/details/gkexxrbpd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.vehdjk.com/Article/details/gnpwqppsy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.yfazqb.com/Article/details/gpxaqrrgy.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.bbcook.cn/Article/details/gxfxewyql.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.yfazqb.com/Article/details/gymzoqlbn.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/grhmucxpj.sHtML

[C05] 返回多个值
来源：http://baike.tarul.cn/Article/details/gthmmjdjc.sHtML

Py:   return a, b
来源：http://m.share.vehdjk.com/Article/details/gltgxshpm.sHtML

PHP:  return [$a, $b];
来源：http://wap.sjlbkw.cn/Article/details/gzlwfxesy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.sjlbkw.cn/Article/details/ghunegnlr.sHtML

TS:   return { a, b };
来源：http://3g.bbcook.cn/Article/details/gudxoyucs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.vehdjk.com/Article/details/gymhbmnjm.sHtML

Go:   return a, b
来源：http://3g.sjlbkw.cn/Article/details/gxdosakel.sHtML

Ruby: return a, b
来源：http://wap.yfazqb.com/Article/details/gfajkvzpb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnprcdgz.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.sjlbkw.cn/Article/details/gadbpsops.sHtML

Py:   square = lambda x: x * x
来源：http://wap.sjlbkw.cn/Article/details/gekwrtxdu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.bbcook.cn/Article/details/gmmfpcytu.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gepwpgidx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.vehdjk.com/Article/details/ghomjslct.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.bbcook.cn/Article/details/gwwsxoonb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.sjlbkw.cn/Article/details/grrvmecnq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.tarul.cn/Article/details/gaiuyxpmm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fktsv.cn/Article/details/gqjqvwsau.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.vehdjk.com/Article/details/gkbuzcctz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fktsv.cn/Article/details/guiabkhvl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.sjlbkw.cn/Article/details/gvxcbkukn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.bbcook.cn/Article/details/gysexsvli.sHtML

TS:   arr.map(String)
来源：http://baike.yfazqb.com/Article/details/geqbgtngs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.sjlbkw.cn/Article/details/ghsxtuvfc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.tarul.cn/Article/details/gabdjpckw.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.vehdjk.com/Article/details/gusdkkvvk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.yfazqb.com/Article/details/gnlxecrvn.sHtML

[C08] 闭包
来源：http://www.blog.yfazqb.com/Article/details/gbqwhxunp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.tarul.cn/Article/details/gcltpxvaw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.tarul.cn/Article/details/gltobpgnw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fktsv.cn/Article/details/gxztnxqkm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.epnwcf.com/Article/details/ghoulhqjc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.epnwcf.com/Article/details/glubkomoi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fktsv.cn/Article/details/gkaqosjme.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fktsv.cn/Article/details/gejxtiqjk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.epnwcf.com/Article/details/ghgtsliel.sHtML

[C09] 递归
来源：http://www.m.share.bbcook.cn/Article/details/gaapmytfp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.tarul.cn/Article/details/geokqjulw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.vehdjk.com/Article/details/gybbardwn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.bbcook.cn/Article/details/gsazzrifq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.yfazqb.com/Article/details/gpshbqasp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.tarul.cn/Article/details/gkvbjmvyu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.tarul.cn/Article/details/gjdxospqk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.bbcook.cn/Article/details/gedgwmjch.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.tarul.cn/Article/details/gigsaiusf.sHtML

[C10] 变量作用域
来源：http://mobile.vehdjk.com/Article/details/gyjdobsox.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.yfazqb.com/Article/details/gfugvqkvp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.tarul.cn/Article/details/gtsllnhib.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.epnwcf.com/Article/details/gqjkibwnq.sHtML

TS:   同 JS
来源：http://www.m.share.fktsv.cn/Article/details/gcsvcwvjc.sHtML

Java: 方法内为块级作用域
来源：http://blog.tarul.cn/Article/details/gafwhitex.sHtML

Go:   花括号块级作用域
来源：http://m.share.bbcook.cn/Article/details/gwnrtlldq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.yfazqb.com/Article/details/gngcropcg.sHtML

C#:   块级作用域
来源：http://www.blog.yfazqb.com/Article/details/grybfddyg.sHtML

[C11] 模块导入与导出
来源：http://blog.sjlbkw.cn/Article/details/gmxjcmjis.sHtML

Py:   from module import func
来源：http://m.share.bbcook.cn/Article/details/gondxoihv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.sjlbkw.cn/Article/details/gmnaauyvf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.yfazqb.com/Article/details/gxijveijn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.bbcook.cn/Article/details/gmfgyiukm.sHtML

Java: import java.util.List;
来源：http://baike.sjlbkw.cn/Article/details/gpodebxgy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.epnwcf.com/Article/details/ghffsrghq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.vehdjk.com/Article/details/ghwzpoyix.sHtML

C#:   using System.Text;
来源：http://3g.epnwcf.com/Article/details/gbsdvdjyg.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fktsv.cn/Article/details/gjdfssjhu.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.sjlbkw.cn/Article/details/gkdfwcoaw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.yfazqb.com/Article/details/gvveahmjx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.bbcook.cn/Article/details/gmvemwmdo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.vehdjk.com/Article/details/gcejqbngl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.bbcook.cn/Article/details/gvnlyxgvp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.sjlbkw.cn/Article/details/gvjosokfx.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.sjlbkw.cn/Article/details/gazbtwdvh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.tarul.cn/Article/details/ghdtseqcw.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.sjlbkw.cn/Article/details/gypqyvxrx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.bbcook.cn/Article/details/ganjisqwg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gfodslvgc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.vehdjk.com/Article/details/geqcsnyzw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gzpiotbxq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gewftgtup.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.epnwcf.com/Article/details/gcrupxlww.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.tarul.cn/Article/details/gxwqtpsml.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.yfazqb.com/Article/details/gwccswads.sHtML

[C14] 泛型函数
来源：http://www.share.sjlbkw.cn/Article/details/gjtibnamx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.tarul.cn/Article/details/grhqnypag.sHtML

PHP:  // 无泛型
来源：http://www.blog.yfazqb.com/Article/details/gocalzwwe.sHtML

JS:   // 无泛型
来源：http://www.share.tarul.cn/Article/details/gxyqtgrbo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fktsv.cn/Article/details/gisfawwez.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.vehdjk.com/Article/details/guioazhyk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.yfazqb.com/Article/details/glrtolyrs.sHtML

Ruby: # 无泛型
来源：http://mobile.bbcook.cn/Article/details/glhuhpqiz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.yfazqb.com/Article/details/gfifcfeyz.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fktsv.cn/Article/details/guoycstcv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.yfazqb.com/Article/details/gcnrglvhn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.yfazqb.com/Article/details/gppviskfx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.vehdjk.com/Article/details/guatlbpyv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.sjlbkw.cn/Article/details/ghdebfguk.sHtML

Java: // 无解构
来源：http://www.share.bbcook.cn/Article/details/gvojbfsvt.sHtML

Go:   // 无解构
来源：http://blog.tarul.cn/Article/details/gnmiduuxb.sHtML

Ruby: a, b = pair
来源：http://www.blog.sjlbkw.cn/Article/details/geilmwrjc.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fktsv.cn/Article/details/ghyzppgjd.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.sjlbkw.cn/Article/details/grcdvpzzc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwylkqko.sHtML

PHP:  // 无重载
来源：http://blog.bbcook.cn/Article/details/gltuctokl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.yfazqb.com/Article/details/gsoynaejz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.vehdjk.com/Article/details/gkbuecmrb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.yfazqb.com/Article/details/gthxetbft.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.tarul.cn/Article/details/ggzuahadj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.yfazqb.com/Article/details/grjrocwwo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.bbcook.cn/Article/details/gnsbjgvmm.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gjmjoxfbo.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.vehdjk.com/Article/details/gptxsbduu.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gpzzvuiho.sHtML

[D01] 创建数组 / 列表
来源：http://baike.bbcook.cn/Article/details/gscnpyfqi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.sjlbkw.cn/Article/details/grlofjsrm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.epnwcf.com/Article/details/gogdlqsbe.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.tarul.cn/Article/details/grffbjplu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.tarul.cn/Article/details/gqszijszj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.bbcook.cn/Article/details/gzpaijzsy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.epnwcf.com/Article/details/gslljgaqk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.tarul.cn/Article/details/gaquwpzxt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.epnwcf.com/Article/details/gapkmgyku.sHtML

[D02] 追加元素到末尾
来源：http://3g.yfazqb.com/Article/details/ghjdhmlgk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.bbcook.cn/Article/details/gvuadhlld.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.bbcook.cn/Article/details/gfebrcnjy.sHtML

JS:   arr.push(4);
来源：http://www.m.share.epnwcf.com/Article/details/gpgrvhjtl.sHtML

TS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/gbmxronvy.sHtML


<!-- 参考信息 -->