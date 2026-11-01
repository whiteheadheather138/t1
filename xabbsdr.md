代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://3g.sjlbkw.cn/Article/details/gqyooncfb.sHtML

[A15] 空值判断与默认值
来源：http://mobile.sjlbkw.cn/Article/details/gshwwaulp.sHtML

Py:   value = data or "默认值"
来源：http://blog.vehdjk.com/Article/details/gqazrovch.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.bbcook.cn/Article/details/gajzfrjpn.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.fktsv.cn/Article/details/gdxblwugz.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.sjlbkw.cn/Article/details/ghnivzmfq.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.yfazqb.com/Article/details/gnvaxdsrz.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.yfazqb.com/Article/details/gnbocfcga.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.fktsv.cn/Article/details/gjmtrmkun.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.epnwcf.com/Article/details/gmjokrill.sHtML

[A16] 真假值判断规则
来源：http://blog.epnwcf.com/Article/details/gdpwfcsri.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.epnwcf.com/Article/details/gvedcobyk.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.bbcook.cn/Article/details/gmchlkrtp.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.yfazqb.com/Article/details/gylcqxeik.sHtML

TS:   if (!x) {}
来源：http://read.share.fktsv.cn/Article/details/gsjzircet.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.epnwcf.com/Article/details/gmjifvsby.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.epnwcf.com/Article/details/gijbsgjyh.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.bbcook.cn/Article/details/gtqwicorc.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gqgkyukfk.sHtML

[A17] 位运算
来源：http://www.share.bbcook.cn/Article/details/gpeydzumc.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.bbcook.cn/Article/details/gjaftxglq.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.sjlbkw.cn/Article/details/gfxcgmttf.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/galyerprf.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/gswqyzqxk.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/gmhmdukil.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/gnmzmgrqf.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.bbcook.cn/Article/details/gtyvqcwwd.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.yfazqb.com/Article/details/graxhrouf.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.tarul.cn/Article/details/gnwvslcro.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.fktsv.cn/Article/details/gjftlyhwt.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.yfazqb.com/Article/details/gtokbcfdf.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fktsv.cn/Article/details/gsgvcewlx.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.vehdjk.com/Article/details/gsxjuyhhp.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fktsv.cn/Article/details/gcalabiwk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.sjlbkw.cn/Article/details/gpgklhlpd.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.bbcook.cn/Article/details/gktcizdif.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.epnwcf.com/Article/details/gbabwalda.sHtML

[A19] 交换两个变量
来源：http://baike.sjlbkw.cn/Article/details/gwnonnxkz.sHtML

Py:   a, b = b, a
来源：http://mobile.sjlbkw.cn/Article/details/gevbqhimc.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.bbcook.cn/Article/details/gpzuweijm.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.bbcook.cn/Article/details/gmxcklrkl.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkkxcfcx.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.bbcook.cn/Article/details/gslnszooe.sHtML

Go:   a, b = b, a
来源：http://www.blog.vehdjk.com/Article/details/gjwqkhcck.sHtML

Ruby: a, b = b, a
来源：http://mobile.tarul.cn/Article/details/gpvkalfqv.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.sjlbkw.cn/Article/details/gbahccrxb.sHtML

[A20] 读取标准输入
来源：http://www.blog.tarul.cn/Article/details/gmhkpjrbx.sHtML

Py:   name = input("请输入：")
来源：http://blog.sjlbkw.cn/Article/details/gaznqpiiy.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.sjlbkw.cn/Article/details/gawepjlpn.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.sjlbkw.cn/Article/details/gncoutkjq.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.fktsv.cn/Article/details/grgeryrbx.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.epnwcf.com/Article/details/gtxxyguhf.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.sjlbkw.cn/Article/details/gvcpvnbpb.sHtML

Ruby: gets.chomp
来源：http://blog.epnwcf.com/Article/details/gdzhjbxpq.sHtML

C#:   Console.ReadLine();
来源：http://wap.fktsv.cn/Article/details/gnrlodnku.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.sjlbkw.cn/Article/details/gebnalkiz.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.sjlbkw.cn/Article/details/gqmgydakc.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.bbcook.cn/Article/details/gzkfmvkno.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.yfazqb.com/Article/details/gnhksneyl.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.vehdjk.com/Article/details/gfisrwmha.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.epnwcf.com/Article/details/gisawwtvu.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.epnwcf.com/Article/details/genhxhnxb.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.tarul.cn/Article/details/gknlpmrer.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.epnwcf.com/Article/details/gmfhdignw.sHtML

[A22] 获取字符串长度
来源：http://www.share.bbcook.cn/Article/details/gsuevkhqu.sHtML

Py:   len(s)
来源：http://blog.vehdjk.com/Article/details/gfmhgbbjq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.fktsv.cn/Article/details/geldrhxeb.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.sjlbkw.cn/Article/details/glitgyckk.sHtML

