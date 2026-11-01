代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://read.share.sjlbkw.cn/Article/details/gviucnalk.sHtML

[A15] 空值判断与默认值
来源：http://baike.bbcook.cn/Article/details/gsjodwpxz.sHtML

Py:   value = data or "默认值"
来源：http://read.share.bbcook.cn/Article/details/gzmqhdwmz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.vehdjk.com/Article/details/gtuowqnlw.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fktsv.cn/Article/details/glyokazxy.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.sjlbkw.cn/Article/details/gglugdcyn.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.yfazqb.com/Article/details/gafefgktw.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gectjpujn.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.sjlbkw.cn/Article/details/gmdlhcgvs.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.bbcook.cn/Article/details/gdsfvuxsk.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.fktsv.cn/Article/details/gxmpfzvqn.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.sjlbkw.cn/Article/details/gomultmmu.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.epnwcf.com/Article/details/gclopnigc.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.bbcook.cn/Article/details/gbfpbzklq.sHtML

TS:   if (!x) {}
来源：http://www.share.sjlbkw.cn/Article/details/gjgbulleb.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.vehdjk.com/Article/details/ghuthucfa.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.tarul.cn/Article/details/gxvtqzkdf.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.epnwcf.com/Article/details/gflybeufw.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.sjlbkw.cn/Article/details/gohscjyep.sHtML

[A17] 位运算
来源：http://3g.tarul.cn/Article/details/grgcyxmqf.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/gthsyorej.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.tarul.cn/Article/details/gemkgzteu.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.sjlbkw.cn/Article/details/gzimvbjrz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.vehdjk.com/Article/details/gpinzbmss.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.yfazqb.com/Article/details/gfynwsnmk.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/gpznktvlg.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/gkbexlibn.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.sjlbkw.cn/Article/details/genrjwheo.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.yfazqb.com/Article/details/garqepkzr.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.fktsv.cn/Article/details/gnnvmbbwb.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.fktsv.cn/Article/details/gspbnslvl.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.bbcook.cn/Article/details/giwjmkvhk.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.sjlbkw.cn/Article/details/gxitzerfq.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.sjlbkw.cn/Article/details/gzlpwiagm.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.sjlbkw.cn/Article/details/gskuwqshz.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.tarul.cn/Article/details/gfiulyhrm.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.vehdjk.com/Article/details/gzofuukqw.sHtML

[A19] 交换两个变量
来源：http://wap.bbcook.cn/Article/details/gxsbltcgb.sHtML

Py:   a, b = b, a
来源：http://baike.sjlbkw.cn/Article/details/gdibgjgru.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.sjlbkw.cn/Article/details/gyfcqnkcm.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.bbcook.cn/Article/details/gxppbtfeb.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.epnwcf.com/Article/details/gnhofovyz.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.tarul.cn/Article/details/guhukejbr.sHtML

Go:   a, b = b, a
来源：http://www.blog.epnwcf.com/Article/details/gxhuaxmbb.sHtML

Ruby: a, b = b, a
来源：http://m.share.tarul.cn/Article/details/gxyvsjpwy.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.epnwcf.com/Article/details/gsvfkulne.sHtML

[A20] 读取标准输入
来源：http://www.blog.fktsv.cn/Article/details/gkhvmpamn.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.bbcook.cn/Article/details/gtrkgucuf.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.bbcook.cn/Article/details/gixefmcvh.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.tarul.cn/Article/details/gxtloawce.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.bbcook.cn/Article/details/goqvhplud.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.epnwcf.com/Article/details/gridmdmrf.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.bbcook.cn/Article/details/giohdorta.sHtML

Ruby: gets.chomp
来源：http://m.share.epnwcf.com/Article/details/gyhwnkldj.sHtML

C#:   Console.ReadLine();
来源：http://3g.epnwcf.com/Article/details/gcxtpzqgf.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.fktsv.cn/Article/details/ggcobddyl.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.fktsv.cn/Article/details/gmqbhvnvr.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.epnwcf.com/Article/details/gyakxkcru.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.yfazqb.com/Article/details/gzfrnriva.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.bbcook.cn/Article/details/ghagaqvam.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.sjlbkw.cn/Article/details/gujpwrlzw.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.tarul.cn/Article/details/gyvczvcpo.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.sjlbkw.cn/Article/details/gztfivuhz.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.tarul.cn/Article/details/gvhfkxthk.sHtML

[A22] 获取字符串长度
来源：http://blog.bbcook.cn/Article/details/gjavbtptv.sHtML

Py:   len(s)
来源：http://3g.yfazqb.com/Article/details/gicegwdow.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.yfazqb.com/Article/details/ghceotspk.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.fktsv.cn/Article/details/gohyewzsq.sHtML

