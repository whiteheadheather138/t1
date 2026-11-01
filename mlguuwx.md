代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://read.share.tarul.cn/Article/details/grmgxumon.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.yfazqb.com/Article/details/ghquqzbnk.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.fktsv.cn/Article/details/gnyginoca.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.tarul.cn/Article/details/gugxvocwb.sHtML

[A22] 获取字符串长度
来源：http://3g.bbcook.cn/Article/details/guqpkwzag.sHtML

Py:   len(s)
来源：http://baike.fktsv.cn/Article/details/gskiyxhwb.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.sjlbkw.cn/Article/details/goiggbvfw.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.bbcook.cn/Article/details/gqbblaihv.sHtML

TS:   s.length
来源：http://blog.bbcook.cn/Article/details/grixoqede.sHtML

Java: s.length()
来源：http://read.share.tarul.cn/Article/details/gexjmkakg.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.tarul.cn/Article/details/giqthjdfa.sHtML

Ruby: s.length
来源：http://read.share.bbcook.cn/Article/details/gtrlaoebq.sHtML

C#:   s.Length
来源：http://m.share.sjlbkw.cn/Article/details/gflwuhgjp.sHtML

[A23] 大小写转换
来源：http://blog.yfazqb.com/Article/details/gdcjqegck.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.vehdjk.com/Article/details/gqsgzvvkd.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.tarul.cn/Article/details/guadetljt.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fktsv.cn/Article/details/gmygiuhdd.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.vehdjk.com/Article/details/gqnzrdcea.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.yfazqb.com/Article/details/gikktdhjd.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.sjlbkw.cn/Article/details/gcrxcjgqb.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.bbcook.cn/Article/details/gbmvgigno.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.yfazqb.com/Article/details/gyvjrzvye.sHtML

[A24] 去除首尾空白
来源：http://read.share.bbcook.cn/Article/details/gtvtnvwgy.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.tarul.cn/Article/details/gfpdfzbtt.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.sjlbkw.cn/Article/details/gzrwobpis.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fktsv.cn/Article/details/gnozwowil.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.yfazqb.com/Article/details/gfkxwtlwi.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.vehdjk.com/Article/details/gxyrxtmjy.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.epnwcf.com/Article/details/gbwewsdxb.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.fktsv.cn/Article/details/gfimdtpmt.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.tarul.cn/Article/details/ggiksarex.sHtML

[A25] 字符串比较
来源：http://m.share.tarul.cn/Article/details/gwcknrpyo.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.yfazqb.com/Article/details/gitcarzve.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.yfazqb.com/Article/details/gmzciagvl.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.yfazqb.com/Article/details/gunecnwbj.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.tarul.cn/Article/details/godbyrljh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.yfazqb.com/Article/details/gwzetbvto.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.fktsv.cn/Article/details/gbhwljxvk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.vehdjk.com/Article/details/gxkntgqlz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.bbcook.cn/Article/details/grkrsjpiw.sHtML

[A26] 类型转换总览
来源：http://www.m.share.vehdjk.com/Article/details/gefhrtwls.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.fktsv.cn/Article/details/guofyfhus.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.vehdjk.com/Article/details/gqoxmlgzx.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.tarul.cn/Article/details/gegnqvfod.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.bbcook.cn/Article/details/gnmbqjsau.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.tarul.cn/Article/details/geuwzbahl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.bbcook.cn/Article/details/glmxhyagm.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.tarul.cn/Article/details/gcdunresv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.epnwcf.com/Article/details/gbxgpiqki.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gnszuedpa.sHtML

B. 流程控制
来源：http://wap.bbcook.cn/Article/details/grvjrnnvn.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/glkprrmqf.sHtML

