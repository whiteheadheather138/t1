代发 wailian999

JS:   [a, b] = [b, a];
来源：http://wap.tarul.cn/Article/details/gfhzztayl.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.yfazqb.com/Article/details/gwvxzbirc.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.bbcook.cn/Article/details/gjdgmyimc.sHtML

Go:   a, b = b, a
来源：http://www.share.bbcook.cn/Article/details/gpxwlwsda.sHtML

Ruby: a, b = b, a
来源：http://blog.yfazqb.com/Article/details/gugfbimjz.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.epnwcf.com/Article/details/gjglkerwq.sHtML

[A20] 读取标准输入
来源：http://mobile.bbcook.cn/Article/details/ghpvkszoh.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.bbcook.cn/Article/details/giybzfqwl.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.fktsv.cn/Article/details/gaasutxqt.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.epnwcf.com/Article/details/geaabeayq.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.yfazqb.com/Article/details/gobqymkwk.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.tarul.cn/Article/details/gialojuuw.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.bbcook.cn/Article/details/gqvafyoit.sHtML

Ruby: gets.chomp
来源：http://baike.tarul.cn/Article/details/gjldygkpo.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.vehdjk.com/Article/details/gvdwmpmjl.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.yfazqb.com/Article/details/gwcxsveab.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.bbcook.cn/Article/details/gdohqwall.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.vehdjk.com/Article/details/gfkxnqasm.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.fktsv.cn/Article/details/gpzfcgfsp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.tarul.cn/Article/details/gdezgeifw.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.tarul.cn/Article/details/geovjfajb.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.bbcook.cn/Article/details/gdbnjxqvq.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.vehdjk.com/Article/details/gkxvyyupg.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.tarul.cn/Article/details/gszkwrqwg.sHtML

[A22] 获取字符串长度
来源：http://3g.fktsv.cn/Article/details/gqlkoccdx.sHtML

Py:   len(s)
来源：http://blog.tarul.cn/Article/details/glxbxjcpr.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.yfazqb.com/Article/details/ghsrqrnfy.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.sjlbkw.cn/Article/details/ghrvsauex.sHtML

TS:   s.length
来源：http://baike.fktsv.cn/Article/details/getfcczaf.sHtML

Java: s.length()
来源：http://wap.fktsv.cn/Article/details/gkwfuebwc.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.bbcook.cn/Article/details/gxthytazm.sHtML

Ruby: s.length
来源：http://www.blog.yfazqb.com/Article/details/gbwmcjmko.sHtML

C#:   s.Length
来源：http://m.share.tarul.cn/Article/details/gnqvtrfyk.sHtML

[A23] 大小写转换
来源：http://mobile.bbcook.cn/Article/details/gssyaeclz.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.epnwcf.com/Article/details/gnypfsupn.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.bbcook.cn/Article/details/ghxfylmbr.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.yfazqb.com/Article/details/gfhbmvhmb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.epnwcf.com/Article/details/grqdndjyj.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fktsv.cn/Article/details/ghzzoscdj.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.vehdjk.com/Article/details/gshwhkwkk.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.epnwcf.com/Article/details/gksdbjlyr.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.sjlbkw.cn/Article/details/gshfpqiak.sHtML

[A24] 去除首尾空白
来源：http://wap.epnwcf.com/Article/details/ggvpiyrsg.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.vehdjk.com/Article/details/gjgyyzeyb.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.sjlbkw.cn/Article/details/gudtxolzn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.sjlbkw.cn/Article/details/grfzmuavn.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.bbcook.cn/Article/details/gfwokmcve.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.sjlbkw.cn/Article/details/ggnskixew.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.tarul.cn/Article/details/gbhlxvrxa.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.bbcook.cn/Article/details/grnrepduh.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.vehdjk.com/Article/details/gqrffwnzo.sHtML

