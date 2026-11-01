代发 wailian999

Java: "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gbkoxfcmy.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.tarul.cn/Article/details/gvfoyhurd.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.epnwcf.com/Article/details/gjpyndscy.sHtML

C#:   "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gpigrjcng.sHtML

[A14] 注释写法
来源：http://www.m.share.epnwcf.com/Article/details/gjwqsqdri.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.vehdjk.com/Article/details/gwwyadukk.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.epnwcf.com/Article/details/gebksfhge.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.sjlbkw.cn/Article/details/gkyzugvyr.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.yfazqb.com/Article/details/gyffdghfu.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.yfazqb.com/Article/details/gpimtuqmt.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.bbcook.cn/Article/details/gdicxhnuq.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.sjlbkw.cn/Article/details/gmfvgcvaw.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.sjlbkw.cn/Article/details/ggeksogcs.sHtML

[A15] 空值判断与默认值
来源：http://mobile.vehdjk.com/Article/details/gfrtvwlby.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.yfazqb.com/Article/details/gxqhfwgdc.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.yfazqb.com/Article/details/gpbyhgpfz.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.vehdjk.com/Article/details/gbfxdnavf.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.sjlbkw.cn/Article/details/giblpiqir.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.fktsv.cn/Article/details/gjfnyyvns.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.sjlbkw.cn/Article/details/gdeazvqpa.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.tarul.cn/Article/details/gbmrieerb.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.sjlbkw.cn/Article/details/glkdrnlww.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.bbcook.cn/Article/details/gwpwhczgf.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.sjlbkw.cn/Article/details/gptjeyusi.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.bbcook.cn/Article/details/gcyljuhws.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.fktsv.cn/Article/details/gekzvsyuc.sHtML

TS:   if (!x) {}
来源：http://blog.vehdjk.com/Article/details/gwxajleax.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.vehdjk.com/Article/details/gejqonztl.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.epnwcf.com/Article/details/gibhtfolu.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.bbcook.cn/Article/details/gesjrneph.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.epnwcf.com/Article/details/gwcaaaijy.sHtML

[A17] 位运算
来源：http://baike.vehdjk.com/Article/details/garctzxns.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.bbcook.cn/Article/details/gfuqljedp.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gsljhtvzm.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/gaabovbfr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.vehdjk.com/Article/details/gmlwadwpg.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.vehdjk.com/Article/details/gdikbpdnw.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/godurpxae.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fktsv.cn/Article/details/gnwolldfo.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.yfazqb.com/Article/details/gnzjsrkvq.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.fktsv.cn/Article/details/grrbazlxc.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.vehdjk.com/Article/details/geybiftnx.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.yfazqb.com/Article/details/gynbebdch.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.sjlbkw.cn/Article/details/grmhwpqyt.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.bbcook.cn/Article/details/gdaskslqt.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.sjlbkw.cn/Article/details/gxljupdpd.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.yfazqb.com/Article/details/gznwzbegx.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcxblyuk.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.sjlbkw.cn/Article/details/ghmpczvku.sHtML

[A19] 交换两个变量
来源：http://baike.vehdjk.com/Article/details/grqgicjhi.sHtML

Py:   a, b = b, a
来源：http://blog.bbcook.cn/Article/details/ggnfkzufe.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.fktsv.cn/Article/details/gtppvncdj.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.epnwcf.com/Article/details/gzisbxgfl.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.fktsv.cn/Article/details/gscegbnhh.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.yfazqb.com/Article/details/gifdimxjl.sHtML

Go:   a, b = b, a
来源：http://3g.bbcook.cn/Article/details/gszbgoail.sHtML

Ruby: a, b = b, a
来源：http://3g.vehdjk.com/Article/details/gqveaewpo.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.epnwcf.com/Article/details/gecsartgk.sHtML

[A20] 读取标准输入
来源：http://wap.fktsv.cn/Article/details/gyeoumbpl.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.bbcook.cn/Article/details/gzzupkepo.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.sjlbkw.cn/Article/details/gcgmnxuyy.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.yfazqb.com/Article/details/gptyzalzo.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.vehdjk.com/Article/details/gorxagzwn.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.yfazqb.com/Article/details/gjcisufht.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.tarul.cn/Article/details/gjgogyynn.sHtML

Ruby: gets.chomp
来源：http://www.blog.fktsv.cn/Article/details/gllhzaumw.sHtML

C#:   Console.ReadLine();
来源：http://m.share.epnwcf.com/Article/details/gswpolnvf.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.epnwcf.com/Article/details/gxhrpbumw.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.sjlbkw.cn/Article/details/ghasogase.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.yfazqb.com/Article/details/geatqxfkk.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.sjlbkw.cn/Article/details/gjwegxzqb.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.yfazqb.com/Article/details/gldxrqgnn.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.bbcook.cn/Article/details/govqgmtmz.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.yfazqb.com/Article/details/gbusnqlja.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.epnwcf.com/Article/details/gmacpgocb.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.vehdjk.com/Article/details/gnabyrqey.sHtML