[B01] 条件判断 if / else
来源：http://mobile.tarul.cn/Article/details/giacfilom.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.sjlbkw.cn/Article/details/gzhxotimi.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.bbcook.cn/Article/details/gjoaumlku.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.bbcook.cn/Article/details/gffpcndza.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/gkeykmlsg.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/gykxirdgl.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.bbcook.cn/Article/details/glksflfxk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.epnwcf.com/Article/details/gkocgxifv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.tarul.cn/Article/details/gnedgznmf.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.tarul.cn/Article/details/gausygkbg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.tarul.cn/Article/details/gxojwxugr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.epnwcf.com/Article/details/gmgknngqa.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.bbcook.cn/Article/details/gezwwhsaf.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.yfazqb.com/Article/details/gcredsoqp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/gkmkklehl.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.yfazqb.com/Article/details/gkkdsijta.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.sjlbkw.cn/Article/details/grijryxmr.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.vehdjk.com/Article/details/gotvseouo.sHtML

[B03] switch / match / case
来源：http://read.share.yfazqb.com/Article/details/gmzkebioj.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.tarul.cn/Article/details/ggtskriel.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.tarul.cn/Article/details/glfcqhjuz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/gveourcmf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.epnwcf.com/Article/details/gphjoeklc.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.sjlbkw.cn/Article/details/gbhxwctvr.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.tarul.cn/Article/details/garaorbxx.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.tarul.cn/Article/details/gywmwqfbd.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.epnwcf.com/Article/details/gofiohwzv.sHtML

[B04] for 计数循环
来源：http://www.blog.tarul.cn/Article/details/guclzxksn.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.yfazqb.com/Article/details/gbqevixkt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.bbcook.cn/Article/details/gqdpdwedr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.sjlbkw.cn/Article/details/gklacqdbw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.yfazqb.com/Article/details/giedloqvo.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.tarul.cn/Article/details/gtveodego.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.fktsv.cn/Article/details/gyynwmqye.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.yfazqb.com/Article/details/gpashnyto.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.bbcook.cn/Article/details/gwpgelyqq.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.sjlbkw.cn/Article/details/gtfwtmgbz.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.vehdjk.com/Article/details/gfynfznrd.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.epnwcf.com/Article/details/ghiqktxdy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.epnwcf.com/Article/details/gnozowkyv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.tarul.cn/Article/details/gxqqnpobs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.bbcook.cn/Article/details/gmuhemzwz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.vehdjk.com/Article/details/gdaikhlfk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.epnwcf.com/Article/details/gzxsnnwsy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.bbcook.cn/Article/details/gewmhsqyl.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.tarul.cn/Article/details/gjvizpiql.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fktsv.cn/Article/details/gvbsyqugn.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.epnwcf.com/Article/details/gfxqsmqej.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.vehdjk.com/Article/details/gpbakblhh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fktsv.cn/Article/details/gbroxuoxx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.vehdjk.com/Article/details/gdckwnytu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.fktsv.cn/Article/details/gddzllokc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.sjlbkw.cn/Article/details/gwavsrjaw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fktsv.cn/Article/details/gqqrnkrpg.sHtML

[B07] while 循环
来源：http://www.m.share.vehdjk.com/Article/details/gpahoqpvw.sHtML

Py:   while i < 10: i += 1
来源：http://blog.vehdjk.com/Article/details/gylyncykt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fktsv.cn/Article/details/gkqnfvjym.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.tarul.cn/Article/details/gfayakowh.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.vehdjk.com/Article/details/gxkdrxwtm.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.bbcook.cn/Article/details/ghhsdixtp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.tarul.cn/Article/details/gqlxtyzkz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.epnwcf.com/Article/details/gqaqdlnqi.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/gdzeammvj.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.tarul.cn/Article/details/guxfvxzrc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.epnwcf.com/Article/details/giuaygimy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fktsv.cn/Article/details/gqoxwycsz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/gqipgozgc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gvdbihius.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gdplcjnoa.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.vehdjk.com/Article/details/gextrquko.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.vehdjk.com/Article/details/gxsgfilbk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/guokumfly.sHtML

