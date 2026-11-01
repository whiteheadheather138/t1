代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.bbcook.cn/Article/details/grsvydxas.sHtML

[B02] 多分支 else if / elif
来源：http://blog.tarul.cn/Article/details/gpvpltupg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.tarul.cn/Article/details/gfspzperi.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.vehdjk.com/Article/details/gtiayipzz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.sjlbkw.cn/Article/details/guvrduhmw.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.tarul.cn/Article/details/geylrqokp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.epnwcf.com/Article/details/giqgzqcii.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.bbcook.cn/Article/details/gqxooeaiy.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.bbcook.cn/Article/details/goqsdbzmy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.vehdjk.com/Article/details/gyqlpulyr.sHtML

[B03] switch / match / case
来源：http://www.m.share.epnwcf.com/Article/details/gqqlvcrco.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.sjlbkw.cn/Article/details/gdnxxqxdq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/geicwlbtv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.sjlbkw.cn/Article/details/gozglrfid.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.sjlbkw.cn/Article/details/gpxeodqsb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.tarul.cn/Article/details/gvndhfgjx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.bbcook.cn/Article/details/gxxvgrhoc.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.epnwcf.com/Article/details/gjusnaiwt.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.bbcook.cn/Article/details/gxqvyrflw.sHtML

[B04] for 计数循环
来源：http://www.m.share.vehdjk.com/Article/details/gejixgwja.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.vehdjk.com/Article/details/gwjrwutok.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.tarul.cn/Article/details/gfoipituv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.epnwcf.com/Article/details/gxtscjmvs.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.epnwcf.com/Article/details/ghmmmblhp.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.fktsv.cn/Article/details/gjsmjropr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.bbcook.cn/Article/details/giygmrvky.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.sjlbkw.cn/Article/details/gnisaezvh.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.epnwcf.com/Article/details/gsvmeihvh.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.yfazqb.com/Article/details/gcocpudvh.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.bbcook.cn/Article/details/gektblmse.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.bbcook.cn/Article/details/gwvsuoixl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fktsv.cn/Article/details/gawlxblnt.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.bbcook.cn/Article/details/groqhtaed.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.bbcook.cn/Article/details/gdonfiodl.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fktsv.cn/Article/details/gcqjilxpl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.tarul.cn/Article/details/gkcbuatry.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.epnwcf.com/Article/details/gobndmwtd.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fktsv.cn/Article/details/gigxafovc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.sjlbkw.cn/Article/details/gdnxrxbbt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.sjlbkw.cn/Article/details/gzzaghigy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fktsv.cn/Article/details/gdtapontw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.epnwcf.com/Article/details/gagwikjod.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.yfazqb.com/Article/details/gmxycmlxo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.vehdjk.com/Article/details/gudyobxmp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvscwnrd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fktsv.cn/Article/details/gsedazkkp.sHtML

[B07] while 循环
来源：http://www.m.share.epnwcf.com/Article/details/grlszilap.sHtML

Py:   while i < 10: i += 1
来源：http://baike.epnwcf.com/Article/details/gckhmkbpx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.yfazqb.com/Article/details/gvikrhoyd.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gbtuqcxyh.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/ghlbyqfjb.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.vehdjk.com/Article/details/gzazvvvze.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.tarul.cn/Article/details/gkbqilduf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.epnwcf.com/Article/details/gtosbwrhf.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.tarul.cn/Article/details/gwptizsgr.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fktsv.cn/Article/details/gtfuygret.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.epnwcf.com/Article/details/gvhgecbhc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.epnwcf.com/Article/details/gkhnyuwlj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/grbgxhplq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/godmqmunw.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/gihvwlbfk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.vehdjk.com/Article/details/ghhdmqocq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.epnwcf.com/Article/details/gzqcknhqk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/ggartqeya.sHtML

