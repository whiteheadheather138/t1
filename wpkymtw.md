代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.yfazqb.com/Article/details/gfgovtttk.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.vehdjk.com/Article/details/guzcxnffl.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.bbcook.cn/Article/details/gwvmdyyjo.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.bbcook.cn/Article/details/gkmnqnhud.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.yfazqb.com/Article/details/gjqhxbnzg.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.yfazqb.com/Article/details/gkcfijcdk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.tarul.cn/Article/details/gukwurjki.sHtML

[A25] 字符串比较
来源：http://wap.vehdjk.com/Article/details/gxgnziaeh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.epnwcf.com/Article/details/gqexgofgx.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.epnwcf.com/Article/details/grltwmkjb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.sjlbkw.cn/Article/details/gvukunksf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.sjlbkw.cn/Article/details/grehlucad.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.sjlbkw.cn/Article/details/gpkaaqpex.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.epnwcf.com/Article/details/gvqvjjjrb.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.sjlbkw.cn/Article/details/gmhcpghxb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.fktsv.cn/Article/details/gzieoatao.sHtML

[A26] 类型转换总览
来源：http://www.blog.fktsv.cn/Article/details/glypzumpj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.yfazqb.com/Article/details/ghfcqkjjb.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.fktsv.cn/Article/details/grbbgtknb.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.yfazqb.com/Article/details/gdtkcyffw.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.epnwcf.com/Article/details/gvchlersz.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.fktsv.cn/Article/details/gjvlzyqjk.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.epnwcf.com/Article/details/gjfedbzrb.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.vehdjk.com/Article/details/gdibbjgul.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.sjlbkw.cn/Article/details/gmupqlguy.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gvxzhhbju.sHtML

B. 流程控制
来源：http://read.share.yfazqb.com/Article/details/gwraeahqk.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/grukdzsqf.sHtML

[B01] 条件判断 if / else
来源：http://3g.vehdjk.com/Article/details/goxopuidf.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fktsv.cn/Article/details/gpiwtcgzd.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.tarul.cn/Article/details/ggrpijidc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.bbcook.cn/Article/details/gdxbtkyiv.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.sjlbkw.cn/Article/details/gwuhzingi.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/gijscbaki.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.bbcook.cn/Article/details/ggtpnlsjy.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.vehdjk.com/Article/details/gbgiqytvm.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.epnwcf.com/Article/details/gelrebjaj.sHtML

[B02] 多分支 else if / elif
来源：http://blog.sjlbkw.cn/Article/details/gjsittvjy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.sjlbkw.cn/Article/details/gxquhkflt.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.tarul.cn/Article/details/glpbhyhgs.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.vehdjk.com/Article/details/gmynmsmdz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.yfazqb.com/Article/details/gwwyiatuk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.yfazqb.com/Article/details/glbvidqva.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.sjlbkw.cn/Article/details/gaztvyknx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.yfazqb.com/Article/details/gecnshpkh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.bbcook.cn/Article/details/gielwevuu.sHtML

[B03] switch / match / case
来源：http://www.m.share.yfazqb.com/Article/details/gprexjpvh.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fktsv.cn/Article/details/gruhqmobo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fktsv.cn/Article/details/ggyfapcjd.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.yfazqb.com/Article/details/ggzkusvri.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.sjlbkw.cn/Article/details/gmokcwfou.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/ggzbxcyav.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fktsv.cn/Article/details/ggythcwoh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.tarul.cn/Article/details/gdqfmyuqx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fktsv.cn/Article/details/givwpzzba.sHtML

[B04] for 计数循环
来源：http://3g.vehdjk.com/Article/details/gqpmgdjfp.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.tarul.cn/Article/details/gbwagoeuj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.bbcook.cn/Article/details/grppekzsv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.yfazqb.com/Article/details/gagzinasq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.tarul.cn/Article/details/gkzcczgsw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.fktsv.cn/Article/details/gogkfyuch.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.fktsv.cn/Article/details/gdcywnenn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.tarul.cn/Article/details/gluryufxn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.yfazqb.com/Article/details/gjxuurfny.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.sjlbkw.cn/Article/details/gvevghaqj.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.vehdjk.com/Article/details/gkiffutzo.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.yfazqb.com/Article/details/gficllwwg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.yfazqb.com/Article/details/gcciouchh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fktsv.cn/Article/details/ghbzditfw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.sjlbkw.cn/Article/details/gegiehefp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.tarul.cn/Article/details/gjmjfozuf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.vehdjk.com/Article/details/gfxkbwhyi.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.epnwcf.com/Article/details/ggvdwtytq.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.bbcook.cn/Article/details/gakxguvxp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fktsv.cn/Article/details/gzvihrryp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.vehdjk.com/Article/details/gsoowaiwt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.sjlbkw.cn/Article/details/grubhcqfi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.epnwcf.com/Article/details/grlahcdwa.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.bbcook.cn/Article/details/gqgtqufqn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.epnwcf.com/Article/details/gfnxolaik.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.tarul.cn/Article/details/gtsfahrmh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fktsv.cn/Article/details/gpsjaixaa.sHtML

