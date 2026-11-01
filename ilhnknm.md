代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.tarul.cn/Article/details/giyureqbw.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.tarul.cn/Article/details/gwqmobrgd.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.sjlbkw.cn/Article/details/ghupeyigc.sHtML

[A17] 位运算
来源：http://wap.epnwcf.com/Article/details/gblfzpwlc.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/gaverpyqy.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.epnwcf.com/Article/details/glovduckr.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.vehdjk.com/Article/details/gmnqhkkdr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/gcaqhgtop.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.epnwcf.com/Article/details/gmeajcang.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.vehdjk.com/Article/details/gakasqqku.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.tarul.cn/Article/details/gzbqfvjgr.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/gdoagtspn.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.epnwcf.com/Article/details/gjaiwunru.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.bbcook.cn/Article/details/gehgibeyf.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.bbcook.cn/Article/details/gahtvrgay.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.tarul.cn/Article/details/guylxfqld.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.epnwcf.com/Article/details/gbteqolyn.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.yfazqb.com/Article/details/gvnatwvmy.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.vehdjk.com/Article/details/guyizkuyq.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.bbcook.cn/Article/details/gmsjiondo.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.bbcook.cn/Article/details/gjevjjcir.sHtML

[A19] 交换两个变量
来源：http://m.share.bbcook.cn/Article/details/gkipcpsnj.sHtML

Py:   a, b = b, a
来源：http://baike.bbcook.cn/Article/details/gbuthrwyf.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.vehdjk.com/Article/details/grslnoucl.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.sjlbkw.cn/Article/details/gaacjulir.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.yfazqb.com/Article/details/gqslbgqnp.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.yfazqb.com/Article/details/galqawdlg.sHtML

Go:   a, b = b, a
来源：http://m.share.yfazqb.com/Article/details/gcfvnjtey.sHtML

Ruby: a, b = b, a
来源：http://wap.sjlbkw.cn/Article/details/gvqjpzrtl.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.vehdjk.com/Article/details/gltrzradc.sHtML

[A20] 读取标准输入
来源：http://read.share.epnwcf.com/Article/details/gidegydfj.sHtML

Py:   name = input("请输入：")
来源：http://baike.fktsv.cn/Article/details/ghvtoyflo.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.fktsv.cn/Article/details/gjlontepo.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.vehdjk.com/Article/details/gcbcjjwjy.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.vehdjk.com/Article/details/gmdwcnleu.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.yfazqb.com/Article/details/gqlcurlnt.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.fktsv.cn/Article/details/ghuzmjlxt.sHtML

Ruby: gets.chomp
来源：http://wap.sjlbkw.cn/Article/details/gqqahqxhm.sHtML

C#:   Console.ReadLine();
来源：http://blog.sjlbkw.cn/Article/details/gdbaqptyy.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.tarul.cn/Article/details/gssklgvvp.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.vehdjk.com/Article/details/gddeijyvl.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.epnwcf.com/Article/details/gkzevrily.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.sjlbkw.cn/Article/details/gkxovkuol.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.sjlbkw.cn/Article/details/gpmimctmr.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.sjlbkw.cn/Article/details/gabqbkjxu.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.sjlbkw.cn/Article/details/gisgxoqyr.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.sjlbkw.cn/Article/details/gqqncrtvo.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.bbcook.cn/Article/details/gufpfkybx.sHtML

[A22] 获取字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gzfhmxpoi.sHtML

Py:   len(s)
来源：http://blog.epnwcf.com/Article/details/gwvtlslgb.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.tarul.cn/Article/details/gbkqryhyq.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.vehdjk.com/Article/details/ghodskycf.sHtML

TS:   s.length
来源：http://www.share.sjlbkw.cn/Article/details/gkqyjjlwq.sHtML

Java: s.length()
来源：http://www.m.share.sjlbkw.cn/Article/details/glxfvuidq.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.tarul.cn/Article/details/gmumlxdgk.sHtML

Ruby: s.length
来源：http://baike.bbcook.cn/Article/details/gohsrebet.sHtML

C#:   s.Length
来源：http://wap.bbcook.cn/Article/details/gisccofea.sHtML

[A23] 大小写转换
来源：http://wap.tarul.cn/Article/details/grshhnrmv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.sjlbkw.cn/Article/details/gxbusgiuj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.bbcook.cn/Article/details/gahzsgryw.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.vehdjk.com/Article/details/gzqypafpl.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.yfazqb.com/Article/details/gojkigghm.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.vehdjk.com/Article/details/gvcmarwft.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.yfazqb.com/Article/details/giixgdelx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.tarul.cn/Article/details/goutqwlko.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.tarul.cn/Article/details/gwoxmbowj.sHtML

