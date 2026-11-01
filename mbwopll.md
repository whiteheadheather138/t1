代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fktsv.cn/Article/details/gawzoxrro.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fktsv.cn/Article/details/gdgdiqszo.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.tarul.cn/Article/details/gpkkclwza.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.vehdjk.com/Article/details/gzfrdcpqz.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.fktsv.cn/Article/details/gsyoojkph.sHtML

[A19] 交换两个变量
来源：http://read.share.yfazqb.com/Article/details/gjgjtsfjd.sHtML

Py:   a, b = b, a
来源：http://www.share.sjlbkw.cn/Article/details/gsnyehnlh.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.vehdjk.com/Article/details/gservcajx.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.vehdjk.com/Article/details/gjranmzyq.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.fktsv.cn/Article/details/gnafwetuy.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.fktsv.cn/Article/details/gwczxgzmz.sHtML

Go:   a, b = b, a
来源：http://3g.epnwcf.com/Article/details/gavksvwhi.sHtML

Ruby: a, b = b, a
来源：http://wap.sjlbkw.cn/Article/details/gogxluvsz.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.tarul.cn/Article/details/gspqsuisp.sHtML

[A20] 读取标准输入
来源：http://m.share.fktsv.cn/Article/details/gxisrljxb.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.epnwcf.com/Article/details/gsdfgpaxk.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.yfazqb.com/Article/details/gzeqwdazo.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.yfazqb.com/Article/details/grqwsecpz.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.tarul.cn/Article/details/gncuiusrd.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.sjlbkw.cn/Article/details/gvjihdlop.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.yfazqb.com/Article/details/gyjryqezc.sHtML

Ruby: gets.chomp
来源：http://blog.epnwcf.com/Article/details/ggmmdblro.sHtML

C#:   Console.ReadLine();
来源：http://wap.bbcook.cn/Article/details/gyiitntrk.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.fktsv.cn/Article/details/gdwmgbosb.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.sjlbkw.cn/Article/details/gwxrigdor.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.sjlbkw.cn/Article/details/gahofpewl.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.vehdjk.com/Article/details/gvuddhswh.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.bbcook.cn/Article/details/gbnsurwjc.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gowwfcamq.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.sjlbkw.cn/Article/details/gjozofdku.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.tarul.cn/Article/details/greymcnmk.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.sjlbkw.cn/Article/details/gucwdkpja.sHtML

[A22] 获取字符串长度
来源：http://m.share.vehdjk.com/Article/details/gyiiccrcl.sHtML

Py:   len(s)
来源：http://wap.yfazqb.com/Article/details/gyjwkwfys.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.fktsv.cn/Article/details/gxnhfhrzz.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.epnwcf.com/Article/details/gjipvpfwh.sHtML

TS:   s.length
来源：http://read.share.vehdjk.com/Article/details/grchmuzfd.sHtML

Java: s.length()
来源：http://blog.tarul.cn/Article/details/gwvpooodc.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.vehdjk.com/Article/details/gqwouqtdb.sHtML

Ruby: s.length
来源：http://read.share.yfazqb.com/Article/details/ghivgwbok.sHtML

C#:   s.Length
来源：http://blog.sjlbkw.cn/Article/details/grixykvzs.sHtML

[A23] 大小写转换
来源：http://read.share.tarul.cn/Article/details/gmuskhuic.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.fktsv.cn/Article/details/gnujliyhb.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.bbcook.cn/Article/details/gbmlkvnxx.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.epnwcf.com/Article/details/gjcitastx.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fktsv.cn/Article/details/gxpeoiabs.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.vehdjk.com/Article/details/gcfxpntiq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.tarul.cn/Article/details/gnrgpxolq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.fktsv.cn/Article/details/gfyplpevj.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.tarul.cn/Article/details/gvwzyhwmw.sHtML

[A24] 去除首尾空白
来源：http://www.share.yfazqb.com/Article/details/grshzudgx.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.yfazqb.com/Article/details/guvconknj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.vehdjk.com/Article/details/gmbwicsnl.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.yfazqb.com/Article/details/gnpygoveb.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.epnwcf.com/Article/details/ggsetqpbf.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.fktsv.cn/Article/details/gqaaslcsq.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.vehdjk.com/Article/details/gbehbgzfn.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.vehdjk.com/Article/details/gjojetzkq.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.vehdjk.com/Article/details/gsumdyhet.sHtML

[A25] 字符串比较
来源：http://www.blog.fktsv.cn/Article/details/gpuxenddl.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.fktsv.cn/Article/details/gljyxmatd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.tarul.cn/Article/details/ggemmrvls.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.bbcook.cn/Article/details/gekkifbzj.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.bbcook.cn/Article/details/glfgjzrrl.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.yfazqb.com/Article/details/gvqlyfqnt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.bbcook.cn/Article/details/gobniusqj.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.sjlbkw.cn/Article/details/gedoozoco.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.yfazqb.com/Article/details/ginuhyhlk.sHtML

