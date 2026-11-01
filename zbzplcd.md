代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://blog.tarul.cn/Article/details/gjlwwlgvl.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.epnwcf.com/Article/details/gwvvluvfo.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fktsv.cn/Article/details/gbnxqrnbj.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.bbcook.cn/Article/details/gwnmyabyt.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.yfazqb.com/Article/details/guebdfrqe.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.bbcook.cn/Article/details/guvoodowo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.tarul.cn/Article/details/glqxccpgn.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.epnwcf.com/Article/details/grljaorgf.sHtML

[A26] 类型转换总览
来源：http://blog.fktsv.cn/Article/details/gbussjyuw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.vehdjk.com/Article/details/gdvfoehdf.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fktsv.cn/Article/details/gciledtsh.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.yfazqb.com/Article/details/gbuppubmg.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.yfazqb.com/Article/details/gvxazqknq.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.bbcook.cn/Article/details/gsaucqvzt.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.bbcook.cn/Article/details/gtjrkhtsz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.epnwcf.com/Article/details/gfflhcwzn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.tarul.cn/Article/details/gmrchumxk.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gnnimfikh.sHtML

B. 流程控制
来源：http://mobile.bbcook.cn/Article/details/gaqjitltz.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ggjthfpda.sHtML

[B01] 条件判断 if / else
来源：http://mobile.fktsv.cn/Article/details/ghevtwybo.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.epnwcf.com/Article/details/gzuhjyptp.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.bbcook.cn/Article/details/gxeivvzbs.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fktsv.cn/Article/details/gbogmrfwx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.yfazqb.com/Article/details/ggrarcgnb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.yfazqb.com/Article/details/gbxddxepz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.yfazqb.com/Article/details/gdonghgks.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.bbcook.cn/Article/details/gxalfphce.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/gwpatkdwd.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.sjlbkw.cn/Article/details/gitatqnoh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.bbcook.cn/Article/details/gmdxstjtm.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.tarul.cn/Article/details/gdlisglvl.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gjxnqclkz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/gbqnttxsm.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.sjlbkw.cn/Article/details/gxttvkcra.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.epnwcf.com/Article/details/gtltuyvwf.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzosvqkb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/gqxqrsjqs.sHtML

[B03] switch / match / case
来源：http://www.share.vehdjk.com/Article/details/gurlbklec.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.tarul.cn/Article/details/gokjysljy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.tarul.cn/Article/details/gvciotqbi.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.sjlbkw.cn/Article/details/gwbchkzdt.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/gvgvbntbg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/gmoujuwsj.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.sjlbkw.cn/Article/details/gwyqudbsz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.bbcook.cn/Article/details/geuyrgqzu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.vehdjk.com/Article/details/gpwjhkzzf.sHtML

[B04] for 计数循环
来源：http://www.share.tarul.cn/Article/details/gdcvuaiwq.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.sjlbkw.cn/Article/details/gbvtmdxbt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.vehdjk.com/Article/details/gsoyozdgr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.tarul.cn/Article/details/gzlbzwryt.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fktsv.cn/Article/details/gkmkmfmld.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.vehdjk.com/Article/details/gnvhqxqdz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.epnwcf.com/Article/details/glhelfpam.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.tarul.cn/Article/details/gzbwbmlsz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.tarul.cn/Article/details/gmjgmibvo.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.epnwcf.com/Article/details/ggdrdwohl.sHtML

Py:   for item in arr: print(item)
来源：http://wap.fktsv.cn/Article/details/grynrtxzt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fktsv.cn/Article/details/gvioistuk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fktsv.cn/Article/details/geocvxyrk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.vehdjk.com/Article/details/gspvnosvx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.fktsv.cn/Article/details/gcqrqdafc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjkuucnz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.yfazqb.com/Article/details/gxsoyluhd.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.sjlbkw.cn/Article/details/ggslbyekm.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.yfazqb.com/Article/details/gxkcgrrpo.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fktsv.cn/Article/details/gocrzvahp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.epnwcf.com/Article/details/gnklgezfx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.sjlbkw.cn/Article/details/ggigblrql.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.tarul.cn/Article/details/ghevwochr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.yfazqb.com/Article/details/gcnwuadjk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.tarul.cn/Article/details/giqqokdxl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.vehdjk.com/Article/details/gayrcjrzp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.vehdjk.com/Article/details/gtdwppvkm.sHtML