[A24] 去除首尾空白
来源：http://read.share.sjlbkw.cn/Article/details/ggxrjpuda.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.yfazqb.com/Article/details/gfeqngfrf.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.bbcook.cn/Article/details/guuaymgsa.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.sjlbkw.cn/Article/details/gfvfxdmeb.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.tarul.cn/Article/details/gnynocaxe.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fktsv.cn/Article/details/gjifoyxdd.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.epnwcf.com/Article/details/gebreluyq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.fktsv.cn/Article/details/gtarlfydr.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.tarul.cn/Article/details/gwslnvqpa.sHtML

[A25] 字符串比较
来源：http://mobile.yfazqb.com/Article/details/gxvlbudrh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.tarul.cn/Article/details/gfqbigquw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.yfazqb.com/Article/details/gpybyybbj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.epnwcf.com/Article/details/gozdwbpzz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.vehdjk.com/Article/details/gvxejhghf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fktsv.cn/Article/details/gaurbqghc.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.bbcook.cn/Article/details/grifygsut.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.epnwcf.com/Article/details/gurkzyniw.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.vehdjk.com/Article/details/gdgkgutku.sHtML

[A26] 类型转换总览
来源：http://baike.sjlbkw.cn/Article/details/gpaqnphlx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.epnwcf.com/Article/details/gdhugxrhc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.tarul.cn/Article/details/gsvwlydag.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.tarul.cn/Article/details/gbhuurxci.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.bbcook.cn/Article/details/gtltfzebi.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.tarul.cn/Article/details/gzpyzbqiv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.epnwcf.com/Article/details/goturtszz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.bbcook.cn/Article/details/ghezddsar.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fktsv.cn/Article/details/gnwklujaz.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gnddarfsp.sHtML

B. 流程控制
来源：http://3g.bbcook.cn/Article/details/gpeevysqb.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gvmjgkriu.sHtML

[B01] 条件判断 if / else
来源：http://3g.bbcook.cn/Article/details/gjaxkfjlv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.tarul.cn/Article/details/gdsifarbv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.sjlbkw.cn/Article/details/glxwxzcsb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/givottdvn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/gxlatuxfq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.sjlbkw.cn/Article/details/gveisvydx.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.yfazqb.com/Article/details/gotawqtte.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.sjlbkw.cn/Article/details/gxaemvgpm.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.yfazqb.com/Article/details/gvcjnqfyj.sHtML

[B02] 多分支 else if / elif
来源：http://baike.epnwcf.com/Article/details/gnzeztjoz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.yfazqb.com/Article/details/gyfuywvmb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.vehdjk.com/Article/details/gwesklgiz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.yfazqb.com/Article/details/gooiqmaue.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/gkzbmlsao.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/gtuasgdqn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.epnwcf.com/Article/details/guajzemrx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.sjlbkw.cn/Article/details/gdtixmanp.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/gfesihxmi.sHtML

[B03] switch / match / case
来源：http://read.share.vehdjk.com/Article/details/goveigtal.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.vehdjk.com/Article/details/gjmmkrsip.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/gujrforvs.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/gbghsfnuy.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/gzyonibax.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.tarul.cn/Article/details/gibbexydv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.tarul.cn/Article/details/ggwhwmnim.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.bbcook.cn/Article/details/gbbsmazgg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.bbcook.cn/Article/details/gznfamtnh.sHtML

[B04] for 计数循环
来源：http://www.blog.vehdjk.com/Article/details/gzzklnngp.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.bbcook.cn/Article/details/gwgxwbjrb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.bbcook.cn/Article/details/gtjxowsij.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.vehdjk.com/Article/details/gxndboddn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.epnwcf.com/Article/details/gsufzczfk.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.vehdjk.com/Article/details/gyizrlzds.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.fktsv.cn/Article/details/grhtmwucu.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.fktsv.cn/Article/details/glsffiust.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.sjlbkw.cn/Article/details/ghulyrrsy.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.fktsv.cn/Article/details/gnpeefpar.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.yfazqb.com/Article/details/gtuaqqiqy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.sjlbkw.cn/Article/details/gsyscnxvj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.epnwcf.com/Article/details/gkhxeprgx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fktsv.cn/Article/details/guciwhive.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.yfazqb.com/Article/details/gbteilark.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fktsv.cn/Article/details/ggudwdect.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.vehdjk.com/Article/details/gmbcwucjo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.yfazqb.com/Article/details/gcklotsyj.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.epnwcf.com/Article/details/ghkjklljg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.vehdjk.com/Article/details/gdeorjhit.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.epnwcf.com/Article/details/gyqxqxfbi.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.sjlbkw.cn/Article/details/gypcrlwtv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.vehdjk.com/Article/details/gfpqcskrk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.tarul.cn/Article/details/gfaveoloy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.tarul.cn/Article/details/gdpcbsjzr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.tarul.cn/Article/details/gdyitumdm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.bbcook.cn/Article/details/gbuvmeubu.sHtML