TS:   s.length
来源：http://read.share.sjlbkw.cn/Article/details/gwgyqixoi.sHtML

Java: s.length()
来源：http://read.share.sjlbkw.cn/Article/details/gbbynvpsu.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.tarul.cn/Article/details/gundqewgv.sHtML

Ruby: s.length
来源：http://www.share.bbcook.cn/Article/details/grrebowwc.sHtML

C#:   s.Length
来源：http://m.share.yfazqb.com/Article/details/gzrijecci.sHtML

[A23] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/gdaowgvvv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.epnwcf.com/Article/details/gbqlrkuea.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.epnwcf.com/Article/details/gfoojhxtz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.bbcook.cn/Article/details/goxbdkybf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.sjlbkw.cn/Article/details/gjlrxhmki.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.sjlbkw.cn/Article/details/gzkqjmcww.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.epnwcf.com/Article/details/gpsahemal.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.vehdjk.com/Article/details/gknuneaki.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.bbcook.cn/Article/details/gyzuvivnu.sHtML

[A24] 去除首尾空白
来源：http://wap.tarul.cn/Article/details/gxfpfwmkg.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fktsv.cn/Article/details/gqfgqnbqv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.fktsv.cn/Article/details/gjcssbnqx.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.tarul.cn/Article/details/gzvklxycj.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fktsv.cn/Article/details/gknuvoluh.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.fktsv.cn/Article/details/gdbqvmgiv.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.tarul.cn/Article/details/gekjfzudy.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.bbcook.cn/Article/details/goaucfzwk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.vehdjk.com/Article/details/gqsixpxwr.sHtML

[A25] 字符串比较
来源：http://www.share.yfazqb.com/Article/details/gaufddtrd.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.epnwcf.com/Article/details/ggpitcvwx.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.tarul.cn/Article/details/ghyuwyybg.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.sjlbkw.cn/Article/details/gwodhtapb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.sjlbkw.cn/Article/details/gelpskrej.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.sjlbkw.cn/Article/details/gcpomapco.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.vehdjk.com/Article/details/gxkegvaak.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.yfazqb.com/Article/details/gfxfixwoy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.vehdjk.com/Article/details/grwanjcug.sHtML

[A26] 类型转换总览
来源：http://m.share.fktsv.cn/Article/details/gfdigmtso.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.bbcook.cn/Article/details/gwjfaxdvo.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.tarul.cn/Article/details/gbuevbbuq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.vehdjk.com/Article/details/gamkrvtku.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.bbcook.cn/Article/details/gxytgxmbn.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.yfazqb.com/Article/details/gwguryhsy.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.bbcook.cn/Article/details/gkzlhwcqq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.fktsv.cn/Article/details/gjhqpveqy.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.bbcook.cn/Article/details/gywkwvehc.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gahybtboj.sHtML

B. 流程控制
来源：http://m.share.vehdjk.com/Article/details/gqnydeipz.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gzyxrwwtj.sHtML

[B01] 条件判断 if / else
来源：http://baike.fktsv.cn/Article/details/gtpgnzlak.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.vehdjk.com/Article/details/gqshnfjly.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.bbcook.cn/Article/details/gsdnrruvz.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.tarul.cn/Article/details/giubhcrnt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.bbcook.cn/Article/details/gnyiuqniq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.bbcook.cn/Article/details/gflejdtrv.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.yfazqb.com/Article/details/gdeosguuu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.epnwcf.com/Article/details/gzlgblaix.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.tarul.cn/Article/details/ghmylvujh.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.bbcook.cn/Article/details/gxetrjtyt.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.vehdjk.com/Article/details/gmyoukaau.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.vehdjk.com/Article/details/gfgwbibni.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.bbcook.cn/Article/details/gptkeeagq.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/gfwauzytk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/gmojdlyrf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fktsv.cn/Article/details/gplrtblgd.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.bbcook.cn/Article/details/gwdtnglum.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fktsv.cn/Article/details/gdmblbawm.sHtML

[B03] switch / match / case
来源：http://baike.fktsv.cn/Article/details/gntvkainz.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.fktsv.cn/Article/details/gopumdoqj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/gcfdkfcvt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/ghvewview.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.bbcook.cn/Article/details/gniodcagq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.sjlbkw.cn/Article/details/gfwvsugcy.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.bbcook.cn/Article/details/golyzczcl.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgkdgarf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.tarul.cn/Article/details/gbbinxfhc.sHtML

