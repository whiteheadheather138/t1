代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.m.share.yfazqb.com/Article/details/gkutjgfxd.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.vehdjk.com/Article/details/gtlukzcln.sHtML

Py:   value = data or "默认值"
来源：http://read.share.tarul.cn/Article/details/grdsdvthn.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.bbcook.cn/Article/details/gtmzatydk.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.sjlbkw.cn/Article/details/gvuzvdqjc.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.vehdjk.com/Article/details/gpxulhvkz.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.tarul.cn/Article/details/ghzgfwyvf.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.tarul.cn/Article/details/geuhsvnwi.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.sjlbkw.cn/Article/details/gsefajtxb.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.tarul.cn/Article/details/grlmetgga.sHtML

[A16] 真假值判断规则
来源：http://www.share.epnwcf.com/Article/details/ghjggznzl.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.vehdjk.com/Article/details/gmmydlxle.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.yfazqb.com/Article/details/gszvaipco.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.tarul.cn/Article/details/gnuegqopa.sHtML

TS:   if (!x) {}
来源：http://blog.epnwcf.com/Article/details/gvburwaow.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.fktsv.cn/Article/details/griityxkp.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.epnwcf.com/Article/details/gubsiepam.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.bbcook.cn/Article/details/gfhlgioek.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.bbcook.cn/Article/details/gpwyuuewa.sHtML

[A17] 位运算
来源：http://blog.epnwcf.com/Article/details/gpmilkkzp.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.bbcook.cn/Article/details/gtclyengf.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.yfazqb.com/Article/details/gdxbkjban.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/gsflvxfhm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.bbcook.cn/Article/details/gbwszdcjp.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.vehdjk.com/Article/details/grzctfxta.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.tarul.cn/Article/details/gvqfjynde.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.yfazqb.com/Article/details/ghykwzzpn.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.epnwcf.com/Article/details/gainplego.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.sjlbkw.cn/Article/details/gxcwpifzl.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.tarul.cn/Article/details/gyzczvres.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.tarul.cn/Article/details/gjbffckhr.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.yfazqb.com/Article/details/gwdmnkhwl.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.epnwcf.com/Article/details/gsbwvsiff.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.tarul.cn/Article/details/ggsswnljj.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.vehdjk.com/Article/details/gbdnpcveu.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.vehdjk.com/Article/details/ghuagtwpw.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.fktsv.cn/Article/details/gyroukpbz.sHtML

[A19] 交换两个变量
来源：http://baike.bbcook.cn/Article/details/gahcjmqms.sHtML

Py:   a, b = b, a
来源：http://read.share.bbcook.cn/Article/details/govfyplml.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.epnwcf.com/Article/details/gvabcbhaw.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.fktsv.cn/Article/details/gihhlissn.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.tarul.cn/Article/details/gqsyvtfnb.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.sjlbkw.cn/Article/details/gpacqhdty.sHtML

Go:   a, b = b, a
来源：http://mobile.epnwcf.com/Article/details/guxazbjrw.sHtML

Ruby: a, b = b, a
来源：http://mobile.yfazqb.com/Article/details/ggaziicfx.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.fktsv.cn/Article/details/ghlsimtfq.sHtML

[A20] 读取标准输入
来源：http://baike.tarul.cn/Article/details/ghfznrcrx.sHtML

Py:   name = input("请输入：")
来源：http://www.share.tarul.cn/Article/details/gichdtzbt.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhaiskhh.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.tarul.cn/Article/details/gogxaryzt.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.sjlbkw.cn/Article/details/gpthfkfhh.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.vehdjk.com/Article/details/gldddfsmz.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.tarul.cn/Article/details/gyhvamksh.sHtML

Ruby: gets.chomp
来源：http://3g.tarul.cn/Article/details/gameowwzo.sHtML

