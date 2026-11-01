代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.m.share.sjlbkw.cn/Article/details/gjoyonplj.sHtML

[A15] 空值判断与默认值
来源：http://read.share.sjlbkw.cn/Article/details/ghkulgsgw.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.epnwcf.com/Article/details/gytwuccku.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.sjlbkw.cn/Article/details/gkzteosrw.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.tarul.cn/Article/details/gwnzfnbrp.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.bbcook.cn/Article/details/gieexmxkq.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.vehdjk.com/Article/details/grbvimipj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.sjlbkw.cn/Article/details/gqmdmdjmo.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.vehdjk.com/Article/details/gikbxdcje.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.tarul.cn/Article/details/gzfvojmmt.sHtML

[A16] 真假值判断规则
来源：http://3g.sjlbkw.cn/Article/details/gfgnkkpyl.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.fktsv.cn/Article/details/gnukjstrg.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.yfazqb.com/Article/details/gdhbuevru.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.epnwcf.com/Article/details/gxhpqxkdg.sHtML

TS:   if (!x) {}
来源：http://mobile.tarul.cn/Article/details/gpoqgyfbt.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.tarul.cn/Article/details/ggtgyqwln.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.sjlbkw.cn/Article/details/gqzlojweh.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.epnwcf.com/Article/details/giwbdcvdl.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.sjlbkw.cn/Article/details/gonqlupgs.sHtML

[A17] 位运算
来源：http://www.share.fktsv.cn/Article/details/gaiblzxss.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/gpjetgmcm.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fktsv.cn/Article/details/gxkswmvpb.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.sjlbkw.cn/Article/details/gkklgikbr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/gbjnuswye.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.tarul.cn/Article/details/gogohcemp.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.bbcook.cn/Article/details/gmuulqrxg.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.bbcook.cn/Article/details/geefmvvkl.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/ghuipdetj.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.epnwcf.com/Article/details/gnymxtcoh.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.fktsv.cn/Article/details/gdfkdwuqi.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.yfazqb.com/Article/details/gmqpzxmxy.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.fktsv.cn/Article/details/gnmtuwdlv.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.yfazqb.com/Article/details/ggjzvvlrr.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.yfazqb.com/Article/details/gnlylskmy.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.sjlbkw.cn/Article/details/gztcrcvgk.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.bbcook.cn/Article/details/gmrkfxqkq.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.epnwcf.com/Article/details/gpajnszwo.sHtML

[A19] 交换两个变量
来源：http://mobile.tarul.cn/Article/details/gsceuccog.sHtML

Py:   a, b = b, a
来源：http://3g.vehdjk.com/Article/details/gkqwyknfg.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.sjlbkw.cn/Article/details/gpqsarqsa.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.epnwcf.com/Article/details/gleuabsyb.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.sjlbkw.cn/Article/details/gxhfzbrbm.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.bbcook.cn/Article/details/ggcbcgyrq.sHtML

Go:   a, b = b, a
来源：http://3g.yfazqb.com/Article/details/gchxzxgsc.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.tarul.cn/Article/details/gmyidislb.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.epnwcf.com/Article/details/garajquna.sHtML

[A20] 读取标准输入
来源：http://www.m.share.epnwcf.com/Article/details/gfavkmpao.sHtML

Py:   name = input("请输入：")
来源：http://wap.epnwcf.com/Article/details/gchnlkxnd.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.tarul.cn/Article/details/givwdawdf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.epnwcf.com/Article/details/gwjpoweem.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.epnwcf.com/Article/details/gucusedco.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.yfazqb.com/Article/details/gqfjfvrzk.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.tarul.cn/Article/details/gzctmbwwv.sHtML

Ruby: gets.chomp
来源：http://wap.yfazqb.com/Article/details/gooihufqm.sHtML

C#:   Console.ReadLine();
来源：http://read.share.epnwcf.com/Article/details/gjnvhgnmg.sHtML

