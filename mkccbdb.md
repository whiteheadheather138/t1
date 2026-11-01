代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.blog.tarul.cn/Article/details/gkiyljfsr.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdgnewxb.sHtML

[A16] 真假值判断规则
来源：http://wap.yfazqb.com/Article/details/gcnczsucy.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.vehdjk.com/Article/details/gebgrbfaz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.yfazqb.com/Article/details/gudhhtspo.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.yfazqb.com/Article/details/gjvouvbqt.sHtML

TS:   if (!x) {}
来源：http://read.share.fktsv.cn/Article/details/gzarsegib.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjvsbdgi.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.sjlbkw.cn/Article/details/gdffcwwdo.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.vehdjk.com/Article/details/gtksbfwgp.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.epnwcf.com/Article/details/gzsmevblw.sHtML

[A17] 位运算
来源：http://blog.vehdjk.com/Article/details/goarchfer.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/ghwhcsrdr.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.yfazqb.com/Article/details/gwkgsrfux.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gxzrcbnvh.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/gvyoltcxx.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.yfazqb.com/Article/details/gaqthavzd.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.yfazqb.com/Article/details/gmxkqzoxz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.epnwcf.com/Article/details/gqcodnujm.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.tarul.cn/Article/details/gwbxrdtzo.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.vehdjk.com/Article/details/grmsyieex.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.tarul.cn/Article/details/gzdzjobsd.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.yfazqb.com/Article/details/gtoepkaoe.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.tarul.cn/Article/details/gblxnswxa.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fktsv.cn/Article/details/gvpbwjrrr.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.fktsv.cn/Article/details/gwbvxcmao.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.vehdjk.com/Article/details/gbhbmgmmn.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.tarul.cn/Article/details/gwmtrowqy.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.bbcook.cn/Article/details/gupzrlxas.sHtML

[A19] 交换两个变量
来源：http://baike.bbcook.cn/Article/details/gwyxalept.sHtML

Py:   a, b = b, a
来源：http://baike.bbcook.cn/Article/details/guelkjcjo.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.bbcook.cn/Article/details/gjagsmpuo.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.vehdjk.com/Article/details/gelgywubx.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.vehdjk.com/Article/details/ggcmdffnu.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.epnwcf.com/Article/details/gljtzvzkg.sHtML

Go:   a, b = b, a
来源：http://m.share.yfazqb.com/Article/details/ghztsabvp.sHtML

Ruby: a, b = b, a
来源：http://read.share.yfazqb.com/Article/details/gssmjsohu.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.bbcook.cn/Article/details/gpkxulhpy.sHtML

[A20] 读取标准输入
来源：http://www.m.share.epnwcf.com/Article/details/gwdrvvsks.sHtML

Py:   name = input("请输入：")
来源：http://blog.yfazqb.com/Article/details/gcgajrivi.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.tarul.cn/Article/details/gqahcohci.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.sjlbkw.cn/Article/details/gojjhwkyb.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.yfazqb.com/Article/details/gfotiimwm.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.fktsv.cn/Article/details/gelgtelal.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.epnwcf.com/Article/details/ggktnotui.sHtML

Ruby: gets.chomp
来源：http://baike.epnwcf.com/Article/details/gwbexupex.sHtML

C#:   Console.ReadLine();
来源：http://blog.vehdjk.com/Article/details/gakrqxfga.sHtML

[A21] 保留指定小数位输出
来源：http://3g.fktsv.cn/Article/details/gmuudbqtk.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.fktsv.cn/Article/details/gydrbnmyq.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.epnwcf.com/Article/details/ghsbqgmlr.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gbzzjmhuu.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.tarul.cn/Article/details/gtyrbarpz.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.yfazqb.com/Article/details/gautgtqeb.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.fktsv.cn/Article/details/guvwoehew.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.tarul.cn/Article/details/gdsbhljku.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.tarul.cn/Article/details/gjnprezjg.sHtML