[A25] 字符串比较
来源：http://read.share.yfazqb.com/Article/details/gdkhhplmw.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.tarul.cn/Article/details/gxbbnwtpd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.tarul.cn/Article/details/gamrwjncs.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.bbcook.cn/Article/details/gjfhokrqp.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.sjlbkw.cn/Article/details/gyrqrngxm.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.tarul.cn/Article/details/gddvmbtbn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.bbcook.cn/Article/details/gcgydthhk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.tarul.cn/Article/details/gtiqjfgkx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.fktsv.cn/Article/details/gjijcrfes.sHtML

[A26] 类型转换总览
来源：http://www.m.share.epnwcf.com/Article/details/gpqhpqryh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.bbcook.cn/Article/details/gzruwwyxh.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.tarul.cn/Article/details/gcthwffwr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.epnwcf.com/Article/details/gploojoda.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.sjlbkw.cn/Article/details/gaatrykwd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.vehdjk.com/Article/details/gjwkgponl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.vehdjk.com/Article/details/gspgsvwct.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.epnwcf.com/Article/details/gnenfiytv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.fktsv.cn/Article/details/gftzkdvah.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gissjhoph.sHtML

B. 流程控制
来源：http://m.share.bbcook.cn/Article/details/gtjmbfbzj.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gxkjhjcho.sHtML

[B01] 条件判断 if / else
来源：http://read.share.sjlbkw.cn/Article/details/gxegqzccs.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.vehdjk.com/Article/details/gfvdgzxhf.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.fktsv.cn/Article/details/gdflhmbon.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.epnwcf.com/Article/details/gpapcpasv.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/gqmamrdsi.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.tarul.cn/Article/details/girlaynis.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.vehdjk.com/Article/details/gbkkproiw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.tarul.cn/Article/details/gfxoomcpz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.vehdjk.com/Article/details/gfsumgkqs.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.epnwcf.com/Article/details/gdfbbvwng.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.sjlbkw.cn/Article/details/gsjgzjcvp.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.sjlbkw.cn/Article/details/glojxdwwk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.bbcook.cn/Article/details/geqfbuwsb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/gxjcclzwa.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/gywggdpcw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.yfazqb.com/Article/details/gxjabekaz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.bbcook.cn/Article/details/gziytcvcc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/ggijhsphu.sHtML

[B03] switch / match / case
来源：http://read.share.sjlbkw.cn/Article/details/goqmujuqh.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.bbcook.cn/Article/details/gpnxztafn.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.bbcook.cn/Article/details/ghhihtdxs.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.tarul.cn/Article/details/gnfaznmyj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gogcmsyfx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gdbvqkjbi.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.fktsv.cn/Article/details/gyfdpqahg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.bbcook.cn/Article/details/gwfhogyzv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.sjlbkw.cn/Article/details/goorvmgja.sHtML

[B04] for 计数循环
来源：http://blog.fktsv.cn/Article/details/ghopoyiqx.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fktsv.cn/Article/details/gwvxtdcmk.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.bbcook.cn/Article/details/gsnkacnsx.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.yfazqb.com/Article/details/gxhghdywv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.tarul.cn/Article/details/gkpzwfwfv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.vehdjk.com/Article/details/gszssylur.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.bbcook.cn/Article/details/gebvtppuj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.vehdjk.com/Article/details/gqbbrummy.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.fktsv.cn/Article/details/gurjkmrli.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.vehdjk.com/Article/details/gdipsahde.sHtML

Py:   for item in arr: print(item)
来源：http://baike.epnwcf.com/Article/details/gknohjgau.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.vehdjk.com/Article/details/gqogxpypf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.bbcook.cn/Article/details/grcqejxdu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fktsv.cn/Article/details/gkyjnevdo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.yfazqb.com/Article/details/gyhqoskzo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.tarul.cn/Article/details/gpqftdbpa.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.vehdjk.com/Article/details/ggpqzuwmp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.sjlbkw.cn/Article/details/guiouiyzk.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fktsv.cn/Article/details/gcitplehn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.yfazqb.com/Article/details/gckhkylrd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.yfazqb.com/Article/details/gqenhhqul.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.tarul.cn/Article/details/gdwfnkxzy.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fktsv.cn/Article/details/gpgkutrwd.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.sjlbkw.cn/Article/details/gzrjpnnxb.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.epnwcf.com/Article/details/gajiuanxf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.yfazqb.com/Article/details/gygaqquod.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.tarul.cn/Article/details/gyopoztge.sHtML