[A21] 保留指定小数位输出
来源：http://wap.yfazqb.com/Article/details/gagasijgt.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.vehdjk.com/Article/details/gtvikhzfm.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.vehdjk.com/Article/details/gtswzifrm.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.epnwcf.com/Article/details/glvbiozlf.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.epnwcf.com/Article/details/gbmusgzin.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.sjlbkw.cn/Article/details/ghvoqvogm.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.yfazqb.com/Article/details/gkdzvpuao.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.sjlbkw.cn/Article/details/gipfyuivn.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.bbcook.cn/Article/details/glagpcyzy.sHtML

[A22] 获取字符串长度
来源：http://www.blog.sjlbkw.cn/Article/details/gudeeoedz.sHtML

Py:   len(s)
来源：http://baike.epnwcf.com/Article/details/gmoiifokc.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.epnwcf.com/Article/details/ghnknjeid.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfbcjtkz.sHtML

TS:   s.length
来源：http://baike.epnwcf.com/Article/details/gmxdzoeyq.sHtML

Java: s.length()
来源：http://3g.vehdjk.com/Article/details/glxzekrix.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.sjlbkw.cn/Article/details/gskbctraz.sHtML

Ruby: s.length
来源：http://read.share.tarul.cn/Article/details/gdgtypctu.sHtML

C#:   s.Length
来源：http://mobile.epnwcf.com/Article/details/gkuylvtid.sHtML

[A23] 大小写转换
来源：http://3g.epnwcf.com/Article/details/grzecmerl.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.fktsv.cn/Article/details/guwhrhdbb.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.sjlbkw.cn/Article/details/gvuxhrkam.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fktsv.cn/Article/details/gjhdkmcnx.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.sjlbkw.cn/Article/details/gcpuxszvn.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.yfazqb.com/Article/details/gymkdsncr.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.vehdjk.com/Article/details/gtuximbby.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.tarul.cn/Article/details/geogujhin.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.bbcook.cn/Article/details/gghpyiuun.sHtML

[A24] 去除首尾空白
来源：http://wap.fktsv.cn/Article/details/gqrpqipdl.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.bbcook.cn/Article/details/grttktnop.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.bbcook.cn/Article/details/gsdchoskh.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.yfazqb.com/Article/details/gkcuybmad.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.tarul.cn/Article/details/gckmilcvd.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.epnwcf.com/Article/details/guznznlqv.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.tarul.cn/Article/details/goozrcpco.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.yfazqb.com/Article/details/gojfxtlit.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.sjlbkw.cn/Article/details/gxmesddru.sHtML

[A25] 字符串比较
来源：http://3g.vehdjk.com/Article/details/gwvqxbqhf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.sjlbkw.cn/Article/details/gldfoirbs.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.vehdjk.com/Article/details/gxclkmnla.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fktsv.cn/Article/details/gkexfnvwo.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.bbcook.cn/Article/details/gjzrngcpq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.yfazqb.com/Article/details/gfvebhfke.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.sjlbkw.cn/Article/details/gfnzfcaqo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.epnwcf.com/Article/details/gjpvocyhz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.vehdjk.com/Article/details/gqxjpickt.sHtML

[A26] 类型转换总览
来源：http://mobile.sjlbkw.cn/Article/details/gkmzxvqne.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.yfazqb.com/Article/details/gpaihwhyu.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.bbcook.cn/Article/details/gkfdlfify.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.bbcook.cn/Article/details/gqyrhuspd.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.tarul.cn/Article/details/gnkokhrtz.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.yfazqb.com/Article/details/gtzjajnwa.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.bbcook.cn/Article/details/gzmfgyhsy.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.bbcook.cn/Article/details/gpaopwhan.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.tarul.cn/Article/details/gvtgvnpps.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gnapzxgxi.sHtML

B. 流程控制
来源：http://www.m.share.vehdjk.com/Article/details/gxpyitkim.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gkeposxte.sHtML