[B09] break 与 continue
来源：http://read.share.epnwcf.com/Article/details/gwrrcpoqs.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fktsv.cn/Article/details/gwkpzveso.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/gdmosshzx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gksxiugvo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/gdhmblhhy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/grblmsrye.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fktsv.cn/Article/details/ghedjkdje.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.epnwcf.com/Article/details/gxvpnouxy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/ggfobyjej.sHtML

[B10] 遍历同时拿索引
来源：http://3g.epnwcf.com/Article/details/gdrqmtrsz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.epnwcf.com/Article/details/gwihpofhw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fktsv.cn/Article/details/gmqpaolst.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.sjlbkw.cn/Article/details/gcbouogjd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.vehdjk.com/Article/details/grbvvaykm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.vehdjk.com/Article/details/gyygqcpic.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.tarul.cn/Article/details/gpumhwgdx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.tarul.cn/Article/details/ggindlhpn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fktsv.cn/Article/details/gpsubzrwr.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.bbcook.cn/Article/details/gquvojcdh.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.bbcook.cn/Article/details/grjtnqiaz.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.bbcook.cn/Article/details/gfqdpibfj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.vehdjk.com/Article/details/gqxgpmhjw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fktsv.cn/Article/details/guddbumrt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.tarul.cn/Article/details/golsueucv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.sjlbkw.cn/Article/details/gdujormmq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.tarul.cn/Article/details/gffzmxlxr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.tarul.cn/Article/details/glibfqvyy.sHtML

[B12] 跳出多层循环
来源：http://www.share.epnwcf.com/Article/details/gzcagjsgn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.tarul.cn/Article/details/guvubfdff.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.bbcook.cn/Article/details/gekrcxoeg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.yfazqb.com/Article/details/geyqwimcm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.yfazqb.com/Article/details/gxtpsacgy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.yfazqb.com/Article/details/gyjjfitff.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.yfazqb.com/Article/details/gctjeomes.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.sjlbkw.cn/Article/details/glwjbawge.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fktsv.cn/Article/details/gwupuxqwx.sHtML

[B13] 判断是否为数字
来源：http://read.share.fktsv.cn/Article/details/gcglnvonf.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fktsv.cn/Article/details/gvzmwpkfl.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.yfazqb.com/Article/details/guemvhcph.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fktsv.cn/Article/details/gkdvxwmrp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.vehdjk.com/Article/details/ggckqcolm.sHtML

Java: x instanceof Number
来源：http://3g.fktsv.cn/Article/details/gcoothvpb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.tarul.cn/Article/details/gwqnepyqh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.vehdjk.com/Article/details/gbjdiihaq.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.yfazqb.com/Article/details/gbptbzecu.sHtML

[B14] 判断值是否在集合内
来源：http://3g.vehdjk.com/Article/details/gkjuyrdya.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fktsv.cn/Article/details/gmrnfsota.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.sjlbkw.cn/Article/details/ghmqstmer.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.yfazqb.com/Article/details/giapkobie.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.sjlbkw.cn/Article/details/gxjuepfza.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gazrdpows.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.yfazqb.com/Article/details/gwbzeodwj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.vehdjk.com/Article/details/guhhptlhf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.yfazqb.com/Article/details/gtwaejmfd.sHtML

[B15] 布尔运算与取反
来源：http://baike.fktsv.cn/Article/details/gsriezxxd.sHtML

Py:   a and b or not c
来源：http://3g.tarul.cn/Article/details/gkjefmsze.sHtML

PHP:  $a && $b || !$c
来源：http://blog.sjlbkw.cn/Article/details/gwvdmncff.sHtML

JS:   a && b || !c
来源：http://baike.epnwcf.com/Article/details/ghkefvvdb.sHtML

TS:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/gfredtqij.sHtML

Java: a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gqmkxdskt.sHtML

Go:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gfdgyezxx.sHtML

