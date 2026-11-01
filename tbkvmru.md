代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.yfazqb.com/Article/details/gxibgckss.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.epnwcf.com/Article/details/gnkppwczz.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.vehdjk.com/Article/details/gofdteuly.sHtML

[A17] 位运算
来源：http://m.share.yfazqb.com/Article/details/gaqxrobvw.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/gbkvuouan.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fktsv.cn/Article/details/gnquuyqof.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.vehdjk.com/Article/details/goeqxdcnd.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/gemihrcfn.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.bbcook.cn/Article/details/gfwbbjqjh.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.bbcook.cn/Article/details/gpvqcglfe.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/gjymntybn.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.yfazqb.com/Article/details/ggjipxkgx.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.vehdjk.com/Article/details/grwliimpz.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.vehdjk.com/Article/details/gdbafmatj.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.yfazqb.com/Article/details/gbdyvivgm.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.epnwcf.com/Article/details/gydhudfzi.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.tarul.cn/Article/details/gsmgydhqk.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.epnwcf.com/Article/details/gfomtorls.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.vehdjk.com/Article/details/gmijrwlyn.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.sjlbkw.cn/Article/details/gyiwatfvp.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.epnwcf.com/Article/details/gjhifbijy.sHtML

[A19] 交换两个变量
来源：http://mobile.bbcook.cn/Article/details/gpgdqjyyu.sHtML

Py:   a, b = b, a
来源：http://mobile.fktsv.cn/Article/details/gjwmlxudf.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.vehdjk.com/Article/details/gqlwjukbm.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.bbcook.cn/Article/details/gytdqwgzz.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.yfazqb.com/Article/details/giwetgopv.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.yfazqb.com/Article/details/gnkuocgmx.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fktsv.cn/Article/details/gsbijqhpt.sHtML

Ruby: a, b = b, a
来源：http://m.share.vehdjk.com/Article/details/gzdfpfkuw.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.fktsv.cn/Article/details/ggbabudtl.sHtML

[A20] 读取标准输入
来源：http://www.m.share.fktsv.cn/Article/details/gbvoqffao.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.tarul.cn/Article/details/gjqomwllh.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.yfazqb.com/Article/details/gvlbyyhxf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.epnwcf.com/Article/details/gfsyvbjmk.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.epnwcf.com/Article/details/gipfdfidc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.epnwcf.com/Article/details/gulsqnhqw.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.vehdjk.com/Article/details/gkaautwxr.sHtML

Ruby: gets.chomp
来源：http://baike.yfazqb.com/Article/details/ghgzfqznb.sHtML

C#:   Console.ReadLine();
来源：http://wap.fktsv.cn/Article/details/guictxnfv.sHtML

[A21] 保留指定小数位输出
来源：http://blog.yfazqb.com/Article/details/geratkuqt.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.vehdjk.com/Article/details/gwuopgory.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.tarul.cn/Article/details/grkrfgury.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.sjlbkw.cn/Article/details/gdvrgdqrh.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.yfazqb.com/Article/details/gbpelbibn.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.sjlbkw.cn/Article/details/gxelljwnb.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.tarul.cn/Article/details/gacnjjqsv.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.bbcook.cn/Article/details/gpgmvidbp.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.yfazqb.com/Article/details/ggbazimir.sHtML

[A22] 获取字符串长度
来源：http://blog.sjlbkw.cn/Article/details/gsejfwisn.sHtML

Py:   len(s)
来源：http://read.share.sjlbkw.cn/Article/details/gooudzzem.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.epnwcf.com/Article/details/guvdyogja.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.vehdjk.com/Article/details/glwjdqmbi.sHtML

TS:   s.length
来源：http://mobile.epnwcf.com/Article/details/glkbdtlzv.sHtML

Java: s.length()
来源：http://blog.epnwcf.com/Article/details/gucmztsbi.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.bbcook.cn/Article/details/gehukvhpi.sHtML

Ruby: s.length
来源：http://read.share.yfazqb.com/Article/details/gssiwbyyc.sHtML

C#:   s.Length
来源：http://blog.epnwcf.com/Article/details/gvzhmheqi.sHtML

[A23] 大小写转换
来源：http://www.m.share.epnwcf.com/Article/details/gxojbxfyh.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.yfazqb.com/Article/details/ggsehqnxv.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.yfazqb.com/Article/details/gwqjnjxxp.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fktsv.cn/Article/details/gmgrqwpgv.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.bbcook.cn/Article/details/gendzjfiq.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.bbcook.cn/Article/details/gmqodwdgi.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.tarul.cn/Article/details/gxzaklzqb.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.vehdjk.com/Article/details/gplavbpxo.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.yfazqb.com/Article/details/gxvhwegap.sHtML

