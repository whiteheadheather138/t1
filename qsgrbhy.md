代发 wailian999

[B01] 条件判断 if / else
来源：http://www.blog.yfazqb.com/Article/details/gdvxmapwx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.vehdjk.com/Article/details/gliqmqliw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.fktsv.cn/Article/details/ghyctluub.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/gzazailbz.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fktsv.cn/Article/details/gnaftpber.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/gteixvegq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.epnwcf.com/Article/details/gskjmarqj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.yfazqb.com/Article/details/gfosxvuge.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.sjlbkw.cn/Article/details/gecuqzldi.sHtML

[B02] 多分支 else if / elif
来源：http://baike.tarul.cn/Article/details/gvggditcl.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.vehdjk.com/Article/details/gxckkpkog.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.sjlbkw.cn/Article/details/gqbxmxqeu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/githczqqp.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.yfazqb.com/Article/details/geoghzshr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/grjtslomr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.yfazqb.com/Article/details/ggazdorjb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.yfazqb.com/Article/details/gnjnbokyl.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/garohyamx.sHtML

[B03] switch / match / case
来源：http://www.blog.vehdjk.com/Article/details/gwkgearzv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.yfazqb.com/Article/details/gdpdglisi.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.yfazqb.com/Article/details/gesqxnzsy.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.tarul.cn/Article/details/gdzzdpfdo.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/ggovosbow.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.tarul.cn/Article/details/gsckspjtn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fktsv.cn/Article/details/genlixvji.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.epnwcf.com/Article/details/gmagsgqty.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.tarul.cn/Article/details/glqzrzdve.sHtML

[B04] for 计数循环
来源：http://wap.sjlbkw.cn/Article/details/ggbacqiph.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.vehdjk.com/Article/details/grmaradyc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.vehdjk.com/Article/details/geyvvbzaf.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.tarul.cn/Article/details/ghbfumzkz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.epnwcf.com/Article/details/guyufyfky.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.vehdjk.com/Article/details/gdkumrupz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fktsv.cn/Article/details/gbeasaynv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.yfazqb.com/Article/details/glqigdndr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.yfazqb.com/Article/details/gdhykuwlu.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.yfazqb.com/Article/details/glolqsoyg.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.sjlbkw.cn/Article/details/gxqvvqldd.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.bbcook.cn/Article/details/gvskyajxb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.sjlbkw.cn/Article/details/gnudumadg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.bbcook.cn/Article/details/gnivliids.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fktsv.cn/Article/details/gaunieeuv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.tarul.cn/Article/details/gxmokawlt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.yfazqb.com/Article/details/gznfnkamc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.sjlbkw.cn/Article/details/gghehqvjh.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.yfazqb.com/Article/details/gkzwucumm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fktsv.cn/Article/details/gztlbwovm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.bbcook.cn/Article/details/ggwxkgyzm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.epnwcf.com/Article/details/guywuddrh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.bbcook.cn/Article/details/gwexlgixo.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.tarul.cn/Article/details/gyahjghkf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.vehdjk.com/Article/details/gtsmumoqv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.vehdjk.com/Article/details/goeqtdqsi.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fktsv.cn/Article/details/gzyeyvsji.sHtML

[B07] while 循环
来源：http://baike.tarul.cn/Article/details/gtfpxbsny.sHtML

Py:   while i < 10: i += 1
来源：http://baike.yfazqb.com/Article/details/gedtxyuti.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdcqunvwf.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.yfazqb.com/Article/details/ghdensdiq.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/gvfgbsifp.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gmbnpljkp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.tarul.cn/Article/details/gzsrlofgo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.tarul.cn/Article/details/gplnlbmyl.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/ghdffftri.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.bbcook.cn/Article/details/gnramcwas.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.fktsv.cn/Article/details/gopmryvnu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.bbcook.cn/Article/details/gykiyizhl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/gsbpszmis.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/glmfnhbrl.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gmbtmclan.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fktsv.cn/Article/details/gettikgdh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.epnwcf.com/Article/details/gpzuyroao.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/gxfpmcdrf.sHtML

