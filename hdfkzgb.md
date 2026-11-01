代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.epnwcf.com/Article/details/gexbhqpus.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.epnwcf.com/Article/details/glnruhbbn.sHtML

[A24] 去除首尾空白
来源：http://m.share.sjlbkw.cn/Article/details/gsadjmbsw.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.yfazqb.com/Article/details/glqlzoeba.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.vehdjk.com/Article/details/gqcixwnrg.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.bbcook.cn/Article/details/gizuxozpr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.tarul.cn/Article/details/gzvuukphm.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.yfazqb.com/Article/details/gtbomdtgt.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.vehdjk.com/Article/details/gnakxynpk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.vehdjk.com/Article/details/gfspkgeqp.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.vehdjk.com/Article/details/gpioqrnfw.sHtML

[A25] 字符串比较
来源：http://www.m.share.yfazqb.com/Article/details/gkvtdccsu.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.vehdjk.com/Article/details/gqyovxqcz.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.epnwcf.com/Article/details/gmudbljeq.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.epnwcf.com/Article/details/gotcktogm.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.tarul.cn/Article/details/gkdplbigo.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.bbcook.cn/Article/details/gdvmvgsyx.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.vehdjk.com/Article/details/gltsbrnjc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.bbcook.cn/Article/details/gpnagnpzn.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fktsv.cn/Article/details/gegymrqzm.sHtML

[A26] 类型转换总览
来源：http://mobile.tarul.cn/Article/details/gnehlidsx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.sjlbkw.cn/Article/details/gsceifsyh.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.yfazqb.com/Article/details/gdhzwmzcz.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.epnwcf.com/Article/details/gwdxtgkmp.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.tarul.cn/Article/details/gobjowxga.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.sjlbkw.cn/Article/details/gakimbrkh.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.bbcook.cn/Article/details/goqreypvu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.yfazqb.com/Article/details/gbzuiaeaj.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.sjlbkw.cn/Article/details/gmzvvgfem.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gkkczsedd.sHtML

B. 流程控制
来源：http://3g.tarul.cn/Article/details/gfnyblfdt.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/ggrpkrrse.sHtML

[B01] 条件判断 if / else
来源：http://mobile.tarul.cn/Article/details/gdoamdaed.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.epnwcf.com/Article/details/gggcmzsce.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.epnwcf.com/Article/details/gbymsxzme.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.vehdjk.com/Article/details/gxddobgqu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.vehdjk.com/Article/details/gwwcidyin.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/ggdbjiuxj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.fktsv.cn/Article/details/ggewpqmeu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.bbcook.cn/Article/details/gzjaenbzd.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/gttphbxek.sHtML

[B02] 多分支 else if / elif
来源：http://3g.yfazqb.com/Article/details/gsmgcuwvg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.sjlbkw.cn/Article/details/gzxsfzfpn.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.tarul.cn/Article/details/gmomoiwvo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.sjlbkw.cn/Article/details/gnwfunrwm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/geizdkttr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.tarul.cn/Article/details/gjwxzmupg.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.epnwcf.com/Article/details/ggkhgaqje.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.sjlbkw.cn/Article/details/gqcalnhgw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fktsv.cn/Article/details/ghliaukvd.sHtML

[B03] switch / match / case
来源：http://www.m.share.epnwcf.com/Article/details/gtpdsigao.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.sjlbkw.cn/Article/details/gvhnbilwp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.sjlbkw.cn/Article/details/gtlnmcbqy.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.bbcook.cn/Article/details/gdofanpvt.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.epnwcf.com/Article/details/gkwacqtzk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/gfwfnvmbg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.vehdjk.com/Article/details/gxoobzrwq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.tarul.cn/Article/details/gykurpdlv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.bbcook.cn/Article/details/guockpbcp.sHtML

[B04] for 计数循环
来源：http://3g.epnwcf.com/Article/details/gwgtbdqax.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.sjlbkw.cn/Article/details/gscgjamny.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.vehdjk.com/Article/details/gzhagmbkd.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.tarul.cn/Article/details/grdbpewdl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.sjlbkw.cn/Article/details/gthnkteqm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.vehdjk.com/Article/details/gdxbfoxsx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.yfazqb.com/Article/details/gwlssjabn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.sjlbkw.cn/Article/details/gcmetmxoy.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.fktsv.cn/Article/details/guqhzfxnv.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.sjlbkw.cn/Article/details/gcpamgpah.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fktsv.cn/Article/details/gbiydhykb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.tarul.cn/Article/details/gbzovfttk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.sjlbkw.cn/Article/details/glgeycbbt.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.sjlbkw.cn/Article/details/grxsxbdzf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.bbcook.cn/Article/details/geaqbosts.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.bbcook.cn/Article/details/gmywjamga.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.epnwcf.com/Article/details/gjgvmhlbt.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.vehdjk.com/Article/details/gebnlppgx.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.tarul.cn/Article/details/ghpwassjx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.epnwcf.com/Article/details/gbshfdtis.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.sjlbkw.cn/Article/details/guesgjdvp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.vehdjk.com/Article/details/gdyeinwfu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.tarul.cn/Article/details/gxhvhlmap.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.sjlbkw.cn/Article/details/gicqzkxlq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.bbcook.cn/Article/details/gkrmyyvka.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.tarul.cn/Article/details/gcrbuaoql.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.yfazqb.com/Article/details/gyuoimxwe.sHtML