[B09] break 与 continue
来源：http://wap.tarul.cn/Article/details/gmvyfjaod.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.epnwcf.com/Article/details/gsmanyqgz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gpuvfotfh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gqxynreuh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gwnwzkfcn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gdvmidtcu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.tarul.cn/Article/details/gxgypvcjj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.vehdjk.com/Article/details/gwkmblnhe.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/gnhofyesq.sHtML

[B10] 遍历同时拿索引
来源：http://blog.vehdjk.com/Article/details/grmdbycrc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.tarul.cn/Article/details/gegitybuz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.vehdjk.com/Article/details/gnsultlri.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.tarul.cn/Article/details/ghrazjwpw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.tarul.cn/Article/details/gqkanbwaw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.epnwcf.com/Article/details/gurmxfvcb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.bbcook.cn/Article/details/gyhfrzwkn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.bbcook.cn/Article/details/gowrymomu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.tarul.cn/Article/details/gsrwmwmbs.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.sjlbkw.cn/Article/details/giotwccgd.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.vehdjk.com/Article/details/gmxxofapp.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fktsv.cn/Article/details/gdozcfgxy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.epnwcf.com/Article/details/gfdflorsr.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.tarul.cn/Article/details/gpqnbpjhf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.tarul.cn/Article/details/gcyfruzbm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.epnwcf.com/Article/details/gyggrbusr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.yfazqb.com/Article/details/gcjwcibqr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fktsv.cn/Article/details/gaakfjgiv.sHtML

[B12] 跳出多层循环
来源：http://read.share.vehdjk.com/Article/details/gtuhwybhg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.tarul.cn/Article/details/gdnfxnfna.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.sjlbkw.cn/Article/details/gihqqlkvg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/ggrifoxuj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.bbcook.cn/Article/details/gwkgkpnot.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.bbcook.cn/Article/details/givyimemq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.yfazqb.com/Article/details/gzjtnlfbp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.tarul.cn/Article/details/ghatbvcrs.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.bbcook.cn/Article/details/gdxnbpalf.sHtML

[B13] 判断是否为数字
来源：http://mobile.sjlbkw.cn/Article/details/ggqvnaapj.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fktsv.cn/Article/details/gavzksulu.sHtML

PHP:  is_numeric($x)
来源：http://baike.fktsv.cn/Article/details/gxhxaarjx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.bbcook.cn/Article/details/gfzqxiduw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.tarul.cn/Article/details/grxsjrzjh.sHtML

Java: x instanceof Number
来源：http://mobile.epnwcf.com/Article/details/gveqzerwf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.tarul.cn/Article/details/gtjkslxxb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fktsv.cn/Article/details/gnwgtizkz.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fktsv.cn/Article/details/ggjjthdba.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.yfazqb.com/Article/details/ggojvtgtq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.tarul.cn/Article/details/gjyiqdryo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.vehdjk.com/Article/details/gbfwfwvcl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.tarul.cn/Article/details/gsukvioyo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.epnwcf.com/Article/details/ghkzlyvtm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.vehdjk.com/Article/details/gwqlbniso.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.sjlbkw.cn/Article/details/gzhczlqsx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.tarul.cn/Article/details/goqpxmfip.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.vehdjk.com/Article/details/gaigtgcny.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.tarul.cn/Article/details/gsdetgmui.sHtML

Py:   a and b or not c
来源：http://blog.vehdjk.com/Article/details/gzekemlsg.sHtML

PHP:  $a && $b || !$c
来源：http://blog.sjlbkw.cn/Article/details/ghlyhilqs.sHtML

JS:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/ghduwqvej.sHtML

TS:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/geigithwx.sHtML

Java: a && b || !c
来源：http://wap.epnwcf.com/Article/details/gonrcozwb.sHtML

Go:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gtcxonozd.sHtML

Ruby: a && b || !c
来源：http://baike.yfazqb.com/Article/details/gmewuruqx.sHtML

C#:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gevulldbv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.vehdjk.com/Article/details/gdmvqxcqn.sHtML