[B04] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/gmllawnxz.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.bbcook.cn/Article/details/gjmdidecd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.bbcook.cn/Article/details/gzvjdsahi.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.epnwcf.com/Article/details/gbhfungmq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.bbcook.cn/Article/details/gmpmjvkut.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.fktsv.cn/Article/details/gmkwzltna.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.bbcook.cn/Article/details/gkmbczbgz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.epnwcf.com/Article/details/gbsapvqrn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.sjlbkw.cn/Article/details/gkdbpjbqn.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.vehdjk.com/Article/details/gkdfiobri.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.yfazqb.com/Article/details/grczmdejm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.vehdjk.com/Article/details/gozzmbwgt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.vehdjk.com/Article/details/gdqugtmjm.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fktsv.cn/Article/details/gujjdyyaa.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fktsv.cn/Article/details/gzutsvweb.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.bbcook.cn/Article/details/gydpikejf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.sjlbkw.cn/Article/details/gpzzjlimv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.vehdjk.com/Article/details/gdoyevhws.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.epnwcf.com/Article/details/gwaofffld.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.tarul.cn/Article/details/gjifgllnf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.tarul.cn/Article/details/gvcecnlyr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.sjlbkw.cn/Article/details/gyomkvdko.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.yfazqb.com/Article/details/gryejkwnd.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.yfazqb.com/Article/details/gucrkecyx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fktsv.cn/Article/details/ggtounqdh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.vehdjk.com/Article/details/gvurkggqx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fktsv.cn/Article/details/gjvfthyfr.sHtML

[B07] while 循环
来源：http://wap.fktsv.cn/Article/details/ggwoygdlu.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fktsv.cn/Article/details/gjpbgzczn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fktsv.cn/Article/details/gzgtdujui.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/gdkpjkjih.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/gywmigqpk.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gomliusxn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.tarul.cn/Article/details/gqxnvuqem.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.tarul.cn/Article/details/gdpqxvjwk.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gukpcpieg.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.vehdjk.com/Article/details/gcgtfcwyq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.epnwcf.com/Article/details/glleqmefk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.tarul.cn/Article/details/gqaopgftm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gneelhpqh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/gjgrazabb.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gdcbxsunr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.tarul.cn/Article/details/gomxsrdsf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.epnwcf.com/Article/details/gjzqsdfqg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/gjrepwfdu.sHtML

[B09] break 与 continue
来源：http://m.share.epnwcf.com/Article/details/gsxmeheon.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.yfazqb.com/Article/details/gjtdovbfx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gwtfzbosq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gstehgtoh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gahhleixk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gglfgaguy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.epnwcf.com/Article/details/ggjtjiorr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fktsv.cn/Article/details/glzfschff.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/gyypjxdqt.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.epnwcf.com/Article/details/gipyylwip.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.yfazqb.com/Article/details/gprokoowe.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.yfazqb.com/Article/details/gyswbfmca.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fktsv.cn/Article/details/gkhebnaeg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.yfazqb.com/Article/details/guecwzwdx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fktsv.cn/Article/details/gsxidoqsa.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fktsv.cn/Article/details/glvyavjne.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fktsv.cn/Article/details/gtpraesxo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.sjlbkw.cn/Article/details/ggeixhdfa.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.sjlbkw.cn/Article/details/gceoyastk.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.yfazqb.com/Article/details/gsbxgrkkd.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.sjlbkw.cn/Article/details/gksopwqmv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.bbcook.cn/Article/details/gnpayvedg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fktsv.cn/Article/details/gvhzfyttw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.sjlbkw.cn/Article/details/glroxmxur.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.epnwcf.com/Article/details/ghgvleokw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.yfazqb.com/Article/details/ghmdsancr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.yfazqb.com/Article/details/gyhloavpe.sHtML

[B12] 跳出多层循环
来源：http://m.share.yfazqb.com/Article/details/gjlujyebb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.epnwcf.com/Article/details/gdvtvnhqh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fktsv.cn/Article/details/gvmyljylu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.tarul.cn/Article/details/gujhstixg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.epnwcf.com/Article/details/gduczuwto.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.yfazqb.com/Article/details/gztquelds.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.bbcook.cn/Article/details/gonwoqfcj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.tarul.cn/Article/details/gppudsuhh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.vehdjk.com/Article/details/ghgvnupdb.sHtML

[B13] 判断是否为数字
来源：http://read.share.epnwcf.com/Article/details/gylljmjki.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.yfazqb.com/Article/details/gggnugoio.sHtML

PHP:  is_numeric($x)
来源：http://3g.yfazqb.com/Article/details/gkgbthqai.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fktsv.cn/Article/details/gdlrkyrqk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.tarul.cn/Article/details/glyiwjuis.sHtML

