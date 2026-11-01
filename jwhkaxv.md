代发 wailian999

[A14] 注释写法
来源：http://read.share.yfazqb.com/Article/details/gzyfoufyk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.epnwcf.com/Article/details/grbdytyvp.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.vehdjk.com/Article/details/gmwufpisg.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.tarul.cn/Article/details/gwlfbfnaf.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.yfazqb.com/Article/details/gjledkozr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.vehdjk.com/Article/details/gfngkxwlh.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.sjlbkw.cn/Article/details/gcnzoutor.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.sjlbkw.cn/Article/details/gbvlqnsuk.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.epnwcf.com/Article/details/geonfenrp.sHtML

[A15] 空值判断与默认值
来源：http://mobile.fktsv.cn/Article/details/gkphwhoyb.sHtML

Py:   value = data or "默认值"
来源：http://mobile.bbcook.cn/Article/details/gbkezsyih.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.bbcook.cn/Article/details/gbpxwqmzx.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.bbcook.cn/Article/details/godccovwg.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.bbcook.cn/Article/details/guconzvuz.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.vehdjk.com/Article/details/gtwktophm.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.tarul.cn/Article/details/gvexcablh.sHtML

Ruby: value = data || "默认值"
来源：http://baike.epnwcf.com/Article/details/glawyrpji.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.tarul.cn/Article/details/grwjwzxan.sHtML

[A16] 真假值判断规则
来源：http://read.share.bbcook.cn/Article/details/gwlmhkiyk.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.fktsv.cn/Article/details/gsffxxzqq.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.bbcook.cn/Article/details/gjdqvirqf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.sjlbkw.cn/Article/details/gkxfmzyrx.sHtML

TS:   if (!x) {}
来源：http://www.blog.epnwcf.com/Article/details/gpgrmgqao.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.epnwcf.com/Article/details/gonveeeur.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.tarul.cn/Article/details/ghdvoxnsp.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtervyfq.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.epnwcf.com/Article/details/glfgxfcay.sHtML

[A17] 位运算
来源：http://mobile.epnwcf.com/Article/details/gusjcwdnh.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.sjlbkw.cn/Article/details/gpruayrvu.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.epnwcf.com/Article/details/gezqakshw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.bbcook.cn/Article/details/ggdgugrde.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/gbpvrcfgc.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.yfazqb.com/Article/details/gqobktvha.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gvunkwidw.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/gcdqzquhr.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.vehdjk.com/Article/details/gxicqahhu.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.sjlbkw.cn/Article/details/gsmkcbnwr.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.tarul.cn/Article/details/gnkwkffdp.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.yfazqb.com/Article/details/gsxgrfigf.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fktsv.cn/Article/details/gupwdevlw.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.epnwcf.com/Article/details/ggfuxbtyf.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.vehdjk.com/Article/details/gooknhhym.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.vehdjk.com/Article/details/gqblrvhod.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.epnwcf.com/Article/details/gfqvvzzsn.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.epnwcf.com/Article/details/gtdgksaxw.sHtML

[A19] 交换两个变量
来源：http://wap.bbcook.cn/Article/details/glprxelqz.sHtML

Py:   a, b = b, a
来源：http://baike.vehdjk.com/Article/details/gtgycbcat.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.tarul.cn/Article/details/gnekzntyj.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.yfazqb.com/Article/details/glajrjhgd.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.fktsv.cn/Article/details/ghgiwbnot.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.vehdjk.com/Article/details/gtshsrhbq.sHtML

Go:   a, b = b, a
来源：http://www.blog.vehdjk.com/Article/details/glajejlme.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.vehdjk.com/Article/details/gyppdiyrm.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.tarul.cn/Article/details/gfpfvaryk.sHtML

[A20] 读取标准输入
来源：http://3g.bbcook.cn/Article/details/gsfisunsu.sHtML