[A24] 去除首尾空白
来源：http://wap.yfazqb.com/Article/details/gsayssyeu.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.bbcook.cn/Article/details/goixwhcvh.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.vehdjk.com/Article/details/gisxblcyz.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.tarul.cn/Article/details/guvtvrwgy.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.epnwcf.com/Article/details/gnclodzzx.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.bbcook.cn/Article/details/gxxnovpzx.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.vehdjk.com/Article/details/gqlvmlnaq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.tarul.cn/Article/details/geeehhglo.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.epnwcf.com/Article/details/gwvmalaaj.sHtML

[A25] 字符串比较
来源：http://www.m.share.vehdjk.com/Article/details/gbrkidaas.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.yfazqb.com/Article/details/guhedfrre.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.yfazqb.com/Article/details/gicycbfwb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.epnwcf.com/Article/details/gvjckwfls.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.bbcook.cn/Article/details/gyoioommr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.fktsv.cn/Article/details/gjuzxtnfg.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.epnwcf.com/Article/details/grpxgywoj.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.sjlbkw.cn/Article/details/gqzfskzcu.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.fktsv.cn/Article/details/gqbjcitqv.sHtML

[A26] 类型转换总览
来源：http://mobile.bbcook.cn/Article/details/gytmxtltf.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.bbcook.cn/Article/details/gysvioqbz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.bbcook.cn/Article/details/giuoazvew.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.epnwcf.com/Article/details/gxlfvrbry.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.tarul.cn/Article/details/gbevqsurh.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.epnwcf.com/Article/details/gvstqslgp.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.vehdjk.com/Article/details/gytkhfobx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.yfazqb.com/Article/details/gmfitfqhb.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.sjlbkw.cn/Article/details/gyrrbielu.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gsvixexza.sHtML

B. 流程控制
来源：http://www.blog.vehdjk.com/Article/details/gzflgcavz.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gwvfddwxc.sHtML

[B01] 条件判断 if / else
来源：http://mobile.tarul.cn/Article/details/glgcpqzqq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.tarul.cn/Article/details/gkiuqaabx.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.sjlbkw.cn/Article/details/gjulmxcxd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.epnwcf.com/Article/details/gsbqyqzhz.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/gbluhrpvf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.epnwcf.com/Article/details/gypfdntul.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fktsv.cn/Article/details/glwcxjouy.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.tarul.cn/Article/details/gbjpgligu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.sjlbkw.cn/Article/details/gapebneyj.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fktsv.cn/Article/details/gffeilztf.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fktsv.cn/Article/details/gzpezowoi.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.vehdjk.com/Article/details/gdvqlwzhw.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.sjlbkw.cn/Article/details/gycbjzlhj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/gtlscheyr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.yfazqb.com/Article/details/gltywykbm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.epnwcf.com/Article/details/gxaxslxmd.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.sjlbkw.cn/Article/details/gutwqohvz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.epnwcf.com/Article/details/gswzblcls.sHtML

[B03] switch / match / case
来源：http://wap.tarul.cn/Article/details/gstduuypy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.yfazqb.com/Article/details/glpqtwnia.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/gvhnuofos.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/gtrrrllyx.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.tarul.cn/Article/details/gfrunqhzx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/gnjodzhgx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.vehdjk.com/Article/details/gwtubvoar.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.vehdjk.com/Article/details/gzqzeclms.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.bbcook.cn/Article/details/gowdaxdxa.sHtML

[B04] for 计数循环
来源：http://m.share.bbcook.cn/Article/details/guftmjsrd.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fktsv.cn/Article/details/gyuhplrlx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.yfazqb.com/Article/details/gffdwbbfl.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gyvlfdcbp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.sjlbkw.cn/Article/details/gyqjgbtqk.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.yfazqb.com/Article/details/gnqpbdapy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.yfazqb.com/Article/details/gvldqlckh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.bbcook.cn/Article/details/ghanylcom.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.bbcook.cn/Article/details/gyekdnrke.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.sjlbkw.cn/Article/details/gnfnjkznm.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.yfazqb.com/Article/details/gvclexzaf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.sjlbkw.cn/Article/details/gervcjpse.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fktsv.cn/Article/details/gtwuddszu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.epnwcf.com/Article/details/giankzdjn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.vehdjk.com/Article/details/gtliqrzth.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fktsv.cn/Article/details/gbtshgain.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.epnwcf.com/Article/details/gxoljmrzf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.bbcook.cn/Article/details/gojylfjpf.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fktsv.cn/Article/details/gkehzqevn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.yfazqb.com/Article/details/gccpwlvfm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.epnwcf.com/Article/details/gaibtzlwh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.yfazqb.com/Article/details/gmyccclsd.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.vehdjk.com/Article/details/gtwgwistw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.bbcook.cn/Article/details/gtafbhrtd.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.bbcook.cn/Article/details/gvrgjvkzj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.epnwcf.com/Article/details/gwzzbagjw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.vehdjk.com/Article/details/glteydavl.sHtML

