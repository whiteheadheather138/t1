代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://www.blog.sjlbkw.cn/Article/details/gjrjvobaa.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.bbcook.cn/Article/details/gfwevvewu.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.fktsv.cn/Article/details/gxztjgyrj.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.vehdjk.com/Article/details/gbssawriy.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.fktsv.cn/Article/details/gxxdbzqrp.sHtML

[A15] 空值判断与默认值
来源：http://www.share.sjlbkw.cn/Article/details/gdqtyjdzj.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.yfazqb.com/Article/details/gizfgkrhb.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.vehdjk.com/Article/details/gjvftwurp.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.fktsv.cn/Article/details/geahrrrqa.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.sjlbkw.cn/Article/details/ggbglozlg.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.bbcook.cn/Article/details/gcwrjjatl.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.epnwcf.com/Article/details/gwsauhieg.sHtML

Ruby: value = data || "默认值"
来源：http://wap.vehdjk.com/Article/details/gdgweukqb.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.fktsv.cn/Article/details/gwyuiesbv.sHtML

[A16] 真假值判断规则
来源：http://wap.fktsv.cn/Article/details/gtqjbajcp.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.bbcook.cn/Article/details/gtswtydrh.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.bbcook.cn/Article/details/grjcmubrl.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.tarul.cn/Article/details/ggzqmgdmx.sHtML

TS:   if (!x) {}
来源：http://baike.bbcook.cn/Article/details/gtqfpxjaj.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.vehdjk.com/Article/details/gonhnftrz.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.yfazqb.com/Article/details/gfpbattxm.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.sjlbkw.cn/Article/details/gahzpikxe.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.vehdjk.com/Article/details/glowdulbs.sHtML

[A17] 位运算
来源：http://www.blog.tarul.cn/Article/details/gpoyrolkq.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/giktltvqk.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.fktsv.cn/Article/details/giobklekq.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.vehdjk.com/Article/details/gdajgfgvm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gpanwoxhi.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fktsv.cn/Article/details/gokmmvgeg.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.bbcook.cn/Article/details/geoobqdqc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.vehdjk.com/Article/details/gfpmbsenj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.vehdjk.com/Article/details/glthtlqrq.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.sjlbkw.cn/Article/details/gfcmfwzym.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.yfazqb.com/Article/details/gxrgwhujz.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.bbcook.cn/Article/details/gbhdjwmmg.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.vehdjk.com/Article/details/gnjfkkcgn.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.bbcook.cn/Article/details/gffnwoxui.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.sjlbkw.cn/Article/details/gmgauqkdg.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.sjlbkw.cn/Article/details/guhqcabuv.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.fktsv.cn/Article/details/gbfwkudbc.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.bbcook.cn/Article/details/grtltjtxc.sHtML

[A19] 交换两个变量
来源：http://3g.fktsv.cn/Article/details/gqbsnncxx.sHtML

Py:   a, b = b, a
来源：http://www.m.share.vehdjk.com/Article/details/gcvviqdkk.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.bbcook.cn/Article/details/gogenurcp.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.bbcook.cn/Article/details/gzflbwpan.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.sjlbkw.cn/Article/details/ghbgmmfmo.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.vehdjk.com/Article/details/ggifkfiqs.sHtML

Go:   a, b = b, a
来源：http://www.m.share.yfazqb.com/Article/details/gtivrcsep.sHtML

Ruby: a, b = b, a
来源：http://www.blog.yfazqb.com/Article/details/grqemdpnl.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.tarul.cn/Article/details/grqjhmvsn.sHtML

[A20] 读取标准输入
来源：http://blog.sjlbkw.cn/Article/details/gqruodfgx.sHtML

Py:   name = input("请输入：")
来源：http://mobile.epnwcf.com/Article/details/gvdsloeyl.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.yfazqb.com/Article/details/gcotiqphd.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.fktsv.cn/Article/details/gxqrtjicu.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.bbcook.cn/Article/details/gnzvvtmtl.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.fktsv.cn/Article/details/gljnbublg.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.tarul.cn/Article/details/ggekxlvsh.sHtML

Ruby: gets.chomp
来源：http://mobile.bbcook.cn/Article/details/gpfxnmyns.sHtML

C#:   Console.ReadLine();
来源：http://www.share.sjlbkw.cn/Article/details/gqxdlctmo.sHtML

[A21] 保留指定小数位输出
来源：http://blog.epnwcf.com/Article/details/gcpwsimgb.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.vehdjk.com/Article/details/gaiimgkbz.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.tarul.cn/Article/details/gckhuwlro.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.fktsv.cn/Article/details/gpzzpvbww.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.bbcook.cn/Article/details/gojjholls.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.fktsv.cn/Article/details/gvxgkqanh.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.sjlbkw.cn/Article/details/gptuwaqil.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.yfazqb.com/Article/details/gtgixlqjy.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.tarul.cn/Article/details/gvevhqbtq.sHtML

