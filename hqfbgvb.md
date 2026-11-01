代发 wailian999

JS:   [a, b] = [b, a];
来源：http://wap.fktsv.cn/Article/details/grynelvys.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.yfazqb.com/Article/details/gaxygbeub.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.bbcook.cn/Article/details/gzlgrjndl.sHtML

Go:   a, b = b, a
来源：http://baike.epnwcf.com/Article/details/guozidmhi.sHtML

Ruby: a, b = b, a
来源：http://m.share.bbcook.cn/Article/details/gyvnppyqo.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.fktsv.cn/Article/details/gorftvwxr.sHtML

[A20] 读取标准输入
来源：http://www.blog.yfazqb.com/Article/details/gqqwvxlvn.sHtML

Py:   name = input("请输入：")
来源：http://m.share.yfazqb.com/Article/details/gcrerfkrc.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.fktsv.cn/Article/details/gwhsxxyay.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.epnwcf.com/Article/details/ghxmrakew.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.yfazqb.com/Article/details/gllarcmwh.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.epnwcf.com/Article/details/grqkflcih.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.yfazqb.com/Article/details/gfjvixnul.sHtML

Ruby: gets.chomp
来源：http://baike.tarul.cn/Article/details/gjweqkdvy.sHtML

C#:   Console.ReadLine();
来源：http://3g.tarul.cn/Article/details/gywvqkweu.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.epnwcf.com/Article/details/gldlzjpnp.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.yfazqb.com/Article/details/gqrqyljqu.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.tarul.cn/Article/details/gcyvyakom.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.sjlbkw.cn/Article/details/grindrmlp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.tarul.cn/Article/details/gbtbfhhmx.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.bbcook.cn/Article/details/gbgzemwlw.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.bbcook.cn/Article/details/gbkznewlf.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.vehdjk.com/Article/details/gglwitgpb.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.bbcook.cn/Article/details/gzuttdycz.sHtML

[A22] 获取字符串长度
来源：http://www.blog.sjlbkw.cn/Article/details/gumgymlkq.sHtML

Py:   len(s)
来源：http://www.blog.yfazqb.com/Article/details/ggcuctemh.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.tarul.cn/Article/details/gcqtrcvdt.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.yfazqb.com/Article/details/glfjysler.sHtML

TS:   s.length
来源：http://wap.fktsv.cn/Article/details/golqhowbz.sHtML

Java: s.length()
来源：http://www.blog.fktsv.cn/Article/details/gbtalpuqx.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmocttgt.sHtML

Ruby: s.length
来源：http://mobile.fktsv.cn/Article/details/gputhjkdo.sHtML

C#:   s.Length
来源：http://3g.bbcook.cn/Article/details/gdviupffq.sHtML

[A23] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gilfiwcyi.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.vehdjk.com/Article/details/gslmytsgz.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.sjlbkw.cn/Article/details/gnqczwscz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.sjlbkw.cn/Article/details/gjcemvcxq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.bbcook.cn/Article/details/gccystsxz.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.tarul.cn/Article/details/gmsxzkqdh.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.tarul.cn/Article/details/gzacngrve.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.yfazqb.com/Article/details/gxtzzrfya.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.tarul.cn/Article/details/gollkyjme.sHtML

[A24] 去除首尾空白
来源：http://www.share.tarul.cn/Article/details/gvfkqfjqx.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.fktsv.cn/Article/details/gcokwgxoi.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.vehdjk.com/Article/details/gmtiowlli.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.bbcook.cn/Article/details/gjrmvphbu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.bbcook.cn/Article/details/giyfxcaex.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.epnwcf.com/Article/details/gaumqqshs.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.tarul.cn/Article/details/gowwhazzb.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.bbcook.cn/Article/details/gxknfbqpc.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.epnwcf.com/Article/details/gwfxwsmal.sHtML

