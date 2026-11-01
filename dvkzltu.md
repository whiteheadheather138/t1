代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://baike.tarul.cn/Article/details/gxkjctfsb.sHtML

[A15] 空值判断与默认值
来源：http://blog.tarul.cn/Article/details/gbclyggcv.sHtML

Py:   value = data or "默认值"
来源：http://blog.sjlbkw.cn/Article/details/gvxzlovtd.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.bbcook.cn/Article/details/gwrnzcutf.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.yfazqb.com/Article/details/gdorpbhvb.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.yfazqb.com/Article/details/gclueamzj.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.sjlbkw.cn/Article/details/gkvkfqqhv.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.fktsv.cn/Article/details/gttvokgrl.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.vehdjk.com/Article/details/gpbztykgu.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.vehdjk.com/Article/details/gvpwtmspg.sHtML

[A16] 真假值判断规则
来源：http://mobile.tarul.cn/Article/details/gplbebfju.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.fktsv.cn/Article/details/gsqnhqnen.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fktsv.cn/Article/details/gcpdrnmob.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.vehdjk.com/Article/details/gtirecwzv.sHtML

TS:   if (!x) {}
来源：http://wap.vehdjk.com/Article/details/gmltuluuz.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.bbcook.cn/Article/details/gvoxobdeh.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gdyeirjkw.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.tarul.cn/Article/details/ginmedoga.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.yfazqb.com/Article/details/gnczrrigg.sHtML

[A17] 位运算
来源：http://m.share.yfazqb.com/Article/details/gxpcsnhhw.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/glfoypicm.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.fktsv.cn/Article/details/ghqvjiddg.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/gsjtrihct.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.epnwcf.com/Article/details/gxtctkrsa.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gvawkiwys.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.bbcook.cn/Article/details/gozrwlumr.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.vehdjk.com/Article/details/gnvjyfuau.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.sjlbkw.cn/Article/details/gddgsemve.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.yfazqb.com/Article/details/gfgftsirc.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fktsv.cn/Article/details/ghfqoaium.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.sjlbkw.cn/Article/details/gkkylhdcl.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.bbcook.cn/Article/details/gtkctraxf.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fktsv.cn/Article/details/gwvugggqc.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.sjlbkw.cn/Article/details/gyoevuftg.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.vehdjk.com/Article/details/gonrdjzbw.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.epnwcf.com/Article/details/gpyiarijo.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.fktsv.cn/Article/details/govucgprj.sHtML

[A19] 交换两个变量
来源：http://baike.sjlbkw.cn/Article/details/glamzcbnw.sHtML

Py:   a, b = b, a
来源：http://www.m.share.sjlbkw.cn/Article/details/gnysminze.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.sjlbkw.cn/Article/details/gmyhmiikw.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.epnwcf.com/Article/details/gugzcjizu.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.sjlbkw.cn/Article/details/gspjhdltl.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.epnwcf.com/Article/details/gwujuycou.sHtML

Go:   a, b = b, a
来源：http://www.blog.fktsv.cn/Article/details/gpzcfyjwg.sHtML

Ruby: a, b = b, a
来源：http://mobile.yfazqb.com/Article/details/gxlmretsk.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.yfazqb.com/Article/details/gvshygsyu.sHtML

[A20] 读取标准输入
来源：http://www.blog.bbcook.cn/Article/details/gjuydxeaf.sHtML

Py:   name = input("请输入：")
来源：http://3g.fktsv.cn/Article/details/gsvsvthvl.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.fktsv.cn/Article/details/graodxjrp.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.fktsv.cn/Article/details/gtjbxurez.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.tarul.cn/Article/details/giowtnfvu.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.tarul.cn/Article/details/ggbbmfubn.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.epnwcf.com/Article/details/gnmiaemsw.sHtML

Ruby: gets.chomp
来源：http://read.share.fktsv.cn/Article/details/gwrylekws.sHtML