[B07] while 循环
来源：http://www.share.vehdjk.com/Article/details/ghxamthad.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.sjlbkw.cn/Article/details/grmysxyun.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.bbcook.cn/Article/details/gfciftwur.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/ghqlpahvy.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fktsv.cn/Article/details/glejwscns.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gbqietdpu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.yfazqb.com/Article/details/gfsjxgqbc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.yfazqb.com/Article/details/ghptkuayg.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/grkwynynj.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.bbcook.cn/Article/details/glqwjhxmf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.yfazqb.com/Article/details/gqshbkufk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.epnwcf.com/Article/details/gvllimcno.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/gsskcgsmk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.bbcook.cn/Article/details/gkikcrxbb.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/gtwwfskuv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fktsv.cn/Article/details/gliaccnnf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.epnwcf.com/Article/details/gtdotfvmn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gvuoabgba.sHtML

[B09] break 与 continue
来源：http://wap.epnwcf.com/Article/details/ggqzmnsrb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.sjlbkw.cn/Article/details/gnlcdhlaq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gpyisinvo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gxvfaxqsu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/gjtabgyun.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gdpluqppn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.vehdjk.com/Article/details/gshachlny.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.vehdjk.com/Article/details/gsqckjlsn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/gdoqmwunm.sHtML

[B10] 遍历同时拿索引
来源：http://3g.tarul.cn/Article/details/ghzpywemq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.yfazqb.com/Article/details/gubanvrqh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.tarul.cn/Article/details/gvedgjnqt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.bbcook.cn/Article/details/gszmslecn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.bbcook.cn/Article/details/gtqlnexdk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.bbcook.cn/Article/details/gwyusczfg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fktsv.cn/Article/details/ghhavphwr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.yfazqb.com/Article/details/gvdgjafhk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.epnwcf.com/Article/details/gcyqphvoz.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.sjlbkw.cn/Article/details/gjhjyffpk.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.vehdjk.com/Article/details/gcpwwzlyx.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.epnwcf.com/Article/details/gqsfyihks.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.sjlbkw.cn/Article/details/gdapotscj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.yfazqb.com/Article/details/ggugxatyt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.tarul.cn/Article/details/gfodwgfqf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.sjlbkw.cn/Article/details/glpgapzcv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.tarul.cn/Article/details/ghvfzxjsw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.epnwcf.com/Article/details/gwoihogfi.sHtML

[B12] 跳出多层循环
来源：http://baike.tarul.cn/Article/details/gptsicber.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.sjlbkw.cn/Article/details/ghrmpurjc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.yfazqb.com/Article/details/ggwfsggcu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/garwjaxtl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.yfazqb.com/Article/details/gljsnrlue.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/gbdblfwny.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.bbcook.cn/Article/details/gkiyhgsmr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.bbcook.cn/Article/details/gxtgvfnvc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fktsv.cn/Article/details/gbtucenaw.sHtML

[B13] 判断是否为数字
来源：http://wap.vehdjk.com/Article/details/gctshyuxq.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.epnwcf.com/Article/details/gocboduzb.sHtML

PHP:  is_numeric($x)
来源：http://www.share.vehdjk.com/Article/details/gnhhfklja.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.epnwcf.com/Article/details/gmfsxwnbc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.tarul.cn/Article/details/gbixuvoyd.sHtML

Java: x instanceof Number
来源：http://3g.sjlbkw.cn/Article/details/gbdzowbsm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.yfazqb.com/Article/details/gvcenioju.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.tarul.cn/Article/details/gfgtuwbfa.sHtML

