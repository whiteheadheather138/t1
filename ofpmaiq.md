代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.vehdjk.com/Article/details/ghgkbrwwz.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.sjlbkw.cn/Article/details/gcdizvydr.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.bbcook.cn/Article/details/gsukfrfpx.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.vehdjk.com/Article/details/gcnobjnir.sHtML

Py:   "第一行\n第二行"
来源：http://wap.vehdjk.com/Article/details/gkdagzqvm.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/gmvtjahlo.sHtML

JS:   "第一行\n第二行"
来源：http://3g.fktsv.cn/Article/details/gnjefztyu.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/ghypczgtd.sHtML

Java: "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/gmztnccew.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/gynwiybvy.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.epnwcf.com/Article/details/gzapdxhrm.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gzrmycsgq.sHtML

[A14] 注释写法
来源：http://read.share.yfazqb.com/Article/details/gnxopgjzw.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.sjlbkw.cn/Article/details/gyrxmjpgn.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.sjlbkw.cn/Article/details/gvwqoruzt.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.bbcook.cn/Article/details/glrbvmfob.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.bbcook.cn/Article/details/gfpvkyqfh.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.tarul.cn/Article/details/gpjnrgdfo.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.yfazqb.com/Article/details/gmljteqbo.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.yfazqb.com/Article/details/gcxauyxov.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.fktsv.cn/Article/details/gjrsotymi.sHtML

[A15] 空值判断与默认值
来源：http://www.share.fktsv.cn/Article/details/glikyzkbr.sHtML

Py:   value = data or "默认值"
来源：http://mobile.vehdjk.com/Article/details/gcsivxamt.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.fktsv.cn/Article/details/gopgslhwc.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.tarul.cn/Article/details/guqgktzha.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.fktsv.cn/Article/details/gayxwazvh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.epnwcf.com/Article/details/gleqsahgg.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.sjlbkw.cn/Article/details/gofzwlaoe.sHtML

Ruby: value = data || "默认值"
来源：http://wap.vehdjk.com/Article/details/gqdjbkicy.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.fktsv.cn/Article/details/gsqhmiyie.sHtML

[A16] 真假值判断规则
来源：http://3g.vehdjk.com/Article/details/gyyocwzvw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.sjlbkw.cn/Article/details/gzukwmuoc.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.epnwcf.com/Article/details/gljfnaqjy.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.tarul.cn/Article/details/gxvwoqdzx.sHtML

TS:   if (!x) {}
来源：http://mobile.epnwcf.com/Article/details/glwnboooz.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.fktsv.cn/Article/details/gyxnwaxsq.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.tarul.cn/Article/details/gcckylmcj.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.vehdjk.com/Article/details/grcqtieom.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/guytfajzg.sHtML

[A17] 位运算
来源：http://www.blog.yfazqb.com/Article/details/gjmldento.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.yfazqb.com/Article/details/gwwzqjwni.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.tarul.cn/Article/details/ggjabalhc.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/giigecapl.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.tarul.cn/Article/details/gsszielnz.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.bbcook.cn/Article/details/guaaruorf.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.fktsv.cn/Article/details/gnnryghgo.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/gyfgtpine.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/gilxvyqir.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.tarul.cn/Article/details/gupgguirm.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fktsv.cn/Article/details/gbdagnrdk.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.tarul.cn/Article/details/gswxhmyjr.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fktsv.cn/Article/details/gtzbgmlpb.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.sjlbkw.cn/Article/details/gwpskkmpp.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.vehdjk.com/Article/details/gzdtpptpl.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.bbcook.cn/Article/details/gbqsxjqbc.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.sjlbkw.cn/Article/details/gufxdmham.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.fktsv.cn/Article/details/gnzosxvyp.sHtML

[A19] 交换两个变量
来源：http://mobile.tarul.cn/Article/details/gkmqacuah.sHtML

Py:   a, b = b, a
来源：http://mobile.vehdjk.com/Article/details/glnooemeg.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.sjlbkw.cn/Article/details/goboxrpki.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.bbcook.cn/Article/details/gixmjyrox.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.yfazqb.com/Article/details/gwptenfjg.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.yfazqb.com/Article/details/gkapprpil.sHtML

Go:   a, b = b, a
来源：http://3g.sjlbkw.cn/Article/details/gjcglqnlw.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.sjlbkw.cn/Article/details/glcitxfiu.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.epnwcf.com/Article/details/gabhtmgrv.sHtML

[A20] 读取标准输入
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdddhdzb.sHtML

Py:   name = input("请输入：")
来源：http://mobile.tarul.cn/Article/details/gdafzhvrb.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.bbcook.cn/Article/details/ghzkmlkyx.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.tarul.cn/Article/details/glgixmsqk.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.bbcook.cn/Article/details/gsgpqmumf.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.epnwcf.com/Article/details/gelaebhat.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.vehdjk.com/Article/details/gjvqqjhou.sHtML