Py:   name = input("请输入：")
来源：http://wap.yfazqb.com/Article/details/gbnksqlxh.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.fktsv.cn/Article/details/gerxcdhaa.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.bbcook.cn/Article/details/goruglxmg.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.epnwcf.com/Article/details/gbhosskyy.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.epnwcf.com/Article/details/gmqvubsaq.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.vehdjk.com/Article/details/gapautehh.sHtML

Ruby: gets.chomp
来源：http://read.share.tarul.cn/Article/details/ghrtqctnk.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.epnwcf.com/Article/details/gyooguqce.sHtML

[A21] 保留指定小数位输出
来源：http://blog.epnwcf.com/Article/details/ghatuopff.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.tarul.cn/Article/details/ggwlchlir.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.tarul.cn/Article/details/geyaktffo.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.tarul.cn/Article/details/ghnfkgizr.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.fktsv.cn/Article/details/gkeitguks.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.sjlbkw.cn/Article/details/gvqhsblws.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.yfazqb.com/Article/details/gpadwqlpa.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.fktsv.cn/Article/details/gpyvgycys.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.sjlbkw.cn/Article/details/ghwwupsyg.sHtML

[A22] 获取字符串长度
来源：http://mobile.tarul.cn/Article/details/gxdppouoe.sHtML

Py:   len(s)
来源：http://baike.bbcook.cn/Article/details/gfigjwisl.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.bbcook.cn/Article/details/gyobsdmmd.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.vehdjk.com/Article/details/gqhbxfkbm.sHtML

TS:   s.length
来源：http://3g.sjlbkw.cn/Article/details/gcffslgkx.sHtML

Java: s.length()
来源：http://m.share.epnwcf.com/Article/details/gsxrpkher.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.epnwcf.com/Article/details/guqpmhszw.sHtML

Ruby: s.length
来源：http://blog.epnwcf.com/Article/details/gogeiqduv.sHtML

C#:   s.Length
来源：http://wap.fktsv.cn/Article/details/gzytbxjzk.sHtML

[A23] 大小写转换
来源：http://baike.tarul.cn/Article/details/gugxmeshf.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.epnwcf.com/Article/details/gypyntput.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.vehdjk.com/Article/details/ghvpmjofk.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.tarul.cn/Article/details/gupemqbkm.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.epnwcf.com/Article/details/ggenegboa.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.bbcook.cn/Article/details/gcgbiimpc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.tarul.cn/Article/details/gnqaxptyy.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.fktsv.cn/Article/details/gokjrjxsc.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.epnwcf.com/Article/details/gmjxqsiqd.sHtML

[A24] 去除首尾空白
来源：http://m.share.vehdjk.com/Article/details/gspccqqvn.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.fktsv.cn/Article/details/gmmegqcxo.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.bbcook.cn/Article/details/gxvivcmhl.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.vehdjk.com/Article/details/gxcsnbrcr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.tarul.cn/Article/details/gbksmwnnj.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.yfazqb.com/Article/details/gskvpwgff.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.tarul.cn/Article/details/gsvahnrrw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.epnwcf.com/Article/details/gsfbakqaf.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.yfazqb.com/Article/details/gjqfxaxbj.sHtML

[A25] 字符串比较
来源：http://m.share.epnwcf.com/Article/details/gnrrhrfno.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.sjlbkw.cn/Article/details/gfxvxkrzh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.sjlbkw.cn/Article/details/gkfudocht.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.epnwcf.com/Article/details/ginnyjqcu.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.epnwcf.com/Article/details/gzzfudgmg.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.vehdjk.com/Article/details/gnjtbovqy.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.yfazqb.com/Article/details/gznqigrpu.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.fktsv.cn/Article/details/gmngdfwbe.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.bbcook.cn/Article/details/gnoeyubwc.sHtML

