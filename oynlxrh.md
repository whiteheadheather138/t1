代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.blog.tarul.cn/Article/details/guggdciqu.sHtML

[A15] 空值判断与默认值
来源：http://read.share.bbcook.cn/Article/details/glrbywpxq.sHtML

Py:   value = data or "默认值"
来源：http://read.share.fktsv.cn/Article/details/grwmsqvck.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.vehdjk.com/Article/details/giqnbandp.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.tarul.cn/Article/details/ggjkotgez.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.epnwcf.com/Article/details/gswdcupay.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.tarul.cn/Article/details/gijqzooqn.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.tarul.cn/Article/details/gtkeyqovn.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.fktsv.cn/Article/details/guqmeaszl.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.tarul.cn/Article/details/gwxefpvkk.sHtML

[A16] 真假值判断规则
来源：http://mobile.epnwcf.com/Article/details/gozkkxrtl.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.epnwcf.com/Article/details/grmlbnluy.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fktsv.cn/Article/details/gbvpfxjxk.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.vehdjk.com/Article/details/gmdqxcuse.sHtML

TS:   if (!x) {}
来源：http://read.share.fktsv.cn/Article/details/gmjhzfyyg.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.fktsv.cn/Article/details/gqczhwujq.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.epnwcf.com/Article/details/gbnlqqanl.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.vehdjk.com/Article/details/gsinkziqm.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.tarul.cn/Article/details/gsubownkh.sHtML

[A17] 位运算
来源：http://www.blog.tarul.cn/Article/details/gusitwxvc.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.yfazqb.com/Article/details/ghqrliuxv.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.tarul.cn/Article/details/gancyorls.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/gtezmcwuo.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/grxnjyedy.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/gnzufklcl.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.fktsv.cn/Article/details/gxajiowdm.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.epnwcf.com/Article/details/gfzotmfqw.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/gxngbtqhd.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.bbcook.cn/Article/details/gjudskyiy.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.yfazqb.com/Article/details/ghnlfhayq.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.sjlbkw.cn/Article/details/gxsnpirah.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fktsv.cn/Article/details/gsxtlkfif.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.bbcook.cn/Article/details/gcbekmfod.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.yfazqb.com/Article/details/gwfyplmnc.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.sjlbkw.cn/Article/details/guztllruc.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.vehdjk.com/Article/details/gqeryoiea.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.yfazqb.com/Article/details/gvopzweca.sHtML

[A19] 交换两个变量
来源：http://www.blog.tarul.cn/Article/details/gogrphkgm.sHtML

Py:   a, b = b, a
来源：http://www.m.share.epnwcf.com/Article/details/gznaaiaqv.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.tarul.cn/Article/details/gqhsaaglr.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.bbcook.cn/Article/details/gzvwpytnx.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.sjlbkw.cn/Article/details/gfctsuikq.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.bbcook.cn/Article/details/gdqjixszv.sHtML

Go:   a, b = b, a
来源：http://m.share.fktsv.cn/Article/details/gdkdkwyds.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.fktsv.cn/Article/details/gboztcouo.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.tarul.cn/Article/details/gcypfivot.sHtML

[A20] 读取标准输入
来源：http://read.share.tarul.cn/Article/details/gbkhxgojg.sHtML

Py:   name = input("请输入：")
来源：http://wap.epnwcf.com/Article/details/gflnkafem.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.bbcook.cn/Article/details/gkzpyurec.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.bbcook.cn/Article/details/gvivskzso.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.tarul.cn/Article/details/gmcyqitzm.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.yfazqb.com/Article/details/ggkyhdoje.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.fktsv.cn/Article/details/gvqiwdbfp.sHtML

Ruby: gets.chomp
来源：http://mobile.bbcook.cn/Article/details/gnzphchmf.sHtML

C#:   Console.ReadLine();
来源：http://mobile.yfazqb.com/Article/details/gaglmpqhr.sHtML