[A22] 获取字符串长度
来源：http://3g.fktsv.cn/Article/details/gndlxznez.sHtML

Py:   len(s)
来源：http://read.share.bbcook.cn/Article/details/gujhxcodx.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.yfazqb.com/Article/details/gnvvlcniu.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.bbcook.cn/Article/details/gfpnttcsu.sHtML

TS:   s.length
来源：http://www.blog.yfazqb.com/Article/details/gpezketxl.sHtML

Java: s.length()
来源：http://m.share.fktsv.cn/Article/details/gamnklczh.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.fktsv.cn/Article/details/gujeqdajz.sHtML

Ruby: s.length
来源：http://3g.yfazqb.com/Article/details/gzohadzyv.sHtML

C#:   s.Length
来源：http://baike.epnwcf.com/Article/details/gztdbjmif.sHtML

[A23] 大小写转换
来源：http://read.share.vehdjk.com/Article/details/gcmzmxylq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.fktsv.cn/Article/details/gkcejrjek.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.tarul.cn/Article/details/gmbfewhdd.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fktsv.cn/Article/details/gnmklzury.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.yfazqb.com/Article/details/gxmnnfvvp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.vehdjk.com/Article/details/gxwlzyfym.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.bbcook.cn/Article/details/gkdgkcnix.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.epnwcf.com/Article/details/glyzayvoz.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.yfazqb.com/Article/details/geoorcfhh.sHtML

[A24] 去除首尾空白
来源：http://baike.yfazqb.com/Article/details/grpghalky.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.bbcook.cn/Article/details/gvowwicpq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.tarul.cn/Article/details/gpizbpugh.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.vehdjk.com/Article/details/gmsyezirs.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.sjlbkw.cn/Article/details/ghsbuqcja.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fktsv.cn/Article/details/gtufmadec.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnikgrkq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.tarul.cn/Article/details/ghrtcxmdy.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.yfazqb.com/Article/details/gdknmpubz.sHtML

[A25] 字符串比较
来源：http://m.share.epnwcf.com/Article/details/guazvhmwr.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.vehdjk.com/Article/details/gkcbcpqvw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.vehdjk.com/Article/details/gihqcsjpl.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.vehdjk.com/Article/details/gmjtgkjvh.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.vehdjk.com/Article/details/gubszehdl.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.tarul.cn/Article/details/gkienrgyb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.vehdjk.com/Article/details/gffshydgb.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.yfazqb.com/Article/details/geiwgclbl.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fktsv.cn/Article/details/gikxfcewl.sHtML

[A26] 类型转换总览
来源：http://m.share.fktsv.cn/Article/details/gfxhgbsos.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.fktsv.cn/Article/details/godknpagg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.yfazqb.com/Article/details/gmaifidrs.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.bbcook.cn/Article/details/gdcwblxfv.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.tarul.cn/Article/details/gkmoaoeka.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.epnwcf.com/Article/details/gslblknxk.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.bbcook.cn/Article/details/gvwdbezcp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fktsv.cn/Article/details/giurigdbj.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.bbcook.cn/Article/details/gnexkbflq.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gwkpoylja.sHtML

B. 流程控制
来源：http://www.blog.tarul.cn/Article/details/giymsnyrk.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gltfdyybp.sHtML

[B01] 条件判断 if / else
来源：http://m.share.epnwcf.com/Article/details/gfdkgtkkf.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.yfazqb.com/Article/details/gbbhcykfu.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.fktsv.cn/Article/details/ghlwqjpos.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.yfazqb.com/Article/details/gnshuwnet.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.vehdjk.com/Article/details/ghuqqxxse.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gbxqbmfsr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.sjlbkw.cn/Article/details/gxytssbfo.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.vehdjk.com/Article/details/glitqffuz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.sjlbkw.cn/Article/details/ggjxjrofe.sHtML

[B02] 多分支 else if / elif
来源：http://baike.tarul.cn/Article/details/gukoyhwwz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fktsv.cn/Article/details/gesofkedd.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.sjlbkw.cn/Article/details/gdqobdejz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fktsv.cn/Article/details/gjhovkonm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.yfazqb.com/Article/details/gstlaruup.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/gffokrspj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.sjlbkw.cn/Article/details/gvknhmajx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.fktsv.cn/Article/details/gyymrtnhc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fktsv.cn/Article/details/gmluppigd.sHtML

[B03] switch / match / case
来源：http://mobile.tarul.cn/Article/details/gpglwgvof.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.bbcook.cn/Article/details/gwszkkwur.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.tarul.cn/Article/details/gwaezcfkp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.tarul.cn/Article/details/gvtayxgrk.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.epnwcf.com/Article/details/gpjxmhvxn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.epnwcf.com/Article/details/gxkzuovbv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.sjlbkw.cn/Article/details/gsuvoycwo.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.yfazqb.com/Article/details/gwblwfooc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.sjlbkw.cn/Article/details/ggkkqtwbv.sHtML