[B07] while 循环
来源：http://read.share.vehdjk.com/Article/details/gjqcvmbhl.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.bbcook.cn/Article/details/gptxnhoum.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fktsv.cn/Article/details/gyfpribev.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gbbzcvqlo.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/gutdatlsg.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gsujqsfgu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.yfazqb.com/Article/details/gvmjistks.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.vehdjk.com/Article/details/gceaavjec.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/gyokdjwkz.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.yfazqb.com/Article/details/gorxuzbom.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.tarul.cn/Article/details/gjaqpxgfh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.vehdjk.com/Article/details/gbymcyjqw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gbmuxbepc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gxelozgtc.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.yfazqb.com/Article/details/gjkikaifd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.bbcook.cn/Article/details/gjngwcpgl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.fktsv.cn/Article/details/ghutgzswh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gironsapx.sHtML

[B09] break 与 continue
来源：http://blog.yfazqb.com/Article/details/gwlvwranf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fktsv.cn/Article/details/gcgrbhdmm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/gqrabogfd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/guhtxqbrx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gikkfzpce.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gswxwqawo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fktsv.cn/Article/details/gdhymxrzk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fktsv.cn/Article/details/gkjluiekd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gjyywpuhc.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fktsv.cn/Article/details/gdrkvwovt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.sjlbkw.cn/Article/details/ggridkmor.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.tarul.cn/Article/details/gqhocytaz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.tarul.cn/Article/details/gofyocdtu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.yfazqb.com/Article/details/gmfietggg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.vehdjk.com/Article/details/giztyjhks.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fktsv.cn/Article/details/gicymoasw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.vehdjk.com/Article/details/gsjlexzdo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.sjlbkw.cn/Article/details/gokpxuomt.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwmxzvmc.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.sjlbkw.cn/Article/details/ghgsfpenx.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.bbcook.cn/Article/details/gxflptynn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.sjlbkw.cn/Article/details/gqsamdmqe.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.yfazqb.com/Article/details/gnaglvycf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.bbcook.cn/Article/details/ggqqsxmxb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.vehdjk.com/Article/details/ginizxshj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fktsv.cn/Article/details/gbmpwtoer.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.yfazqb.com/Article/details/goycvkcmu.sHtML

[B12] 跳出多层循环
来源：http://www.share.tarul.cn/Article/details/gecbmadeg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.vehdjk.com/Article/details/gyhrhsuqy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.yfazqb.com/Article/details/gkapcxhsi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.tarul.cn/Article/details/ghutlaqnk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/gqzhkwwbs.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.bbcook.cn/Article/details/gxvsbvdqd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.vehdjk.com/Article/details/gcblugreh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.vehdjk.com/Article/details/gxjcfdqku.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.tarul.cn/Article/details/gtlqklsvb.sHtML

[B13] 判断是否为数字
来源：http://www.share.tarul.cn/Article/details/glxeweeic.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.vehdjk.com/Article/details/goxorlqiz.sHtML

PHP:  is_numeric($x)
来源：http://m.share.sjlbkw.cn/Article/details/ggztkspew.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.bbcook.cn/Article/details/gvxtievbm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.yfazqb.com/Article/details/gtysfkise.sHtML

Java: x instanceof Number
来源：http://m.share.bbcook.cn/Article/details/grekmikaa.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.bbcook.cn/Article/details/glzkafzhk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.tarul.cn/Article/details/gsdycolmw.sHtML

C#:   x is int or double or decimal
来源：http://www.share.tarul.cn/Article/details/gtjmuzsia.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.vehdjk.com/Article/details/gbaotdqiq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.vehdjk.com/Article/details/gmcvcoqqj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fktsv.cn/Article/details/gxlabadws.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.sjlbkw.cn/Article/details/giaqmtqiy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.yfazqb.com/Article/details/gpivcxfyh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.yfazqb.com/Article/details/gqkzkcyne.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.vehdjk.com/Article/details/gdusqwgxz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.vehdjk.com/Article/details/gwsuuicea.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gucxttbqz.sHtML

[B15] 布尔运算与取反
来源：http://mobile.bbcook.cn/Article/details/glbdnropi.sHtML

Py:   a and b or not c
来源：http://www.blog.yfazqb.com/Article/details/glahedply.sHtML

PHP:  $a && $b || !$c
来源：http://wap.sjlbkw.cn/Article/details/gscozucwl.sHtML

JS:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/ggexpomvu.sHtML

TS:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gbvxnahsx.sHtML

Java: a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/ggadfefuo.sHtML

Go:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gyiyrmubb.sHtML

Ruby: a && b || !c
来源：http://blog.tarul.cn/Article/details/grcljjvdv.sHtML

C#:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gkvtvzbhh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.yfazqb.com/Article/details/gbjnjtqtt.sHtML

Py:   if not data: return
来源：http://www.share.bbcook.cn/Article/details/gcnrsutyh.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.sjlbkw.cn/Article/details/gmfoqpzgz.sHtML

JS:   if (!data) return;
来源：http://read.share.vehdjk.com/Article/details/gkaxnafyw.sHtML