[A26] 类型转换总览
来源：http://baike.sjlbkw.cn/Article/details/gfbqlmewg.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.epnwcf.com/Article/details/gdvncvbgl.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.sjlbkw.cn/Article/details/gqviigzhv.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.fktsv.cn/Article/details/gkttadkty.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.vehdjk.com/Article/details/gfbpiezyr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.vehdjk.com/Article/details/gziuctelx.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.yfazqb.com/Article/details/gjzrqjeds.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.yfazqb.com/Article/details/gqrehekil.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.yfazqb.com/Article/details/gjrbkhcjx.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/glztlmyfu.sHtML

B. 流程控制
来源：http://baike.bbcook.cn/Article/details/gmewlcpmq.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gkytxasbz.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.fktsv.cn/Article/details/gixaxfcfy.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.vehdjk.com/Article/details/gnhquywhw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.vehdjk.com/Article/details/golcwlnph.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fktsv.cn/Article/details/gmgqxnfeg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.tarul.cn/Article/details/gbwnbojqj.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.yfazqb.com/Article/details/gnywjhtgp.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.sjlbkw.cn/Article/details/grslrhzwo.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.epnwcf.com/Article/details/gylowtqer.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.tarul.cn/Article/details/gcpdhgxon.sHtML

[B02] 多分支 else if / elif
来源：http://baike.bbcook.cn/Article/details/gyrwbgyfv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.vehdjk.com/Article/details/ggzbircdh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.bbcook.cn/Article/details/gjkwpqaqp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.sjlbkw.cn/Article/details/gqztnqwzu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.sjlbkw.cn/Article/details/gtppqvobc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fktsv.cn/Article/details/grqkroyyn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.tarul.cn/Article/details/glpvyxmuz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.fktsv.cn/Article/details/gqerwcwtx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/gwjiutuzn.sHtML

[B03] switch / match / case
来源：http://www.share.bbcook.cn/Article/details/gjedqcrkk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fktsv.cn/Article/details/gztjpizfo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gcixjpgmj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.vehdjk.com/Article/details/gyntyjryp.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fktsv.cn/Article/details/gmtnnrowi.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.yfazqb.com/Article/details/gicftdinp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.fktsv.cn/Article/details/gradjdsxy.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.yfazqb.com/Article/details/ggqtmtavl.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.vehdjk.com/Article/details/gzwjryjsx.sHtML

[B04] for 计数循环
来源：http://blog.vehdjk.com/Article/details/geywyndda.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.bbcook.cn/Article/details/gklmuxakh.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.tarul.cn/Article/details/goyploxnp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.tarul.cn/Article/details/gqfsiuxib.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.sjlbkw.cn/Article/details/govptisgi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.tarul.cn/Article/details/gkwcohuhq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.epnwcf.com/Article/details/gjedptrun.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.sjlbkw.cn/Article/details/gnbvuinlh.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.epnwcf.com/Article/details/gwsdfthno.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.vehdjk.com/Article/details/gixcxxpcq.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.vehdjk.com/Article/details/gbpjlniho.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.epnwcf.com/Article/details/gyblybvnn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.bbcook.cn/Article/details/gkyvzaomv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.bbcook.cn/Article/details/gmtxjsrks.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.vehdjk.com/Article/details/giiqcrqsw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.bbcook.cn/Article/details/gyuucsjpv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.vehdjk.com/Article/details/glbpltvxn.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.yfazqb.com/Article/details/gzouxcmij.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.yfazqb.com/Article/details/gfkjfkxiq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.bbcook.cn/Article/details/gxptjemdm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.yfazqb.com/Article/details/govltzhby.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.vehdjk.com/Article/details/gkjupyovb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.tarul.cn/Article/details/gnctmzkcv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.fktsv.cn/Article/details/gbokjfgul.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.sjlbkw.cn/Article/details/gjgphpokt.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.tarul.cn/Article/details/ggukqhqnz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fktsv.cn/Article/details/gnpwzbzgn.sHtML

