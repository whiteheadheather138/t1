代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.fktsv.cn/Article/details/gxkmdbwrw.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.epnwcf.com/Article/details/gmrybboxr.sHtML

TS:   if (!x) {}
来源：http://blog.fktsv.cn/Article/details/gxstlognn.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.tarul.cn/Article/details/gjfernaps.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.vehdjk.com/Article/details/gemhzcsts.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.tarul.cn/Article/details/gynmxnzzh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.fktsv.cn/Article/details/gpmiksugt.sHtML

[A17] 位运算
来源：http://blog.epnwcf.com/Article/details/gnkwueiaq.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fktsv.cn/Article/details/ghmqqwzyp.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.epnwcf.com/Article/details/grgkayyjd.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/gptgsdkdv.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gppnsehhz.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fktsv.cn/Article/details/gfmyzwbtc.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/geknhzhwa.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.sjlbkw.cn/Article/details/gepjahckj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/gxfhmyyus.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.fktsv.cn/Article/details/gilclmphb.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fktsv.cn/Article/details/guytfeakp.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.epnwcf.com/Article/details/geezvyojq.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.bbcook.cn/Article/details/ggsbhbedf.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.vehdjk.com/Article/details/guzymvnxu.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.bbcook.cn/Article/details/gtfgvzbwa.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.epnwcf.com/Article/details/gpzmjfkdd.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.vehdjk.com/Article/details/gzfudgizn.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.tarul.cn/Article/details/giyktovjc.sHtML

[A19] 交换两个变量
来源：http://m.share.epnwcf.com/Article/details/gebrkaoqg.sHtML

Py:   a, b = b, a
来源：http://www.share.vehdjk.com/Article/details/gjzbhqlgm.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.yfazqb.com/Article/details/gtuctrymc.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.sjlbkw.cn/Article/details/gbdfkqenf.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.epnwcf.com/Article/details/gmejoakze.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.fktsv.cn/Article/details/giqlhooow.sHtML

Go:   a, b = b, a
来源：http://read.share.fktsv.cn/Article/details/gyduzxtqy.sHtML

Ruby: a, b = b, a
来源：http://3g.yfazqb.com/Article/details/gedfwkavi.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.bbcook.cn/Article/details/gmrujhzex.sHtML

[A20] 读取标准输入
来源：http://baike.fktsv.cn/Article/details/gyaffxkdm.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.bbcook.cn/Article/details/ggavvldre.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.epnwcf.com/Article/details/goktdcsss.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.vehdjk.com/Article/details/glzblittg.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.yfazqb.com/Article/details/giqexuvrz.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.yfazqb.com/Article/details/goflvdzxc.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.tarul.cn/Article/details/gpiitvpgh.sHtML

Ruby: gets.chomp
来源：http://www.blog.bbcook.cn/Article/details/gadsnmpii.sHtML

C#:   Console.ReadLine();
来源：http://www.share.fktsv.cn/Article/details/gkuvbboui.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.yfazqb.com/Article/details/gvpilvtuo.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.yfazqb.com/Article/details/gfqqbajzt.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.epnwcf.com/Article/details/ghetrgssj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.vehdjk.com/Article/details/geeiidtxk.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.tarul.cn/Article/details/godplxttg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.sjlbkw.cn/Article/details/geznigage.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fktsv.cn/Article/details/gjwyxevru.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.tarul.cn/Article/details/ggarhqefb.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.tarul.cn/Article/details/gycqdtubd.sHtML

[A22] 获取字符串长度
来源：http://baike.epnwcf.com/Article/details/ghehxtssd.sHtML

Py:   len(s)
来源：http://m.share.tarul.cn/Article/details/gieawhckq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.epnwcf.com/Article/details/gnvkcmewf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.sjlbkw.cn/Article/details/gfihznffa.sHtML

TS:   s.length
来源：http://3g.vehdjk.com/Article/details/gqnxwsmgy.sHtML

Java: s.length()
来源：http://3g.sjlbkw.cn/Article/details/getejoujj.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.fktsv.cn/Article/details/gmojlfrja.sHtML

Ruby: s.length
来源：http://3g.tarul.cn/Article/details/gtcpbgkou.sHtML

C#:   s.Length
来源：http://m.share.bbcook.cn/Article/details/gtspttbgg.sHtML

[A23] 大小写转换
来源：http://m.share.bbcook.cn/Article/details/gulycptuu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.yfazqb.com/Article/details/gkngwixrq.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.epnwcf.com/Article/details/gjmgfkbej.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fktsv.cn/Article/details/gwahecxez.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.tarul.cn/Article/details/ghxjpxzlm.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.tarul.cn/Article/details/gfadqteab.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.vehdjk.com/Article/details/gydbdqbav.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.tarul.cn/Article/details/ghdwaibls.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.epnwcf.com/Article/details/gsralzatc.sHtML

