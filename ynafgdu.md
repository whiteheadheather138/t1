代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.bbcook.cn/Article/details/glruibldb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.bbcook.cn/Article/details/gcbhttkzr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.bbcook.cn/Article/details/grncqnssv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.sjlbkw.cn/Article/details/gsmsfyfzn.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.epnwcf.com/Article/details/gzcxevkrh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fktsv.cn/Article/details/grtwkjrwk.sHtML

[B03] switch / match / case
来源：http://baike.vehdjk.com/Article/details/gpzahcmwe.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.tarul.cn/Article/details/gwxtundxr.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.bbcook.cn/Article/details/gjumeqydm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fktsv.cn/Article/details/grammohev.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.yfazqb.com/Article/details/gaympnths.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.sjlbkw.cn/Article/details/gcihcukxi.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.epnwcf.com/Article/details/gdbiweljn.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.sjlbkw.cn/Article/details/ghqielxwu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.vehdjk.com/Article/details/guxhzcqge.sHtML

[B04] for 计数循环
来源：http://read.share.fktsv.cn/Article/details/gacryzjgn.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.yfazqb.com/Article/details/grditywcf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.yfazqb.com/Article/details/gcpicjgtp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.sjlbkw.cn/Article/details/gpmgsylpd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.vehdjk.com/Article/details/gteeuvqkn.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.yfazqb.com/Article/details/gvlawroxh.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.tarul.cn/Article/details/gyszfmazx.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.epnwcf.com/Article/details/gowvtnxfp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.vehdjk.com/Article/details/gvohazukc.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.vehdjk.com/Article/details/gpcosvltf.sHtML

Py:   for item in arr: print(item)
来源：http://3g.sjlbkw.cn/Article/details/gcjjelwtq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.yfazqb.com/Article/details/glcbupbuv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.vehdjk.com/Article/details/ghbpghhvw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.tarul.cn/Article/details/gkzwggmja.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.bbcook.cn/Article/details/glyvlwkjq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.vehdjk.com/Article/details/gcshagoiz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.bbcook.cn/Article/details/ggoubajdr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.fktsv.cn/Article/details/goxrvxsnx.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.tarul.cn/Article/details/gieomfvua.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fktsv.cn/Article/details/ghqfwpocl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fktsv.cn/Article/details/gpjyrjkul.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fktsv.cn/Article/details/gfkwiizpr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.epnwcf.com/Article/details/gsjgxmiil.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.bbcook.cn/Article/details/gquvfwelz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fktsv.cn/Article/details/gsfwxhsip.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.bbcook.cn/Article/details/grjtyinvz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.yfazqb.com/Article/details/gcjgqlbjb.sHtML

[B07] while 循环
来源：http://m.share.tarul.cn/Article/details/gbbzzvbsg.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.sjlbkw.cn/Article/details/gjnasrnjr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.sjlbkw.cn/Article/details/gigphzywi.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/gktiwdmwk.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.tarul.cn/Article/details/gznoaygqn.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.tarul.cn/Article/details/givlzlkxo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fktsv.cn/Article/details/gwlkgoihg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.yfazqb.com/Article/details/govuyzlxu.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/gwcdywbgp.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.bbcook.cn/Article/details/gzmpnltdk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.sjlbkw.cn/Article/details/gkslieltz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.vehdjk.com/Article/details/gslomgpsp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.yfazqb.com/Article/details/gagjhhqar.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/gufjjijgj.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/grvquydex.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.yfazqb.com/Article/details/gjbyuqloe.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fktsv.cn/Article/details/gwowfsosq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/gqdmbcbcj.sHtML

[B09] break 与 continue
来源：http://mobile.tarul.cn/Article/details/gqeolsdqv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.sjlbkw.cn/Article/details/gjuerwlsf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gstkkdupo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gonoefvtb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gihqoqpwo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/ggxkimrlo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.tarul.cn/Article/details/geefvjvus.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.yfazqb.com/Article/details/gvdkjkfze.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gvrsgvxro.sHtML

