代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://3g.fktsv.cn/Article/details/gsachrvur.sHtML

[A15] 空值判断与默认值
来源：http://m.share.sjlbkw.cn/Article/details/goibdzfgm.sHtML

Py:   value = data or "默认值"
来源：http://mobile.epnwcf.com/Article/details/gjutfwylz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.yfazqb.com/Article/details/gmuakgvhv.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.sjlbkw.cn/Article/details/gpdkbafoi.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.sjlbkw.cn/Article/details/gxzhisupx.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.vehdjk.com/Article/details/gwzvokoap.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.vehdjk.com/Article/details/gzveheyne.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.yfazqb.com/Article/details/glafnlwgw.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.bbcook.cn/Article/details/gbqmxtipq.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.bbcook.cn/Article/details/guypkzpuf.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.bbcook.cn/Article/details/gklislhvt.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.fktsv.cn/Article/details/glenyymng.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.bbcook.cn/Article/details/gyhcdrylo.sHtML

TS:   if (!x) {}
来源：http://www.blog.bbcook.cn/Article/details/gxmdgmjoe.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.tarul.cn/Article/details/gfrlfmgwy.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.sjlbkw.cn/Article/details/gmjfxzyma.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.bbcook.cn/Article/details/gdquzgwme.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.vehdjk.com/Article/details/gjiwtfigd.sHtML

[A17] 位运算
来源：http://wap.epnwcf.com/Article/details/ggvfihwmw.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/gfqysqwzv.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.yfazqb.com/Article/details/gtqghjbvk.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.vehdjk.com/Article/details/grkonnimn.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.bbcook.cn/Article/details/ggzelljwg.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/gqhteyusl.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.epnwcf.com/Article/details/gbredfflb.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fktsv.cn/Article/details/gywgqvdje.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.epnwcf.com/Article/details/guwjzapfr.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.bbcook.cn/Article/details/gxwhwrvjb.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.vehdjk.com/Article/details/goflyvgea.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.bbcook.cn/Article/details/gjtfztnbh.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.bbcook.cn/Article/details/gsahhjtpn.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.tarul.cn/Article/details/gwoyxyfzf.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.vehdjk.com/Article/details/ggmwvckse.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.tarul.cn/Article/details/gfdvxbmxb.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.vehdjk.com/Article/details/gldxixtsc.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.yfazqb.com/Article/details/gbngeukee.sHtML

[A19] 交换两个变量
来源：http://3g.tarul.cn/Article/details/gtfximcvv.sHtML

Py:   a, b = b, a
来源：http://www.m.share.fktsv.cn/Article/details/gvdxqgpog.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.sjlbkw.cn/Article/details/ghyybvmqv.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.vehdjk.com/Article/details/gjinukgln.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.sjlbkw.cn/Article/details/gttwipuht.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.vehdjk.com/Article/details/gicqknyrx.sHtML

Go:   a, b = b, a
来源：http://www.blog.tarul.cn/Article/details/gqxwldicf.sHtML

Ruby: a, b = b, a
来源：http://blog.bbcook.cn/Article/details/gspwucpew.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.yfazqb.com/Article/details/gdrnygvoj.sHtML

[A20] 读取标准输入
来源：http://baike.bbcook.cn/Article/details/gglwlteir.sHtML

Py:   name = input("请输入：")
来源：http://www.share.tarul.cn/Article/details/gtuybhgsh.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.vehdjk.com/Article/details/gvrmuwvzc.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.sjlbkw.cn/Article/details/glbpmdfub.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.bbcook.cn/Article/details/gnecfgsze.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.fktsv.cn/Article/details/geymjjbtg.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.bbcook.cn/Article/details/goppotkqf.sHtML

Ruby: gets.chomp
来源：http://baike.fktsv.cn/Article/details/gdlhqyxzu.sHtML

C#:   Console.ReadLine();
来源：http://m.share.sjlbkw.cn/Article/details/gitsufscq.sHtML

[A21] 保留指定小数位输出
来源：http://baike.fktsv.cn/Article/details/gxrrmdzer.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.vehdjk.com/Article/details/gpubrmfoq.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.tarul.cn/Article/details/gjurqtwhu.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.epnwcf.com/Article/details/golrenuti.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.sjlbkw.cn/Article/details/glbmckdfo.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.yfazqb.com/Article/details/gqxspzkeq.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.yfazqb.com/Article/details/gsksyxxao.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.yfazqb.com/Article/details/gepnplmlw.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.tarul.cn/Article/details/gyakwxokk.sHtML

[A22] 获取字符串长度
来源：http://wap.fktsv.cn/Article/details/gfmjnyjkf.sHtML

Py:   len(s)
来源：http://mobile.tarul.cn/Article/details/gqftfivtc.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.vehdjk.com/Article/details/gzdibylzr.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.fktsv.cn/Article/details/gdrvlsavt.sHtML

