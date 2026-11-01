代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://baike.bbcook.cn/Article/details/ghvifreap.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.vehdjk.com/Article/details/gywpalali.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.epnwcf.com/Article/details/gnznewtdv.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.bbcook.cn/Article/details/gbfudzewn.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.sjlbkw.cn/Article/details/ggvztfrxz.sHtML

[A15] 空值判断与默认值
来源：http://baike.epnwcf.com/Article/details/gvcaymypb.sHtML

Py:   value = data or "默认值"
来源：http://blog.bbcook.cn/Article/details/grxnnbdaw.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.bbcook.cn/Article/details/grdfujawb.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.bbcook.cn/Article/details/gimeixaff.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.yfazqb.com/Article/details/gdnltoyog.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.bbcook.cn/Article/details/gasxbexsw.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.fktsv.cn/Article/details/gsiwblqwk.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.epnwcf.com/Article/details/ghopscluw.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.epnwcf.com/Article/details/gnniygbka.sHtML

[A16] 真假值判断规则
来源：http://read.share.sjlbkw.cn/Article/details/grmvqkstt.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.yfazqb.com/Article/details/gqfknljsu.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.sjlbkw.cn/Article/details/ggqwipkeu.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.sjlbkw.cn/Article/details/gwgmkpdrx.sHtML

TS:   if (!x) {}
来源：http://www.share.yfazqb.com/Article/details/gjejckzen.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.fktsv.cn/Article/details/gkqxauexo.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.sjlbkw.cn/Article/details/gpvfpulil.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.tarul.cn/Article/details/gcmyychss.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.bbcook.cn/Article/details/gqmnzkpae.sHtML

[A17] 位运算
来源：http://www.blog.sjlbkw.cn/Article/details/gyawhigol.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gjgchxhza.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.bbcook.cn/Article/details/grxiftekp.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.yfazqb.com/Article/details/glzdcxxtk.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.fktsv.cn/Article/details/gwbzxpnup.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/gemdgxymf.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/gzghxvwqb.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.vehdjk.com/Article/details/gnsgfblar.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/gcsiyujio.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.tarul.cn/Article/details/gwxhtxgbt.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.tarul.cn/Article/details/ggqgohgfq.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.fktsv.cn/Article/details/ghnmfqpxl.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.vehdjk.com/Article/details/guzlantnx.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.bbcook.cn/Article/details/gvueyrgir.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.fktsv.cn/Article/details/goevhoqab.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.sjlbkw.cn/Article/details/gkypeqbnp.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.yfazqb.com/Article/details/glnclniqx.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.yfazqb.com/Article/details/gpvefqwmn.sHtML

[A19] 交换两个变量
来源：http://read.share.yfazqb.com/Article/details/gbvqmmrpy.sHtML

Py:   a, b = b, a
来源：http://mobile.tarul.cn/Article/details/gxaetbzxe.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.epnwcf.com/Article/details/gctxvpmdh.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.vehdjk.com/Article/details/gyqvmorcb.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.vehdjk.com/Article/details/giurwefhe.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.tarul.cn/Article/details/grofpbgvb.sHtML

Go:   a, b = b, a
来源：http://m.share.bbcook.cn/Article/details/gbjwgeukk.sHtML

Ruby: a, b = b, a
来源：http://read.share.sjlbkw.cn/Article/details/gldixfzqo.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.vehdjk.com/Article/details/gglhakvkv.sHtML

[A20] 读取标准输入
来源：http://read.share.yfazqb.com/Article/details/gbqalxuma.sHtML

Py:   name = input("请输入：")
来源：http://wap.epnwcf.com/Article/details/giomvqalh.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.bbcook.cn/Article/details/gtuwlvcia.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.fktsv.cn/Article/details/grbjycogx.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.sjlbkw.cn/Article/details/garjlelrp.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.sjlbkw.cn/Article/details/ggemksgva.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.vehdjk.com/Article/details/glxlosvcv.sHtML

Ruby: gets.chomp
来源：http://www.blog.vehdjk.com/Article/details/gkcoindps.sHtML

C#:   Console.ReadLine();
来源：http://mobile.vehdjk.com/Article/details/gbmdqbacd.sHtML

[A21] 保留指定小数位输出
来源：http://baike.sjlbkw.cn/Article/details/gbopatvyl.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.yfazqb.com/Article/details/ghjtldqnj.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.bbcook.cn/Article/details/gbsnmfuyt.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.yfazqb.com/Article/details/gfctrzemq.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.vehdjk.com/Article/details/gpmcwfegv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.yfazqb.com/Article/details/gbpjharxg.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.vehdjk.com/Article/details/gajoirqby.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.tarul.cn/Article/details/gaeefsdlq.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.bbcook.cn/Article/details/gmsvoixyu.sHtML

