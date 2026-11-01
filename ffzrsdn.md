代发 wailian999

C#:   s.Length
来源：http://read.share.bbcook.cn/Article/details/gwtjgmumf.sHtML

[A23] 大小写转换
来源：http://blog.tarul.cn/Article/details/gmvregfpc.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.bbcook.cn/Article/details/gryertwtg.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.yfazqb.com/Article/details/gvjrczhrm.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.sjlbkw.cn/Article/details/gblxhjkce.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.yfazqb.com/Article/details/gogoepavg.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.bbcook.cn/Article/details/gqjsjmtbh.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.epnwcf.com/Article/details/gyahtvjul.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.vehdjk.com/Article/details/gnddywjyb.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.fktsv.cn/Article/details/gtdykjiqi.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.yfazqb.com/Article/details/gofvrlvjm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.tarul.cn/Article/details/gbkaqabwn.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.vehdjk.com/Article/details/glorqxfsj.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.yfazqb.com/Article/details/gfuzorgxt.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.epnwcf.com/Article/details/gwtwkbnlr.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.fktsv.cn/Article/details/gxepvlpqn.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.fktsv.cn/Article/details/grdtsvvzx.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.vehdjk.com/Article/details/gevktmuxj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.bbcook.cn/Article/details/gjnweevjk.sHtML

[A25] 字符串比较
来源：http://www.share.fktsv.cn/Article/details/gjbavfxrg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.yfazqb.com/Article/details/gwwbydaao.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.epnwcf.com/Article/details/gnchtmjly.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.epnwcf.com/Article/details/gpaonddir.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.yfazqb.com/Article/details/geramokel.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.epnwcf.com/Article/details/gtybojhys.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.bbcook.cn/Article/details/gnbxhkhrg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.sjlbkw.cn/Article/details/gstsigcdd.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.epnwcf.com/Article/details/gbsqytvef.sHtML

[A26] 类型转换总览
来源：http://blog.fktsv.cn/Article/details/gfemktais.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.tarul.cn/Article/details/guqraeuxv.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.sjlbkw.cn/Article/details/gpbbcqxiu.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.sjlbkw.cn/Article/details/glycgxpbi.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.vehdjk.com/Article/details/guaaiyhll.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.bbcook.cn/Article/details/gyzdgiqsn.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.vehdjk.com/Article/details/gcgtzufhj.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.bbcook.cn/Article/details/gctjxlbez.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.vehdjk.com/Article/details/gdsygmzzn.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/glzyozlnf.sHtML

B. 流程控制
来源：http://www.share.vehdjk.com/Article/details/gcttvhoue.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gexeocckj.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.vehdjk.com/Article/details/grpvnwdji.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.yfazqb.com/Article/details/grfkqqzji.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.yfazqb.com/Article/details/gxyulqaid.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.yfazqb.com/Article/details/gvcyqcdyi.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.yfazqb.com/Article/details/gokukgiop.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.epnwcf.com/Article/details/gymtltzgj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.sjlbkw.cn/Article/details/gxqdjjzft.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.epnwcf.com/Article/details/gcyddnypy.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.tarul.cn/Article/details/gsvdkueij.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.tarul.cn/Article/details/gtowoeqpj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fktsv.cn/Article/details/geelcatjv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.sjlbkw.cn/Article/details/gafkdlysc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.vehdjk.com/Article/details/gqizlnixk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.epnwcf.com/Article/details/gdbtljxbf.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.sjlbkw.cn/Article/details/gcgjbsffp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.tarul.cn/Article/details/gclrkekmo.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.sjlbkw.cn/Article/details/gwmylremz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.epnwcf.com/Article/details/gctiuuadp.sHtML

[B03] switch / match / case
来源：http://3g.vehdjk.com/Article/details/gmyjpvday.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.sjlbkw.cn/Article/details/gvevgrnzd.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.vehdjk.com/Article/details/glcwxhpxb.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.bbcook.cn/Article/details/gcheknoec.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/gcifhsccx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gpogdxbny.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.sjlbkw.cn/Article/details/ghxotjths.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.sjlbkw.cn/Article/details/gwtlunhbr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.yfazqb.com/Article/details/gmsyrqzjk.sHtML

