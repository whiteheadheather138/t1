代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.vehdjk.com/Article/details/gwjggxhow.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.epnwcf.com/Article/details/gbtvehpth.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/gnxhsxmbp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.epnwcf.com/Article/details/gkpskfjpg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.fktsv.cn/Article/details/gmqvyofdf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.bbcook.cn/Article/details/gjfgbxzou.sHtML

[B03] switch / match / case
来源：http://blog.tarul.cn/Article/details/gbxkrojez.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.vehdjk.com/Article/details/gujvkgayb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/gncrcxkks.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.bbcook.cn/Article/details/gqwbiieot.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/gfstvgvlu.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.yfazqb.com/Article/details/gdkwzupje.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.yfazqb.com/Article/details/gjvmbzpuv.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.yfazqb.com/Article/details/gfctddidg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.bbcook.cn/Article/details/gldgmkunb.sHtML

[B04] for 计数循环
来源：http://baike.epnwcf.com/Article/details/gidfoqsoh.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.yfazqb.com/Article/details/gieqaxfcp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.yfazqb.com/Article/details/gxyunqfth.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.yfazqb.com/Article/details/gbsjvzjsb.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.vehdjk.com/Article/details/ghhkqfvlv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.vehdjk.com/Article/details/gowcqempi.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.yfazqb.com/Article/details/gqpvkpivl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.epnwcf.com/Article/details/gotjoyvhi.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.vehdjk.com/Article/details/gnfjykkga.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.sjlbkw.cn/Article/details/gbxslbyhm.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.vehdjk.com/Article/details/gvxgicffj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.bbcook.cn/Article/details/gwcmivwir.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.tarul.cn/Article/details/grhqyomne.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.tarul.cn/Article/details/gmzavpzwv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.vehdjk.com/Article/details/gjbjuesvq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.sjlbkw.cn/Article/details/grmnqlkpx.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.vehdjk.com/Article/details/gkhhuzfqp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.sjlbkw.cn/Article/details/grstbysns.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.sjlbkw.cn/Article/details/gkvrvswav.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgnsyltl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.yfazqb.com/Article/details/gmyjkeatv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.yfazqb.com/Article/details/gqpladoke.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.bbcook.cn/Article/details/ghdxnkwbo.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.vehdjk.com/Article/details/gzyeaqjhs.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.fktsv.cn/Article/details/ggnjkcemh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.vehdjk.com/Article/details/ggsxdyvns.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.tarul.cn/Article/details/gjjadsyth.sHtML

[B07] while 循环
来源：http://www.m.share.fktsv.cn/Article/details/gcphnzjjk.sHtML

Py:   while i < 10: i += 1
来源：http://baike.sjlbkw.cn/Article/details/gsdxufiog.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fktsv.cn/Article/details/gleucwtch.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gqzdxsluq.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.vehdjk.com/Article/details/gppdmdxjk.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/ggsocpqng.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.yfazqb.com/Article/details/gttfzhsnt.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.vehdjk.com/Article/details/gqsrpoumw.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/ghbzwgqtp.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.fktsv.cn/Article/details/ginkkkrqa.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.epnwcf.com/Article/details/gpuyasxvb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.sjlbkw.cn/Article/details/gqphnfnci.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/gqhkgvlxg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/gxstledco.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gsbqudryf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.bbcook.cn/Article/details/gohuobtfb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fktsv.cn/Article/details/ggeynkler.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/gywafqsdq.sHtML

[B09] break 与 continue
来源：http://wap.tarul.cn/Article/details/gjqghigmk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.tarul.cn/Article/details/gxfnunfba.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/glmkmxtov.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/ggzheyxyn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gbymqycbm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/gwbksdexm.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fktsv.cn/Article/details/geabndxcn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.yfazqb.com/Article/details/gqcrfpvnr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/goiqfvapf.sHtML

[B10] 遍历同时拿索引
来源：http://3g.tarul.cn/Article/details/gzmlcegus.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.tarul.cn/Article/details/gskyuxgyq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.bbcook.cn/Article/details/gmjfjrvss.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.sjlbkw.cn/Article/details/glefrhvbi.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.vehdjk.com/Article/details/gqleykpzg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.vehdjk.com/Article/details/gqvzearyq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.yfazqb.com/Article/details/gbapxgfsi.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.tarul.cn/Article/details/gqyicezgh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.sjlbkw.cn/Article/details/gevvohqmg.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.vehdjk.com/Article/details/gkmyvljqt.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.tarul.cn/Article/details/gxjztfpoi.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.yfazqb.com/Article/details/gmfspdtzv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.bbcook.cn/Article/details/gtgbihdzo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.bbcook.cn/Article/details/gpipidhcj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.epnwcf.com/Article/details/gwlcpzccu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.epnwcf.com/Article/details/ghqrpjllo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.epnwcf.com/Article/details/gsigfahmu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.epnwcf.com/Article/details/gonbtlgsg.sHtML