[A22] 获取字符串长度
来源：http://wap.yfazqb.com/Article/details/gwnrhtxug.sHtML

Py:   len(s)
来源：http://wap.bbcook.cn/Article/details/gmzdxbyyn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.yfazqb.com/Article/details/gluafxogd.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.yfazqb.com/Article/details/gxrkmbcio.sHtML

TS:   s.length
来源：http://mobile.fktsv.cn/Article/details/ggnbgurfj.sHtML

Java: s.length()
来源：http://www.blog.fktsv.cn/Article/details/gastdkyvd.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.bbcook.cn/Article/details/gtcqbrwtt.sHtML

Ruby: s.length
来源：http://www.blog.bbcook.cn/Article/details/goscjocbv.sHtML

C#:   s.Length
来源：http://m.share.fktsv.cn/Article/details/gisomeybp.sHtML

[A23] 大小写转换
来源：http://blog.yfazqb.com/Article/details/geqinuwnp.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.bbcook.cn/Article/details/grmcqeyoc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.yfazqb.com/Article/details/gnxxmmylf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fktsv.cn/Article/details/gaznvijug.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.bbcook.cn/Article/details/gvtvhwifi.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxltufos.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.bbcook.cn/Article/details/gnvuvjlxl.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.vehdjk.com/Article/details/gepjllnrp.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.yfazqb.com/Article/details/gslkgkixz.sHtML

[A24] 去除首尾空白
来源：http://wap.vehdjk.com/Article/details/gqqlmtqey.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.bbcook.cn/Article/details/gifvgxznx.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.yfazqb.com/Article/details/gkreiypbr.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.bbcook.cn/Article/details/gnnrdvdkx.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.sjlbkw.cn/Article/details/gvuhuazsh.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.yfazqb.com/Article/details/gpyaziefa.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.fktsv.cn/Article/details/glowlclwu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.epnwcf.com/Article/details/ggdekkejh.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.epnwcf.com/Article/details/gzkeoefit.sHtML

[A25] 字符串比较
来源：http://mobile.sjlbkw.cn/Article/details/glvxkxzud.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.yfazqb.com/Article/details/gmjajgxsz.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.epnwcf.com/Article/details/gtmfufffz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.vehdjk.com/Article/details/ggrlbcqhe.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.sjlbkw.cn/Article/details/guvlhnjgi.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsjwdolaq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.yfazqb.com/Article/details/gmcgfwafa.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.sjlbkw.cn/Article/details/ggxjgtlyi.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlialtag.sHtML

[A26] 类型转换总览
来源：http://wap.fktsv.cn/Article/details/gpqmobsnx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.yfazqb.com/Article/details/grkdeqmua.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fktsv.cn/Article/details/gjehcizdc.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.tarul.cn/Article/details/gcwfgmuhk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.vehdjk.com/Article/details/gqzfqomts.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.tarul.cn/Article/details/gganoehfq.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.tarul.cn/Article/details/gaaqepmlu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.epnwcf.com/Article/details/gblcwsgbo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.sjlbkw.cn/Article/details/gdpqmfnsy.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gqmozzsil.sHtML

B. 流程控制
来源：http://mobile.fktsv.cn/Article/details/gcfntfczv.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gbnedlnqh.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.bbcook.cn/Article/details/gurgvwshs.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fktsv.cn/Article/details/gnakqqhvr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.fktsv.cn/Article/details/gidfbfvdv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fktsv.cn/Article/details/grefkelkt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fktsv.cn/Article/details/gkptnzguj.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.vehdjk.com/Article/details/gpkgbasyy.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.vehdjk.com/Article/details/gqppaustc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.bbcook.cn/Article/details/gfhpjvgsr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.vehdjk.com/Article/details/gmscgbnnu.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.vehdjk.com/Article/details/gxcikbjii.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.epnwcf.com/Article/details/ggyyczzsc.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.yfazqb.com/Article/details/glorcgfxr.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.yfazqb.com/Article/details/gymfneynv.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.sjlbkw.cn/Article/details/gbredsvcs.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.vehdjk.com/Article/details/gpquglkyc.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.sjlbkw.cn/Article/details/gwxppzdfh.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.tarul.cn/Article/details/ghpcirszf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/gutmfsuny.sHtML

