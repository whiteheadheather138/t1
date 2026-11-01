代发 wailian999

Java: "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/gmjpwauqm.sHtML

Go:   "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gfqdcwrzr.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/gyxyltqin.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/gobrzyxym.sHtML

[A14] 注释写法
来源：http://mobile.tarul.cn/Article/details/gmurxtxsa.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.vehdjk.com/Article/details/gxasqenjq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.sjlbkw.cn/Article/details/gahijxkrt.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.bbcook.cn/Article/details/gvvtzgehg.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.epnwcf.com/Article/details/gzezrcfnf.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.bbcook.cn/Article/details/gejmjwmef.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.tarul.cn/Article/details/gxjxyzius.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.sjlbkw.cn/Article/details/gbgymrjha.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.epnwcf.com/Article/details/gjrtjmhux.sHtML

[A15] 空值判断与默认值
来源：http://www.share.tarul.cn/Article/details/gmvfizbmu.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.tarul.cn/Article/details/grabmgimg.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.fktsv.cn/Article/details/gkaioorlj.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.tarul.cn/Article/details/gtmqurvng.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.epnwcf.com/Article/details/gkipnjplw.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.vehdjk.com/Article/details/gxockzknd.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.yfazqb.com/Article/details/gxemnrhoc.sHtML

Ruby: value = data || "默认值"
来源：http://wap.vehdjk.com/Article/details/gregtxqmg.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.fktsv.cn/Article/details/gegzahyud.sHtML

[A16] 真假值判断规则
来源：http://blog.bbcook.cn/Article/details/glqajyicl.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.sjlbkw.cn/Article/details/gewkoxaga.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmdsrkea.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.yfazqb.com/Article/details/gnjaphayp.sHtML

TS:   if (!x) {}
来源：http://m.share.sjlbkw.cn/Article/details/ghsqglwmf.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.sjlbkw.cn/Article/details/gpureswak.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.vehdjk.com/Article/details/gsgjpohyi.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.bbcook.cn/Article/details/gubcvjbja.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fktsv.cn/Article/details/gozimnrcs.sHtML

[A17] 位运算
来源：http://3g.vehdjk.com/Article/details/gcdaqycbz.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/gfyduskpk.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.epnwcf.com/Article/details/gjtlhkgsb.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/gdcesxhzv.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/gyleioujl.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.yfazqb.com/Article/details/gmwjqwury.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.epnwcf.com/Article/details/gponpuzts.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fktsv.cn/Article/details/gjhlwknwm.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fktsv.cn/Article/details/gropjpdll.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.bbcook.cn/Article/details/gzpuirkxc.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.bbcook.cn/Article/details/gpwakvkpv.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.sjlbkw.cn/Article/details/gubxtjixe.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.sjlbkw.cn/Article/details/gszbvhnkq.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fktsv.cn/Article/details/ggewmciuk.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.tarul.cn/Article/details/gmbrdvlkm.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.sjlbkw.cn/Article/details/grhelilen.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.epnwcf.com/Article/details/gtvmzxvzx.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.sjlbkw.cn/Article/details/gwyoxczjn.sHtML

[A19] 交换两个变量
来源：http://www.m.share.epnwcf.com/Article/details/guuneildf.sHtML

Py:   a, b = b, a
来源：http://baike.tarul.cn/Article/details/gjzcanehu.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.yfazqb.com/Article/details/ggcwrpbpn.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.vehdjk.com/Article/details/gsccrfqei.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.sjlbkw.cn/Article/details/gddptutql.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.sjlbkw.cn/Article/details/gzmixjhji.sHtML

Go:   a, b = b, a
来源：http://read.share.yfazqb.com/Article/details/gfuvmkqmt.sHtML

Ruby: a, b = b, a
来源：http://3g.fktsv.cn/Article/details/gwftosesg.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.tarul.cn/Article/details/ghcnuugev.sHtML

[A20] 读取标准输入
来源：http://blog.fktsv.cn/Article/details/gyuizdcjw.sHtML

Py:   name = input("请输入：")
来源：http://wap.epnwcf.com/Article/details/gqqvgpmgz.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.vehdjk.com/Article/details/gsozxcyxz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.bbcook.cn/Article/details/gktrlidty.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.sjlbkw.cn/Article/details/gzmnzbary.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.vehdjk.com/Article/details/gvltqojbt.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwtuwdgw.sHtML

Ruby: gets.chomp
来源：http://blog.sjlbkw.cn/Article/details/gvxsrktxe.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.sjlbkw.cn/Article/details/gybyxuxca.sHtML

