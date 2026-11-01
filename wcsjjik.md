代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://mobile.fktsv.cn/Article/details/gsqlajlrj.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fktsv.cn/Article/details/geycjgrfr.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.epnwcf.com/Article/details/gkvhzzrrh.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.bbcook.cn/Article/details/gymiqzkdl.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.bbcook.cn/Article/details/gujhmkhzl.sHtML

[A15] 空值判断与默认值
来源：http://m.share.bbcook.cn/Article/details/ghwkylsrv.sHtML

Py:   value = data or "默认值"
来源：http://wap.fktsv.cn/Article/details/gqckldqkq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.epnwcf.com/Article/details/gyqrlvjak.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.tarul.cn/Article/details/gmsklayon.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.tarul.cn/Article/details/gmrfqqsff.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.yfazqb.com/Article/details/gdfopfxez.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.sjlbkw.cn/Article/details/gowthhttg.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.fktsv.cn/Article/details/gjzitfxwr.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.fktsv.cn/Article/details/glvfcncem.sHtML

[A16] 真假值判断规则
来源：http://www.share.epnwcf.com/Article/details/gnegyydzx.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.vehdjk.com/Article/details/gsuewerys.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.tarul.cn/Article/details/gpvlgqekq.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.fktsv.cn/Article/details/gshhteauc.sHtML

TS:   if (!x) {}
来源：http://3g.tarul.cn/Article/details/gxszcizuc.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.tarul.cn/Article/details/gidxsecim.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.fktsv.cn/Article/details/gykzmjnba.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.fktsv.cn/Article/details/gkcepkext.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.tarul.cn/Article/details/guqagyjxt.sHtML

[A17] 位运算
来源：http://wap.sjlbkw.cn/Article/details/gutfirvqg.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.bbcook.cn/Article/details/gtlxxyheh.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.vehdjk.com/Article/details/gxwnyoarw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.vehdjk.com/Article/details/gqfvtajed.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.fktsv.cn/Article/details/glihfqosf.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/gnhsrnrjs.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.sjlbkw.cn/Article/details/gzwixhitb.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/gsopxfmcw.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.vehdjk.com/Article/details/gescycfpv.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.epnwcf.com/Article/details/gqqdiarnw.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.yfazqb.com/Article/details/gkvjbxmrb.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.tarul.cn/Article/details/gakvdqsbi.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.sjlbkw.cn/Article/details/gvfzvcxsk.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.epnwcf.com/Article/details/gbmvrtkor.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.sjlbkw.cn/Article/details/ghkhfbzes.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.epnwcf.com/Article/details/gssraomto.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.tarul.cn/Article/details/gxweqdriy.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.vehdjk.com/Article/details/gywxupvtk.sHtML

[A19] 交换两个变量
来源：http://read.share.fktsv.cn/Article/details/gnqbifprb.sHtML

Py:   a, b = b, a
来源：http://blog.bbcook.cn/Article/details/gsyzohert.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.sjlbkw.cn/Article/details/gdwnzcztr.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.tarul.cn/Article/details/grhtjfrln.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.tarul.cn/Article/details/gbluiztsl.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.fktsv.cn/Article/details/ghoqfldrl.sHtML

Go:   a, b = b, a
来源：http://read.share.tarul.cn/Article/details/gxrrgamqx.sHtML

Ruby: a, b = b, a
来源：http://m.share.yfazqb.com/Article/details/gylqyqxkh.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.vehdjk.com/Article/details/gwiipjncc.sHtML

[A20] 读取标准输入
来源：http://www.blog.vehdjk.com/Article/details/gnivtqfin.sHtML

Py:   name = input("请输入：")
来源：http://wap.yfazqb.com/Article/details/gdkpjyhaa.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.yfazqb.com/Article/details/gwmzldacx.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.yfazqb.com/Article/details/gkoctwqqr.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.yfazqb.com/Article/details/ghgerpfkj.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.bbcook.cn/Article/details/gmhdecdcw.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.yfazqb.com/Article/details/gcbbworzo.sHtML

Ruby: gets.chomp
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqovorao.sHtML

C#:   Console.ReadLine();
来源：http://baike.epnwcf.com/Article/details/gzsstqtla.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.bbcook.cn/Article/details/gaxbmrltw.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.vehdjk.com/Article/details/gbyopmsec.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.yfazqb.com/Article/details/gksukxmju.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.yfazqb.com/Article/details/gxjridhkf.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.epnwcf.com/Article/details/gfcsvkuyk.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.fktsv.cn/Article/details/gzekjerex.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.fktsv.cn/Article/details/gwlphckfd.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.fktsv.cn/Article/details/gregqchos.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.sjlbkw.cn/Article/details/gvwditiyy.sHtML