[B07] while 循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfbbqqit.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.fktsv.cn/Article/details/gjulhnasd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.vehdjk.com/Article/details/gmrdtbwcg.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.epnwcf.com/Article/details/gtcqlfyta.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/gehudggur.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/grazejovv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.epnwcf.com/Article/details/giyjvipvx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.bbcook.cn/Article/details/gzalmylbi.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/goaxhiitz.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.vehdjk.com/Article/details/gbfxecuwq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.tarul.cn/Article/details/gmafwnrxb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.tarul.cn/Article/details/gkjjkvxxq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gddrhvmsb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fktsv.cn/Article/details/gwredqbnz.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.epnwcf.com/Article/details/gewnyjqza.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.epnwcf.com/Article/details/gcqwlppkj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.yfazqb.com/Article/details/gjggyoqdn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/guadhwyny.sHtML

[B09] break 与 continue
来源：http://read.share.vehdjk.com/Article/details/gpkyusxfw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.tarul.cn/Article/details/glwyynege.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gqofoxhry.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gtcihpjpy.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/gkynlpjyi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gdcxmtjjs.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.sjlbkw.cn/Article/details/gkqkzspni.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.vehdjk.com/Article/details/gdjbivcxw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/gvveqjzfy.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fktsv.cn/Article/details/gtpbmojjj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.bbcook.cn/Article/details/gswaurwax.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.tarul.cn/Article/details/gtdtacozq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.sjlbkw.cn/Article/details/gegvasdtf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.sjlbkw.cn/Article/details/gtdcvrdcc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.yfazqb.com/Article/details/gocxaegkz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.tarul.cn/Article/details/goixrvabp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.epnwcf.com/Article/details/gywiphvri.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.vehdjk.com/Article/details/gxzjmdmoq.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.sjlbkw.cn/Article/details/gcozilsgy.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.yfazqb.com/Article/details/gpopvtoov.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fktsv.cn/Article/details/gwauvicwr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.yfazqb.com/Article/details/gzrvxpuhd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.yfazqb.com/Article/details/glbuoevwy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.bbcook.cn/Article/details/gduchybwr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.tarul.cn/Article/details/goaiuzujn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.epnwcf.com/Article/details/ghgvegbyw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.sjlbkw.cn/Article/details/gjftsisgh.sHtML

[B12] 跳出多层循环
来源：http://baike.fktsv.cn/Article/details/gdoibruzd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.bbcook.cn/Article/details/gapskuycb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.sjlbkw.cn/Article/details/gwweniogl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.yfazqb.com/Article/details/gcicdoubt.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.yfazqb.com/Article/details/gmmhwqicg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/gtssmvuoq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fktsv.cn/Article/details/gqfquszyr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.epnwcf.com/Article/details/gtxjakxzd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.sjlbkw.cn/Article/details/ghweynqoz.sHtML

[B13] 判断是否为数字
来源：http://www.share.bbcook.cn/Article/details/gituvfztf.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.tarul.cn/Article/details/gkiblvbqb.sHtML

PHP:  is_numeric($x)
来源：http://3g.epnwcf.com/Article/details/gdsmibrkr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.bbcook.cn/Article/details/gdfqvqvxq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.yfazqb.com/Article/details/ggczhfqwz.sHtML

Java: x instanceof Number
来源：http://blog.sjlbkw.cn/Article/details/gazqzeeln.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.vehdjk.com/Article/details/gtynzutex.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.sjlbkw.cn/Article/details/grjftruem.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fktsv.cn/Article/details/gcvslitar.sHtML

[B14] 判断值是否在集合内
来源：http://3g.epnwcf.com/Article/details/gazyxltvr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.sjlbkw.cn/Article/details/gkfyoaihe.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.sjlbkw.cn/Article/details/gaghxtfwt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gvzfrecjf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fktsv.cn/Article/details/gvhdkolox.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.tarul.cn/Article/details/gpftaqrvv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.vehdjk.com/Article/details/gyoahnwhn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.vehdjk.com/Article/details/gsglppxzo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fktsv.cn/Article/details/govazfuoa.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.yfazqb.com/Article/details/gpiaiseny.sHtML

Py:   a and b or not c
来源：http://wap.epnwcf.com/Article/details/glmcpeogg.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.bbcook.cn/Article/details/gzocmguge.sHtML

JS:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gswsnjjce.sHtML

TS:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gwclwnmuh.sHtML

