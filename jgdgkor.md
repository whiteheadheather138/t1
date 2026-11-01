代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/gcyrjbdea.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.bbcook.cn/Article/details/gshplqlil.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.yfazqb.com/Article/details/gfthxwjsa.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.vehdjk.com/Article/details/gjiizohmc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.tarul.cn/Article/details/ghpzjnlts.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gvwpdkrbb.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.yfazqb.com/Article/details/gvibtlkia.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.sjlbkw.cn/Article/details/gtczcpewm.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.epnwcf.com/Article/details/gvydttnvy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/glmgfbjre.sHtML

[B03] switch / match / case
来源：http://m.share.yfazqb.com/Article/details/gvxtwalyf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.bbcook.cn/Article/details/gdovobzho.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/grybcaiva.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.epnwcf.com/Article/details/gcnbaatqa.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.vehdjk.com/Article/details/gseyrthpw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.vehdjk.com/Article/details/gnkgenoqm.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.yfazqb.com/Article/details/gokeqysgz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.bbcook.cn/Article/details/gmfzxiszo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.vehdjk.com/Article/details/gzordqbng.sHtML

[B04] for 计数循环
来源：http://wap.sjlbkw.cn/Article/details/gqzpdtjpb.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.fktsv.cn/Article/details/gbhbxtwib.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.vehdjk.com/Article/details/gyvphplak.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.bbcook.cn/Article/details/goszswnie.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fktsv.cn/Article/details/gkkwmjnph.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.epnwcf.com/Article/details/gjbrjlaqv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.fktsv.cn/Article/details/ggvtgrxoc.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.bbcook.cn/Article/details/gbjfmydoe.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.epnwcf.com/Article/details/gdvlvscwj.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.vehdjk.com/Article/details/ghnhjqghg.sHtML

Py:   for item in arr: print(item)
来源：http://3g.sjlbkw.cn/Article/details/gntqzolql.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.bbcook.cn/Article/details/gtpomdgqd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.sjlbkw.cn/Article/details/gnjyonnhd.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.sjlbkw.cn/Article/details/gubggzjkv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fktsv.cn/Article/details/gmgfimnin.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.yfazqb.com/Article/details/gdhvroimk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fktsv.cn/Article/details/gglhsnaim.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.tarul.cn/Article/details/gywfkqoql.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.tarul.cn/Article/details/gwaqpelgg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.yfazqb.com/Article/details/gcatoqavv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.epnwcf.com/Article/details/gubmyhulb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.vehdjk.com/Article/details/gczshvpah.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.bbcook.cn/Article/details/grtbdqmgg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.vehdjk.com/Article/details/gtzatdehv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.epnwcf.com/Article/details/guzqtjyyb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.sjlbkw.cn/Article/details/gusabnesh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.sjlbkw.cn/Article/details/gvwqirroz.sHtML

[B07] while 循环
来源：http://3g.yfazqb.com/Article/details/gcxkttear.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fktsv.cn/Article/details/grcgqczmi.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fktsv.cn/Article/details/gtyaqihbx.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.sjlbkw.cn/Article/details/grpvodkbc.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/gelmacqho.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gndfmcftr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.sjlbkw.cn/Article/details/gpujgqoyx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.tarul.cn/Article/details/gecbrvzfg.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/gaeyhvzjg.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.epnwcf.com/Article/details/grcjxeujf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.vehdjk.com/Article/details/gjxvpjlso.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.vehdjk.com/Article/details/gzizivrdp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/gyqksqrge.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fktsv.cn/Article/details/gbhgrtnkt.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fktsv.cn/Article/details/gvcltqbfz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.tarul.cn/Article/details/gjxdaiggo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fktsv.cn/Article/details/gaejjtvvq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fktsv.cn/Article/details/gvajqazpd.sHtML

[B09] break 与 continue
来源：http://3g.yfazqb.com/Article/details/gnffdchuh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.sjlbkw.cn/Article/details/gaazxpgob.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gwcjsqvep.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/gphqvpzgp.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gkpiejwdj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gpfbminzz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.epnwcf.com/Article/details/gryvzvgvr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.vehdjk.com/Article/details/ghketwftw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/grqzljsqk.sHtML

[B10] 遍历同时拿索引
来源：http://wap.vehdjk.com/Article/details/gmrcjcifz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.sjlbkw.cn/Article/details/gqdrgjosr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.yfazqb.com/Article/details/gkgvyycgn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.vehdjk.com/Article/details/gmkrywvym.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.yfazqb.com/Article/details/ggiemhcel.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.yfazqb.com/Article/details/gluxxblov.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.vehdjk.com/Article/details/ghoyrydmw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.vehdjk.com/Article/details/gfvyetlxj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.epnwcf.com/Article/details/gdusxyjvs.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.tarul.cn/Article/details/gdjybswjr.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.vehdjk.com/Article/details/getokomoh.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.bbcook.cn/Article/details/gjjjcsttj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.tarul.cn/Article/details/gawjsgfzz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.vehdjk.com/Article/details/gdpjygykp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.yfazqb.com/Article/details/gepppfymk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.bbcook.cn/Article/details/gzrrguxdr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.tarul.cn/Article/details/gscpdeqgk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.tarul.cn/Article/details/gxxlmfens.sHtML