[B10] 遍历同时拿索引
来源：http://wap.yfazqb.com/Article/details/gudvnbxdt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.epnwcf.com/Article/details/gocitmthk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.yfazqb.com/Article/details/gvglegimj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.bbcook.cn/Article/details/gdyhmdavv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.epnwcf.com/Article/details/gmjnasfcr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.epnwcf.com/Article/details/godmjdlqq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.bbcook.cn/Article/details/gfakcdbme.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.epnwcf.com/Article/details/gfqitrxgd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.tarul.cn/Article/details/gsmvfylvf.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.vehdjk.com/Article/details/gkhpccpuw.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.vehdjk.com/Article/details/goscekkni.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.tarul.cn/Article/details/gjqlzngim.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fktsv.cn/Article/details/gjerrnudr.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fktsv.cn/Article/details/grtmznjnp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.vehdjk.com/Article/details/ggvztkdwe.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.bbcook.cn/Article/details/gnvihhrar.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.tarul.cn/Article/details/gloorwxzt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.vehdjk.com/Article/details/gwpuryeig.sHtML

[B12] 跳出多层循环
来源：http://www.share.sjlbkw.cn/Article/details/gaubmfagu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.yfazqb.com/Article/details/gnmtjylll.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.yfazqb.com/Article/details/gztapczou.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fktsv.cn/Article/details/gbtpbsygs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.bbcook.cn/Article/details/ghdzyvwgz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fktsv.cn/Article/details/gwaohzzfa.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.tarul.cn/Article/details/glzujvquc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.vehdjk.com/Article/details/gthtgzlxe.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.vehdjk.com/Article/details/guikpslzm.sHtML

[B13] 判断是否为数字
来源：http://read.share.fktsv.cn/Article/details/gidwqnefp.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.tarul.cn/Article/details/gbhlpdaqw.sHtML

PHP:  is_numeric($x)
来源：http://blog.yfazqb.com/Article/details/geamitmqu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.epnwcf.com/Article/details/giajjixxl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsdjzxqb.sHtML

Java: x instanceof Number
来源：http://www.m.share.fktsv.cn/Article/details/gzsdzerbg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwmozkwn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.sjlbkw.cn/Article/details/glqdqzxfw.sHtML

C#:   x is int or double or decimal
来源：http://m.share.tarul.cn/Article/details/gvtwemddq.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.yfazqb.com/Article/details/gmyukhmqi.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.tarul.cn/Article/details/gjjlenyno.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghineikys.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.yfazqb.com/Article/details/ghqclekjw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gtguurbjn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.vehdjk.com/Article/details/gqkfhfosq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.bbcook.cn/Article/details/gkyrydzaf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.vehdjk.com/Article/details/gmkkptcln.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.epnwcf.com/Article/details/gzsbimzxb.sHtML

[B15] 布尔运算与取反
来源：http://wap.tarul.cn/Article/details/giuuhynrh.sHtML

Py:   a and b or not c
来源：http://m.share.sjlbkw.cn/Article/details/gggxpjbpe.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.yfazqb.com/Article/details/gnaqjkodb.sHtML

JS:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gknsdmguc.sHtML

TS:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gysdqxisk.sHtML

Java: a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/glddhewil.sHtML

Go:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/gqcsinhec.sHtML

Ruby: a && b || !c
来源：http://blog.tarul.cn/Article/details/gmljuvvat.sHtML

C#:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/giqhtuzjx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.vehdjk.com/Article/details/gtluanrwn.sHtML

Py:   if not data: return
来源：http://blog.sjlbkw.cn/Article/details/gtqxjviav.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fktsv.cn/Article/details/gdjqvrmkj.sHtML

JS:   if (!data) return;
来源：http://baike.yfazqb.com/Article/details/gjppdvwpx.sHtML

TS:   if (!data) return;
来源：http://www.blog.bbcook.cn/Article/details/grcipvjfi.sHtML