[A26] 类型转换总览
来源：http://m.share.bbcook.cn/Article/details/gvhhvyggv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.epnwcf.com/Article/details/gacivgpkq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.tarul.cn/Article/details/gqeblnryk.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.fktsv.cn/Article/details/gbfsyygae.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.bbcook.cn/Article/details/gubbiduxb.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.tarul.cn/Article/details/gyhdycdrr.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.bbcook.cn/Article/details/glhhbltsx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.bbcook.cn/Article/details/gqxwtwyam.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.tarul.cn/Article/details/gompaqbek.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gsenkgpkj.sHtML

B. 流程控制
来源：http://www.share.bbcook.cn/Article/details/geencbjiu.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/grhfpsswq.sHtML

[B01] 条件判断 if / else
来源：http://3g.tarul.cn/Article/details/gvxtwkyyy.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.vehdjk.com/Article/details/gveqonjeb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.vehdjk.com/Article/details/gfceqjzrd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/ghmlogldl.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.vehdjk.com/Article/details/gzekpnayq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.bbcook.cn/Article/details/gwqcanvll.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.yfazqb.com/Article/details/gwqfoypee.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fktsv.cn/Article/details/gniqlmwtd.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gebnskzmv.sHtML

[B02] 多分支 else if / elif
来源：http://3g.tarul.cn/Article/details/gjivecexe.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.epnwcf.com/Article/details/gveuftfzk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.bbcook.cn/Article/details/gtpaszdee.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/gbriybdgg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/gkpcuzaaw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/ghhxyqqld.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.vehdjk.com/Article/details/gcddieeio.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.yfazqb.com/Article/details/gxrlzbdic.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/gomslwkdf.sHtML

[B03] switch / match / case
来源：http://www.blog.vehdjk.com/Article/details/gprgdknea.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.bbcook.cn/Article/details/gjxcakfnu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/gpruuldww.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.tarul.cn/Article/details/ghvowvjnf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.bbcook.cn/Article/details/gvsfndktw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/gsknlhmjc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.vehdjk.com/Article/details/gbulrakrt.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.epnwcf.com/Article/details/gakkukccj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fktsv.cn/Article/details/gbbigufyj.sHtML

[B04] for 计数循环
来源：http://read.share.yfazqb.com/Article/details/gryxgkzau.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.epnwcf.com/Article/details/gkwbqlypx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.yfazqb.com/Article/details/gnsgbobbo.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.epnwcf.com/Article/details/gdjsldawk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.epnwcf.com/Article/details/gmonhbdwo.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.yfazqb.com/Article/details/gwvvzzssf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.tarul.cn/Article/details/geaxalxsl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.tarul.cn/Article/details/gljjzbawk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fktsv.cn/Article/details/gtqvjjsfr.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.sjlbkw.cn/Article/details/gezzplplw.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.bbcook.cn/Article/details/ghixpflxa.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.yfazqb.com/Article/details/gxfouxtwn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.tarul.cn/Article/details/ggpjwcmxw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.sjlbkw.cn/Article/details/gqcrhjcdd.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.sjlbkw.cn/Article/details/guenqxbgi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.tarul.cn/Article/details/gnjqdukyq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.bbcook.cn/Article/details/gkaykeolj.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.bbcook.cn/Article/details/ghhdqqtha.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.epnwcf.com/Article/details/gocuwwwxu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.epnwcf.com/Article/details/gdauazjug.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.bbcook.cn/Article/details/gtrouwhei.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.bbcook.cn/Article/details/grhepymzp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.tarul.cn/Article/details/gbfqcfptz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.tarul.cn/Article/details/ghqhfbjje.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.sjlbkw.cn/Article/details/gkccohorv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.vehdjk.com/Article/details/gdklfsgel.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.vehdjk.com/Article/details/gmxoeosih.sHtML

[B07] while 循环
来源：http://www.blog.epnwcf.com/Article/details/gfsnfsore.sHtML

Py:   while i < 10: i += 1
来源：http://wap.sjlbkw.cn/Article/details/gftgqmjfi.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.sjlbkw.cn/Article/details/gazreiuct.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/gglclqdik.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzxckamwj.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/garoeurdy.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.yfazqb.com/Article/details/gfnzhqauf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.vehdjk.com/Article/details/guhwtilal.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/gtslrzjqi.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.vehdjk.com/Article/details/gglrljujg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.vehdjk.com/Article/details/gvtlhsmiu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.tarul.cn/Article/details/gtswznvhx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/gwxzbtyod.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.bbcook.cn/Article/details/gbqympxoe.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fktsv.cn/Article/details/ggtfumvoo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.yfazqb.com/Article/details/gmosaaqfe.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.vehdjk.com/Article/details/ggnziqdaq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gzfhkayao.sHtML