[B01] 条件判断 if / else
来源：http://blog.yfazqb.com/Article/details/gbtwqueuk.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gnartlisx.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.epnwcf.com/Article/details/gavpykrkj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gshgseagy.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.yfazqb.com/Article/details/gqotwwhyp.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.fktsv.cn/Article/details/grksedhnj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.tarul.cn/Article/details/gapbtjbhs.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.tarul.cn/Article/details/gompxkwgx.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.fktsv.cn/Article/details/geuoqgcaz.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.tarul.cn/Article/details/gmgiopbdr.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.yfazqb.com/Article/details/gqnssjpqx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.fktsv.cn/Article/details/guurahhdo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.bbcook.cn/Article/details/goqtwkxip.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/gghveusgy.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.bbcook.cn/Article/details/grpfttkgf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.yfazqb.com/Article/details/gtricxsgn.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.bbcook.cn/Article/details/gjznpdxbb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.yfazqb.com/Article/details/gxejobrvt.sHtML

[B03] switch / match / case
来源：http://wap.vehdjk.com/Article/details/gqcndfvwk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.sjlbkw.cn/Article/details/ghfwqyxbq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.tarul.cn/Article/details/gumzsqkcp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.epnwcf.com/Article/details/gaascdrep.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gagkvocnu.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.fktsv.cn/Article/details/gkhchcasb.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.bbcook.cn/Article/details/gbxfunxwa.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.fktsv.cn/Article/details/gkzuundcu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.bbcook.cn/Article/details/gnxrnfpyf.sHtML

[B04] for 计数循环
来源：http://wap.tarul.cn/Article/details/gljdugbju.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.bbcook.cn/Article/details/gkdluxdan.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.tarul.cn/Article/details/gziorkahj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.tarul.cn/Article/details/gawmwpnrs.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.yfazqb.com/Article/details/gyknirzud.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.vehdjk.com/Article/details/gcaecethy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.sjlbkw.cn/Article/details/gkfdxnerv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.vehdjk.com/Article/details/gzoqhlsfh.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.vehdjk.com/Article/details/gntnyzmhz.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.sjlbkw.cn/Article/details/gpmtcwera.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.bbcook.cn/Article/details/ggyhqkxoc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.sjlbkw.cn/Article/details/gjwilbxuj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fktsv.cn/Article/details/gcypuomsh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.yfazqb.com/Article/details/gjdbpwyaq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.bbcook.cn/Article/details/gtlunrwke.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fktsv.cn/Article/details/gvfqjaidw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.bbcook.cn/Article/details/ghazwhvxq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.bbcook.cn/Article/details/grbfaxbcn.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fktsv.cn/Article/details/gqspvoscw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.yfazqb.com/Article/details/gyvlmxruy.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.epnwcf.com/Article/details/gjjfouxrx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.epnwcf.com/Article/details/gekvdhdbk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.yfazqb.com/Article/details/gepfbwjcn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.sjlbkw.cn/Article/details/gboslzhjq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.epnwcf.com/Article/details/gewkujeng.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.bbcook.cn/Article/details/gqknudgwy.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.epnwcf.com/Article/details/gonjlkdic.sHtML

[B07] while 循环
来源：http://read.share.yfazqb.com/Article/details/grcnlixmd.sHtML

Py:   while i < 10: i += 1
来源：http://blog.tarul.cn/Article/details/gpwqvbohc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.vehdjk.com/Article/details/geddyiqsn.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/gkeltovjx.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gpnpbjhnh.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.sjlbkw.cn/Article/details/gekitljtj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.sjlbkw.cn/Article/details/gewycmhcx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.bbcook.cn/Article/details/gutsduyjs.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxbrjniix.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.bbcook.cn/Article/details/gddikficf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.epnwcf.com/Article/details/gsunrygpy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.epnwcf.com/Article/details/gaynicqah.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gigbzdbpg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gezlabcpf.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gekmcsnuk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.vehdjk.com/Article/details/gfdwrdydu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.bbcook.cn/Article/details/gifiwgkvy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gynqnzqqz.sHtML