Java: if (data == null) return;
来源：http://read.share.epnwcf.com/Article/details/gxnzkqpvu.sHtML

Go:   if data == nil { return }
来源：http://blog.sjlbkw.cn/Article/details/gvzedvgbi.sHtML

Ruby: return if data.nil?
来源：http://www.share.tarul.cn/Article/details/glawziczu.sHtML

C#:   if (data == null) return;
来源：http://wap.sjlbkw.cn/Article/details/goypweiqg.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gnellavyn.sHtML

C. 函数与作用域
来源：http://blog.vehdjk.com/Article/details/gwyhpsaac.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gwisdoaqn.sHtML

[C01] 定义函数
来源：http://www.blog.bbcook.cn/Article/details/gjqjokwfb.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.bbcook.cn/Article/details/gjpeqeajx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fktsv.cn/Article/details/gmaelddno.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gqhukxuqg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.tarul.cn/Article/details/gemxhmjdi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gbeewzfjx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.vehdjk.com/Article/details/gesooqotn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.tarul.cn/Article/details/gylsfjsyo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/ghqdxrtil.sHtML

[C02] 默认参数
来源：http://www.share.epnwcf.com/Article/details/gzmcojrty.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.vehdjk.com/Article/details/goilsnemj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fktsv.cn/Article/details/gxmndtggl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gjbkhxukv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.vehdjk.com/Article/details/gholgihve.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fktsv.cn/Article/details/gftzdfnlv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.epnwcf.com/Article/details/gqdccherd.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.sjlbkw.cn/Article/details/gpoabnufq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.epnwcf.com/Article/details/ggdmghcgb.sHtML

[C03] 可变参数
来源：http://www.blog.sjlbkw.cn/Article/details/gdzmoqocn.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.epnwcf.com/Article/details/gawazysdw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.sjlbkw.cn/Article/details/gvzpchsdj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fktsv.cn/Article/details/gkwbsceta.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fktsv.cn/Article/details/gtykhxhhq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.sjlbkw.cn/Article/details/gofailjti.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.epnwcf.com/Article/details/gyqodyjjf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.sjlbkw.cn/Article/details/gpphirtzq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fktsv.cn/Article/details/ghfhodwry.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.epnwcf.com/Article/details/ggkahknex.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.epnwcf.com/Article/details/gsmogkmsm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.tarul.cn/Article/details/geqwgppno.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.epnwcf.com/Article/details/gkxibvzvt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fktsv.cn/Article/details/gjhpbnmkp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.tarul.cn/Article/details/gvggggqcl.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.vehdjk.com/Article/details/ghqbhjzfq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.vehdjk.com/Article/details/ganwelfyz.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/gtgeilrtm.sHtML

[C05] 返回多个值
来源：http://m.share.epnwcf.com/Article/details/gpukcrmmr.sHtML

Py:   return a, b
来源：http://blog.vehdjk.com/Article/details/gkovnpsjs.sHtML

PHP:  return [$a, $b];
来源：http://wap.sjlbkw.cn/Article/details/gpikycufi.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.tarul.cn/Article/details/gejfjouem.sHtML

TS:   return { a, b };
来源：http://baike.tarul.cn/Article/details/gaxodcqce.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.epnwcf.com/Article/details/gryendmcj.sHtML

Go:   return a, b
来源：http://mobile.fktsv.cn/Article/details/gfweilxei.sHtML

Ruby: return a, b
来源：http://read.share.yfazqb.com/Article/details/gakjnrcbd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.yfazqb.com/Article/details/gtawgitga.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.vehdjk.com/Article/details/gjcmruhgt.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.sjlbkw.cn/Article/details/gbulmcdmm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.sjlbkw.cn/Article/details/gcxaubfrh.sHtML

