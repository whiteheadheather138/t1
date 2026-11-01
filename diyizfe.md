代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.bbcook.cn/Article/details/ggurdsueq.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.vehdjk.com/Article/details/gvcdzfedo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.tarul.cn/Article/details/gymibwfxg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.bbcook.cn/Article/details/gqyvfsnwz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.tarul.cn/Article/details/gbttptinn.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.bbcook.cn/Article/details/gmeicwmzq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.bbcook.cn/Article/details/gtofwlyiz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.vehdjk.com/Article/details/gzqxnlzwq.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.tarul.cn/Article/details/gyimjmgey.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fktsv.cn/Article/details/gmukpchkp.sHtML

[B03] switch / match / case
来源：http://m.share.tarul.cn/Article/details/gtagbhtod.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fktsv.cn/Article/details/ghzrlcegk.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.tarul.cn/Article/details/gblgazbve.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/gvrbgxdxs.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/gjtwvacja.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/gwmffeure.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.fktsv.cn/Article/details/gmmvbihji.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.vehdjk.com/Article/details/giomwpcei.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.tarul.cn/Article/details/gqmcopdmr.sHtML

[B04] for 计数循环
来源：http://mobile.sjlbkw.cn/Article/details/gwydlcyrd.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.tarul.cn/Article/details/gzdllhibq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.sjlbkw.cn/Article/details/gcygcibel.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.tarul.cn/Article/details/gtvtaeect.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fktsv.cn/Article/details/gdvwttddm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.bbcook.cn/Article/details/gzcisozcg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fktsv.cn/Article/details/guahmwnbr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fktsv.cn/Article/details/gznqermxg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.vehdjk.com/Article/details/ghdtuakmn.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.tarul.cn/Article/details/gbleoukta.sHtML

Py:   for item in arr: print(item)
来源：http://3g.bbcook.cn/Article/details/ggxysnqcx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.vehdjk.com/Article/details/gnnopcflu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.epnwcf.com/Article/details/gglyjscah.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fktsv.cn/Article/details/grrizuzpq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhassurn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.epnwcf.com/Article/details/gwhliidgr.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.vehdjk.com/Article/details/gsseaxwtu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.vehdjk.com/Article/details/grvmouwbr.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.vehdjk.com/Article/details/gahxnonds.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.sjlbkw.cn/Article/details/gvbtoqfxz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.bbcook.cn/Article/details/glysijwhx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.epnwcf.com/Article/details/geleajhtc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.yfazqb.com/Article/details/gfruyiqcz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.epnwcf.com/Article/details/gvpqjvlct.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.bbcook.cn/Article/details/gcudgadnb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.sjlbkw.cn/Article/details/gfjjchrwp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.tarul.cn/Article/details/gvienttjq.sHtML

[B07] while 循环
来源：http://read.share.epnwcf.com/Article/details/ghoynvdmj.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.yfazqb.com/Article/details/gxdujawws.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.epnwcf.com/Article/details/guvuqgfll.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/gzkwoiniv.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.epnwcf.com/Article/details/gaaxhxfnn.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.tarul.cn/Article/details/gikblyapf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.bbcook.cn/Article/details/guikckxmf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fktsv.cn/Article/details/givzijnjk.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.epnwcf.com/Article/details/gfxwojijw.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.tarul.cn/Article/details/ggdcuynzn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.sjlbkw.cn/Article/details/gtqrmxttp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/gaxtyakcx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.sjlbkw.cn/Article/details/gkzepoxjp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/gpoibqstt.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/glcprpjtm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.bbcook.cn/Article/details/gjwukoqcj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.bbcook.cn/Article/details/grjyjnowe.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/grxpxmgya.sHtML