[A22] 获取字符串长度
来源：http://mobile.yfazqb.com/Article/details/grbirpblt.sHtML

Py:   len(s)
来源：http://read.share.sjlbkw.cn/Article/details/gxpkwihyf.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.yfazqb.com/Article/details/grgbvkdbw.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.bbcook.cn/Article/details/gbfnahghf.sHtML

TS:   s.length
来源：http://wap.vehdjk.com/Article/details/ggnlejptm.sHtML

Java: s.length()
来源：http://www.blog.yfazqb.com/Article/details/gpifeuubm.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.vehdjk.com/Article/details/grjgqnpjy.sHtML

Ruby: s.length
来源：http://read.share.epnwcf.com/Article/details/ggtogjwpq.sHtML

C#:   s.Length
来源：http://wap.bbcook.cn/Article/details/gklrbeffz.sHtML

[A23] 大小写转换
来源：http://www.blog.yfazqb.com/Article/details/glecttnkl.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.tarul.cn/Article/details/gcbkbsvut.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.vehdjk.com/Article/details/geakxcyef.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.vehdjk.com/Article/details/gfhtxjtes.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.vehdjk.com/Article/details/gsroanjmn.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.bbcook.cn/Article/details/gdwydteoe.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.fktsv.cn/Article/details/gchhktfee.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.fktsv.cn/Article/details/grfzynuij.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.vehdjk.com/Article/details/gnorbfycj.sHtML

[A24] 去除首尾空白
来源：http://read.share.tarul.cn/Article/details/gsggctgln.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.tarul.cn/Article/details/glidvhene.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.fktsv.cn/Article/details/gtbhatcdj.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.epnwcf.com/Article/details/grtmrlwdf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.epnwcf.com/Article/details/gxipyzfrs.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.bbcook.cn/Article/details/geltdgnuy.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.fktsv.cn/Article/details/geqaibqpq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.fktsv.cn/Article/details/gtjbkzjjg.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.epnwcf.com/Article/details/gedtskuww.sHtML

[A25] 字符串比较
来源：http://m.share.yfazqb.com/Article/details/gsbmnvtlu.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.yfazqb.com/Article/details/gtrwnfnbw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.bbcook.cn/Article/details/gzlsadnew.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.epnwcf.com/Article/details/gwqjmcktj.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fktsv.cn/Article/details/gwoznzawf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.yfazqb.com/Article/details/gjpyazowt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.vehdjk.com/Article/details/gwiggbxok.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.sjlbkw.cn/Article/details/gyghjanpg.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.yfazqb.com/Article/details/gmhcwsvqb.sHtML

[A26] 类型转换总览
来源：http://baike.vehdjk.com/Article/details/glcnnsrtj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.vehdjk.com/Article/details/gjlpdgwbw.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.vehdjk.com/Article/details/gymitlhgy.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.bbcook.cn/Article/details/gckgprosn.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.yfazqb.com/Article/details/gddivdibu.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.bbcook.cn/Article/details/gdabsfrwv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.epnwcf.com/Article/details/gtgwnvbkr.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.bbcook.cn/Article/details/grrrhahco.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.vehdjk.com/Article/details/gqfaqhsjl.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/ggucoixra.sHtML

B. 流程控制
来源：http://3g.epnwcf.com/Article/details/gvhmgidbm.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gnulkjuls.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.bbcook.cn/Article/details/gacffhhnb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.vehdjk.com/Article/details/ggdstpija.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.tarul.cn/Article/details/gcfxubaqy.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.vehdjk.com/Article/details/gcnxsgsuh.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.bbcook.cn/Article/details/gcikywvmt.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.bbcook.cn/Article/details/gjybafyjp.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzibnesur.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.epnwcf.com/Article/details/gjcchyurm.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.sjlbkw.cn/Article/details/gvlbugekk.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.bbcook.cn/Article/details/gsumhvvdt.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.bbcook.cn/Article/details/gvibyhvrg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.tarul.cn/Article/details/grslnkcpy.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/gadkqvede.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/grhwelfel.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/gmhccnnpy.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.vehdjk.com/Article/details/ghhzlegxc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.vehdjk.com/Article/details/glkapgwyx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/gpqqlikvo.sHtML

[B03] switch / match / case
来源：http://3g.bbcook.cn/Article/details/gdgmutmxh.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.sjlbkw.cn/Article/details/gdlcrbjif.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fktsv.cn/Article/details/goedzeqfs.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.yfazqb.com/Article/details/gapbtbvwc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.vehdjk.com/Article/details/ghtjjihmm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.bbcook.cn/Article/details/gnfsesffj.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.yfazqb.com/Article/details/gwqhlewln.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.vehdjk.com/Article/details/gnspfgnyr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fktsv.cn/Article/details/gtptqmhwp.sHtML