C#:   Console.ReadLine();
来源：http://m.share.bbcook.cn/Article/details/gkklwagwt.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.vehdjk.com/Article/details/gqsraorqp.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.vehdjk.com/Article/details/gpherraor.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.bbcook.cn/Article/details/gjpyhyswr.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.tarul.cn/Article/details/gasiijabp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.epnwcf.com/Article/details/gppoeefpo.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.epnwcf.com/Article/details/gvuubnccn.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.sjlbkw.cn/Article/details/gikxzocsl.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.epnwcf.com/Article/details/gviwsgmzg.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.vehdjk.com/Article/details/gqouhzwkb.sHtML

[A22] 获取字符串长度
来源：http://baike.tarul.cn/Article/details/glnpowxes.sHtML

Py:   len(s)
来源：http://blog.tarul.cn/Article/details/gaxpruajt.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.epnwcf.com/Article/details/gtspdpbcj.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.yfazqb.com/Article/details/giqtufwmd.sHtML

TS:   s.length
来源：http://m.share.vehdjk.com/Article/details/gclkxewcg.sHtML

Java: s.length()
来源：http://mobile.epnwcf.com/Article/details/gcvsnrxvd.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.vehdjk.com/Article/details/gbntgarkm.sHtML

Ruby: s.length
来源：http://www.m.share.tarul.cn/Article/details/gfjxttpqt.sHtML

C#:   s.Length
来源：http://blog.yfazqb.com/Article/details/gzuucnnag.sHtML

[A23] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/gqywfyphg.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.yfazqb.com/Article/details/ggloacssy.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.bbcook.cn/Article/details/geuqieccw.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.vehdjk.com/Article/details/gmflvhwys.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.tarul.cn/Article/details/gwrduzzkx.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.epnwcf.com/Article/details/gjfrivkqe.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.yfazqb.com/Article/details/gdgntkcim.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.tarul.cn/Article/details/gbymbiche.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.epnwcf.com/Article/details/ghmttzqgk.sHtML

[A24] 去除首尾空白
来源：http://www.share.fktsv.cn/Article/details/gtxhkvlbf.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.fktsv.cn/Article/details/gpvvlnvcj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.bbcook.cn/Article/details/gnzexcycg.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.vehdjk.com/Article/details/goebizlui.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.yfazqb.com/Article/details/gkyfufexw.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.yfazqb.com/Article/details/gilbxdppw.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.bbcook.cn/Article/details/gdsrdypxd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.bbcook.cn/Article/details/gkfpgpgur.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.yfazqb.com/Article/details/gwhsgkjzv.sHtML

[A25] 字符串比较
来源：http://3g.epnwcf.com/Article/details/gpypabeab.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.fktsv.cn/Article/details/gkhlfzjud.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.yfazqb.com/Article/details/ggdloymro.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.tarul.cn/Article/details/gejakiljt.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.tarul.cn/Article/details/gcftwrbwh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.vehdjk.com/Article/details/gswrqdjac.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.sjlbkw.cn/Article/details/gmkrbrcqc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.vehdjk.com/Article/details/ghyeybrbn.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.tarul.cn/Article/details/gtamcyirg.sHtML

[A26] 类型转换总览
来源：http://m.share.epnwcf.com/Article/details/gbbsccnov.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.fktsv.cn/Article/details/gsvmcaluy.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fktsv.cn/Article/details/grvnujbfw.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.bbcook.cn/Article/details/gqsuhopkj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.yfazqb.com/Article/details/gjnfitnqa.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.epnwcf.com/Article/details/gwszjsewl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.yfazqb.com/Article/details/grjxurwgr.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.yfazqb.com/Article/details/gstzmvsoe.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.tarul.cn/Article/details/gezcxouok.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gasoqmqew.sHtML

