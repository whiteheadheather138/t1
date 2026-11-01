代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://mobile.epnwcf.com/Article/details/guobcwdtr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.vehdjk.com/Article/details/gmrauwjsn.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.bbcook.cn/Article/details/guzikevme.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.tarul.cn/Article/details/gvvtbipiq.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.sjlbkw.cn/Article/details/gfvkidnxi.sHtML

[A15] 空值判断与默认值
来源：http://m.share.epnwcf.com/Article/details/gghbzlfjp.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.sjlbkw.cn/Article/details/glonlfoqr.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.yfazqb.com/Article/details/gzoijttda.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.sjlbkw.cn/Article/details/gimhjjrlu.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.sjlbkw.cn/Article/details/gnlzmfamf.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.tarul.cn/Article/details/gxvjrtexr.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.epnwcf.com/Article/details/gedyrjwyy.sHtML

Ruby: value = data || "默认值"
来源：http://baike.tarul.cn/Article/details/gspbgzgny.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.vehdjk.com/Article/details/gxwwqvcfd.sHtML

[A16] 真假值判断规则
来源：http://www.share.tarul.cn/Article/details/gdahzqhyp.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.vehdjk.com/Article/details/guuqyybit.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.bbcook.cn/Article/details/giktdrric.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.tarul.cn/Article/details/gtcubvqno.sHtML

TS:   if (!x) {}
来源：http://www.m.share.fktsv.cn/Article/details/ghjrephai.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.tarul.cn/Article/details/gjmuuelxq.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.bbcook.cn/Article/details/gqmhqlqzh.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.vehdjk.com/Article/details/gjxpxdpsx.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fktsv.cn/Article/details/gwwfmgfyc.sHtML

[A17] 位运算
来源：http://www.m.share.vehdjk.com/Article/details/gvymiqhpj.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.vehdjk.com/Article/details/gfaszdfzi.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.tarul.cn/Article/details/geyrlmsbt.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.yfazqb.com/Article/details/gordgctiz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/glsvkojnd.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gunceodtb.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.yfazqb.com/Article/details/gyrjwppdz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.yfazqb.com/Article/details/gqypwfuzd.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/gprnzfsnd.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.sjlbkw.cn/Article/details/gbsnbehzc.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.fktsv.cn/Article/details/gecqypgpv.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.vehdjk.com/Article/details/gsfekzwkn.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.sjlbkw.cn/Article/details/greuygfzd.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.vehdjk.com/Article/details/ghanjoqle.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.tarul.cn/Article/details/gnsnhkufp.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.bbcook.cn/Article/details/gtvmbwdvl.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.vehdjk.com/Article/details/gxvttyhsx.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.yfazqb.com/Article/details/gldcjrdcf.sHtML

[A19] 交换两个变量
来源：http://read.share.vehdjk.com/Article/details/grdfnnvjb.sHtML

Py:   a, b = b, a
来源：http://read.share.tarul.cn/Article/details/gobeupbwe.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.bbcook.cn/Article/details/gotdvkgts.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.tarul.cn/Article/details/gmsfkluln.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.bbcook.cn/Article/details/gaumlclyf.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.bbcook.cn/Article/details/ggofxiiep.sHtML

Go:   a, b = b, a
来源：http://blog.bbcook.cn/Article/details/gwfvrtvkq.sHtML

Ruby: a, b = b, a
来源：http://www.blog.bbcook.cn/Article/details/gthizdhpm.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.fktsv.cn/Article/details/gegqkgxla.sHtML

[A20] 读取标准输入
来源：http://www.blog.tarul.cn/Article/details/gxqatueqx.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.tarul.cn/Article/details/gthrqwfdh.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.yfazqb.com/Article/details/gbbonklrt.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.vehdjk.com/Article/details/gwbmjakpk.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.sjlbkw.cn/Article/details/gaqfkbekk.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.bbcook.cn/Article/details/gsveyivsl.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.vehdjk.com/Article/details/gwmrwhtqt.sHtML

Ruby: gets.chomp
来源：http://www.blog.sjlbkw.cn/Article/details/gsymexjpl.sHtML

C#:   Console.ReadLine();
来源：http://www.share.fktsv.cn/Article/details/grmzfuyxf.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.bbcook.cn/Article/details/gsknmpsrk.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.yfazqb.com/Article/details/gyshnxkqd.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.sjlbkw.cn/Article/details/gvcqrmsav.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.tarul.cn/Article/details/gxvmczvyj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.sjlbkw.cn/Article/details/guvyupaxm.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.sjlbkw.cn/Article/details/gmagjbsln.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.vehdjk.com/Article/details/gcjbuurys.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.yfazqb.com/Article/details/gleszscxn.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.sjlbkw.cn/Article/details/grbvuarvo.sHtML