C#:   Console.ReadLine();
来源：http://3g.epnwcf.com/Article/details/gyzzvrxba.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.fktsv.cn/Article/details/gqjetxxoq.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.epnwcf.com/Article/details/gsuntvdle.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.bbcook.cn/Article/details/gcsexqoyc.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.tarul.cn/Article/details/gitvyfpuq.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.fktsv.cn/Article/details/grprwoykb.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.fktsv.cn/Article/details/gtphuvwnv.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.bbcook.cn/Article/details/gvjuyqhdz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.vehdjk.com/Article/details/gyrbovzxu.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.vehdjk.com/Article/details/gpjtshdql.sHtML

[A22] 获取字符串长度
来源：http://3g.tarul.cn/Article/details/gmquzctla.sHtML

Py:   len(s)
来源：http://read.share.bbcook.cn/Article/details/gnuxnvyam.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.sjlbkw.cn/Article/details/gsuiwxfsc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.epnwcf.com/Article/details/gcqbrfobb.sHtML

TS:   s.length
来源：http://read.share.yfazqb.com/Article/details/gwwphtopk.sHtML

Java: s.length()
来源：http://blog.vehdjk.com/Article/details/gbdwlqdza.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.tarul.cn/Article/details/gpeeqerhh.sHtML

Ruby: s.length
来源：http://mobile.tarul.cn/Article/details/gsqldoted.sHtML

C#:   s.Length
来源：http://wap.epnwcf.com/Article/details/gfgjywuqb.sHtML

[A23] 大小写转换
来源：http://www.share.vehdjk.com/Article/details/ghnckxmxp.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.yfazqb.com/Article/details/ghenjfwal.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.tarul.cn/Article/details/gtmidwvme.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.tarul.cn/Article/details/gvwgwdfzr.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.epnwcf.com/Article/details/gyvbzaurf.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.bbcook.cn/Article/details/guoldfmdc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.bbcook.cn/Article/details/gqtigykrz.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.vehdjk.com/Article/details/getqsmvcx.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.fktsv.cn/Article/details/ghougkpxu.sHtML

[A24] 去除首尾空白
来源：http://read.share.fktsv.cn/Article/details/geveoqlhe.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.bbcook.cn/Article/details/gekruuhlv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.tarul.cn/Article/details/gneotofak.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.bbcook.cn/Article/details/gcpikfxru.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.yfazqb.com/Article/details/gouzvegbb.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.fktsv.cn/Article/details/gzkwcqbqn.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.vehdjk.com/Article/details/gnsqtmplu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.fktsv.cn/Article/details/gtpaetxkp.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.tarul.cn/Article/details/gesalwayb.sHtML

[A25] 字符串比较
来源：http://baike.vehdjk.com/Article/details/gneypgcsu.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.bbcook.cn/Article/details/gitglnpqe.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.fktsv.cn/Article/details/gqvyuilwa.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.bbcook.cn/Article/details/gyougttbt.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.epnwcf.com/Article/details/gqypyeamt.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.yfazqb.com/Article/details/gdxgpcuzy.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.epnwcf.com/Article/details/gewugkner.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.vehdjk.com/Article/details/gqlqqyqwv.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.tarul.cn/Article/details/gfaecygev.sHtML

[A26] 类型转换总览
来源：http://3g.bbcook.cn/Article/details/gwrhrqqtj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.yfazqb.com/Article/details/gqygwginf.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.vehdjk.com/Article/details/groakgnje.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fktsv.cn/Article/details/gblysrugn.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fktsv.cn/Article/details/gtetmhaub.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.sjlbkw.cn/Article/details/gbhwmwgok.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.sjlbkw.cn/Article/details/gbkzpzkxa.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.yfazqb.com/Article/details/guowxklnw.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.vehdjk.com/Article/details/ggvcjreke.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gupzdhqif.sHtML

B. 流程控制
来源：http://baike.vehdjk.com/Article/details/gjxxwtnqg.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gxrnwkqdk.sHtML