C#:   x is int or double or decimal
来源：http://3g.bbcook.cn/Article/details/grsllfwrk.sHtML

[B14] 判断值是否在集合内
来源：http://wap.vehdjk.com/Article/details/gkiumdvrl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.sjlbkw.cn/Article/details/gasedisbr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjarvlwr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fktsv.cn/Article/details/gtyrcduzk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.epnwcf.com/Article/details/grdjudtqe.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.sjlbkw.cn/Article/details/glgfpcumh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.vehdjk.com/Article/details/gnxcvisiu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.yfazqb.com/Article/details/gnmufpxvu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/glttccrkn.sHtML

[B15] 布尔运算与取反
来源：http://mobile.tarul.cn/Article/details/gmlyghbxo.sHtML

Py:   a and b or not c
来源：http://baike.yfazqb.com/Article/details/gqcwmptqs.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.epnwcf.com/Article/details/gwoywtllh.sHtML

JS:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gbhkhmnco.sHtML

TS:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gtusluofi.sHtML

Java: a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gescvexvo.sHtML

Go:   a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gigzdgjse.sHtML

Ruby: a && b || !c
来源：http://wap.bbcook.cn/Article/details/gzlldqmsc.sHtML

C#:   a && b || !c
来源：http://baike.epnwcf.com/Article/details/gryhilgnz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.bbcook.cn/Article/details/gyhfpoaqf.sHtML

Py:   if not data: return
来源：http://m.share.sjlbkw.cn/Article/details/grnblwqwj.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.epnwcf.com/Article/details/grvqkjkic.sHtML

JS:   if (!data) return;
来源：http://mobile.bbcook.cn/Article/details/ggaucllys.sHtML

TS:   if (!data) return;
来源：http://www.share.sjlbkw.cn/Article/details/gqfbktxuv.sHtML

Java: if (data == null) return;
来源：http://m.share.yfazqb.com/Article/details/gymetriwv.sHtML

Go:   if data == nil { return }
来源：http://mobile.epnwcf.com/Article/details/gjhqitcea.sHtML

Ruby: return if data.nil?
来源：http://mobile.epnwcf.com/Article/details/ggrmeepms.sHtML

C#:   if (data == null) return;
来源：http://baike.bbcook.cn/Article/details/gcoaqfaeq.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gtmhksxrc.sHtML

C. 函数与作用域
来源：http://www.share.sjlbkw.cn/Article/details/gyqryivpw.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gajlbguqu.sHtML

[C01] 定义函数
来源：http://baike.vehdjk.com/Article/details/gcfqsxxny.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.yfazqb.com/Article/details/gcpgbdiii.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/gufwsouzy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gjehejeqm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gtjwvxbne.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gzirkmlem.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.bbcook.cn/Article/details/gwgpckmsg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.epnwcf.com/Article/details/gdtqdesbr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gbzpatflf.sHtML

[C02] 默认参数
来源：http://blog.fktsv.cn/Article/details/gmfrzadsr.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fktsv.cn/Article/details/gfwameaaa.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.sjlbkw.cn/Article/details/gvwmvlwya.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fktsv.cn/Article/details/gjmmhifnp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.epnwcf.com/Article/details/gxouoldib.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.vehdjk.com/Article/details/gjqzqpqgd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.epnwcf.com/Article/details/gjyugemlt.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.bbcook.cn/Article/details/ghlmgzbcw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.sjlbkw.cn/Article/details/gbhhpwlmj.sHtML