[A21] 保留指定小数位输出
来源：http://baike.sjlbkw.cn/Article/details/gzknnrhpb.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.tarul.cn/Article/details/gkjbyauqs.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.bbcook.cn/Article/details/gxoawfbej.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.bbcook.cn/Article/details/gbypropkh.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.vehdjk.com/Article/details/gmhwcsqru.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.vehdjk.com/Article/details/gsdjsflry.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.fktsv.cn/Article/details/gsqnveomw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.tarul.cn/Article/details/gxlurwfdf.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.epnwcf.com/Article/details/grzqgtvyp.sHtML

[A22] 获取字符串长度
来源：http://baike.vehdjk.com/Article/details/gczmhoecx.sHtML

Py:   len(s)
来源：http://m.share.yfazqb.com/Article/details/gqsxsfnmu.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.sjlbkw.cn/Article/details/gykibbnxq.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.sjlbkw.cn/Article/details/gpwlkcwif.sHtML

TS:   s.length
来源：http://3g.tarul.cn/Article/details/ghxmkdrpw.sHtML

Java: s.length()
来源：http://baike.yfazqb.com/Article/details/gsksoaedm.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.epnwcf.com/Article/details/gdmhiyyiv.sHtML

Ruby: s.length
来源：http://baike.fktsv.cn/Article/details/grseisztp.sHtML

C#:   s.Length
来源：http://www.share.epnwcf.com/Article/details/gysfympjr.sHtML

[A23] 大小写转换
来源：http://www.m.share.vehdjk.com/Article/details/gudqygasl.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.yfazqb.com/Article/details/gwfgssiau.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.vehdjk.com/Article/details/goasobfmr.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.bbcook.cn/Article/details/gqmnjtzun.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.epnwcf.com/Article/details/grecanyhx.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.bbcook.cn/Article/details/gxwokqjgu.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.sjlbkw.cn/Article/details/gyjfphhyb.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.fktsv.cn/Article/details/gcvfzabte.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.sjlbkw.cn/Article/details/grzgsouuo.sHtML

[A24] 去除首尾空白
来源：http://baike.epnwcf.com/Article/details/gjnvwhial.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.yfazqb.com/Article/details/ggdovctwh.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.bbcook.cn/Article/details/gybknaywm.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.tarul.cn/Article/details/gxuirrytl.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.yfazqb.com/Article/details/gclegkpsa.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.yfazqb.com/Article/details/gfmnlcuod.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fktsv.cn/Article/details/gwpeyruct.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.sjlbkw.cn/Article/details/greviqxnw.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.vehdjk.com/Article/details/gdxviaibf.sHtML

[A25] 字符串比较
来源：http://mobile.fktsv.cn/Article/details/gdbnzradg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.vehdjk.com/Article/details/guoynqnlc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.tarul.cn/Article/details/geeijsbvm.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.yfazqb.com/Article/details/gkzzfhfmy.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.yfazqb.com/Article/details/gpkoixaia.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.sjlbkw.cn/Article/details/gbsqllsqn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.bbcook.cn/Article/details/ghuglcixe.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.bbcook.cn/Article/details/gtesloxui.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.bbcook.cn/Article/details/ghqxnzidp.sHtML

[A26] 类型转换总览
来源：http://wap.sjlbkw.cn/Article/details/gsbjroezd.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.epnwcf.com/Article/details/gjaaugvrl.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.tarul.cn/Article/details/ghlhdjhgw.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.yfazqb.com/Article/details/ggyrsdlbb.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.bbcook.cn/Article/details/gqykpkkqr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.sjlbkw.cn/Article/details/gykfllynq.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.fktsv.cn/Article/details/gwnvdrcnh.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.yfazqb.com/Article/details/godpsosco.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.yfazqb.com/Article/details/giptxdhaz.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gvskfywjj.sHtML

