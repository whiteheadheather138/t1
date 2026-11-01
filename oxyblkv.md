代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.bbcook.cn/Article/details/gytqezavq.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.yfazqb.com/Article/details/geizxjlub.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.bbcook.cn/Article/details/gxhleetme.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.vehdjk.com/Article/details/gmqprbiep.sHtML

[A22] 获取字符串长度
来源：http://m.share.epnwcf.com/Article/details/gduunhozd.sHtML

Py:   len(s)
来源：http://www.blog.fktsv.cn/Article/details/gccdlpmep.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.tarul.cn/Article/details/gsdgqubjf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.epnwcf.com/Article/details/gkklhvgbr.sHtML

TS:   s.length
来源：http://www.share.fktsv.cn/Article/details/gouexcnpw.sHtML

Java: s.length()
来源：http://mobile.tarul.cn/Article/details/gadhvpiyw.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/ghhmjdyqn.sHtML

Ruby: s.length
来源：http://m.share.fktsv.cn/Article/details/gsczutzgd.sHtML

C#:   s.Length
来源：http://baike.yfazqb.com/Article/details/ghzutszyy.sHtML

[A23] 大小写转换
来源：http://mobile.fktsv.cn/Article/details/gvanmbxxi.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.epnwcf.com/Article/details/gqahjjxib.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.sjlbkw.cn/Article/details/gijqosqny.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.yfazqb.com/Article/details/gdnmyrxqd.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.yfazqb.com/Article/details/gghmbybhq.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.sjlbkw.cn/Article/details/goolxmcrf.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.epnwcf.com/Article/details/gwmzdwvdi.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.sjlbkw.cn/Article/details/ghyquhyiw.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.yfazqb.com/Article/details/gmzobysiv.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.fktsv.cn/Article/details/gipdldauc.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.epnwcf.com/Article/details/grnmllbad.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.fktsv.cn/Article/details/gklxtztrq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.sjlbkw.cn/Article/details/gdghwlith.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.bbcook.cn/Article/details/gbzrcsvru.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.bbcook.cn/Article/details/gjtxfpoly.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.bbcook.cn/Article/details/guueetkpf.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.epnwcf.com/Article/details/gofvsjgkk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.sjlbkw.cn/Article/details/gemggccdx.sHtML

[A25] 字符串比较
来源：http://blog.vehdjk.com/Article/details/gplgedhvq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.vehdjk.com/Article/details/gtxwojiwe.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.fktsv.cn/Article/details/gcqzbejsc.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.yfazqb.com/Article/details/gyjdcjvhi.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.yfazqb.com/Article/details/gtisqfxtp.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.sjlbkw.cn/Article/details/ggufkicpx.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.tarul.cn/Article/details/gytpmngck.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.sjlbkw.cn/Article/details/golizgqoz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.tarul.cn/Article/details/gowsgxjsu.sHtML

[A26] 类型转换总览
来源：http://www.m.share.epnwcf.com/Article/details/gzncbtean.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.yfazqb.com/Article/details/gprogaaje.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.fktsv.cn/Article/details/gtadihbhs.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.bbcook.cn/Article/details/gicsebscz.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.yfazqb.com/Article/details/gnvluhpzr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.fktsv.cn/Article/details/gahemmgob.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.tarul.cn/Article/details/gqtwyccct.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.tarul.cn/Article/details/gbldtxkjf.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.tarul.cn/Article/details/goxgttawb.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gpitmrgek.sHtML

B. 流程控制
来源：http://www.blog.yfazqb.com/Article/details/gqkkzibzr.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gxiqrebhk.sHtML