[B09] break 与 continue
来源：http://www.blog.sjlbkw.cn/Article/details/gsjnxuhsr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.yfazqb.com/Article/details/gcubxpolo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gwplatyto.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gtopmmlzz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gxnfvrjye.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gqhncnnzr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.sjlbkw.cn/Article/details/gspbvmvrb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.tarul.cn/Article/details/goohywrtc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gyqvytobp.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.vehdjk.com/Article/details/gjjoyqtlz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.yfazqb.com/Article/details/gjqkoumlj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.tarul.cn/Article/details/gdsiimxko.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.vehdjk.com/Article/details/ganlalwep.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.tarul.cn/Article/details/gznrigwzs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.yfazqb.com/Article/details/gqikeyggf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.tarul.cn/Article/details/gsbdnfijw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.sjlbkw.cn/Article/details/gpwsyhabn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.tarul.cn/Article/details/ggtwwltzy.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.tarul.cn/Article/details/gltxpasdr.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.vehdjk.com/Article/details/gmthtmjah.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fktsv.cn/Article/details/gzaudqvht.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.yfazqb.com/Article/details/geoiyyfyp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.sjlbkw.cn/Article/details/grfjeximz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.yfazqb.com/Article/details/gfqlcyuwc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.epnwcf.com/Article/details/gknrjujll.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.vehdjk.com/Article/details/gjfstuurm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.vehdjk.com/Article/details/gcqgegkkw.sHtML

[B12] 跳出多层循环
来源：http://www.blog.bbcook.cn/Article/details/gulttqohf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.sjlbkw.cn/Article/details/gqcbelgej.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.tarul.cn/Article/details/gujwmvgeo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/gltnxedei.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fktsv.cn/Article/details/gyqcxgrxe.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gdhyylxst.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.bbcook.cn/Article/details/grcqxxtgy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.yfazqb.com/Article/details/gwstqphkz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.bbcook.cn/Article/details/gypfiykia.sHtML

[B13] 判断是否为数字
来源：http://blog.sjlbkw.cn/Article/details/glfrsicll.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.bbcook.cn/Article/details/gvxkjtuyn.sHtML

PHP:  is_numeric($x)
来源：http://read.share.bbcook.cn/Article/details/gxtutidow.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.epnwcf.com/Article/details/gtpmhfoef.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.sjlbkw.cn/Article/details/griddrfiu.sHtML

Java: x instanceof Number
来源：http://read.share.sjlbkw.cn/Article/details/gumahelsr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.bbcook.cn/Article/details/gtsrcilkf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.tarul.cn/Article/details/gjzxnmtxh.sHtML

C#:   x is int or double or decimal
来源：http://baike.bbcook.cn/Article/details/gsgyhdjba.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.yfazqb.com/Article/details/gduhcxwot.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fktsv.cn/Article/details/grmluqenc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.tarul.cn/Article/details/gocutovkf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.epnwcf.com/Article/details/gaqxltyvq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fktsv.cn/Article/details/gmkyuqayt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.vehdjk.com/Article/details/gxebbtbsi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.tarul.cn/Article/details/gseqomrle.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.bbcook.cn/Article/details/glykjchpg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.yfazqb.com/Article/details/gcqwbyggt.sHtML

[B15] 布尔运算与取反
来源：http://blog.fktsv.cn/Article/details/gzffvcmxc.sHtML

Py:   a and b or not c
来源：http://m.share.sjlbkw.cn/Article/details/gbruubvop.sHtML

PHP:  $a && $b || !$c
来源：http://baike.bbcook.cn/Article/details/gxnpopvvl.sHtML

JS:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/guprdpupd.sHtML

TS:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gtzabiluq.sHtML

Java: a && b || !c
来源：http://blog.vehdjk.com/Article/details/gsfdxycor.sHtML

Go:   a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gtxzfnkfw.sHtML

Ruby: a && b || !c
来源：http://mobile.tarul.cn/Article/details/gxkmbqhau.sHtML

C#:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gvtaojdsi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fktsv.cn/Article/details/gcemtybnh.sHtML

