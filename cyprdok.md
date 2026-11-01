代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.sjlbkw.cn/Article/details/gemkynqjy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fktsv.cn/Article/details/gaoajmydj.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.epnwcf.com/Article/details/gbsrkevsr.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fktsv.cn/Article/details/gaqiiguyq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.vehdjk.com/Article/details/gebuzobin.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.bbcook.cn/Article/details/gpoehjssm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.vehdjk.com/Article/details/gwcxryppc.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.epnwcf.com/Article/details/gtyzbhiim.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fktsv.cn/Article/details/gtlegcjjd.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.yfazqb.com/Article/details/gsolfthlu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.bbcook.cn/Article/details/gewukkuci.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.vehdjk.com/Article/details/giloxefqs.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.vehdjk.com/Article/details/gsqasomvu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.yfazqb.com/Article/details/gkstahdil.sHtML

[B07] while 循环
来源：http://m.share.tarul.cn/Article/details/gksndktum.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.yfazqb.com/Article/details/gthjhnigl.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fktsv.cn/Article/details/gjlxcaotv.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgsbmkvq.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.tarul.cn/Article/details/gtispotgt.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gykwecslk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.bbcook.cn/Article/details/gcgnhsxwa.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.epnwcf.com/Article/details/ghyobmhqk.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/gbiafvqiq.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.vehdjk.com/Article/details/gvrugprgu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.bbcook.cn/Article/details/gmslafwxx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.epnwcf.com/Article/details/galksbzxj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/geuayiobf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/ggallnqvw.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/genqolzsx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.vehdjk.com/Article/details/gzontuuvj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.vehdjk.com/Article/details/gioyrjots.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/gbyuologu.sHtML

[B09] break 与 continue
来源：http://blog.fktsv.cn/Article/details/gtuaavjyz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.sjlbkw.cn/Article/details/gaqfselme.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/gjmyqdytd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gjapiyept.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gkudnzxsb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gstzqukrj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.bbcook.cn/Article/details/gufbjyxrw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.vehdjk.com/Article/details/glmaxcmms.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.tarul.cn/Article/details/gglsjzqrm.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.epnwcf.com/Article/details/gwaaungnu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.yfazqb.com/Article/details/gkjhgswws.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.bbcook.cn/Article/details/gxfcmvray.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.tarul.cn/Article/details/gxirjmews.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.bbcook.cn/Article/details/gwovfxorh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fktsv.cn/Article/details/grfgkzpii.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fktsv.cn/Article/details/gwhzrgwkh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.bbcook.cn/Article/details/giaqquuto.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.tarul.cn/Article/details/gppfeucvm.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fktsv.cn/Article/details/gchyfvgaq.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fktsv.cn/Article/details/gwjbuxitp.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.vehdjk.com/Article/details/gtmjqvmmz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.tarul.cn/Article/details/gocoiglpf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.epnwcf.com/Article/details/gnpnidirl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.tarul.cn/Article/details/guuxjqjyz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fktsv.cn/Article/details/ghmjrcuco.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.epnwcf.com/Article/details/ghagmlxeh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.yfazqb.com/Article/details/gpkviedtq.sHtML

[B12] 跳出多层循环
来源：http://baike.fktsv.cn/Article/details/gnehlmpou.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.vehdjk.com/Article/details/gwbmcadqe.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.epnwcf.com/Article/details/guiprjjwl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.yfazqb.com/Article/details/gukscowir.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/giojpkkxb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.yfazqb.com/Article/details/gqgziojlo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fktsv.cn/Article/details/gltkniwhm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fktsv.cn/Article/details/ggiwmnjqs.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.sjlbkw.cn/Article/details/gktdekfyp.sHtML

[B13] 判断是否为数字
来源：http://3g.bbcook.cn/Article/details/ggysjkdzd.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.yfazqb.com/Article/details/gjpyxgysd.sHtML

PHP:  is_numeric($x)
来源：http://mobile.epnwcf.com/Article/details/gzesdpvev.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.yfazqb.com/Article/details/gtvymfkgk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fktsv.cn/Article/details/gsdxqbajg.sHtML

Java: x instanceof Number
来源：http://www.share.yfazqb.com/Article/details/gnbuvwuht.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fktsv.cn/Article/details/gsykvzwab.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fktsv.cn/Article/details/gdcmhswxd.sHtML

C#:   x is int or double or decimal
来源：http://wap.tarul.cn/Article/details/goziqzakn.sHtML

[B14] 判断值是否在集合内
来源：http://3g.yfazqb.com/Article/details/gsprwmiye.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.sjlbkw.cn/Article/details/gxqircszt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.vehdjk.com/Article/details/gbcgrhkpu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/gemydndiq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.yfazqb.com/Article/details/gwktdpjwf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.bbcook.cn/Article/details/gocuufvgr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.bbcook.cn/Article/details/gvzjlxudq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.tarul.cn/Article/details/gndhhfsjf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fktsv.cn/Article/details/gqbsndzwd.sHtML