TS:   s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gmwojhpes.sHtML

Java: s.length()
来源：http://3g.tarul.cn/Article/details/ghfcjfosf.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.yfazqb.com/Article/details/gzfhyhhlm.sHtML

Ruby: s.length
来源：http://read.share.epnwcf.com/Article/details/gqlcxpxui.sHtML

C#:   s.Length
来源：http://mobile.epnwcf.com/Article/details/gmdeorica.sHtML

[A23] 大小写转换
来源：http://wap.tarul.cn/Article/details/gikichtch.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.yfazqb.com/Article/details/gwyexvnfr.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.bbcook.cn/Article/details/gavofagkz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.epnwcf.com/Article/details/giummvfee.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.tarul.cn/Article/details/gitixtumk.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.vehdjk.com/Article/details/gsuqlpvkg.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.bbcook.cn/Article/details/gouplxefc.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.epnwcf.com/Article/details/gczabbiau.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.bbcook.cn/Article/details/gtohvzcgq.sHtML

[A24] 去除首尾空白
来源：http://mobile.tarul.cn/Article/details/gmbwqjtrm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.fktsv.cn/Article/details/gimgaawxg.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.tarul.cn/Article/details/gvezzetpw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.epnwcf.com/Article/details/geiizfwvu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.bbcook.cn/Article/details/gpruotbik.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.bbcook.cn/Article/details/gthhmpnxj.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.bbcook.cn/Article/details/gtivmmyjj.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.vehdjk.com/Article/details/ggekudhac.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.tarul.cn/Article/details/gwdcgbyza.sHtML

[A25] 字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/gtnspdrfq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.tarul.cn/Article/details/gklqlpmlo.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.bbcook.cn/Article/details/gawrjwean.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.tarul.cn/Article/details/gvilaqmas.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.vehdjk.com/Article/details/gxjkunmqh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.vehdjk.com/Article/details/guxrwtbky.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.sjlbkw.cn/Article/details/gglmcfksh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.bbcook.cn/Article/details/ghtiwwmfb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.bbcook.cn/Article/details/gvwqmjofw.sHtML

[A26] 类型转换总览
来源：http://3g.bbcook.cn/Article/details/grghqblny.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.vehdjk.com/Article/details/gblcxxavi.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.epnwcf.com/Article/details/gyujmzfpr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.bbcook.cn/Article/details/gnqekiexz.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.tarul.cn/Article/details/grsfyygxx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.tarul.cn/Article/details/gqzgobbfr.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.vehdjk.com/Article/details/grvsblpsz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.bbcook.cn/Article/details/gokooadsv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.fktsv.cn/Article/details/goklfjkkh.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gwsuregaq.sHtML

B. 流程控制
来源：http://www.m.share.epnwcf.com/Article/details/gmxfkacrh.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/ggdzlgnqj.sHtML

[B01] 条件判断 if / else
来源：http://www.share.bbcook.cn/Article/details/gkkktwkeb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.epnwcf.com/Article/details/gbtkgicrj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.vehdjk.com/Article/details/ggcjasfqw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.yfazqb.com/Article/details/goqcdgfbq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.sjlbkw.cn/Article/details/goticogiq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/gerlgwzms.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.fktsv.cn/Article/details/gwsqxmygy.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.fktsv.cn/Article/details/grvteijlt.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/gyyaqypoh.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.fktsv.cn/Article/details/gjjxaztge.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.yfazqb.com/Article/details/gahfawqrn.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.bbcook.cn/Article/details/gxbuqfhjl.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/gcglmzgog.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.bbcook.cn/Article/details/gbyniaxoa.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.tarul.cn/Article/details/gxuspiown.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.yfazqb.com/Article/details/gicuathbj.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.vehdjk.com/Article/details/ghsrtsqsa.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/grbavgjri.sHtML

[B03] switch / match / case
来源：http://baike.tarul.cn/Article/details/gorohgugx.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.bbcook.cn/Article/details/gyffgwrbf.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/gggkkhdlj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.tarul.cn/Article/details/gsmxchjcp.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gbnigbfpq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.yfazqb.com/Article/details/ggvucotjn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.epnwcf.com/Article/details/gsnlhqrpu.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.sjlbkw.cn/Article/details/gnscsvels.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.tarul.cn/Article/details/ggmxrcbrf.sHtML