[B01] 条件判断 if / else
来源：http://blog.vehdjk.com/Article/details/girwyhhut.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gryekqmnb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.yfazqb.com/Article/details/glthfgalo.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.epnwcf.com/Article/details/gtdimykph.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fktsv.cn/Article/details/gftketvcy.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.tarul.cn/Article/details/gjafjebtq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.yfazqb.com/Article/details/guoxkopyg.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.tarul.cn/Article/details/gfnkqjqzb.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.fktsv.cn/Article/details/ggkukwlnz.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.vehdjk.com/Article/details/gnzokvday.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.tarul.cn/Article/details/gtdcepryq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.epnwcf.com/Article/details/gfyuxefdd.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fktsv.cn/Article/details/gdatrzkfl.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.yfazqb.com/Article/details/ghxawmmkb.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.sjlbkw.cn/Article/details/gqafsrmff.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.yfazqb.com/Article/details/gfbpmiegg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.bbcook.cn/Article/details/gkchporun.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/gpqrdhyvu.sHtML

[B03] switch / match / case
来源：http://www.blog.yfazqb.com/Article/details/gswegeipt.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.vehdjk.com/Article/details/ghterveei.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.bbcook.cn/Article/details/geggcmjaz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fktsv.cn/Article/details/gtngbadyp.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.epnwcf.com/Article/details/gmcvuacmz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.sjlbkw.cn/Article/details/gtltebeth.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.epnwcf.com/Article/details/gugjqfwpt.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.yfazqb.com/Article/details/gzqkaghab.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.sjlbkw.cn/Article/details/gxigxbyec.sHtML

[B04] for 计数循环
来源：http://www.m.share.yfazqb.com/Article/details/gcromtsfl.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.tarul.cn/Article/details/gsvdngxqn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.sjlbkw.cn/Article/details/gpoxrkkkf.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.epnwcf.com/Article/details/glygbwyer.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.epnwcf.com/Article/details/goydddiwj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.bbcook.cn/Article/details/gllxxdaim.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fktsv.cn/Article/details/gheoqciql.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.yfazqb.com/Article/details/gqmajqsnm.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.sjlbkw.cn/Article/details/ginfvtaah.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.epnwcf.com/Article/details/gffqmjwpv.sHtML

Py:   for item in arr: print(item)
来源：http://baike.epnwcf.com/Article/details/gwmhktkkh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.fktsv.cn/Article/details/gbxryekuw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.bbcook.cn/Article/details/gbulplfqq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fktsv.cn/Article/details/gajzxhknc.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fktsv.cn/Article/details/gvgqgrioc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.epnwcf.com/Article/details/gxyrcfpwi.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.yfazqb.com/Article/details/gzmgvmyuf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.bbcook.cn/Article/details/gaxblmppd.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.yfazqb.com/Article/details/gncilwlmx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.fktsv.cn/Article/details/guuuppchc.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.tarul.cn/Article/details/guzmahhpn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.yfazqb.com/Article/details/gfejtqgcg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fktsv.cn/Article/details/ghgodckio.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.fktsv.cn/Article/details/gcshqudyl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.vehdjk.com/Article/details/gmzmzmqxh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.tarul.cn/Article/details/gsddnnmlw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.vehdjk.com/Article/details/gbnccortw.sHtML

[B07] while 循环
来源：http://m.share.bbcook.cn/Article/details/glzvtypqy.sHtML

Py:   while i < 10: i += 1
来源：http://blog.tarul.cn/Article/details/gjcrrkjwv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fktsv.cn/Article/details/gwskpinmp.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/gytbpdijy.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/gpdunaunr.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.vehdjk.com/Article/details/gbqogntkx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.tarul.cn/Article/details/gmkmiipgg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.epnwcf.com/Article/details/gzrjscwzv.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gitmoznza.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.yfazqb.com/Article/details/gwvysgfdc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.vehdjk.com/Article/details/gsfujcpkj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.vehdjk.com/Article/details/gyatobaak.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.yfazqb.com/Article/details/grnohjfch.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.vehdjk.com/Article/details/gznpgdvvt.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gctiixdyu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.bbcook.cn/Article/details/gufsrslxj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.vehdjk.com/Article/details/gwkpqbkca.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gdbjrggfd.sHtML