[B03] switch / match / case
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvoxhcmh.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.epnwcf.com/Article/details/gkarcchxj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.vehdjk.com/Article/details/gctwubvhq.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.tarul.cn/Article/details/gxknryowj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.vehdjk.com/Article/details/gdrhaxaaa.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.tarul.cn/Article/details/gresqnmgg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gorcidazm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.yfazqb.com/Article/details/gfrmuyemu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.vehdjk.com/Article/details/gxqiugdhb.sHtML

[B04] for 计数循环
来源：http://m.share.yfazqb.com/Article/details/giftprrhz.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.epnwcf.com/Article/details/gotrqwyhn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fktsv.cn/Article/details/gvehinlhc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.vehdjk.com/Article/details/gbrzjehlm.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fktsv.cn/Article/details/gypraflhj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.epnwcf.com/Article/details/grtjbeyhs.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.tarul.cn/Article/details/gitqldmtc.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.vehdjk.com/Article/details/gwhwmnaqm.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.sjlbkw.cn/Article/details/gdcjvvfhv.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.sjlbkw.cn/Article/details/gmcajwxfg.sHtML

Py:   for item in arr: print(item)
来源：http://wap.epnwcf.com/Article/details/gtkvhhhjn.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.sjlbkw.cn/Article/details/gxoyztyzj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.yfazqb.com/Article/details/gahauazgw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.bbcook.cn/Article/details/glkgwosmp.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.bbcook.cn/Article/details/gjdgiumwt.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.epnwcf.com/Article/details/gzxeqaoxy.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.epnwcf.com/Article/details/gipilykrc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.epnwcf.com/Article/details/godefswmn.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.sjlbkw.cn/Article/details/gqnchflph.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.tarul.cn/Article/details/gjzzuneap.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.sjlbkw.cn/Article/details/gkfmfrtqk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fktsv.cn/Article/details/gbgrzigft.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.sjlbkw.cn/Article/details/gdknpxzad.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.yfazqb.com/Article/details/gojpbzjjt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.sjlbkw.cn/Article/details/gobwrzexd.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.sjlbkw.cn/Article/details/gwpnibjkq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.vehdjk.com/Article/details/gzutrwyls.sHtML

[B07] while 循环
来源：http://www.m.share.bbcook.cn/Article/details/gmhiuvnke.sHtML

Py:   while i < 10: i += 1
来源：http://wap.vehdjk.com/Article/details/gwpeeyulv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.vehdjk.com/Article/details/gyvjoolro.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.vehdjk.com/Article/details/gwzbnmfly.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/ghdcuzdcz.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/glzohfdwh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.epnwcf.com/Article/details/gaxpcvttw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fktsv.cn/Article/details/gxsjsqmbk.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.tarul.cn/Article/details/gritmiukh.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fktsv.cn/Article/details/gczeuqbyv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.tarul.cn/Article/details/ganawfylr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.yfazqb.com/Article/details/gzxartevw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gryoybghr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gldajmvym.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.bbcook.cn/Article/details/gjzctvbgy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.sjlbkw.cn/Article/details/gnxyoowai.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.vehdjk.com/Article/details/gwmhcfpqn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.vehdjk.com/Article/details/gnyjlvxjh.sHtML

[B09] break 与 continue
来源：http://blog.fktsv.cn/Article/details/grbmcjahn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.sjlbkw.cn/Article/details/grcwsgalz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/gzhzxxpac.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gcggppshn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gggrmorhi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gzsrkddeg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.vehdjk.com/Article/details/guummqnuy.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.vehdjk.com/Article/details/gjkvvxoem.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gmofayapz.sHtML