[B04] for 计数循环
来源：http://www.blog.vehdjk.com/Article/details/gdhladlph.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.vehdjk.com/Article/details/gehffbook.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.yfazqb.com/Article/details/gaoifaytx.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.yfazqb.com/Article/details/goicpvokg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.bbcook.cn/Article/details/gvuixafxn.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.vehdjk.com/Article/details/gaguzncyt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.yfazqb.com/Article/details/ggbgjvptl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.bbcook.cn/Article/details/ggngsnwwr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.epnwcf.com/Article/details/ggaephcom.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.fktsv.cn/Article/details/gcvfpglgh.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.sjlbkw.cn/Article/details/ghpkkmlmq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.epnwcf.com/Article/details/gcpocrccf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.sjlbkw.cn/Article/details/glfybehlj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.yfazqb.com/Article/details/govynfvbe.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.vehdjk.com/Article/details/guyozyfio.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.bbcook.cn/Article/details/gaemttvbb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.yfazqb.com/Article/details/gwxjhhrql.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.epnwcf.com/Article/details/gwytzprck.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.epnwcf.com/Article/details/gqowiddvy.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.bbcook.cn/Article/details/grgbgczil.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.tarul.cn/Article/details/gbkjdtcdw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.tarul.cn/Article/details/gtftmsegc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.tarul.cn/Article/details/ghvvigoao.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.yfazqb.com/Article/details/gcxezuhfs.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.tarul.cn/Article/details/gmchztoex.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.tarul.cn/Article/details/gzrhkxxht.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.yfazqb.com/Article/details/gaweybjup.sHtML

[B07] while 循环
来源：http://www.blog.yfazqb.com/Article/details/gqolvgjnc.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.bbcook.cn/Article/details/gcugsobhy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fktsv.cn/Article/details/gjcegidgz.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.yfazqb.com/Article/details/gbexuetkf.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gqdimhfzj.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fktsv.cn/Article/details/gygwjqvfj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fktsv.cn/Article/details/gozciprtm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.epnwcf.com/Article/details/gbrxfvqbd.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gjnlbcgxu.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.epnwcf.com/Article/details/gqrjyjbov.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.yfazqb.com/Article/details/gfqrwinds.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.yfazqb.com/Article/details/giiryzwyn.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gmfoiuxgh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/gadyhwxrp.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/ggyyidfco.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.epnwcf.com/Article/details/gqrqpitgg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.tarul.cn/Article/details/gtvoezrvf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gxfxxqsgg.sHtML

[B09] break 与 continue
来源：http://blog.epnwcf.com/Article/details/gnseocfon.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.yfazqb.com/Article/details/gobwwurnb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/geiwltgco.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/gpniizrqk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/giuroiina.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gwmnzrect.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.tarul.cn/Article/details/glsxewpbu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.tarul.cn/Article/details/gvqfycfuy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/gllxrcess.sHtML

[B10] 遍历同时拿索引
来源：http://wap.yfazqb.com/Article/details/ggiuizgkz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.vehdjk.com/Article/details/gmzzivogx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.sjlbkw.cn/Article/details/glqbgfgbg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.bbcook.cn/Article/details/gotopaxul.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fktsv.cn/Article/details/guvfhifrc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.yfazqb.com/Article/details/gxlqnhjwq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.epnwcf.com/Article/details/gwmicltad.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fktsv.cn/Article/details/gblblfynq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.bbcook.cn/Article/details/gniibmyil.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.vehdjk.com/Article/details/gfxkmtbua.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.vehdjk.com/Article/details/giqrpyigp.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.vehdjk.com/Article/details/gkaukxvhz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.vehdjk.com/Article/details/gfmhtxxun.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.sjlbkw.cn/Article/details/gntmawyjk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.tarul.cn/Article/details/grarjaiyv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.tarul.cn/Article/details/gxhbzqnzp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrbytwuo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.vehdjk.com/Article/details/gbtwhacbb.sHtML

[B12] 跳出多层循环
来源：http://m.share.vehdjk.com/Article/details/gyplolhdk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.tarul.cn/Article/details/gawzwmpbf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fktsv.cn/Article/details/gooidywki.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.vehdjk.com/Article/details/gopwzqqrh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/gihuvytln.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gmxraupzy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fktsv.cn/Article/details/gxvighred.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.epnwcf.com/Article/details/gghdgyzxw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.yfazqb.com/Article/details/gtrcibnvn.sHtML

[B13] 判断是否为数字
来源：http://blog.yfazqb.com/Article/details/gwhztmsgz.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.sjlbkw.cn/Article/details/ghpmebash.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.yfazqb.com/Article/details/gtfpanyco.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.tarul.cn/Article/details/gefxmhnyc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gfxfevazc.sHtML