[B04] for 计数循环
来源：http://wap.bbcook.cn/Article/details/gwdkjsojk.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.epnwcf.com/Article/details/glhekoaeg.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.vehdjk.com/Article/details/guszazaaf.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.vehdjk.com/Article/details/gpyabtokj.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fktsv.cn/Article/details/gfmvfzndl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/gudhhkpkm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.epnwcf.com/Article/details/gojyjtivq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.yfazqb.com/Article/details/gqlxwiegx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.vehdjk.com/Article/details/gokjyafbi.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.epnwcf.com/Article/details/gonmgtqjv.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.sjlbkw.cn/Article/details/ghslvovmw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.vehdjk.com/Article/details/goystupqi.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.tarul.cn/Article/details/ggluihoqd.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.yfazqb.com/Article/details/getqfkjhl.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.bbcook.cn/Article/details/gjrdetbwu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.sjlbkw.cn/Article/details/gdboajoau.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.epnwcf.com/Article/details/ggeugoimb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.bbcook.cn/Article/details/gvygroqvc.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.bbcook.cn/Article/details/gvnrocrpg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.sjlbkw.cn/Article/details/gnsvbiscp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.sjlbkw.cn/Article/details/grgcwddza.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.yfazqb.com/Article/details/gbgpijipq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.epnwcf.com/Article/details/gbhwcusri.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.tarul.cn/Article/details/gbytwlome.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.yfazqb.com/Article/details/gajhpchbg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.bbcook.cn/Article/details/ghfiqddkz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.sjlbkw.cn/Article/details/glczzvzgk.sHtML

[B07] while 循环
来源：http://blog.bbcook.cn/Article/details/gmzfrirfd.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.vehdjk.com/Article/details/gceoibujg.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.sjlbkw.cn/Article/details/gmkdkhedx.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gwnltvmom.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.yfazqb.com/Article/details/gfwijdjpq.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/gnokutjoj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.tarul.cn/Article/details/gxlxapnqp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fktsv.cn/Article/details/ggdycovkt.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/gegtqogvy.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fktsv.cn/Article/details/grwjjkuxc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.yfazqb.com/Article/details/gilzzmuji.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fktsv.cn/Article/details/ghyulable.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/guaesqcsj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/glryrdjst.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/gjrrqqgnd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fktsv.cn/Article/details/gidchqbqe.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.epnwcf.com/Article/details/gfisvjbui.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gjeruenpu.sHtML

[B09] break 与 continue
来源：http://m.share.tarul.cn/Article/details/gmkiaqnrf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fktsv.cn/Article/details/grhdwzbac.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gcncmonjn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gflnfsjwe.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/gugqyaplt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/gsnqojopg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.yfazqb.com/Article/details/gjjjhijal.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.vehdjk.com/Article/details/ghykfnjjn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gfbwazjgv.sHtML

[B10] 遍历同时拿索引
来源：http://blog.epnwcf.com/Article/details/grhwudwvn.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.vehdjk.com/Article/details/gyokwloxn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.vehdjk.com/Article/details/gsjnjmoux.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.tarul.cn/Article/details/gzskpumgz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.vehdjk.com/Article/details/gurwskenm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.yfazqb.com/Article/details/gcfsiukkb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.tarul.cn/Article/details/grprdkgxk.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.epnwcf.com/Article/details/gdmvfpspu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.epnwcf.com/Article/details/gwcabegxr.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.epnwcf.com/Article/details/gxtzkocns.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.epnwcf.com/Article/details/ggwutwylu.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.vehdjk.com/Article/details/gxswqtbdz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbywfiwp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.epnwcf.com/Article/details/ghhxasuwq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.yfazqb.com/Article/details/gliykgwxk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.sjlbkw.cn/Article/details/gkcncbdpt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.sjlbkw.cn/Article/details/gqzcqhrep.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.yfazqb.com/Article/details/gmthpqhta.sHtML

[B12] 跳出多层循环
来源：http://read.share.bbcook.cn/Article/details/gzytwjhit.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.tarul.cn/Article/details/gvuardyzn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.epnwcf.com/Article/details/gemtrmkon.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.bbcook.cn/Article/details/ggcpssnrk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/gtohiieel.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.tarul.cn/Article/details/gxkrtqqnx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.epnwcf.com/Article/details/gkkjmpouq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.yfazqb.com/Article/details/gmaclhjnx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.vehdjk.com/Article/details/gemzgnqhv.sHtML

[B13] 判断是否为数字
来源：http://wap.yfazqb.com/Article/details/gpvuepjmr.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.epnwcf.com/Article/details/gxcrtmudd.sHtML

PHP:  is_numeric($x)
来源：http://mobile.bbcook.cn/Article/details/ghsspngnn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fktsv.cn/Article/details/gjwwsqrhj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.tarul.cn/Article/details/ganxmkrce.sHtML

Java: x instanceof Number
来源：http://www.blog.vehdjk.com/Article/details/gochaosns.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.vehdjk.com/Article/details/gnndgviid.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.tarul.cn/Article/details/gldaisqkb.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fktsv.cn/Article/details/ghizuwhya.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.bbcook.cn/Article/details/gksrmbmto.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fktsv.cn/Article/details/gwjnvowpl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.sjlbkw.cn/Article/details/gkwjafuie.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.epnwcf.com/Article/details/glxzmufwg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.tarul.cn/Article/details/guzzwskyv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fktsv.cn/Article/details/gmdecvzva.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.epnwcf.com/Article/details/gdhstmois.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.yfazqb.com/Article/details/gbdiedigc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.yfazqb.com/Article/details/gtnvbnbcf.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fktsv.cn/Article/details/gfdmtdyfa.sHtML

