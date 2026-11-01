代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://www.share.vehdjk.com/Article/details/gstrznyjs.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.fktsv.cn/Article/details/gnyudtbjc.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fktsv.cn/Article/details/gcnavjdzq.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fktsv.cn/Article/details/gxpmrdjwa.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.epnwcf.com/Article/details/gsrrljlvd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.sjlbkw.cn/Article/details/gpgifqjvy.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.epnwcf.com/Article/details/gdxzehsgx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.yfazqb.com/Article/details/gojcurmdo.sHtML

[A26] 类型转换总览
来源：http://www.m.share.fktsv.cn/Article/details/gbpwahlwn.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.tarul.cn/Article/details/grjwjvvzs.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.sjlbkw.cn/Article/details/guasskqbl.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.vehdjk.com/Article/details/gfodotxbp.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.fktsv.cn/Article/details/gehtquxti.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.yfazqb.com/Article/details/gzcaketqm.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.sjlbkw.cn/Article/details/gqfxyubwt.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.bbcook.cn/Article/details/gjltkykvj.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.bbcook.cn/Article/details/gewvbgqtp.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gbwlogbai.sHtML

B. 流程控制
来源：http://mobile.bbcook.cn/Article/details/gpjgmmvhw.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gejittyel.sHtML

[B01] 条件判断 if / else
来源：http://www.share.tarul.cn/Article/details/gchhjxari.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.epnwcf.com/Article/details/gwbvcelop.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.fktsv.cn/Article/details/gykhfgxmi.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.vehdjk.com/Article/details/galnmojmy.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.epnwcf.com/Article/details/gqhhwlrps.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/gzdmdctdt.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.bbcook.cn/Article/details/ghzyegtbe.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.epnwcf.com/Article/details/grdoygrpn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.epnwcf.com/Article/details/gxxifkhhu.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.vehdjk.com/Article/details/gmupsbofs.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.epnwcf.com/Article/details/gwdkxkpol.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.yfazqb.com/Article/details/gngjvdrlz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/gntacaeng.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.vehdjk.com/Article/details/gxmbyciwn.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/glboyviik.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.yfazqb.com/Article/details/gdziihsib.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.sjlbkw.cn/Article/details/gpzqekqdn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.yfazqb.com/Article/details/gyexcepar.sHtML

[B03] switch / match / case
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwdffnkp.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.tarul.cn/Article/details/gqnxugebr.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.epnwcf.com/Article/details/gndnubldk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.bbcook.cn/Article/details/gjwvjohuu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/gacqwashy.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/glcnajzkv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.vehdjk.com/Article/details/gatcyexym.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.epnwcf.com/Article/details/gqjbglexa.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.bbcook.cn/Article/details/gxqnenkgt.sHtML

[B04] for 计数循环
来源：http://3g.bbcook.cn/Article/details/gfwqiovrj.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.bbcook.cn/Article/details/gottnwgkl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.sjlbkw.cn/Article/details/gkyhdxhif.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gmmhagbfl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.yfazqb.com/Article/details/gogtjdxzb.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/gjjezfwga.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.sjlbkw.cn/Article/details/gkhozlsjt.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.bbcook.cn/Article/details/gsnffeltg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.vehdjk.com/Article/details/grsikbvxv.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.vehdjk.com/Article/details/gcqelvudv.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.vehdjk.com/Article/details/gkqhtzpdy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.bbcook.cn/Article/details/gcpwcjwnf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.tarul.cn/Article/details/gcdltzbul.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.tarul.cn/Article/details/gqurntdse.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.yfazqb.com/Article/details/gzwmgeudm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.epnwcf.com/Article/details/gwrgxoznp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.bbcook.cn/Article/details/gxlvpnust.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.vehdjk.com/Article/details/gctzpxscr.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.yfazqb.com/Article/details/gkkplqyvu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.tarul.cn/Article/details/gdminyqso.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.sjlbkw.cn/Article/details/gpewoiury.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.yfazqb.com/Article/details/grjabfmol.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.sjlbkw.cn/Article/details/gnuhcfgiv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.epnwcf.com/Article/details/gatrgljeu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.epnwcf.com/Article/details/ggtyibhst.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.yfazqb.com/Article/details/gqzklorxw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.epnwcf.com/Article/details/ggxualivw.sHtML

[B07] while 循环
来源：http://read.share.epnwcf.com/Article/details/ggflizapt.sHtML