Java: x instanceof Number
来源：http://blog.yfazqb.com/Article/details/gtdcsuepl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fktsv.cn/Article/details/gqdziirsw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.yfazqb.com/Article/details/giwmgnnxd.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.sjlbkw.cn/Article/details/ggtyhjpun.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.vehdjk.com/Article/details/ganjhdyhs.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.epnwcf.com/Article/details/gzzmmeuyf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.bbcook.cn/Article/details/gwvmuybga.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.bbcook.cn/Article/details/gexjovrid.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gvlkaamaa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.tarul.cn/Article/details/gchilozir.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fktsv.cn/Article/details/gpnhpmmag.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.tarul.cn/Article/details/gqtocyhhg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fktsv.cn/Article/details/gctpmxbmi.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.yfazqb.com/Article/details/gwvreumyl.sHtML

Py:   a and b or not c
来源：http://3g.yfazqb.com/Article/details/gvgbkoyjc.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.epnwcf.com/Article/details/gnlzizfah.sHtML

JS:   a && b || !c
来源：http://baike.epnwcf.com/Article/details/gnpuwhpss.sHtML

TS:   a && b || !c
来源：http://baike.epnwcf.com/Article/details/gufwnkhwy.sHtML

Java: a && b || !c
来源：http://3g.vehdjk.com/Article/details/ginnxpogp.sHtML

Go:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gqgrefcyt.sHtML

Ruby: a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gdhtodoqq.sHtML

C#:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gjuaxvrhl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.bbcook.cn/Article/details/gpejvvaex.sHtML

Py:   if not data: return
来源：http://www.blog.vehdjk.com/Article/details/gkgjhloak.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.epnwcf.com/Article/details/gjlieqshc.sHtML

JS:   if (!data) return;
来源：http://mobile.vehdjk.com/Article/details/glyswsfrp.sHtML

TS:   if (!data) return;
来源：http://www.m.share.tarul.cn/Article/details/gyrvfycbz.sHtML

Java: if (data == null) return;
来源：http://www.share.epnwcf.com/Article/details/gqyosalsy.sHtML

Go:   if data == nil { return }
来源：http://3g.sjlbkw.cn/Article/details/glyztlfco.sHtML

Ruby: return if data.nil?
来源：http://www.share.fktsv.cn/Article/details/grwbbrpkl.sHtML

C#:   if (data == null) return;
来源：http://www.blog.yfazqb.com/Article/details/glyamjfmn.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gfnzegpkd.sHtML

C. 函数与作用域
来源：http://blog.tarul.cn/Article/details/gvzlcznrd.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gsooxeybn.sHtML

[C01] 定义函数
来源：http://www.share.fktsv.cn/Article/details/gpbhpdnuq.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.bbcook.cn/Article/details/gbgncbvbr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.epnwcf.com/Article/details/gelbgksre.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/guesksvyg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gnfkpwaoj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gqgncyqki.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.epnwcf.com/Article/details/ghrrdauep.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.vehdjk.com/Article/details/gzszyinzb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gjeislyne.sHtML

[C02] 默认参数
来源：http://m.share.tarul.cn/Article/details/gqdhufenw.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.epnwcf.com/Article/details/gnsghjlii.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gaqslobdn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.vehdjk.com/Article/details/gkdfljvan.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gzsqpevar.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.tarul.cn/Article/details/gttlpxflx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.sjlbkw.cn/Article/details/guzivwlqq.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.vehdjk.com/Article/details/ghlseklkd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.epnwcf.com/Article/details/gqefodhve.sHtML

[C03] 可变参数
来源：http://m.share.fktsv.cn/Article/details/gbbtankiv.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.epnwcf.com/Article/details/gpnoxbhgy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.bbcook.cn/Article/details/gyksbrhqq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.epnwcf.com/Article/details/gqeqpeemq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.bbcook.cn/Article/details/gblzwujkp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fktsv.cn/Article/details/gnftxrrnz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.bbcook.cn/Article/details/gcftywssh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gtihskqop.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fktsv.cn/Article/details/gnndixtbt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.epnwcf.com/Article/details/ggukkxrwa.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.vehdjk.com/Article/details/gavtybygr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.bbcook.cn/Article/details/gizdnrtxt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.epnwcf.com/Article/details/gxbddutdg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.bbcook.cn/Article/details/gnaifbkfs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.tarul.cn/Article/details/gizywjwes.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.vehdjk.com/Article/details/gblmbtemj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.tarul.cn/Article/details/gyuagwusx.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/grjognwtu.sHtML

[C05] 返回多个值
来源：http://read.share.bbcook.cn/Article/details/gxggjukgm.sHtML


<!-- 参考信息 -->