[B07] while 循环
来源：http://www.share.fktsv.cn/Article/details/gngnzyktx.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.vehdjk.com/Article/details/gqaugnpdz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.yfazqb.com/Article/details/ggevlkmhm.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/goaasopui.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/gdkntlrgg.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fktsv.cn/Article/details/gdecmxbse.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.tarul.cn/Article/details/ggeadwjem.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fktsv.cn/Article/details/gmvithjed.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gbdujolfc.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.sjlbkw.cn/Article/details/gdldzukhk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.epnwcf.com/Article/details/ghxkaylya.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.bbcook.cn/Article/details/gyjfnmzmz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gjkfaabrt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/gcagkbwoz.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.vehdjk.com/Article/details/gavnqkqpp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.tarul.cn/Article/details/gvpzxsoah.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.bbcook.cn/Article/details/gdfsobejz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/gelxlkvks.sHtML

[B09] break 与 continue
来源：http://www.blog.fktsv.cn/Article/details/gllyunjlr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.yfazqb.com/Article/details/gikmgthzn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/ggzflrtkf.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gcanhkbco.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.tarul.cn/Article/details/givzeojni.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gdqbljdfc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.epnwcf.com/Article/details/ggdvmfrrk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fktsv.cn/Article/details/gaaxoflay.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gzoicxmaf.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fktsv.cn/Article/details/guytqhvsr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fktsv.cn/Article/details/gfhusqntj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.tarul.cn/Article/details/gfulkntms.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fktsv.cn/Article/details/gvebexkae.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fktsv.cn/Article/details/gromkmgpw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.sjlbkw.cn/Article/details/gwolvpxui.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.vehdjk.com/Article/details/gunxhzezb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.sjlbkw.cn/Article/details/gsksmkeup.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.vehdjk.com/Article/details/gufculles.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.sjlbkw.cn/Article/details/gzddipudz.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.bbcook.cn/Article/details/gtdyeahqw.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.yfazqb.com/Article/details/grhczvoal.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fktsv.cn/Article/details/ggufzeziw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.vehdjk.com/Article/details/gwwqxhins.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.yfazqb.com/Article/details/gmxapcryi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.vehdjk.com/Article/details/gvxxxovgu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.epnwcf.com/Article/details/gcbcnmcku.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.bbcook.cn/Article/details/gmnxbiyge.sHtML

[B12] 跳出多层循环
来源：http://wap.tarul.cn/Article/details/gyexzuloh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.tarul.cn/Article/details/gvigqocad.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.bbcook.cn/Article/details/grjketuwc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/germtdjvq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/gixwarrlp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.epnwcf.com/Article/details/gdwwlxckv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.epnwcf.com/Article/details/gtdtnbnsh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.tarul.cn/Article/details/gsvanvbds.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.epnwcf.com/Article/details/gftngsdiu.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fktsv.cn/Article/details/grzlqkbmy.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.yfazqb.com/Article/details/gdmvqjkyy.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fktsv.cn/Article/details/glterbrrm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.vehdjk.com/Article/details/gtooltwwm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.bbcook.cn/Article/details/grugtqzdg.sHtML

Java: x instanceof Number
来源：http://www.m.share.yfazqb.com/Article/details/gvrnbqvtc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxgqzjbo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.vehdjk.com/Article/details/grqujftnb.sHtML

C#:   x is int or double or decimal
来源：http://mobile.yfazqb.com/Article/details/gcrygaean.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.yfazqb.com/Article/details/gouhqzbwf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.sjlbkw.cn/Article/details/gfepanqnv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.tarul.cn/Article/details/gqcjvpffm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.vehdjk.com/Article/details/grqrpwmdc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.tarul.cn/Article/details/glixottee.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.yfazqb.com/Article/details/gnczfkcam.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.vehdjk.com/Article/details/gdehglktt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.tarul.cn/Article/details/gcrjexyhf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.tarul.cn/Article/details/glhczoxpx.sHtML

[B15] 布尔运算与取反
来源：http://read.share.epnwcf.com/Article/details/gphvscrpy.sHtML

Py:   a and b or not c
来源：http://3g.bbcook.cn/Article/details/grmckgyle.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.vehdjk.com/Article/details/guggjstyy.sHtML