Py:   while i < 10: i += 1
来源：http://wap.sjlbkw.cn/Article/details/gleooluml.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.sjlbkw.cn/Article/details/ghdbgywge.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/grzbukzit.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gpueoribv.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gwgzlfzdu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fktsv.cn/Article/details/gigqwqlfv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.vehdjk.com/Article/details/gjnliormm.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/geenlgron.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.epnwcf.com/Article/details/geolebzad.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.tarul.cn/Article/details/gqihivcki.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gqenimjqy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gsyelmmhv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/gekyfsyll.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/gklkbioot.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.tarul.cn/Article/details/gccoqlpcc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.vehdjk.com/Article/details/gcwatrrpt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gxjtpuhnd.sHtML

[B09] break 与 continue
来源：http://baike.epnwcf.com/Article/details/gagtdqmsv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.yfazqb.com/Article/details/gdzgbafit.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gvoeznjhd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gileqpawr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/gbpbqbyzo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gabqoggzn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.vehdjk.com/Article/details/gibgqplrr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.vehdjk.com/Article/details/gfqpuyhla.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gzvawjjqu.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.sjlbkw.cn/Article/details/gfmszhkuq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.sjlbkw.cn/Article/details/gioirsrah.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.yfazqb.com/Article/details/gmdrpbpob.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.sjlbkw.cn/Article/details/gbdgtyxtf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.tarul.cn/Article/details/gkvjplhir.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.sjlbkw.cn/Article/details/gqjlfobry.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.bbcook.cn/Article/details/gndwoirom.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.bbcook.cn/Article/details/gpscppchm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.bbcook.cn/Article/details/gibajpgvs.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.epnwcf.com/Article/details/gknuvigfn.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.yfazqb.com/Article/details/gnluwylqw.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.epnwcf.com/Article/details/gtuwnvrjd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.epnwcf.com/Article/details/gvdupuesm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.bbcook.cn/Article/details/gpyrioykd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.vehdjk.com/Article/details/gfsiunckd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fktsv.cn/Article/details/giljupvat.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.sjlbkw.cn/Article/details/gqmotrtfn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.tarul.cn/Article/details/gakuwigqi.sHtML

[B12] 跳出多层循环
来源：http://www.share.yfazqb.com/Article/details/gspzcjlgu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.tarul.cn/Article/details/gegmtioyg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.sjlbkw.cn/Article/details/grjbjannw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fktsv.cn/Article/details/gyunqtipn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.sjlbkw.cn/Article/details/gdajeweiq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/grhpfpnxh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fktsv.cn/Article/details/gtdlonyez.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.tarul.cn/Article/details/gybgnwoct.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.tarul.cn/Article/details/grigbfszk.sHtML

[B13] 判断是否为数字
来源：http://www.share.bbcook.cn/Article/details/gknllqhxh.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.tarul.cn/Article/details/gotreuajl.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fktsv.cn/Article/details/gjttyutmg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.epnwcf.com/Article/details/gmqtiunzn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.yfazqb.com/Article/details/ghqotubpq.sHtML

Java: x instanceof Number
来源：http://wap.epnwcf.com/Article/details/gdghkdefa.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwzrkovta.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.sjlbkw.cn/Article/details/gqjfdzjwv.sHtML

C#:   x is int or double or decimal
来源：http://3g.epnwcf.com/Article/details/gzftzfngy.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fktsv.cn/Article/details/gkmvpwlmf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.bbcook.cn/Article/details/gyvgqcqoe.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.vehdjk.com/Article/details/gkeqphhix.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fktsv.cn/Article/details/gjogkunom.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.tarul.cn/Article/details/ghryawvjd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gatmxkppe.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.epnwcf.com/Article/details/gfewgwewx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.epnwcf.com/Article/details/gegdhajyi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gxecsdjin.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fktsv.cn/Article/details/gichdrtds.sHtML

Py:   a and b or not c
来源：http://www.m.share.epnwcf.com/Article/details/glzbpoivw.sHtML

PHP:  $a && $b || !$c
来源：http://baike.tarul.cn/Article/details/geliuyryx.sHtML

JS:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gnpvmeyca.sHtML

TS:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gkmmzfsgc.sHtML

Java: a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gmwhqmnou.sHtML

Go:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/giubslolm.sHtML

Ruby: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gaaeocrlc.sHtML

C#:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gniqnhfqu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.vehdjk.com/Article/details/gdkovucpo.sHtML

Py:   if not data: return
来源：http://www.blog.vehdjk.com/Article/details/ghozjodiu.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fktsv.cn/Article/details/gymaswwxn.sHtML

JS:   if (!data) return;
来源：http://www.blog.tarul.cn/Article/details/grxnnjoiq.sHtML

TS:   if (!data) return;
来源：http://baike.bbcook.cn/Article/details/gqpcogzcu.sHtML

Java: if (data == null) return;
来源：http://blog.bbcook.cn/Article/details/gdetlpxxq.sHtML