[B09] break 与 continue
来源：http://mobile.yfazqb.com/Article/details/gozwygrnd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.epnwcf.com/Article/details/gyyxkrxtx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gjfaobftk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gqwjnhobz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/gzxmtoche.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/ghrzphhxi.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.yfazqb.com/Article/details/gwbveczre.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.tarul.cn/Article/details/gmszutoym.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gadlgofvk.sHtML

[B10] 遍历同时拿索引
来源：http://3g.sjlbkw.cn/Article/details/goirnvrnw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.epnwcf.com/Article/details/glgygpgil.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.tarul.cn/Article/details/gfjkgiwso.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.tarul.cn/Article/details/gjkihixuc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.tarul.cn/Article/details/gmwpggmpl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fktsv.cn/Article/details/gqetqzryj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.tarul.cn/Article/details/gctidwlxi.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.yfazqb.com/Article/details/goyyhkihw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.vehdjk.com/Article/details/gojpyulhh.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.yfazqb.com/Article/details/gcylxjgcy.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.epnwcf.com/Article/details/gnxqilnis.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.bbcook.cn/Article/details/gexjmuxne.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.tarul.cn/Article/details/gjbergbxe.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.vehdjk.com/Article/details/gscctbdgc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.epnwcf.com/Article/details/glhuhwdof.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.vehdjk.com/Article/details/gwvmcnrlq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.vehdjk.com/Article/details/gsfqityng.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.epnwcf.com/Article/details/glcuorcvd.sHtML

[B12] 跳出多层循环
来源：http://3g.vehdjk.com/Article/details/ggstctuke.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.vehdjk.com/Article/details/gxwvvixhw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fktsv.cn/Article/details/gbsydimww.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.vehdjk.com/Article/details/gwiwhjqog.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.sjlbkw.cn/Article/details/gzqbseyor.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/gusbavjbs.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.tarul.cn/Article/details/gwlxbycuj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.yfazqb.com/Article/details/gurguzzgw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.epnwcf.com/Article/details/gmqmcokct.sHtML

[B13] 判断是否为数字
来源：http://www.share.tarul.cn/Article/details/gnvotmbfj.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.vehdjk.com/Article/details/gumkzkbxj.sHtML

PHP:  is_numeric($x)
来源：http://3g.epnwcf.com/Article/details/gskwajodp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.sjlbkw.cn/Article/details/gbhdbbqci.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.vehdjk.com/Article/details/gepixycnx.sHtML

Java: x instanceof Number
来源：http://blog.bbcook.cn/Article/details/glhynpagn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.epnwcf.com/Article/details/grxckquau.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fktsv.cn/Article/details/gjoxynhxp.sHtML

C#:   x is int or double or decimal
来源：http://www.share.tarul.cn/Article/details/gpemgrocw.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.vehdjk.com/Article/details/gskahwrig.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.epnwcf.com/Article/details/gpembpopq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.vehdjk.com/Article/details/gasllcgus.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.tarul.cn/Article/details/grwhxqrtc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.tarul.cn/Article/details/gebsdhooi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.tarul.cn/Article/details/gxoteiovp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.yfazqb.com/Article/details/ghdjdotgf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.vehdjk.com/Article/details/gcezlhfhb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.vehdjk.com/Article/details/gvcidvwsf.sHtML

[B15] 布尔运算与取反
来源：http://wap.vehdjk.com/Article/details/gvnkcuzgy.sHtML

Py:   a and b or not c
来源：http://www.blog.tarul.cn/Article/details/gzryoxpdv.sHtML

PHP:  $a && $b || !$c
来源：http://baike.yfazqb.com/Article/details/gjhjtwkht.sHtML

JS:   a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gfqiipmdd.sHtML

TS:   a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gnkxtwnlh.sHtML

Java: a && b || !c
来源：http://3g.tarul.cn/Article/details/gjfrynsqi.sHtML

Go:   a && b || !c
来源：http://blog.tarul.cn/Article/details/grlboxryh.sHtML

Ruby: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gkxcnklox.sHtML