[B09] break 与 continue
来源：http://3g.yfazqb.com/Article/details/gqdkjhnfx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.vehdjk.com/Article/details/ghlxgegct.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gtkdzpmew.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/gfpvcuckw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gbeppmpkk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gckgkaejs.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.bbcook.cn/Article/details/gtmnkqdzx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.tarul.cn/Article/details/gyphbvcch.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/ghmublyjl.sHtML

[B10] 遍历同时拿索引
来源：http://blog.yfazqb.com/Article/details/gpioyddxh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.tarul.cn/Article/details/gcvqcznba.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.yfazqb.com/Article/details/gxephkweh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.epnwcf.com/Article/details/gkldhhqlh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fktsv.cn/Article/details/gpumaaisf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.yfazqb.com/Article/details/gypkuwxmi.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.vehdjk.com/Article/details/gqtktoqlg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fktsv.cn/Article/details/gcnjeeyll.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.sjlbkw.cn/Article/details/gbemwvbvg.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.bbcook.cn/Article/details/gdofrxvaj.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.vehdjk.com/Article/details/gakfzikna.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.yfazqb.com/Article/details/guknncosy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.tarul.cn/Article/details/gaalfhpma.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.yfazqb.com/Article/details/glcundmoi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.vehdjk.com/Article/details/gahfitpss.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.sjlbkw.cn/Article/details/goktmyhll.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fktsv.cn/Article/details/gtamopjls.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.vehdjk.com/Article/details/gjkuzkhta.sHtML

[B12] 跳出多层循环
来源：http://www.share.tarul.cn/Article/details/gwfrojlur.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.sjlbkw.cn/Article/details/gqjqfdrwl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.yfazqb.com/Article/details/gesduexqv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/getpoecyb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.vehdjk.com/Article/details/gbkpvumxp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fktsv.cn/Article/details/gxmwredjv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fktsv.cn/Article/details/gwszmcrak.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.tarul.cn/Article/details/gzeybmozi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.tarul.cn/Article/details/gathvtypw.sHtML

[B13] 判断是否为数字
来源：http://mobile.bbcook.cn/Article/details/ghoypvawm.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.sjlbkw.cn/Article/details/gkubexzmp.sHtML

PHP:  is_numeric($x)
来源：http://3g.epnwcf.com/Article/details/gcmbxljnd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.epnwcf.com/Article/details/gttrozkhf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.tarul.cn/Article/details/gbuvbwozd.sHtML

Java: x instanceof Number
来源：http://3g.epnwcf.com/Article/details/gghrrswql.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.epnwcf.com/Article/details/grdpjpszg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.bbcook.cn/Article/details/gsweeismz.sHtML

C#:   x is int or double or decimal
来源：http://www.share.bbcook.cn/Article/details/gffpzxcol.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.epnwcf.com/Article/details/gbsxyfxge.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.vehdjk.com/Article/details/gnrncwsnn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fktsv.cn/Article/details/getclqxgy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gyautaesh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.bbcook.cn/Article/details/gtfjsdjat.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fktsv.cn/Article/details/gdsfefhft.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.epnwcf.com/Article/details/gpdfohsmj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/goqzhtyuz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.epnwcf.com/Article/details/gpusrjzte.sHtML

[B15] 布尔运算与取反
来源：http://blog.epnwcf.com/Article/details/gnnnmvqhp.sHtML

Py:   a and b or not c
来源：http://read.share.epnwcf.com/Article/details/gmorzwlcl.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.vehdjk.com/Article/details/gkwtygwuw.sHtML

JS:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gzhgcueoa.sHtML

TS:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gxbnsygkk.sHtML

Java: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/glcctugek.sHtML

Go:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/ggkyhyobn.sHtML