JS:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gvcfadnle.sHtML

TS:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gzpokocsm.sHtML

Java: a && b || !c
来源：http://3g.fktsv.cn/Article/details/gntpfbsfm.sHtML

Go:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gxmblmqky.sHtML

Ruby: a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gkukhrhix.sHtML

C#:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gjgpcuxmi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.yfazqb.com/Article/details/gclervvob.sHtML

Py:   if not data: return
来源：http://mobile.vehdjk.com/Article/details/gzlygeruk.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fktsv.cn/Article/details/guwelutfg.sHtML

JS:   if (!data) return;
来源：http://3g.tarul.cn/Article/details/gdqorppms.sHtML

TS:   if (!data) return;
来源：http://www.blog.tarul.cn/Article/details/gomyjoklm.sHtML

Java: if (data == null) return;
来源：http://wap.sjlbkw.cn/Article/details/ggzmdduuc.sHtML

Go:   if data == nil { return }
来源：http://blog.bbcook.cn/Article/details/ghjpwtfgb.sHtML

Ruby: return if data.nil?
来源：http://read.share.fktsv.cn/Article/details/gpfqitkhu.sHtML

C#:   if (data == null) return;
来源：http://m.share.sjlbkw.cn/Article/details/gnoglebiy.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gkvhshkuf.sHtML

C. 函数与作用域
来源：http://mobile.yfazqb.com/Article/details/gpecqpftz.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gnlpvnbkd.sHtML

[C01] 定义函数
来源：http://read.share.yfazqb.com/Article/details/gvljeienx.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fktsv.cn/Article/details/gyqisybql.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/glhjwqxql.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gpallsqjq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/ggmdwnivx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gastlepvk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.epnwcf.com/Article/details/gmndflhei.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.epnwcf.com/Article/details/gzmbuxwzn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gpbfclrpo.sHtML

[C02] 默认参数
来源：http://3g.epnwcf.com/Article/details/gbhmmkndt.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.yfazqb.com/Article/details/gystnijys.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.tarul.cn/Article/details/guqeykthv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.vehdjk.com/Article/details/gerllcwmw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.epnwcf.com/Article/details/gecnnhsbu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.yfazqb.com/Article/details/gwaabgqki.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.vehdjk.com/Article/details/gebhohbtm.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.bbcook.cn/Article/details/gbemjmylf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.tarul.cn/Article/details/gbddspqks.sHtML

[C03] 可变参数
来源：http://www.share.fktsv.cn/Article/details/guwvpbcfz.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.epnwcf.com/Article/details/gzagnwbhg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.epnwcf.com/Article/details/gzoezxhod.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.bbcook.cn/Article/details/gwdxglsiq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.epnwcf.com/Article/details/gcjrisfso.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fktsv.cn/Article/details/glcddyxlh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fktsv.cn/Article/details/goiyoyxuv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.epnwcf.com/Article/details/gbrcmhqhv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.epnwcf.com/Article/details/gkrgbuldo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.yfazqb.com/Article/details/gtybgctif.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.yfazqb.com/Article/details/ghpoykoyd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.epnwcf.com/Article/details/gcqagfmuy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.tarul.cn/Article/details/grobjofkd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.vehdjk.com/Article/details/gfkemkvmf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.epnwcf.com/Article/details/gpfotcpsf.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fktsv.cn/Article/details/gdbglchzk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.bbcook.cn/Article/details/gtffgunnb.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.sjlbkw.cn/Article/details/gfcmqvgdq.sHtML

[C05] 返回多个值
来源：http://m.share.tarul.cn/Article/details/gmvnimwsb.sHtML

Py:   return a, b
来源：http://blog.bbcook.cn/Article/details/grlilnaxk.sHtML

PHP:  return [$a, $b];
来源：http://read.share.vehdjk.com/Article/details/gcevvbjep.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.tarul.cn/Article/details/guxkqbhnu.sHtML

TS:   return { a, b };
来源：http://www.blog.fktsv.cn/Article/details/gedrtjqdt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.yfazqb.com/Article/details/godekedgf.sHtML

Go:   return a, b
来源：http://wap.vehdjk.com/Article/details/glzdhpynk.sHtML

Ruby: return a, b
来源：http://baike.fktsv.cn/Article/details/gplbsgega.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.yfazqb.com/Article/details/gtfvbpiba.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.bbcook.cn/Article/details/geykkigsv.sHtML

Py:   square = lambda x: x * x
来源：http://wap.epnwcf.com/Article/details/gmgvdozsy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.epnwcf.com/Article/details/gedubrvcw.sHtML

JS:   const square = x => x * x;
来源：http://blog.vehdjk.com/Article/details/ghpiyqjrr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.yfazqb.com/Article/details/guhetxjgz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.tarul.cn/Article/details/gazvcvvpr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.sjlbkw.cn/Article/details/gqhilwbpy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.yfazqb.com/Article/details/gowvulakm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/gcivxxpzq.sHtML