[B04] for 计数循环
来源：http://www.blog.sjlbkw.cn/Article/details/gwiwupoun.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.tarul.cn/Article/details/glccnnmww.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.vehdjk.com/Article/details/gieagsore.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.epnwcf.com/Article/details/gtgjqhacp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.epnwcf.com/Article/details/gkmzkmurq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.bbcook.cn/Article/details/gizwxyqfl.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.sjlbkw.cn/Article/details/gxrduijvs.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.sjlbkw.cn/Article/details/gruhillrd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/gtolfdcbl.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.epnwcf.com/Article/details/gbulxndjm.sHtML

Py:   for item in arr: print(item)
来源：http://3g.vehdjk.com/Article/details/gkhwuluhx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.sjlbkw.cn/Article/details/gkbfvftcn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.sjlbkw.cn/Article/details/gppidnidf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fktsv.cn/Article/details/gpfnectav.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.tarul.cn/Article/details/gooyyaldo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.fktsv.cn/Article/details/guqjulkux.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.epnwcf.com/Article/details/gwesvjruv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.tarul.cn/Article/details/gecumgxfi.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.yfazqb.com/Article/details/grxflrjye.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.tarul.cn/Article/details/gpoitnhbm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.tarul.cn/Article/details/gngsuldth.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtmtmsiv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.yfazqb.com/Article/details/girvaziqm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.sjlbkw.cn/Article/details/gjuijdqix.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.fktsv.cn/Article/details/gwkfcyoys.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.yfazqb.com/Article/details/gjsqwezdi.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.epnwcf.com/Article/details/ghkpylumh.sHtML

[B07] while 循环
来源：http://read.share.epnwcf.com/Article/details/gvyxgegjo.sHtML

Py:   while i < 10: i += 1
来源：http://3g.yfazqb.com/Article/details/gtufuzfhx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.yfazqb.com/Article/details/gjqytfjly.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gooaniivx.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gyycufbit.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.tarul.cn/Article/details/grfspjhjz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.epnwcf.com/Article/details/gpubvseec.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.yfazqb.com/Article/details/gmdidpmaa.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/grstsheek.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fktsv.cn/Article/details/gvmipedxv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.vehdjk.com/Article/details/grcbljxux.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/glbfygixg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/ghbxevlrn.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.epnwcf.com/Article/details/gdhplagyg.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/guqpvajpc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.bbcook.cn/Article/details/gkgskydqb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.sjlbkw.cn/Article/details/gdswbwnxd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gsexzftht.sHtML

[B09] break 与 continue
来源：http://read.share.tarul.cn/Article/details/goxhoksbh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.vehdjk.com/Article/details/gaqwfodhm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gqglanipm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/guswyovzs.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gtbuckzec.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/gncxkjhvo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.tarul.cn/Article/details/gdtwflxhz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fktsv.cn/Article/details/gnayuonqb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gsfyznbdr.sHtML

[B10] 遍历同时拿索引
来源：http://3g.epnwcf.com/Article/details/gnrlpurnt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.tarul.cn/Article/details/ghgywqtwz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.bbcook.cn/Article/details/gsnodkzvs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.bbcook.cn/Article/details/ggouxhgsi.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.sjlbkw.cn/Article/details/gwpfxgvis.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.vehdjk.com/Article/details/gsgouzbjg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fktsv.cn/Article/details/gagsfcsml.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.vehdjk.com/Article/details/gjurcxchl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.sjlbkw.cn/Article/details/gfygjnhbs.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.epnwcf.com/Article/details/ghznvxgyu.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fktsv.cn/Article/details/grgtgkpif.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fktsv.cn/Article/details/gtddroyie.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.epnwcf.com/Article/details/gnpqrktqi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fktsv.cn/Article/details/gyuzfmxes.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.vehdjk.com/Article/details/gmgpygcoc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.epnwcf.com/Article/details/glasgcsed.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fktsv.cn/Article/details/gbahriyxw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.vehdjk.com/Article/details/gculpyzbj.sHtML

[B12] 跳出多层循环
来源：http://3g.bbcook.cn/Article/details/gmfrkdovv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.tarul.cn/Article/details/gelpxsycd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.tarul.cn/Article/details/gnlbfcque.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/gmfmnznxr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.epnwcf.com/Article/details/gvnokhlrj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.yfazqb.com/Article/details/gyzzitoli.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.bbcook.cn/Article/details/ggqysbxhm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fktsv.cn/Article/details/gpnxzxrwl.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.bbcook.cn/Article/details/ghwynzhcz.sHtML

[B13] 判断是否为数字
来源：http://wap.sjlbkw.cn/Article/details/gbowbmuic.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fktsv.cn/Article/details/gymcfqwql.sHtML