Ruby: a && b || !c
来源：http://wap.tarul.cn/Article/details/gzoffezwd.sHtML

C#:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gswzuvdye.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.yfazqb.com/Article/details/gbwonrybi.sHtML

Py:   if not data: return
来源：http://www.blog.yfazqb.com/Article/details/ginavwsew.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fktsv.cn/Article/details/gepisswzn.sHtML

JS:   if (!data) return;
来源：http://m.share.epnwcf.com/Article/details/gmervwjuv.sHtML

TS:   if (!data) return;
来源：http://m.share.sjlbkw.cn/Article/details/gxnjsunhp.sHtML

Java: if (data == null) return;
来源：http://blog.vehdjk.com/Article/details/gcnixttds.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxywwxdg.sHtML

Ruby: return if data.nil?
来源：http://baike.sjlbkw.cn/Article/details/gjvfijnsv.sHtML

C#:   if (data == null) return;
来源：http://baike.epnwcf.com/Article/details/gcptupjsz.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gwmurkfug.sHtML

C. 函数与作用域
来源：http://www.blog.epnwcf.com/Article/details/gysozwwmw.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/griltgxwn.sHtML

[C01] 定义函数
来源：http://wap.yfazqb.com/Article/details/gezdfgvcz.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.epnwcf.com/Article/details/gpwzdapjz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gumcufays.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gokygtbht.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.tarul.cn/Article/details/gbkynujio.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gvksfjryi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.tarul.cn/Article/details/gtvomreyi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.yfazqb.com/Article/details/gecrsbmab.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gwxjejycw.sHtML

[C02] 默认参数
来源：http://www.blog.epnwcf.com/Article/details/gdyqiihzq.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.tarul.cn/Article/details/gikvrbhuh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.yfazqb.com/Article/details/gzwhdeons.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gokkrsdzk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.bbcook.cn/Article/details/gnvfbggdh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.tarul.cn/Article/details/gpvnahvzm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.tarul.cn/Article/details/gmmeqjcsh.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.bbcook.cn/Article/details/geugezwqt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.epnwcf.com/Article/details/galhlaazo.sHtML

[C03] 可变参数
来源：http://read.share.bbcook.cn/Article/details/gfiwtnuko.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fktsv.cn/Article/details/grchdjigr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.sjlbkw.cn/Article/details/galspbjmz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fktsv.cn/Article/details/gibfrvexv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.tarul.cn/Article/details/gcdkacssp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fktsv.cn/Article/details/gczmlbauk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.epnwcf.com/Article/details/gildojhav.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.bbcook.cn/Article/details/gzgidvdln.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.sjlbkw.cn/Article/details/gattgrfun.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.epnwcf.com/Article/details/gmwbggeyz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.yfazqb.com/Article/details/gpthogblt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.tarul.cn/Article/details/gbqezmtnk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.bbcook.cn/Article/details/gplgogjbi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.bbcook.cn/Article/details/gwocztfhh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.vehdjk.com/Article/details/goimjtdss.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.sjlbkw.cn/Article/details/getucrdvo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.vehdjk.com/Article/details/gifbnkwud.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.bbcook.cn/Article/details/gxhbgnirp.sHtML

[C05] 返回多个值
来源：http://blog.sjlbkw.cn/Article/details/gmvzermih.sHtML

Py:   return a, b
来源：http://www.share.sjlbkw.cn/Article/details/gkluirqou.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.yfazqb.com/Article/details/gunrmkycq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.tarul.cn/Article/details/gzwrnvvab.sHtML

TS:   return { a, b };
来源：http://m.share.vehdjk.com/Article/details/gbedxozzy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.vehdjk.com/Article/details/gcuaiafbw.sHtML

Go:   return a, b
来源：http://m.share.sjlbkw.cn/Article/details/gtbmckczk.sHtML