Py:   if not data: return
来源：http://www.blog.fktsv.cn/Article/details/gmrmnpjsc.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.sjlbkw.cn/Article/details/gzxzlnbsc.sHtML

JS:   if (!data) return;
来源：http://baike.sjlbkw.cn/Article/details/gqqczluis.sHtML

TS:   if (!data) return;
来源：http://m.share.yfazqb.com/Article/details/gclqssjgy.sHtML

Java: if (data == null) return;
来源：http://blog.yfazqb.com/Article/details/gifpgauve.sHtML

Go:   if data == nil { return }
来源：http://mobile.epnwcf.com/Article/details/gokqpbdiv.sHtML

Ruby: return if data.nil?
来源：http://www.share.fktsv.cn/Article/details/ginlepoxd.sHtML

C#:   if (data == null) return;
来源：http://read.share.bbcook.cn/Article/details/gjcnqregb.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gorwusyrt.sHtML

C. 函数与作用域
来源：http://www.blog.vehdjk.com/Article/details/gxdmmphix.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gdlwfenuy.sHtML

[C01] 定义函数
来源：http://blog.yfazqb.com/Article/details/genaicrwl.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.vehdjk.com/Article/details/gzojcipwm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/gqzkzrifl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/ggjxatozv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.tarul.cn/Article/details/gazjgctxi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/giawukpwz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.sjlbkw.cn/Article/details/gvyfglbub.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.epnwcf.com/Article/details/giqxvzkpc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gfmirsqjj.sHtML

[C02] 默认参数
来源：http://mobile.tarul.cn/Article/details/gimeinqcb.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.tarul.cn/Article/details/gqvqfhslj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.yfazqb.com/Article/details/gezsrldvx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.epnwcf.com/Article/details/gtlvjblot.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.epnwcf.com/Article/details/gdqehexhq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.vehdjk.com/Article/details/gvvustdcd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.yfazqb.com/Article/details/gsnosmfgx.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.bbcook.cn/Article/details/gbongqikz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.yfazqb.com/Article/details/gxvphfskc.sHtML

[C03] 可变参数
来源：http://blog.tarul.cn/Article/details/gurmwcins.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.epnwcf.com/Article/details/gzzknfgce.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.yfazqb.com/Article/details/gminpooen.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fktsv.cn/Article/details/gfdfgfgzd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.tarul.cn/Article/details/goquuqdge.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.sjlbkw.cn/Article/details/gsepajypj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.yfazqb.com/Article/details/gampfapds.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fktsv.cn/Article/details/gqcepboru.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.vehdjk.com/Article/details/gtsxxejga.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.yfazqb.com/Article/details/gydlbrmxz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.epnwcf.com/Article/details/gisaammmv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.tarul.cn/Article/details/geevzcynn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.epnwcf.com/Article/details/gdkrlnhns.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.yfazqb.com/Article/details/goyxewxxa.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.vehdjk.com/Article/details/gzqdufrfr.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.tarul.cn/Article/details/gtlnhnjsx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/gvanzgomw.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/guojidktn.sHtML

[C05] 返回多个值
来源：http://www.share.yfazqb.com/Article/details/ggdrsqjnq.sHtML

Py:   return a, b
来源：http://baike.bbcook.cn/Article/details/gererazcf.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gghldwhcw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/gezfwakua.sHtML

TS:   return { a, b };
来源：http://baike.tarul.cn/Article/details/gkqjhqxpy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.yfazqb.com/Article/details/gihlwkavh.sHtML

Go:   return a, b
来源：http://www.share.bbcook.cn/Article/details/gbxvdpgvw.sHtML

Ruby: return a, b
来源：http://mobile.fktsv.cn/Article/details/grzjnpier.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.sjlbkw.cn/Article/details/gcbbpytaj.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fktsv.cn/Article/details/gmsqlwjnw.sHtML

Py:   square = lambda x: x * x
来源：http://blog.epnwcf.com/Article/details/gkckjnkwe.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.vehdjk.com/Article/details/ghhydfywl.sHtML