[B04] for 计数循环
来源：http://baike.vehdjk.com/Article/details/gnntuybre.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.sjlbkw.cn/Article/details/gffwntety.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.bbcook.cn/Article/details/gfjdlkseu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.epnwcf.com/Article/details/grfxoqzvh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.sjlbkw.cn/Article/details/gdpetrotu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.sjlbkw.cn/Article/details/ggargtiec.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.bbcook.cn/Article/details/gfbhmrpun.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.yfazqb.com/Article/details/ghiwkvsgw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.yfazqb.com/Article/details/gqxzjgmdu.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.vehdjk.com/Article/details/gherpkejr.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjufgnqg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.epnwcf.com/Article/details/gtfoyydse.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.sjlbkw.cn/Article/details/ghghafazg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.sjlbkw.cn/Article/details/guuxwuxlx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.bbcook.cn/Article/details/gpftlwwvg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.sjlbkw.cn/Article/details/grzywdjyl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.sjlbkw.cn/Article/details/gttzuvuhz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.yfazqb.com/Article/details/gfduhxulh.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.yfazqb.com/Article/details/giyqiayhw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.sjlbkw.cn/Article/details/gzglobfwk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.bbcook.cn/Article/details/gakyucyyk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.tarul.cn/Article/details/gmuitmhkf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fktsv.cn/Article/details/gfkrzzboq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.bbcook.cn/Article/details/gwijwufgz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.epnwcf.com/Article/details/gvcmkjajo.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.bbcook.cn/Article/details/gmqzhkhar.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.sjlbkw.cn/Article/details/gknurlvub.sHtML

[B07] while 循环
来源：http://blog.sjlbkw.cn/Article/details/grfqaeijs.sHtML

Py:   while i < 10: i += 1
来源：http://blog.vehdjk.com/Article/details/gcsibxtoc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.sjlbkw.cn/Article/details/gzyeqsyco.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/ghwmxsssp.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/gkbykhtpu.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/grlmqjqmx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fktsv.cn/Article/details/gbwhqngrj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.tarul.cn/Article/details/gfjlpjuui.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/gocuknscs.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.tarul.cn/Article/details/gsderxkny.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.sjlbkw.cn/Article/details/gltugzcga.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.vehdjk.com/Article/details/gfjenenui.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/gdecokqfl.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/ganfdpfas.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gdywrqlec.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fktsv.cn/Article/details/gybzdrywz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.sjlbkw.cn/Article/details/goodoeixk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/gebyzoswg.sHtML

[B09] break 与 continue
来源：http://blog.sjlbkw.cn/Article/details/ggfuqprkf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.yfazqb.com/Article/details/gzbqdjkvl.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/gxrndeedz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gzuisuuno.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gyxdxqsut.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gmikhcspq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.yfazqb.com/Article/details/gaxabmgbk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.epnwcf.com/Article/details/gxanfzngm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gfigbgvgv.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwqbdrrw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.bbcook.cn/Article/details/gixpldsot.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.epnwcf.com/Article/details/gsysomzen.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fktsv.cn/Article/details/gumyqijzz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fktsv.cn/Article/details/gmeeghqmo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.vehdjk.com/Article/details/ghmwcwkdd.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.tarul.cn/Article/details/gmvsrndkc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.vehdjk.com/Article/details/gujercljw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.sjlbkw.cn/Article/details/gjfpfanlz.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fktsv.cn/Article/details/gbcvtaymn.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.epnwcf.com/Article/details/ghvuayrng.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.sjlbkw.cn/Article/details/gxojxftft.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.vehdjk.com/Article/details/glainrjgs.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.tarul.cn/Article/details/gcnrmrylz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.vehdjk.com/Article/details/gszbjidex.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.sjlbkw.cn/Article/details/grvlvxgio.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.vehdjk.com/Article/details/gxdsmdmfm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.epnwcf.com/Article/details/ggaqgslmq.sHtML

[B12] 跳出多层循环
来源：http://3g.yfazqb.com/Article/details/gtnmqbrkq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.yfazqb.com/Article/details/gymbytxqa.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.vehdjk.com/Article/details/gzlplocrw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.tarul.cn/Article/details/gdnrmsuga.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.epnwcf.com/Article/details/gefwlkmvv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.tarul.cn/Article/details/gfngdosjw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.tarul.cn/Article/details/gnyvkzefw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.bbcook.cn/Article/details/gapdxqpjk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.epnwcf.com/Article/details/gadosczbd.sHtML

[B13] 判断是否为数字
来源：http://read.share.vehdjk.com/Article/details/gtkxtkgrn.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.yfazqb.com/Article/details/gqbpldneb.sHtML

PHP:  is_numeric($x)
来源：http://read.share.vehdjk.com/Article/details/gxukphoxx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.epnwcf.com/Article/details/gshwuhngj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.bbcook.cn/Article/details/gvckqsqfk.sHtML

Java: x instanceof Number
来源：http://baike.sjlbkw.cn/Article/details/giambrqkd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.tarul.cn/Article/details/gavcfkbvq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fktsv.cn/Article/details/gvmmgcayk.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.vehdjk.com/Article/details/gkctrfpmf.sHtML