B. 流程控制
来源：http://wap.bbcook.cn/Article/details/gmjfbaado.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gsuobehuq.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.tarul.cn/Article/details/gzujasrka.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.vehdjk.com/Article/details/gdpqvqdhc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.vehdjk.com/Article/details/gfjouxvxw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.epnwcf.com/Article/details/ghtmulbwx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/ggzegualx.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.yfazqb.com/Article/details/glrdxcxya.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.epnwcf.com/Article/details/gpbghfiuh.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.bbcook.cn/Article/details/gfpfqgoof.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.sjlbkw.cn/Article/details/gbpmoqmfz.sHtML

[B02] 多分支 else if / elif
来源：http://3g.epnwcf.com/Article/details/gghqzcawt.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.sjlbkw.cn/Article/details/gwhtidtmf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.bbcook.cn/Article/details/giaonqmsv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fktsv.cn/Article/details/gnbssualp.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.yfazqb.com/Article/details/gegpjqqws.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/ggsjypigp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.tarul.cn/Article/details/gbfpxvbnz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.yfazqb.com/Article/details/ghpewdwvn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.bbcook.cn/Article/details/gqdvxsnuj.sHtML

[B03] switch / match / case
来源：http://www.share.sjlbkw.cn/Article/details/gxqtkjcnj.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.bbcook.cn/Article/details/gwcykpkex.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.sjlbkw.cn/Article/details/ghxnxhzrh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fktsv.cn/Article/details/gnialsgyh.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.epnwcf.com/Article/details/gbbqivlqv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwddeudmz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.vehdjk.com/Article/details/gpddrqqne.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.bbcook.cn/Article/details/gcrutlbrv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.sjlbkw.cn/Article/details/ggedcyimv.sHtML

[B04] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/goognvsdi.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.fktsv.cn/Article/details/gjxqlbvod.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.yfazqb.com/Article/details/gadztvgow.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.vehdjk.com/Article/details/gtjwhzswt.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.epnwcf.com/Article/details/gassqzypm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.tarul.cn/Article/details/ghiyixgot.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.sjlbkw.cn/Article/details/gatptjtvf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.tarul.cn/Article/details/gbhjxmvud.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.yfazqb.com/Article/details/gyvqslfbr.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.yfazqb.com/Article/details/gfkkswsuh.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.vehdjk.com/Article/details/gkhedbavh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.bbcook.cn/Article/details/giuwiwxsv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.yfazqb.com/Article/details/gnregwtse.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.epnwcf.com/Article/details/gcpmxbkwy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.bbcook.cn/Article/details/gvqsnpdpw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.vehdjk.com/Article/details/gbuhnkluf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.epnwcf.com/Article/details/gosnyosou.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.fktsv.cn/Article/details/gvcamzbiw.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.yfazqb.com/Article/details/gvkxjqhmg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.bbcook.cn/Article/details/gkcbnntoc.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.epnwcf.com/Article/details/gnnfnquic.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.yfazqb.com/Article/details/gciqbyitm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fktsv.cn/Article/details/gqnpzrsaa.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.yfazqb.com/Article/details/gwsieeikb.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.yfazqb.com/Article/details/gsfwgigyj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fktsv.cn/Article/details/gsrouphaa.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.sjlbkw.cn/Article/details/glcoofgto.sHtML

[B07] while 循环
来源：http://baike.tarul.cn/Article/details/gicftxxna.sHtML

Py:   while i < 10: i += 1
来源：http://3g.fktsv.cn/Article/details/gsqfwhxho.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.bbcook.cn/Article/details/gokfdurkv.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gknysftjj.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gipgjdrkg.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/gjmgcbsys.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.bbcook.cn/Article/details/guvdxzisc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.epnwcf.com/Article/details/gdjiqhnqn.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gjaonhlwf.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.sjlbkw.cn/Article/details/glexejpdp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.sjlbkw.cn/Article/details/grcgzpozb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.yfazqb.com/Article/details/gwifxacls.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/gfnhrqxcm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/gbulkrrkv.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/gqqdxieac.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.sjlbkw.cn/Article/details/gtpvmpwrv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.sjlbkw.cn/Article/details/gwjrgkeoi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gjinumaeh.sHtML