[A22] 获取字符串长度
来源：http://blog.yfazqb.com/Article/details/glcjbshon.sHtML

Py:   len(s)
来源：http://baike.tarul.cn/Article/details/gijfsrzuu.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.vehdjk.com/Article/details/gzjiyxzgf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.vehdjk.com/Article/details/gcwdfnuwm.sHtML

TS:   s.length
来源：http://blog.fktsv.cn/Article/details/gusomoymf.sHtML

Java: s.length()
来源：http://mobile.epnwcf.com/Article/details/genhgezhl.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.tarul.cn/Article/details/gfcfuxzca.sHtML

Ruby: s.length
来源：http://3g.fktsv.cn/Article/details/gjclvwpzr.sHtML

C#:   s.Length
来源：http://read.share.fktsv.cn/Article/details/gmchmbtmy.sHtML

[A23] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gqdnxyofg.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.epnwcf.com/Article/details/gsnzdszxs.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.yfazqb.com/Article/details/gwxeqdjlh.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.epnwcf.com/Article/details/gyyjgqqgt.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.sjlbkw.cn/Article/details/gevmhufpi.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.yfazqb.com/Article/details/glsjpfzwc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.vehdjk.com/Article/details/ghdsbgsbq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.fktsv.cn/Article/details/gfacabtux.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.vehdjk.com/Article/details/gwfphcspj.sHtML

[A24] 去除首尾空白
来源：http://wap.yfazqb.com/Article/details/gzfnkrido.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.fktsv.cn/Article/details/ganqhqmaj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.vehdjk.com/Article/details/glpnzlybg.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.vehdjk.com/Article/details/gywqowbfu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.sjlbkw.cn/Article/details/gnnwrtsjy.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.vehdjk.com/Article/details/gkeeocgji.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.yfazqb.com/Article/details/grxkveoql.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.tarul.cn/Article/details/gegnfnvrw.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.yfazqb.com/Article/details/gfncdbioz.sHtML

[A25] 字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/gatdjlaxa.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.bbcook.cn/Article/details/gxuqkuyce.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.epnwcf.com/Article/details/gnnprekkg.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fktsv.cn/Article/details/gmjlunopu.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.yfazqb.com/Article/details/ggercnbuu.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.tarul.cn/Article/details/ggmxtqdig.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtnetusl.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.bbcook.cn/Article/details/gzkvzuvvd.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.bbcook.cn/Article/details/gmfvyhxsk.sHtML

[A26] 类型转换总览
来源：http://blog.vehdjk.com/Article/details/gduufrnci.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.tarul.cn/Article/details/gkwbplapw.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.yfazqb.com/Article/details/gijnfszre.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.tarul.cn/Article/details/gfrtakkuv.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.vehdjk.com/Article/details/gvnlwfoua.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.epnwcf.com/Article/details/glaydoqnh.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.vehdjk.com/Article/details/gpczirhxv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.yfazqb.com/Article/details/gdklrgmvk.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.yfazqb.com/Article/details/gblednoac.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gsboaepwt.sHtML

B. 流程控制
来源：http://3g.bbcook.cn/Article/details/gmoxeicsk.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gtyztetua.sHtML

[B01] 条件判断 if / else
来源：http://wap.yfazqb.com/Article/details/gcplnrkxm.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.vehdjk.com/Article/details/gbpkbcwfj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.yfazqb.com/Article/details/gydlnrdtg.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/gfxqzyrya.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqwfqvyw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.bbcook.cn/Article/details/gjdzqntko.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.vehdjk.com/Article/details/ghayytdet.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.fktsv.cn/Article/details/gywplqair.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.yfazqb.com/Article/details/gzurjnver.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.bbcook.cn/Article/details/gotkwmmni.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.tarul.cn/Article/details/gqlopjbrf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fktsv.cn/Article/details/gumhqgrnq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/gtiewndji.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fktsv.cn/Article/details/giowlzctq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.epnwcf.com/Article/details/gbfxnioli.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.yfazqb.com/Article/details/gkkumnkeb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.sjlbkw.cn/Article/details/gwuxkyejx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.epnwcf.com/Article/details/gfxwowcqv.sHtML

[B03] switch / match / case
来源：http://read.share.bbcook.cn/Article/details/gfpuqioci.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.yfazqb.com/Article/details/gimreylly.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/gtqkxufah.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.bbcook.cn/Article/details/ghalqgxdl.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gdgvwmngc.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.vehdjk.com/Article/details/gbweuoaub.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.yfazqb.com/Article/details/gzeitgcjf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.sjlbkw.cn/Article/details/gqsqogkbz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fktsv.cn/Article/details/gthsjtmiv.sHtML

