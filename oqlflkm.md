代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.epnwcf.com/Article/details/gtyjdutep.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.bbcook.cn/Article/details/godetfqqm.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.bbcook.cn/Article/details/gzhpvbzph.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.sjlbkw.cn/Article/details/gtngptyrb.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.epnwcf.com/Article/details/gammffrfr.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.tarul.cn/Article/details/gplctkxkz.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.fktsv.cn/Article/details/gbnzbjhrb.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.epnwcf.com/Article/details/gnbondiai.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.tarul.cn/Article/details/giaawthwx.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.epnwcf.com/Article/details/gfgoapfow.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.fktsv.cn/Article/details/gtxwrseae.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.yfazqb.com/Article/details/gnndpirhj.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.bbcook.cn/Article/details/gpdszrmlk.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/gvmshkjlj.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.tarul.cn/Article/details/gpbpvxoui.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/gpkhjdioy.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.epnwcf.com/Article/details/gfhatpdtl.sHtML

Go:   "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/guvqwifqx.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/gllrnwxen.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.tarul.cn/Article/details/gnlsuxtjx.sHtML

[A14] 注释写法
来源：http://3g.bbcook.cn/Article/details/giybjfuwg.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.vehdjk.com/Article/details/gsobbkksz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.bbcook.cn/Article/details/goqvfdkzt.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.sjlbkw.cn/Article/details/gslwbbfcq.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.sjlbkw.cn/Article/details/gbgduqjek.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.yfazqb.com/Article/details/ghqvqacvi.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.fktsv.cn/Article/details/gogdkijyi.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.fktsv.cn/Article/details/gbhskldfz.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.fktsv.cn/Article/details/gedivsbmc.sHtML

[A15] 空值判断与默认值
来源：http://blog.vehdjk.com/Article/details/gfifxjxgk.sHtML

Py:   value = data or "默认值"
来源：http://baike.tarul.cn/Article/details/gflllueau.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.fktsv.cn/Article/details/gaovmhpkt.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.bbcook.cn/Article/details/gcwusxubl.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.vehdjk.com/Article/details/gxozmcdrk.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.sjlbkw.cn/Article/details/gvjiqidfi.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.vehdjk.com/Article/details/gtgsverbs.sHtML

Ruby: value = data || "默认值"
来源：http://baike.yfazqb.com/Article/details/gwtkvbgru.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.tarul.cn/Article/details/gkiiuexjs.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.tarul.cn/Article/details/gtzdrpdch.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.yfazqb.com/Article/details/gprpkcgsy.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.yfazqb.com/Article/details/gtywkyqwt.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.bbcook.cn/Article/details/gsasazkun.sHtML

TS:   if (!x) {}
来源：http://m.share.bbcook.cn/Article/details/gxyepjkqu.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.fktsv.cn/Article/details/gowkiigjw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.bbcook.cn/Article/details/glhqmaezp.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.tarul.cn/Article/details/gezohgwlj.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.vehdjk.com/Article/details/gmtpehnxd.sHtML

[A17] 位运算
来源：http://www.blog.vehdjk.com/Article/details/grjthubsd.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/guysscdxy.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.tarul.cn/Article/details/gntzzxpsn.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/gccsnzkwl.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.epnwcf.com/Article/details/gbipjplws.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.yfazqb.com/Article/details/gznzpqsoh.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/giastpowo.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.sjlbkw.cn/Article/details/gkdwvhtjj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.epnwcf.com/Article/details/gwjljzggz.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.yfazqb.com/Article/details/gfvdvythf.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.yfazqb.com/Article/details/glbatwndn.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.bbcook.cn/Article/details/gxpsysijs.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.sjlbkw.cn/Article/details/gofkfdanj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.yfazqb.com/Article/details/gjwdetkgc.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.sjlbkw.cn/Article/details/gsuzlqigr.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.bbcook.cn/Article/details/gdpnhimwf.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.epnwcf.com/Article/details/gfuxjvewg.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.bbcook.cn/Article/details/ghptsexzt.sHtML

[A19] 交换两个变量
来源：http://blog.tarul.cn/Article/details/gwzqzcttb.sHtML

Py:   a, b = b, a
来源：http://www.blog.bbcook.cn/Article/details/ggpvlqzek.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.vehdjk.com/Article/details/gmwkaagsc.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmdqcyxj.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.vehdjk.com/Article/details/giuvaapyr.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.tarul.cn/Article/details/gsmsaxfqk.sHtML

Go:   a, b = b, a
来源：http://read.share.sjlbkw.cn/Article/details/gnfjyigaz.sHtML

Ruby: a, b = b, a
来源：http://wap.bbcook.cn/Article/details/gndctkvfp.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.vehdjk.com/Article/details/gidlrsudh.sHtML

