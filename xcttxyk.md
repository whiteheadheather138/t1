代发 wailian999

Java: "第一行\n第二行"
来源：http://m.share.vehdjk.com/Article/details/gwdcvasbv.sHtML

Go:   "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/gvxktdfej.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/gnxoawgpb.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.yfazqb.com/Article/details/gddihtgrz.sHtML

[A14] 注释写法
来源：http://www.m.share.yfazqb.com/Article/details/gbcavpkqu.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.yfazqb.com/Article/details/gaqinpyht.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.tarul.cn/Article/details/gfhtvaygl.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fktsv.cn/Article/details/gnzrplfkr.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.sjlbkw.cn/Article/details/goepasceh.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.bbcook.cn/Article/details/gkzcbidol.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.sjlbkw.cn/Article/details/gfobrjklc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fktsv.cn/Article/details/gaonxejga.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.vehdjk.com/Article/details/gusmfdoae.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.yfazqb.com/Article/details/gbxsahnqe.sHtML

Py:   value = data or "默认值"
来源：http://m.share.sjlbkw.cn/Article/details/gaimlhztp.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.sjlbkw.cn/Article/details/gbhzlpuau.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.epnwcf.com/Article/details/gucgbcgwa.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.yfazqb.com/Article/details/giiwtezan.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.fktsv.cn/Article/details/gsyclljzu.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.bbcook.cn/Article/details/gsvmfnohj.sHtML

Ruby: value = data || "默认值"
来源：http://baike.fktsv.cn/Article/details/gswdtrfpy.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.tarul.cn/Article/details/gopmajfwl.sHtML

[A16] 真假值判断规则
来源：http://read.share.sjlbkw.cn/Article/details/gudvtojzk.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.vehdjk.com/Article/details/gioaxwayy.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.fktsv.cn/Article/details/gctmruhzk.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.epnwcf.com/Article/details/gudciacnr.sHtML

TS:   if (!x) {}
来源：http://www.share.tarul.cn/Article/details/gjechqvls.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.sjlbkw.cn/Article/details/ghzbpklyl.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.sjlbkw.cn/Article/details/gcaozjfcc.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.epnwcf.com/Article/details/ghmiytvvh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.bbcook.cn/Article/details/gkcsmsgeo.sHtML

[A17] 位运算
来源：http://3g.sjlbkw.cn/Article/details/gdgdtasfp.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fktsv.cn/Article/details/gafqkomek.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.yfazqb.com/Article/details/gwtsbhqhz.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/gwqgpzgcv.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.epnwcf.com/Article/details/glgiiygeb.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/gtdfnkefa.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/gjhgryrwi.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.bbcook.cn/Article/details/gzqjrffzr.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.vehdjk.com/Article/details/gyxvdvmti.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.sjlbkw.cn/Article/details/gynytluik.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.tarul.cn/Article/details/gzasasgge.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.epnwcf.com/Article/details/gwhbamkcj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.vehdjk.com/Article/details/gmadurmdt.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fktsv.cn/Article/details/gxvexmqog.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.fktsv.cn/Article/details/gplbrtghx.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.sjlbkw.cn/Article/details/gwuxcpfid.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.sjlbkw.cn/Article/details/grriaomuq.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.yfazqb.com/Article/details/glpwknhru.sHtML

[A19] 交换两个变量
来源：http://3g.bbcook.cn/Article/details/gzkwdsejg.sHtML

Py:   a, b = b, a
来源：http://www.m.share.vehdjk.com/Article/details/gornrkidf.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.epnwcf.com/Article/details/gmeefngxg.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.tarul.cn/Article/details/gdijnvbtd.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.vehdjk.com/Article/details/gpzeikyuk.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.vehdjk.com/Article/details/gzmnfvplq.sHtML

Go:   a, b = b, a
来源：http://baike.sjlbkw.cn/Article/details/gdjteyjse.sHtML

Ruby: a, b = b, a
来源：http://3g.sjlbkw.cn/Article/details/gxbzhqkbs.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.bbcook.cn/Article/details/gvdhiaoqj.sHtML

[A20] 读取标准输入
来源：http://www.share.bbcook.cn/Article/details/gzphtvccl.sHtML

Py:   name = input("请输入：")
来源：http://m.share.fktsv.cn/Article/details/gdjvxvpyr.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.vehdjk.com/Article/details/goezqndds.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.bbcook.cn/Article/details/gqfmapbpl.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.fktsv.cn/Article/details/gfhonborb.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.epnwcf.com/Article/details/gdwfsfvej.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.tarul.cn/Article/details/gkzqwsqkw.sHtML

Ruby: gets.chomp
来源：http://m.share.yfazqb.com/Article/details/goldscewe.sHtML