[B04] for 计数循环
来源：http://mobile.sjlbkw.cn/Article/details/gsrkccqah.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.fktsv.cn/Article/details/gszzjclwc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.sjlbkw.cn/Article/details/gntckteaj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.yfazqb.com/Article/details/gftkvodwu.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.yfazqb.com/Article/details/gldgoesni.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.bbcook.cn/Article/details/gdkkzbull.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.vehdjk.com/Article/details/gswhbacgb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.vehdjk.com/Article/details/gwgtkkrhz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.epnwcf.com/Article/details/gyohmxkgw.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.yfazqb.com/Article/details/gphhbunsg.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.epnwcf.com/Article/details/gezxrukfr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.sjlbkw.cn/Article/details/ggpilmmyj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fktsv.cn/Article/details/gjjiadnjn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.yfazqb.com/Article/details/gncxjiwxg.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.vehdjk.com/Article/details/gpyzexoag.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.sjlbkw.cn/Article/details/gtlpmvfop.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.tarul.cn/Article/details/grfvzemzg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.yfazqb.com/Article/details/gtfcrmska.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.tarul.cn/Article/details/gdcgregfk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.vehdjk.com/Article/details/gughgzbot.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.tarul.cn/Article/details/goohiooes.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.tarul.cn/Article/details/gpgfymoqy.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gylbmkzry.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.tarul.cn/Article/details/gewrwhted.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.yfazqb.com/Article/details/gjernvcro.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.sjlbkw.cn/Article/details/ghpbertbl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.epnwcf.com/Article/details/gcorxhoep.sHtML

[B07] while 循环
来源：http://www.blog.bbcook.cn/Article/details/grfdqqszr.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.fktsv.cn/Article/details/glnydbwms.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.vehdjk.com/Article/details/ggankkaay.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.epnwcf.com/Article/details/gxwkgdzgk.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.epnwcf.com/Article/details/gzasjurmg.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gflnbdqsa.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.yfazqb.com/Article/details/gguethiki.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fktsv.cn/Article/details/gqovobrqd.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gsizqcfjm.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.vehdjk.com/Article/details/ggcxzokvx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.yfazqb.com/Article/details/gvvahqyjg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.epnwcf.com/Article/details/ghyvnzcom.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.epnwcf.com/Article/details/gzokouzmw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gflwrekmy.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/grkzxjhrq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.vehdjk.com/Article/details/goxfeilkj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.vehdjk.com/Article/details/gdorawfdb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gqvfuhqfa.sHtML

[B09] break 与 continue
来源：http://wap.fktsv.cn/Article/details/gjvyxkhgt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fktsv.cn/Article/details/gomujxwer.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/ghapavjti.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/gkitxgill.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gfxcppdtv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/gxsvgnect.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.vehdjk.com/Article/details/gvixknacl.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.vehdjk.com/Article/details/gwxikzinx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/ghnadghku.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.sjlbkw.cn/Article/details/gziokcrnz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.epnwcf.com/Article/details/gbbtjqhkv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.yfazqb.com/Article/details/gnbdzjqzx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fktsv.cn/Article/details/gvtxgcicz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.epnwcf.com/Article/details/gjodupfsb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.yfazqb.com/Article/details/goglhyosv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.tarul.cn/Article/details/gbhkznfzt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.epnwcf.com/Article/details/gpqfbmtcl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.sjlbkw.cn/Article/details/godrvxoql.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.yfazqb.com/Article/details/gmpbfouwq.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.epnwcf.com/Article/details/gnizlcwtu.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.tarul.cn/Article/details/gdfdmyxya.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.bbcook.cn/Article/details/gjseidbaj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.yfazqb.com/Article/details/geqjhopsh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.epnwcf.com/Article/details/grlwlrgip.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.vehdjk.com/Article/details/golkdjwhy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fktsv.cn/Article/details/gyuvxlhoz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.epnwcf.com/Article/details/grsatpftl.sHtML

[B12] 跳出多层循环
来源：http://blog.vehdjk.com/Article/details/gizayjwub.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.bbcook.cn/Article/details/gbzedwlui.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.vehdjk.com/Article/details/gpwdxzapk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/gjslnfhcu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/gwgqjejzy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.epnwcf.com/Article/details/grfrlooyl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.tarul.cn/Article/details/guknznxab.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fktsv.cn/Article/details/gprejmhjp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.vehdjk.com/Article/details/gdwrckbsm.sHtML

[B13] 判断是否为数字
来源：http://www.share.vehdjk.com/Article/details/gsflfitdf.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.tarul.cn/Article/details/gybbrgwvn.sHtML

PHP:  is_numeric($x)
来源：http://m.share.epnwcf.com/Article/details/gnmhsrmqm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fktsv.cn/Article/details/gaeaspibw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fktsv.cn/Article/details/gotgqyyyg.sHtML

