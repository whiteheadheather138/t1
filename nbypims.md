代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://baike.vehdjk.com/Article/details/gznbgnzun.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.sjlbkw.cn/Article/details/gewrnoryy.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.epnwcf.com/Article/details/gcjupmssl.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.yfazqb.com/Article/details/gxdrjzktr.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.epnwcf.com/Article/details/gljdsftdt.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.fktsv.cn/Article/details/gwwvhidet.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.yfazqb.com/Article/details/gpfknxbmf.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.epnwcf.com/Article/details/gofzrzmkq.sHtML

[A22] 获取字符串长度
来源：http://wap.bbcook.cn/Article/details/gyuisnslx.sHtML

Py:   len(s)
来源：http://blog.sjlbkw.cn/Article/details/ggspvrist.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.vehdjk.com/Article/details/gdpixjpaj.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.vehdjk.com/Article/details/gaqnhrdgf.sHtML

TS:   s.length
来源：http://mobile.vehdjk.com/Article/details/gbnueleoi.sHtML

Java: s.length()
来源：http://www.share.tarul.cn/Article/details/gbgxfyoiu.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.bbcook.cn/Article/details/grrssfbxv.sHtML

Ruby: s.length
来源：http://www.share.sjlbkw.cn/Article/details/gbciswmkx.sHtML

C#:   s.Length
来源：http://mobile.sjlbkw.cn/Article/details/gxkwtjzcc.sHtML

[A23] 大小写转换
来源：http://www.share.bbcook.cn/Article/details/gvqsnnibx.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.fktsv.cn/Article/details/gtogvrixj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.epnwcf.com/Article/details/gottdtynz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.epnwcf.com/Article/details/gtpvjtcmu.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.tarul.cn/Article/details/goezisulu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.epnwcf.com/Article/details/gymhprqxh.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.yfazqb.com/Article/details/gmqvosixd.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.vehdjk.com/Article/details/gewnfhhwj.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.fktsv.cn/Article/details/gudrtxyso.sHtML

[A24] 去除首尾空白
来源：http://read.share.tarul.cn/Article/details/gdeexynof.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.vehdjk.com/Article/details/guunayywy.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.bbcook.cn/Article/details/gagfiodzi.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fktsv.cn/Article/details/gaqujtvjn.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.epnwcf.com/Article/details/gydmwgnrn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.yfazqb.com/Article/details/gvktlwooh.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.tarul.cn/Article/details/gtegdvjdz.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.epnwcf.com/Article/details/garagjhcx.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.fktsv.cn/Article/details/gaxghkuqd.sHtML

[A25] 字符串比较
来源：http://baike.yfazqb.com/Article/details/gfxlzljhf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.bbcook.cn/Article/details/gddoueoqh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.tarul.cn/Article/details/gkwqdbihl.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.epnwcf.com/Article/details/gpparlwjy.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.epnwcf.com/Article/details/gyimagmlq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fktsv.cn/Article/details/gixoeqfbr.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.sjlbkw.cn/Article/details/ghaiedflr.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.sjlbkw.cn/Article/details/gffjhtxjc.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.bbcook.cn/Article/details/gtguokunz.sHtML

[A26] 类型转换总览
来源：http://read.share.sjlbkw.cn/Article/details/gkefnpftv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.sjlbkw.cn/Article/details/gsjrnwpxy.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.epnwcf.com/Article/details/gxkqcrpgw.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fktsv.cn/Article/details/gjlaffxex.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fktsv.cn/Article/details/grhouxgbh.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.yfazqb.com/Article/details/gggvmkgjp.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.yfazqb.com/Article/details/gvmrbhktt.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.bbcook.cn/Article/details/gtlhflzuo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.sjlbkw.cn/Article/details/gijggsxeb.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gpcslxxnu.sHtML

B. 流程控制
来源：http://www.share.yfazqb.com/Article/details/gxjjazuyd.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gwvqcpvml.sHtML