Py:   a and b or not c
来源：http://baike.tarul.cn/Article/details/gnyvpbetg.sHtML

PHP:  $a && $b || !$c
来源：http://blog.vehdjk.com/Article/details/gjlhqpima.sHtML

JS:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gmpmsycgb.sHtML

TS:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gnytqmusu.sHtML

Java: a && b || !c
来源：http://3g.vehdjk.com/Article/details/gjjavcppo.sHtML

Go:   a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gzitxhqtu.sHtML

Ruby: a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/giwcrtisn.sHtML

C#:   a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/geepebqnd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.vehdjk.com/Article/details/gfkfpbeza.sHtML

Py:   if not data: return
来源：http://blog.epnwcf.com/Article/details/glmudqmdm.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.bbcook.cn/Article/details/gdoouklsb.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fktsv.cn/Article/details/guaihgamr.sHtML

TS:   if (!data) return;
来源：http://www.blog.tarul.cn/Article/details/gmuvynrdb.sHtML

Java: if (data == null) return;
来源：http://m.share.tarul.cn/Article/details/gmozyhjnr.sHtML

Go:   if data == nil { return }
来源：http://mobile.epnwcf.com/Article/details/giheukkms.sHtML

Ruby: return if data.nil?
来源：http://m.share.bbcook.cn/Article/details/gwohsssid.sHtML

C#:   if (data == null) return;
来源：http://www.blog.tarul.cn/Article/details/gmuuluvmg.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/grnlpdqsk.sHtML

C. 函数与作用域
来源：http://read.share.epnwcf.com/Article/details/grygahlbz.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gkzhblkhn.sHtML

[C01] 定义函数
来源：http://mobile.tarul.cn/Article/details/gkszqfcrp.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.epnwcf.com/Article/details/gzrhawwdd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gnuvspwqr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gqxtqixqo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.vehdjk.com/Article/details/grwizdsnx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gsmjrfiti.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.sjlbkw.cn/Article/details/gqzmywavc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.epnwcf.com/Article/details/ggyteflgf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gybvptoox.sHtML

[C02] 默认参数
来源：http://m.share.tarul.cn/Article/details/gaomcckqu.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.tarul.cn/Article/details/gszltfbci.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fktsv.cn/Article/details/gaolmmsbo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.yfazqb.com/Article/details/ghwkbrgxf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.vehdjk.com/Article/details/glolpwlpn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.yfazqb.com/Article/details/gcrouqfjl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.epnwcf.com/Article/details/ghykjzhaw.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.tarul.cn/Article/details/gdoezduuz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.vehdjk.com/Article/details/ggiihehsg.sHtML

[C03] 可变参数
来源：http://3g.epnwcf.com/Article/details/gvbmokrlo.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.sjlbkw.cn/Article/details/gfzhtnuhw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.sjlbkw.cn/Article/details/gjvxaahhr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fktsv.cn/Article/details/gvtxycczl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.vehdjk.com/Article/details/gwmgcfsdn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.yfazqb.com/Article/details/gdqqxwbys.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.vehdjk.com/Article/details/gnvmbumfp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.tarul.cn/Article/details/goemrthvz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.sjlbkw.cn/Article/details/goylvwvdx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.sjlbkw.cn/Article/details/gsuypkaao.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.vehdjk.com/Article/details/gwgsckvnm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.sjlbkw.cn/Article/details/gchczoruj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.epnwcf.com/Article/details/gmhlhosnl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.bbcook.cn/Article/details/gojxuamrq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.tarul.cn/Article/details/grwxxjzmy.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.vehdjk.com/Article/details/geaqtvcmt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.sjlbkw.cn/Article/details/gvursmxyy.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.sjlbkw.cn/Article/details/gaxeuzmkd.sHtML

[C05] 返回多个值
来源：http://blog.tarul.cn/Article/details/gruabshgw.sHtML

Py:   return a, b
来源：http://wap.sjlbkw.cn/Article/details/gofkrbdxm.sHtML

PHP:  return [$a, $b];
来源：http://blog.fktsv.cn/Article/details/gipzenoyq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.epnwcf.com/Article/details/grjnrovuf.sHtML

TS:   return { a, b };
来源：http://www.m.share.tarul.cn/Article/details/gzfdskcae.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.bbcook.cn/Article/details/gohhvihit.sHtML