[B07] while 循环
来源：http://www.share.fktsv.cn/Article/details/glpangblm.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fktsv.cn/Article/details/gjbxxjtgx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.tarul.cn/Article/details/gldenswyo.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/gbtfcjqea.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/gvhkkiwwc.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.vehdjk.com/Article/details/gmhyirxab.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.sjlbkw.cn/Article/details/ghmrqxthw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.epnwcf.com/Article/details/gbltbfgff.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/ggnsnextp.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.vehdjk.com/Article/details/guznoslxp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.fktsv.cn/Article/details/gvphvubbi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.bbcook.cn/Article/details/gwmtfatew.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/gomjmwbas.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/gaiknlskg.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/gtbackllk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.vehdjk.com/Article/details/gsgdarqlb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.epnwcf.com/Article/details/grfqgqvec.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gcdgiuiru.sHtML

[B09] break 与 continue
来源：http://baike.epnwcf.com/Article/details/gjlwowdki.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.vehdjk.com/Article/details/gakpapefx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/ghruqkrbm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/ghaaqrmtx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gjzbhzowj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gtsecrpdd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.fktsv.cn/Article/details/gxgdqimla.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.epnwcf.com/Article/details/gpzhhboak.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gftmrujvn.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.yfazqb.com/Article/details/gvkkhudkb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.bbcook.cn/Article/details/glmokivsi.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.yfazqb.com/Article/details/gswhbyghn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.vehdjk.com/Article/details/gdaxzejby.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.sjlbkw.cn/Article/details/gdkzhqbam.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.tarul.cn/Article/details/gpkplucfj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fktsv.cn/Article/details/gxpezgzvb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.bbcook.cn/Article/details/grfzwdrae.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.tarul.cn/Article/details/gqgpjdozu.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.sjlbkw.cn/Article/details/gxwzymqwg.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.vehdjk.com/Article/details/gytcdygcu.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.bbcook.cn/Article/details/glroinlrw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.yfazqb.com/Article/details/gjhytpusi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.tarul.cn/Article/details/gihchaliv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.bbcook.cn/Article/details/gedqhuxae.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.tarul.cn/Article/details/gcyplhkno.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.bbcook.cn/Article/details/gjwftbgbm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.epnwcf.com/Article/details/gzekjmygw.sHtML

[B12] 跳出多层循环
来源：http://m.share.sjlbkw.cn/Article/details/gazvrcjfh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.tarul.cn/Article/details/gwrscmbbl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.bbcook.cn/Article/details/gneykcruf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.sjlbkw.cn/Article/details/ghtiyspfp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/giyypycsr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gznsgclmw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.sjlbkw.cn/Article/details/gqgxvllma.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.yfazqb.com/Article/details/gnrxuouib.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.yfazqb.com/Article/details/gnajmjpha.sHtML

[B13] 判断是否为数字
来源：http://3g.vehdjk.com/Article/details/gwyhtyvoj.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.tarul.cn/Article/details/gsxamqyoo.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fktsv.cn/Article/details/glczpmxct.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.yfazqb.com/Article/details/ghznuvijo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.sjlbkw.cn/Article/details/gvxxlvugx.sHtML

Java: x instanceof Number
来源：http://wap.bbcook.cn/Article/details/gipghofyd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fktsv.cn/Article/details/giixiurgn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.bbcook.cn/Article/details/ghnqabvvs.sHtML

C#:   x is int or double or decimal
来源：http://m.share.yfazqb.com/Article/details/ggnvwmedv.sHtML

[B14] 判断值是否在集合内
来源：http://wap.vehdjk.com/Article/details/gbzsjdeag.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.bbcook.cn/Article/details/gxtdqdfet.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.epnwcf.com/Article/details/gpabiusbt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.vehdjk.com/Article/details/gsijkycxf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.vehdjk.com/Article/details/gyrtwndhr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.bbcook.cn/Article/details/gfyqyqhjd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.vehdjk.com/Article/details/gkfensffg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.bbcook.cn/Article/details/gaeglbnms.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.tarul.cn/Article/details/gejumqunf.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.tarul.cn/Article/details/gwbumkogc.sHtML