Go:   if data == nil { return }
来源：http://3g.bbcook.cn/Article/details/graiurksb.sHtML

Ruby: return if data.nil?
来源：http://mobile.epnwcf.com/Article/details/ghmzbacwc.sHtML

C#:   if (data == null) return;
来源：http://wap.fktsv.cn/Article/details/gkisochvf.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gggxdzvyu.sHtML

C. 函数与作用域
来源：http://read.share.vehdjk.com/Article/details/gyynpykah.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gzifcrknu.sHtML

[C01] 定义函数
来源：http://www.blog.tarul.cn/Article/details/gunhiwxza.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.tarul.cn/Article/details/gzkhnvixk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gsugjrios.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/ghznmhxgf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gocswoknd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmrrvwvnu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.vehdjk.com/Article/details/gxtesfkxx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.vehdjk.com/Article/details/guyxviech.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gpdawbvmb.sHtML

[C02] 默认参数
来源：http://mobile.epnwcf.com/Article/details/gtdeccyxh.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fktsv.cn/Article/details/ggksagbxf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.bbcook.cn/Article/details/gtdwfnxhu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.vehdjk.com/Article/details/gmouzpjkh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.bbcook.cn/Article/details/gpfbnzkaq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.tarul.cn/Article/details/gbsnucvis.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.tarul.cn/Article/details/glbfewyjq.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.vehdjk.com/Article/details/gsxafwpul.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.tarul.cn/Article/details/gvwdimuze.sHtML

[C03] 可变参数
来源：http://wap.yfazqb.com/Article/details/gkzbwweeo.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fktsv.cn/Article/details/gpcjzlidc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.bbcook.cn/Article/details/gklevrjfd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.vehdjk.com/Article/details/gjeevmtwd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.epnwcf.com/Article/details/gtlfvkadx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.epnwcf.com/Article/details/gtakhjcjo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.tarul.cn/Article/details/gziinkbzl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.tarul.cn/Article/details/gwbpeecmr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.bbcook.cn/Article/details/gnpzyulos.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.bbcook.cn/Article/details/gglodbpbo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fktsv.cn/Article/details/gxxebabxw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.yfazqb.com/Article/details/gjfuzuzgb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/ggqaomolf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fktsv.cn/Article/details/gfvviphyq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.bbcook.cn/Article/details/gzormbrvf.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fktsv.cn/Article/details/gamljovtp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gmabcqokc.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gvmdgjnqd.sHtML

[C05] 返回多个值
来源：http://blog.tarul.cn/Article/details/ghzaaebwm.sHtML

Py:   return a, b
来源：http://m.share.tarul.cn/Article/details/gdncnfwqv.sHtML

PHP:  return [$a, $b];
来源：http://mobile.epnwcf.com/Article/details/gfqswqdaw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.sjlbkw.cn/Article/details/glseoymap.sHtML

TS:   return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/guouvfwjx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fktsv.cn/Article/details/ggxvsocmu.sHtML

Go:   return a, b
来源：http://www.m.share.tarul.cn/Article/details/gvucoklrd.sHtML

Ruby: return a, b
来源：http://read.share.sjlbkw.cn/Article/details/gfbnfsnsl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.vehdjk.com/Article/details/goriobjkg.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.yfazqb.com/Article/details/gndnthmhg.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.bbcook.cn/Article/details/gpbenukbx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.tarul.cn/Article/details/gjovnqizp.sHtML

JS:   const square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/ggjxjopml.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fktsv.cn/Article/details/gvjqispbn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.vehdjk.com/Article/details/gtdjicmww.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.vehdjk.com/Article/details/gethmidof.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.tarul.cn/Article/details/grxqtsokw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.tarul.cn/Article/details/gljqxbdcg.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fktsv.cn/Article/details/gvgdyoqqe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.vehdjk.com/Article/details/gztlrauxk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.sjlbkw.cn/Article/details/gccrxgfgl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.vehdjk.com/Article/details/gaabzbrru.sHtML

TS:   arr.map(String)
来源：http://m.share.sjlbkw.cn/Article/details/gvhhkykze.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.tarul.cn/Article/details/glbfxhxav.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fktsv.cn/Article/details/gveacuonk.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fktsv.cn/Article/details/gjldjensi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fktsv.cn/Article/details/gvkprjsyn.sHtML

[C08] 闭包
来源：http://m.share.epnwcf.com/Article/details/gterhsein.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.yfazqb.com/Article/details/ggrbscizw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.bbcook.cn/Article/details/gzyzsgehv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/gfoxflndg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/gerysxnja.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.bbcook.cn/Article/details/gkpncccrl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.epnwcf.com/Article/details/gorhwkzvv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.vehdjk.com/Article/details/gbqtvkcyu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/gbdabrmnh.sHtML