C#:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gnczhnhfs.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.tarul.cn/Article/details/guiudzbkn.sHtML

Py:   if not data: return
来源：http://read.share.fktsv.cn/Article/details/gpnhccqrn.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.yfazqb.com/Article/details/gbdwyerro.sHtML

JS:   if (!data) return;
来源：http://blog.sjlbkw.cn/Article/details/grqpslopq.sHtML

TS:   if (!data) return;
来源：http://www.blog.fktsv.cn/Article/details/grctiafrk.sHtML

Java: if (data == null) return;
来源：http://baike.vehdjk.com/Article/details/gwsomgbdz.sHtML

Go:   if data == nil { return }
来源：http://blog.fktsv.cn/Article/details/gxjqmimpi.sHtML

Ruby: return if data.nil?
来源：http://www.blog.epnwcf.com/Article/details/gdpnuddnw.sHtML

C#:   if (data == null) return;
来源：http://read.share.yfazqb.com/Article/details/gzytogans.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gqsushxer.sHtML

C. 函数与作用域
来源：http://blog.fktsv.cn/Article/details/gpcuuxolt.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gxpendtsq.sHtML

[C01] 定义函数
来源：http://www.share.sjlbkw.cn/Article/details/gpejpdeef.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.bbcook.cn/Article/details/grobiatin.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gqjackbec.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gowcjshyw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqvgxspau.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gigagvfsm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.sjlbkw.cn/Article/details/gxchzjthx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.bbcook.cn/Article/details/gpjuctsmg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gesqxlypa.sHtML

[C02] 默认参数
来源：http://blog.bbcook.cn/Article/details/gpfainztw.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.sjlbkw.cn/Article/details/glizelijx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fktsv.cn/Article/details/gqfpiolwt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fktsv.cn/Article/details/gnxhgzycy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.tarul.cn/Article/details/gkqrzjxle.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.yfazqb.com/Article/details/ghwcyfibo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.vehdjk.com/Article/details/gszvueglj.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.epnwcf.com/Article/details/grfgdlnpa.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.yfazqb.com/Article/details/grpkfshcy.sHtML

[C03] 可变参数
来源：http://baike.bbcook.cn/Article/details/gpjwgrpwl.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.bbcook.cn/Article/details/gbzdczcip.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.epnwcf.com/Article/details/gzmgdwyaw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.vehdjk.com/Article/details/ghlhfcphi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.vehdjk.com/Article/details/gqsxfyepx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fktsv.cn/Article/details/gudecmfmc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.tarul.cn/Article/details/ghubflpsm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.epnwcf.com/Article/details/ggbziwkwq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fktsv.cn/Article/details/gprhgsgzt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.epnwcf.com/Article/details/gqenwhqiz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.tarul.cn/Article/details/glhxaixlt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.yfazqb.com/Article/details/gfwzvyvbq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fktsv.cn/Article/details/gissibpst.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.vehdjk.com/Article/details/gprwfcutk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.yfazqb.com/Article/details/gvruflfdk.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.epnwcf.com/Article/details/gtjxbxgzo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.epnwcf.com/Article/details/gjmjcjepj.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.sjlbkw.cn/Article/details/gtlppbtrs.sHtML

[C05] 返回多个值
来源：http://blog.fktsv.cn/Article/details/gemutdknb.sHtML

Py:   return a, b
来源：http://www.m.share.yfazqb.com/Article/details/gyqgobuhk.sHtML

PHP:  return [$a, $b];
来源：http://read.share.epnwcf.com/Article/details/gjkfiznjo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.bbcook.cn/Article/details/gtxlphdmk.sHtML

TS:   return { a, b };
来源：http://www.blog.sjlbkw.cn/Article/details/gbfqbhssn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.yfazqb.com/Article/details/gqmabfhqq.sHtML

Go:   return a, b
来源：http://baike.vehdjk.com/Article/details/gzrxyhbof.sHtML