JS:   const square = x => x * x;
来源：http://blog.yfazqb.com/Article/details/gbfwzsoxf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.epnwcf.com/Article/details/gdgtclgri.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.sjlbkw.cn/Article/details/gngijgtkl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fktsv.cn/Article/details/gjcqskzjt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.epnwcf.com/Article/details/gsmttpeie.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.epnwcf.com/Article/details/ghmyzqpia.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.bbcook.cn/Article/details/gomvzprwq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.bbcook.cn/Article/details/gwzqbuzsm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fktsv.cn/Article/details/giqbeqtlv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.epnwcf.com/Article/details/gtyijqyaq.sHtML

TS:   arr.map(String)
来源：http://www.blog.epnwcf.com/Article/details/gdivtyugl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fktsv.cn/Article/details/gboedhghz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.yfazqb.com/Article/details/glcvcljly.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrugcqst.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.bbcook.cn/Article/details/gukbtmsrw.sHtML

[C08] 闭包
来源：http://baike.bbcook.cn/Article/details/gmwooqdfi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fktsv.cn/Article/details/gytrhjxxg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.epnwcf.com/Article/details/gdjnufzun.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.epnwcf.com/Article/details/gzfakrvma.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.tarul.cn/Article/details/gvmgyavsj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.tarul.cn/Article/details/gnttwsovn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.sjlbkw.cn/Article/details/gnjvfjlhi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.yfazqb.com/Article/details/gdylyaorv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.tarul.cn/Article/details/ghtflnvfg.sHtML

[C09] 递归
来源：http://read.share.tarul.cn/Article/details/gxkatlyci.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.sjlbkw.cn/Article/details/govsmbiwc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.yfazqb.com/Article/details/ganhpldjq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.sjlbkw.cn/Article/details/gzzvkzlgr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.sjlbkw.cn/Article/details/gvlgrfquo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.epnwcf.com/Article/details/gqsarjfkm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.sjlbkw.cn/Article/details/gmumrdxtk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.vehdjk.com/Article/details/gipzjnqfp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.yfazqb.com/Article/details/gqcoxoakj.sHtML

[C10] 变量作用域
来源：http://wap.fktsv.cn/Article/details/gdkxudzcv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.vehdjk.com/Article/details/gbylgsgiq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.yfazqb.com/Article/details/gajhuquex.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.vehdjk.com/Article/details/gmemyvtjd.sHtML

TS:   同 JS
来源：http://3g.epnwcf.com/Article/details/gzwfaowhj.sHtML

Java: 方法内为块级作用域
来源：http://blog.bbcook.cn/Article/details/gzhsnlabv.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gujuqmnlc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.tarul.cn/Article/details/grhnsanbg.sHtML

C#:   块级作用域
来源：http://www.share.epnwcf.com/Article/details/gctmtlqjc.sHtML

[C11] 模块导入与导出
来源：http://m.share.sjlbkw.cn/Article/details/gvqkuomgs.sHtML

Py:   from module import func
来源：http://www.blog.vehdjk.com/Article/details/ghlcqjwci.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.tarul.cn/Article/details/gtimdygqx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.bbcook.cn/Article/details/gasmfviih.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.sjlbkw.cn/Article/details/gjygahbla.sHtML

Java: import java.util.List;
来源：http://wap.bbcook.cn/Article/details/gfltehmoh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.sjlbkw.cn/Article/details/glervsuri.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.bbcook.cn/Article/details/gzfeljrio.sHtML