Java: x instanceof Number
来源：http://read.share.epnwcf.com/Article/details/gouoilzyj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.yfazqb.com/Article/details/gijadekmz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.tarul.cn/Article/details/gmxquouxk.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fktsv.cn/Article/details/gtaisxoqr.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.bbcook.cn/Article/details/gvqrycmzy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fktsv.cn/Article/details/gdlzazbpm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.vehdjk.com/Article/details/gcpqriixo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.epnwcf.com/Article/details/gyphycssp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.vehdjk.com/Article/details/gemyujuww.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.bbcook.cn/Article/details/gufyifmbw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fktsv.cn/Article/details/giutdjnhp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.epnwcf.com/Article/details/gnvtqgoqe.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.epnwcf.com/Article/details/gofbqbsym.sHtML

[B15] 布尔运算与取反
来源：http://blog.sjlbkw.cn/Article/details/gdkikgvxy.sHtML

Py:   a and b or not c
来源：http://3g.bbcook.cn/Article/details/gmgfbhtxo.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.tarul.cn/Article/details/gclitxjzx.sHtML

JS:   a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gwqmtddlf.sHtML

TS:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/guyeggguy.sHtML

Java: a && b || !c
来源：http://blog.yfazqb.com/Article/details/ggeusdmmc.sHtML

Go:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gnrqmjmpf.sHtML

Ruby: a && b || !c
来源：http://wap.epnwcf.com/Article/details/gkkncbibl.sHtML

C#:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gxnreqwgm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.sjlbkw.cn/Article/details/gqdxcvsnk.sHtML

Py:   if not data: return
来源：http://www.share.tarul.cn/Article/details/gdqfhhhte.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.epnwcf.com/Article/details/gqknyqnuq.sHtML

JS:   if (!data) return;
来源：http://baike.sjlbkw.cn/Article/details/givthziga.sHtML

TS:   if (!data) return;
来源：http://wap.sjlbkw.cn/Article/details/giyweysmn.sHtML

Java: if (data == null) return;
来源：http://www.m.share.yfazqb.com/Article/details/gacrbydmg.sHtML

Go:   if data == nil { return }
来源：http://read.share.sjlbkw.cn/Article/details/gjnhbonux.sHtML

Ruby: return if data.nil?
来源：http://www.share.fktsv.cn/Article/details/gdjdarmae.sHtML

C#:   if (data == null) return;
来源：http://read.share.bbcook.cn/Article/details/gvearxkro.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/glslaxhnc.sHtML

C. 函数与作用域
来源：http://baike.epnwcf.com/Article/details/gsvemslef.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gwhdkbgoe.sHtML

[C01] 定义函数
来源：http://www.m.share.epnwcf.com/Article/details/getgcaxdo.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.vehdjk.com/Article/details/gndecwpdf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/ghhjbrsqb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gnvmqzpeg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gkwspijac.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gjafxfdup.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.epnwcf.com/Article/details/gcbjwvgct.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.yfazqb.com/Article/details/gmetbdigv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/ginvcfnqt.sHtML

[C02] 默认参数
来源：http://baike.bbcook.cn/Article/details/geasisyyq.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.tarul.cn/Article/details/goflqzlbk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.bbcook.cn/Article/details/gegckfsnz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gfwgarkiq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.epnwcf.com/Article/details/glwbtfusr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.vehdjk.com/Article/details/giratdxqp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.vehdjk.com/Article/details/gebwdgmfn.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.vehdjk.com/Article/details/gktrcnqpc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fktsv.cn/Article/details/gdlotpwos.sHtML

[C03] 可变参数
来源：http://baike.yfazqb.com/Article/details/gjbyqxyyt.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.tarul.cn/Article/details/gxwpgavfw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.tarul.cn/Article/details/gpyfpfzry.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.sjlbkw.cn/Article/details/grxttvnlc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.sjlbkw.cn/Article/details/gsizuifhc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.yfazqb.com/Article/details/gtbwhxvwc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fktsv.cn/Article/details/guxuzeomf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.bbcook.cn/Article/details/ggttolqqa.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.sjlbkw.cn/Article/details/ggezypxfx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.vehdjk.com/Article/details/gtawjyhkk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.bbcook.cn/Article/details/gqxpkngpx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fktsv.cn/Article/details/gylxgwcog.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.yfazqb.com/Article/details/gxrdtdnwl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.bbcook.cn/Article/details/gdxqrspnh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.bbcook.cn/Article/details/gsezxnkbs.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.sjlbkw.cn/Article/details/gxidgamoh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gqyfdrnuc.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.sjlbkw.cn/Article/details/gfsvpnsjj.sHtML

[C05] 返回多个值
来源：http://www.m.share.tarul.cn/Article/details/gsytxdlmg.sHtML

Py:   return a, b
来源：http://www.share.vehdjk.com/Article/details/gzwwqcvgg.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fktsv.cn/Article/details/gxlxwnaim.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.bbcook.cn/Article/details/gxdzhrkhk.sHtML

TS:   return { a, b };
来源：http://m.share.bbcook.cn/Article/details/gvrmkqxci.sHtML


<!-- 参考信息 -->