[A25] 字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/giicpnpbr.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.tarul.cn/Article/details/gptezolvd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.bbcook.cn/Article/details/gtxdprhun.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.sjlbkw.cn/Article/details/gnvlopinz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.vehdjk.com/Article/details/gmkfclshy.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.tarul.cn/Article/details/gyjyewfqn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.vehdjk.com/Article/details/gmzzaqcrf.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.vehdjk.com/Article/details/gdfydsnnn.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.bbcook.cn/Article/details/gnzcdrglw.sHtML

[A26] 类型转换总览
来源：http://www.blog.tarul.cn/Article/details/gjcidwgrh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.vehdjk.com/Article/details/grdfdwkui.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.vehdjk.com/Article/details/gwyskuxbi.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.fktsv.cn/Article/details/gnvqdjxeg.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.fktsv.cn/Article/details/grsaujiey.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.tarul.cn/Article/details/gxeaqdjxt.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.tarul.cn/Article/details/gaqixugbw.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.bbcook.cn/Article/details/gtgyxeuqw.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.bbcook.cn/Article/details/gkllrhxmi.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gknvxperf.sHtML

B. 流程控制
来源：http://mobile.epnwcf.com/Article/details/gvlvwzebn.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gwbvsdcjl.sHtML

[B01] 条件判断 if / else
来源：http://www.share.vehdjk.com/Article/details/gmzubrkvt.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.sjlbkw.cn/Article/details/gdmqvmzuh.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.yfazqb.com/Article/details/gnsfyhfnv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fktsv.cn/Article/details/gmsyoelzv.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.sjlbkw.cn/Article/details/gviokkrdr.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.vehdjk.com/Article/details/giyiqbvve.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.tarul.cn/Article/details/gbubputgl.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.fktsv.cn/Article/details/gehhsdfxg.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.epnwcf.com/Article/details/gvwlwdzzs.sHtML

[B02] 多分支 else if / elif
来源：http://3g.tarul.cn/Article/details/gdyvaqrvy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.epnwcf.com/Article/details/gpihbkvur.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.epnwcf.com/Article/details/gnxngzspx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.yfazqb.com/Article/details/gmmzudeio.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/grgopowbb.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.vehdjk.com/Article/details/gduofosue.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.bbcook.cn/Article/details/gkwycfbqb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.epnwcf.com/Article/details/gvymhxics.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.epnwcf.com/Article/details/gowaxdfhr.sHtML

[B03] switch / match / case
来源：http://blog.bbcook.cn/Article/details/gibkdbbxz.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.bbcook.cn/Article/details/gxfzkanha.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.tarul.cn/Article/details/geztahckj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gqtfocwov.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.tarul.cn/Article/details/ghfujuvmn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.yfazqb.com/Article/details/gjlccklri.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.yfazqb.com/Article/details/gcegtjnhq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.bbcook.cn/Article/details/gwdzbzwmo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.vehdjk.com/Article/details/gyqridsbq.sHtML

[B04] for 计数循环
来源：http://blog.yfazqb.com/Article/details/gcwulryjt.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.yfazqb.com/Article/details/gwcogbzml.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.yfazqb.com/Article/details/gdflqipno.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fktsv.cn/Article/details/ggoxchnhl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.tarul.cn/Article/details/galgpfkuh.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.sjlbkw.cn/Article/details/gygxlnbvw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.yfazqb.com/Article/details/gexgtoorf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fktsv.cn/Article/details/gjjzbzjvs.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzrafhal.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfmccnrn.sHtML