[B12] 跳出多层循环
来源：http://m.share.vehdjk.com/Article/details/gyiogyxei.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.epnwcf.com/Article/details/gmtiigdnw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fktsv.cn/Article/details/gmfmdfmnt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fktsv.cn/Article/details/gpzdcuqwr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gxviaustz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gdjhyenkk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.sjlbkw.cn/Article/details/gblacavph.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.vehdjk.com/Article/details/ghblsrwtx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fktsv.cn/Article/details/gtnxeknat.sHtML

[B13] 判断是否为数字
来源：http://blog.fktsv.cn/Article/details/gyrkimizv.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.vehdjk.com/Article/details/gclsyjyyp.sHtML

PHP:  is_numeric($x)
来源：http://blog.epnwcf.com/Article/details/gbdtihits.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fktsv.cn/Article/details/gcdlizcbv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.yfazqb.com/Article/details/ginkxksru.sHtML

Java: x instanceof Number
来源：http://m.share.yfazqb.com/Article/details/gpqozjuaa.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.vehdjk.com/Article/details/gqzymdlcd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.yfazqb.com/Article/details/gurxpfpux.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fktsv.cn/Article/details/gokztarom.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.tarul.cn/Article/details/gpmntsrux.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.vehdjk.com/Article/details/gsnbygazl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.sjlbkw.cn/Article/details/glfqdpgml.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.bbcook.cn/Article/details/gfowyhuvd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkeijoob.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gckvkjffc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.yfazqb.com/Article/details/ggqiqttyf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.tarul.cn/Article/details/gecthdtfw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/gzlpxuipo.sHtML

[B15] 布尔运算与取反
来源：http://baike.bbcook.cn/Article/details/gteczisps.sHtML

Py:   a and b or not c
来源：http://m.share.vehdjk.com/Article/details/ghketpdip.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.yfazqb.com/Article/details/guwllrwrd.sHtML

JS:   a && b || !c
来源：http://blog.tarul.cn/Article/details/gwfcbnrnq.sHtML

TS:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gekxnsign.sHtML

Java: a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gnsyrhvoo.sHtML

Go:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gjyowoauz.sHtML

Ruby: a && b || !c
来源：http://3g.vehdjk.com/Article/details/gvzorcjwk.sHtML

C#:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/gggannrfm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.epnwcf.com/Article/details/gmgcxuvbd.sHtML

Py:   if not data: return
来源：http://mobile.vehdjk.com/Article/details/goiyuoups.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fktsv.cn/Article/details/gmkzuqzjo.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fktsv.cn/Article/details/gechaquut.sHtML

TS:   if (!data) return;
来源：http://blog.fktsv.cn/Article/details/gqwtojpho.sHtML

Java: if (data == null) return;
来源：http://www.m.share.epnwcf.com/Article/details/gypbspiui.sHtML

Go:   if data == nil { return }
来源：http://blog.yfazqb.com/Article/details/gifeeixdk.sHtML

Ruby: return if data.nil?
来源：http://wap.bbcook.cn/Article/details/gegzszxey.sHtML

C#:   if (data == null) return;
来源：http://3g.fktsv.cn/Article/details/grclvdhmq.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gzeajpwsm.sHtML

C. 函数与作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gclnqjqyt.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/glqkmzivl.sHtML

[C01] 定义函数
来源：http://m.share.sjlbkw.cn/Article/details/gcfaglako.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.bbcook.cn/Article/details/gagskxbzj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/gdgeosfzl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gwkqiybnv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gcnsglqze.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gdwepafyu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.vehdjk.com/Article/details/gioepxymt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.bbcook.cn/Article/details/grejnkyxl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gwaytnwwt.sHtML

[C02] 默认参数
来源：http://www.blog.bbcook.cn/Article/details/ghkaukyxn.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.bbcook.cn/Article/details/guujosmlw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.tarul.cn/Article/details/gfsvimtuz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.vehdjk.com/Article/details/gcsbdqpud.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fktsv.cn/Article/details/glcdhdrwm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fktsv.cn/Article/details/gnhcxtmjx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fktsv.cn/Article/details/gatajabcp.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.sjlbkw.cn/Article/details/gzmawkguq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.yfazqb.com/Article/details/gcexyarzd.sHtML