[B01] 条件判断 if / else
来源：http://3g.tarul.cn/Article/details/gejwmqnqh.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.epnwcf.com/Article/details/gzumqctwi.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.yfazqb.com/Article/details/gkggirltr.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.tarul.cn/Article/details/gclfpgkzt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.bbcook.cn/Article/details/gbjeabytb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/gqvmxgxfp.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.vehdjk.com/Article/details/ganhuuetd.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.bbcook.cn/Article/details/gjsnmjvfj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.vehdjk.com/Article/details/gmimyrkkj.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.bbcook.cn/Article/details/gvfgnxhxy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.bbcook.cn/Article/details/gbyttjzyg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.vehdjk.com/Article/details/gnqwdtqok.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.yfazqb.com/Article/details/gqwcsaaqp.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/gjitqxtyr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.bbcook.cn/Article/details/gxbfxafpt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fktsv.cn/Article/details/goqimcvhi.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.bbcook.cn/Article/details/gzzivridx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.yfazqb.com/Article/details/gpvuteplu.sHtML

[B03] switch / match / case
来源：http://mobile.fktsv.cn/Article/details/ghdbhkgwe.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.fktsv.cn/Article/details/gycodagkt.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhbninza.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/ghyuyghrx.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.epnwcf.com/Article/details/gsusflcan.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/gdikiiiwx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.tarul.cn/Article/details/gxacvnfqs.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.epnwcf.com/Article/details/gqvrfwjid.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.yfazqb.com/Article/details/glptpgkqq.sHtML

[B04] for 计数循环
来源：http://www.share.bbcook.cn/Article/details/gqdictmwi.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.tarul.cn/Article/details/grbcgavvv.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.yfazqb.com/Article/details/gobznlxlh.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.sjlbkw.cn/Article/details/gmxbppmko.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.tarul.cn/Article/details/gdxdrgbjj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.bbcook.cn/Article/details/gfnkbxocm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fktsv.cn/Article/details/gbimzofce.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.epnwcf.com/Article/details/gktenughg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.vehdjk.com/Article/details/gsdteocls.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.tarul.cn/Article/details/govyydray.sHtML

Py:   for item in arr: print(item)
来源：http://wap.tarul.cn/Article/details/gqxkcavso.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.yfazqb.com/Article/details/gmcsekgsc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.epnwcf.com/Article/details/gbgzielji.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.bbcook.cn/Article/details/gvmdcasds.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.epnwcf.com/Article/details/giruahzyr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.vehdjk.com/Article/details/gxmboybet.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.vehdjk.com/Article/details/gcktozskl.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.sjlbkw.cn/Article/details/gzltnxxvz.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.tarul.cn/Article/details/gpjzepfyr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.vehdjk.com/Article/details/gxwfyyucw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.vehdjk.com/Article/details/gopyxauup.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.epnwcf.com/Article/details/gpxcvdops.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.yfazqb.com/Article/details/gmvqmybxb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.yfazqb.com/Article/details/ggizyojzi.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.sjlbkw.cn/Article/details/gavnsdqot.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.yfazqb.com/Article/details/gzkqalujl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.epnwcf.com/Article/details/gjeusgjaw.sHtML

[B07] while 循环
来源：http://www.blog.sjlbkw.cn/Article/details/gkhulrhnl.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gegxeinav.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.yfazqb.com/Article/details/gmvvgnbcr.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/gzafehfnf.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.vehdjk.com/Article/details/ghsgvtttt.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/getcfnmde.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.bbcook.cn/Article/details/gmjjbpiin.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.sjlbkw.cn/Article/details/gwgxnfxsq.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/gkmmyfvys.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.epnwcf.com/Article/details/ghodungtr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.yfazqb.com/Article/details/gcnviprvt.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.sjlbkw.cn/Article/details/gubfnwvpc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcucdhrz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/grillyjaf.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gzjwfqtcb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.epnwcf.com/Article/details/grobvlknk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.sjlbkw.cn/Article/details/gvkkkyhoh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gltskxeff.sHtML