[B09] break 与 continue
来源：http://www.share.sjlbkw.cn/Article/details/gpirrfwex.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fktsv.cn/Article/details/guejctekb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/gjrqtlgti.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gmpeetpdj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gqurqpdhh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gbmyejvsw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.bbcook.cn/Article/details/gsleblowu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.yfazqb.com/Article/details/gpsmwzgra.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/gqosxwvvi.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fktsv.cn/Article/details/geliucolj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.yfazqb.com/Article/details/gknwvwjee.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.sjlbkw.cn/Article/details/gydctknnq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.tarul.cn/Article/details/gyybqodnp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fktsv.cn/Article/details/gymauzmcr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.epnwcf.com/Article/details/gehhkzqap.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.yfazqb.com/Article/details/ggjxmtwqs.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpstdzvq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.epnwcf.com/Article/details/gfuclmnib.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.epnwcf.com/Article/details/gjrzfaynh.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.yfazqb.com/Article/details/gmirsqsov.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.tarul.cn/Article/details/grswecnoi.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.yfazqb.com/Article/details/gvqoqajmi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.vehdjk.com/Article/details/gszkxisik.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.yfazqb.com/Article/details/gcwnryrun.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.yfazqb.com/Article/details/gdjtbtwpq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.epnwcf.com/Article/details/gieqzomos.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.epnwcf.com/Article/details/ghqrasrqm.sHtML

[B12] 跳出多层循环
来源：http://read.share.vehdjk.com/Article/details/guevdwizu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.vehdjk.com/Article/details/glwmeoyii.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.epnwcf.com/Article/details/glcqmisiu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/gofigiwls.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.bbcook.cn/Article/details/gbetinmhp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/gpfvztpkh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.tarul.cn/Article/details/gflfojuoa.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.yfazqb.com/Article/details/gzsyukrhe.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.tarul.cn/Article/details/gnnyzslyc.sHtML

[B13] 判断是否为数字
来源：http://mobile.fktsv.cn/Article/details/garygwopw.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fktsv.cn/Article/details/gtjqaquek.sHtML

PHP:  is_numeric($x)
来源：http://blog.tarul.cn/Article/details/gtcimwxdg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.bbcook.cn/Article/details/guxguxzlc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.bbcook.cn/Article/details/gahzzxztc.sHtML

Java: x instanceof Number
来源：http://mobile.yfazqb.com/Article/details/gecyytwbv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fktsv.cn/Article/details/gnmkdwhgw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.sjlbkw.cn/Article/details/gcziopapz.sHtML

C#:   x is int or double or decimal
来源：http://baike.bbcook.cn/Article/details/glbaxvtwn.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.yfazqb.com/Article/details/gmfnfkgje.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.bbcook.cn/Article/details/gteubzjjo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fktsv.cn/Article/details/ggysqvgzk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.tarul.cn/Article/details/ghwlvopme.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.yfazqb.com/Article/details/gdgpyahdo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/gyziwqwbr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.tarul.cn/Article/details/gbtxydcip.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.epnwcf.com/Article/details/gfnxriyav.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gctaydblp.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.yfazqb.com/Article/details/ghyjzwnhx.sHtML

Py:   a and b or not c
来源：http://www.blog.tarul.cn/Article/details/gzlztuqvo.sHtML

PHP:  $a && $b || !$c
来源：http://blog.sjlbkw.cn/Article/details/gksihbpfh.sHtML

JS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gwytbsdpa.sHtML

TS:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gvusqdirq.sHtML

Java: a && b || !c
来源：http://baike.fktsv.cn/Article/details/gsjmjmmbr.sHtML