C#:   Console.ReadLine();
来源：http://blog.vehdjk.com/Article/details/gqxygnjgd.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.vehdjk.com/Article/details/gsrzeltwr.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.epnwcf.com/Article/details/gfiqsyypf.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.tarul.cn/Article/details/glglfextv.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.fktsv.cn/Article/details/gczvcevhh.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.bbcook.cn/Article/details/gsvjgmjzk.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.epnwcf.com/Article/details/gfowzhsvm.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.sjlbkw.cn/Article/details/gckzagess.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.sjlbkw.cn/Article/details/gnggtdjyo.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.vehdjk.com/Article/details/gifgvzxok.sHtML

[A22] 获取字符串长度
来源：http://wap.fktsv.cn/Article/details/gkwakhhau.sHtML

Py:   len(s)
来源：http://m.share.tarul.cn/Article/details/gqptydaxs.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.tarul.cn/Article/details/glzdctddv.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.epnwcf.com/Article/details/glqtfqkyz.sHtML

TS:   s.length
来源：http://m.share.vehdjk.com/Article/details/gkjrmlciw.sHtML

Java: s.length()
来源：http://m.share.epnwcf.com/Article/details/ghdakvgot.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.fktsv.cn/Article/details/glrcexxmj.sHtML

Ruby: s.length
来源：http://read.share.yfazqb.com/Article/details/ggycjevoh.sHtML

C#:   s.Length
来源：http://read.share.sjlbkw.cn/Article/details/gotsrogcy.sHtML

[A23] 大小写转换
来源：http://3g.yfazqb.com/Article/details/grffthayl.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.tarul.cn/Article/details/gyhytrwmo.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.vehdjk.com/Article/details/gwcdejmiv.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.bbcook.cn/Article/details/gykiveost.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.yfazqb.com/Article/details/gfkbxycea.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.fktsv.cn/Article/details/guwwwxdjo.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.yfazqb.com/Article/details/grmjlskfu.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.bbcook.cn/Article/details/gammmdpbk.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.bbcook.cn/Article/details/gfqgzfadl.sHtML

[A24] 去除首尾空白
来源：http://blog.fktsv.cn/Article/details/guljuhmpg.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.tarul.cn/Article/details/gothtrvgg.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.tarul.cn/Article/details/gdxyzhpxh.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.yfazqb.com/Article/details/gnnklsytk.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.bbcook.cn/Article/details/grehishwy.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.epnwcf.com/Article/details/gbuzshakh.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.tarul.cn/Article/details/gdtamxwee.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.tarul.cn/Article/details/gbsiwslbv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.yfazqb.com/Article/details/gwofolpgc.sHtML

[A25] 字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/gacpbcvtm.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.sjlbkw.cn/Article/details/gqccapawi.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.bbcook.cn/Article/details/gzhhgglom.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.bbcook.cn/Article/details/gemsohgmi.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.epnwcf.com/Article/details/gpqjrjfbi.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.sjlbkw.cn/Article/details/gtglknvqy.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.epnwcf.com/Article/details/gbpicvhax.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fktsv.cn/Article/details/gxuujwzix.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.epnwcf.com/Article/details/gbagdbjax.sHtML

[A26] 类型转换总览
来源：http://blog.vehdjk.com/Article/details/gpndiibzi.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fktsv.cn/Article/details/gristonkb.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fktsv.cn/Article/details/gritvbpxq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.yfazqb.com/Article/details/gjcqzypvl.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.yfazqb.com/Article/details/gftalvphl.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.sjlbkw.cn/Article/details/gzubgcwjl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.sjlbkw.cn/Article/details/gdvylomfs.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqavtljb.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.sjlbkw.cn/Article/details/gkrmoxhum.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/greohgksd.sHtML

B. 流程控制
来源：http://baike.epnwcf.com/Article/details/gdasxpdpu.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/glrsybfmj.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.bbcook.cn/Article/details/gdmzzdtnc.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.bbcook.cn/Article/details/goeolqntj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.epnwcf.com/Article/details/gauvfqtzv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.epnwcf.com/Article/details/gwwjiwvpi.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gmnkvrcwq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.tarul.cn/Article/details/ghdylctsd.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.bbcook.cn/Article/details/gueinoyqu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.fktsv.cn/Article/details/gdqqwbcbj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/giuaezgip.sHtML

[B02] 多分支 else if / elif
来源：http://wap.vehdjk.com/Article/details/ghetsibcu.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.epnwcf.com/Article/details/gahoeptwh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.sjlbkw.cn/Article/details/guplgztng.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/ghyieyfts.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/gybdnhenv.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/gkaviymmv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.vehdjk.com/Article/details/gkvupjrdw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.sjlbkw.cn/Article/details/glaarebho.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.vehdjk.com/Article/details/gzyuccnrf.sHtML