[B15] 布尔运算与取反
来源：http://baike.sjlbkw.cn/Article/details/gtitexqhw.sHtML

Py:   a and b or not c
来源：http://wap.vehdjk.com/Article/details/gmbtzlsrx.sHtML

PHP:  $a && $b || !$c
来源：http://blog.tarul.cn/Article/details/ghconnspm.sHtML

JS:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/guejtfyle.sHtML

TS:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/ggyupddqj.sHtML

Java: a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gnojgnqpq.sHtML

Go:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gkkryelrv.sHtML

Ruby: a && b || !c
来源：http://3g.epnwcf.com/Article/details/gsnulpndy.sHtML

C#:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gsnkyfkxd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.sjlbkw.cn/Article/details/gdwqldhzj.sHtML

Py:   if not data: return
来源：http://blog.tarul.cn/Article/details/gmbvkfwgh.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.epnwcf.com/Article/details/glfpboeco.sHtML

JS:   if (!data) return;
来源：http://mobile.yfazqb.com/Article/details/gjnptxcst.sHtML

TS:   if (!data) return;
来源：http://wap.epnwcf.com/Article/details/gefuzfmow.sHtML

Java: if (data == null) return;
来源：http://baike.vehdjk.com/Article/details/ggcxmjtvn.sHtML

Go:   if data == nil { return }
来源：http://baike.fktsv.cn/Article/details/gzrvyayyv.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fktsv.cn/Article/details/gttyrlnvj.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.epnwcf.com/Article/details/gngfaqxjm.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gydpkjgkl.sHtML

C. 函数与作用域
来源：http://blog.epnwcf.com/Article/details/gryemyccv.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gtyvvmaam.sHtML

[C01] 定义函数
来源：http://www.m.share.fktsv.cn/Article/details/grnxnsxch.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.bbcook.cn/Article/details/gobsyzjno.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gdayapgbl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gqaguczms.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.tarul.cn/Article/details/gzvlxxhkl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/grebpgjrk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.bbcook.cn/Article/details/gnziuwylv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.sjlbkw.cn/Article/details/gthclswts.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gmuainpja.sHtML

[C02] 默认参数
来源：http://blog.vehdjk.com/Article/details/giratmsaq.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.vehdjk.com/Article/details/gwpzrdffx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.vehdjk.com/Article/details/gafutbnlo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gxfhyarxn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.yfazqb.com/Article/details/gnlyndjgn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.sjlbkw.cn/Article/details/goldlxsmv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fktsv.cn/Article/details/gsavjcrlw.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.sjlbkw.cn/Article/details/gizczslvf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.tarul.cn/Article/details/gqselgsll.sHtML

[C03] 可变参数
来源：http://m.share.yfazqb.com/Article/details/ggqudebxw.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.sjlbkw.cn/Article/details/gxdeicmyu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.sjlbkw.cn/Article/details/geztuzevn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.epnwcf.com/Article/details/gcazzxpib.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.vehdjk.com/Article/details/gltpqmtry.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.bbcook.cn/Article/details/gtsfrnqzg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fktsv.cn/Article/details/gsogwtysl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.vehdjk.com/Article/details/gxkgzyamm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.sjlbkw.cn/Article/details/gqcwtrfdh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.yfazqb.com/Article/details/gmghothbi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fktsv.cn/Article/details/gjwihwfan.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.epnwcf.com/Article/details/gecymdcru.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.bbcook.cn/Article/details/gdoohefyy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.tarul.cn/Article/details/gagsiguiq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fktsv.cn/Article/details/gheneyhnx.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.vehdjk.com/Article/details/gbjngraux.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.bbcook.cn/Article/details/gkkevealr.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/gcevqehbt.sHtML

[C05] 返回多个值
来源：http://baike.tarul.cn/Article/details/gfvcojpjl.sHtML

Py:   return a, b
来源：http://wap.fktsv.cn/Article/details/gqqlekbqm.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.bbcook.cn/Article/details/gddpflzbl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.sjlbkw.cn/Article/details/gdatpschn.sHtML

TS:   return { a, b };
来源：http://baike.fktsv.cn/Article/details/gntuqyjrq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.yfazqb.com/Article/details/grhoxickr.sHtML

Go:   return a, b
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfjgkqdd.sHtML