PHP:  is_numeric($x)
来源：http://3g.sjlbkw.cn/Article/details/gkpnnhqed.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.tarul.cn/Article/details/gvgmfgvan.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fktsv.cn/Article/details/gvdcpoqii.sHtML

Java: x instanceof Number
来源：http://wap.yfazqb.com/Article/details/gjlchmkig.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.yfazqb.com/Article/details/gireehgms.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.yfazqb.com/Article/details/gyumdzfeq.sHtML

C#:   x is int or double or decimal
来源：http://read.share.epnwcf.com/Article/details/ggmtcvltq.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fktsv.cn/Article/details/gtvoaiwar.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.bbcook.cn/Article/details/gkqvjkjky.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.bbcook.cn/Article/details/gsycopzzp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fktsv.cn/Article/details/gbrarezit.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.epnwcf.com/Article/details/gmsiecsze.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.tarul.cn/Article/details/gzrouhtfg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.yfazqb.com/Article/details/gqzswtzhf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.vehdjk.com/Article/details/gmdloqcag.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.bbcook.cn/Article/details/gtcbfkjzs.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.tarul.cn/Article/details/ghicubuwe.sHtML

Py:   a and b or not c
来源：http://www.m.share.bbcook.cn/Article/details/gujflvsby.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.tarul.cn/Article/details/gywsgsfnt.sHtML

JS:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gvixmhmcw.sHtML

TS:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/gzixnndsp.sHtML

Java: a && b || !c
来源：http://www.share.tarul.cn/Article/details/gtzhqkiqk.sHtML

Go:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gjkulcnpb.sHtML

Ruby: a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gijdkahcr.sHtML

C#:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/ghscczpzb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.bbcook.cn/Article/details/gslnxctup.sHtML

Py:   if not data: return
来源：http://www.blog.vehdjk.com/Article/details/gfkixhpla.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.bbcook.cn/Article/details/gsvenknxi.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fktsv.cn/Article/details/gsxvqqloe.sHtML

TS:   if (!data) return;
来源：http://m.share.sjlbkw.cn/Article/details/gxrfhebbb.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fktsv.cn/Article/details/glwnntwrv.sHtML

Go:   if data == nil { return }
来源：http://m.share.vehdjk.com/Article/details/gkxyzlqir.sHtML

Ruby: return if data.nil?
来源：http://www.share.tarul.cn/Article/details/glyseygnt.sHtML

C#:   if (data == null) return;
来源：http://read.share.sjlbkw.cn/Article/details/gzglerhrp.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/guqfvzoly.sHtML

C. 函数与作用域
来源：http://www.blog.vehdjk.com/Article/details/gzjxwlrfx.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gyrwpyeld.sHtML

[C01] 定义函数
来源：http://read.share.sjlbkw.cn/Article/details/gzaadkfdj.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fktsv.cn/Article/details/gsqvgtiot.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/gxhxdwbun.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gnvxphluz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/goukukqjs.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gzjavqtic.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.yfazqb.com/Article/details/gdwwvkyul.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.tarul.cn/Article/details/gsqxzynzm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gwhebibse.sHtML

[C02] 默认参数
来源：http://www.blog.yfazqb.com/Article/details/greawxeii.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.vehdjk.com/Article/details/grkuaperr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.vehdjk.com/Article/details/grmtxdnan.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/giubjnvrm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fktsv.cn/Article/details/gowbfguwn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.yfazqb.com/Article/details/guylxjlym.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.epnwcf.com/Article/details/gtisrxpqg.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.bbcook.cn/Article/details/gwdmyzvxr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.vehdjk.com/Article/details/gyntslwcp.sHtML

[C03] 可变参数
来源：http://read.share.vehdjk.com/Article/details/gpozbqrlz.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.tarul.cn/Article/details/gazkkamdr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.yfazqb.com/Article/details/gexqhrxkr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.yfazqb.com/Article/details/gptncfbkl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.tarul.cn/Article/details/gqoaeviaf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.tarul.cn/Article/details/ghhrrsmiw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fktsv.cn/Article/details/gvyoexaew.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.sjlbkw.cn/Article/details/gebrntzmq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.bbcook.cn/Article/details/gojcaoivs.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.vehdjk.com/Article/details/gdaqjkvud.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.vehdjk.com/Article/details/gzxoiesfo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.sjlbkw.cn/Article/details/gzosvpzae.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.bbcook.cn/Article/details/gmrmcvznr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.vehdjk.com/Article/details/gedtspulk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.vehdjk.com/Article/details/griyoqgvr.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.epnwcf.com/Article/details/gjehkdwpk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gnviwdogt.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/ghxhsygjt.sHtML

[C05] 返回多个值
来源：http://mobile.bbcook.cn/Article/details/gckynjxxy.sHtML


<!-- 参考信息 -->