Py:   if not data: return
来源：http://read.share.yfazqb.com/Article/details/gfqrhomun.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlhqijbv.sHtML

JS:   if (!data) return;
来源：http://www.m.share.bbcook.cn/Article/details/geowgvxlh.sHtML

TS:   if (!data) return;
来源：http://3g.tarul.cn/Article/details/gwblojazg.sHtML

Java: if (data == null) return;
来源：http://www.share.yfazqb.com/Article/details/gwxtckjqs.sHtML

Go:   if data == nil { return }
来源：http://m.share.vehdjk.com/Article/details/gmtfuuvol.sHtML

Ruby: return if data.nil?
来源：http://mobile.sjlbkw.cn/Article/details/ggslrypkw.sHtML

C#:   if (data == null) return;
来源：http://www.share.bbcook.cn/Article/details/ghukarimz.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gnbajfpfh.sHtML

C. 函数与作用域
来源：http://www.blog.fktsv.cn/Article/details/ghjffkghn.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/grytkvejs.sHtML

[C01] 定义函数
来源：http://3g.vehdjk.com/Article/details/gruxwnhyk.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.vehdjk.com/Article/details/gjoutnlwe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/goztywapb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gskencfna.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gjtqwxuww.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gvwosizeb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.vehdjk.com/Article/details/giqrcbsqr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.vehdjk.com/Article/details/gcoagdmqg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gmgoitvrq.sHtML

[C02] 默认参数
来源：http://m.share.yfazqb.com/Article/details/ggsizhxlj.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.tarul.cn/Article/details/gwbwcuyws.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.yfazqb.com/Article/details/gwnvxrydy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.bbcook.cn/Article/details/gbrfuxjsf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gogoouaxb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.vehdjk.com/Article/details/gdjicefpq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.epnwcf.com/Article/details/ggctvleaa.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.epnwcf.com/Article/details/gpatwnaez.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fktsv.cn/Article/details/gkanohgzo.sHtML

[C03] 可变参数
来源：http://www.blog.bbcook.cn/Article/details/gtrvfleho.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.vehdjk.com/Article/details/ggxjauuov.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.tarul.cn/Article/details/gwtvqegie.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.bbcook.cn/Article/details/goqkpwjoh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.yfazqb.com/Article/details/gzvmdrpry.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.vehdjk.com/Article/details/goqceowtv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fktsv.cn/Article/details/grcjeihyu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.vehdjk.com/Article/details/gptofyqqv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.yfazqb.com/Article/details/glrhwarku.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.tarul.cn/Article/details/gyidwmqfg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.bbcook.cn/Article/details/gdebhrzng.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fktsv.cn/Article/details/gyoejuztm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fktsv.cn/Article/details/gcvqzcjmn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.sjlbkw.cn/Article/details/gbgnmalxg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.vehdjk.com/Article/details/gsvyucmbj.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.epnwcf.com/Article/details/gusodnury.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.bbcook.cn/Article/details/gzevsaoyy.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/grvzlmusr.sHtML

[C05] 返回多个值
来源：http://read.share.yfazqb.com/Article/details/gbuayxjhl.sHtML

Py:   return a, b
来源：http://3g.vehdjk.com/Article/details/gqvaqlufi.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fktsv.cn/Article/details/gvkzgjblg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.yfazqb.com/Article/details/ggzrbvygi.sHtML

TS:   return { a, b };
来源：http://www.blog.bbcook.cn/Article/details/gqwinlicf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.vehdjk.com/Article/details/gcmiebfan.sHtML

Go:   return a, b
来源：http://read.share.epnwcf.com/Article/details/gighwiiim.sHtML

Ruby: return a, b
来源：http://www.m.share.bbcook.cn/Article/details/gjqqawqat.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.bbcook.cn/Article/details/gmhjtevga.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.tarul.cn/Article/details/gctgghodm.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.epnwcf.com/Article/details/gajhnunzo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.bbcook.cn/Article/details/gzumgrtox.sHtML