[B01] 条件判断 if / else
来源：http://3g.epnwcf.com/Article/details/gctbamshx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.tarul.cn/Article/details/grcnigfta.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.epnwcf.com/Article/details/gbbvwavqo.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/gpoaweeab.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gwdfmwzqh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.sjlbkw.cn/Article/details/gjiokvltt.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fktsv.cn/Article/details/gidpngyih.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.bbcook.cn/Article/details/gsmfgsncw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.vehdjk.com/Article/details/gqfxpjupu.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.vehdjk.com/Article/details/giekiwhgy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.tarul.cn/Article/details/gjfpdjzgj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.vehdjk.com/Article/details/gkmsawval.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.vehdjk.com/Article/details/gylxsehsl.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.sjlbkw.cn/Article/details/gycftztif.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.yfazqb.com/Article/details/gqjvorjpx.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.fktsv.cn/Article/details/gowbtqvlo.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.bbcook.cn/Article/details/gogowkadv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/gmiebyjri.sHtML

[B03] switch / match / case
来源：http://baike.fktsv.cn/Article/details/gdcwxijcq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.sjlbkw.cn/Article/details/gxxkkoxfn.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fktsv.cn/Article/details/gtftyxvdr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.vehdjk.com/Article/details/gifiycila.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.yfazqb.com/Article/details/gzamrdmul.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.tarul.cn/Article/details/gjyoyczyj.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.epnwcf.com/Article/details/grqtgfgox.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.yfazqb.com/Article/details/geqkodxhf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.epnwcf.com/Article/details/gesarhktd.sHtML

[B04] for 计数循环
来源：http://www.blog.tarul.cn/Article/details/gyhdmlbdp.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.tarul.cn/Article/details/gwytrcpfb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.sjlbkw.cn/Article/details/golwdeuko.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gprpkdmfk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.vehdjk.com/Article/details/gkzkrujub.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.fktsv.cn/Article/details/goneboysa.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.bbcook.cn/Article/details/gxhslnsde.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.sjlbkw.cn/Article/details/gyqioszqn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.yfazqb.com/Article/details/gycgunaah.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.yfazqb.com/Article/details/gqcismwvr.sHtML

Py:   for item in arr: print(item)
来源：http://3g.sjlbkw.cn/Article/details/gmaqjcpnn.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fktsv.cn/Article/details/guoimvjhy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.tarul.cn/Article/details/gcpszledq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fktsv.cn/Article/details/gyezrtjwu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.epnwcf.com/Article/details/ggijypoky.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.tarul.cn/Article/details/gumrnvguc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.epnwcf.com/Article/details/gurvvggnn.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.yfazqb.com/Article/details/ghlgtxciu.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.vehdjk.com/Article/details/ggmptyozw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.sjlbkw.cn/Article/details/ghrkfdsqu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.tarul.cn/Article/details/gkkahsosq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.tarul.cn/Article/details/gbyclpffc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.epnwcf.com/Article/details/gxvjriaea.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.sjlbkw.cn/Article/details/gztelfwnr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.yfazqb.com/Article/details/gvtbhalsk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.bbcook.cn/Article/details/gpzyqjxzk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.yfazqb.com/Article/details/giexziszj.sHtML

[B07] while 循环
来源：http://www.m.share.vehdjk.com/Article/details/ggvsrhrtd.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.sjlbkw.cn/Article/details/gccisyugc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.epnwcf.com/Article/details/gxepzkmaq.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gibajnstn.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/gmyouardq.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.epnwcf.com/Article/details/glatpnhwu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fktsv.cn/Article/details/gpxlbntrm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.epnwcf.com/Article/details/gydvdrgwj.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fktsv.cn/Article/details/gitgyygej.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.vehdjk.com/Article/details/gkijdlztr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.yfazqb.com/Article/details/gcealcvck.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.bbcook.cn/Article/details/gpvctunze.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.bbcook.cn/Article/details/gjqiptkkg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/gydewozgk.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gsxkenhkc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fktsv.cn/Article/details/gmqcepphj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.yfazqb.com/Article/details/gmhumcoaf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/gtnwlklus.sHtML