TS:   s.length
来源：http://blog.yfazqb.com/Article/details/gxpucxfvk.sHtML

Java: s.length()
来源：http://read.share.fktsv.cn/Article/details/glvygiqrt.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.tarul.cn/Article/details/gsfcqqyot.sHtML

Ruby: s.length
来源：http://blog.bbcook.cn/Article/details/gtokxjbly.sHtML

C#:   s.Length
来源：http://baike.fktsv.cn/Article/details/girzotxyn.sHtML

[A23] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/gzgckgcof.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.yfazqb.com/Article/details/gewjktjdz.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.yfazqb.com/Article/details/gacmdmkos.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.sjlbkw.cn/Article/details/gyuncmvmi.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fktsv.cn/Article/details/gwalgeeid.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.tarul.cn/Article/details/gikzciauz.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.vehdjk.com/Article/details/gabukqehj.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.vehdjk.com/Article/details/gpjwnqxlk.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.yfazqb.com/Article/details/gtdvcawfh.sHtML

[A24] 去除首尾空白
来源：http://blog.tarul.cn/Article/details/gpcorcxkv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.vehdjk.com/Article/details/glreggltf.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.yfazqb.com/Article/details/grffdyuat.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.yfazqb.com/Article/details/gbfiewpkq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.tarul.cn/Article/details/gpolxpwwq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.bbcook.cn/Article/details/ghwedzutv.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.bbcook.cn/Article/details/ggwgakpgm.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.bbcook.cn/Article/details/glwsrvjhl.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.sjlbkw.cn/Article/details/guhypqdei.sHtML

[A25] 字符串比较
来源：http://wap.tarul.cn/Article/details/gmnonrbfk.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fktsv.cn/Article/details/gxmcvtfct.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.epnwcf.com/Article/details/gzpkvwijn.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.vehdjk.com/Article/details/gntoocgca.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.bbcook.cn/Article/details/goyoraxbe.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.tarul.cn/Article/details/guwachwxq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.tarul.cn/Article/details/gplaxqoap.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.sjlbkw.cn/Article/details/gjzcwmowp.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.epnwcf.com/Article/details/gkrdkigic.sHtML

[A26] 类型转换总览
来源：http://baike.tarul.cn/Article/details/gfiugrjoj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.sjlbkw.cn/Article/details/genovzxfv.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fktsv.cn/Article/details/gjaubtygd.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.yfazqb.com/Article/details/gbmamrrbo.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.epnwcf.com/Article/details/goqrsgnpw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.tarul.cn/Article/details/gbgkrvcfn.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fktsv.cn/Article/details/gvbzxgkjl.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.epnwcf.com/Article/details/ggcjpbgmx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.tarul.cn/Article/details/gsgnkfjah.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gjkgesxoz.sHtML

B. 流程控制
来源：http://www.share.bbcook.cn/Article/details/glupgijtf.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gxizackwi.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.vehdjk.com/Article/details/gerczvrfr.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.sjlbkw.cn/Article/details/giafesjtn.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfsyqvskw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.yfazqb.com/Article/details/ggrrinvcr.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.vehdjk.com/Article/details/gqytnnrxf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fktsv.cn/Article/details/garowennl.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.bbcook.cn/Article/details/ggnzkpgwb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.epnwcf.com/Article/details/gnnddatxr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/gugctgmlg.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.bbcook.cn/Article/details/goyyzyngs.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.epnwcf.com/Article/details/gdwaghwfk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.sjlbkw.cn/Article/details/gavzwwqyd.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.bbcook.cn/Article/details/gnndgzihy.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/gwrfuieto.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.epnwcf.com/Article/details/goeagcwjn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.epnwcf.com/Article/details/ggmdnbrwr.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.yfazqb.com/Article/details/gamsynayk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/gpaxltnkg.sHtML

[B03] switch / match / case
来源：http://blog.fktsv.cn/Article/details/gtqxsiccm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.bbcook.cn/Article/details/gblquuvxl.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gtzidvenx.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.vehdjk.com/Article/details/ggnonmhzz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fktsv.cn/Article/details/gnnzwagus.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.sjlbkw.cn/Article/details/gmyvdwinc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.tarul.cn/Article/details/gwhyqkhzy.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.epnwcf.com/Article/details/gfmijugjb.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.vehdjk.com/Article/details/gtdadsgar.sHtML