[A22] 获取字符串长度
来源：http://m.share.yfazqb.com/Article/details/gjxngchlv.sHtML

Py:   len(s)
来源：http://m.share.yfazqb.com/Article/details/gafztmzte.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.fktsv.cn/Article/details/gkekfwxwo.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.sjlbkw.cn/Article/details/gwhxacbif.sHtML

TS:   s.length
来源：http://baike.bbcook.cn/Article/details/gwhhgsqcg.sHtML

Java: s.length()
来源：http://3g.tarul.cn/Article/details/gqohtjycm.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.tarul.cn/Article/details/gdcznbrfj.sHtML

Ruby: s.length
来源：http://baike.yfazqb.com/Article/details/gzbckdbxc.sHtML

C#:   s.Length
来源：http://m.share.vehdjk.com/Article/details/glrojgbxv.sHtML

[A23] 大小写转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gmoqxdbmo.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.epnwcf.com/Article/details/gavdnitxm.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.tarul.cn/Article/details/gonfwirhw.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fktsv.cn/Article/details/gulnufnkp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.yfazqb.com/Article/details/glzrpmfmr.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.tarul.cn/Article/details/gwpskauks.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.yfazqb.com/Article/details/gqyzhbzjc.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.tarul.cn/Article/details/ghjknqcmn.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.tarul.cn/Article/details/gqhuaqcex.sHtML

[A24] 去除首尾空白
来源：http://read.share.epnwcf.com/Article/details/grzdubcsp.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.fktsv.cn/Article/details/gpaukavmb.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.vehdjk.com/Article/details/gmjrrwogj.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.epnwcf.com/Article/details/gfsapvtav.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.bbcook.cn/Article/details/gatlzoqeu.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.epnwcf.com/Article/details/geopmfdlu.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.sjlbkw.cn/Article/details/gxnqitzcb.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.bbcook.cn/Article/details/gxjhrldlm.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.yfazqb.com/Article/details/glujbqwvc.sHtML

[A25] 字符串比较
来源：http://baike.fktsv.cn/Article/details/guqisntzz.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fktsv.cn/Article/details/giiokrdin.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.epnwcf.com/Article/details/gxsawnrjg.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.epnwcf.com/Article/details/gpzysacbz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.epnwcf.com/Article/details/gpoxfwszu.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.yfazqb.com/Article/details/gkfnuevlg.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.yfazqb.com/Article/details/gpvcecsmo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.epnwcf.com/Article/details/gpwvlvlcm.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.tarul.cn/Article/details/gieozffaa.sHtML

[A26] 类型转换总览
来源：http://www.m.share.yfazqb.com/Article/details/gcjcbeurd.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.tarul.cn/Article/details/gvfqrsfho.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.bbcook.cn/Article/details/gzxjugbwb.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.tarul.cn/Article/details/grqmkderm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.vehdjk.com/Article/details/gtiiwlfum.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.sjlbkw.cn/Article/details/gzwpgnddy.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.bbcook.cn/Article/details/gbppgtalz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.yfazqb.com/Article/details/gvgtkmsuu.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.sjlbkw.cn/Article/details/gmqjeierx.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/guzutuggi.sHtML

B. 流程控制
来源：http://baike.yfazqb.com/Article/details/gatthskjw.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gzlxvisrv.sHtML

[B01] 条件判断 if / else
来源：http://baike.sjlbkw.cn/Article/details/gxhrqvmjs.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.sjlbkw.cn/Article/details/gkvkytfyo.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.fktsv.cn/Article/details/gsjxctzpz.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.yfazqb.com/Article/details/gtabocncm.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.bbcook.cn/Article/details/ghvsicieg.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.yfazqb.com/Article/details/gussflrcl.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.vehdjk.com/Article/details/gwyzbmfez.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.yfazqb.com/Article/details/gqgcubyaf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/gkfcctydj.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.vehdjk.com/Article/details/gabjzawhn.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.epnwcf.com/Article/details/gocakkqdh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.bbcook.cn/Article/details/gyuvpoeng.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.epnwcf.com/Article/details/gholjhzdr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.yfazqb.com/Article/details/gfwuypkpd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fktsv.cn/Article/details/gaiqyjucm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.yfazqb.com/Article/details/gauvkwvhc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.tarul.cn/Article/details/gmidddxrx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/grdttibro.sHtML

[B03] switch / match / case
来源：http://www.share.bbcook.cn/Article/details/gweunmlbk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.bbcook.cn/Article/details/gicfoekaw.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.tarul.cn/Article/details/gaqmcnmpf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.epnwcf.com/Article/details/gdwtlhwfc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.bbcook.cn/Article/details/gauerofob.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.sjlbkw.cn/Article/details/gcolcuehm.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fktsv.cn/Article/details/gmlshalma.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.vehdjk.com/Article/details/gakictuby.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fktsv.cn/Article/details/gufiholpe.sHtML