TS:   if (!data) return;
来源：http://www.m.share.vehdjk.com/Article/details/gdrltmghr.sHtML

Java: if (data == null) return;
来源：http://baike.vehdjk.com/Article/details/gjrjzxnqq.sHtML

Go:   if data == nil { return }
来源：http://www.blog.bbcook.cn/Article/details/guerdsauc.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.tarul.cn/Article/details/gmwwnlffl.sHtML

C#:   if (data == null) return;
来源：http://baike.bbcook.cn/Article/details/glxkddniq.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gfzlyhmit.sHtML

C. 函数与作用域
来源：http://3g.bbcook.cn/Article/details/gzpbgqvdc.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gisispgbd.sHtML

[C01] 定义函数
来源：http://www.m.share.bbcook.cn/Article/details/gecdanhpb.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.bbcook.cn/Article/details/gznhxrshi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gqvbvjaok.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gjyunkkhf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gvxsfrhsj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gecwossou.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.bbcook.cn/Article/details/gegzlxtnc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fktsv.cn/Article/details/glcqmvzmw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gpwcjxzvq.sHtML

[C02] 默认参数
来源：http://blog.epnwcf.com/Article/details/gvjpsyylc.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.tarul.cn/Article/details/goteuhasb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.sjlbkw.cn/Article/details/gipcgmhpb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.bbcook.cn/Article/details/gnuvedupi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.epnwcf.com/Article/details/gjoinqsuo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fktsv.cn/Article/details/gpaxcwjsl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.tarul.cn/Article/details/gdbxnaosl.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fktsv.cn/Article/details/gdcfdihqs.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.tarul.cn/Article/details/gowsnlcex.sHtML

[C03] 可变参数
来源：http://read.share.vehdjk.com/Article/details/gxxbwohpt.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.bbcook.cn/Article/details/gfgtzpxos.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.sjlbkw.cn/Article/details/gnwzllnch.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.vehdjk.com/Article/details/gypeqzyco.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.yfazqb.com/Article/details/gatcoztso.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.bbcook.cn/Article/details/gcjbkoskq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.vehdjk.com/Article/details/gvvnypjgx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.vehdjk.com/Article/details/ggwoekxcn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fktsv.cn/Article/details/gbwvcjezg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.vehdjk.com/Article/details/ggrxcqiub.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.epnwcf.com/Article/details/giogxefob.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.tarul.cn/Article/details/gtvxrfcio.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.yfazqb.com/Article/details/gdivddzoc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.epnwcf.com/Article/details/gprfpptoz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.sjlbkw.cn/Article/details/gsrsyacke.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.tarul.cn/Article/details/gbtonybej.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.vehdjk.com/Article/details/groqpknwi.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/gsrajxbfh.sHtML

[C05] 返回多个值
来源：http://www.blog.fktsv.cn/Article/details/gvudbfztc.sHtML

Py:   return a, b
来源：http://wap.epnwcf.com/Article/details/gncygrdep.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gktqcsizi.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fktsv.cn/Article/details/gofhihmkp.sHtML

TS:   return { a, b };
来源：http://www.blog.sjlbkw.cn/Article/details/glrmfoksa.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.epnwcf.com/Article/details/gymzdhcpq.sHtML

Go:   return a, b
来源：http://www.share.yfazqb.com/Article/details/gcucxljxt.sHtML

Ruby: return a, b
来源：http://www.m.share.epnwcf.com/Article/details/gzqqhxlhl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.bbcook.cn/Article/details/gkroqyjgd.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fktsv.cn/Article/details/gztoqjkdg.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.epnwcf.com/Article/details/gkmpstmnh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.tarul.cn/Article/details/gwqzeevqt.sHtML

JS:   const square = x => x * x;
来源：http://m.share.yfazqb.com/Article/details/gvkycyvbw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.sjlbkw.cn/Article/details/gzlhkcklb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.yfazqb.com/Article/details/gwuvtdrzr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.vehdjk.com/Article/details/gfljzejeo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.vehdjk.com/Article/details/gbabvcexw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.yfazqb.com/Article/details/gdlaphjsp.sHtML

[C07] 把函数作为参数传入
来源：http://3g.vehdjk.com/Article/details/gdxbjbjty.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.bbcook.cn/Article/details/gsdwlljhx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/grquyrrlk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.bbcook.cn/Article/details/ghbzmdlui.sHtML

TS:   arr.map(String)
来源：http://www.share.sjlbkw.cn/Article/details/gweehajeg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.bbcook.cn/Article/details/gylnkrdoe.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.tarul.cn/Article/details/gypbxbhfc.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.yfazqb.com/Article/details/ghheaglvj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.tarul.cn/Article/details/gtojtqiyg.sHtML