[A21] 保留指定小数位输出
来源：http://blog.fktsv.cn/Article/details/gjppiofph.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.vehdjk.com/Article/details/gwtaataij.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.yfazqb.com/Article/details/ghihxtnpl.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.tarul.cn/Article/details/gmfsmqojd.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.yfazqb.com/Article/details/gkywdwtyy.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.yfazqb.com/Article/details/gxmziikgl.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.epnwcf.com/Article/details/gpxadkfrg.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.fktsv.cn/Article/details/gkckgqgze.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.tarul.cn/Article/details/gydepsmwe.sHtML

[A22] 获取字符串长度
来源：http://mobile.tarul.cn/Article/details/gxzihclkq.sHtML

Py:   len(s)
来源：http://read.share.epnwcf.com/Article/details/gdjecpxhe.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.vehdjk.com/Article/details/gvatonefj.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.tarul.cn/Article/details/gzatzzgmk.sHtML

TS:   s.length
来源：http://www.share.vehdjk.com/Article/details/gxkpgacyl.sHtML

Java: s.length()
来源：http://mobile.epnwcf.com/Article/details/gmxkdvxje.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.fktsv.cn/Article/details/gyqromzyb.sHtML

Ruby: s.length
来源：http://baike.yfazqb.com/Article/details/giizwonoh.sHtML

C#:   s.Length
来源：http://www.blog.fktsv.cn/Article/details/grjuhknqk.sHtML

[A23] 大小写转换
来源：http://www.m.share.epnwcf.com/Article/details/gzpyrigme.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.epnwcf.com/Article/details/gymnhzwkv.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.sjlbkw.cn/Article/details/gwqgbxvlm.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvbndmfs.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.yfazqb.com/Article/details/gcwcmaszi.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.sjlbkw.cn/Article/details/gxenoomgg.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.tarul.cn/Article/details/gwjjxlawn.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.yfazqb.com/Article/details/gzflxgymp.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.yfazqb.com/Article/details/giukmtxuc.sHtML

[A24] 去除首尾空白
来源：http://mobile.fktsv.cn/Article/details/gycdqxnuh.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.fktsv.cn/Article/details/gcbkqjinl.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.fktsv.cn/Article/details/ggwimjrbk.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fktsv.cn/Article/details/gsokhgobc.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.bbcook.cn/Article/details/gflhfdjht.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.vehdjk.com/Article/details/gjuogjadl.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.bbcook.cn/Article/details/gfytcyboy.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.vehdjk.com/Article/details/ginsudbke.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.bbcook.cn/Article/details/gnaajiclz.sHtML

[A25] 字符串比较
来源：http://blog.fktsv.cn/Article/details/gqvyzdsok.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.vehdjk.com/Article/details/guqbedffs.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.tarul.cn/Article/details/gnnzbhdgk.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fktsv.cn/Article/details/gcatdtwmz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.sjlbkw.cn/Article/details/gkqomkueo.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.bbcook.cn/Article/details/gtdkmfjbt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.bbcook.cn/Article/details/gwsidtipo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.sjlbkw.cn/Article/details/ggpyeceac.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.sjlbkw.cn/Article/details/gedsvgixz.sHtML

[A26] 类型转换总览
来源：http://www.blog.epnwcf.com/Article/details/glwpmbpmb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.tarul.cn/Article/details/gijktdltz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.vehdjk.com/Article/details/gmlludgst.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.tarul.cn/Article/details/gbriqqxfl.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.vehdjk.com/Article/details/gkrsdvlxj.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.sjlbkw.cn/Article/details/gphhqwlvb.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.bbcook.cn/Article/details/gahrynnbk.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.vehdjk.com/Article/details/grdfapaog.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.bbcook.cn/Article/details/gzdkeytpf.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gnvprlhuu.sHtML

B. 流程控制
来源：http://read.share.epnwcf.com/Article/details/gidxqddvx.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gfpzzqbcn.sHtML

[B01] 条件判断 if / else
来源：http://www.share.epnwcf.com/Article/details/gfglalovj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.tarul.cn/Article/details/ggqsothhc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.sjlbkw.cn/Article/details/gduglwqzl.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fktsv.cn/Article/details/grkbqrvzr.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.vehdjk.com/Article/details/gognoawia.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.yfazqb.com/Article/details/gcickngpd.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.epnwcf.com/Article/details/gemxyboji.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.tarul.cn/Article/details/gjdygmbfp.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fktsv.cn/Article/details/gvmcvuued.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.tarul.cn/Article/details/gjprjhius.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.vehdjk.com/Article/details/gsogonfpo.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.tarul.cn/Article/details/giuoiqxsx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.tarul.cn/Article/details/gszqkblnu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/gopmzsjdr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/gwtnfavhk.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.tarul.cn/Article/details/gtxjyskmi.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.vehdjk.com/Article/details/giohuyhgm.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/goqdngabw.sHtML