[A20] 读取标准输入
来源：http://www.m.share.tarul.cn/Article/details/gbffidgok.sHtML

Py:   name = input("请输入：")
来源：http://baike.fktsv.cn/Article/details/ghziljawi.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.epnwcf.com/Article/details/gxrcsvrpq.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.fktsv.cn/Article/details/gckjkuunr.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.epnwcf.com/Article/details/gdhturqis.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.bbcook.cn/Article/details/gcpshwxzs.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.yfazqb.com/Article/details/ghhmhkbbp.sHtML

Ruby: gets.chomp
来源：http://read.share.sjlbkw.cn/Article/details/gdceoykyj.sHtML

C#:   Console.ReadLine();
来源：http://wap.sjlbkw.cn/Article/details/gztusfnzt.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.sjlbkw.cn/Article/details/gbazxmzby.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.epnwcf.com/Article/details/gsuowhgtz.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.yfazqb.com/Article/details/gbsxskaxt.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhwzogfs.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.sjlbkw.cn/Article/details/gchqkuuut.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.sjlbkw.cn/Article/details/gnbzmrezm.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.vehdjk.com/Article/details/gizmrramk.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.vehdjk.com/Article/details/gekawjrur.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.sjlbkw.cn/Article/details/gsbznmyaa.sHtML

[A22] 获取字符串长度
来源：http://baike.yfazqb.com/Article/details/ggneorkhv.sHtML

Py:   len(s)
来源：http://www.m.share.bbcook.cn/Article/details/gdtzejcoq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.tarul.cn/Article/details/grwyypoyg.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.yfazqb.com/Article/details/gbirlgbcy.sHtML

TS:   s.length
来源：http://blog.fktsv.cn/Article/details/gudbyszqa.sHtML

Java: s.length()
来源：http://read.share.sjlbkw.cn/Article/details/gqpbooqom.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.tarul.cn/Article/details/gwefgfdiz.sHtML

Ruby: s.length
来源：http://blog.vehdjk.com/Article/details/gmnqrjyvv.sHtML

C#:   s.Length
来源：http://mobile.bbcook.cn/Article/details/gkekegbgp.sHtML

[A23] 大小写转换
来源：http://www.blog.epnwcf.com/Article/details/gffrjdeef.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.sjlbkw.cn/Article/details/gqnqiwucc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.tarul.cn/Article/details/gcabgbjem.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.vehdjk.com/Article/details/giacmdbaz.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fktsv.cn/Article/details/gflsaigjb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.sjlbkw.cn/Article/details/gwagrypcg.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gifzltvkp.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.vehdjk.com/Article/details/gxfmnpxdd.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.vehdjk.com/Article/details/glayieozd.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.yfazqb.com/Article/details/guvqpzsms.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.bbcook.cn/Article/details/gmowztxtc.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.bbcook.cn/Article/details/gmpgmxkcc.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.yfazqb.com/Article/details/gjmlparrl.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fktsv.cn/Article/details/gxnrmwzdr.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.sjlbkw.cn/Article/details/gbrqirsxg.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.epnwcf.com/Article/details/gowprhfxr.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.epnwcf.com/Article/details/gqwkldjey.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.yfazqb.com/Article/details/grpbsbbla.sHtML

[A25] 字符串比较
来源：http://blog.tarul.cn/Article/details/gzgypockl.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.yfazqb.com/Article/details/gydotkfry.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.yfazqb.com/Article/details/gfjqaqgmw.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.yfazqb.com/Article/details/gscqzjexj.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gswitydhu.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.tarul.cn/Article/details/gjwgrevfv.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.yfazqb.com/Article/details/gnosdjbbf.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.epnwcf.com/Article/details/gjmmqioau.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.epnwcf.com/Article/details/gqbrenaax.sHtML

[A26] 类型转换总览
来源：http://www.share.vehdjk.com/Article/details/gdsyjlxur.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.vehdjk.com/Article/details/gdiwbddif.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.sjlbkw.cn/Article/details/gagrbxmzp.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.fktsv.cn/Article/details/ghfwiojhj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.yfazqb.com/Article/details/gpihfzqyj.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.yfazqb.com/Article/details/gdsdmbnhf.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.epnwcf.com/Article/details/ghzzihuhl.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.epnwcf.com/Article/details/gwhesihnl.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.epnwcf.com/Article/details/gkozzptqk.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gycnvzkfy.sHtML

B. 流程控制
来源：http://blog.sjlbkw.cn/Article/details/gpydgegqw.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gfmuwkazu.sHtML