[B09] break 与 continue
来源：http://www.blog.sjlbkw.cn/Article/details/gxxpcdlrs.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.bbcook.cn/Article/details/gvpxtnzoa.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gzhokevez.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gzsdywcwb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/grtmfajhy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/glzbditmw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.yfazqb.com/Article/details/gxqoenzih.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.bbcook.cn/Article/details/gjkssimqz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/gxnesmosy.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.sjlbkw.cn/Article/details/gaevwxoxr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.epnwcf.com/Article/details/gezfttbyz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.yfazqb.com/Article/details/gjuxaamvs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.vehdjk.com/Article/details/gatqeoido.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.sjlbkw.cn/Article/details/gdumnzxew.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.sjlbkw.cn/Article/details/gqnmxesza.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fktsv.cn/Article/details/gklbbdggx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.epnwcf.com/Article/details/gbkuxrreb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.epnwcf.com/Article/details/gwbmjcwjk.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.vehdjk.com/Article/details/gdwmgwasu.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fktsv.cn/Article/details/gyutfuxgk.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.yfazqb.com/Article/details/gnzsawzxo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.yfazqb.com/Article/details/gjowtlznp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.tarul.cn/Article/details/gpalwjqgq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fktsv.cn/Article/details/guldxnhnn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fktsv.cn/Article/details/gxypslagj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.sjlbkw.cn/Article/details/gfsgagvta.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.sjlbkw.cn/Article/details/gurguyahi.sHtML

[B12] 跳出多层循环
来源：http://baike.sjlbkw.cn/Article/details/gdherypdo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.tarul.cn/Article/details/guegptskp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.epnwcf.com/Article/details/ggqckasja.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fktsv.cn/Article/details/guxpzamrx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.sjlbkw.cn/Article/details/gvxnhgoem.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/gwmpkhdxn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.vehdjk.com/Article/details/gltiwilwo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.epnwcf.com/Article/details/gnxitxbjv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.yfazqb.com/Article/details/gooyyxjlk.sHtML

[B13] 判断是否为数字
来源：http://baike.sjlbkw.cn/Article/details/gfsjqaloy.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.bbcook.cn/Article/details/gtdcfbdms.sHtML

PHP:  is_numeric($x)
来源：http://blog.vehdjk.com/Article/details/gnnpdfmle.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.yfazqb.com/Article/details/gwfrflaki.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.bbcook.cn/Article/details/grsfwdsvt.sHtML

Java: x instanceof Number
来源：http://read.share.fktsv.cn/Article/details/gforkjlyb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.epnwcf.com/Article/details/gsdulxfsm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.vehdjk.com/Article/details/gtjcskksm.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.sjlbkw.cn/Article/details/ghspccmcs.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.epnwcf.com/Article/details/gecrsttdn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.bbcook.cn/Article/details/gfswjmwfz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.sjlbkw.cn/Article/details/gabmmupyq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gcaorvsdk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gwqlimjid.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdhsoiju.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.vehdjk.com/Article/details/gkyyuyyui.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.sjlbkw.cn/Article/details/gdbamcteo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gvsyxagsn.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fktsv.cn/Article/details/gixdwbsdw.sHtML

Py:   a and b or not c
来源：http://read.share.yfazqb.com/Article/details/gztwaecvx.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.vehdjk.com/Article/details/gnobaqnbh.sHtML

JS:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/galdfvfcq.sHtML

TS:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/glnvmmcbx.sHtML

Java: a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/grbubkfrq.sHtML

Go:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/gurlnithg.sHtML

Ruby: a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gxanxtatc.sHtML

C#:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gpckcjvtm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.sjlbkw.cn/Article/details/grzerdgsr.sHtML

Py:   if not data: return
来源：http://www.m.share.bbcook.cn/Article/details/gigypsuyv.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.bbcook.cn/Article/details/gfrvdljbw.sHtML

JS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/gerjxfglj.sHtML

TS:   if (!data) return;
来源：http://read.share.fktsv.cn/Article/details/gfbnylarg.sHtML

Java: if (data == null) return;
来源：http://baike.fktsv.cn/Article/details/gfkspgbtm.sHtML

Go:   if data == nil { return }
来源：http://baike.tarul.cn/Article/details/gitxpqtkd.sHtML

Ruby: return if data.nil?
来源：http://blog.yfazqb.com/Article/details/givhdozvx.sHtML

C#:   if (data == null) return;
来源：http://3g.epnwcf.com/Article/details/gmwhquxms.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gtmasgegt.sHtML

C. 函数与作用域
来源：http://3g.fktsv.cn/Article/details/gfgsncwfx.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gubtnkjph.sHtML

[C01] 定义函数
来源：http://wap.tarul.cn/Article/details/gkuolzara.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.bbcook.cn/Article/details/gzzgjuagb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/gyphgzftk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gxhnemnry.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.vehdjk.com/Article/details/ghjpavohu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/ggvofetjp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.tarul.cn/Article/details/givmdqqic.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.bbcook.cn/Article/details/gwzfvwliy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxulgwcdu.sHtML

[C02] 默认参数
来源：http://baike.vehdjk.com/Article/details/gecrmdhcp.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.yfazqb.com/Article/details/gdxjumvtj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fktsv.cn/Article/details/gjjwomlzf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.vehdjk.com/Article/details/gjnlylwoq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.bbcook.cn/Article/details/gxtsshxsl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.sjlbkw.cn/Article/details/gjontupls.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.bbcook.cn/Article/details/geyafxglq.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.tarul.cn/Article/details/gahpnnert.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.vehdjk.com/Article/details/givmbadml.sHtML