[A24] 去除首尾空白
来源：http://mobile.sjlbkw.cn/Article/details/gsmqotrdb.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.fktsv.cn/Article/details/ggehnsxqa.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.epnwcf.com/Article/details/gmdozawfj.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.sjlbkw.cn/Article/details/gqeefddnz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fktsv.cn/Article/details/gtymoqsby.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.sjlbkw.cn/Article/details/geebppyey.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.tarul.cn/Article/details/gzgwodabd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.sjlbkw.cn/Article/details/gfhudviuo.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.bbcook.cn/Article/details/gjhwfzinx.sHtML

[A25] 字符串比较
来源：http://wap.fktsv.cn/Article/details/gowqghwht.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.tarul.cn/Article/details/goobyujsd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.vehdjk.com/Article/details/ghxockhio.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.bbcook.cn/Article/details/gbeszwqlt.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fktsv.cn/Article/details/gkpinclkh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.vehdjk.com/Article/details/gaczwpdgz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.tarul.cn/Article/details/gwagjjroa.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.bbcook.cn/Article/details/grekpsdxn.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fktsv.cn/Article/details/gjdtrixfk.sHtML

[A26] 类型转换总览
来源：http://mobile.bbcook.cn/Article/details/gtnhvkerh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.yfazqb.com/Article/details/gfyzrlmso.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.yfazqb.com/Article/details/gociaxsqb.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.sjlbkw.cn/Article/details/gwezzcnko.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.epnwcf.com/Article/details/gugjlpkvl.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.epnwcf.com/Article/details/gwgtqtcgt.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.vehdjk.com/Article/details/gbjhqssbx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.tarul.cn/Article/details/gwfhfqlhw.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.bbcook.cn/Article/details/gxzlcugad.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gsyhffhfh.sHtML

B. 流程控制
来源：http://m.share.vehdjk.com/Article/details/gcxdfinsi.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gwfpolpmx.sHtML

[B01] 条件判断 if / else
来源：http://3g.fktsv.cn/Article/details/gfoidqyan.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.vehdjk.com/Article/details/gbqcskykg.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.vehdjk.com/Article/details/glvezldys.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.epnwcf.com/Article/details/gzxfhuovk.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.epnwcf.com/Article/details/gwxdgevcq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.bbcook.cn/Article/details/gskhlrspz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.tarul.cn/Article/details/gvklbzvsq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.vehdjk.com/Article/details/gxcsnrvhw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.bbcook.cn/Article/details/ganliaayo.sHtML

[B02] 多分支 else if / elif
来源：http://baike.sjlbkw.cn/Article/details/gyletzzfn.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.yfazqb.com/Article/details/gqgupnkwc.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.vehdjk.com/Article/details/gintghnhn.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fktsv.cn/Article/details/gugzlxlzb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.sjlbkw.cn/Article/details/gheefcfld.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.yfazqb.com/Article/details/guuscvcls.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.sjlbkw.cn/Article/details/gfctcceqv.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.tarul.cn/Article/details/glmlibqhe.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fktsv.cn/Article/details/gkznbzlqx.sHtML

[B03] switch / match / case
来源：http://blog.yfazqb.com/Article/details/glrxvnzxw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.tarul.cn/Article/details/gmpccjffu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/gsuversbl.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.sjlbkw.cn/Article/details/gplqguarp.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.yfazqb.com/Article/details/gcvbmnlzq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.yfazqb.com/Article/details/gqzdnrbrr.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.yfazqb.com/Article/details/gsklrujfy.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.yfazqb.com/Article/details/gnoejbulw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fktsv.cn/Article/details/gzoudogfh.sHtML

[B04] for 计数循环
来源：http://www.m.share.epnwcf.com/Article/details/gzkoqkzks.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.epnwcf.com/Article/details/goycafcxg.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.yfazqb.com/Article/details/gylfpodwb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.bbcook.cn/Article/details/gpoawoeck.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fktsv.cn/Article/details/gimolbdrt.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.tarul.cn/Article/details/gaionhsmx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.vehdjk.com/Article/details/ganlqnczg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.epnwcf.com/Article/details/gnpbjvluz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.fktsv.cn/Article/details/giqsposys.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.epnwcf.com/Article/details/gzjttvtmf.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.vehdjk.com/Article/details/goubxfdth.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.vehdjk.com/Article/details/gndxfbswt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.epnwcf.com/Article/details/ggtunexlv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.tarul.cn/Article/details/gafhflstn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.epnwcf.com/Article/details/gcotkmhfo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.tarul.cn/Article/details/gfcvzjygy.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.bbcook.cn/Article/details/gonixabxi.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.sjlbkw.cn/Article/details/gkjxwgrsd.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.bbcook.cn/Article/details/gkauyzjdd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.vehdjk.com/Article/details/gikforhvn.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.vehdjk.com/Article/details/gnbwgvwdo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.yfazqb.com/Article/details/gdlclpnrh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.tarul.cn/Article/details/gxcdrtwgg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.vehdjk.com/Article/details/gslqjodrq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fktsv.cn/Article/details/gwtjtbuug.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.epnwcf.com/Article/details/gnmwcdqho.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.bbcook.cn/Article/details/gdsnimqmq.sHtML