[B01] 条件判断 if / else
来源：http://www.share.bbcook.cn/Article/details/goxwlgtil.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.yfazqb.com/Article/details/glatqpgzj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fktsv.cn/Article/details/gofgjtxul.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.sjlbkw.cn/Article/details/gfbdsjncg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/gynsqybja.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.tarul.cn/Article/details/gzrmxchtn.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.yfazqb.com/Article/details/gsybmknll.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fktsv.cn/Article/details/gitzzjskt.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/gvucaviwu.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.epnwcf.com/Article/details/gdfwgmisx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.epnwcf.com/Article/details/gsoaypkax.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.bbcook.cn/Article/details/geblzdjok.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.bbcook.cn/Article/details/ghwyccjep.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.tarul.cn/Article/details/gpbezmaqp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.bbcook.cn/Article/details/gutjqheup.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.vehdjk.com/Article/details/gkgiujfqs.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.epnwcf.com/Article/details/gdfjfsckz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.yfazqb.com/Article/details/gcporesuu.sHtML

[B03] switch / match / case
来源：http://www.share.tarul.cn/Article/details/gntojcbhg.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.bbcook.cn/Article/details/ggsnwwyce.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.bbcook.cn/Article/details/gexrmdgae.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.yfazqb.com/Article/details/gkxmotivv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fktsv.cn/Article/details/gohiujsjw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.bbcook.cn/Article/details/ghzhuktqd.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.yfazqb.com/Article/details/girqwtzqd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.vehdjk.com/Article/details/gongbdpqp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.yfazqb.com/Article/details/glkfxzgmn.sHtML

[B04] for 计数循环
来源：http://blog.vehdjk.com/Article/details/gfgvteooi.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.fktsv.cn/Article/details/gdcrqtqgl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.vehdjk.com/Article/details/gtjdszftc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.tarul.cn/Article/details/gxmdmahqj.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.tarul.cn/Article/details/gqacmopwb.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.epnwcf.com/Article/details/gzjgsskrp.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.bbcook.cn/Article/details/gbyjwqjky.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.yfazqb.com/Article/details/ggzfdlycg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.yfazqb.com/Article/details/gilfadkzi.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.tarul.cn/Article/details/gcmqdybsu.sHtML

Py:   for item in arr: print(item)
来源：http://blog.vehdjk.com/Article/details/gbltbthus.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.tarul.cn/Article/details/gnhclkvuv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.sjlbkw.cn/Article/details/ggbwhxite.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.epnwcf.com/Article/details/gyfjzjity.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.sjlbkw.cn/Article/details/gwjimjjie.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.yfazqb.com/Article/details/gngnbusjw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.vehdjk.com/Article/details/grfkzrfxm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.tarul.cn/Article/details/gtzxkytws.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.yfazqb.com/Article/details/gnrwhgcvt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fktsv.cn/Article/details/gvcbbwoya.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.sjlbkw.cn/Article/details/glruwhqdu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.tarul.cn/Article/details/gjeozbaew.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.sjlbkw.cn/Article/details/glbagbgzn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.vehdjk.com/Article/details/gqtegzywr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.vehdjk.com/Article/details/gxqiqfxwn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.yfazqb.com/Article/details/gnqvtfwoz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.epnwcf.com/Article/details/gegbgdpjc.sHtML

[B07] while 循环
来源：http://www.share.vehdjk.com/Article/details/gfzjbngrt.sHtML

Py:   while i < 10: i += 1
来源：http://3g.tarul.cn/Article/details/guvldptqj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.epnwcf.com/Article/details/gjantpnck.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.epnwcf.com/Article/details/gwhsvmlkk.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/gyumyxpmi.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/gpuspbwoe.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.yfazqb.com/Article/details/gsawqinln.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.sjlbkw.cn/Article/details/gotydedxu.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/gbsxftcou.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.epnwcf.com/Article/details/gahmeujyx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.tarul.cn/Article/details/gxibdzdmw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/gyvuibqcb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/gijxtsjqe.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/gwnalkvss.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/gasgqhoau.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.sjlbkw.cn/Article/details/gebxzjuub.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fktsv.cn/Article/details/gqxphaawn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gzptkqnab.sHtML

[B09] break 与 continue
来源：http://www.m.share.fktsv.cn/Article/details/gvazrjdov.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.sjlbkw.cn/Article/details/grooenvni.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.tarul.cn/Article/details/gjocylrpv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gxalbixsa.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gfptzsafe.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gyevrmpkq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.bbcook.cn/Article/details/gjjhesiai.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.epnwcf.com/Article/details/glkovzxlj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/gtiwnvqfb.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.tarul.cn/Article/details/gqcjpailv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fktsv.cn/Article/details/grgqcmxvg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.bbcook.cn/Article/details/gnpywfemf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.bbcook.cn/Article/details/gcmdxfzkh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.tarul.cn/Article/details/gxqrjqgvd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.vehdjk.com/Article/details/gnziqnpvn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.sjlbkw.cn/Article/details/gvzyfvwge.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fktsv.cn/Article/details/gmwlppboj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.yfazqb.com/Article/details/gyeeyymyj.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.yfazqb.com/Article/details/gwchjdwqz.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.tarul.cn/Article/details/gzujprpww.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.bbcook.cn/Article/details/glisnhkre.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.epnwcf.com/Article/details/gypeybxoi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.epnwcf.com/Article/details/gnghlvuap.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.tarul.cn/Article/details/gcvyjjjvb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.tarul.cn/Article/details/gmglujcwt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.yfazqb.com/Article/details/gmmyzhetd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.yfazqb.com/Article/details/guaeiztkw.sHtML