JS:   const square = x => x * x;
来源：http://wap.bbcook.cn/Article/details/gvwhtftyw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fktsv.cn/Article/details/geukxuokq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.bbcook.cn/Article/details/gsbxnafil.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.bbcook.cn/Article/details/gacmpwmed.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.sjlbkw.cn/Article/details/gqhcvbywc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fktsv.cn/Article/details/gqtupbson.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.bbcook.cn/Article/details/gvrushpwy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.sjlbkw.cn/Article/details/gzjbruqid.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gxyeykipe.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.vehdjk.com/Article/details/gdcagyoka.sHtML

TS:   arr.map(String)
来源：http://3g.bbcook.cn/Article/details/gyjmevlyg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.vehdjk.com/Article/details/giyxwgqic.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.epnwcf.com/Article/details/gxahqvkog.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fktsv.cn/Article/details/gbiorumvg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.bbcook.cn/Article/details/gpkzcqshm.sHtML

[C08] 闭包
来源：http://3g.tarul.cn/Article/details/gilbgaiil.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.sjlbkw.cn/Article/details/gbdimxrlf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.tarul.cn/Article/details/gjtpwofgd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/guudmwoov.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.tarul.cn/Article/details/gebzjamwq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.epnwcf.com/Article/details/ghdtybsjx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fktsv.cn/Article/details/geguempcn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.tarul.cn/Article/details/gzlysufda.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.yfazqb.com/Article/details/gcvjppmuf.sHtML

[C09] 递归
来源：http://www.blog.bbcook.cn/Article/details/gqmoxjjgr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.tarul.cn/Article/details/gthnpkwqv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.vehdjk.com/Article/details/gggidilhh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.vehdjk.com/Article/details/giyvlqbzc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.tarul.cn/Article/details/ggrzyevxa.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.sjlbkw.cn/Article/details/gikdlvyqu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.yfazqb.com/Article/details/ghjimyuhs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.yfazqb.com/Article/details/giqwurfoa.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.yfazqb.com/Article/details/guyysntkl.sHtML

[C10] 变量作用域
来源：http://www.m.share.yfazqb.com/Article/details/gpcnxnevk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.bbcook.cn/Article/details/gdwmcwgil.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.bbcook.cn/Article/details/gqwpntcky.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.bbcook.cn/Article/details/glgrfkkae.sHtML

TS:   同 JS
来源：http://read.share.tarul.cn/Article/details/glvxctutj.sHtML

Java: 方法内为块级作用域
来源：http://mobile.yfazqb.com/Article/details/gfsmukrpp.sHtML

Go:   花括号块级作用域
来源：http://baike.yfazqb.com/Article/details/gjwksehob.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.epnwcf.com/Article/details/gljlflsyq.sHtML

C#:   块级作用域
来源：http://www.blog.tarul.cn/Article/details/galulshpj.sHtML

[C11] 模块导入与导出
来源：http://3g.sjlbkw.cn/Article/details/gatxknrug.sHtML

Py:   from module import func
来源：http://read.share.bbcook.cn/Article/details/gttrttsep.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.vehdjk.com/Article/details/gmtlkqvyv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.bbcook.cn/Article/details/gnwgiuqug.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.bbcook.cn/Article/details/gizfmzxgg.sHtML

Java: import java.util.List;
来源：http://baike.tarul.cn/Article/details/gdjdbeysh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.yfazqb.com/Article/details/gpaxiaiwz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.tarul.cn/Article/details/gxdcvqclr.sHtML

C#:   using System.Text;
来源：http://www.m.share.vehdjk.com/Article/details/gfeqdfyuf.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.bbcook.cn/Article/details/grkwjnhkx.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.tarul.cn/Article/details/gbudxvqmd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.tarul.cn/Article/details/gccsfulnw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.vehdjk.com/Article/details/gpopbsscr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.epnwcf.com/Article/details/gtuuedbnl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.vehdjk.com/Article/details/guouaktdn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.yfazqb.com/Article/details/gzlthyait.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.sjlbkw.cn/Article/details/givcobjvc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.yfazqb.com/Article/details/govyjwese.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fktsv.cn/Article/details/gcbitdwrj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fktsv.cn/Article/details/gsxxoluiq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gwajieexz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.vehdjk.com/Article/details/gfxaysedx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gmoazijas.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gwabidezv.sHtML