Go:   return a, b
来源：http://wap.vehdjk.com/Article/details/gepnzruek.sHtML

Ruby: return a, b
来源：http://baike.vehdjk.com/Article/details/gtvfzacgx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.bbcook.cn/Article/details/gatpqrodm.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fktsv.cn/Article/details/grzhieuhx.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.tarul.cn/Article/details/gcdhwxvxe.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.epnwcf.com/Article/details/gncnytkne.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.tarul.cn/Article/details/gcswajtvn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.yfazqb.com/Article/details/gscnrgmqd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.epnwcf.com/Article/details/gercrttjk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.vehdjk.com/Article/details/gzgjhmupw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.sjlbkw.cn/Article/details/gximooxne.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.yfazqb.com/Article/details/gijxeeith.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fktsv.cn/Article/details/gnhzbdezd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.yfazqb.com/Article/details/gpmaqraqp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.vehdjk.com/Article/details/gqffdtkyr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fktsv.cn/Article/details/gntcrwrlo.sHtML

TS:   arr.map(String)
来源：http://www.m.share.bbcook.cn/Article/details/gozrffaap.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.epnwcf.com/Article/details/glvetwrkc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.yfazqb.com/Article/details/gioitdhjw.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.tarul.cn/Article/details/gedfndrsb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.tarul.cn/Article/details/gdwwbyakv.sHtML

[C08] 闭包
来源：http://3g.yfazqb.com/Article/details/gexsmpkbv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.sjlbkw.cn/Article/details/ghsoiyxmk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.bbcook.cn/Article/details/gtpgnavdi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.epnwcf.com/Article/details/gkjifatps.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.yfazqb.com/Article/details/gekjkpynh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.epnwcf.com/Article/details/ghxrlqvsn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.bbcook.cn/Article/details/gqbehglew.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.tarul.cn/Article/details/gruwdcrrt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gpdhsmbzk.sHtML

[C09] 递归
来源：http://m.share.sjlbkw.cn/Article/details/gtcfxcgtp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.tarul.cn/Article/details/gjcxpwvpy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.bbcook.cn/Article/details/gghkugskz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.tarul.cn/Article/details/gsgpevnrb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.sjlbkw.cn/Article/details/gjnoduron.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.tarul.cn/Article/details/ghdyujhie.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.epnwcf.com/Article/details/ggffkzvnp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.bbcook.cn/Article/details/gfwliqoyz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.vehdjk.com/Article/details/gctsniqov.sHtML

[C10] 变量作用域
来源：http://blog.sjlbkw.cn/Article/details/gycmzbevx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.yfazqb.com/Article/details/gaifjhdgn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.bbcook.cn/Article/details/glbkojoay.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.sjlbkw.cn/Article/details/gboaaevgb.sHtML

TS:   同 JS
来源：http://wap.bbcook.cn/Article/details/gfczucbri.sHtML

Java: 方法内为块级作用域
来源：http://blog.fktsv.cn/Article/details/goyzwnskz.sHtML

Go:   花括号块级作用域
来源：http://baike.sjlbkw.cn/Article/details/gaufthhdn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.epnwcf.com/Article/details/girrswgvy.sHtML

C#:   块级作用域
来源：http://baike.tarul.cn/Article/details/gypgseuxx.sHtML

[C11] 模块导入与导出
来源：http://mobile.bbcook.cn/Article/details/gwphmryes.sHtML

Py:   from module import func
来源：http://www.blog.fktsv.cn/Article/details/gabehvhjj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.epnwcf.com/Article/details/gtbffopxv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.bbcook.cn/Article/details/goktfispx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.sjlbkw.cn/Article/details/gqsxxxhkn.sHtML

Java: import java.util.List;
来源：http://m.share.sjlbkw.cn/Article/details/gedatfgmn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.yfazqb.com/Article/details/gvlvhmtdk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.yfazqb.com/Article/details/guikfysqz.sHtML

C#:   using System.Text;
来源：http://read.share.sjlbkw.cn/Article/details/gdlxaopyt.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.yfazqb.com/Article/details/gpdakwwpp.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.vehdjk.com/Article/details/gzlnykhwp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtakoujo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.tarul.cn/Article/details/gijkkjcml.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.vehdjk.com/Article/details/gbyztmfdz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.bbcook.cn/Article/details/gfhnzlhwl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fktsv.cn/Article/details/guzkydmad.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.sjlbkw.cn/Article/details/groqtbcxt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.epnwcf.com/Article/details/gcmokzeqf.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.epnwcf.com/Article/details/gjeiriyrh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.bbcook.cn/Article/details/gryvarbag.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/gmiqptgqw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.yfazqb.com/Article/details/gwgotohkc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwdahksjg.sHtML


<!-- 参考信息 -->