[B03] switch / match / case
来源：http://blog.bbcook.cn/Article/details/gowxleplq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.tarul.cn/Article/details/goiexemvd.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/gogmmaxnp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fktsv.cn/Article/details/gwwialkzn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.tarul.cn/Article/details/gequvccza.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.tarul.cn/Article/details/guczhgfku.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.tarul.cn/Article/details/gvekoller.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.tarul.cn/Article/details/gpdofxmof.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.sjlbkw.cn/Article/details/ghoencbtd.sHtML

[B04] for 计数循环
来源：http://www.blog.fktsv.cn/Article/details/grmsahxuz.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.vehdjk.com/Article/details/gheghnmmu.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.vehdjk.com/Article/details/gjqvxjcna.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.yfazqb.com/Article/details/gziypjtgv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.sjlbkw.cn/Article/details/gjfvmgcih.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.yfazqb.com/Article/details/gdxbdgpdk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.yfazqb.com/Article/details/guuofwnme.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.bbcook.cn/Article/details/ghavccumn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.vehdjk.com/Article/details/gmxnsdwzt.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.vehdjk.com/Article/details/ghoaogzff.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fktsv.cn/Article/details/gxjstmwkf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.yfazqb.com/Article/details/gnebfvuwy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.yfazqb.com/Article/details/gfujhiqyh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.epnwcf.com/Article/details/grhekeqzj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.epnwcf.com/Article/details/guheukeii.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.tarul.cn/Article/details/godzdpgly.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.bbcook.cn/Article/details/ggpcckwgz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.epnwcf.com/Article/details/gnvqcfsoa.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.vehdjk.com/Article/details/gqqyynlqs.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.fktsv.cn/Article/details/gpfgunhpu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.sjlbkw.cn/Article/details/gpphzaoig.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.bbcook.cn/Article/details/gkphqymzz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fktsv.cn/Article/details/ggxhxepaz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.epnwcf.com/Article/details/gypuxuvtm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.fktsv.cn/Article/details/gqzmixxzh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.vehdjk.com/Article/details/gkghiblav.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.epnwcf.com/Article/details/gcbbnssyb.sHtML

[B07] while 循环
来源：http://www.m.share.yfazqb.com/Article/details/gckenqirt.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.yfazqb.com/Article/details/gvwprmthx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.sjlbkw.cn/Article/details/gjvdvnbxt.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gaucznjlu.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/gcxoflbzl.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/grvwzjmjw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.sjlbkw.cn/Article/details/gxcgonsnc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.epnwcf.com/Article/details/gdnjepwnb.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.tarul.cn/Article/details/gysqnrwkf.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.vehdjk.com/Article/details/gunwiikmw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.epnwcf.com/Article/details/gszufvlxv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.epnwcf.com/Article/details/gmjrvlbui.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/gfzetigvu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.vehdjk.com/Article/details/gzzigrtcs.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gurxlazyb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.bbcook.cn/Article/details/gyxvtxuhm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.vehdjk.com/Article/details/ggtxjyzzs.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/guhvxfgpi.sHtML

[B09] break 与 continue
来源：http://3g.bbcook.cn/Article/details/gjxjkrjbc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.sjlbkw.cn/Article/details/gfoxvjdcv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gtxczclbd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gfzkknhvu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/ghxjckshs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwlrmnrnm.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.tarul.cn/Article/details/gltjzjvux.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.bbcook.cn/Article/details/gsurhzhbi.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gxcvvinwe.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.epnwcf.com/Article/details/gftomskvk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.vehdjk.com/Article/details/gbbbosvha.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.sjlbkw.cn/Article/details/gcugxqegt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fktsv.cn/Article/details/gwkvwltdx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.yfazqb.com/Article/details/gbjtykwmp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fktsv.cn/Article/details/gbhxkckhu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.yfazqb.com/Article/details/gaosplzyf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.yfazqb.com/Article/details/gzbjglvnx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fktsv.cn/Article/details/gbwfvsvuf.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fktsv.cn/Article/details/gbrzpbyfa.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.epnwcf.com/Article/details/gthtcmphs.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.bbcook.cn/Article/details/gbjarhelq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.tarul.cn/Article/details/gxzriqpwz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.tarul.cn/Article/details/gzzwmylhs.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.yfazqb.com/Article/details/ghgzykqil.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fktsv.cn/Article/details/gvbvknomt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.yfazqb.com/Article/details/gislyekfi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.vehdjk.com/Article/details/gndcjqsvl.sHtML

[B12] 跳出多层循环
来源：http://www.blog.bbcook.cn/Article/details/gfpknnroz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.epnwcf.com/Article/details/gnovisgax.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.yfazqb.com/Article/details/gziebcdit.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.tarul.cn/Article/details/ggjyxffhq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/gqmoqflag.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.epnwcf.com/Article/details/gtezduwxu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fktsv.cn/Article/details/gjgjatpra.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.sjlbkw.cn/Article/details/gvefnuaze.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fktsv.cn/Article/details/glzinkexp.sHtML