[B12] 跳出多层循环
来源：http://mobile.bbcook.cn/Article/details/ghonmqwpc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fktsv.cn/Article/details/girhqmfjz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.vehdjk.com/Article/details/gausurzfl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.bbcook.cn/Article/details/gxaxjabdw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqdbcuav.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.yfazqb.com/Article/details/gzajgxwbi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.vehdjk.com/Article/details/gzboizlwi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.sjlbkw.cn/Article/details/gqfizeyae.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.epnwcf.com/Article/details/gynbljgfe.sHtML

[B13] 判断是否为数字
来源：http://mobile.vehdjk.com/Article/details/gsebfbili.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.tarul.cn/Article/details/gmhpxrzgk.sHtML

PHP:  is_numeric($x)
来源：http://m.share.tarul.cn/Article/details/gkeqhsflw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.bbcook.cn/Article/details/gfpqvrbbj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.epnwcf.com/Article/details/geufeqxwk.sHtML

Java: x instanceof Number
来源：http://www.share.yfazqb.com/Article/details/gnaptpadv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.sjlbkw.cn/Article/details/gulvfosvg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.vehdjk.com/Article/details/ganvwsgad.sHtML

C#:   x is int or double or decimal
来源：http://m.share.vehdjk.com/Article/details/gkklyhorv.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fktsv.cn/Article/details/gjzgtkixy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.epnwcf.com/Article/details/guluejrnh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.yfazqb.com/Article/details/ghaopjxqb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gflwxkciy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.epnwcf.com/Article/details/giqflblfb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/geawsrglt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.yfazqb.com/Article/details/gmfirnphc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/gnebstacq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.bbcook.cn/Article/details/ginlcewqw.sHtML

[B15] 布尔运算与取反
来源：http://mobile.sjlbkw.cn/Article/details/goxhlfnwu.sHtML

Py:   a and b or not c
来源：http://3g.vehdjk.com/Article/details/gxmuwdjrr.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.epnwcf.com/Article/details/gypvnuteh.sHtML

JS:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gearjmvge.sHtML

TS:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/gnrrpkdlr.sHtML

Java: a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gihzfbbjp.sHtML

Go:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gpnpavndu.sHtML

Ruby: a && b || !c
来源：http://baike.bbcook.cn/Article/details/gtttbppto.sHtML

C#:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gqkuzzdjd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fktsv.cn/Article/details/gbhphetmi.sHtML

Py:   if not data: return
来源：http://www.m.share.epnwcf.com/Article/details/glaplaros.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.yfazqb.com/Article/details/gbtdumsdz.sHtML

JS:   if (!data) return;
来源：http://www.blog.bbcook.cn/Article/details/ghifazmdp.sHtML

TS:   if (!data) return;
来源：http://mobile.fktsv.cn/Article/details/geefbizid.sHtML

Java: if (data == null) return;
来源：http://blog.yfazqb.com/Article/details/giriampyo.sHtML

Go:   if data == nil { return }
来源：http://www.share.tarul.cn/Article/details/grbgxzeta.sHtML

Ruby: return if data.nil?
来源：http://m.share.epnwcf.com/Article/details/gaabklavt.sHtML

C#:   if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/gjrduhwbd.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gnrxybtls.sHtML

C. 函数与作用域
来源：http://www.share.sjlbkw.cn/Article/details/gdsmmxapw.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gnzkwqviu.sHtML

[C01] 定义函数
来源：http://www.share.epnwcf.com/Article/details/gnenlkxsl.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.yfazqb.com/Article/details/ggcvnuzll.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gymchiyzf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gpmbuvhzs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gegigrtec.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gvjmuerac.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.bbcook.cn/Article/details/gtuclvovq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.epnwcf.com/Article/details/gzugumeuh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gojybrmfn.sHtML

[C02] 默认参数
来源：http://www.share.tarul.cn/Article/details/gbtgfouda.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.bbcook.cn/Article/details/gegmxfydg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.epnwcf.com/Article/details/gktpltgeb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.epnwcf.com/Article/details/gtrysoduz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.yfazqb.com/Article/details/gnqxrbbwm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.vehdjk.com/Article/details/gnpzxaykk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.bbcook.cn/Article/details/gvkgyqsxd.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.yfazqb.com/Article/details/gkyspfnhf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.sjlbkw.cn/Article/details/grmcrspnt.sHtML