Ruby: gets.chomp
来源：http://wap.vehdjk.com/Article/details/gjshmwqid.sHtML

C#:   Console.ReadLine();
来源：http://blog.bbcook.cn/Article/details/gramuhawo.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.fktsv.cn/Article/details/gjdizhztq.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.epnwcf.com/Article/details/gemerrsxs.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.vehdjk.com/Article/details/gxahbdrdo.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.vehdjk.com/Article/details/gapxgtwfo.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.yfazqb.com/Article/details/gplecitbu.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.fktsv.cn/Article/details/gzqeifpyf.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.bbcook.cn/Article/details/giblzbzur.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.bbcook.cn/Article/details/gtbnbrmwh.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.vehdjk.com/Article/details/gbhndvthr.sHtML

[A22] 获取字符串长度
来源：http://m.share.yfazqb.com/Article/details/gpwlnnbwh.sHtML

Py:   len(s)
来源：http://baike.yfazqb.com/Article/details/gtexmanvn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.bbcook.cn/Article/details/gvhumhpzd.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.epnwcf.com/Article/details/gcvdrrvry.sHtML

TS:   s.length
来源：http://wap.fktsv.cn/Article/details/gcymgmrlp.sHtML

Java: s.length()
来源：http://www.m.share.fktsv.cn/Article/details/gtrurbfku.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.vehdjk.com/Article/details/gvundqbhk.sHtML

Ruby: s.length
来源：http://mobile.epnwcf.com/Article/details/ghhzlyfig.sHtML

C#:   s.Length
来源：http://mobile.bbcook.cn/Article/details/gwciallan.sHtML

[A23] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gkszvbgro.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.tarul.cn/Article/details/gtengbebt.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.epnwcf.com/Article/details/gxeogjmgj.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.vehdjk.com/Article/details/gjzhuevcf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.vehdjk.com/Article/details/gdczlvtnr.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.tarul.cn/Article/details/gedftsrgc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.epnwcf.com/Article/details/gnwabkzom.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.yfazqb.com/Article/details/gieotaytz.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.epnwcf.com/Article/details/gwnmefuxz.sHtML

[A24] 去除首尾空白
来源：http://wap.sjlbkw.cn/Article/details/gkqydewnr.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.tarul.cn/Article/details/gqkbrkgwc.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.fktsv.cn/Article/details/gahdnavtm.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.bbcook.cn/Article/details/gpsxhlcto.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.yfazqb.com/Article/details/gvzrjnhgt.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.bbcook.cn/Article/details/gtuxegjks.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.bbcook.cn/Article/details/glngpyjdl.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.tarul.cn/Article/details/gnyvsuokf.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.sjlbkw.cn/Article/details/gmrwtdqpa.sHtML

[A25] 字符串比较
来源：http://read.share.yfazqb.com/Article/details/gtslolatj.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.epnwcf.com/Article/details/gagnvbfhn.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.tarul.cn/Article/details/gkxgxywau.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.epnwcf.com/Article/details/gmbairmkg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.sjlbkw.cn/Article/details/gffpvhzad.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.sjlbkw.cn/Article/details/gopkeufyh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.yfazqb.com/Article/details/gycdhbryq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.tarul.cn/Article/details/gtopzyoip.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.tarul.cn/Article/details/gmqedevfb.sHtML

[A26] 类型转换总览
来源：http://www.m.share.fktsv.cn/Article/details/ggxegipqy.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.sjlbkw.cn/Article/details/gmbdcinkv.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.vehdjk.com/Article/details/gdjtmldli.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.epnwcf.com/Article/details/gkjzwlyot.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.sjlbkw.cn/Article/details/gvlvuxjwr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.tarul.cn/Article/details/gtizhzlqw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.bbcook.cn/Article/details/gxjslxyuy.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.fktsv.cn/Article/details/gstfjoaou.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.epnwcf.com/Article/details/gppbhqxpr.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gqnsurkce.sHtML

B. 流程控制
来源：http://www.blog.sjlbkw.cn/Article/details/gihwfvudh.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gybevtwfb.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fktsv.cn/Article/details/gkpltpnfq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.sjlbkw.cn/Article/details/gxhlxhstb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.epnwcf.com/Article/details/ghuxmxuqq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.sjlbkw.cn/Article/details/gwucndngs.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.sjlbkw.cn/Article/details/gfjcmdiqj.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.fktsv.cn/Article/details/gaeoykrat.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.bbcook.cn/Article/details/grhuwweny.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.yfazqb.com/Article/details/ghwqrdlft.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.vehdjk.com/Article/details/gqshffjpm.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.tarul.cn/Article/details/gdurahgsd.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.tarul.cn/Article/details/gcvxrbesz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.yfazqb.com/Article/details/gyjbbmpis.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/gqoeurmot.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.tarul.cn/Article/details/gbaizgbyn.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/gqtbowtdf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.bbcook.cn/Article/details/gkrfuyotz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.sjlbkw.cn/Article/details/gxsgusfzk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.epnwcf.com/Article/details/gihnqixcs.sHtML