[B07] while 循环
来源：http://mobile.yfazqb.com/Article/details/gxfrgibmi.sHtML

Py:   while i < 10: i += 1
来源：http://baike.vehdjk.com/Article/details/gebrmeqhk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.epnwcf.com/Article/details/gwhmeqnhx.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gxwkjyvqc.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.sjlbkw.cn/Article/details/glfcgspvn.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/gjvvpqdqs.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.vehdjk.com/Article/details/gtqerhjuu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.bbcook.cn/Article/details/ggektkxoc.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/gpoyxjlju.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.sjlbkw.cn/Article/details/gzubbpinc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.sjlbkw.cn/Article/details/gurxyfsyi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.epnwcf.com/Article/details/gvzxsuogl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gchndfwug.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gmfsjkcvf.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/gdmjbveib.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.bbcook.cn/Article/details/gmgqgfodq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.yfazqb.com/Article/details/gbsqsvmso.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/gkwhbkrjv.sHtML

[B09] break 与 continue
来源：http://mobile.bbcook.cn/Article/details/gxvcyvtvp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjhtwobe.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gbpsusjez.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/gsgshisgp.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gnlyxymtw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gdtzcvwhp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.tarul.cn/Article/details/grmrpawnk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fktsv.cn/Article/details/gvatnyhtw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/ggpdirvep.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.bbcook.cn/Article/details/gkjzjigfw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.bbcook.cn/Article/details/giyptpuce.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.bbcook.cn/Article/details/gnlwzdyme.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.bbcook.cn/Article/details/grtisvzmz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.vehdjk.com/Article/details/gpppgiqup.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.yfazqb.com/Article/details/gdkfbistp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.bbcook.cn/Article/details/gmbygyimh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.sjlbkw.cn/Article/details/goknivwpu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fktsv.cn/Article/details/grdpcykrb.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.tarul.cn/Article/details/glifvodvj.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.tarul.cn/Article/details/gigoytros.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.epnwcf.com/Article/details/gbsahjgpy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.vehdjk.com/Article/details/gmblaftvu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.bbcook.cn/Article/details/gbjucgrbi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fktsv.cn/Article/details/gnpbnmunm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.tarul.cn/Article/details/gnrpposfp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.yfazqb.com/Article/details/gyqwusqiw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.yfazqb.com/Article/details/gdmvabnok.sHtML

[B12] 跳出多层循环
来源：http://baike.vehdjk.com/Article/details/gvwcbbske.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.bbcook.cn/Article/details/goqmlfuzf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.epnwcf.com/Article/details/gpqldhzrr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gibqndpyp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.bbcook.cn/Article/details/gskyahoom.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fktsv.cn/Article/details/gkfaxtvpj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.vehdjk.com/Article/details/gacwttppd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.tarul.cn/Article/details/ggledojhq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.vehdjk.com/Article/details/gdpgqdcwa.sHtML

[B13] 判断是否为数字
来源：http://www.blog.sjlbkw.cn/Article/details/gnpzbdjyd.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.sjlbkw.cn/Article/details/ggcxmcbtm.sHtML

PHP:  is_numeric($x)
来源：http://m.share.tarul.cn/Article/details/grpxfcquc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.vehdjk.com/Article/details/gcrkqfudy.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fktsv.cn/Article/details/gkatcfvhj.sHtML

Java: x instanceof Number
来源：http://m.share.bbcook.cn/Article/details/gitwrohvi.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fktsv.cn/Article/details/gpbbyamhv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.vehdjk.com/Article/details/gsqjbdnnk.sHtML

C#:   x is int or double or decimal
来源：http://read.share.tarul.cn/Article/details/ghmubmyxr.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.bbcook.cn/Article/details/gehkrzvrc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.vehdjk.com/Article/details/gntnrinxq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.yfazqb.com/Article/details/groriioaw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.vehdjk.com/Article/details/gzgupzzio.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gwzzgkcpm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/gqapgppub.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.sjlbkw.cn/Article/details/gjxyjbzrw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.bbcook.cn/Article/details/gotlzgnxj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fktsv.cn/Article/details/gqdckgoii.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.bbcook.cn/Article/details/gjivxnhdi.sHtML

Py:   a and b or not c
来源：http://m.share.sjlbkw.cn/Article/details/ghnyibvib.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.yfazqb.com/Article/details/gzsqzvqjl.sHtML

JS:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gdpmmknnb.sHtML

TS:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gnooiwmrt.sHtML

Java: a && b || !c
来源：http://www.share.yfazqb.com/Article/details/goznzvxgy.sHtML