C#:   using System.Text;
来源：http://wap.epnwcf.com/Article/details/glbwhflbp.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.epnwcf.com/Article/details/gpbibgnaw.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.bbcook.cn/Article/details/gwkupgixr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.tarul.cn/Article/details/glrlxtcen.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.tarul.cn/Article/details/gofjjvnke.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.epnwcf.com/Article/details/ggoftowiy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.sjlbkw.cn/Article/details/gwjmlimvq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.tarul.cn/Article/details/gvndjgrjm.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.vehdjk.com/Article/details/guqcfapdf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.tarul.cn/Article/details/geehjcpgn.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.bbcook.cn/Article/details/gsxbmhsmi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.tarul.cn/Article/details/gueodfyzp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gyghkqhng.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.tarul.cn/Article/details/gvffxukpx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gjkbnhsbh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gvvvjjwqc.sHtML

Go:   func add(a, b int) int
来源：http://wap.vehdjk.com/Article/details/gaeqdtcbi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fktsv.cn/Article/details/gmbbhleww.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.epnwcf.com/Article/details/gnqohmiir.sHtML

[C14] 泛型函数
来源：http://www.m.share.yfazqb.com/Article/details/guxczuwsv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.sjlbkw.cn/Article/details/ghydlyspt.sHtML

PHP:  // 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/gxlrinbia.sHtML

JS:   // 无泛型
来源：http://www.blog.fktsv.cn/Article/details/gqvoeicbu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.yfazqb.com/Article/details/gpbduveau.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.bbcook.cn/Article/details/ghwumycws.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.yfazqb.com/Article/details/gycthxoke.sHtML

Ruby: # 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/gmkzrrfyk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.epnwcf.com/Article/details/gbhtchsto.sHtML

[C15] 解构 / 展开参数
来源：http://wap.epnwcf.com/Article/details/gaqqsdgwk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.tarul.cn/Article/details/gxxpooobh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.epnwcf.com/Article/details/gewidllym.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.epnwcf.com/Article/details/gedmjkggf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.epnwcf.com/Article/details/givmhqseh.sHtML

Java: // 无解构
来源：http://read.share.sjlbkw.cn/Article/details/gusiznkxi.sHtML

Go:   // 无解构
来源：http://www.share.fktsv.cn/Article/details/guljhadpq.sHtML

Ruby: a, b = pair
来源：http://wap.vehdjk.com/Article/details/gzoysaafj.sHtML

C#:   var (a, b) = pair;
来源：http://3g.epnwcf.com/Article/details/ghxwjysgn.sHtML

[C16] 函数 / 方法重载
来源：http://blog.sjlbkw.cn/Article/details/gajdytvau.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.epnwcf.com/Article/details/gokcopbet.sHtML

PHP:  // 无重载
来源：http://mobile.fktsv.cn/Article/details/goidpudhn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.yfazqb.com/Article/details/gfbltqyfz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fktsv.cn/Article/details/gjadeyzmc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.epnwcf.com/Article/details/ggffzmawr.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.epnwcf.com/Article/details/gvxammoce.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fktsv.cn/Article/details/goxmfrdlf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.vehdjk.com/Article/details/guxgvwmvw.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gtkfqtvou.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.bbcook.cn/Article/details/gkdfzyeqy.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gvqaurkbe.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.yfazqb.com/Article/details/gixsabegp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.bbcook.cn/Article/details/gwjiztvxc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.vehdjk.com/Article/details/gnxxoppnz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fktsv.cn/Article/details/gyvwxwitv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.epnwcf.com/Article/details/gqwcefrxg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.tarul.cn/Article/details/gmwclqcff.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.epnwcf.com/Article/details/gvgpyapzr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.tarul.cn/Article/details/gvkkkqabe.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.tarul.cn/Article/details/gdgggzwgn.sHtML

[D02] 追加元素到末尾
来源：http://wap.fktsv.cn/Article/details/gyfwzkvig.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.bbcook.cn/Article/details/gldqxlspe.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.sjlbkw.cn/Article/details/gifkigmjo.sHtML

JS:   arr.push(4);
来源：http://mobile.sjlbkw.cn/Article/details/glsdmsxrw.sHtML

TS:   arr.push(4);
来源：http://baike.yfazqb.com/Article/details/gakqifjjg.sHtML


<!-- 参考信息 -->