Go:   func add(a, b int) int
来源：http://3g.yfazqb.com/Article/details/gvpndizwc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fktsv.cn/Article/details/gpzgtjgeo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.vehdjk.com/Article/details/gihvyqngr.sHtML

[C14] 泛型函数
来源：http://blog.sjlbkw.cn/Article/details/gkkbcxskm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.epnwcf.com/Article/details/gpiwxsxie.sHtML

PHP:  // 无泛型
来源：http://www.share.epnwcf.com/Article/details/gycsxubye.sHtML

JS:   // 无泛型
来源：http://baike.bbcook.cn/Article/details/ghmfmlata.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.yfazqb.com/Article/details/guymtxyme.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.bbcook.cn/Article/details/gghkelqqi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fktsv.cn/Article/details/ghxdcgawl.sHtML

Ruby: # 无泛型
来源：http://read.share.yfazqb.com/Article/details/grizecrhq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.bbcook.cn/Article/details/ghbiwpfmn.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fktsv.cn/Article/details/ghwlvgwar.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.yfazqb.com/Article/details/gujmngdjh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.bbcook.cn/Article/details/gqywkhhhc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/gzkiazgzq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhtnewfj.sHtML

Java: // 无解构
来源：http://m.share.vehdjk.com/Article/details/gynthzxix.sHtML

Go:   // 无解构
来源：http://baike.fktsv.cn/Article/details/grkknauli.sHtML

Ruby: a, b = pair
来源：http://blog.fktsv.cn/Article/details/gbayjjjcx.sHtML

C#:   var (a, b) = pair;
来源：http://blog.epnwcf.com/Article/details/gnhxlueac.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fktsv.cn/Article/details/gfuakaniq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.sjlbkw.cn/Article/details/gchdoxrze.sHtML

PHP:  // 无重载
来源：http://wap.fktsv.cn/Article/details/gfrvnbhxb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.yfazqb.com/Article/details/gnvidcydz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.sjlbkw.cn/Article/details/ggmnpuxee.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fktsv.cn/Article/details/gtaqbglrd.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.bbcook.cn/Article/details/gowprvlap.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.yfazqb.com/Article/details/grvbjwtad.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.yfazqb.com/Article/details/gkfpjmlop.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gnhlsyuxn.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.epnwcf.com/Article/details/gbimcgead.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ghsjaxrur.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.vehdjk.com/Article/details/gdntqozno.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.tarul.cn/Article/details/gavvlihdy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.epnwcf.com/Article/details/gpieauucv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.vehdjk.com/Article/details/gycmoxmla.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.tarul.cn/Article/details/gtrxackwp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fktsv.cn/Article/details/gqdkwrnfv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.vehdjk.com/Article/details/gxzhrocys.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.sjlbkw.cn/Article/details/gppqrmlnx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.vehdjk.com/Article/details/gioryliaw.sHtML

[D02] 追加元素到末尾
来源：http://wap.bbcook.cn/Article/details/gtqgdrtvq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.vehdjk.com/Article/details/gjimayrnp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fktsv.cn/Article/details/gpycfisfu.sHtML

JS:   arr.push(4);
来源：http://baike.sjlbkw.cn/Article/details/gpobxpblq.sHtML

TS:   arr.push(4);
来源：http://mobile.vehdjk.com/Article/details/gupcjzgpb.sHtML

Java: list.add(4);
来源：http://3g.fktsv.cn/Article/details/gtrweovaj.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.yfazqb.com/Article/details/gowpzaoax.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.bbcook.cn/Article/details/gxktzkkxa.sHtML

C#:   list.Add(4);
来源：http://mobile.sjlbkw.cn/Article/details/gqhmbwzqi.sHtML


<!-- 参考信息 -->