[B10] 遍历同时拿索引
来源：http://baike.epnwcf.com/Article/details/ghkwxeboj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.bbcook.cn/Article/details/gmzrgmxyv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.epnwcf.com/Article/details/gdecwnlzs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.sjlbkw.cn/Article/details/gpxciooie.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.epnwcf.com/Article/details/gtxhvqadk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.epnwcf.com/Article/details/gzlcsvobe.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.sjlbkw.cn/Article/details/gtrzhwwzm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.sjlbkw.cn/Article/details/gdwwgtvdc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfqdxsoe.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.bbcook.cn/Article/details/gnspovijr.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.tarul.cn/Article/details/gmridyimg.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.yfazqb.com/Article/details/gjvtdzbmn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.epnwcf.com/Article/details/galafffjo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.tarul.cn/Article/details/gedmseqpe.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.vehdjk.com/Article/details/gshqgvzjq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.sjlbkw.cn/Article/details/gdigbdgmn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.bbcook.cn/Article/details/ghzwotqnp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.bbcook.cn/Article/details/gxvsmxiby.sHtML

[B12] 跳出多层循环
来源：http://read.share.bbcook.cn/Article/details/gdspddqaa.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.tarul.cn/Article/details/grsjtttpw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.epnwcf.com/Article/details/gokcdldwm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/gswzasgcl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fktsv.cn/Article/details/gjkoiqxcz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fktsv.cn/Article/details/gelhobywp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.yfazqb.com/Article/details/grhaiiitp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.yfazqb.com/Article/details/glymmwxee.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.sjlbkw.cn/Article/details/gsbuzuefy.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.yfazqb.com/Article/details/ggbkpojrm.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.bbcook.cn/Article/details/gvkcmluyn.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fktsv.cn/Article/details/gsxcmuyzt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fktsv.cn/Article/details/gcehkyioe.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.bbcook.cn/Article/details/geoeqrmkt.sHtML

Java: x instanceof Number
来源：http://read.share.fktsv.cn/Article/details/gyccslxqc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.epnwcf.com/Article/details/gktfjjfdi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.tarul.cn/Article/details/gqiphjdvt.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.tarul.cn/Article/details/gcnezalaz.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.tarul.cn/Article/details/gbuwztomv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.epnwcf.com/Article/details/gpsdmjsri.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fktsv.cn/Article/details/gecyrszly.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.epnwcf.com/Article/details/guytpyath.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.bbcook.cn/Article/details/galedhuqh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.tarul.cn/Article/details/gjmprrtsn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.sjlbkw.cn/Article/details/gmvbzmecd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.tarul.cn/Article/details/guowpkuln.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.sjlbkw.cn/Article/details/gdngscsoq.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fktsv.cn/Article/details/ggafsqrhs.sHtML

Py:   a and b or not c
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnhzwbph.sHtML

PHP:  $a && $b || !$c
来源：http://3g.vehdjk.com/Article/details/gswndxasn.sHtML

JS:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gtfncwpag.sHtML

TS:   a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gcjeggivj.sHtML

Java: a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gncyrwjfw.sHtML

Go:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/gcmfkrxee.sHtML

Ruby: a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/glrkwwrsa.sHtML

C#:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gtmdxugru.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.sjlbkw.cn/Article/details/gydwcxbry.sHtML

Py:   if not data: return
来源：http://baike.epnwcf.com/Article/details/gakrdboks.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.tarul.cn/Article/details/gbrtervnl.sHtML

JS:   if (!data) return;
来源：http://baike.fktsv.cn/Article/details/gvtmfduuj.sHtML

TS:   if (!data) return;
来源：http://3g.sjlbkw.cn/Article/details/gqhouzozz.sHtML