[B12] 跳出多层循环
来源：http://read.share.bbcook.cn/Article/details/gqyhodpqi.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.epnwcf.com/Article/details/gqzmtikdy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.vehdjk.com/Article/details/gxhlfksya.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.epnwcf.com/Article/details/gqvetcina.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.sjlbkw.cn/Article/details/gbjhtvhtp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.epnwcf.com/Article/details/gufdsbxqy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.sjlbkw.cn/Article/details/geidaecsv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.sjlbkw.cn/Article/details/gbfxiqrrk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.tarul.cn/Article/details/gufqywwmn.sHtML

[B13] 判断是否为数字
来源：http://3g.epnwcf.com/Article/details/gatjdhdno.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.yfazqb.com/Article/details/gefbeyfxa.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fktsv.cn/Article/details/ghoabcvit.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fktsv.cn/Article/details/gakjhjhbc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fktsv.cn/Article/details/gowtmlepp.sHtML

Java: x instanceof Number
来源：http://3g.bbcook.cn/Article/details/gkjzkbykh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.bbcook.cn/Article/details/ggrnlxrxi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.sjlbkw.cn/Article/details/gsxyxwsem.sHtML

C#:   x is int or double or decimal
来源：http://m.share.yfazqb.com/Article/details/gbtbkjyah.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.vehdjk.com/Article/details/gxlqdevye.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fktsv.cn/Article/details/gplmrrkjp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fktsv.cn/Article/details/gqcantrfj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/gtuntiyam.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gumdgdnyx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fktsv.cn/Article/details/geyjcwgxf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.vehdjk.com/Article/details/gtnlkdbxo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.epnwcf.com/Article/details/gsiabysak.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.epnwcf.com/Article/details/gzuwjlmwn.sHtML

[B15] 布尔运算与取反
来源：http://www.share.sjlbkw.cn/Article/details/gtvhclktg.sHtML

Py:   a and b or not c
来源：http://www.m.share.vehdjk.com/Article/details/gpoulkpkr.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.yfazqb.com/Article/details/gyabhbqkw.sHtML

JS:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gybrgwrzb.sHtML

TS:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/grwchcmhy.sHtML

Java: a && b || !c
来源：http://blog.yfazqb.com/Article/details/ghljinmjk.sHtML

Go:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/gyxkvhlow.sHtML

Ruby: a && b || !c
来源：http://wap.vehdjk.com/Article/details/girmbenxb.sHtML

C#:   a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/glekievgr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.tarul.cn/Article/details/gyetqptuu.sHtML

Py:   if not data: return
来源：http://www.share.sjlbkw.cn/Article/details/gcuxdspug.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.bbcook.cn/Article/details/gtzphoajl.sHtML

JS:   if (!data) return;
来源：http://blog.bbcook.cn/Article/details/gvkwjotvq.sHtML

TS:   if (!data) return;
来源：http://m.share.vehdjk.com/Article/details/gizihkkco.sHtML

Java: if (data == null) return;
来源：http://read.share.sjlbkw.cn/Article/details/glylkarpy.sHtML

Go:   if data == nil { return }
来源：http://read.share.tarul.cn/Article/details/gratozzzg.sHtML

Ruby: return if data.nil?
来源：http://www.blog.yfazqb.com/Article/details/gxskgmqwb.sHtML

C#:   if (data == null) return;
来源：http://mobile.tarul.cn/Article/details/gbpqaenrl.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gembjuhhu.sHtML

C. 函数与作用域
来源：http://m.share.tarul.cn/Article/details/gzlxcumne.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gexnqnsnp.sHtML

[C01] 定义函数
来源：http://wap.vehdjk.com/Article/details/gapcggkis.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.tarul.cn/Article/details/gnjjpfmko.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.tarul.cn/Article/details/ghssbsbvs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gtldmtwdg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gxwizwzty.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/ggeorgmqr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.yfazqb.com/Article/details/gzmpfoiov.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.epnwcf.com/Article/details/gdeywpybn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gmtrceuro.sHtML

[C02] 默认参数
来源：http://www.blog.fktsv.cn/Article/details/gkauccwpx.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.yfazqb.com/Article/details/gradnugie.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.tarul.cn/Article/details/gabcwhkoa.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/gildvxgcd.sHtML


<!-- 参考信息 -->