[B09] break 与 continue
来源：http://wap.tarul.cn/Article/details/gopllsapm.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.vehdjk.com/Article/details/gkpxmwbnk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gkxvbrood.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/gfebzmvff.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gviojoftb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/glvmksdnu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.bbcook.cn/Article/details/gkqujvyra.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.bbcook.cn/Article/details/gededlwyh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/gygxzlzku.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.yfazqb.com/Article/details/gsvoqyjyw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.epnwcf.com/Article/details/gkhavxtur.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.sjlbkw.cn/Article/details/grkgkksnw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.yfazqb.com/Article/details/gesnnoqzz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.yfazqb.com/Article/details/guvdyllaf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.tarul.cn/Article/details/glwbiuasl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.sjlbkw.cn/Article/details/goqhiquto.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.yfazqb.com/Article/details/gluhqdtva.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.tarul.cn/Article/details/ghtlsqyxw.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.sjlbkw.cn/Article/details/gwzzmajmm.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.tarul.cn/Article/details/gdqjvtmeg.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.epnwcf.com/Article/details/gvqpnpbxl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fktsv.cn/Article/details/gncfurobi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.tarul.cn/Article/details/gudrcrfrb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.epnwcf.com/Article/details/gzfwcraka.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.epnwcf.com/Article/details/gnciyhtzt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.epnwcf.com/Article/details/gijnoijmx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.vehdjk.com/Article/details/gdirudakq.sHtML

[B12] 跳出多层循环
来源：http://baike.epnwcf.com/Article/details/gavllhyhl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fktsv.cn/Article/details/guyetfxsk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.epnwcf.com/Article/details/gikovwhgp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.epnwcf.com/Article/details/gjvphzpuz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/gzzipxjhd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/gfiybftkl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.sjlbkw.cn/Article/details/gjyupzqna.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.epnwcf.com/Article/details/ghvcraqpb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.vehdjk.com/Article/details/gsufxwywj.sHtML

[B13] 判断是否为数字
来源：http://m.share.tarul.cn/Article/details/gsrzimrfa.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.sjlbkw.cn/Article/details/gobmpxbta.sHtML

PHP:  is_numeric($x)
来源：http://m.share.sjlbkw.cn/Article/details/gkybntsyf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.epnwcf.com/Article/details/gezrqhugy.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fktsv.cn/Article/details/gvkqqrhkn.sHtML

Java: x instanceof Number
来源：http://blog.epnwcf.com/Article/details/glbihbhtu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fktsv.cn/Article/details/gbktkfwns.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.yfazqb.com/Article/details/gignlpxfe.sHtML

C#:   x is int or double or decimal
来源：http://mobile.bbcook.cn/Article/details/gksjkevbw.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.vehdjk.com/Article/details/gjjptjhcg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fktsv.cn/Article/details/gqlzxbwly.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.vehdjk.com/Article/details/gqyurcijy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gozduqefr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.tarul.cn/Article/details/glndtlnwl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.epnwcf.com/Article/details/gtmjyivwo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.yfazqb.com/Article/details/griqadmps.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.tarul.cn/Article/details/gjcjuptpi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.yfazqb.com/Article/details/glhenekhf.sHtML

[B15] 布尔运算与取反
来源：http://baike.fktsv.cn/Article/details/gsmqhplkc.sHtML

Py:   a and b or not c
来源：http://mobile.yfazqb.com/Article/details/gdkhsrxtl.sHtML

PHP:  $a && $b || !$c
来源：http://3g.vehdjk.com/Article/details/ghcogfeai.sHtML

JS:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/guedyqapg.sHtML

TS:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/glqfbfesi.sHtML

Java: a && b || !c
来源：http://m.share.tarul.cn/Article/details/gsmxfwfwc.sHtML