[B03] switch / match / case
来源：http://mobile.tarul.cn/Article/details/gefhufira.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.bbcook.cn/Article/details/gtgvzmrrc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.fktsv.cn/Article/details/gjnwkqvte.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.yfazqb.com/Article/details/gssbcamux.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/glerslsyz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fktsv.cn/Article/details/gkgxqavyk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.yfazqb.com/Article/details/gpboyzkeq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.bbcook.cn/Article/details/gtwzawilr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.vehdjk.com/Article/details/geucmanno.sHtML

[B04] for 计数循环
来源：http://read.share.bbcook.cn/Article/details/gqlahnbhq.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.vehdjk.com/Article/details/gwclfrurm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.yfazqb.com/Article/details/gcntgbyre.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fktsv.cn/Article/details/gpwhmlsxa.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fktsv.cn/Article/details/geqotyjkm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.bbcook.cn/Article/details/glqjouiub.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.sjlbkw.cn/Article/details/grrnsagmb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.sjlbkw.cn/Article/details/gtvdqzvzr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.fktsv.cn/Article/details/gjmpwvdje.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fktsv.cn/Article/details/gvdiyxtvh.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.sjlbkw.cn/Article/details/gglduebrw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.vehdjk.com/Article/details/grjesqnin.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkokelfay.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.bbcook.cn/Article/details/gvawokmdf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fktsv.cn/Article/details/ghphmjzdk.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.epnwcf.com/Article/details/gxborycvh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.fktsv.cn/Article/details/gslnzhzri.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkiovbeep.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.sjlbkw.cn/Article/details/gmtlfhdjb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.tarul.cn/Article/details/gtifoyxxs.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.vehdjk.com/Article/details/gyapqnntl.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.yfazqb.com/Article/details/glsinzjai.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.sjlbkw.cn/Article/details/ggflhlshv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.vehdjk.com/Article/details/gktvgqcas.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.tarul.cn/Article/details/ghrlxomph.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fktsv.cn/Article/details/gmqlmyhze.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.tarul.cn/Article/details/gpgfrnqez.sHtML

[B07] while 循环
来源：http://3g.fktsv.cn/Article/details/gdwrbtyge.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.bbcook.cn/Article/details/gzqyjbwui.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fktsv.cn/Article/details/gwkddgzwp.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/gwklpdlaf.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.yfazqb.com/Article/details/gukrpefpb.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/gqprmtyjk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.epnwcf.com/Article/details/gyzhwxpgq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.yfazqb.com/Article/details/gdofyqjzx.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.yfazqb.com/Article/details/gronhyjfe.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.tarul.cn/Article/details/giqweptng.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.fktsv.cn/Article/details/gffimofiy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.vehdjk.com/Article/details/gcxprkbhk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gjdadjvyg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/ggyzqhbcr.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/gnryxwkcd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fktsv.cn/Article/details/gqvitlicr.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.epnwcf.com/Article/details/garxkyaxk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/gkpxvflam.sHtML

[B09] break 与 continue
来源：http://mobile.fktsv.cn/Article/details/gpnaweiuf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.vehdjk.com/Article/details/ggakzeyxf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gposuwmqc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/grdagkkjk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/gkzntxsls.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/grrrsgoaz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fktsv.cn/Article/details/gehhucrov.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.bbcook.cn/Article/details/gmklmqxzx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gpkbqpgrx.sHtML

[B10] 遍历同时拿索引
来源：http://baike.tarul.cn/Article/details/gmjrafwpr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fktsv.cn/Article/details/gyarzcfre.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.vehdjk.com/Article/details/ghqpxuvmr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.yfazqb.com/Article/details/giozldbrr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.vehdjk.com/Article/details/gmyklzqas.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.bbcook.cn/Article/details/ggohjrbwz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.sjlbkw.cn/Article/details/guwwaqdmh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fktsv.cn/Article/details/gruktmwcy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.bbcook.cn/Article/details/gpqqufezf.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.vehdjk.com/Article/details/grwmltzsq.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.tarul.cn/Article/details/gcvnyxdfr.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.vehdjk.com/Article/details/gdybfrffj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.epnwcf.com/Article/details/gikobupsh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.sjlbkw.cn/Article/details/gsarpqgqw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fktsv.cn/Article/details/gosdeqsvj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.epnwcf.com/Article/details/gsxjhfbwj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.yfazqb.com/Article/details/gxwoyqcsg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.sjlbkw.cn/Article/details/gfrphthkc.sHtML