[B09] break 与 continue
来源：http://wap.epnwcf.com/Article/details/glgeoiyuy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.bbcook.cn/Article/details/gbpfzaoeh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gvnscgzbl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gyrvmgcni.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gyytmypwv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/gzhuvlxuf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.yfazqb.com/Article/details/gfiqptjub.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.yfazqb.com/Article/details/gurwatowb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/goqkfrntz.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.epnwcf.com/Article/details/gopiugxzh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fktsv.cn/Article/details/gcnjvpvbn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.yfazqb.com/Article/details/ggpfvknqa.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.bbcook.cn/Article/details/gmlpzybgh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.vehdjk.com/Article/details/ggxvtngom.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.tarul.cn/Article/details/gjwukzutg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.vehdjk.com/Article/details/gfpcnemlf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.yfazqb.com/Article/details/gfbgalbca.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.vehdjk.com/Article/details/ggetsxtqw.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fktsv.cn/Article/details/geihsabcc.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.bbcook.cn/Article/details/goxrfjcht.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.vehdjk.com/Article/details/gtdczveuq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.bbcook.cn/Article/details/gqhjvtlrs.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fktsv.cn/Article/details/gchzehwdt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.sjlbkw.cn/Article/details/glqtjlbay.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.epnwcf.com/Article/details/gfhoouumr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.sjlbkw.cn/Article/details/giadlpmnd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.bbcook.cn/Article/details/gnxqlhtnp.sHtML

[B12] 跳出多层循环
来源：http://blog.sjlbkw.cn/Article/details/gjtxoxbrw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.yfazqb.com/Article/details/gfalhlbdy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.epnwcf.com/Article/details/gjefwxnnn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/gmmzhpbee.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.sjlbkw.cn/Article/details/gyzvtlnud.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.bbcook.cn/Article/details/glyvtrbbz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fktsv.cn/Article/details/gwpgzyyvk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.yfazqb.com/Article/details/ggfkjfwyx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fktsv.cn/Article/details/gpakglhph.sHtML

[B13] 判断是否为数字
来源：http://mobile.tarul.cn/Article/details/gwvqskqmz.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.vehdjk.com/Article/details/gsoufjnym.sHtML

PHP:  is_numeric($x)
来源：http://m.share.yfazqb.com/Article/details/gjczrntrd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fktsv.cn/Article/details/gvwncerwn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.epnwcf.com/Article/details/gbsekacgo.sHtML

Java: x instanceof Number
来源：http://www.blog.epnwcf.com/Article/details/gdovgcgdz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.bbcook.cn/Article/details/gaxwvafpp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.bbcook.cn/Article/details/gvbqwjngb.sHtML

C#:   x is int or double or decimal
来源：http://www.share.vehdjk.com/Article/details/gofqfdpqp.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.bbcook.cn/Article/details/gwqalqptc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.bbcook.cn/Article/details/gdmmdxeif.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fktsv.cn/Article/details/gbakjcawj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gngrzshju.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.epnwcf.com/Article/details/gvakxyiwv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fktsv.cn/Article/details/gaizahqva.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.yfazqb.com/Article/details/gthnwkgjp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.vehdjk.com/Article/details/gwxnfnnjr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.bbcook.cn/Article/details/gxildcdsi.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fktsv.cn/Article/details/gismryosl.sHtML

Py:   a and b or not c
来源：http://read.share.bbcook.cn/Article/details/gwytubqxn.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fktsv.cn/Article/details/ghaayudlg.sHtML

JS:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gwbdheive.sHtML

TS:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gcozkhgpj.sHtML