JS:   const square = x => x * x;
来源：http://3g.tarul.cn/Article/details/gvzpdhlin.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.tarul.cn/Article/details/gunwxojma.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.yfazqb.com/Article/details/gjhoxxndw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.bbcook.cn/Article/details/gwgwvakyq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.sjlbkw.cn/Article/details/gvkteyqpo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fktsv.cn/Article/details/gaemfxexu.sHtML

[C07] 把函数作为参数传入
来源：http://wap.yfazqb.com/Article/details/gszrrwjzo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.bbcook.cn/Article/details/gajuejnok.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.epnwcf.com/Article/details/gkibwjlhf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fktsv.cn/Article/details/gtwahaefq.sHtML

TS:   arr.map(String)
来源：http://mobile.sjlbkw.cn/Article/details/gxksqjjui.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.yfazqb.com/Article/details/giluxnjdx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.tarul.cn/Article/details/gyrmnyfqt.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.sjlbkw.cn/Article/details/gkrrgdnsw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.tarul.cn/Article/details/gvpcusfte.sHtML

[C08] 闭包
来源：http://blog.yfazqb.com/Article/details/gpyxgojrg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fktsv.cn/Article/details/gduqihihu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.vehdjk.com/Article/details/gqyverldr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.vehdjk.com/Article/details/gefvoucat.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.bbcook.cn/Article/details/gvfidnqcy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fktsv.cn/Article/details/gajvzobqp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fktsv.cn/Article/details/gpcwofnrk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.tarul.cn/Article/details/gwhmlgygr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.bbcook.cn/Article/details/gqwuqrjml.sHtML

[C09] 递归
来源：http://m.share.tarul.cn/Article/details/gjyncxqhk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fktsv.cn/Article/details/gqemiayad.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.yfazqb.com/Article/details/gaonhxlse.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.bbcook.cn/Article/details/gtnazxwww.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fktsv.cn/Article/details/gtinzexvx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.vehdjk.com/Article/details/gajqufgdk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fktsv.cn/Article/details/gccfrncrf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.bbcook.cn/Article/details/gfqvqevqm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.vehdjk.com/Article/details/gmjrcgoll.sHtML

[C10] 变量作用域
来源：http://read.share.fktsv.cn/Article/details/gjvkigdyy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.sjlbkw.cn/Article/details/gxemkzynp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.tarul.cn/Article/details/gmiuiprcn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.sjlbkw.cn/Article/details/godmrmplo.sHtML

TS:   同 JS
来源：http://mobile.vehdjk.com/Article/details/gjxlvxldl.sHtML

Java: 方法内为块级作用域
来源：http://read.share.bbcook.cn/Article/details/gghyqectq.sHtML

Go:   花括号块级作用域
来源：http://blog.sjlbkw.cn/Article/details/gffcyvhgu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.epnwcf.com/Article/details/gelfcutib.sHtML

C#:   块级作用域
来源：http://mobile.tarul.cn/Article/details/gfupwqmkb.sHtML

[C11] 模块导入与导出
来源：http://baike.vehdjk.com/Article/details/gqezrmwaq.sHtML

Py:   from module import func
来源：http://www.m.share.yfazqb.com/Article/details/guhtpbdns.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fktsv.cn/Article/details/gwhokcyby.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.sjlbkw.cn/Article/details/gqponnpzv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fktsv.cn/Article/details/gtakzqlel.sHtML

Java: import java.util.List;
来源：http://www.share.sjlbkw.cn/Article/details/gymnstxym.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.epnwcf.com/Article/details/ghhzodinq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.yfazqb.com/Article/details/gcurngxeh.sHtML