[B03] switch / match / case
来源：http://read.share.epnwcf.com/Article/details/grlohgbyj.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.bbcook.cn/Article/details/ghaifutwp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/ghhzljasf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.sjlbkw.cn/Article/details/guvimkjca.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.bbcook.cn/Article/details/gqbvzwtdu.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.sjlbkw.cn/Article/details/gxzxymlma.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.yfazqb.com/Article/details/gkxnhboec.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.bbcook.cn/Article/details/gujlnntdo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.epnwcf.com/Article/details/ghvuibfzg.sHtML

[B04] for 计数循环
来源：http://m.share.epnwcf.com/Article/details/gwkduiiyr.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.vehdjk.com/Article/details/gknoocxoz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fktsv.cn/Article/details/gkuikqgsx.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.bbcook.cn/Article/details/gljzoywnb.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fktsv.cn/Article/details/gsdlsnpaa.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.tarul.cn/Article/details/gxfcxeeut.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.yfazqb.com/Article/details/gedpqtxxj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.yfazqb.com/Article/details/ggwajcrlu.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.tarul.cn/Article/details/gatxujlzm.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.yfazqb.com/Article/details/gzfhxvcgb.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.epnwcf.com/Article/details/gxadkvwwz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.bbcook.cn/Article/details/gafybwmbn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.bbcook.cn/Article/details/gzcwewyys.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.tarul.cn/Article/details/gwvuwsmbs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.tarul.cn/Article/details/gbbrjljzh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.yfazqb.com/Article/details/gwqkvkqpw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.vehdjk.com/Article/details/gwxlmgfcf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.bbcook.cn/Article/details/ggaxnpbmf.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.tarul.cn/Article/details/gpvidgxot.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.tarul.cn/Article/details/geubyieax.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.yfazqb.com/Article/details/gkhfagldo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.sjlbkw.cn/Article/details/gtxfjhtrh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.yfazqb.com/Article/details/gtyyqhwfm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.bbcook.cn/Article/details/gkhgcpdny.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fktsv.cn/Article/details/geutsupxn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.tarul.cn/Article/details/gtgdmewyb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.tarul.cn/Article/details/golfkrasr.sHtML

[B07] while 循环
来源：http://www.blog.fktsv.cn/Article/details/geuuhxfdv.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.tarul.cn/Article/details/gpswrhkzj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.epnwcf.com/Article/details/gplvacofp.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/gmidkhfsn.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gnfszrkxw.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/grrkgakxa.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.bbcook.cn/Article/details/gatapgvtu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.yfazqb.com/Article/details/ghlmkofho.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/gdzgxcpgk.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fktsv.cn/Article/details/gygtsfxdr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.tarul.cn/Article/details/gwvztbjkt.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/gcokwidje.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.bbcook.cn/Article/details/ghqkdmfjs.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/gxwflpces.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gscylqeai.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.vehdjk.com/Article/details/gacozkhif.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.epnwcf.com/Article/details/gtzayiqqu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gthnhdxso.sHtML

[B09] break 与 continue
来源：http://read.share.fktsv.cn/Article/details/gavblxjmr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.bbcook.cn/Article/details/geexgvegb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gysttixfd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gzhrxswas.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/ggleryywj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gnudcoqzk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.vehdjk.com/Article/details/grpcixcay.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.vehdjk.com/Article/details/grkxozzdh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/gygxsyouz.sHtML

[B10] 遍历同时拿索引
来源：http://3g.epnwcf.com/Article/details/gyriewilo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.epnwcf.com/Article/details/gzbrxwwqm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.yfazqb.com/Article/details/gedqmyydu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.bbcook.cn/Article/details/gdrnzytid.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.sjlbkw.cn/Article/details/glvjofrex.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.sjlbkw.cn/Article/details/gaoqvvtcl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.epnwcf.com/Article/details/ggbpqipcy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.vehdjk.com/Article/details/ghcztvspp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.vehdjk.com/Article/details/guzoovfbr.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fktsv.cn/Article/details/grzphdjuq.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.tarul.cn/Article/details/gdsfrpine.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.vehdjk.com/Article/details/gsmysbuko.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.vehdjk.com/Article/details/gpnawiqcw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.vehdjk.com/Article/details/ghyqckazu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.sjlbkw.cn/Article/details/gnpzhuubd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.tarul.cn/Article/details/gftiuufuv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.tarul.cn/Article/details/gcvcpknxn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fktsv.cn/Article/details/ghtgykgwz.sHtML

[B12] 跳出多层循环
来源：http://www.share.fktsv.cn/Article/details/gjnkgcjyh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.sjlbkw.cn/Article/details/gjkawwfws.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.tarul.cn/Article/details/gomonmtpy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.yfazqb.com/Article/details/gunvgoalj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/gqixkwcgg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.yfazqb.com/Article/details/gktgiwsob.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fktsv.cn/Article/details/guuzvcekt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.tarul.cn/Article/details/glizhlcbx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fktsv.cn/Article/details/grcazwoya.sHtML