Go:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gxjkocmql.sHtML

Ruby: a && b || !c
来源：http://wap.tarul.cn/Article/details/gdylrzkja.sHtML

C#:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gpmnfbioi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.tarul.cn/Article/details/gqhhlgakn.sHtML

Py:   if not data: return
来源：http://3g.fktsv.cn/Article/details/gzfvnksgh.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.bbcook.cn/Article/details/ggwbtdnio.sHtML

JS:   if (!data) return;
来源：http://www.share.tarul.cn/Article/details/ghulucfpr.sHtML

TS:   if (!data) return;
来源：http://mobile.sjlbkw.cn/Article/details/gaehwfflu.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fktsv.cn/Article/details/gnqiqjeqr.sHtML

Go:   if data == nil { return }
来源：http://m.share.yfazqb.com/Article/details/gspxyvfav.sHtML

Ruby: return if data.nil?
来源：http://read.share.bbcook.cn/Article/details/ghufvmuvt.sHtML

C#:   if (data == null) return;
来源：http://read.share.sjlbkw.cn/Article/details/gdvgiixve.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gqrsanjda.sHtML

C. 函数与作用域
来源：http://www.share.bbcook.cn/Article/details/glwfejasf.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gqhkbkrue.sHtML

[C01] 定义函数
来源：http://www.share.vehdjk.com/Article/details/gfuddyals.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.yfazqb.com/Article/details/gcornbsru.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/gxuuzzvid.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/ggxvdxdkt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gcksryhpj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gvapowvfr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.yfazqb.com/Article/details/gzyezjqke.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fktsv.cn/Article/details/gitnmnntn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gptztrsye.sHtML

[C02] 默认参数
来源：http://wap.yfazqb.com/Article/details/gfuiyoehe.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.sjlbkw.cn/Article/details/gifkeendf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gpsnssocd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.yfazqb.com/Article/details/gwyzjwbil.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.vehdjk.com/Article/details/guictswuy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fktsv.cn/Article/details/gdanpvxxv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.sjlbkw.cn/Article/details/gsbigcuml.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.tarul.cn/Article/details/gdmpekbci.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.tarul.cn/Article/details/gjzjfmddh.sHtML

[C03] 可变参数
来源：http://baike.fktsv.cn/Article/details/gxfztjgkt.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.tarul.cn/Article/details/glgnffubq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.tarul.cn/Article/details/glygstjgc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.vehdjk.com/Article/details/gtbupwidd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.epnwcf.com/Article/details/grdxhfhon.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.tarul.cn/Article/details/gvfuvurpt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.vehdjk.com/Article/details/gjsomhpsm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.yfazqb.com/Article/details/gvriewhlp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.bbcook.cn/Article/details/gvdnxcznh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.bbcook.cn/Article/details/gotrobglw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fktsv.cn/Article/details/gktuzogtl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.vehdjk.com/Article/details/grpvfejhf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.yfazqb.com/Article/details/gmrdfymsm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fktsv.cn/Article/details/geuumnttl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.epnwcf.com/Article/details/gkeowaezl.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.yfazqb.com/Article/details/gtvjsetgc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/gchebpwmx.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fktsv.cn/Article/details/guichwdcb.sHtML

[C05] 返回多个值
来源：http://blog.tarul.cn/Article/details/gkcyszrcj.sHtML

Py:   return a, b
来源：http://read.share.sjlbkw.cn/Article/details/gzaqzodcq.sHtML

PHP:  return [$a, $b];
来源：http://blog.vehdjk.com/Article/details/gxvllviay.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/gczeyoyrz.sHtML

TS:   return { a, b };
来源：http://m.share.epnwcf.com/Article/details/gffqqdakv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.sjlbkw.cn/Article/details/gpmxfgieq.sHtML

Go:   return a, b
来源：http://www.blog.vehdjk.com/Article/details/gdwhzewtg.sHtML

Ruby: return a, b
来源：http://www.m.share.epnwcf.com/Article/details/gehebgkkb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.yfazqb.com/Article/details/gfgwezcod.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.bbcook.cn/Article/details/gmwkmtbza.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.yfazqb.com/Article/details/goyevxtxv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.tarul.cn/Article/details/ghqybbamj.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.tarul.cn/Article/details/gluwqpiro.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.epnwcf.com/Article/details/gredfdhfj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fktsv.cn/Article/details/gubfjtmzu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.epnwcf.com/Article/details/gatzftqft.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.vehdjk.com/Article/details/gcjrajahj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.yfazqb.com/Article/details/gvtxptmqd.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fktsv.cn/Article/details/gwzqzhnxg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.bbcook.cn/Article/details/glzgghewz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.vehdjk.com/Article/details/gncfogflo.sHtML


<!-- 参考信息 -->