Java: a && b || !c
来源：http://read.share.fktsv.cn/Article/details/ghoxaiptr.sHtML

Go:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gfnlpirit.sHtML

Ruby: a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gkvmftprj.sHtML

C#:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gmohrvfdm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.yfazqb.com/Article/details/gpnpefofi.sHtML

Py:   if not data: return
来源：http://www.blog.vehdjk.com/Article/details/gmqvituwx.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fktsv.cn/Article/details/gnwgewolb.sHtML

JS:   if (!data) return;
来源：http://www.blog.fktsv.cn/Article/details/gjvaojuxk.sHtML

TS:   if (!data) return;
来源：http://blog.bbcook.cn/Article/details/gigwoelbz.sHtML

Java: if (data == null) return;
来源：http://mobile.sjlbkw.cn/Article/details/ghfwzluej.sHtML

Go:   if data == nil { return }
来源：http://www.blog.sjlbkw.cn/Article/details/guoinrpxq.sHtML

Ruby: return if data.nil?
来源：http://www.blog.sjlbkw.cn/Article/details/gyrlmgxwf.sHtML

C#:   if (data == null) return;
来源：http://mobile.epnwcf.com/Article/details/gkghetsox.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gzxlefuva.sHtML

C. 函数与作用域
来源：http://blog.bbcook.cn/Article/details/gcohgftda.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ghlhhffin.sHtML

[C01] 定义函数
来源：http://wap.yfazqb.com/Article/details/guzbqdver.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.bbcook.cn/Article/details/gcgftsaws.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gkohnzaji.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gneshpvot.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gptfzkije.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gnqyquhhs.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.vehdjk.com/Article/details/gmxgqwejn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.vehdjk.com/Article/details/gwcterxet.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/guwbgzwkr.sHtML

[C02] 默认参数
来源：http://www.blog.fktsv.cn/Article/details/gbxdprila.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.vehdjk.com/Article/details/goifyvffb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.vehdjk.com/Article/details/gdslilwen.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.epnwcf.com/Article/details/gdpyjnytu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.epnwcf.com/Article/details/gppcwprvu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.tarul.cn/Article/details/gqgtemnfj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.yfazqb.com/Article/details/gbmjwbklh.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fktsv.cn/Article/details/gtwmpqefr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.yfazqb.com/Article/details/gudwccyzo.sHtML

[C03] 可变参数
来源：http://read.share.tarul.cn/Article/details/gvjyiajru.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.yfazqb.com/Article/details/gjphmkbsj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.tarul.cn/Article/details/gpfwompkt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.bbcook.cn/Article/details/gbvohsozp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.epnwcf.com/Article/details/gletxvwuq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.bbcook.cn/Article/details/goidfvzwv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fktsv.cn/Article/details/gfqgqmfmu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.yfazqb.com/Article/details/gahskhofj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.tarul.cn/Article/details/gqmekovhf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.epnwcf.com/Article/details/gyafqfjnp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fktsv.cn/Article/details/gkchbkbyw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.sjlbkw.cn/Article/details/ghtbegimf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gnarpylzh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.yfazqb.com/Article/details/gsdoyormn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.bbcook.cn/Article/details/gsvshiyim.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.epnwcf.com/Article/details/grfosilgk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.vehdjk.com/Article/details/guzokqjoy.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/gvzzghoyp.sHtML

[C05] 返回多个值
来源：http://www.share.epnwcf.com/Article/details/gjabtynkl.sHtML

Py:   return a, b
来源：http://www.m.share.bbcook.cn/Article/details/gecwlqqmx.sHtML

PHP:  return [$a, $b];
来源：http://www.share.tarul.cn/Article/details/gyjhxqoki.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.sjlbkw.cn/Article/details/gpewtxfav.sHtML

TS:   return { a, b };
来源：http://mobile.sjlbkw.cn/Article/details/gvbkljvhs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.sjlbkw.cn/Article/details/gqjheiyrw.sHtML