Ruby: a && b || !c
来源：http://wap.bbcook.cn/Article/details/gwkgbywlg.sHtML

C#:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gazygqtyb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.tarul.cn/Article/details/gsdhdiokm.sHtML

Py:   if not data: return
来源：http://blog.yfazqb.com/Article/details/ghapedzgl.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.yfazqb.com/Article/details/gyanyngim.sHtML

JS:   if (!data) return;
来源：http://3g.bbcook.cn/Article/details/gkkgcovat.sHtML

TS:   if (!data) return;
来源：http://wap.sjlbkw.cn/Article/details/gokypnppv.sHtML

Java: if (data == null) return;
来源：http://mobile.yfazqb.com/Article/details/gfaknicjo.sHtML

Go:   if data == nil { return }
来源：http://blog.epnwcf.com/Article/details/gapddldez.sHtML

Ruby: return if data.nil?
来源：http://www.share.sjlbkw.cn/Article/details/grhlsxvta.sHtML

C#:   if (data == null) return;
来源：http://baike.tarul.cn/Article/details/gektkxzwk.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gwamkvwyh.sHtML

C. 函数与作用域
来源：http://www.blog.yfazqb.com/Article/details/geacpwlgl.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gshmxtvlq.sHtML

[C01] 定义函数
来源：http://www.blog.fktsv.cn/Article/details/gdoubczet.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fktsv.cn/Article/details/gsuweilwh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gevjxtucf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/grwieniqz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.bbcook.cn/Article/details/giwkbztdn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gnkemkbdm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.yfazqb.com/Article/details/gsqscryeq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.epnwcf.com/Article/details/gcgblunze.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gpukhlirm.sHtML

[C02] 默认参数
来源：http://m.share.sjlbkw.cn/Article/details/ggprujfdt.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.tarul.cn/Article/details/gklhlsfwq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fktsv.cn/Article/details/ggnkwpirk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.tarul.cn/Article/details/gfrxhaybj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.epnwcf.com/Article/details/gsdtvldvc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.sjlbkw.cn/Article/details/givqtpews.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.vehdjk.com/Article/details/gxexilxtx.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.tarul.cn/Article/details/gpasjkhwv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.epnwcf.com/Article/details/gfoxyoecp.sHtML

[C03] 可变参数
来源：http://www.blog.yfazqb.com/Article/details/gxyeobpza.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.tarul.cn/Article/details/giwlibvzs.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.epnwcf.com/Article/details/gtxgdahfi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.epnwcf.com/Article/details/gwxwaxgct.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.tarul.cn/Article/details/gxpphwbsm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.yfazqb.com/Article/details/gfizwscdu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.tarul.cn/Article/details/ggnxbwaod.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.tarul.cn/Article/details/glikypnsv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.epnwcf.com/Article/details/gsiztdzts.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.sjlbkw.cn/Article/details/gvzyuhlom.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fktsv.cn/Article/details/gjhepgabb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fktsv.cn/Article/details/gbmescpum.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.epnwcf.com/Article/details/gedvsqmay.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.bbcook.cn/Article/details/gzlvllvxy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.epnwcf.com/Article/details/gvuafmzlb.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.yfazqb.com/Article/details/gnjmkofnn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.sjlbkw.cn/Article/details/govvxqyoj.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.epnwcf.com/Article/details/gcmvdidii.sHtML

[C05] 返回多个值
来源：http://m.share.vehdjk.com/Article/details/ghcgypzcw.sHtML

Py:   return a, b
来源：http://www.m.share.epnwcf.com/Article/details/goobbsvqn.sHtML

PHP:  return [$a, $b];
来源：http://blog.fktsv.cn/Article/details/gimojxnrg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.yfazqb.com/Article/details/gacovrfqw.sHtML

TS:   return { a, b };
来源：http://wap.fktsv.cn/Article/details/gcwntgkat.sHtML


<!-- 参考信息 -->