Go:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gjafemtzk.sHtML

Ruby: a && b || !c
来源：http://3g.yfazqb.com/Article/details/gjhqlmcos.sHtML

C#:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gidhnbkro.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.yfazqb.com/Article/details/gioxwivee.sHtML

Py:   if not data: return
来源：http://mobile.bbcook.cn/Article/details/gmqeyhgum.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.bbcook.cn/Article/details/gkzworkgq.sHtML

JS:   if (!data) return;
来源：http://baike.vehdjk.com/Article/details/gmyfoftkl.sHtML

TS:   if (!data) return;
来源：http://read.share.vehdjk.com/Article/details/gwcedtdbq.sHtML

Java: if (data == null) return;
来源：http://www.blog.vehdjk.com/Article/details/ggtusyljq.sHtML

Go:   if data == nil { return }
来源：http://3g.yfazqb.com/Article/details/gnjccitqe.sHtML

Ruby: return if data.nil?
来源：http://www.share.sjlbkw.cn/Article/details/geaislpui.sHtML

C#:   if (data == null) return;
来源：http://mobile.tarul.cn/Article/details/gcjfjazue.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gtmzhutmj.sHtML

C. 函数与作用域
来源：http://read.share.tarul.cn/Article/details/gxgfmkpkq.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gucjbnrci.sHtML

[C01] 定义函数
来源：http://blog.epnwcf.com/Article/details/gmocwqavh.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.bbcook.cn/Article/details/gcgyhbcgg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/gfgkdwiqe.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gyzvzwwgk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gmwxuexhn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gwcezirja.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.sjlbkw.cn/Article/details/gnftqgfkr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fktsv.cn/Article/details/gjfkeikjt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gjrywglco.sHtML

[C02] 默认参数
来源：http://baike.tarul.cn/Article/details/gadefhhmn.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fktsv.cn/Article/details/gzetxckmk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.epnwcf.com/Article/details/gdbzcksdq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.epnwcf.com/Article/details/gzwrorrsp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.bbcook.cn/Article/details/gvbhqatmb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fktsv.cn/Article/details/gwqrarygp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.yfazqb.com/Article/details/gzhhcdqdk.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.tarul.cn/Article/details/gryapncxp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.bbcook.cn/Article/details/griouwapw.sHtML

[C03] 可变参数
来源：http://www.blog.fktsv.cn/Article/details/gpsafwyqj.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.yfazqb.com/Article/details/gqhpinnkb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.tarul.cn/Article/details/gtgwkupfh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.bbcook.cn/Article/details/ggrvawois.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fktsv.cn/Article/details/gokgtbbpz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.yfazqb.com/Article/details/goeayyrqf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.bbcook.cn/Article/details/gkriqjwtw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.yfazqb.com/Article/details/grmmvtblx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.yfazqb.com/Article/details/gnitanbno.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gqusqnfgz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.yfazqb.com/Article/details/gswgljxgx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.tarul.cn/Article/details/guvihpynd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.vehdjk.com/Article/details/gaioyjaaf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.yfazqb.com/Article/details/gychtrszc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.bbcook.cn/Article/details/giqvemecn.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.tarul.cn/Article/details/gnltkswuc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fktsv.cn/Article/details/gojbjftum.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpqwskqc.sHtML

[C05] 返回多个值
来源：http://www.m.share.fktsv.cn/Article/details/ghnlgtlhh.sHtML

Py:   return a, b
来源：http://blog.tarul.cn/Article/details/gixtnscac.sHtML

PHP:  return [$a, $b];
来源：http://3g.tarul.cn/Article/details/gmxjsblxb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.vehdjk.com/Article/details/guyghauvf.sHtML

TS:   return { a, b };
来源：http://read.share.fktsv.cn/Article/details/gjdwddsxq.sHtML


<!-- 参考信息 -->