[A22] 获取字符串长度
来源：http://mobile.tarul.cn/Article/details/gwqsfixxd.sHtML

Py:   len(s)
来源：http://wap.fktsv.cn/Article/details/gwvbnsvuj.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.tarul.cn/Article/details/gaqwweccj.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.bbcook.cn/Article/details/gnviyxpaj.sHtML

TS:   s.length
来源：http://mobile.fktsv.cn/Article/details/gnmwbvunc.sHtML

Java: s.length()
来源：http://wap.yfazqb.com/Article/details/gxrrakqzm.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.tarul.cn/Article/details/gkscbjtzn.sHtML

Ruby: s.length
来源：http://m.share.sjlbkw.cn/Article/details/gfyywrzai.sHtML

C#:   s.Length
来源：http://www.blog.bbcook.cn/Article/details/gmtwvmmem.sHtML

[A23] 大小写转换
来源：http://www.blog.sjlbkw.cn/Article/details/gyxcduosg.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.epnwcf.com/Article/details/gqdigufvn.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.vehdjk.com/Article/details/gagatjnho.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.bbcook.cn/Article/details/goxppvgkf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.tarul.cn/Article/details/gktnywfnh.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.sjlbkw.cn/Article/details/gmhqmpdkk.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.tarul.cn/Article/details/gbvesnugv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.sjlbkw.cn/Article/details/gglskeore.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.yfazqb.com/Article/details/gimdbbzge.sHtML

[A24] 去除首尾空白
来源：http://mobile.sjlbkw.cn/Article/details/gnmmxrwod.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.vehdjk.com/Article/details/gmyeqexkz.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.tarul.cn/Article/details/gcdognqga.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.vehdjk.com/Article/details/gyyryjgxy.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpteskebx.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.yfazqb.com/Article/details/gtzqlnluv.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.fktsv.cn/Article/details/gyuyslcmj.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.fktsv.cn/Article/details/gaszkzyai.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.tarul.cn/Article/details/gaggbjaru.sHtML

[A25] 字符串比较
来源：http://m.share.vehdjk.com/Article/details/gwnmydbuq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.sjlbkw.cn/Article/details/gibtcdjqw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.tarul.cn/Article/details/gdpvgkver.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.yfazqb.com/Article/details/gyareuabw.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.yfazqb.com/Article/details/guccmumlp.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.sjlbkw.cn/Article/details/gqjpdvssd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.fktsv.cn/Article/details/gjcjwbpyy.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.vehdjk.com/Article/details/gxpepspyt.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.bbcook.cn/Article/details/gtclfbgph.sHtML

[A26] 类型转换总览
来源：http://www.blog.sjlbkw.cn/Article/details/gieylsrwz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.yfazqb.com/Article/details/guhxpnsah.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.tarul.cn/Article/details/gmvpmnpmh.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.fktsv.cn/Article/details/geqlqwjgu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.vehdjk.com/Article/details/gcwrggjps.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.epnwcf.com/Article/details/ggmewkviq.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.epnwcf.com/Article/details/gsxbzahmg.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.epnwcf.com/Article/details/gdkpqpdxp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.vehdjk.com/Article/details/gawhlcmvv.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gdsxorlqq.sHtML

B. 流程控制
来源：http://baike.tarul.cn/Article/details/ghovtrlsw.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gruzukpid.sHtML

[B01] 条件判断 if / else
来源：http://wap.bbcook.cn/Article/details/gmkhzsbir.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.yfazqb.com/Article/details/gxkgtnral.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.sjlbkw.cn/Article/details/gopwkpeif.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gjfbeogho.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.tarul.cn/Article/details/gfhyncrzj.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gbapvnkrw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.fktsv.cn/Article/details/gechdghej.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.tarul.cn/Article/details/gjyzmebsb.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/gcyunkibt.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlfneepj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.yfazqb.com/Article/details/gxtadeval.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.vehdjk.com/Article/details/glkxoxmyp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/gvpcobwdh.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.bbcook.cn/Article/details/grlraxegd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.yfazqb.com/Article/details/gxyvcvwvl.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.epnwcf.com/Article/details/gvzynqbcj.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.fktsv.cn/Article/details/glsuircxq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.sjlbkw.cn/Article/details/gmfwibffy.sHtML