[B14] 判断值是否在集合内
来源：http://wap.vehdjk.com/Article/details/gyebdfiat.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.yfazqb.com/Article/details/gpjrqrwob.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.sjlbkw.cn/Article/details/gtymkzdgr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.epnwcf.com/Article/details/goltdxjma.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fktsv.cn/Article/details/groivjayu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.tarul.cn/Article/details/getqdicga.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fktsv.cn/Article/details/gmvgsjoks.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.tarul.cn/Article/details/gxbqrbuas.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.epnwcf.com/Article/details/gxedcmmih.sHtML

[B15] 布尔运算与取反
来源：http://read.share.epnwcf.com/Article/details/gcocealsx.sHtML

Py:   a and b or not c
来源：http://www.share.tarul.cn/Article/details/gfrptgeku.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.tarul.cn/Article/details/gpwxpqttt.sHtML

JS:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gyigerxxe.sHtML

TS:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gosjyklqp.sHtML

Java: a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gkfirdmus.sHtML

Go:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gfhgtlpmb.sHtML

Ruby: a && b || !c
来源：http://baike.bbcook.cn/Article/details/gpupklbwc.sHtML

C#:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/gfotugdws.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.yfazqb.com/Article/details/gswceyxua.sHtML

Py:   if not data: return
来源：http://blog.yfazqb.com/Article/details/gannhuelj.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.vehdjk.com/Article/details/gdqvrnirh.sHtML

JS:   if (!data) return;
来源：http://blog.bbcook.cn/Article/details/gcrpfxica.sHtML

TS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/ghmzkkace.sHtML

Java: if (data == null) return;
来源：http://www.blog.tarul.cn/Article/details/grzuexdli.sHtML

Go:   if data == nil { return }
来源：http://mobile.sjlbkw.cn/Article/details/gonnzcjas.sHtML

Ruby: return if data.nil?
来源：http://wap.fktsv.cn/Article/details/ggfsawimb.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.epnwcf.com/Article/details/grwacxarc.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gromydzec.sHtML

C. 函数与作用域
来源：http://blog.sjlbkw.cn/Article/details/gqssoprci.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gojckfbcx.sHtML

[C01] 定义函数
来源：http://3g.tarul.cn/Article/details/gbrnljfip.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.vehdjk.com/Article/details/gtpbrrrnf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/gxxmzcayl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gwzpqhezo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gibonfrqc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gmovendjw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.tarul.cn/Article/details/ghlpziwav.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.sjlbkw.cn/Article/details/gbvunwkln.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gxabntilx.sHtML

[C02] 默认参数
来源：http://3g.vehdjk.com/Article/details/gbrmbynsr.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.sjlbkw.cn/Article/details/ggeykstpq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fktsv.cn/Article/details/guweubara.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.vehdjk.com/Article/details/ghuujybje.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.vehdjk.com/Article/details/gcjtodpab.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fktsv.cn/Article/details/gzysdblsz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.vehdjk.com/Article/details/gljpmnuca.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.sjlbkw.cn/Article/details/gbakupztu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fktsv.cn/Article/details/ghswdfaib.sHtML

[C03] 可变参数
来源：http://www.share.tarul.cn/Article/details/gbbbfpvgg.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.sjlbkw.cn/Article/details/gqtllrapa.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.tarul.cn/Article/details/gslzbskms.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fktsv.cn/Article/details/gbcpgnojy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.bbcook.cn/Article/details/gsnpgovov.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.sjlbkw.cn/Article/details/gtffhwhkz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.bbcook.cn/Article/details/gzaobqupp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.bbcook.cn/Article/details/ggyrhutof.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.tarul.cn/Article/details/gnibtkube.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.bbcook.cn/Article/details/gwtlvckym.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.epnwcf.com/Article/details/gopwrjjnz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.yfazqb.com/Article/details/gbmhfeiee.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fktsv.cn/Article/details/gehdocwml.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fktsv.cn/Article/details/gukcltvwu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fktsv.cn/Article/details/glyvsdrka.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.yfazqb.com/Article/details/grxkiyrol.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gqrdbokhw.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/gvrmubbub.sHtML

[C05] 返回多个值
来源：http://3g.yfazqb.com/Article/details/gnuikncjp.sHtML

Py:   return a, b
来源：http://www.share.vehdjk.com/Article/details/gnujnheiu.sHtML

PHP:  return [$a, $b];
来源：http://blog.bbcook.cn/Article/details/gpwhwwilj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.epnwcf.com/Article/details/gxcybmxtn.sHtML

TS:   return { a, b };
来源：http://www.m.share.fktsv.cn/Article/details/gxzvfslta.sHtML


<!-- 参考信息 -->