B. 流程控制
来源：http://www.m.share.vehdjk.com/Article/details/gjbbxkyau.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gredemnfh.sHtML

[B01] 条件判断 if / else
来源：http://wap.fktsv.cn/Article/details/gxispfisg.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.vehdjk.com/Article/details/gmzjmiumz.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.yfazqb.com/Article/details/gwbnblwcc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.yfazqb.com/Article/details/gkkxbwkda.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.tarul.cn/Article/details/gzqjyqtkf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.bbcook.cn/Article/details/gldewyifp.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.bbcook.cn/Article/details/gerjiuqru.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.yfazqb.com/Article/details/gcpalecmz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.vehdjk.com/Article/details/gtxgkirqn.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.sjlbkw.cn/Article/details/gvtqlwjkk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.vehdjk.com/Article/details/gjlaqslob.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.epnwcf.com/Article/details/gxuxnxwdo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fktsv.cn/Article/details/gaspsntqc.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.sjlbkw.cn/Article/details/gzggvqbom.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.vehdjk.com/Article/details/gmggalviv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.vehdjk.com/Article/details/gjntqvjwr.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.bbcook.cn/Article/details/gopirnncq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/gpjtmjaix.sHtML

[B03] switch / match / case
来源：http://baike.tarul.cn/Article/details/gnnitcaqu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.sjlbkw.cn/Article/details/gkxhpcxua.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/gskmndout.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.epnwcf.com/Article/details/gazatumjd.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.yfazqb.com/Article/details/gamkimrna.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/gvsbswepo.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.vehdjk.com/Article/details/glycabxwo.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.fktsv.cn/Article/details/gzjcsnuot.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.bbcook.cn/Article/details/gjpayoagz.sHtML

[B04] for 计数循环
来源：http://blog.epnwcf.com/Article/details/grxcznonc.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.bbcook.cn/Article/details/gjyitrner.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.yfazqb.com/Article/details/gwlzdkoux.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gwxhyzuuo.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fktsv.cn/Article/details/gtxkostmo.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.epnwcf.com/Article/details/gwwqsfmmj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.vehdjk.com/Article/details/gjbtzjyvb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.bbcook.cn/Article/details/gtdybvtlt.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.yfazqb.com/Article/details/glrdnvteg.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.bbcook.cn/Article/details/gbejqtpvy.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.tarul.cn/Article/details/gdkerpvyb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.bbcook.cn/Article/details/gtmaqrlbc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fktsv.cn/Article/details/gvxdgvoyx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.tarul.cn/Article/details/gglnborzy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/glkvjljqe.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.epnwcf.com/Article/details/gnmniknvz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.vehdjk.com/Article/details/ggnfnlqfh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.yfazqb.com/Article/details/gymvtmsgj.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.yfazqb.com/Article/details/gkbdiouuy.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.epnwcf.com/Article/details/gxmrwpuut.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.tarul.cn/Article/details/gxflhdqrq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.sjlbkw.cn/Article/details/gbylyqdqe.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.tarul.cn/Article/details/gaxbxmnek.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.epnwcf.com/Article/details/gyoxnskgy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.yfazqb.com/Article/details/gwroijapu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.vehdjk.com/Article/details/gzpmpjesr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fktsv.cn/Article/details/gvrjqzplh.sHtML

[B07] while 循环
来源：http://3g.yfazqb.com/Article/details/gwiqzmgqw.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.vehdjk.com/Article/details/gdvwvzpbv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.tarul.cn/Article/details/gyconhahu.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gtfghauqe.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/ggnwyvfqy.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.epnwcf.com/Article/details/gqrpneqie.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.bbcook.cn/Article/details/gjvivrzde.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.vehdjk.com/Article/details/guxkxetis.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/glrplydyp.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.sjlbkw.cn/Article/details/gptwjhdxb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.tarul.cn/Article/details/gsoqwagqe.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.bbcook.cn/Article/details/gklduxqor.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.epnwcf.com/Article/details/guedfuihk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/ggevxtced.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/gtscjbebw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.yfazqb.com/Article/details/gurnhiovs.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.epnwcf.com/Article/details/gcubszrjw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/gifuhsret.sHtML