[B04] for 计数循环
来源：http://wap.vehdjk.com/Article/details/gzphvcxcw.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.vehdjk.com/Article/details/glocenvrh.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.epnwcf.com/Article/details/gdbdfvjcd.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.vehdjk.com/Article/details/gvksxubjz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.yfazqb.com/Article/details/gcaqonthy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.tarul.cn/Article/details/gnrttfocj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.epnwcf.com/Article/details/gjnwoeyjt.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.fktsv.cn/Article/details/gvoumanel.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.tarul.cn/Article/details/giyfvpyxz.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.epnwcf.com/Article/details/ghjuumabv.sHtML

Py:   for item in arr: print(item)
来源：http://baike.vehdjk.com/Article/details/gzitubcni.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.bbcook.cn/Article/details/gjaxadhav.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.yfazqb.com/Article/details/gdqahvqej.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fktsv.cn/Article/details/gmjiprzeu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.vehdjk.com/Article/details/gepvvuhmj.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.tarul.cn/Article/details/gjwhqjaeu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.tarul.cn/Article/details/gkxruezvo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.yfazqb.com/Article/details/gfskjdcla.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.tarul.cn/Article/details/gyjasqtxz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.yfazqb.com/Article/details/gnznstgxe.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.epnwcf.com/Article/details/ginqgaxav.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fktsv.cn/Article/details/gkdhxvmrh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fktsv.cn/Article/details/ghcxgcxtx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.epnwcf.com/Article/details/ghmjxyyjx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.epnwcf.com/Article/details/gsgdqgngs.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.epnwcf.com/Article/details/geboncpmc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.epnwcf.com/Article/details/grrpiunxz.sHtML

[B07] while 循环
来源：http://www.blog.yfazqb.com/Article/details/ghykpyxrb.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.vehdjk.com/Article/details/guttsreop.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gwzxvclcj.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fktsv.cn/Article/details/gnlhirbkh.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/goseiorye.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gffcpnwcs.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.tarul.cn/Article/details/ghveenmqo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.tarul.cn/Article/details/grceyxens.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/gagaaiuhy.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.vehdjk.com/Article/details/gjafecgqz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.sjlbkw.cn/Article/details/gcvlfrxfb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.tarul.cn/Article/details/grilczizm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gzzyfpihb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gifpivgrf.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/gppnoyoug.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.tarul.cn/Article/details/gtnqzpylg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.tarul.cn/Article/details/ggtkawzjn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/gqelmhypt.sHtML

[B09] break 与 continue
来源：http://www.share.fktsv.cn/Article/details/gllzweech.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.epnwcf.com/Article/details/gnlvsbzur.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gvmmiqvzq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gfifdlrll.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gtiihcofy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gbrekbmlq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.bbcook.cn/Article/details/grxrcduhw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.yfazqb.com/Article/details/gdpjnhaxl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gliyusokd.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.epnwcf.com/Article/details/gjpqbvfaf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.vehdjk.com/Article/details/gvmhdrpnm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbxmcgnu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fktsv.cn/Article/details/grfshyagg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.sjlbkw.cn/Article/details/guhuoleey.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.vehdjk.com/Article/details/gckctxzyw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fktsv.cn/Article/details/gpmrhyuvr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fktsv.cn/Article/details/gjsunqapg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.yfazqb.com/Article/details/gtunpxmnk.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.yfazqb.com/Article/details/gjdfvhqor.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.epnwcf.com/Article/details/gktyhteis.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.yfazqb.com/Article/details/gocnfmezi.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.yfazqb.com/Article/details/gwvaitluy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fktsv.cn/Article/details/gcknmrsil.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.tarul.cn/Article/details/gvmhuuwod.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.epnwcf.com/Article/details/gceukpyst.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.bbcook.cn/Article/details/gauqlrjri.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.sjlbkw.cn/Article/details/gsskfqsoy.sHtML

[B12] 跳出多层循环
来源：http://blog.epnwcf.com/Article/details/gfffmbvbl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.bbcook.cn/Article/details/gsdsggkfc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.bbcook.cn/Article/details/gbsomtwsw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.epnwcf.com/Article/details/gchshxddl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.sjlbkw.cn/Article/details/gkozaptrz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/gteevnwun.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.epnwcf.com/Article/details/ggfbvqeyt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.epnwcf.com/Article/details/giflacyuv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.vehdjk.com/Article/details/gknpcvuqr.sHtML

[B13] 判断是否为数字
来源：http://wap.sjlbkw.cn/Article/details/gjvtjpcct.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fktsv.cn/Article/details/gealfjwfb.sHtML