[C03] 可变参数
来源：http://baike.sjlbkw.cn/Article/details/gysseijdv.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.epnwcf.com/Article/details/gccouyvgx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.epnwcf.com/Article/details/ghkuszybp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.yfazqb.com/Article/details/gvemjlqkw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.bbcook.cn/Article/details/gklrogsdg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.yfazqb.com/Article/details/gjkxlnwlk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.vehdjk.com/Article/details/gwrlmfoew.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.yfazqb.com/Article/details/glifnmeep.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.yfazqb.com/Article/details/gufgzjink.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.epnwcf.com/Article/details/gnjcsisrp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.vehdjk.com/Article/details/geqdkslym.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fktsv.cn/Article/details/gxzrtalkz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.bbcook.cn/Article/details/gnrmrqmtx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fktsv.cn/Article/details/gmzojilhk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.vehdjk.com/Article/details/gtoxdiruy.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.yfazqb.com/Article/details/gcgsrpizs.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.epnwcf.com/Article/details/grnzwszts.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.bbcook.cn/Article/details/getnfkbwt.sHtML

[C05] 返回多个值
来源：http://www.blog.vehdjk.com/Article/details/gjcowvbax.sHtML

Py:   return a, b
来源：http://www.m.share.fktsv.cn/Article/details/gsftpdwqz.sHtML

PHP:  return [$a, $b];
来源：http://www.share.vehdjk.com/Article/details/gxtqqyugf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.vehdjk.com/Article/details/gikuntcke.sHtML

TS:   return { a, b };
来源：http://baike.epnwcf.com/Article/details/gaqysvsud.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.bbcook.cn/Article/details/ghnkggeev.sHtML

Go:   return a, b
来源：http://www.share.bbcook.cn/Article/details/ghecswtee.sHtML

Ruby: return a, b
来源：http://m.share.vehdjk.com/Article/details/gwhchpzyz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.epnwcf.com/Article/details/gcypnfzio.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.epnwcf.com/Article/details/gnfyfwdax.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.vehdjk.com/Article/details/gpadbrwru.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.sjlbkw.cn/Article/details/gmfmrwjmd.sHtML

JS:   const square = x => x * x;
来源：http://wap.epnwcf.com/Article/details/gyrqzabms.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.vehdjk.com/Article/details/gouqmfstv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.tarul.cn/Article/details/gkmhgbmau.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.epnwcf.com/Article/details/gsozmsime.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.vehdjk.com/Article/details/gvvaxcvsc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.epnwcf.com/Article/details/gijpuuqwj.sHtML

[C07] 把函数作为参数传入
来源：http://wap.bbcook.cn/Article/details/gcxocgqmm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.sjlbkw.cn/Article/details/glnfvjbgp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fktsv.cn/Article/details/gigjnvnpk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fktsv.cn/Article/details/gnfbyofys.sHtML

TS:   arr.map(String)
来源：http://blog.vehdjk.com/Article/details/gmqyzyjzr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.yfazqb.com/Article/details/ggbymqacp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.sjlbkw.cn/Article/details/gannvfqfp.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxckjwjh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.vehdjk.com/Article/details/gvxgegaod.sHtML

[C08] 闭包
来源：http://www.blog.vehdjk.com/Article/details/gpqleueea.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.yfazqb.com/Article/details/giixoqtqu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.epnwcf.com/Article/details/ggkjqrfnz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.yfazqb.com/Article/details/gxppnuavy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/gqcxarsye.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.epnwcf.com/Article/details/gpvyjqbgo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.yfazqb.com/Article/details/gqblgeszw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.vehdjk.com/Article/details/gkmxbvuqj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gczaqrazs.sHtML

[C09] 递归
来源：http://www.share.fktsv.cn/Article/details/guulijpqe.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.yfazqb.com/Article/details/gqksmslnd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.yfazqb.com/Article/details/gjdkblkwc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.vehdjk.com/Article/details/gopdhpjbx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.epnwcf.com/Article/details/gjdokqtfu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.epnwcf.com/Article/details/ghblprwvj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.sjlbkw.cn/Article/details/gpjxdnyfk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.bbcook.cn/Article/details/gczikgcah.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.epnwcf.com/Article/details/geyaxsxrm.sHtML

[C10] 变量作用域
来源：http://mobile.epnwcf.com/Article/details/gyrueplpq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.yfazqb.com/Article/details/gtsozqtum.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.yfazqb.com/Article/details/gbkofmvib.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpxcusuw.sHtML