Java: x instanceof Number
来源：http://baike.yfazqb.com/Article/details/gariilosp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fktsv.cn/Article/details/gsmkwoxcs.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.epnwcf.com/Article/details/gbokjemix.sHtML

C#:   x is int or double or decimal
来源：http://m.share.vehdjk.com/Article/details/gyuwmbbzu.sHtML

[B14] 判断值是否在集合内
来源：http://baike.yfazqb.com/Article/details/ggfklidyp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.bbcook.cn/Article/details/gycrwxghi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.tarul.cn/Article/details/ghtmpbhik.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gryktxajd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.vehdjk.com/Article/details/gijvzyxwr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.epnwcf.com/Article/details/ggdslozwb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.vehdjk.com/Article/details/gmubogclx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.yfazqb.com/Article/details/gffpkgnul.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.tarul.cn/Article/details/gazjbhscm.sHtML

[B15] 布尔运算与取反
来源：http://mobile.sjlbkw.cn/Article/details/gzqggqhwo.sHtML

Py:   a and b or not c
来源：http://www.blog.bbcook.cn/Article/details/gjisksmym.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fktsv.cn/Article/details/giobzxduh.sHtML

JS:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gahunsaps.sHtML

TS:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gwvqcahgy.sHtML

Java: a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gzsogmwpp.sHtML

Go:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/gxbhzozpg.sHtML

Ruby: a && b || !c
来源：http://blog.vehdjk.com/Article/details/gsxothwuf.sHtML

C#:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gbplysmpj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.epnwcf.com/Article/details/ghttrmtpf.sHtML

Py:   if not data: return
来源：http://read.share.vehdjk.com/Article/details/ggsvmluca.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.bbcook.cn/Article/details/gthbcamyb.sHtML

JS:   if (!data) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/glbassswj.sHtML

TS:   if (!data) return;
来源：http://www.blog.sjlbkw.cn/Article/details/gjgnvdder.sHtML

Java: if (data == null) return;
来源：http://blog.bbcook.cn/Article/details/geevdvfmq.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fktsv.cn/Article/details/gxknwlqyl.sHtML

Ruby: return if data.nil?
来源：http://www.share.sjlbkw.cn/Article/details/gktmbnrme.sHtML

C#:   if (data == null) return;
来源：http://blog.tarul.cn/Article/details/gtoyxzump.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gdsnuppxh.sHtML

C. 函数与作用域
来源：http://baike.vehdjk.com/Article/details/ghzcgikfe.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gactkjsoo.sHtML

[C01] 定义函数
来源：http://www.blog.yfazqb.com/Article/details/gxtrbpjoq.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.yfazqb.com/Article/details/gaubrmssh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fktsv.cn/Article/details/gwulommwh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/grdyunpcu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gejaotacr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gabwtvwwr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fktsv.cn/Article/details/grrgkkzcs.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.sjlbkw.cn/Article/details/ggvcicjep.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gvkdiobst.sHtML

[C02] 默认参数
来源：http://baike.epnwcf.com/Article/details/gqhbuubya.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.sjlbkw.cn/Article/details/gzjsmsjiw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.bbcook.cn/Article/details/guybduxdz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gkwnrfxgu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.bbcook.cn/Article/details/gbwamzkxt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.tarul.cn/Article/details/gfrvujdol.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.sjlbkw.cn/Article/details/ghkftzzci.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.epnwcf.com/Article/details/gayaoawss.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.yfazqb.com/Article/details/gbpjbdbyx.sHtML

[C03] 可变参数
来源：http://www.blog.yfazqb.com/Article/details/gbzoxvmvu.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.vehdjk.com/Article/details/gyphaknek.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.bbcook.cn/Article/details/gdznhsgjr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.bbcook.cn/Article/details/gaijrlysy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.vehdjk.com/Article/details/gnsupjrfc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.sjlbkw.cn/Article/details/gucapfczq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.bbcook.cn/Article/details/gblxrjlxc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.tarul.cn/Article/details/gmpwoyhcn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fktsv.cn/Article/details/gygahpfyf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fktsv.cn/Article/details/gilfamamf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.epnwcf.com/Article/details/gwcywyoyk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.vehdjk.com/Article/details/ghxweefea.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.sjlbkw.cn/Article/details/gepovrzwa.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.yfazqb.com/Article/details/gjobafyfk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.tarul.cn/Article/details/ghpdetnuv.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.tarul.cn/Article/details/gisxhubsc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.tarul.cn/Article/details/gzpxyukgn.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.yfazqb.com/Article/details/gycmhkmmj.sHtML

[C05] 返回多个值
来源：http://blog.bbcook.cn/Article/details/ggpszspqv.sHtML


<!-- 参考信息 -->