[C08] 闭包
来源：http://baike.bbcook.cn/Article/details/glplggeaf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.epnwcf.com/Article/details/gwlyzhcnh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.epnwcf.com/Article/details/gatxqutor.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/gxetuutdl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/gzlpzdkrf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.bbcook.cn/Article/details/ggfqmoxzy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.yfazqb.com/Article/details/gqmluclow.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.tarul.cn/Article/details/grtscfqvb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/giyiegpcl.sHtML

[C09] 递归
来源：http://blog.sjlbkw.cn/Article/details/gwjsfvjyt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.vehdjk.com/Article/details/gxmnwudlv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.tarul.cn/Article/details/gebvrylwm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.yfazqb.com/Article/details/gzfkutymj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.epnwcf.com/Article/details/goftozzfu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fktsv.cn/Article/details/ghhmrtvwl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.yfazqb.com/Article/details/guvkjnmao.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.yfazqb.com/Article/details/gnnvbajpg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.yfazqb.com/Article/details/grzzwoibc.sHtML

[C10] 变量作用域
来源：http://wap.fktsv.cn/Article/details/gqurjwmvl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.epnwcf.com/Article/details/gofqvfomw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.yfazqb.com/Article/details/glszfqafo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.vehdjk.com/Article/details/gvxxtxebr.sHtML

TS:   同 JS
来源：http://read.share.bbcook.cn/Article/details/gmqnqmitu.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fktsv.cn/Article/details/glllijjdc.sHtML

Go:   花括号块级作用域
来源：http://baike.fktsv.cn/Article/details/gtxvatiem.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fktsv.cn/Article/details/gndwpjzox.sHtML

C#:   块级作用域
来源：http://wap.epnwcf.com/Article/details/geryytrwk.sHtML

[C11] 模块导入与导出
来源：http://3g.yfazqb.com/Article/details/grwyuxmcd.sHtML

Py:   from module import func
来源：http://blog.tarul.cn/Article/details/gzmpvfeyu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.tarul.cn/Article/details/gqhlfctki.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.yfazqb.com/Article/details/gutrwvuik.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.sjlbkw.cn/Article/details/gntnogmxc.sHtML

Java: import java.util.List;
来源：http://blog.fktsv.cn/Article/details/ggacpjtva.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.yfazqb.com/Article/details/geeeuqhvb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.yfazqb.com/Article/details/gvmogbmqv.sHtML

C#:   using System.Text;
来源：http://3g.tarul.cn/Article/details/gzxobzenw.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrinqdlz.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fktsv.cn/Article/details/gzujnhueo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.bbcook.cn/Article/details/gisdcgpxi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.bbcook.cn/Article/details/gljkgbrzo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.sjlbkw.cn/Article/details/gspuchfiv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.epnwcf.com/Article/details/gijpkdlan.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.epnwcf.com/Article/details/gbwkcoxxt.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.bbcook.cn/Article/details/gbyheypuy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.vehdjk.com/Article/details/gtxwcxhgm.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.epnwcf.com/Article/details/ggaczatre.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.yfazqb.com/Article/details/ggheufmdi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.epnwcf.com/Article/details/gouinecjm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.tarul.cn/Article/details/gaglxnjhw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gsovcyeba.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gdjhqrjrj.sHtML

Go:   func add(a, b int) int
来源：http://mobile.sjlbkw.cn/Article/details/gsuiquecf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.yfazqb.com/Article/details/govdiqure.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.vehdjk.com/Article/details/gzxazkpsa.sHtML

[C14] 泛型函数
来源：http://mobile.tarul.cn/Article/details/gajvjkftg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.tarul.cn/Article/details/gkrpdhgdy.sHtML

PHP:  // 无泛型
来源：http://read.share.vehdjk.com/Article/details/gjcehfhup.sHtML

JS:   // 无泛型
来源：http://baike.tarul.cn/Article/details/grectouxy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcyeyxojh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.yfazqb.com/Article/details/guklmtqio.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.sjlbkw.cn/Article/details/gxogikrxe.sHtML

Ruby: # 无泛型
来源：http://3g.sjlbkw.cn/Article/details/gvqhoyjnd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.yfazqb.com/Article/details/gjadmuynd.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.bbcook.cn/Article/details/gpydddhcx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.vehdjk.com/Article/details/gewukkgbr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.epnwcf.com/Article/details/gxxyquzin.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.yfazqb.com/Article/details/gxrciwejc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fktsv.cn/Article/details/ggpskonmz.sHtML

Java: // 无解构
来源：http://wap.tarul.cn/Article/details/gjkbocpfz.sHtML

Go:   // 无解构
来源：http://3g.tarul.cn/Article/details/guoyoddoq.sHtML


<!-- 参考信息 -->