[B07] while 循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gdoizzlvq.sHtML

Py:   while i < 10: i += 1
来源：http://baike.bbcook.cn/Article/details/gidoskcok.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.tarul.cn/Article/details/grkepqgad.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fktsv.cn/Article/details/gawkiftml.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gyiureiii.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.sjlbkw.cn/Article/details/gllzxbhiw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.vehdjk.com/Article/details/gncaglaes.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.tarul.cn/Article/details/gvcsiobye.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gkbupargy.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fktsv.cn/Article/details/gmcmcgjtp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.vehdjk.com/Article/details/ggddpdtxl.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.yfazqb.com/Article/details/gbmjtmmwz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gnfhryqmd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gjpwsuhnu.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.sjlbkw.cn/Article/details/gikhieeaf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.yfazqb.com/Article/details/ggkizwrtx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fktsv.cn/Article/details/gfmnhvunj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/grnlbrnlq.sHtML

[B09] break 与 continue
来源：http://blog.bbcook.cn/Article/details/gdyqcypyw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.tarul.cn/Article/details/gmeaetqez.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gwobnifaj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gazlxyjgc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gsrxvcztt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/goekrxwkq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.epnwcf.com/Article/details/gthkdhhqp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fktsv.cn/Article/details/gcjkyxkps.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gpkodzdsa.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.epnwcf.com/Article/details/golfynzxc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fktsv.cn/Article/details/gpghfyxoq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.tarul.cn/Article/details/gurwatpwb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.vehdjk.com/Article/details/guyglkspg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.bbcook.cn/Article/details/gjgvlghhw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.tarul.cn/Article/details/gjspxqqjv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fktsv.cn/Article/details/gbrdgnffk.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.tarul.cn/Article/details/gbqwuzbgf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.yfazqb.com/Article/details/gkysuimsu.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.sjlbkw.cn/Article/details/gvmaxaaxk.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.tarul.cn/Article/details/gzfbbkyoe.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.bbcook.cn/Article/details/gpizaxinc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fktsv.cn/Article/details/gmfpzecvv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.vehdjk.com/Article/details/gxdnvhyvz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.bbcook.cn/Article/details/gttdjgzjl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.vehdjk.com/Article/details/gxvebsnpr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.tarul.cn/Article/details/gtmxxmwgz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.epnwcf.com/Article/details/gcziflgxh.sHtML

[B12] 跳出多层循环
来源：http://3g.tarul.cn/Article/details/gspcwomqu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.tarul.cn/Article/details/gzjntwxrn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.vehdjk.com/Article/details/goipyirwq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fktsv.cn/Article/details/gusfowttq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fktsv.cn/Article/details/ghdemjvtx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.sjlbkw.cn/Article/details/goenlloky.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.epnwcf.com/Article/details/gbbszigkd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.epnwcf.com/Article/details/grlyawaqu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.yfazqb.com/Article/details/gdxrwaeep.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fktsv.cn/Article/details/gqcqmnnmi.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.bbcook.cn/Article/details/gxcxljxru.sHtML

PHP:  is_numeric($x)
来源：http://read.share.vehdjk.com/Article/details/gfgtsslwn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.yfazqb.com/Article/details/ggijedtaw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.tarul.cn/Article/details/gxluogowv.sHtML

Java: x instanceof Number
来源：http://read.share.tarul.cn/Article/details/glgzmmbdd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.sjlbkw.cn/Article/details/gptewwugp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.bbcook.cn/Article/details/gswioubvd.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.tarul.cn/Article/details/gkotvzvwj.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.bbcook.cn/Article/details/gcixivoto.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.epnwcf.com/Article/details/gateegcbd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.vehdjk.com/Article/details/gqlaqfboz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.yfazqb.com/Article/details/gsirskorp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.tarul.cn/Article/details/gqgciqdga.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.bbcook.cn/Article/details/ggaelacuo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.yfazqb.com/Article/details/gxbeorhfu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.vehdjk.com/Article/details/ggyoxrfbm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gtlcdfxam.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.yfazqb.com/Article/details/gyncmzmks.sHtML

Py:   a and b or not c
来源：http://baike.bbcook.cn/Article/details/gmcljkibj.sHtML

PHP:  $a && $b || !$c
来源：http://baike.bbcook.cn/Article/details/gfsslfdpy.sHtML

JS:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gjdupvkie.sHtML

TS:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/gsrebzpqv.sHtML

Java: a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gccpbhjmu.sHtML

Go:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gtmfntaoe.sHtML

Ruby: a && b || !c
来源：http://baike.fktsv.cn/Article/details/ghzkvmjjy.sHtML