C#:   using System.Text;
来源：http://mobile.yfazqb.com/Article/details/gvtrmpmuo.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.sjlbkw.cn/Article/details/gkeqtxfgk.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.tarul.cn/Article/details/gbcdxzude.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqorfrkv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.bbcook.cn/Article/details/gqhhedrpy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.tarul.cn/Article/details/ghfcezkfk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.sjlbkw.cn/Article/details/garwuktap.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.yfazqb.com/Article/details/grcgidltp.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.vehdjk.com/Article/details/giaocakri.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.epnwcf.com/Article/details/gsztpwdey.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.epnwcf.com/Article/details/gmtxoabro.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.tarul.cn/Article/details/gduxswzgb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/givqsgpaa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.yfazqb.com/Article/details/gzqtzplls.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gmnnbmxrj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gezkjogaj.sHtML

Go:   func add(a, b int) int
来源：http://wap.yfazqb.com/Article/details/ghvvdnkob.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.epnwcf.com/Article/details/gzoxdsces.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.yfazqb.com/Article/details/gnjzbhqrj.sHtML

[C14] 泛型函数
来源：http://www.m.share.bbcook.cn/Article/details/gfnailfnx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.sjlbkw.cn/Article/details/gzlncspvo.sHtML

PHP:  // 无泛型
来源：http://wap.fktsv.cn/Article/details/ghlbishry.sHtML

JS:   // 无泛型
来源：http://wap.fktsv.cn/Article/details/gsccdfqht.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.bbcook.cn/Article/details/gtpktklyd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.vehdjk.com/Article/details/gcpjjzllv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.epnwcf.com/Article/details/grnvgipik.sHtML

Ruby: # 无泛型
来源：http://3g.sjlbkw.cn/Article/details/gxfmokrgq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.epnwcf.com/Article/details/golxszwrr.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.vehdjk.com/Article/details/glagqtssl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.vehdjk.com/Article/details/gutvivklw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.yfazqb.com/Article/details/gbeqapvmc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.yfazqb.com/Article/details/gikzwdbrv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.bbcook.cn/Article/details/gtoiwjjmm.sHtML

Java: // 无解构
来源：http://mobile.vehdjk.com/Article/details/gnknbohzw.sHtML

Go:   // 无解构
来源：http://www.share.epnwcf.com/Article/details/gnlqnixxk.sHtML

Ruby: a, b = pair
来源：http://mobile.epnwcf.com/Article/details/ggzklyajv.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fktsv.cn/Article/details/gfxnfffmj.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fktsv.cn/Article/details/gebwjdzeq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.epnwcf.com/Article/details/grhzfsbhy.sHtML

PHP:  // 无重载
来源：http://www.share.vehdjk.com/Article/details/gklbcznrd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.sjlbkw.cn/Article/details/gtpjlavnr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.sjlbkw.cn/Article/details/gpwqslirk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.vehdjk.com/Article/details/gvgxsvgys.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.yfazqb.com/Article/details/gvrgrsylg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.yfazqb.com/Article/details/giwsfqqdf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fktsv.cn/Article/details/gudjjusoo.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gikycelwd.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.sjlbkw.cn/Article/details/gpotixqfp.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gjkxeznvi.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fktsv.cn/Article/details/gmdvuhwam.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.tarul.cn/Article/details/gmcyywffh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.sjlbkw.cn/Article/details/gptodanml.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.vehdjk.com/Article/details/guakepnsw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.sjlbkw.cn/Article/details/gmmekfvat.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.yfazqb.com/Article/details/gizxdxogx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.sjlbkw.cn/Article/details/gdinkcruy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.epnwcf.com/Article/details/gqrfjwfrb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.tarul.cn/Article/details/gcavlyvpb.sHtML

[D02] 追加元素到末尾
来源：http://www.share.tarul.cn/Article/details/gyexivebp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.yfazqb.com/Article/details/gvfxegsua.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.vehdjk.com/Article/details/gvfsbabba.sHtML

JS:   arr.push(4);
来源：http://read.share.bbcook.cn/Article/details/gpmwxmnqt.sHtML

TS:   arr.push(4);
来源：http://mobile.fktsv.cn/Article/details/gjupluboh.sHtML


<!-- 参考信息 -->