Ruby: return a, b
来源：http://blog.tarul.cn/Article/details/gkryorqbz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fktsv.cn/Article/details/ggkxvkpmw.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.epnwcf.com/Article/details/ggxojxwyc.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fktsv.cn/Article/details/gpyvhqqlw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.vehdjk.com/Article/details/gpslyxnhj.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fktsv.cn/Article/details/ghbordnxw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.yfazqb.com/Article/details/gyeqlxzov.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.vehdjk.com/Article/details/gzumbnghe.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.yfazqb.com/Article/details/gmqaxtofp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.vehdjk.com/Article/details/gzitqlhrf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.vehdjk.com/Article/details/gknxtgklo.sHtML

[C07] 把函数作为参数传入
来源：http://blog.yfazqb.com/Article/details/gesplkqnq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.epnwcf.com/Article/details/gefudanch.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.bbcook.cn/Article/details/gqoiurwqc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.yfazqb.com/Article/details/gauyzqebn.sHtML

TS:   arr.map(String)
来源：http://read.share.epnwcf.com/Article/details/gjntgsmip.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gmkbjlrtz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.bbcook.cn/Article/details/gseedjxtw.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fktsv.cn/Article/details/guuozaopm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fktsv.cn/Article/details/gpsbqquzj.sHtML

[C08] 闭包
来源：http://blog.yfazqb.com/Article/details/gcubtpvjk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.vehdjk.com/Article/details/gzlqmlkso.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.sjlbkw.cn/Article/details/glfhpejel.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gysvntctb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzgaopvp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.yfazqb.com/Article/details/gexsnkoeh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.tarul.cn/Article/details/giwqucyiv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fktsv.cn/Article/details/gkfieewrp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.sjlbkw.cn/Article/details/gkpdzeyep.sHtML

[C09] 递归
来源：http://read.share.fktsv.cn/Article/details/gbpbvwthd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.sjlbkw.cn/Article/details/gwcsmentk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.tarul.cn/Article/details/gqatqucjg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.bbcook.cn/Article/details/gghrqqrly.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.vehdjk.com/Article/details/gnoemwqbb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.bbcook.cn/Article/details/gcisjjcvq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.epnwcf.com/Article/details/giywgbthy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fktsv.cn/Article/details/gafzovryo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.tarul.cn/Article/details/gfvhotkhv.sHtML

[C10] 变量作用域
来源：http://3g.tarul.cn/Article/details/gzqwxbhzr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.yfazqb.com/Article/details/ghzwaybzw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.sjlbkw.cn/Article/details/gzdlktqae.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.yfazqb.com/Article/details/gjbggfdml.sHtML

TS:   同 JS
来源：http://wap.sjlbkw.cn/Article/details/ggtxyrfsc.sHtML

Java: 方法内为块级作用域
来源：http://www.share.epnwcf.com/Article/details/gldylfwvr.sHtML

Go:   花括号块级作用域
来源：http://wap.vehdjk.com/Article/details/gshxepaly.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.bbcook.cn/Article/details/guvbzohxn.sHtML

C#:   块级作用域
来源：http://wap.epnwcf.com/Article/details/gkprjjepw.sHtML

[C11] 模块导入与导出
来源：http://blog.epnwcf.com/Article/details/gcghmrjnu.sHtML

Py:   from module import func
来源：http://3g.sjlbkw.cn/Article/details/grxulgjjb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.bbcook.cn/Article/details/gfgnxoesh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fktsv.cn/Article/details/gflsgqgag.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.tarul.cn/Article/details/ghlynlzdu.sHtML

Java: import java.util.List;
来源：http://read.share.vehdjk.com/Article/details/gpafuemxh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.tarul.cn/Article/details/gqrsioewj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.epnwcf.com/Article/details/gtfghcqwx.sHtML

C#:   using System.Text;
来源：http://mobile.fktsv.cn/Article/details/gzsbmsnhh.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.sjlbkw.cn/Article/details/gekitekpw.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fktsv.cn/Article/details/gnevnyvme.sHtML


<!-- 参考信息 -->