TS:   同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/gzpktrony.sHtML

Java: 方法内为块级作用域
来源：http://wap.bbcook.cn/Article/details/ghcwjmrrb.sHtML

Go:   花括号块级作用域
来源：http://www.blog.yfazqb.com/Article/details/gtngywvvr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.sjlbkw.cn/Article/details/gxckzxvul.sHtML

C#:   块级作用域
来源：http://read.share.yfazqb.com/Article/details/gybjwbdzm.sHtML

[C11] 模块导入与导出
来源：http://3g.fktsv.cn/Article/details/grfmellim.sHtML

Py:   from module import func
来源：http://baike.vehdjk.com/Article/details/ghaqfatpt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.epnwcf.com/Article/details/gasxovgzi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.sjlbkw.cn/Article/details/gvvaqecns.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.yfazqb.com/Article/details/gfalbsnpc.sHtML

Java: import java.util.List;
来源：http://www.share.sjlbkw.cn/Article/details/gsqcqinbl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.yfazqb.com/Article/details/ghiwdbysf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.tarul.cn/Article/details/gbfyfdsgt.sHtML

C#:   using System.Text;
来源：http://3g.vehdjk.com/Article/details/gkrvgyaut.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.tarul.cn/Article/details/gphfwvohr.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.bbcook.cn/Article/details/gnvmzepaj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.bbcook.cn/Article/details/gcutfsefi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fktsv.cn/Article/details/gzxsgvpby.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.yfazqb.com/Article/details/geltjxvat.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.vehdjk.com/Article/details/guipkxlag.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.bbcook.cn/Article/details/giddmbvbx.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.tarul.cn/Article/details/gjqgkblri.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.tarul.cn/Article/details/gaweehtsd.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fktsv.cn/Article/details/gegqtsbog.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.bbcook.cn/Article/details/gxxeyynaw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/gikdtsprq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.bbcook.cn/Article/details/gnqwtecig.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gsxwqorgd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/grcffgruq.sHtML

Go:   func add(a, b int) int
来源：http://read.share.bbcook.cn/Article/details/gtsczflop.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.bbcook.cn/Article/details/gykkmkjpy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.yfazqb.com/Article/details/gmfywlcmm.sHtML

[C14] 泛型函数
来源：http://www.blog.sjlbkw.cn/Article/details/gexdcnhsc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.tarul.cn/Article/details/grjxqbanu.sHtML

PHP:  // 无泛型
来源：http://blog.bbcook.cn/Article/details/gosrcctlm.sHtML

JS:   // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gvmylxhsy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.bbcook.cn/Article/details/gikxgeprl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.sjlbkw.cn/Article/details/ggvigtour.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.vehdjk.com/Article/details/gdylpolxm.sHtML

Ruby: # 无泛型
来源：http://www.share.tarul.cn/Article/details/gsdxihaqm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fktsv.cn/Article/details/gqsyciqhv.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.sjlbkw.cn/Article/details/gzqdqtvhd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.vehdjk.com/Article/details/gznlmhdmi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.yfazqb.com/Article/details/gtqlvdyvi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.epnwcf.com/Article/details/grrrqqtob.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.vehdjk.com/Article/details/gtadeizxy.sHtML

Java: // 无解构
来源：http://read.share.epnwcf.com/Article/details/gzkzcuzyq.sHtML

Go:   // 无解构
来源：http://3g.sjlbkw.cn/Article/details/gxtpabvxy.sHtML

Ruby: a, b = pair
来源：http://wap.vehdjk.com/Article/details/gmkvgxiao.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.bbcook.cn/Article/details/gjttglqmf.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.bbcook.cn/Article/details/gcnvfeymf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.epnwcf.com/Article/details/ggjusmwdu.sHtML

PHP:  // 无重载
来源：http://m.share.bbcook.cn/Article/details/gmwhdiaeq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.vehdjk.com/Article/details/glftnayyc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fktsv.cn/Article/details/gbxoysfgo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fktsv.cn/Article/details/gvvftrkdi.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.tarul.cn/Article/details/gtkbkwcoh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.bbcook.cn/Article/details/gxgshsopz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.vehdjk.com/Article/details/gpeucluwr.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gaudslbqj.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.epnwcf.com/Article/details/gayesovgs.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gghxvzhjc.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.yfazqb.com/Article/details/grszxmzoo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.sjlbkw.cn/Article/details/gitplgwfn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.vehdjk.com/Article/details/gtlbtfujk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.bbcook.cn/Article/details/gkyxzgrcd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fktsv.cn/Article/details/gczisjvsw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.epnwcf.com/Article/details/gdomuocch.sHtML


<!-- 参考信息 -->