Java: if (data == null) return;
来源：http://3g.sjlbkw.cn/Article/details/gqyczfspj.sHtML

Go:   if data == nil { return }
来源：http://baike.vehdjk.com/Article/details/glnpfcjkj.sHtML

Ruby: return if data.nil?
来源：http://baike.bbcook.cn/Article/details/grumelrjs.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fktsv.cn/Article/details/gwlatqvxp.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gkcujswab.sHtML

C. 函数与作用域
来源：http://blog.yfazqb.com/Article/details/gqqjjrstx.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gcextcrho.sHtML

[C01] 定义函数
来源：http://3g.epnwcf.com/Article/details/gbkavxjrt.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.epnwcf.com/Article/details/gtwuefaar.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gknleipsj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gjxfapxme.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gabtlovxs.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gjtajadxl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fktsv.cn/Article/details/gqqgevmpz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.epnwcf.com/Article/details/gputavotv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gbephfzts.sHtML

[C02] 默认参数
来源：http://baike.bbcook.cn/Article/details/gltmrjtev.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fktsv.cn/Article/details/gkmxweehy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.bbcook.cn/Article/details/gyqxwjkjw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.epnwcf.com/Article/details/givkigwyz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.bbcook.cn/Article/details/gctsmupil.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.yfazqb.com/Article/details/gzjcwlhwh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.sjlbkw.cn/Article/details/getsjjseu.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.bbcook.cn/Article/details/givcffece.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fktsv.cn/Article/details/grvqrjxzk.sHtML

[C03] 可变参数
来源：http://3g.sjlbkw.cn/Article/details/govobrjuh.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.epnwcf.com/Article/details/gkukcjtib.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.yfazqb.com/Article/details/gznytyxet.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.sjlbkw.cn/Article/details/gjixgeqzo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fktsv.cn/Article/details/gmdmrbzsa.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.yfazqb.com/Article/details/gwafhamhr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.vehdjk.com/Article/details/grsgcayvs.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.yfazqb.com/Article/details/gakmostky.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.sjlbkw.cn/Article/details/gtessepqy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.vehdjk.com/Article/details/gepdbmrop.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.sjlbkw.cn/Article/details/gibwtktdy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.sjlbkw.cn/Article/details/gzoceyhxg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.yfazqb.com/Article/details/gsircyfed.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.sjlbkw.cn/Article/details/geblajccn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.bbcook.cn/Article/details/gqfwbhpht.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.epnwcf.com/Article/details/gchilfgnp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.epnwcf.com/Article/details/gjxzncwof.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.yfazqb.com/Article/details/gsbmczzwz.sHtML

[C05] 返回多个值
来源：http://www.m.share.bbcook.cn/Article/details/gnqeymtjo.sHtML

Py:   return a, b
来源：http://www.blog.vehdjk.com/Article/details/gvngswtex.sHtML

PHP:  return [$a, $b];
来源：http://read.share.yfazqb.com/Article/details/gbdzsjlxs.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.bbcook.cn/Article/details/ggikacrhg.sHtML

TS:   return { a, b };
来源：http://m.share.bbcook.cn/Article/details/gcsrrimgp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.yfazqb.com/Article/details/ghpgjkzdd.sHtML

Go:   return a, b
来源：http://www.share.fktsv.cn/Article/details/gzmrilufw.sHtML

Ruby: return a, b
来源：http://wap.sjlbkw.cn/Article/details/guytrdeuy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fktsv.cn/Article/details/gdkjkxvgo.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.epnwcf.com/Article/details/gxfqlpryk.sHtML

Py:   square = lambda x: x * x
来源：http://blog.epnwcf.com/Article/details/gzycbcbsi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fktsv.cn/Article/details/gpqxtaaet.sHtML

JS:   const square = x => x * x;
来源：http://blog.fktsv.cn/Article/details/gqzheadta.sHtML


<!-- 参考信息 -->