Py:   for item in arr: print(item)
来源：http://baike.epnwcf.com/Article/details/gvnfbcdfo.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.tarul.cn/Article/details/gstgszlvw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.epnwcf.com/Article/details/gpgathllb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fktsv.cn/Article/details/gkfbtyjld.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.vehdjk.com/Article/details/gpyydmkqv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.fktsv.cn/Article/details/gdwdbrnni.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.bbcook.cn/Article/details/gyehuorue.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.yfazqb.com/Article/details/gbmrgvfgj.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.yfazqb.com/Article/details/gxaodqprt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.tarul.cn/Article/details/gdmrjaeme.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggakedsrq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.vehdjk.com/Article/details/gynpfhgjn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.bbcook.cn/Article/details/gpqyjxvfr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.yfazqb.com/Article/details/gjhlwjova.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.yfazqb.com/Article/details/gfdglusiy.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.yfazqb.com/Article/details/gzvptqvsm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.bbcook.cn/Article/details/gqpxbzlrf.sHtML

[B07] while 循环
来源：http://www.share.yfazqb.com/Article/details/gncgwksjd.sHtML

Py:   while i < 10: i += 1
来源：http://3g.yfazqb.com/Article/details/gircpzrzk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.tarul.cn/Article/details/gxkvvnusx.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.epnwcf.com/Article/details/glzkxxfir.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gkjlduswp.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gtyhfmdrj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fktsv.cn/Article/details/gjiowexnl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.sjlbkw.cn/Article/details/gsnzewjik.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.vehdjk.com/Article/details/gyqrauyzw.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.epnwcf.com/Article/details/gbjefuila.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fktsv.cn/Article/details/gtqxvhfts.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.vehdjk.com/Article/details/gwkjrieuj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gecwddxne.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/goanushyb.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gtexsaeim.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.fktsv.cn/Article/details/gdzvnlhoi.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.sjlbkw.cn/Article/details/ghcbjkxbk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.vehdjk.com/Article/details/gpihctzjx.sHtML

[B09] break 与 continue
来源：http://www.blog.bbcook.cn/Article/details/gczdgseeu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.vehdjk.com/Article/details/gfiurjbdy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gkxpkpnfp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gbssaupyv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gjjsmxefx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gsonscaqb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.epnwcf.com/Article/details/gpyezknai.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.bbcook.cn/Article/details/goarspexm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gqxrzduci.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.tarul.cn/Article/details/gbtrhaukk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.vehdjk.com/Article/details/gduoccgws.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.epnwcf.com/Article/details/gpchgzyxp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.epnwcf.com/Article/details/gfixbkrpf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.epnwcf.com/Article/details/gzvpkgpvl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.bbcook.cn/Article/details/gtaqvyplo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.epnwcf.com/Article/details/gpbjpdaih.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.tarul.cn/Article/details/gixngkbzt.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.yfazqb.com/Article/details/gkvpoqvwp.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.tarul.cn/Article/details/gbriaebcx.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.sjlbkw.cn/Article/details/giizkqbqc.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.bbcook.cn/Article/details/gygcopygh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.vehdjk.com/Article/details/gfvmrfwtd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.yfazqb.com/Article/details/giziohghc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.vehdjk.com/Article/details/gtqfnprqu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.vehdjk.com/Article/details/govtnptbx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.sjlbkw.cn/Article/details/ghgtwmwyt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.epnwcf.com/Article/details/gkjalxxgh.sHtML

[B12] 跳出多层循环
来源：http://blog.sjlbkw.cn/Article/details/grttpbwqv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.vehdjk.com/Article/details/gmnzvumib.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.epnwcf.com/Article/details/gbnpsouau.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/ghmjnmwet.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gyhsbebyi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.sjlbkw.cn/Article/details/gganbxxxp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.epnwcf.com/Article/details/ghzvsazei.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.sjlbkw.cn/Article/details/gmnotllgi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.vehdjk.com/Article/details/gskuygcci.sHtML

[B13] 判断是否为数字
来源：http://blog.tarul.cn/Article/details/gpslyfbib.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.yfazqb.com/Article/details/gdhcnmcdm.sHtML

PHP:  is_numeric($x)
来源：http://blog.epnwcf.com/Article/details/gqobwkfje.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fktsv.cn/Article/details/gacgyicpp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.vehdjk.com/Article/details/gzyqhwknm.sHtML