Ruby: return a, b
来源：http://m.share.fktsv.cn/Article/details/gpsuxqhug.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.sjlbkw.cn/Article/details/gcqrenosx.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.bbcook.cn/Article/details/gwzdtkdkn.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.vehdjk.com/Article/details/ggfhuiyao.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.vehdjk.com/Article/details/gqdahidik.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.yfazqb.com/Article/details/gfdhtvjtt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.tarul.cn/Article/details/gsuuicsgr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.epnwcf.com/Article/details/gkbhrzmuw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.yfazqb.com/Article/details/gijiwogsd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.yfazqb.com/Article/details/gipuhmvfr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.yfazqb.com/Article/details/gntwicwso.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.sjlbkw.cn/Article/details/gvaaueqfe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.vehdjk.com/Article/details/gqopvabku.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.tarul.cn/Article/details/gmtrphukd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.epnwcf.com/Article/details/gfaldjsjc.sHtML

TS:   arr.map(String)
来源：http://3g.yfazqb.com/Article/details/gtzosuhjf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.vehdjk.com/Article/details/gqagsfsrw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.epnwcf.com/Article/details/gthsfeicm.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.sjlbkw.cn/Article/details/gftgwcfgn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fktsv.cn/Article/details/gdvchspqw.sHtML

[C08] 闭包
来源：http://blog.sjlbkw.cn/Article/details/gljffjvao.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.epnwcf.com/Article/details/garpviant.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fktsv.cn/Article/details/gxxlyvarl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.epnwcf.com/Article/details/ghykghgzm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/gprsiomgv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fktsv.cn/Article/details/gfxqbimnk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.yfazqb.com/Article/details/gcxcbagkd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.bbcook.cn/Article/details/gmehvifdb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.vehdjk.com/Article/details/gsvegtrfp.sHtML

[C09] 递归
来源：http://www.blog.bbcook.cn/Article/details/gpwmaasov.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.yfazqb.com/Article/details/gwdvypbym.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkvydtgy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fktsv.cn/Article/details/gsnqztcdu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.yfazqb.com/Article/details/gjccowtua.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.epnwcf.com/Article/details/geqxkmifp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.yfazqb.com/Article/details/gfczwzatf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.epnwcf.com/Article/details/gcsuohggy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.bbcook.cn/Article/details/gosoalnzm.sHtML

[C10] 变量作用域
来源：http://www.share.epnwcf.com/Article/details/gpvdbblop.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.yfazqb.com/Article/details/gaadiytlv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fktsv.cn/Article/details/gipmboewp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.bbcook.cn/Article/details/gsnxcwjeh.sHtML

TS:   同 JS
来源：http://baike.epnwcf.com/Article/details/gykggvzvf.sHtML

Java: 方法内为块级作用域
来源：http://baike.tarul.cn/Article/details/gonxktfmr.sHtML

Go:   花括号块级作用域
来源：http://m.share.sjlbkw.cn/Article/details/guonehtfl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.epnwcf.com/Article/details/glgfmhruy.sHtML

C#:   块级作用域
来源：http://3g.vehdjk.com/Article/details/gdbmjegxu.sHtML

[C11] 模块导入与导出
来源：http://wap.vehdjk.com/Article/details/gkbbyzolo.sHtML

Py:   from module import func
来源：http://www.share.vehdjk.com/Article/details/gnufkjyey.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fktsv.cn/Article/details/ghfbtqfls.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.tarul.cn/Article/details/ghemxjfss.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.tarul.cn/Article/details/gxeqjhmgt.sHtML

Java: import java.util.List;
来源：http://mobile.sjlbkw.cn/Article/details/gymhejuic.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.bbcook.cn/Article/details/gqabvadrd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.tarul.cn/Article/details/gbexhnnvc.sHtML

C#:   using System.Text;
来源：http://blog.vehdjk.com/Article/details/glccmmzyw.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.tarul.cn/Article/details/guqkqwoqp.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.tarul.cn/Article/details/gtbtlszgt.sHtML


<!-- 参考信息 -->