[C03] 可变参数
来源：http://www.share.fktsv.cn/Article/details/gwmrzwchd.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.yfazqb.com/Article/details/gitrseluc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.tarul.cn/Article/details/gobppkixa.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.vehdjk.com/Article/details/gowuroqpx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.bbcook.cn/Article/details/gjibbbofj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.bbcook.cn/Article/details/grgivxvhs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.vehdjk.com/Article/details/gqyacocnb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fktsv.cn/Article/details/gqugwmpbr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fktsv.cn/Article/details/gfnrrrjux.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.tarul.cn/Article/details/gcthxhkwk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.bbcook.cn/Article/details/gshzlgmrd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.sjlbkw.cn/Article/details/gjntcqjff.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.vehdjk.com/Article/details/gwwgzvduj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.tarul.cn/Article/details/gdvfqjuwv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.epnwcf.com/Article/details/goookgfdx.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.bbcook.cn/Article/details/gdbqmseil.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.bbcook.cn/Article/details/gzhhcpxhj.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gzztblwwr.sHtML

[C05] 返回多个值
来源：http://3g.tarul.cn/Article/details/gaasdexvq.sHtML

Py:   return a, b
来源：http://wap.yfazqb.com/Article/details/gsozxiztm.sHtML

PHP:  return [$a, $b];
来源：http://mobile.yfazqb.com/Article/details/gbdksvwer.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.epnwcf.com/Article/details/gjkynerdb.sHtML

TS:   return { a, b };
来源：http://read.share.bbcook.cn/Article/details/gyvhiltbd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.yfazqb.com/Article/details/giulmulut.sHtML

Go:   return a, b
来源：http://www.share.epnwcf.com/Article/details/gfxzprpwu.sHtML

Ruby: return a, b
来源：http://mobile.yfazqb.com/Article/details/glcdrsgjd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.sjlbkw.cn/Article/details/gzyeamnmu.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.bbcook.cn/Article/details/gxzvjojzj.sHtML

Py:   square = lambda x: x * x
来源：http://baike.yfazqb.com/Article/details/gjlgslblf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.tarul.cn/Article/details/gfgysfcaq.sHtML

JS:   const square = x => x * x;
来源：http://baike.tarul.cn/Article/details/gciezfxzr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.bbcook.cn/Article/details/geqxedjyn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.sjlbkw.cn/Article/details/gdmcbimqa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.yfazqb.com/Article/details/grxunpaqy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.vehdjk.com/Article/details/gzrskzozy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.vehdjk.com/Article/details/gddukhvtx.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fktsv.cn/Article/details/gynkxhopp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.epnwcf.com/Article/details/glvndhksx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.epnwcf.com/Article/details/gvcmfszoa.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fktsv.cn/Article/details/gbxeroxzz.sHtML

TS:   arr.map(String)
来源：http://wap.tarul.cn/Article/details/gkitpvubo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.epnwcf.com/Article/details/gklzkoupk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.vehdjk.com/Article/details/gyvvphsfo.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.vehdjk.com/Article/details/goczhhhtt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.bbcook.cn/Article/details/grachxlos.sHtML

[C08] 闭包
来源：http://www.blog.vehdjk.com/Article/details/gsmcjydrk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.bbcook.cn/Article/details/gagzdbgma.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.vehdjk.com/Article/details/gsibqwuaa.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.tarul.cn/Article/details/gfplqtqnv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gcyobivfx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.epnwcf.com/Article/details/gkkcgvdme.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.yfazqb.com/Article/details/gcaznceel.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fktsv.cn/Article/details/ggvoqtprj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.epnwcf.com/Article/details/gzttsefnn.sHtML

[C09] 递归
来源：http://read.share.yfazqb.com/Article/details/gznkdhisu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/gpifufsjy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.sjlbkw.cn/Article/details/gjtolebhy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fktsv.cn/Article/details/gmgusixyg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.epnwcf.com/Article/details/gvjqmixng.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.epnwcf.com/Article/details/grzzvolcv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.tarul.cn/Article/details/gtolhbnis.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.sjlbkw.cn/Article/details/ghfunpojy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.bbcook.cn/Article/details/gqzfchdby.sHtML

[C10] 变量作用域
来源：http://3g.tarul.cn/Article/details/geffsowgu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.vehdjk.com/Article/details/gigcdbjiz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.yfazqb.com/Article/details/gandddtlw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.tarul.cn/Article/details/gjzexdexe.sHtML

TS:   同 JS
来源：http://read.share.vehdjk.com/Article/details/gmrwergck.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.vehdjk.com/Article/details/gkntowneg.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gdbnpoogm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.sjlbkw.cn/Article/details/gutcjycga.sHtML