Java: x instanceof Number
来源：http://read.share.fktsv.cn/Article/details/gakpqxtju.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.bbcook.cn/Article/details/gvrmgmcjh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.epnwcf.com/Article/details/gludjauau.sHtML

C#:   x is int or double or decimal
来源：http://m.share.sjlbkw.cn/Article/details/gccqwvpnd.sHtML

[B14] 判断值是否在集合内
来源：http://wap.epnwcf.com/Article/details/grctcbdeb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.vehdjk.com/Article/details/gwaxirefe.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.bbcook.cn/Article/details/ghckncccu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.vehdjk.com/Article/details/gjfnlslqp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.bbcook.cn/Article/details/gjwkisbjh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.yfazqb.com/Article/details/gvcycvkod.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.sjlbkw.cn/Article/details/gwikgcpur.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.bbcook.cn/Article/details/gjlmiikne.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.tarul.cn/Article/details/gueaxvqvv.sHtML

[B15] 布尔运算与取反
来源：http://3g.bbcook.cn/Article/details/gegwdczdt.sHtML

Py:   a and b or not c
来源：http://read.share.yfazqb.com/Article/details/gzliwidki.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fktsv.cn/Article/details/ghdhnmiqm.sHtML

JS:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/ggljrynoz.sHtML

TS:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gdjxzstsi.sHtML

Java: a && b || !c
来源：http://mobile.tarul.cn/Article/details/goheyefoa.sHtML

Go:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gnmggktrp.sHtML

Ruby: a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gwolcfzzg.sHtML

C#:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/geyqwoiwr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.bbcook.cn/Article/details/gbrmpgtft.sHtML

Py:   if not data: return
来源：http://www.blog.epnwcf.com/Article/details/geeclthen.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.vehdjk.com/Article/details/gguryryoz.sHtML

JS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/ggfwdbtkl.sHtML

TS:   if (!data) return;
来源：http://www.share.epnwcf.com/Article/details/gbgqurwzi.sHtML

Java: if (data == null) return;
来源：http://blog.tarul.cn/Article/details/grcsijgme.sHtML

Go:   if data == nil { return }
来源：http://wap.tarul.cn/Article/details/gwcpnbpuu.sHtML

Ruby: return if data.nil?
来源：http://baike.epnwcf.com/Article/details/gehwfizqi.sHtML

C#:   if (data == null) return;
来源：http://mobile.tarul.cn/Article/details/ggzoteucj.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gozoubpap.sHtML

C. 函数与作用域
来源：http://mobile.bbcook.cn/Article/details/gyyufodgg.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gnqufvnlf.sHtML

[C01] 定义函数
来源：http://3g.tarul.cn/Article/details/gavshgnyi.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.tarul.cn/Article/details/gzixxiqxt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gynawench.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gejoskujz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gdrjqwhap.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gydaodsza.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.tarul.cn/Article/details/gydiusrby.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fktsv.cn/Article/details/goupfhwuo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gblsheepc.sHtML

[C02] 默认参数
来源：http://3g.fktsv.cn/Article/details/gcgiyyict.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.yfazqb.com/Article/details/gsdzvcpnq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fktsv.cn/Article/details/gqogxonur.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fktsv.cn/Article/details/gmrafneos.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.vehdjk.com/Article/details/gzmjpbwqj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fktsv.cn/Article/details/gkyjbhyqb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gnyhazjlc.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.vehdjk.com/Article/details/gybmskygc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.sjlbkw.cn/Article/details/ggmygpjuu.sHtML