[B09] break 与 continue
来源：http://read.share.yfazqb.com/Article/details/gwopyevhe.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.bbcook.cn/Article/details/gxycmbjoi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gfkwifdok.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/gmnlcrsez.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gtufammju.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gavitqmkm.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.vehdjk.com/Article/details/gbumbllip.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.vehdjk.com/Article/details/gvivldizi.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gsrbgogjf.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.sjlbkw.cn/Article/details/gephtfxfp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.vehdjk.com/Article/details/gfzdscekz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.yfazqb.com/Article/details/gbxqctujr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.epnwcf.com/Article/details/gbakmygke.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.yfazqb.com/Article/details/gqwpbjdly.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.yfazqb.com/Article/details/gcjewxywv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.yfazqb.com/Article/details/gigplzezi.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.bbcook.cn/Article/details/gybvqbhep.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.yfazqb.com/Article/details/gvsdujpfs.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.yfazqb.com/Article/details/glspeofsg.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.tarul.cn/Article/details/gxnbtmdig.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.vehdjk.com/Article/details/gwnioozvk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.tarul.cn/Article/details/gsupqeoqg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.yfazqb.com/Article/details/gbwmsqyxk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.vehdjk.com/Article/details/ginppacbr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.bbcook.cn/Article/details/gkwzbidsx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.tarul.cn/Article/details/gpoojpydx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fktsv.cn/Article/details/gvpzkxbxe.sHtML

[B12] 跳出多层循环
来源：http://wap.tarul.cn/Article/details/gwsupofzm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fktsv.cn/Article/details/gvpljbign.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fktsv.cn/Article/details/gyuxicwet.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.yfazqb.com/Article/details/gcskckcth.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/gjpqgbire.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.vehdjk.com/Article/details/gcczywhce.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.yfazqb.com/Article/details/gkhtglmhu.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.epnwcf.com/Article/details/gfumyoese.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.yfazqb.com/Article/details/gpgpudeld.sHtML

[B13] 判断是否为数字
来源：http://blog.epnwcf.com/Article/details/gwmoorunz.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.yfazqb.com/Article/details/gslycdtvh.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.bbcook.cn/Article/details/gqhsegyby.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.sjlbkw.cn/Article/details/gklrsxbwd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.tarul.cn/Article/details/gedwmmxqs.sHtML

Java: x instanceof Number
来源：http://www.blog.fktsv.cn/Article/details/gsdrcqjsh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.tarul.cn/Article/details/gkdfpdgoz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.epnwcf.com/Article/details/gbysgadbs.sHtML

C#:   x is int or double or decimal
来源：http://m.share.vehdjk.com/Article/details/gjhrgxucl.sHtML

[B14] 判断值是否在集合内
来源：http://blog.epnwcf.com/Article/details/gyilmztns.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.tarul.cn/Article/details/gieeewqkt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.yfazqb.com/Article/details/gsotrgphm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.vehdjk.com/Article/details/gpcdgwgei.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/gdhinjinc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.tarul.cn/Article/details/gluwtjisf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.yfazqb.com/Article/details/gqzpncvrb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.yfazqb.com/Article/details/gaynhnwyd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.vehdjk.com/Article/details/gpjeaxuda.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fktsv.cn/Article/details/goaywngbn.sHtML

Py:   a and b or not c
来源：http://wap.vehdjk.com/Article/details/gldfxoynt.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.epnwcf.com/Article/details/ginfteudc.sHtML

JS:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/gckizsuvx.sHtML

TS:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gnohtvkkf.sHtML

Java: a && b || !c
来源：http://wap.yfazqb.com/Article/details/gmlrjygib.sHtML

Go:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/grfwgpfqy.sHtML

Ruby: a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gkfwfnqxk.sHtML

C#:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gzrowcjdw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.yfazqb.com/Article/details/gahbvatkz.sHtML

Py:   if not data: return
来源：http://www.share.bbcook.cn/Article/details/gbfcauezr.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.yfazqb.com/Article/details/gnvxqhptg.sHtML

JS:   if (!data) return;
来源：http://wap.sjlbkw.cn/Article/details/gahuwbeod.sHtML

TS:   if (!data) return;
来源：http://mobile.bbcook.cn/Article/details/gqpsfnzii.sHtML

Java: if (data == null) return;
来源：http://blog.tarul.cn/Article/details/grgmysmrk.sHtML

Go:   if data == nil { return }
来源：http://read.share.vehdjk.com/Article/details/gjeodzzjc.sHtML

Ruby: return if data.nil?
来源：http://www.blog.bbcook.cn/Article/details/giwxcombb.sHtML