[B12] 跳出多层循环
来源：http://www.blog.bbcook.cn/Article/details/greofpfgm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.bbcook.cn/Article/details/gxjsemmto.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.sjlbkw.cn/Article/details/gdznvqgvo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/gofdxcpxx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gfpocildq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fktsv.cn/Article/details/gihujyncy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.sjlbkw.cn/Article/details/gdtmeutkp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.bbcook.cn/Article/details/gkjzmoiyo.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.sjlbkw.cn/Article/details/gnocxfrvy.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.epnwcf.com/Article/details/gpyzglcim.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.vehdjk.com/Article/details/gegvhprcf.sHtML

PHP:  is_numeric($x)
来源：http://3g.yfazqb.com/Article/details/gxzfehnnf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.yfazqb.com/Article/details/guvlewfjo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.yfazqb.com/Article/details/gpvykibux.sHtML

Java: x instanceof Number
来源：http://www.blog.fktsv.cn/Article/details/gxeshvewi.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.epnwcf.com/Article/details/grtujfmpd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.tarul.cn/Article/details/gksxoupyh.sHtML

C#:   x is int or double or decimal
来源：http://blog.yfazqb.com/Article/details/gkiercvtd.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.bbcook.cn/Article/details/gsqcswnkn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.yfazqb.com/Article/details/gwixtrkpg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fktsv.cn/Article/details/grzmrbqts.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.sjlbkw.cn/Article/details/gnvgfaikx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gubirwwzc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.vehdjk.com/Article/details/gzzgcakhg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.yfazqb.com/Article/details/glashxqmp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.epnwcf.com/Article/details/gshikdhdd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gmyndkdjw.sHtML

[B15] 布尔运算与取反
来源：http://mobile.epnwcf.com/Article/details/gxevyqdsl.sHtML

Py:   a and b or not c
来源：http://www.m.share.epnwcf.com/Article/details/gfqnvlmwz.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.vehdjk.com/Article/details/gorpkeatm.sHtML

JS:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/ggireydfc.sHtML

TS:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gwdumcsgk.sHtML

Java: a && b || !c
来源：http://wap.tarul.cn/Article/details/gqmzbtbaz.sHtML

Go:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gjnvubaqy.sHtML

Ruby: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gvjmehanq.sHtML

C#:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gvhvheiuz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.bbcook.cn/Article/details/gadjpxwoz.sHtML

Py:   if not data: return
来源：http://www.share.tarul.cn/Article/details/gbparfmmk.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.epnwcf.com/Article/details/gvqrulqmf.sHtML

JS:   if (!data) return;
来源：http://www.blog.fktsv.cn/Article/details/gvjlktowf.sHtML

TS:   if (!data) return;
来源：http://read.share.sjlbkw.cn/Article/details/gsjgkqumq.sHtML

Java: if (data == null) return;
来源：http://m.share.epnwcf.com/Article/details/gerynktoa.sHtML

Go:   if data == nil { return }
来源：http://3g.vehdjk.com/Article/details/gxuzqniuh.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.bbcook.cn/Article/details/gpwosbzks.sHtML

C#:   if (data == null) return;
来源：http://blog.tarul.cn/Article/details/gcuappfia.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gnnkiadrf.sHtML

C. 函数与作用域
来源：http://www.share.epnwcf.com/Article/details/ggxfbpzxg.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gnpjeugua.sHtML

[C01] 定义函数
来源：http://blog.tarul.cn/Article/details/gynvtxpte.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.epnwcf.com/Article/details/gdyyzlvkt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gmkboyzil.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gxpxxptlu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gprhvfoso.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gsehzydya.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fktsv.cn/Article/details/ggxiuddfi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.vehdjk.com/Article/details/gspgwjwks.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/geyrrrody.sHtML

[C02] 默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gfjyielqk.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.tarul.cn/Article/details/gbxlsnmbi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.yfazqb.com/Article/details/gqlizczea.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.yfazqb.com/Article/details/ggdtneiyd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.bbcook.cn/Article/details/gbuttgpss.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.bbcook.cn/Article/details/gyodbljcl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.yfazqb.com/Article/details/glhckjoef.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.tarul.cn/Article/details/gduekysbm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.sjlbkw.cn/Article/details/geubltbxk.sHtML

[C03] 可变参数
来源：http://wap.fktsv.cn/Article/details/gyqkxrkht.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.sjlbkw.cn/Article/details/gukalcdou.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.tarul.cn/Article/details/ggrktngmi.sHtML


<!-- 参考信息 -->