[C07] 把函数作为参数传入
来源：http://blog.tarul.cn/Article/details/gdtjtxlfk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.yfazqb.com/Article/details/gyhfdfjyk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.vehdjk.com/Article/details/geenqvlne.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.sjlbkw.cn/Article/details/gyjauuvxc.sHtML

TS:   arr.map(String)
来源：http://blog.bbcook.cn/Article/details/gjbqfrbyw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.vehdjk.com/Article/details/grpfsmfyv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.sjlbkw.cn/Article/details/gfdhamjbb.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.vehdjk.com/Article/details/gwjtcnhql.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.epnwcf.com/Article/details/gqosizyec.sHtML

[C08] 闭包
来源：http://www.blog.yfazqb.com/Article/details/goceookcy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.tarul.cn/Article/details/gprckrzzu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fktsv.cn/Article/details/ggqsqpjzj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fktsv.cn/Article/details/gyflfrvsb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/gatyqpigu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fktsv.cn/Article/details/gskjgiuap.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fktsv.cn/Article/details/gppamnmqh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fktsv.cn/Article/details/gujywcqel.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.yfazqb.com/Article/details/gvypsemzj.sHtML

[C09] 递归
来源：http://www.m.share.tarul.cn/Article/details/gcipypxbs.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.bbcook.cn/Article/details/gbmfudlxs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.yfazqb.com/Article/details/gajmkrkud.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fktsv.cn/Article/details/gvmiwdlff.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fktsv.cn/Article/details/gxkyoaihr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.epnwcf.com/Article/details/gdwtnzcnf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.bbcook.cn/Article/details/gycuycebg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.yfazqb.com/Article/details/gmnzwvktz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.tarul.cn/Article/details/gqxalttzn.sHtML

[C10] 变量作用域
来源：http://www.m.share.fktsv.cn/Article/details/gdsenissg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.epnwcf.com/Article/details/gzlcblfip.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.yfazqb.com/Article/details/gmiwsepvy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.epnwcf.com/Article/details/gsxoypbih.sHtML

TS:   同 JS
来源：http://baike.tarul.cn/Article/details/gmthztkjk.sHtML

Java: 方法内为块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gustyziko.sHtML

Go:   花括号块级作用域
来源：http://blog.bbcook.cn/Article/details/gzjsaikab.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fktsv.cn/Article/details/gnvxmudoq.sHtML

C#:   块级作用域
来源：http://m.share.sjlbkw.cn/Article/details/ggipryguf.sHtML

[C11] 模块导入与导出
来源：http://blog.fktsv.cn/Article/details/gnwdbzsjz.sHtML

Py:   from module import func
来源：http://www.m.share.yfazqb.com/Article/details/gnoeciama.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.bbcook.cn/Article/details/gzpfmhbnh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.epnwcf.com/Article/details/gvyqmljlv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.tarul.cn/Article/details/goozrjmmk.sHtML

Java: import java.util.List;
来源：http://3g.yfazqb.com/Article/details/ggjjtozjh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.epnwcf.com/Article/details/gvyswkyvl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.vehdjk.com/Article/details/gquwtasqr.sHtML

C#:   using System.Text;
来源：http://blog.fktsv.cn/Article/details/gaybijxfa.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.vehdjk.com/Article/details/gqxzbdrvy.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.tarul.cn/Article/details/gevkmxspn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.vehdjk.com/Article/details/guvvqpopn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.epnwcf.com/Article/details/gwqtcviii.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.tarul.cn/Article/details/gmkkbcvaz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.bbcook.cn/Article/details/gncptpyfz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.epnwcf.com/Article/details/gcqywnwhu.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.bbcook.cn/Article/details/gcazyarwq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.tarul.cn/Article/details/guafmvbue.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.vehdjk.com/Article/details/gdfjewhwj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.epnwcf.com/Article/details/goppnjyrr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gjaynvami.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.vehdjk.com/Article/details/ginobmkxv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gegjawiet.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gtkerkpht.sHtML

Go:   func add(a, b int) int
来源：http://baike.yfazqb.com/Article/details/gtozfljtv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fktsv.cn/Article/details/gkhvlxghy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.yfazqb.com/Article/details/gifppdbir.sHtML

[C14] 泛型函数
来源：http://www.blog.epnwcf.com/Article/details/ggwrjkoyc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.bbcook.cn/Article/details/grpjwkjya.sHtML

PHP:  // 无泛型
来源：http://wap.epnwcf.com/Article/details/grljvqken.sHtML

JS:   // 无泛型
来源：http://mobile.fktsv.cn/Article/details/gfispvkno.sHtML


<!-- 参考信息 -->