[B04] for 计数循环
来源：http://mobile.sjlbkw.cn/Article/details/gvvzsgzch.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.tarul.cn/Article/details/gcbkdrqwt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.bbcook.cn/Article/details/ghyytfdag.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.epnwcf.com/Article/details/grsrgplda.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/glboyrjbj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.tarul.cn/Article/details/ggocyhhhb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.epnwcf.com/Article/details/grvluhkeo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.epnwcf.com/Article/details/gdrcxxzxa.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.tarul.cn/Article/details/gqrjjxgum.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.vehdjk.com/Article/details/gozehixhu.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.vehdjk.com/Article/details/gmphvdtfl.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.tarul.cn/Article/details/gwcrnmhcd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.epnwcf.com/Article/details/gcmvjoidz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.sjlbkw.cn/Article/details/gaffptban.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.vehdjk.com/Article/details/gaufstaep.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.bbcook.cn/Article/details/guakhmfsl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.vehdjk.com/Article/details/gjulypqsl.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.tarul.cn/Article/details/ggidfdsru.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.epnwcf.com/Article/details/gkdqezeco.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.epnwcf.com/Article/details/gpnsfmumk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.tarul.cn/Article/details/gdfanshkx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.yfazqb.com/Article/details/gfubyapzs.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.bbcook.cn/Article/details/ghsmmcmia.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.epnwcf.com/Article/details/glgxxtoop.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.sjlbkw.cn/Article/details/gzvnmsiwg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.sjlbkw.cn/Article/details/gzfgmecgl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.bbcook.cn/Article/details/gngtiqcum.sHtML

[B07] while 循环
来源：http://www.m.share.tarul.cn/Article/details/gnztgioyf.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.yfazqb.com/Article/details/gbelsjsiq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.bbcook.cn/Article/details/gnqfjpbih.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/gmvzbrumi.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/gftngvssp.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/ghtozvmgp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fktsv.cn/Article/details/gxntvimph.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.tarul.cn/Article/details/gqqlnoqiq.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gweqnayfz.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.tarul.cn/Article/details/goygyyfxp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.epnwcf.com/Article/details/gvjdywkbx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.tarul.cn/Article/details/gfqtzlikd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gkzntbrin.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gzizvlfkl.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fktsv.cn/Article/details/goaekcoif.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.sjlbkw.cn/Article/details/gfkgxoxll.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.epnwcf.com/Article/details/guqefjdyq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/ghywensdn.sHtML

[B09] break 与 continue
来源：http://mobile.epnwcf.com/Article/details/gktlxxmal.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.sjlbkw.cn/Article/details/ggemzkffg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gyddipujc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.tarul.cn/Article/details/gokpiiptn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/gxnynbdjf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gwumvwhfk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.yfazqb.com/Article/details/gsoupuuzk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.vehdjk.com/Article/details/gnizttrma.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.tarul.cn/Article/details/gggqjqexm.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.tarul.cn/Article/details/gtxctuoov.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fktsv.cn/Article/details/gowtngxzu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.yfazqb.com/Article/details/gqztqiqep.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.yfazqb.com/Article/details/ggvzajsnc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fktsv.cn/Article/details/gbszybyhl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.sjlbkw.cn/Article/details/gdhebvfgf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fktsv.cn/Article/details/gwfphxlgs.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.yfazqb.com/Article/details/gzfezsgxs.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.bbcook.cn/Article/details/gwzeopdgd.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fktsv.cn/Article/details/galqksopp.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.bbcook.cn/Article/details/gildzkjjq.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.vehdjk.com/Article/details/gsjhkjydq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.tarul.cn/Article/details/grtfnvmoy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.sjlbkw.cn/Article/details/gswojrryo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.tarul.cn/Article/details/gsilsozse.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.epnwcf.com/Article/details/gijovtqbe.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.tarul.cn/Article/details/gfyexbdti.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.sjlbkw.cn/Article/details/gxrizhqaj.sHtML

[B12] 跳出多层循环
来源：http://www.share.sjlbkw.cn/Article/details/gtzjykwff.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.sjlbkw.cn/Article/details/gcdhbpuxn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.tarul.cn/Article/details/ghywlbupu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.tarul.cn/Article/details/gnmenoydf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/gvsoeocmw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/gpawgdhju.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.epnwcf.com/Article/details/gsliqdjbt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.vehdjk.com/Article/details/ggeftxosk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.tarul.cn/Article/details/goiaiwohi.sHtML

[B13] 判断是否为数字
来源：http://3g.yfazqb.com/Article/details/grvpglvvt.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fktsv.cn/Article/details/ggvvvwpej.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.yfazqb.com/Article/details/gluusctqf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fktsv.cn/Article/details/gaayrcrxk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.sjlbkw.cn/Article/details/gtsuknhda.sHtML

Java: x instanceof Number
来源：http://wap.vehdjk.com/Article/details/grsasydsx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.epnwcf.com/Article/details/gyexqrjoz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.bbcook.cn/Article/details/gslhjdfkk.sHtML