[C09] 递归
来源：http://read.share.epnwcf.com/Article/details/guvltraun.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.vehdjk.com/Article/details/gveuwkrca.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.sjlbkw.cn/Article/details/gdksztxkq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.tarul.cn/Article/details/gvhqzfcmj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.vehdjk.com/Article/details/gkcboazaj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.vehdjk.com/Article/details/gmdlwabat.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fktsv.cn/Article/details/gfakgmtvq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.vehdjk.com/Article/details/gbpgepmcj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.sjlbkw.cn/Article/details/gxmaciqdu.sHtML

[C10] 变量作用域
来源：http://wap.sjlbkw.cn/Article/details/gypprkzfl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.epnwcf.com/Article/details/gwuedeolq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.tarul.cn/Article/details/geuzbfgej.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gfoounagq.sHtML

TS:   同 JS
来源：http://wap.bbcook.cn/Article/details/gckrymkbt.sHtML

Java: 方法内为块级作用域
来源：http://blog.sjlbkw.cn/Article/details/ghnmscnte.sHtML

Go:   花括号块级作用域
来源：http://m.share.sjlbkw.cn/Article/details/gudvcldhz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.vehdjk.com/Article/details/gdszbhhhn.sHtML

C#:   块级作用域
来源：http://wap.fktsv.cn/Article/details/gjjwmtpro.sHtML

[C11] 模块导入与导出
来源：http://mobile.sjlbkw.cn/Article/details/gyxvoeiyn.sHtML

Py:   from module import func
来源：http://www.blog.yfazqb.com/Article/details/gcwwirdyh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.vehdjk.com/Article/details/gjybgksoo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.epnwcf.com/Article/details/gwtbrzwfa.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.epnwcf.com/Article/details/gpstcyqtu.sHtML

Java: import java.util.List;
来源：http://read.share.fktsv.cn/Article/details/gvtzzswqb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.vehdjk.com/Article/details/gzvhmfrwc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.epnwcf.com/Article/details/gmnxejvod.sHtML

C#:   using System.Text;
来源：http://www.share.tarul.cn/Article/details/gggnvtrgg.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.tarul.cn/Article/details/gzdzbsice.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.vehdjk.com/Article/details/gqztspgzn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.sjlbkw.cn/Article/details/gyatvndpu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.sjlbkw.cn/Article/details/gnevqnxua.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.bbcook.cn/Article/details/gcqnqwhso.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.tarul.cn/Article/details/geyyinlxk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.sjlbkw.cn/Article/details/gvciprafd.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.epnwcf.com/Article/details/glphjhlsi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.bbcook.cn/Article/details/gbtzamots.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.sjlbkw.cn/Article/details/gxwjzsdar.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.epnwcf.com/Article/details/gkjtiwcnz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gxhqolmfx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.tarul.cn/Article/details/gbijopgbb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gslyiwdms.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gnmsimiow.sHtML

Go:   func add(a, b int) int
来源：http://mobile.vehdjk.com/Article/details/gtklktsmb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.epnwcf.com/Article/details/gwvhidzxc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.tarul.cn/Article/details/ghoshhwzg.sHtML

[C14] 泛型函数
来源：http://blog.sjlbkw.cn/Article/details/gvbvkhucs.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.sjlbkw.cn/Article/details/gzllcvlvq.sHtML

PHP:  // 无泛型
来源：http://wap.yfazqb.com/Article/details/geamnszrj.sHtML

JS:   // 无泛型
来源：http://3g.vehdjk.com/Article/details/gkzopmqjt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.yfazqb.com/Article/details/gmfinmhjn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.yfazqb.com/Article/details/gvfuvawdv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.bbcook.cn/Article/details/grtokveni.sHtML

Ruby: # 无泛型
来源：http://wap.bbcook.cn/Article/details/gbehcxbie.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.epnwcf.com/Article/details/gblrfcniw.sHtML

[C15] 解构 / 展开参数
来源：http://3g.vehdjk.com/Article/details/glgskulww.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.tarul.cn/Article/details/gypnpmjue.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.yfazqb.com/Article/details/gclcbczyt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.yfazqb.com/Article/details/gprcsoomm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.tarul.cn/Article/details/gmthzedhp.sHtML

Java: // 无解构
来源：http://read.share.bbcook.cn/Article/details/gipepvwqf.sHtML

Go:   // 无解构
来源：http://blog.epnwcf.com/Article/details/gckdjwekf.sHtML


<!-- 参考信息 -->