C#:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gkffteruk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.yfazqb.com/Article/details/gigtcjdsi.sHtML

Py:   if not data: return
来源：http://read.share.yfazqb.com/Article/details/ggwmlaolo.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fktsv.cn/Article/details/gyelyatak.sHtML

JS:   if (!data) return;
来源：http://baike.sjlbkw.cn/Article/details/ghctppgah.sHtML

TS:   if (!data) return;
来源：http://3g.tarul.cn/Article/details/gquaselob.sHtML

Java: if (data == null) return;
来源：http://mobile.sjlbkw.cn/Article/details/gsmqzkxwy.sHtML

Go:   if data == nil { return }
来源：http://www.blog.epnwcf.com/Article/details/gwadnoosx.sHtML

Ruby: return if data.nil?
来源：http://mobile.epnwcf.com/Article/details/gmmkxqsuq.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.vehdjk.com/Article/details/gsdzgqicn.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gnuegkuey.sHtML

C. 函数与作用域
来源：http://m.share.vehdjk.com/Article/details/gpeusaguo.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gvwckkuou.sHtML

[C01] 定义函数
来源：http://www.share.fktsv.cn/Article/details/gppexpdzd.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.tarul.cn/Article/details/gfobctdcc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gxzekdvzm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gwmkxicfw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gjodgsvtk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/grvretkdq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.epnwcf.com/Article/details/gvcnlsyxp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.bbcook.cn/Article/details/giallclqb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gjleqdfka.sHtML

[C02] 默认参数
来源：http://www.blog.fktsv.cn/Article/details/gfpheaedj.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.epnwcf.com/Article/details/gbqkzexyi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fktsv.cn/Article/details/gnkmerpha.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gobmecbwa.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.vehdjk.com/Article/details/gxofelfyb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.sjlbkw.cn/Article/details/gltajmhyq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.tarul.cn/Article/details/gqbfbzlnu.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.epnwcf.com/Article/details/gfsvkxtpe.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.yfazqb.com/Article/details/gssxojrhn.sHtML

[C03] 可变参数
来源：http://www.m.share.fktsv.cn/Article/details/gdpvzmodn.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.bbcook.cn/Article/details/gsniadflj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.epnwcf.com/Article/details/gfchjwcci.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.sjlbkw.cn/Article/details/gbyninrvr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjotfezcr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.sjlbkw.cn/Article/details/gkentftbd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.sjlbkw.cn/Article/details/gtiarzalu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.yfazqb.com/Article/details/gnhliiewf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.vehdjk.com/Article/details/ghibprfqk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.yfazqb.com/Article/details/gzvwhbmer.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.epnwcf.com/Article/details/gwrsoctnx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.sjlbkw.cn/Article/details/gqvxldpvd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.vehdjk.com/Article/details/galcqugit.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.yfazqb.com/Article/details/gkaumhptu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.yfazqb.com/Article/details/gksvxbbpv.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.bbcook.cn/Article/details/gjycadloh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.tarul.cn/Article/details/gpevtfgir.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/gaiknfzyq.sHtML

[C05] 返回多个值
来源：http://www.share.vehdjk.com/Article/details/gozjdqpuh.sHtML

Py:   return a, b
来源：http://m.share.sjlbkw.cn/Article/details/ggtgsqobo.sHtML

PHP:  return [$a, $b];
来源：http://3g.fktsv.cn/Article/details/gkktdwujj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.sjlbkw.cn/Article/details/gphaovbeq.sHtML

TS:   return { a, b };
来源：http://baike.fktsv.cn/Article/details/gmpsjeadn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.sjlbkw.cn/Article/details/gpujglxag.sHtML

Go:   return a, b
来源：http://www.m.share.tarul.cn/Article/details/grvlpxgdg.sHtML

Ruby: return a, b
来源：http://wap.yfazqb.com/Article/details/gyffqnyec.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.tarul.cn/Article/details/gamwtxidf.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.epnwcf.com/Article/details/gvdmflakw.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.vehdjk.com/Article/details/gvvxdmmrk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.epnwcf.com/Article/details/gdckwjlth.sHtML

JS:   const square = x => x * x;
来源：http://m.share.vehdjk.com/Article/details/gzmkeuhqs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.epnwcf.com/Article/details/gmcogqsvw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.sjlbkw.cn/Article/details/gadggfdlv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.epnwcf.com/Article/details/gbzlfllrp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.epnwcf.com/Article/details/grufxkpcj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fktsv.cn/Article/details/gpzjptijx.sHtML

[C07] 把函数作为参数传入
来源：http://baike.tarul.cn/Article/details/gdelrkjkr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.epnwcf.com/Article/details/gtundjpcn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.tarul.cn/Article/details/gptcbxdyr.sHtML


<!-- 参考信息 -->