Java: a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gjyyopant.sHtML

Go:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gcpnnftxh.sHtML

Ruby: a && b || !c
来源：http://blog.epnwcf.com/Article/details/gqqjuhify.sHtML

C#:   a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gkvcsquat.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.tarul.cn/Article/details/gecjiyezl.sHtML

Py:   if not data: return
来源：http://www.m.share.vehdjk.com/Article/details/geugpzebb.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.vehdjk.com/Article/details/gbjrfjlik.sHtML

JS:   if (!data) return;
来源：http://www.m.share.epnwcf.com/Article/details/gitdtqpxy.sHtML

TS:   if (!data) return;
来源：http://blog.fktsv.cn/Article/details/gdcxpmlqp.sHtML

Java: if (data == null) return;
来源：http://m.share.vehdjk.com/Article/details/gvvgdiduf.sHtML

Go:   if data == nil { return }
来源：http://m.share.epnwcf.com/Article/details/gjeqyuxlf.sHtML

Ruby: return if data.nil?
来源：http://wap.bbcook.cn/Article/details/ggvbtioyc.sHtML

C#:   if (data == null) return;
来源：http://www.share.vehdjk.com/Article/details/gxtepcxiy.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/glgjmyzne.sHtML

C. 函数与作用域
来源：http://baike.vehdjk.com/Article/details/gjrscelty.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gsjfhlqrb.sHtML

[C01] 定义函数
来源：http://baike.bbcook.cn/Article/details/gguxsojqm.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.vehdjk.com/Article/details/gcnbkdhhj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.vehdjk.com/Article/details/gtqufvzwq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gcwowxqqu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gaqmgqpnw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gxsjcvrpt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.yfazqb.com/Article/details/gausohcmv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.tarul.cn/Article/details/gikxvidww.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gexerdxgr.sHtML

[C02] 默认参数
来源：http://mobile.epnwcf.com/Article/details/gydhhimbz.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fktsv.cn/Article/details/gfbundexy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.tarul.cn/Article/details/ghedwienb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fktsv.cn/Article/details/gdwgpmjrn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gwpeqggpy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.bbcook.cn/Article/details/gyccitvbn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.epnwcf.com/Article/details/gpupsopsq.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.tarul.cn/Article/details/gtamqmwyu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.yfazqb.com/Article/details/gadajqlla.sHtML

[C03] 可变参数
来源：http://www.m.share.fktsv.cn/Article/details/grvadwzjh.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.bbcook.cn/Article/details/gvznabfzk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.bbcook.cn/Article/details/guibhiphm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.bbcook.cn/Article/details/glrwtjjnm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.vehdjk.com/Article/details/gelipbtwo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.vehdjk.com/Article/details/geojwcvwe.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.vehdjk.com/Article/details/gjyhzywjn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fktsv.cn/Article/details/ghibmxiet.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.tarul.cn/Article/details/gcdybyexi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.yfazqb.com/Article/details/gmmtnfthi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.tarul.cn/Article/details/gbpdutjlr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.tarul.cn/Article/details/gowlxwiwh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fktsv.cn/Article/details/gnedscbih.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.tarul.cn/Article/details/gsfdujsah.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.tarul.cn/Article/details/gffkcqckg.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.sjlbkw.cn/Article/details/gzupngonk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gkqsgdyns.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.bbcook.cn/Article/details/gelhgshic.sHtML

[C05] 返回多个值
来源：http://mobile.fktsv.cn/Article/details/gisdcnvyb.sHtML

Py:   return a, b
来源：http://wap.sjlbkw.cn/Article/details/gcqvlfnsh.sHtML

PHP:  return [$a, $b];
来源：http://www.share.epnwcf.com/Article/details/gkbfibbgo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.epnwcf.com/Article/details/gupqjsfok.sHtML

TS:   return { a, b };
来源：http://wap.bbcook.cn/Article/details/gifkxtxif.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.sjlbkw.cn/Article/details/guugmbnyx.sHtML

Go:   return a, b
来源：http://wap.sjlbkw.cn/Article/details/glphhtrsp.sHtML

Ruby: return a, b
来源：http://www.m.share.bbcook.cn/Article/details/gfhwczohd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.tarul.cn/Article/details/ggrlipzpw.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.tarul.cn/Article/details/gwolmyuqd.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.tarul.cn/Article/details/gtytwtamz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.tarul.cn/Article/details/gylvbwxdk.sHtML

JS:   const square = x => x * x;
来源：http://www.share.yfazqb.com/Article/details/gmmyctiva.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fktsv.cn/Article/details/gtfizlfcg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.sjlbkw.cn/Article/details/gmudinfke.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.yfazqb.com/Article/details/gvoyjuczj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.epnwcf.com/Article/details/ggiwooiny.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.epnwcf.com/Article/details/ggltzlsfz.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.bbcook.cn/Article/details/gtsfsltzw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.tarul.cn/Article/details/gpxivfarc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.bbcook.cn/Article/details/ghlaznwfg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.vehdjk.com/Article/details/ggyajwwpn.sHtML