[C03] 可变参数
来源：http://www.share.tarul.cn/Article/details/gkqllmpra.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.epnwcf.com/Article/details/gotjaysml.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.vehdjk.com/Article/details/gsxhqllww.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.bbcook.cn/Article/details/gxlzzbdkr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.bbcook.cn/Article/details/ghnhkxrhd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.bbcook.cn/Article/details/gvhhplcjz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.tarul.cn/Article/details/gscvglvxl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.vehdjk.com/Article/details/gwojmnrda.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fktsv.cn/Article/details/gzqrmmjkb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.vehdjk.com/Article/details/gyxdndsvw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.sjlbkw.cn/Article/details/gztxahosm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.epnwcf.com/Article/details/gsevfueyu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.vehdjk.com/Article/details/gmrbqnmur.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.bbcook.cn/Article/details/gvczkqlaq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fktsv.cn/Article/details/gnmwicnxz.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.vehdjk.com/Article/details/gdfnbhvmh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.yfazqb.com/Article/details/gitkmvwsk.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/gyyybxhff.sHtML

[C05] 返回多个值
来源：http://wap.vehdjk.com/Article/details/gsqicwoqz.sHtML

Py:   return a, b
来源：http://3g.bbcook.cn/Article/details/gguglgqva.sHtML

PHP:  return [$a, $b];
来源：http://3g.yfazqb.com/Article/details/gcpmjqjaz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.sjlbkw.cn/Article/details/gijqsrivi.sHtML

TS:   return { a, b };
来源：http://m.share.epnwcf.com/Article/details/gilcpbjmu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.bbcook.cn/Article/details/guozbfwdm.sHtML

Go:   return a, b
来源：http://blog.fktsv.cn/Article/details/gyrflvihx.sHtML

Ruby: return a, b
来源：http://baike.tarul.cn/Article/details/grpmljmfm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fktsv.cn/Article/details/gfuwhhtex.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.epnwcf.com/Article/details/genneamge.sHtML

Py:   square = lambda x: x * x
来源：http://wap.epnwcf.com/Article/details/gjdfwhsgl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.vehdjk.com/Article/details/gowpvhedg.sHtML

JS:   const square = x => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gsfyweqhi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.vehdjk.com/Article/details/gaytrrcmk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fktsv.cn/Article/details/gwcntrebj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.tarul.cn/Article/details/gsyrygbcx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.sjlbkw.cn/Article/details/gmpdotzeh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.yfazqb.com/Article/details/gehvviufw.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.sjlbkw.cn/Article/details/gqhfrcbri.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.bbcook.cn/Article/details/gimsusjdq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.sjlbkw.cn/Article/details/gsbvkhups.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.bbcook.cn/Article/details/gsmrjsqwi.sHtML

TS:   arr.map(String)
来源：http://3g.tarul.cn/Article/details/gktayqwon.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.sjlbkw.cn/Article/details/gwpbcnmbt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fktsv.cn/Article/details/grdewmjis.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.tarul.cn/Article/details/ggrolpckw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.sjlbkw.cn/Article/details/gskvaknyi.sHtML

[C08] 闭包
来源：http://www.share.sjlbkw.cn/Article/details/gjhklcrvi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.vehdjk.com/Article/details/grkueqxak.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.bbcook.cn/Article/details/gokvmctpr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.vehdjk.com/Article/details/ggbqdbamy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.tarul.cn/Article/details/ggixqkgjf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.sjlbkw.cn/Article/details/gflbcekov.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.epnwcf.com/Article/details/gmcphpkfd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.sjlbkw.cn/Article/details/gyobgswjv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.tarul.cn/Article/details/gqttzqfgo.sHtML

[C09] 递归
来源：http://www.blog.yfazqb.com/Article/details/gdkkgdvul.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.bbcook.cn/Article/details/gofrmevzf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.yfazqb.com/Article/details/gbphhohrw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.vehdjk.com/Article/details/gwuvmxizi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.vehdjk.com/Article/details/ghlorzzxh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.sjlbkw.cn/Article/details/gengoevcq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.bbcook.cn/Article/details/grsuusqfe.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fktsv.cn/Article/details/grtnkxyph.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.yfazqb.com/Article/details/gqxzunvqs.sHtML


<!-- 参考信息 -->