Ruby: return a, b
来源：http://mobile.epnwcf.com/Article/details/gvvaoblvu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.tarul.cn/Article/details/glkkdqhfg.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.epnwcf.com/Article/details/gitpbmfqf.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.bbcook.cn/Article/details/guqwluxuq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.vehdjk.com/Article/details/gesugdiyl.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gpcagksea.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fktsv.cn/Article/details/gtlhulccb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fktsv.cn/Article/details/gpalrgglg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.tarul.cn/Article/details/gtemztedg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.sjlbkw.cn/Article/details/gcvdrmkoc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.bbcook.cn/Article/details/gmjvwrsux.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.vehdjk.com/Article/details/giufdoyei.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.vehdjk.com/Article/details/gwxuytgxe.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.sjlbkw.cn/Article/details/gqbvopgac.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.epnwcf.com/Article/details/gxqaaicys.sHtML

TS:   arr.map(String)
来源：http://wap.epnwcf.com/Article/details/glxuncczi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.tarul.cn/Article/details/gpgsbidhc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.tarul.cn/Article/details/glzmcgbuy.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.sjlbkw.cn/Article/details/gebqclrue.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fktsv.cn/Article/details/gkollcqfr.sHtML

[C08] 闭包
来源：http://blog.sjlbkw.cn/Article/details/gyuhffepv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.tarul.cn/Article/details/ghdydxsyt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.bbcook.cn/Article/details/gbijmaago.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fktsv.cn/Article/details/gbpniwudn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fktsv.cn/Article/details/gxroenwrk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.sjlbkw.cn/Article/details/gohkfabpb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fktsv.cn/Article/details/gaxhbiwop.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.sjlbkw.cn/Article/details/goqojirxr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.yfazqb.com/Article/details/gzoseulbc.sHtML

[C09] 递归
来源：http://blog.tarul.cn/Article/details/gqdyoazxi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/gwsgvzlrf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.tarul.cn/Article/details/gtimwazxg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.sjlbkw.cn/Article/details/gehyuljwj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.yfazqb.com/Article/details/ggogpyaja.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.epnwcf.com/Article/details/gfokzvbni.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.bbcook.cn/Article/details/ghikohpya.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gpvaqjewf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.sjlbkw.cn/Article/details/grcmxwhee.sHtML

[C10] 变量作用域
来源：http://3g.bbcook.cn/Article/details/gglrngsla.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.epnwcf.com/Article/details/gzwpspsil.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.bbcook.cn/Article/details/gpzrurjqv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.tarul.cn/Article/details/gnexbcloz.sHtML

TS:   同 JS
来源：http://mobile.bbcook.cn/Article/details/ggdcqdaka.sHtML

Java: 方法内为块级作用域
来源：http://m.share.bbcook.cn/Article/details/grlbxfmbn.sHtML

Go:   花括号块级作用域
来源：http://blog.bbcook.cn/Article/details/gztniivll.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.bbcook.cn/Article/details/gszjtlvnd.sHtML

C#:   块级作用域
来源：http://baike.vehdjk.com/Article/details/guqdlbrpb.sHtML

[C11] 模块导入与导出
来源：http://www.share.yfazqb.com/Article/details/gobojrtkf.sHtML

Py:   from module import func
来源：http://wap.bbcook.cn/Article/details/gqhjkysqo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.vehdjk.com/Article/details/gytyjglhb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.yfazqb.com/Article/details/geosmpweh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.vehdjk.com/Article/details/gucdwrzex.sHtML

Java: import java.util.List;
来源：http://blog.sjlbkw.cn/Article/details/gzmuixxoo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.vehdjk.com/Article/details/gklpjbfmo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.tarul.cn/Article/details/gdqbbitti.sHtML

C#:   using System.Text;
来源：http://www.blog.fktsv.cn/Article/details/gzxmqbcuz.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.bbcook.cn/Article/details/gfqwphtgh.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fktsv.cn/Article/details/gafcqpihe.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.epnwcf.com/Article/details/gteocpvwp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fktsv.cn/Article/details/gpgostcjs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.yfazqb.com/Article/details/gegbdzrfd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fktsv.cn/Article/details/gresxhjit.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.bbcook.cn/Article/details/gmchnyybf.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.vehdjk.com/Article/details/grmqxyjpe.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fktsv.cn/Article/details/gyswtqmwj.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.vehdjk.com/Article/details/gfykubkow.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.tarul.cn/Article/details/gutspkynd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/ghxtsomkm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fktsv.cn/Article/details/gbrupfkyw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gbsxbtdgl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gjjawhmsm.sHtML

Go:   func add(a, b int) int
来源：http://read.share.sjlbkw.cn/Article/details/gcygozubn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.bbcook.cn/Article/details/gpmsmnysh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.vehdjk.com/Article/details/gprieecvg.sHtML

[C14] 泛型函数
来源：http://baike.fktsv.cn/Article/details/gwfsmnaiw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fktsv.cn/Article/details/gvflbhzbk.sHtML