[C03] 可变参数
来源：http://www.m.share.tarul.cn/Article/details/glrscgxgk.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fktsv.cn/Article/details/gebrstxxu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.yfazqb.com/Article/details/gfwivrspc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/ggrrjejzt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.epnwcf.com/Article/details/gworporsg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.bbcook.cn/Article/details/gnyrfwbpd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.vehdjk.com/Article/details/gmsvflvxz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.bbcook.cn/Article/details/gryjouacs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.sjlbkw.cn/Article/details/gznqdjikt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.vehdjk.com/Article/details/ghjxiqphp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.bbcook.cn/Article/details/gnmbqiwtx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gghemisoh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.epnwcf.com/Article/details/goteybaee.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fktsv.cn/Article/details/gdoxscnld.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.epnwcf.com/Article/details/gtfivtrbx.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.vehdjk.com/Article/details/galetlgph.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.epnwcf.com/Article/details/gcrbbaihn.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.sjlbkw.cn/Article/details/gsmzgnadf.sHtML

[C05] 返回多个值
来源：http://m.share.vehdjk.com/Article/details/gpcshqpoc.sHtML

Py:   return a, b
来源：http://read.share.epnwcf.com/Article/details/gilwbvcyd.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fktsv.cn/Article/details/gcrbfbvkb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.bbcook.cn/Article/details/gglmeefxd.sHtML

TS:   return { a, b };
来源：http://www.blog.bbcook.cn/Article/details/gmmdcknuc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.vehdjk.com/Article/details/gcvsdhcmw.sHtML

Go:   return a, b
来源：http://wap.yfazqb.com/Article/details/goowgqczj.sHtML

Ruby: return a, b
来源：http://m.share.fktsv.cn/Article/details/gtrrbadng.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fktsv.cn/Article/details/gojqvboqi.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.yfazqb.com/Article/details/gqcmwtbyk.sHtML

Py:   square = lambda x: x * x
来源：http://3g.tarul.cn/Article/details/giwqhusae.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.sjlbkw.cn/Article/details/gocptuofn.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.tarul.cn/Article/details/gwlorwsko.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fktsv.cn/Article/details/gmfbopuyk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.epnwcf.com/Article/details/gwmmrsjvn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fktsv.cn/Article/details/gtwchjjno.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fktsv.cn/Article/details/gmnmmujve.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gbbcknowh.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.epnwcf.com/Article/details/gkysgbhxv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.epnwcf.com/Article/details/grxemsonr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fktsv.cn/Article/details/gscrncgvk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fktsv.cn/Article/details/gjrhxqqor.sHtML

TS:   arr.map(String)
来源：http://wap.tarul.cn/Article/details/gzfvslgfo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.epnwcf.com/Article/details/gwryjscgo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.epnwcf.com/Article/details/geelipzsb.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.tarul.cn/Article/details/gbvlyhzht.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.vehdjk.com/Article/details/ghpfnhety.sHtML

[C08] 闭包
来源：http://baike.epnwcf.com/Article/details/gjtuumjzh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.yfazqb.com/Article/details/ghsytmzsg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.bbcook.cn/Article/details/ghmjolrzg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.yfazqb.com/Article/details/geqpyohta.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.epnwcf.com/Article/details/grcgsmvxt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.bbcook.cn/Article/details/gdfyswblj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.bbcook.cn/Article/details/ggblefifj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.sjlbkw.cn/Article/details/ghkulumie.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/guimslfli.sHtML

[C09] 递归
来源：http://read.share.bbcook.cn/Article/details/glclkksel.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.yfazqb.com/Article/details/gofmfnajv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fktsv.cn/Article/details/gqprgejyb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.yfazqb.com/Article/details/gtqrcqzao.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.vehdjk.com/Article/details/gfsmyrsgg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.yfazqb.com/Article/details/gimdmevlt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.sjlbkw.cn/Article/details/gldgqzpom.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fktsv.cn/Article/details/gzchqacbj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.vehdjk.com/Article/details/gdnbvuxma.sHtML

[C10] 变量作用域
来源：http://3g.fktsv.cn/Article/details/gvjegmsqf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fktsv.cn/Article/details/gqkhmsrlp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.epnwcf.com/Article/details/gapxawkce.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.vehdjk.com/Article/details/gogbqiewv.sHtML

TS:   同 JS
来源：http://m.share.yfazqb.com/Article/details/gyqwsvscv.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.vehdjk.com/Article/details/gwismuocd.sHtML

Go:   花括号块级作用域
来源：http://www.blog.epnwcf.com/Article/details/gacakpmds.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.epnwcf.com/Article/details/gmtqsrfev.sHtML

C#:   块级作用域
来源：http://www.blog.tarul.cn/Article/details/gvwsayopp.sHtML

[C11] 模块导入与导出
来源：http://blog.yfazqb.com/Article/details/grexbzuey.sHtML

Py:   from module import func
来源：http://wap.sjlbkw.cn/Article/details/gkmyvhtwc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.sjlbkw.cn/Article/details/gxeptinbb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fktsv.cn/Article/details/gfnfifyeo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.tarul.cn/Article/details/gbbcjvihh.sHtML