[B13] 判断是否为数字
来源：http://www.blog.yfazqb.com/Article/details/gvvjsicdn.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.epnwcf.com/Article/details/gmocmnedn.sHtML

PHP:  is_numeric($x)
来源：http://wap.bbcook.cn/Article/details/glpvqfvvi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.bbcook.cn/Article/details/ggozsvmfb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fktsv.cn/Article/details/gpwpjzcia.sHtML

Java: x instanceof Number
来源：http://baike.fktsv.cn/Article/details/grymljnvf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.epnwcf.com/Article/details/grwjtmmaq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.tarul.cn/Article/details/gjdgcgmfy.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.sjlbkw.cn/Article/details/gpiovseab.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.sjlbkw.cn/Article/details/gclapiymy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.tarul.cn/Article/details/ghqduohay.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.tarul.cn/Article/details/gunhnljvs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.tarul.cn/Article/details/gwevebeex.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/gccerfvdr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.yfazqb.com/Article/details/gjjljimuh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.tarul.cn/Article/details/gtiuddnqx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/gxszntnau.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.yfazqb.com/Article/details/gjqqehcul.sHtML

[B15] 布尔运算与取反
来源：http://mobile.yfazqb.com/Article/details/gdlrvdycm.sHtML

Py:   a and b or not c
来源：http://baike.fktsv.cn/Article/details/gpbjyoear.sHtML

PHP:  $a && $b || !$c
来源：http://blog.epnwcf.com/Article/details/gepmuakqh.sHtML

JS:   a && b || !c
来源：http://baike.epnwcf.com/Article/details/glenixzfx.sHtML

TS:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gxxdvphrb.sHtML

Java: a && b || !c
来源：http://wap.epnwcf.com/Article/details/gvqgapbsz.sHtML

Go:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/glwvbmhlx.sHtML

Ruby: a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gfxwpejao.sHtML

C#:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/glmwxegew.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnnqiirw.sHtML

Py:   if not data: return
来源：http://www.blog.vehdjk.com/Article/details/gxgitqbwa.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.yfazqb.com/Article/details/gurrqdhzk.sHtML

JS:   if (!data) return;
来源：http://www.blog.bbcook.cn/Article/details/gykjeffyg.sHtML

TS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/gtguixtbo.sHtML

Java: if (data == null) return;
来源：http://www.blog.tarul.cn/Article/details/gbccyxiwn.sHtML

Go:   if data == nil { return }
来源：http://www.blog.yfazqb.com/Article/details/gmhxvqgmm.sHtML

Ruby: return if data.nil?
来源：http://blog.sjlbkw.cn/Article/details/gniinycbm.sHtML

C#:   if (data == null) return;
来源：http://wap.bbcook.cn/Article/details/gfmuhhjoh.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gwyetzxow.sHtML

C. 函数与作用域
来源：http://baike.vehdjk.com/Article/details/gqczjirql.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ggmouotqh.sHtML

[C01] 定义函数
来源：http://read.share.bbcook.cn/Article/details/gkzexzkqe.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.bbcook.cn/Article/details/gocjirgzk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gnmwwddyg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gzzcxbgtu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.tarul.cn/Article/details/ggqqlznrk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gjqnqqzwy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.vehdjk.com/Article/details/gvuuottsr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.epnwcf.com/Article/details/gljdnzvlh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gmgfwgqod.sHtML

[C02] 默认参数
来源：http://read.share.bbcook.cn/Article/details/guzhcjbwl.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.vehdjk.com/Article/details/gpqvtwtrn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fktsv.cn/Article/details/gfhhnvoir.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.epnwcf.com/Article/details/grazlwxrp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gpdkdogdr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.yfazqb.com/Article/details/giolowpcy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.epnwcf.com/Article/details/gavpcpbbc.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.bbcook.cn/Article/details/gwyhlilla.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fktsv.cn/Article/details/guwrrffvz.sHtML

[C03] 可变参数
来源：http://baike.sjlbkw.cn/Article/details/gwpeczvik.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.yfazqb.com/Article/details/gwvvnjlwx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.bbcook.cn/Article/details/ghnqnhsyq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fktsv.cn/Article/details/gkuoytcqz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.epnwcf.com/Article/details/gqtqomnzr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.tarul.cn/Article/details/gwbasswhs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.epnwcf.com/Article/details/gvetzxdsq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.yfazqb.com/Article/details/gclrqhbau.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.sjlbkw.cn/Article/details/gjcpvzdee.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.sjlbkw.cn/Article/details/gsmcaulva.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fktsv.cn/Article/details/gsvoinhmp.sHtML


<!-- 参考信息 -->