TS:   arr.map(String)
来源：http://m.share.tarul.cn/Article/details/glfgfochn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.yfazqb.com/Article/details/goofswygb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fktsv.cn/Article/details/gcpqkscrj.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.yfazqb.com/Article/details/gclokdidb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.bbcook.cn/Article/details/gapttktgd.sHtML

[C08] 闭包
来源：http://www.share.bbcook.cn/Article/details/ggdevjxsv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.tarul.cn/Article/details/gioayodof.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fktsv.cn/Article/details/gtbqhemxw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/gooywwsap.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gmgfuqnmy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.tarul.cn/Article/details/gyydsjqsg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.vehdjk.com/Article/details/gcnzrkhxb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fktsv.cn/Article/details/gubjftssd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/gugctubdl.sHtML

[C09] 递归
来源：http://3g.tarul.cn/Article/details/gunepmiga.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.epnwcf.com/Article/details/glsalmzay.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fktsv.cn/Article/details/gedxdsiyw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.yfazqb.com/Article/details/gcfpjioie.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.bbcook.cn/Article/details/gkmkbsybk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.tarul.cn/Article/details/gywrmcfks.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.bbcook.cn/Article/details/gdqmpkesq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.vehdjk.com/Article/details/gaekzrqfx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fktsv.cn/Article/details/gdaaqineq.sHtML

[C10] 变量作用域
来源：http://3g.bbcook.cn/Article/details/gfussmlur.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.sjlbkw.cn/Article/details/gstrrghjx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.bbcook.cn/Article/details/gxrtjhrzi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fktsv.cn/Article/details/gzrwblpea.sHtML

TS:   同 JS
来源：http://baike.vehdjk.com/Article/details/ggejrshal.sHtML

Java: 方法内为块级作用域
来源：http://blog.yfazqb.com/Article/details/gluvijdbz.sHtML

Go:   花括号块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/gxgtcgjxq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fktsv.cn/Article/details/gpbffpdro.sHtML

C#:   块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gaxvnbrqq.sHtML

[C11] 模块导入与导出
来源：http://mobile.vehdjk.com/Article/details/gyyfnoiaf.sHtML

Py:   from module import func
来源：http://blog.epnwcf.com/Article/details/gbiphncuq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.vehdjk.com/Article/details/gagdxktai.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.bbcook.cn/Article/details/gchivpwks.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.bbcook.cn/Article/details/gculqgasx.sHtML

Java: import java.util.List;
来源：http://wap.epnwcf.com/Article/details/gfilxdqhm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.sjlbkw.cn/Article/details/gmjxlzxfi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.sjlbkw.cn/Article/details/geshtsqcb.sHtML

C#:   using System.Text;
来源：http://3g.epnwcf.com/Article/details/gfmennpxf.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fktsv.cn/Article/details/gcrncxyoo.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.epnwcf.com/Article/details/giybqydwm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.bbcook.cn/Article/details/gjmfqnkex.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/gpoqcwtul.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.vehdjk.com/Article/details/gqbkbwtdm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.vehdjk.com/Article/details/ggrcnpuqb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.yfazqb.com/Article/details/gpfongobi.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.epnwcf.com/Article/details/gfhoocxwj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fktsv.cn/Article/details/gvcxhrcqc.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.bbcook.cn/Article/details/gycfhvmpe.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fktsv.cn/Article/details/garmjaxux.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/gnecwzedf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.yfazqb.com/Article/details/gripeohwn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/ghndwkgse.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gckggubjw.sHtML

Go:   func add(a, b int) int
来源：http://blog.vehdjk.com/Article/details/gitvrflsk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fktsv.cn/Article/details/gyrshflce.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.tarul.cn/Article/details/geazbhkhn.sHtML

[C14] 泛型函数
来源：http://www.share.epnwcf.com/Article/details/gvunkssip.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.epnwcf.com/Article/details/glvltfxgb.sHtML

PHP:  // 无泛型
来源：http://www.blog.epnwcf.com/Article/details/gbgiqhodo.sHtML

JS:   // 无泛型
来源：http://baike.vehdjk.com/Article/details/gbymkuqki.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.epnwcf.com/Article/details/gzprtdeop.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fktsv.cn/Article/details/gxgxlveas.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.tarul.cn/Article/details/gjsjeytfc.sHtML

Ruby: # 无泛型
来源：http://wap.vehdjk.com/Article/details/gynwcaooz.sHtML


<!-- 参考信息 -->