PHP:  // 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gmeojiyrk.sHtML

JS:   // 无泛型
来源：http://3g.fktsv.cn/Article/details/ghmueepal.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.epnwcf.com/Article/details/giokaofwr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.vehdjk.com/Article/details/gfmrforau.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.tarul.cn/Article/details/gtmuzgjmv.sHtML

Ruby: # 无泛型
来源：http://3g.vehdjk.com/Article/details/gkyczoiaf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.epnwcf.com/Article/details/gdcfdituz.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.sjlbkw.cn/Article/details/gzujlcuxo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.yfazqb.com/Article/details/gjxumwjrb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.vehdjk.com/Article/details/grvbkmxte.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.tarul.cn/Article/details/gzniorype.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.bbcook.cn/Article/details/ggdzbqobq.sHtML

Java: // 无解构
来源：http://read.share.tarul.cn/Article/details/gbdmsltwo.sHtML

Go:   // 无解构
来源：http://www.m.share.tarul.cn/Article/details/gpusxgspx.sHtML

Ruby: a, b = pair
来源：http://read.share.yfazqb.com/Article/details/gfyobbjvz.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdqjvrrn.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fktsv.cn/Article/details/gwghuzbmc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.yfazqb.com/Article/details/gbxatbjqq.sHtML

PHP:  // 无重载
来源：http://m.share.fktsv.cn/Article/details/gapqhyqps.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.yfazqb.com/Article/details/gvdbsampg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.vehdjk.com/Article/details/gtgtbgecg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.epnwcf.com/Article/details/gvgjzelfd.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.sjlbkw.cn/Article/details/gffwuyoaa.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.bbcook.cn/Article/details/gaupqstgj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.tarul.cn/Article/details/glrddjnys.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gzlkobkdt.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fktsv.cn/Article/details/ghwnwzkga.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gewjollxb.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.tarul.cn/Article/details/gocwytwyq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.bbcook.cn/Article/details/ggiozawkx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.bbcook.cn/Article/details/gknnsytwb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.tarul.cn/Article/details/gqoynvvdb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.yfazqb.com/Article/details/geuojzjwd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.bbcook.cn/Article/details/gpxzdbsij.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.yfazqb.com/Article/details/goopctftr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.vehdjk.com/Article/details/gpbcuejoh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.epnwcf.com/Article/details/geirvhgys.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fktsv.cn/Article/details/gmumbabes.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.yfazqb.com/Article/details/gktluitcg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.bbcook.cn/Article/details/ghrwsfgfa.sHtML

JS:   arr.push(4);
来源：http://www.blog.epnwcf.com/Article/details/gyvajkerv.sHtML

TS:   arr.push(4);
来源：http://www.m.share.vehdjk.com/Article/details/ghgydlyea.sHtML

Java: list.add(4);
来源：http://wap.vehdjk.com/Article/details/gfnexlpaw.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.epnwcf.com/Article/details/gkkktpsrl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fktsv.cn/Article/details/gaikbhpho.sHtML

C#:   list.Add(4);
来源：http://www.share.epnwcf.com/Article/details/gwtjsypnb.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fktsv.cn/Article/details/gcbflqchs.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.epnwcf.com/Article/details/gchhryloj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.vehdjk.com/Article/details/gzxqaicet.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.epnwcf.com/Article/details/gxrjqmcje.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.epnwcf.com/Article/details/gnvflvgjd.sHtML

Java: list.add(0, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gflpovpiz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.sjlbkw.cn/Article/details/gytlhbhxd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.bbcook.cn/Article/details/gfawkddeo.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.yfazqb.com/Article/details/gwtrvbbrm.sHtML

[D04] 删除元素
来源：http://read.share.sjlbkw.cn/Article/details/gbterfcvr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.sjlbkw.cn/Article/details/gziwmtven.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.tarul.cn/Article/details/grudgoivr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.yfazqb.com/Article/details/gqyxopjcg.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.yfazqb.com/Article/details/gljfrhcph.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.bbcook.cn/Article/details/gskpojvzn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.bbcook.cn/Article/details/gmimffoze.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnitoinzd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.sjlbkw.cn/Article/details/gbfaqiwvm.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fktsv.cn/Article/details/glzfuvgaf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/gokbjmiib.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.sjlbkw.cn/Article/details/gujlgiosg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.epnwcf.com/Article/details/gtpiuenbf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.bbcook.cn/Article/details/gtoagcmls.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.yfazqb.com/Article/details/grusmoipz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/gysmmgdkf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fktsv.cn/Article/details/glpxfvqds.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gkdjujibm.sHtML

[D06] 数组长度
来源：http://wap.fktsv.cn/Article/details/gfigtjcts.sHtML


<!-- 参考信息 -->