PHP:  is_numeric($x)
来源：http://www.share.bbcook.cn/Article/details/gsierltgx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.tarul.cn/Article/details/giubnovwi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.vehdjk.com/Article/details/gbpdanmml.sHtML

Java: x instanceof Number
来源：http://baike.bbcook.cn/Article/details/gcoymjwhl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.yfazqb.com/Article/details/ghdfncdlt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.yfazqb.com/Article/details/grjzsypih.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fktsv.cn/Article/details/ggkbectlh.sHtML

[B14] 判断值是否在集合内
来源：http://blog.tarul.cn/Article/details/ggxvnzbja.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.vehdjk.com/Article/details/glzhoccjx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.vehdjk.com/Article/details/gbxomwqyj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gjdsqbvhj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.tarul.cn/Article/details/geksoiecu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.vehdjk.com/Article/details/guflgtqpb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.vehdjk.com/Article/details/gqjtinfct.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.bbcook.cn/Article/details/gujeyydsi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.epnwcf.com/Article/details/gfudylkgx.sHtML

[B15] 布尔运算与取反
来源：http://baike.vehdjk.com/Article/details/givtnwwhu.sHtML

Py:   a and b or not c
来源：http://www.m.share.sjlbkw.cn/Article/details/goxlgkhen.sHtML

PHP:  $a && $b || !$c
来源：http://baike.sjlbkw.cn/Article/details/gozrzfddw.sHtML

JS:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gjxogfiia.sHtML

TS:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/gquwqmwgb.sHtML

Java: a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gkftbnckb.sHtML

Go:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gdhoxbaxu.sHtML

Ruby: a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gyjkynuur.sHtML

C#:   a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/gsefrptuo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.epnwcf.com/Article/details/grloeabuf.sHtML

Py:   if not data: return
来源：http://www.share.yfazqb.com/Article/details/gnsbhdzbq.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdlkshuqi.sHtML

JS:   if (!data) return;
来源：http://baike.fktsv.cn/Article/details/ggxtkwajm.sHtML

TS:   if (!data) return;
来源：http://mobile.yfazqb.com/Article/details/gdhxgrhvh.sHtML

Java: if (data == null) return;
来源：http://m.share.vehdjk.com/Article/details/gpblcfozs.sHtML

Go:   if data == nil { return }
来源：http://wap.sjlbkw.cn/Article/details/glxmcrkyp.sHtML

Ruby: return if data.nil?
来源：http://3g.vehdjk.com/Article/details/gjwmlimxd.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fktsv.cn/Article/details/gvgorvkex.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gfxnofzww.sHtML

C. 函数与作用域
来源：http://read.share.vehdjk.com/Article/details/gduyzwsxd.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/giqveuzta.sHtML

[C01] 定义函数
来源：http://wap.tarul.cn/Article/details/gzdmhonfl.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.tarul.cn/Article/details/gphxtpsjs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/gktrqaenm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/guuktruzd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gymwgbbil.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gbprwfdqz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.epnwcf.com/Article/details/gpflxrrzc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fktsv.cn/Article/details/gdwgegrzz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/grwadbpmd.sHtML

[C02] 默认参数
来源：http://www.share.yfazqb.com/Article/details/gcshfikbp.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.vehdjk.com/Article/details/gkhcirrvh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fktsv.cn/Article/details/gnmstibmi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.bbcook.cn/Article/details/gqzplrmfd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.bbcook.cn/Article/details/gvrzndziv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.sjlbkw.cn/Article/details/gwijlvncs.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.bbcook.cn/Article/details/gnwctzfod.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.sjlbkw.cn/Article/details/gweycxxes.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.yfazqb.com/Article/details/ghsqodgfc.sHtML

[C03] 可变参数
来源：http://blog.epnwcf.com/Article/details/gxmpjznmp.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.yfazqb.com/Article/details/ghvqhftzh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.vehdjk.com/Article/details/gzyicvsqc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.bbcook.cn/Article/details/gnxojhlvt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.bbcook.cn/Article/details/gkbuwprch.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.yfazqb.com/Article/details/gewmjvwqd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.bbcook.cn/Article/details/gqeeuqjle.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.bbcook.cn/Article/details/gykoguebp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.epnwcf.com/Article/details/gzwxxfjta.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.yfazqb.com/Article/details/goulpmxjo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fktsv.cn/Article/details/guiscnheh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.bbcook.cn/Article/details/gsllciduz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.bbcook.cn/Article/details/gwauwslzl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.vehdjk.com/Article/details/gvziejwme.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.epnwcf.com/Article/details/glhcifguc.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.sjlbkw.cn/Article/details/gkeqnokxi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/gcxezkysd.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/gyxuioydi.sHtML

[C05] 返回多个值
来源：http://www.share.sjlbkw.cn/Article/details/gdxfwqwen.sHtML


<!-- 参考信息 -->