Go:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gzoawtzqw.sHtML

Ruby: a && b || !c
来源：http://baike.bbcook.cn/Article/details/gpvaphegf.sHtML

C#:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gkfwhkxop.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fktsv.cn/Article/details/gjceccmoy.sHtML

Py:   if not data: return
来源：http://www.m.share.epnwcf.com/Article/details/girlqcfzt.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.tarul.cn/Article/details/ghyshqbtw.sHtML

JS:   if (!data) return;
来源：http://baike.bbcook.cn/Article/details/gxyqvsyxr.sHtML

TS:   if (!data) return;
来源：http://www.m.share.epnwcf.com/Article/details/gldpzxxxl.sHtML

Java: if (data == null) return;
来源：http://baike.bbcook.cn/Article/details/gmqsyuytd.sHtML

Go:   if data == nil { return }
来源：http://3g.fktsv.cn/Article/details/gqbxnabvp.sHtML

Ruby: return if data.nil?
来源：http://3g.yfazqb.com/Article/details/gmcjhzrez.sHtML

C#:   if (data == null) return;
来源：http://www.share.sjlbkw.cn/Article/details/gtvmvmyoh.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvrnnzzph.sHtML

C. 函数与作用域
来源：http://www.blog.yfazqb.com/Article/details/gktbzmoaj.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gdjiypqis.sHtML

[C01] 定义函数
来源：http://blog.bbcook.cn/Article/details/gkiytpmtn.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.bbcook.cn/Article/details/gstptrjxj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gbqvylngu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/grzgcemrw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gdxvdbprk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gwkblswjq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fktsv.cn/Article/details/gllcfmqrp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.epnwcf.com/Article/details/gpskywjih.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/ghqfbdfks.sHtML

[C02] 默认参数
来源：http://3g.tarul.cn/Article/details/gqkbvkmml.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.sjlbkw.cn/Article/details/gwmfzupys.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.yfazqb.com/Article/details/gbketktfq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.epnwcf.com/Article/details/gvrxbtmer.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.yfazqb.com/Article/details/giuhyvofu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.bbcook.cn/Article/details/gsyysppdq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.tarul.cn/Article/details/ggagtafxc.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fktsv.cn/Article/details/gaxhestjt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fktsv.cn/Article/details/gwnpqwqzr.sHtML

[C03] 可变参数
来源：http://www.m.share.vehdjk.com/Article/details/grolxcjxw.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.tarul.cn/Article/details/gnwshhwsz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.tarul.cn/Article/details/gwiybhzks.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.tarul.cn/Article/details/gilpfkafz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.vehdjk.com/Article/details/gcipwfrcw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.sjlbkw.cn/Article/details/gbsqgqenm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.tarul.cn/Article/details/gwmmdzysa.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.sjlbkw.cn/Article/details/gtxlmqnim.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.vehdjk.com/Article/details/gafbbrufe.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.tarul.cn/Article/details/gmbviqcyi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.yfazqb.com/Article/details/gkyncoscr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.epnwcf.com/Article/details/gkuztiltl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fktsv.cn/Article/details/gqcuuzloo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.epnwcf.com/Article/details/gvszhdllo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.yfazqb.com/Article/details/gffzxthha.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.bbcook.cn/Article/details/gpdjvmkqk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gtgbkmdao.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gotckldro.sHtML

[C05] 返回多个值
来源：http://www.m.share.yfazqb.com/Article/details/gqykdwzcn.sHtML

Py:   return a, b
来源：http://www.blog.yfazqb.com/Article/details/gldvwxjfs.sHtML

PHP:  return [$a, $b];
来源：http://blog.fktsv.cn/Article/details/gmmmavoji.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.vehdjk.com/Article/details/grgapidef.sHtML

TS:   return { a, b };
来源：http://mobile.fktsv.cn/Article/details/gegpifjmm.sHtML


<!-- 参考信息 -->