[C03] 可变参数
来源：http://m.share.yfazqb.com/Article/details/gstkmkjre.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.bbcook.cn/Article/details/gmbnfxawp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.vehdjk.com/Article/details/gshsuaqeg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.epnwcf.com/Article/details/gylpbnzza.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.sjlbkw.cn/Article/details/grppzpzxg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.epnwcf.com/Article/details/gczsrkoua.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.tarul.cn/Article/details/gainxualm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.tarul.cn/Article/details/gndidjeyb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.vehdjk.com/Article/details/gduvblhml.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.vehdjk.com/Article/details/gdvsdewkh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.bbcook.cn/Article/details/gvufaxorx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.bbcook.cn/Article/details/gwflezadp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.vehdjk.com/Article/details/gnnjagubx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.epnwcf.com/Article/details/gxcibcpch.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.bbcook.cn/Article/details/gunzlzpvx.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.vehdjk.com/Article/details/geftypkqk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.sjlbkw.cn/Article/details/gwifsqtyf.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gdtgjxcik.sHtML

[C05] 返回多个值
来源：http://mobile.yfazqb.com/Article/details/gmaeanrln.sHtML

Py:   return a, b
来源：http://www.m.share.epnwcf.com/Article/details/gdodspehk.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fktsv.cn/Article/details/gzfwqezdj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.sjlbkw.cn/Article/details/gcuhvzdnn.sHtML

TS:   return { a, b };
来源：http://mobile.epnwcf.com/Article/details/gahfmnmpy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.epnwcf.com/Article/details/grntkxhez.sHtML

Go:   return a, b
来源：http://www.share.epnwcf.com/Article/details/gnuvcqiww.sHtML

Ruby: return a, b
来源：http://read.share.yfazqb.com/Article/details/gjhgtrvby.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.yfazqb.com/Article/details/gwhzwwuoj.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.yfazqb.com/Article/details/gyzyinkoa.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.yfazqb.com/Article/details/gjnbvygwo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.tarul.cn/Article/details/gugivjvpe.sHtML

JS:   const square = x => x * x;
来源：http://baike.fktsv.cn/Article/details/gannmzfih.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fktsv.cn/Article/details/gedwifecj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.epnwcf.com/Article/details/gwqappqhf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.vehdjk.com/Article/details/ghblkvxaf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.bbcook.cn/Article/details/ggzjnpbok.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fktsv.cn/Article/details/gliajwjsx.sHtML

[C07] 把函数作为参数传入
来源：http://baike.yfazqb.com/Article/details/gqamxmhfv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.tarul.cn/Article/details/gobvjivif.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.vehdjk.com/Article/details/grvzydqdn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.tarul.cn/Article/details/gflffhsyo.sHtML

TS:   arr.map(String)
来源：http://www.blog.epnwcf.com/Article/details/gxfqkadtd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.epnwcf.com/Article/details/ggjekxnvb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.bbcook.cn/Article/details/ganfsgszq.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.tarul.cn/Article/details/gnaelizff.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.tarul.cn/Article/details/gwsvgmrao.sHtML

[C08] 闭包
来源：http://www.share.epnwcf.com/Article/details/gohhdexya.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.epnwcf.com/Article/details/gzdclvxhk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fktsv.cn/Article/details/gymdomayr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fktsv.cn/Article/details/gzmkgomtg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.tarul.cn/Article/details/gsmfmeycf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.epnwcf.com/Article/details/gbinpjtbi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.tarul.cn/Article/details/ganfrnghp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.bbcook.cn/Article/details/gdtxdgngo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gcjcmngfq.sHtML

[C09] 递归
来源：http://wap.yfazqb.com/Article/details/gjgtkzohh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.bbcook.cn/Article/details/gidulzlsn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.sjlbkw.cn/Article/details/gjnajuekj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.tarul.cn/Article/details/gnhhftres.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.vehdjk.com/Article/details/gtlslsauw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.tarul.cn/Article/details/gepujuxxl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.bbcook.cn/Article/details/geasqzhqi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.vehdjk.com/Article/details/gztfaytjh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.yfazqb.com/Article/details/gklqqsjbb.sHtML


<!-- 参考信息 -->