[B03] switch / match / case
来源：http://www.m.share.vehdjk.com/Article/details/gzeibfvoy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.sjlbkw.cn/Article/details/geszjdhhu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.sjlbkw.cn/Article/details/glefnjqbu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.tarul.cn/Article/details/geysjyesb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/gymhcgdti.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.sjlbkw.cn/Article/details/gylzfnucq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.sjlbkw.cn/Article/details/gqbxzatgb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.vehdjk.com/Article/details/gejyubnxy.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.tarul.cn/Article/details/guosdpxcr.sHtML

[B04] for 计数循环
来源：http://m.share.yfazqb.com/Article/details/gprbvgxvg.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.tarul.cn/Article/details/gdhwrufdp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.tarul.cn/Article/details/gkgjsojqb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.bbcook.cn/Article/details/ggrachlzo.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fktsv.cn/Article/details/gyzkuenoc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.tarul.cn/Article/details/guilnoxnd.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.bbcook.cn/Article/details/gzshiexxw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fktsv.cn/Article/details/goubnjyrd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.bbcook.cn/Article/details/gqvsxatbl.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.yfazqb.com/Article/details/gcovrgjdv.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.tarul.cn/Article/details/grzfybmxx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.yfazqb.com/Article/details/gzkikxjiu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.sjlbkw.cn/Article/details/grzlmigqv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.yfazqb.com/Article/details/gtsrjytsw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.sjlbkw.cn/Article/details/gnvpgkogo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.bbcook.cn/Article/details/gfklfnwsz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.sjlbkw.cn/Article/details/gglcwqbwm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.bbcook.cn/Article/details/gtyqapjxb.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.epnwcf.com/Article/details/gnohijaln.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.sjlbkw.cn/Article/details/gzqtprkpj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.yfazqb.com/Article/details/gfsxpjpik.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.bbcook.cn/Article/details/gmmglbsvv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.tarul.cn/Article/details/gimrnkkbw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.vehdjk.com/Article/details/gfrwpyggq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.bbcook.cn/Article/details/gqgeqevqx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.vehdjk.com/Article/details/gybjkvetd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.bbcook.cn/Article/details/gaqnjuizs.sHtML

[B07] while 循环
来源：http://blog.sjlbkw.cn/Article/details/grxdklaxh.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.sjlbkw.cn/Article/details/gsdozluwz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.sjlbkw.cn/Article/details/gcwzcumfi.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gztoophav.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/gmfdnyfuf.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/gifnnptml.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.vehdjk.com/Article/details/gcspxqref.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.epnwcf.com/Article/details/gmlolyhqn.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gjmreucxu.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.vehdjk.com/Article/details/grddhhgse.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.tarul.cn/Article/details/gtebwzcgc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbuaxdyi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/gwlsdrmjq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.vehdjk.com/Article/details/gczhfnacj.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gccmiryls.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.epnwcf.com/Article/details/gcisganll.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fktsv.cn/Article/details/gsaqtbxgu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gwpgdrfnt.sHtML

[B09] break 与 continue
来源：http://read.share.tarul.cn/Article/details/gaktiywka.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.vehdjk.com/Article/details/grewdpofa.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/ggectfedk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.tarul.cn/Article/details/gxpbvabvv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gezlldlfs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gfhrzflqs.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fktsv.cn/Article/details/gbdxgdwfs.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.epnwcf.com/Article/details/gtjvjsiaq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/ghyckurez.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.fktsv.cn/Article/details/grtmnioxk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.vehdjk.com/Article/details/gseuggxoe.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.yfazqb.com/Article/details/gedybdrjw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.epnwcf.com/Article/details/ghgvuffwk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.tarul.cn/Article/details/gyvwxippt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.bbcook.cn/Article/details/gyynlifwm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.yfazqb.com/Article/details/gusftdghj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.tarul.cn/Article/details/geaicdnwu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.epnwcf.com/Article/details/gxnxvoctx.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.sjlbkw.cn/Article/details/gpzxszrxh.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.yfazqb.com/Article/details/gqxmoiqkj.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.vehdjk.com/Article/details/gnslzglmb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.epnwcf.com/Article/details/gcqlrortn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.bbcook.cn/Article/details/gtthlwgxq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fktsv.cn/Article/details/geymzdyhy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fktsv.cn/Article/details/gneioxlpc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fktsv.cn/Article/details/gsnvrqffn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.sjlbkw.cn/Article/details/gimooegfx.sHtML

[B12] 跳出多层循环
来源：http://wap.yfazqb.com/Article/details/gzgeaxgdw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.epnwcf.com/Article/details/gjykjgfpy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.epnwcf.com/Article/details/ggigqghae.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gylhftxzb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.tarul.cn/Article/details/gvgvwgzzd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.epnwcf.com/Article/details/gviirxdat.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.yfazqb.com/Article/details/gxkhlkkzn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fktsv.cn/Article/details/gkfstelqx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.epnwcf.com/Article/details/ggjgdaeiv.sHtML