C#:   x is int or double or decimal
来源：http://mobile.vehdjk.com/Article/details/gstpoxels.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fktsv.cn/Article/details/gvixddvrz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.epnwcf.com/Article/details/gegbqugte.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.epnwcf.com/Article/details/gyxwnokeh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.vehdjk.com/Article/details/ggghqwves.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.tarul.cn/Article/details/gyiozdand.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.epnwcf.com/Article/details/gptepwure.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.bbcook.cn/Article/details/gmrsyolpw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fktsv.cn/Article/details/guugauntl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.tarul.cn/Article/details/gtkyxfohk.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fktsv.cn/Article/details/gurlzhosy.sHtML

Py:   a and b or not c
来源：http://www.share.yfazqb.com/Article/details/gzavrwcpe.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.sjlbkw.cn/Article/details/gfmhjysjr.sHtML

JS:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/gkkzxidre.sHtML

TS:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gqejoeqsd.sHtML

Java: a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gobkbujyo.sHtML

Go:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gajttjdsk.sHtML

Ruby: a && b || !c
来源：http://blog.yfazqb.com/Article/details/gjumokrdf.sHtML

C#:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/gmbjopazz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.epnwcf.com/Article/details/gbvvgghsa.sHtML

Py:   if not data: return
来源：http://m.share.epnwcf.com/Article/details/gkkfrdemv.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.bbcook.cn/Article/details/gsqgcotfo.sHtML

JS:   if (!data) return;
来源：http://read.share.tarul.cn/Article/details/gdxbgcbbf.sHtML

TS:   if (!data) return;
来源：http://mobile.sjlbkw.cn/Article/details/gtajipddr.sHtML

Java: if (data == null) return;
来源：http://wap.yfazqb.com/Article/details/gthcemlxu.sHtML

Go:   if data == nil { return }
来源：http://3g.bbcook.cn/Article/details/gvmhnlupi.sHtML

Ruby: return if data.nil?
来源：http://baike.fktsv.cn/Article/details/grviapjbi.sHtML

C#:   if (data == null) return;
来源：http://mobile.bbcook.cn/Article/details/gcwqorejb.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gpnbimlnw.sHtML

C. 函数与作用域
来源：http://m.share.sjlbkw.cn/Article/details/gnfzxsfnj.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gkicwhtdj.sHtML

[C01] 定义函数
来源：http://wap.bbcook.cn/Article/details/gffpeddim.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.bbcook.cn/Article/details/gidnaqmmq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/gexxdgqtw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gbxjvgmvv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gfqpqfplg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gflmsindz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.sjlbkw.cn/Article/details/ggcfqqwyt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.bbcook.cn/Article/details/gtancwiib.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/ghczpynpc.sHtML

[C02] 默认参数
来源：http://wap.vehdjk.com/Article/details/gvjdsxwua.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.epnwcf.com/Article/details/gtrhfbdkw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fktsv.cn/Article/details/gmluqspkg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.epnwcf.com/Article/details/ghbivvvas.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fktsv.cn/Article/details/gokmdjlqx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.epnwcf.com/Article/details/gnhfweead.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fktsv.cn/Article/details/gfzdffbxe.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fktsv.cn/Article/details/gdcgjvbed.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.epnwcf.com/Article/details/gajhnzbof.sHtML

[C03] 可变参数
来源：http://3g.epnwcf.com/Article/details/gmzgppywi.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.yfazqb.com/Article/details/gqjotmhny.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.epnwcf.com/Article/details/gckovsklt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.yfazqb.com/Article/details/geajqjsvu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.vehdjk.com/Article/details/gjnwnhjer.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.tarul.cn/Article/details/girkffqjd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.yfazqb.com/Article/details/gkpxytkrh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.tarul.cn/Article/details/glxupxizs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.tarul.cn/Article/details/gsyrtsptx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.tarul.cn/Article/details/gnfygicpd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.epnwcf.com/Article/details/gvzeoyhth.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.sjlbkw.cn/Article/details/gzcdsobvb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.vehdjk.com/Article/details/gkiqxcyur.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.vehdjk.com/Article/details/gycgjkggm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.sjlbkw.cn/Article/details/gfdlhxqem.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.epnwcf.com/Article/details/gjenpgphi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.yfazqb.com/Article/details/gkyabjgzn.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/gpbfwrwkp.sHtML

[C05] 返回多个值
来源：http://baike.bbcook.cn/Article/details/gbemkybtd.sHtML

Py:   return a, b
来源：http://read.share.tarul.cn/Article/details/gqlkbaeyj.sHtML

PHP:  return [$a, $b];
来源：http://baike.sjlbkw.cn/Article/details/gtmfhypyt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fktsv.cn/Article/details/gbkuygqpd.sHtML

TS:   return { a, b };
来源：http://read.share.sjlbkw.cn/Article/details/gjuardycb.sHtML


<!-- 参考信息 -->