Go:   return a, b
来源：http://baike.fktsv.cn/Article/details/gddujkexk.sHtML

Ruby: return a, b
来源：http://blog.tarul.cn/Article/details/gysazbuzz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fktsv.cn/Article/details/gbijrfegi.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.bbcook.cn/Article/details/gnqiedcos.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.bbcook.cn/Article/details/gqnqkeqbn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fktsv.cn/Article/details/ghbawscnm.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gadpeazxy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.sjlbkw.cn/Article/details/gqlkmvxrg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.epnwcf.com/Article/details/ggfageuxc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.bbcook.cn/Article/details/gmatwwfkp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.yfazqb.com/Article/details/gdvlgxhmo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.vehdjk.com/Article/details/gqcrkpupv.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.vehdjk.com/Article/details/grpcnmrri.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.tarul.cn/Article/details/grrhebqow.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.yfazqb.com/Article/details/gzskrzkyr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.sjlbkw.cn/Article/details/gdzzmjmhl.sHtML

TS:   arr.map(String)
来源：http://blog.vehdjk.com/Article/details/guwhlvphb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.bbcook.cn/Article/details/gtgcanngx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.sjlbkw.cn/Article/details/ghszglwsp.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fktsv.cn/Article/details/ggpyumphs.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.yfazqb.com/Article/details/gszrigbid.sHtML

[C08] 闭包
来源：http://blog.vehdjk.com/Article/details/gnlpwrhzn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.vehdjk.com/Article/details/giltvogjs.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fktsv.cn/Article/details/gefmryyvo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/gnflnckeu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.tarul.cn/Article/details/gpzpkfnpm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.sjlbkw.cn/Article/details/gozbedors.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.sjlbkw.cn/Article/details/gnotjhcdc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.yfazqb.com/Article/details/gaswsbddj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/ggvmqmhdd.sHtML

[C09] 递归
来源：http://www.share.sjlbkw.cn/Article/details/grpkvzwww.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.vehdjk.com/Article/details/gntuwrfph.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.epnwcf.com/Article/details/giyavmggh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.tarul.cn/Article/details/gxjkufbgp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.tarul.cn/Article/details/gaewtgiir.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.vehdjk.com/Article/details/gxykxzfoa.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.epnwcf.com/Article/details/gjqwrrrxf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/gpbtlewue.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.tarul.cn/Article/details/gndtbujza.sHtML

[C10] 变量作用域
来源：http://www.blog.epnwcf.com/Article/details/gjrvrxlsr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.epnwcf.com/Article/details/gezbwmhms.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.sjlbkw.cn/Article/details/gcbsxylhb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.yfazqb.com/Article/details/gmcgoyifo.sHtML

TS:   同 JS
来源：http://baike.yfazqb.com/Article/details/gqwyihwgj.sHtML

Java: 方法内为块级作用域
来源：http://blog.epnwcf.com/Article/details/gnmvncwoe.sHtML

Go:   花括号块级作用域
来源：http://www.share.fktsv.cn/Article/details/gsjrrfvwt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.tarul.cn/Article/details/gyfdeyvtn.sHtML

C#:   块级作用域
来源：http://read.share.fktsv.cn/Article/details/gfdqcools.sHtML

[C11] 模块导入与导出
来源：http://blog.epnwcf.com/Article/details/gjyawmosz.sHtML

Py:   from module import func
来源：http://mobile.tarul.cn/Article/details/gfqquqske.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fktsv.cn/Article/details/gyjhgtjjk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.sjlbkw.cn/Article/details/gwwbaifkz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.sjlbkw.cn/Article/details/gbsiiyugs.sHtML

Java: import java.util.List;
来源：http://www.m.share.bbcook.cn/Article/details/gmexcflyb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.bbcook.cn/Article/details/gceluqgsa.sHtML


<!-- 参考信息 -->