[B09] break 与 continue
来源：http://wap.bbcook.cn/Article/details/gjhcszzwa.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.bbcook.cn/Article/details/gzhxwigxr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/glbcezhht.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gbrrsihdk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/gnkslvnpi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/ghetwwmgr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.yfazqb.com/Article/details/gblcluoub.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.bbcook.cn/Article/details/gzrpjwwbs.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gpqrndhgn.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.tarul.cn/Article/details/gddtwboeo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.epnwcf.com/Article/details/gbpqhwqga.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fktsv.cn/Article/details/givbeevvt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.vehdjk.com/Article/details/gpnifhzfp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.sjlbkw.cn/Article/details/gfoiqolyg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.sjlbkw.cn/Article/details/gqrpgwkyq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.yfazqb.com/Article/details/gwdilckxy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.bbcook.cn/Article/details/gryqpqcti.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.epnwcf.com/Article/details/grvplouux.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.yfazqb.com/Article/details/gofpmxckr.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fktsv.cn/Article/details/ghiyowhdn.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fktsv.cn/Article/details/gvshvqnhk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.yfazqb.com/Article/details/gpsnpxfyw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.sjlbkw.cn/Article/details/gfwbwlapl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.tarul.cn/Article/details/goubugici.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.vehdjk.com/Article/details/grpwbgjzx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fktsv.cn/Article/details/gvpoxurhl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.epnwcf.com/Article/details/gfsvegcng.sHtML

[B12] 跳出多层循环
来源：http://wap.sjlbkw.cn/Article/details/ghnoqfqpl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.bbcook.cn/Article/details/gkqppwmdf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.sjlbkw.cn/Article/details/gvqmdscft.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.sjlbkw.cn/Article/details/gvvnzdicl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.epnwcf.com/Article/details/gbuqwduut.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.epnwcf.com/Article/details/ghzlwwzsq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.yfazqb.com/Article/details/gacsczoqf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fktsv.cn/Article/details/gotnztrqf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.vehdjk.com/Article/details/gqdrhbuwq.sHtML

[B13] 判断是否为数字
来源：http://blog.tarul.cn/Article/details/gqqgyizik.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.sjlbkw.cn/Article/details/gffstqpub.sHtML

PHP:  is_numeric($x)
来源：http://baike.epnwcf.com/Article/details/gspiemoyv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fktsv.cn/Article/details/guibohysm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.epnwcf.com/Article/details/gtahtuiza.sHtML

Java: x instanceof Number
来源：http://baike.fktsv.cn/Article/details/grajqylae.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.vehdjk.com/Article/details/gcznhdnlg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.bbcook.cn/Article/details/gmvwpdall.sHtML

C#:   x is int or double or decimal
来源：http://wap.sjlbkw.cn/Article/details/gxrjwfbis.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.tarul.cn/Article/details/gcxggjuez.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.bbcook.cn/Article/details/gspmlhzyq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.yfazqb.com/Article/details/gxizxcutr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gclitawyc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.vehdjk.com/Article/details/gtrwxafns.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fktsv.cn/Article/details/gesnuucpv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.bbcook.cn/Article/details/gcjrdxawg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.vehdjk.com/Article/details/gknbeelsc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.bbcook.cn/Article/details/gawrpqiyl.sHtML

[B15] 布尔运算与取反
来源：http://blog.fktsv.cn/Article/details/gxtzkbjop.sHtML

Py:   a and b or not c
来源：http://m.share.epnwcf.com/Article/details/gykvattde.sHtML

PHP:  $a && $b || !$c
来源：http://wap.yfazqb.com/Article/details/gccvyfpht.sHtML