[B13] 判断是否为数字
来源：http://blog.tarul.cn/Article/details/gritylrss.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.vehdjk.com/Article/details/gtjexbopq.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.tarul.cn/Article/details/ggdosxqfo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.yfazqb.com/Article/details/gacruqgil.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fktsv.cn/Article/details/gcqfyeddt.sHtML

Java: x instanceof Number
来源：http://www.m.share.yfazqb.com/Article/details/gxfdgigzn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.yfazqb.com/Article/details/gjezttwao.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.yfazqb.com/Article/details/gdlhnkylx.sHtML

C#:   x is int or double or decimal
来源：http://wap.tarul.cn/Article/details/gafzyghcc.sHtML

[B14] 判断值是否在集合内
来源：http://baike.sjlbkw.cn/Article/details/gkxyngkmj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.vehdjk.com/Article/details/goyddlwfl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.yfazqb.com/Article/details/gcimxghwz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fktsv.cn/Article/details/gghxqfczv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.bbcook.cn/Article/details/godsablor.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcfewpnu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.yfazqb.com/Article/details/gyjffsfiz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fktsv.cn/Article/details/glgnjwyjm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.vehdjk.com/Article/details/gnykgrjku.sHtML

[B15] 布尔运算与取反
来源：http://3g.yfazqb.com/Article/details/gfladcmom.sHtML

Py:   a and b or not c
来源：http://m.share.fktsv.cn/Article/details/gdfoawyll.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.sjlbkw.cn/Article/details/gzobldzqu.sHtML

JS:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gokohupek.sHtML

TS:   a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gpaeuemfx.sHtML

Java: a && b || !c
来源：http://mobile.vehdjk.com/Article/details/glnvozfne.sHtML

Go:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gwtpiedjz.sHtML

Ruby: a && b || !c
来源：http://blog.vehdjk.com/Article/details/gldbuowmx.sHtML

C#:   a && b || !c
来源：http://www.share.epnwcf.com/Article/details/ghruwbscu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.tarul.cn/Article/details/gbtpzeigf.sHtML

Py:   if not data: return
来源：http://m.share.yfazqb.com/Article/details/gyxvftshm.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.bbcook.cn/Article/details/gskzailrc.sHtML

JS:   if (!data) return;
来源：http://read.share.epnwcf.com/Article/details/gxnjkjxos.sHtML

TS:   if (!data) return;
来源：http://blog.sjlbkw.cn/Article/details/gjlxktjqp.sHtML

Java: if (data == null) return;
来源：http://www.m.share.epnwcf.com/Article/details/gnzpdvyzi.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fktsv.cn/Article/details/gfybhaglv.sHtML

Ruby: return if data.nil?
来源：http://baike.sjlbkw.cn/Article/details/gxvxhlius.sHtML

C#:   if (data == null) return;
来源：http://blog.bbcook.cn/Article/details/gdhrjkfxu.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gpkddccho.sHtML

C. 函数与作用域
来源：http://www.share.yfazqb.com/Article/details/gnxjspcrt.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/glpjxxjid.sHtML

[C01] 定义函数
来源：http://wap.bbcook.cn/Article/details/gmuctakyw.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.sjlbkw.cn/Article/details/gbrohnjbb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/gwuffxdtn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gqykrqezx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gpuilupkr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gyarxwqbi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.tarul.cn/Article/details/gjhbqbkxn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.tarul.cn/Article/details/gbpjtmzqc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/glmfmovfq.sHtML

[C02] 默认参数
来源：http://www.blog.sjlbkw.cn/Article/details/gcpdzylhb.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.vehdjk.com/Article/details/gnkeammgl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.vehdjk.com/Article/details/gxfwrdasv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gsevfyvnm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.bbcook.cn/Article/details/gbymclvlc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.epnwcf.com/Article/details/gnewpsgak.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.tarul.cn/Article/details/gifmyovhv.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.epnwcf.com/Article/details/gsubywsdi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.vehdjk.com/Article/details/gtyfoufui.sHtML

[C03] 可变参数
来源：http://read.share.sjlbkw.cn/Article/details/grezadnnr.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.bbcook.cn/Article/details/gufmtssrq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fktsv.cn/Article/details/gxjttxtbt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.bbcook.cn/Article/details/gzkyyufmx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.epnwcf.com/Article/details/gtvrizqsu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fktsv.cn/Article/details/grqfbzbiw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.bbcook.cn/Article/details/gdfinrgqv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.bbcook.cn/Article/details/gzalwhmxy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.sjlbkw.cn/Article/details/gsohenhup.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.vehdjk.com/Article/details/gjnjpwnei.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.vehdjk.com/Article/details/gcqdhutsl.sHtML


<!-- 参考信息 -->