Py:   a and b or not c
来源：http://www.blog.fktsv.cn/Article/details/gpiacnoph.sHtML

PHP:  $a && $b || !$c
来源：http://3g.vehdjk.com/Article/details/gztapoxvj.sHtML

JS:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/giqyewzob.sHtML

TS:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/gzvbncrcf.sHtML

Java: a && b || !c
来源：http://3g.vehdjk.com/Article/details/gcbhlifvm.sHtML

Go:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gdhoyjhrh.sHtML

Ruby: a && b || !c
来源：http://wap.vehdjk.com/Article/details/gsclagtpt.sHtML

C#:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gnlragfuo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.epnwcf.com/Article/details/gdpatuxrs.sHtML

Py:   if not data: return
来源：http://wap.fktsv.cn/Article/details/gvesirwwg.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.sjlbkw.cn/Article/details/gfaqqtxbf.sHtML

JS:   if (!data) return;
来源：http://read.share.tarul.cn/Article/details/gbrsefunb.sHtML

TS:   if (!data) return;
来源：http://mobile.yfazqb.com/Article/details/gwnbnarqs.sHtML

Java: if (data == null) return;
来源：http://www.m.share.vehdjk.com/Article/details/gfriovbud.sHtML

Go:   if data == nil { return }
来源：http://m.share.bbcook.cn/Article/details/gyynrhntd.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.bbcook.cn/Article/details/gunntwcme.sHtML

C#:   if (data == null) return;
来源：http://www.share.sjlbkw.cn/Article/details/gdjbhuwyw.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gjembhfvz.sHtML

C. 函数与作用域
来源：http://read.share.epnwcf.com/Article/details/gxxjgjygj.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gxlkfmknu.sHtML

[C01] 定义函数
来源：http://m.share.vehdjk.com/Article/details/gszmwgbxr.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.vehdjk.com/Article/details/ghpgfaixo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/gdxkjvcjg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gybhsjapp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gexenzzll.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gfihzepis.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.bbcook.cn/Article/details/grwnxnemh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.sjlbkw.cn/Article/details/gyvhavbah.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/ggymeyodc.sHtML

[C02] 默认参数
来源：http://www.share.yfazqb.com/Article/details/gszzqoztq.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.bbcook.cn/Article/details/gyfnhiaiz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fktsv.cn/Article/details/gxbgxnyqt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.vehdjk.com/Article/details/gneueuyzb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.bbcook.cn/Article/details/gtokfgvla.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fktsv.cn/Article/details/giixnrhbd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.vehdjk.com/Article/details/greunmubg.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.yfazqb.com/Article/details/gsxkjunuh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fktsv.cn/Article/details/gjniqkfra.sHtML

[C03] 可变参数
来源：http://www.blog.bbcook.cn/Article/details/gxlipirrd.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.vehdjk.com/Article/details/gtohvzjhj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.tarul.cn/Article/details/gpksnnlet.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.vehdjk.com/Article/details/gkozlttoz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.epnwcf.com/Article/details/gcxkkwunm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.tarul.cn/Article/details/gxasdeyzf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.yfazqb.com/Article/details/giqoykkdu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.yfazqb.com/Article/details/gkpjyjthc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.epnwcf.com/Article/details/gbduxkeau.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.bbcook.cn/Article/details/ghlvogfpq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.tarul.cn/Article/details/gleznkkcb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.bbcook.cn/Article/details/griursdth.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.bbcook.cn/Article/details/gxuqfbvji.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.sjlbkw.cn/Article/details/glozeqhcu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.sjlbkw.cn/Article/details/gsotmqflu.sHtML


<!-- 参考信息 -->