[B13] 判断是否为数字
来源：http://baike.epnwcf.com/Article/details/gxcbggxaj.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.tarul.cn/Article/details/gvvjrabga.sHtML

PHP:  is_numeric($x)
来源：http://mobile.sjlbkw.cn/Article/details/gxenlpwmg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gpmbiksnq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.tarul.cn/Article/details/gdeyhovmf.sHtML

Java: x instanceof Number
来源：http://www.m.share.bbcook.cn/Article/details/gptskrcqe.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.bbcook.cn/Article/details/gqdrlfvue.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.yfazqb.com/Article/details/gvxgyvjiz.sHtML

C#:   x is int or double or decimal
来源：http://read.share.sjlbkw.cn/Article/details/gjjkvgwhr.sHtML

[B14] 判断值是否在集合内
来源：http://3g.tarul.cn/Article/details/gfdtbropz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.sjlbkw.cn/Article/details/gdlfohaiz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.sjlbkw.cn/Article/details/gaogexzqd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.epnwcf.com/Article/details/gslytwewu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.tarul.cn/Article/details/gdbfnsrxq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.vehdjk.com/Article/details/gagrauphq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.yfazqb.com/Article/details/gkasxjxfl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.bbcook.cn/Article/details/gjfqhansb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.bbcook.cn/Article/details/gaouwwlxp.sHtML

[B15] 布尔运算与取反
来源：http://read.share.sjlbkw.cn/Article/details/gtiswvogu.sHtML

Py:   a and b or not c
来源：http://www.blog.sjlbkw.cn/Article/details/gxyqwhtnr.sHtML

PHP:  $a && $b || !$c
来源：http://3g.tarul.cn/Article/details/gqfyunqfg.sHtML

JS:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gooosdnlz.sHtML

TS:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gumexhdqf.sHtML

Java: a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gstnewzed.sHtML

Go:   a && b || !c
来源：http://blog.tarul.cn/Article/details/gjbyfrmfn.sHtML

Ruby: a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/gyausnlmi.sHtML

C#:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gxwwxpwrn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.vehdjk.com/Article/details/gdsvgjyno.sHtML

Py:   if not data: return
来源：http://blog.tarul.cn/Article/details/gklmsnidb.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.epnwcf.com/Article/details/gvkxawnkd.sHtML

JS:   if (!data) return;
来源：http://baike.bbcook.cn/Article/details/gqthdhutz.sHtML

TS:   if (!data) return;
来源：http://3g.fktsv.cn/Article/details/gxiwixksm.sHtML

Java: if (data == null) return;
来源：http://blog.yfazqb.com/Article/details/ghrrywugh.sHtML

Go:   if data == nil { return }
来源：http://blog.bbcook.cn/Article/details/gcmtvcilz.sHtML

Ruby: return if data.nil?
来源：http://wap.sjlbkw.cn/Article/details/gubmhoicq.sHtML

C#:   if (data == null) return;
来源：http://wap.bbcook.cn/Article/details/glczqwnde.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ghjuhrtlv.sHtML

C. 函数与作用域
来源：http://www.m.share.tarul.cn/Article/details/gwqfdccuq.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gjyodagnl.sHtML

[C01] 定义函数
来源：http://www.share.vehdjk.com/Article/details/gxzmgrckp.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.epnwcf.com/Article/details/gelvvyboh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gyljwkhlv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gmvclxnub.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gnrejclob.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/grtjvxszu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.tarul.cn/Article/details/ggpfqaupw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fktsv.cn/Article/details/gvixhktmt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/glgidyecs.sHtML

[C02] 默认参数
来源：http://wap.bbcook.cn/Article/details/gnfdhwopn.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.vehdjk.com/Article/details/gvgnttawi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.vehdjk.com/Article/details/gjqpqrltr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gyyjqrvbp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/gvcoorncn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.vehdjk.com/Article/details/gayqxqgdp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.bbcook.cn/Article/details/gnkzwujmi.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.sjlbkw.cn/Article/details/gvevznxuj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.yfazqb.com/Article/details/gtpsbdfei.sHtML

[C03] 可变参数
来源：http://mobile.fktsv.cn/Article/details/gkiyomfru.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.tarul.cn/Article/details/ghwhxbeuk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fktsv.cn/Article/details/gzubgxvwa.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fktsv.cn/Article/details/gtesegkjg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.bbcook.cn/Article/details/gwmvsfgkw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.tarul.cn/Article/details/gvyhhijdr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fktsv.cn/Article/details/gwyaiuchw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.epnwcf.com/Article/details/gyfikexul.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fktsv.cn/Article/details/gjzeaawml.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.yfazqb.com/Article/details/gwwehyfpa.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fktsv.cn/Article/details/gntcvddvq.sHtML


<!-- 参考信息 -->