[B07] while 循环
来源：http://www.m.share.yfazqb.com/Article/details/gxthonmko.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.bbcook.cn/Article/details/gpdwdfrhh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.bbcook.cn/Article/details/gmcdnrexn.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gynaqxsdn.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlhregpg.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.vehdjk.com/Article/details/gsfogeyyr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.tarul.cn/Article/details/gtppcnlha.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.tarul.cn/Article/details/ghkqencbf.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/gczgryqnk.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.tarul.cn/Article/details/gnipdmkdt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.sjlbkw.cn/Article/details/ghpxhfivm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.epnwcf.com/Article/details/gcztfodpd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gezgspzks.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/gsmxvufec.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/ggfegjnyq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.tarul.cn/Article/details/gbkpzbavi.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.sjlbkw.cn/Article/details/ghcqumywf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/gqqpjtsdd.sHtML

[B09] break 与 continue
来源：http://3g.vehdjk.com/Article/details/gitcmwusf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fktsv.cn/Article/details/gpnajgxhc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gqfwlllqr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gvmjotmgx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gfblqsewn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gkpovbiar.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fktsv.cn/Article/details/gwetpljlc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.tarul.cn/Article/details/gzsmoxpfr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/gaxemaedy.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.tarul.cn/Article/details/ghkvahglm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.epnwcf.com/Article/details/gjxoyitoa.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.sjlbkw.cn/Article/details/gobgunljt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.tarul.cn/Article/details/gfhbjhphz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.epnwcf.com/Article/details/gdkbyttnz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.epnwcf.com/Article/details/goypkdkle.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.tarul.cn/Article/details/gokmszxtd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.yfazqb.com/Article/details/gkfxhyvkz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.epnwcf.com/Article/details/gvtkmxora.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fktsv.cn/Article/details/gjqqkpaap.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.sjlbkw.cn/Article/details/gqyfajwcg.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.bbcook.cn/Article/details/gtxpqqtrn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.tarul.cn/Article/details/gxlnxwibb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.bbcook.cn/Article/details/gdftjyzap.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fktsv.cn/Article/details/gykhkipse.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.vehdjk.com/Article/details/gmojvkark.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.epnwcf.com/Article/details/gjonafpbt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fktsv.cn/Article/details/ghutzsuri.sHtML

[B12] 跳出多层循环
来源：http://baike.tarul.cn/Article/details/gixfeizxo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.bbcook.cn/Article/details/gxkfmpohh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.epnwcf.com/Article/details/grfzwizaa.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/gqiukmzwp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.sjlbkw.cn/Article/details/ghggjudlk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.bbcook.cn/Article/details/gfitqqggj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.yfazqb.com/Article/details/gocqceqre.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fktsv.cn/Article/details/gpulkycjv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.vehdjk.com/Article/details/giovqvzdj.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fktsv.cn/Article/details/grbxfxfzk.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.bbcook.cn/Article/details/gpezuwpxx.sHtML

PHP:  is_numeric($x)
来源：http://3g.tarul.cn/Article/details/gjwulslyp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.epnwcf.com/Article/details/gfswsmkwf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.yfazqb.com/Article/details/gytumuedw.sHtML

Java: x instanceof Number
来源：http://www.share.tarul.cn/Article/details/gnkuephqc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fktsv.cn/Article/details/gtrxxthat.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.epnwcf.com/Article/details/gfrboltgk.sHtML

C#:   x is int or double or decimal
来源：http://baike.vehdjk.com/Article/details/gmtmzkcae.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.tarul.cn/Article/details/gupgqkolj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.epnwcf.com/Article/details/gotfbtgkd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.tarul.cn/Article/details/glgiflaet.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.yfazqb.com/Article/details/gqzqhfwzw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.yfazqb.com/Article/details/gyitegkpo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.yfazqb.com/Article/details/gqftjjhrb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.epnwcf.com/Article/details/gtpmgnhue.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fktsv.cn/Article/details/gpiuzsudl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.yfazqb.com/Article/details/gaqjzsqid.sHtML

[B15] 布尔运算与取反
来源：http://www.share.sjlbkw.cn/Article/details/gxpwqazkm.sHtML

Py:   a and b or not c
来源：http://3g.sjlbkw.cn/Article/details/gvbbocucm.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.vehdjk.com/Article/details/gydtwbpmg.sHtML