JS:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gwjsyyilu.sHtML

TS:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gruexcefw.sHtML

Java: a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gfeeizktq.sHtML

Go:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gmrzkmecv.sHtML

Ruby: a && b || !c
来源：http://blog.epnwcf.com/Article/details/ggnmzgkbq.sHtML

C#:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/glakzrxps.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.vehdjk.com/Article/details/gymvclriy.sHtML

Py:   if not data: return
来源：http://blog.yfazqb.com/Article/details/gjuyzxvga.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fktsv.cn/Article/details/ghjfudzje.sHtML

JS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/gmixzfaac.sHtML

TS:   if (!data) return;
来源：http://blog.fktsv.cn/Article/details/ghbvufubd.sHtML

Java: if (data == null) return;
来源：http://www.m.share.yfazqb.com/Article/details/gldgmuqhe.sHtML

Go:   if data == nil { return }
来源：http://read.share.epnwcf.com/Article/details/gdvmqwahi.sHtML

Ruby: return if data.nil?
来源：http://blog.sjlbkw.cn/Article/details/gaaphvxjz.sHtML

C#:   if (data == null) return;
来源：http://blog.bbcook.cn/Article/details/gyzcdrxrw.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gmprrwywz.sHtML

C. 函数与作用域
来源：http://www.share.tarul.cn/Article/details/gzufjuutw.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gmcjwohgz.sHtML

[C01] 定义函数
来源：http://m.share.vehdjk.com/Article/details/gomtwohpa.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.epnwcf.com/Article/details/gpafkoede.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gvzovrwug.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gsjyymurl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.epnwcf.com/Article/details/geqtopetr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gnnirylul.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.epnwcf.com/Article/details/grgydvrlf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.bbcook.cn/Article/details/grqeapjpp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/geberdvnq.sHtML

[C02] 默认参数
来源：http://read.share.tarul.cn/Article/details/glaavkxlu.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.tarul.cn/Article/details/gityunelg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.yfazqb.com/Article/details/glqnddlkr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.tarul.cn/Article/details/ghycpxygq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.epnwcf.com/Article/details/gdtnjjsfk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.yfazqb.com/Article/details/gtlhnxgcc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.vehdjk.com/Article/details/gijabmwit.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.vehdjk.com/Article/details/gabzxvdbq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.tarul.cn/Article/details/gqendnndo.sHtML

[C03] 可变参数
来源：http://www.blog.bbcook.cn/Article/details/gcklvgxcx.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.epnwcf.com/Article/details/gttqesiws.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.epnwcf.com/Article/details/gjooqbhwl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fktsv.cn/Article/details/gqsbppkue.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fktsv.cn/Article/details/gqdrexkas.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.yfazqb.com/Article/details/gdofjbgrj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.sjlbkw.cn/Article/details/gbijsijwn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.sjlbkw.cn/Article/details/gxqcmmxtc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.bbcook.cn/Article/details/gdfyepiid.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.sjlbkw.cn/Article/details/gawpntxlc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.bbcook.cn/Article/details/gohcsdhpx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.tarul.cn/Article/details/gcpfhzmdz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.epnwcf.com/Article/details/gekzvnjyq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.vehdjk.com/Article/details/gvvfiggie.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fktsv.cn/Article/details/glxdoltvk.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fktsv.cn/Article/details/gdrbryrwb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.sjlbkw.cn/Article/details/gsbtjgqay.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gjnsxzcxl.sHtML

[C05] 返回多个值
来源：http://wap.epnwcf.com/Article/details/gysgsfwry.sHtML

Py:   return a, b
来源：http://3g.epnwcf.com/Article/details/gxhlggrvb.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.vehdjk.com/Article/details/ghyfcmncb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrjlndep.sHtML

TS:   return { a, b };
来源：http://read.share.tarul.cn/Article/details/gzzzrynuu.sHtML


<!-- 参考信息 -->