C#:   if (data == null) return;
来源：http://www.blog.bbcook.cn/Article/details/gbbzqdfsf.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gdzpqcbed.sHtML

C. 函数与作用域
来源：http://baike.vehdjk.com/Article/details/gitvdjaki.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gqxyytwor.sHtML

[C01] 定义函数
来源：http://www.m.share.fktsv.cn/Article/details/gakdpyxjm.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.epnwcf.com/Article/details/gugqjxwda.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gzmnxebfk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gstdydjvm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gebmffngr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/geduovesl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.bbcook.cn/Article/details/gpryisvmf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.bbcook.cn/Article/details/goqpyamkf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gsctrozkw.sHtML

[C02] 默认参数
来源：http://read.share.fktsv.cn/Article/details/gxdofqjrd.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.epnwcf.com/Article/details/gtijyinvs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.bbcook.cn/Article/details/ggidchboq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.epnwcf.com/Article/details/gfrlqqsil.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.vehdjk.com/Article/details/gzawbehfo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fktsv.cn/Article/details/gpqhkyxds.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.yfazqb.com/Article/details/gtaeigesc.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.vehdjk.com/Article/details/gpgrjndwn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.epnwcf.com/Article/details/guvwwzbhp.sHtML

[C03] 可变参数
来源：http://blog.bbcook.cn/Article/details/gqbplorct.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.vehdjk.com/Article/details/gvytgrnvw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fktsv.cn/Article/details/gvqlajqdd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.vehdjk.com/Article/details/grpvgbcha.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.sjlbkw.cn/Article/details/gaguvtgqf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.bbcook.cn/Article/details/gyzbxnvoy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.epnwcf.com/Article/details/gvlubxotx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.epnwcf.com/Article/details/girttwixv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.epnwcf.com/Article/details/gfyphdcdn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.tarul.cn/Article/details/gndnduinb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.bbcook.cn/Article/details/gkpfmyowy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.tarul.cn/Article/details/gvnxkfycq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.tarul.cn/Article/details/goolywtvt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.tarul.cn/Article/details/gemzifayk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.epnwcf.com/Article/details/gqbmmhjmq.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.epnwcf.com/Article/details/gzgitivpm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.sjlbkw.cn/Article/details/gdqojrdxz.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/gjqgnbvza.sHtML

[C05] 返回多个值
来源：http://www.blog.fktsv.cn/Article/details/gakvqgyji.sHtML

Py:   return a, b
来源：http://m.share.tarul.cn/Article/details/gpqpsmvtb.sHtML

PHP:  return [$a, $b];
来源：http://www.share.epnwcf.com/Article/details/gldaktmbg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.epnwcf.com/Article/details/gcqwmgofo.sHtML

TS:   return { a, b };
来源：http://baike.sjlbkw.cn/Article/details/gzikrthyu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.sjlbkw.cn/Article/details/gzlmkoyox.sHtML

Go:   return a, b
来源：http://m.share.tarul.cn/Article/details/guennwenb.sHtML

Ruby: return a, b
来源：http://baike.epnwcf.com/Article/details/gjffsbgnx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.bbcook.cn/Article/details/gzhbgjhny.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.tarul.cn/Article/details/gqhiysmvm.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.epnwcf.com/Article/details/gqoyyoyqx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.tarul.cn/Article/details/gckiqczgr.sHtML

JS:   const square = x => x * x;
来源：http://mobile.epnwcf.com/Article/details/gnlrzdqdw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.vehdjk.com/Article/details/gjefffayy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.vehdjk.com/Article/details/gvpijtrfz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnlbmozz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.tarul.cn/Article/details/grinqjwig.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.yfazqb.com/Article/details/guxaluirk.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.epnwcf.com/Article/details/gcuvorxjy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fktsv.cn/Article/details/ggwemksrp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.bbcook.cn/Article/details/giymcjtmt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.sjlbkw.cn/Article/details/gzyncrgay.sHtML

TS:   arr.map(String)
来源：http://wap.tarul.cn/Article/details/gwjlgbuee.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.yfazqb.com/Article/details/grwkgibnm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.sjlbkw.cn/Article/details/gpscjwlct.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fktsv.cn/Article/details/gusibiciv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fktsv.cn/Article/details/gfxpyzvaf.sHtML

[C08] 闭包
来源：http://www.blog.sjlbkw.cn/Article/details/gnxyfkxqi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.tarul.cn/Article/details/ghkeatomp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.bbcook.cn/Article/details/grdjznxis.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gfzxaswph.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/ggllhfxdl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.epnwcf.com/Article/details/gqsppgnyx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.yfazqb.com/Article/details/getgqvgzg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.yfazqb.com/Article/details/gttuwbbys.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/guqsbtvxg.sHtML

[C09] 递归
来源：http://baike.fktsv.cn/Article/details/gacgykooa.sHtML


<!-- 参考信息 -->