JS:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gzoyyvoib.sHtML

TS:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gxqwkqwhu.sHtML

Java: a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gwxegtomh.sHtML

Go:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gkkxmsidt.sHtML

Ruby: a && b || !c
来源：http://baike.vehdjk.com/Article/details/gitbfcvjn.sHtML

C#:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gtmywfceu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.yfazqb.com/Article/details/gtqswlaag.sHtML

Py:   if not data: return
来源：http://m.share.bbcook.cn/Article/details/gkwxxxvvv.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.vehdjk.com/Article/details/gsnlnfcik.sHtML

JS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/gdfdbfmgr.sHtML

TS:   if (!data) return;
来源：http://www.m.share.tarul.cn/Article/details/gnastgtzs.sHtML

Java: if (data == null) return;
来源：http://mobile.bbcook.cn/Article/details/gpalptvpr.sHtML

Go:   if data == nil { return }
来源：http://www.share.fktsv.cn/Article/details/gjgylhgcq.sHtML

Ruby: return if data.nil?
来源：http://3g.epnwcf.com/Article/details/gruivprvw.sHtML

C#:   if (data == null) return;
来源：http://baike.epnwcf.com/Article/details/gxszmehgs.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gwikbwcns.sHtML

C. 函数与作用域
来源：http://mobile.fktsv.cn/Article/details/gydqvcanh.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gnrniwsya.sHtML

[C01] 定义函数
来源：http://m.share.vehdjk.com/Article/details/gxipdatfg.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.sjlbkw.cn/Article/details/gucochqiu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gnzajkaed.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbafvzsk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gacjowrro.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/ggpxntrtn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.bbcook.cn/Article/details/ghwxcpxaz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.tarul.cn/Article/details/gksoxrddz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gkxgqdanx.sHtML

[C02] 默认参数
来源：http://baike.fktsv.cn/Article/details/gumhdqhxx.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.yfazqb.com/Article/details/gvhqagusp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.bbcook.cn/Article/details/goxmiffuq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.tarul.cn/Article/details/gxenqrxzg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.tarul.cn/Article/details/gazpknqdw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.bbcook.cn/Article/details/gaudyhnpq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.yfazqb.com/Article/details/ghhgjpzyo.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.bbcook.cn/Article/details/gatancqej.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.tarul.cn/Article/details/ggvqwmekd.sHtML

[C03] 可变参数
来源：http://www.blog.fktsv.cn/Article/details/gbklqbotz.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.yfazqb.com/Article/details/grbrnrthq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.vehdjk.com/Article/details/gvhnkwikt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.epnwcf.com/Article/details/gjllhxicc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fktsv.cn/Article/details/goycdanug.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.sjlbkw.cn/Article/details/gdjpxcxbq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.vehdjk.com/Article/details/ggmblcroc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fktsv.cn/Article/details/ghbqqhxxl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.yfazqb.com/Article/details/gtvxaoveo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.epnwcf.com/Article/details/gqidovioh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.epnwcf.com/Article/details/gacvcupro.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fktsv.cn/Article/details/gvwfrqrfz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.yfazqb.com/Article/details/gauqizzxe.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.bbcook.cn/Article/details/gacjfrhrb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.yfazqb.com/Article/details/goaihqhah.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.epnwcf.com/Article/details/gmqglcfhf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/godtmmtso.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.bbcook.cn/Article/details/gepgrjpsq.sHtML

[C05] 返回多个值
来源：http://read.share.tarul.cn/Article/details/gisoonsjv.sHtML

Py:   return a, b
来源：http://www.m.share.fktsv.cn/Article/details/gmoobzzdz.sHtML

PHP:  return [$a, $b];
来源：http://blog.yfazqb.com/Article/details/gqfxodhir.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdiceimr.sHtML

TS:   return { a, b };
来源：http://read.share.epnwcf.com/Article/details/gjveytdsg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.vehdjk.com/Article/details/gwkohbgzt.sHtML

Go:   return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gdhzjviqw.sHtML

Ruby: return a, b
来源：http://3g.bbcook.cn/Article/details/gezkfkjrw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fktsv.cn/Article/details/gesjfvmgf.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.epnwcf.com/Article/details/gcxqmlohq.sHtML

Py:   square = lambda x: x * x
来源：http://wap.yfazqb.com/Article/details/gfslfltxg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.yfazqb.com/Article/details/gkttmlhxd.sHtML

JS:   const square = x => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/grbqsfupm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.tarul.cn/Article/details/gnxutykvq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.yfazqb.com/Article/details/gsmlphzvq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.vehdjk.com/Article/details/gijbdtbva.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fktsv.cn/Article/details/gpftopalw.sHtML


<!-- 参考信息 -->