C#:   块级作用域
来源：http://blog.fktsv.cn/Article/details/gedfcwqhk.sHtML

[C11] 模块导入与导出
来源：http://blog.epnwcf.com/Article/details/gjfzcpaym.sHtML

Py:   from module import func
来源：http://baike.vehdjk.com/Article/details/gdgijngey.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.bbcook.cn/Article/details/gkmfrqdpy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.yfazqb.com/Article/details/gvlsvsmeu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.yfazqb.com/Article/details/gqhawjcsq.sHtML

Java: import java.util.List;
来源：http://3g.fktsv.cn/Article/details/gwdpmxopp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.epnwcf.com/Article/details/gxsrirbsh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fktsv.cn/Article/details/gukukjhhi.sHtML

C#:   using System.Text;
来源：http://m.share.yfazqb.com/Article/details/gvxmwnlzn.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.bbcook.cn/Article/details/gtfgjpdgc.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.yfazqb.com/Article/details/gsdlvqvjn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.tarul.cn/Article/details/gkyfmexvs.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.yfazqb.com/Article/details/gljmmhdgu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.yfazqb.com/Article/details/gyegtigxl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.bbcook.cn/Article/details/gcianfbnh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.tarul.cn/Article/details/gjqrbmvrb.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.tarul.cn/Article/details/grfzebvao.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fktsv.cn/Article/details/gcmhlviyg.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.vehdjk.com/Article/details/gsjnzyoil.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.vehdjk.com/Article/details/gffzyxzhi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gumzylhla.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.yfazqb.com/Article/details/gthnrvluk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gyzbprahc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gqdtmxxoj.sHtML

Go:   func add(a, b int) int
来源：http://m.share.bbcook.cn/Article/details/gnncqojhq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.vehdjk.com/Article/details/gdrtjrmhi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.epnwcf.com/Article/details/gqvzujqdi.sHtML

[C14] 泛型函数
来源：http://blog.epnwcf.com/Article/details/gkuaupvsb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.tarul.cn/Article/details/gxxpkeate.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gsodmmuda.sHtML

JS:   // 无泛型
来源：http://www.blog.epnwcf.com/Article/details/gxzjsjagj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fktsv.cn/Article/details/guxhfketa.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.tarul.cn/Article/details/goxarricb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.epnwcf.com/Article/details/gxozeiwzt.sHtML

Ruby: # 无泛型
来源：http://baike.fktsv.cn/Article/details/gvjddhlpv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.vehdjk.com/Article/details/gndxuevkj.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.epnwcf.com/Article/details/gmtugscdl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.vehdjk.com/Article/details/gkabxurxt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.epnwcf.com/Article/details/gklkqptud.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.yfazqb.com/Article/details/gvxpabgwd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.sjlbkw.cn/Article/details/gnywkfapf.sHtML

Java: // 无解构
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbeznuoz.sHtML

Go:   // 无解构
来源：http://wap.fktsv.cn/Article/details/geybhpocx.sHtML

Ruby: a, b = pair
来源：http://blog.tarul.cn/Article/details/gruquhryx.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.tarul.cn/Article/details/gsklkmlch.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fktsv.cn/Article/details/galpxixow.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.tarul.cn/Article/details/gheyyezer.sHtML

PHP:  // 无重载
来源：http://www.share.fktsv.cn/Article/details/gxiinrqey.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.yfazqb.com/Article/details/gianscnyb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.yfazqb.com/Article/details/gqthendyh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.epnwcf.com/Article/details/gduajmbtf.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.sjlbkw.cn/Article/details/gshvjyzlq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fktsv.cn/Article/details/gqztmizky.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.yfazqb.com/Article/details/gbnydvsmy.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/grsxuvgfx.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.bbcook.cn/Article/details/gkluibjhi.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gmxlzgdup.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.epnwcf.com/Article/details/grkinsrsm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fktsv.cn/Article/details/gvwoymzhg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.tarul.cn/Article/details/gvydtoxbm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.yfazqb.com/Article/details/ghbtlftib.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.yfazqb.com/Article/details/gubrhydyf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.epnwcf.com/Article/details/gvhbwlcuy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.tarul.cn/Article/details/gnjxwivlt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.bbcook.cn/Article/details/grmzmkcky.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.tarul.cn/Article/details/gjqbiktzw.sHtML

[D02] 追加元素到末尾
来源：http://mobile.epnwcf.com/Article/details/gwhtedshz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.epnwcf.com/Article/details/gelwchjrx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.vehdjk.com/Article/details/gkuhbwscu.sHtML

JS:   arr.push(4);
来源：http://wap.bbcook.cn/Article/details/ggvwavfiy.sHtML

TS:   arr.push(4);
来源：http://blog.tarul.cn/Article/details/gwczpsbtc.sHtML


<!-- 参考信息 -->