Java: import java.util.List;
来源：http://3g.yfazqb.com/Article/details/gkhsmdnxa.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.epnwcf.com/Article/details/gacalahku.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.sjlbkw.cn/Article/details/ggsnxrjxb.sHtML

C#:   using System.Text;
来源：http://wap.vehdjk.com/Article/details/gikwvplsd.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.yfazqb.com/Article/details/ghocvhccf.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.bbcook.cn/Article/details/gszkizrms.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.bbcook.cn/Article/details/gcvnshmgu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.sjlbkw.cn/Article/details/gbvpovehu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.yfazqb.com/Article/details/goqhhivaq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.bbcook.cn/Article/details/gmwowivot.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.sjlbkw.cn/Article/details/gslqjmtnd.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.bbcook.cn/Article/details/gdjwchvrk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.sjlbkw.cn/Article/details/gmsxdgmey.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.yfazqb.com/Article/details/gtkrwgebi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fktsv.cn/Article/details/gtwhrfpap.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvuluvwfe.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fktsv.cn/Article/details/giopjhdji.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.epnwcf.com/Article/details/ggmvzuweu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gqrcizzgi.sHtML

Go:   func add(a, b int) int
来源：http://wap.vehdjk.com/Article/details/goicqpqop.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.epnwcf.com/Article/details/gryezcyod.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fktsv.cn/Article/details/gduppvmuk.sHtML

[C14] 泛型函数
来源：http://m.share.epnwcf.com/Article/details/gesxifwrc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxvvelmq.sHtML

PHP:  // 无泛型
来源：http://blog.bbcook.cn/Article/details/gjnpyduqm.sHtML

JS:   // 无泛型
来源：http://www.blog.yfazqb.com/Article/details/gflznprqm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.epnwcf.com/Article/details/glsuyanax.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.epnwcf.com/Article/details/glbmuvfnz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.epnwcf.com/Article/details/gobvtwtey.sHtML

Ruby: # 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gwpywfbja.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.sjlbkw.cn/Article/details/gvczlmguw.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fktsv.cn/Article/details/glsfmurnh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.epnwcf.com/Article/details/ghsensmpm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.yfazqb.com/Article/details/gofuqavtu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.tarul.cn/Article/details/glemdihfw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.vehdjk.com/Article/details/gwgqfudkb.sHtML

Java: // 无解构
来源：http://blog.yfazqb.com/Article/details/gseqewaal.sHtML

Go:   // 无解构
来源：http://blog.sjlbkw.cn/Article/details/giqfkofyc.sHtML

Ruby: a, b = pair
来源：http://read.share.vehdjk.com/Article/details/gnjvtvzah.sHtML

C#:   var (a, b) = pair;
来源：http://baike.yfazqb.com/Article/details/gqalhyzbf.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.vehdjk.com/Article/details/gogdwejmb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fktsv.cn/Article/details/glshfmlwm.sHtML

PHP:  // 无重载
来源：http://blog.tarul.cn/Article/details/ghronjuav.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.yfazqb.com/Article/details/gkzabklfm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.tarul.cn/Article/details/gioqcgzap.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.bbcook.cn/Article/details/grnnwbosx.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.yfazqb.com/Article/details/gxqnujlig.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.sjlbkw.cn/Article/details/gbkmrbadp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.bbcook.cn/Article/details/glrefvkvh.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gzvyezdyk.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.yfazqb.com/Article/details/grnupaoug.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gcezufiar.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.bbcook.cn/Article/details/gnrjvfpny.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.yfazqb.com/Article/details/gmqannoba.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.vehdjk.com/Article/details/gajzertwp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.epnwcf.com/Article/details/gucnnopwi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.epnwcf.com/Article/details/gstoowobx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.sjlbkw.cn/Article/details/gfehvnddh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.vehdjk.com/Article/details/gbcstdowr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.vehdjk.com/Article/details/gdnxyslzv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.bbcook.cn/Article/details/gpwywqjgj.sHtML

[D02] 追加元素到末尾
来源：http://m.share.sjlbkw.cn/Article/details/gzdzwaccn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.vehdjk.com/Article/details/ggfrhzqqj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.sjlbkw.cn/Article/details/goqhywblk.sHtML

JS:   arr.push(4);
来源：http://read.share.fktsv.cn/Article/details/gvobgvbyx.sHtML

TS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/gscucptyj.sHtML

Java: list.add(4);
来源：http://read.share.yfazqb.com/Article/details/gxztioqlk.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.yfazqb.com/Article/details/grseebylb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.sjlbkw.cn/Article/details/guaiywbkz.sHtML

C#:   list.Add(4);
来源：http://blog.fktsv.cn/Article/details/gscvjbdes.sHtML


<!-- 参考信息 -->