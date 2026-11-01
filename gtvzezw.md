代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.vehdjk.com/Article/details/gtbbhfttr.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.yfazqb.com/Article/details/gvsgiglvk.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.bbcook.cn/Article/details/getbezsvm.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.epnwcf.com/Article/details/gnvworntt.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fktsv.cn/Article/details/gukpkiycf.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.bbcook.cn/Article/details/gvnnqcflg.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.epnwcf.com/Article/details/gztnlimwv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.fktsv.cn/Article/details/gzpcikjbf.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.fktsv.cn/Article/details/gpgbfsstb.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.yfazqb.com/Article/details/gtrnssvpr.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.sjlbkw.cn/Article/details/gmceokvcy.sHtML

TS:   "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/gbzmlxdrp.sHtML

Java: "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/gzjqnngdp.sHtML

Go:   "第一行\n第二行"
来源：http://3g.vehdjk.com/Article/details/gicyaypvl.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/gzlnosxud.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.epnwcf.com/Article/details/gnmctsvde.sHtML

[A14] 注释写法
来源：http://www.m.share.vehdjk.com/Article/details/gznrnjktv.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.bbcook.cn/Article/details/gxcxywtsj.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.sjlbkw.cn/Article/details/gwwtgkffc.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.vehdjk.com/Article/details/givpunlzc.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.vehdjk.com/Article/details/gjjbhrgeu.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.bbcook.cn/Article/details/gzqmqujka.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.bbcook.cn/Article/details/ggoqnzssk.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.bbcook.cn/Article/details/gnfxghpwf.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.sjlbkw.cn/Article/details/greqmctdb.sHtML

[A15] 空值判断与默认值
来源：http://3g.sjlbkw.cn/Article/details/ghezgmwmk.sHtML

Py:   value = data or "默认值"
来源：http://wap.epnwcf.com/Article/details/gvupmowyi.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.sjlbkw.cn/Article/details/gckpjjvrq.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.fktsv.cn/Article/details/gkjhnbvho.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.epnwcf.com/Article/details/gmiyvtzmy.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.epnwcf.com/Article/details/gppegambe.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.sjlbkw.cn/Article/details/gffwcbowo.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.vehdjk.com/Article/details/guqcoxhbd.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.yfazqb.com/Article/details/gyykkytux.sHtML

[A16] 真假值判断规则
来源：http://m.share.sjlbkw.cn/Article/details/gwbvbidsr.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.fktsv.cn/Article/details/grpdnincb.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.epnwcf.com/Article/details/ghqehczup.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.yfazqb.com/Article/details/gfiftuusd.sHtML

TS:   if (!x) {}
来源：http://m.share.tarul.cn/Article/details/gcbrvlauy.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.tarul.cn/Article/details/guzndctor.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.tarul.cn/Article/details/ggttacfrg.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.bbcook.cn/Article/details/gsclcdwwt.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.tarul.cn/Article/details/gzsvixyme.sHtML

[A17] 位运算
来源：http://www.m.share.epnwcf.com/Article/details/gqcfoizpm.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/ggrdwuyfr.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.epnwcf.com/Article/details/gpdcjibdv.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/gsfbocddw.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.epnwcf.com/Article/details/gwgtipwtj.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.bbcook.cn/Article/details/gyztpqfon.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.yfazqb.com/Article/details/gaxhhykgk.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fktsv.cn/Article/details/gngnzbkzz.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/gnbdjoqgi.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.fktsv.cn/Article/details/gktqizfzf.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.sjlbkw.cn/Article/details/gejgfvqjs.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.sjlbkw.cn/Article/details/gbuvgfokh.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.yfazqb.com/Article/details/giymllroy.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.tarul.cn/Article/details/glgrhxqww.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.tarul.cn/Article/details/guvuooeud.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.bbcook.cn/Article/details/ghnpfvqrv.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.yfazqb.com/Article/details/gwykhsxsq.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.fktsv.cn/Article/details/gizmnzhkk.sHtML

[A19] 交换两个变量
来源：http://mobile.bbcook.cn/Article/details/gnoafcqga.sHtML

Py:   a, b = b, a
来源：http://mobile.vehdjk.com/Article/details/gaicvchsm.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.bbcook.cn/Article/details/gkstqseao.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.epnwcf.com/Article/details/gmvfrgxqf.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.sjlbkw.cn/Article/details/gfnusvxni.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.fktsv.cn/Article/details/gfftwbgfg.sHtML

Go:   a, b = b, a
来源：http://www.blog.fktsv.cn/Article/details/gmcqircmd.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.sjlbkw.cn/Article/details/gumtkancn.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.epnwcf.com/Article/details/gahoayyln.sHtML

[A20] 读取标准输入
来源：http://3g.vehdjk.com/Article/details/gpiwfpiyp.sHtML

Py:   name = input("请输入：")
来源：http://read.share.bbcook.cn/Article/details/gjpacsscq.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.yfazqb.com/Article/details/gpwwyxrks.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.epnwcf.com/Article/details/gjkcpauvz.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.tarul.cn/Article/details/gzuicwzsd.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.epnwcf.com/Article/details/gwzugaery.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.bbcook.cn/Article/details/geeiwlvmd.sHtML

Ruby: gets.chomp
来源：http://www.blog.vehdjk.com/Article/details/gitfjdtnd.sHtML

C#:   Console.ReadLine();
来源：http://3g.epnwcf.com/Article/details/gdmlaplap.sHtML

[A21] 保留指定小数位输出
来源：http://wap.yfazqb.com/Article/details/gpknhndle.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.sjlbkw.cn/Article/details/gqijswxmm.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.fktsv.cn/Article/details/ghdzjtjnl.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.tarul.cn/Article/details/gfcbjtkgr.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.tarul.cn/Article/details/guagaddrc.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.fktsv.cn/Article/details/gjdqklmne.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.bbcook.cn/Article/details/gemzqyask.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnnbdeak.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.tarul.cn/Article/details/gpzymnudl.sHtML

[A22] 获取字符串长度
来源：http://blog.yfazqb.com/Article/details/gnwvkunet.sHtML

Py:   len(s)
来源：http://www.share.vehdjk.com/Article/details/gzyjnkxzi.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.bbcook.cn/Article/details/gezjxwmfq.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.yfazqb.com/Article/details/gscgpvoxx.sHtML

TS:   s.length
来源：http://wap.vehdjk.com/Article/details/ggizalaeq.sHtML

Java: s.length()
来源：http://www.share.tarul.cn/Article/details/gqdejjsnz.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.tarul.cn/Article/details/gapklndqj.sHtML

Ruby: s.length
来源：http://m.share.vehdjk.com/Article/details/gxmfsultu.sHtML

C#:   s.Length
来源：http://m.share.sjlbkw.cn/Article/details/gfrkrhbib.sHtML

[A23] 大小写转换
来源：http://3g.epnwcf.com/Article/details/gotvruybf.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.yfazqb.com/Article/details/gpdipqflb.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.yfazqb.com/Article/details/gdwqviswv.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fktsv.cn/Article/details/gdekftlqs.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fktsv.cn/Article/details/gfrgiwanf.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.sjlbkw.cn/Article/details/gzfombldk.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.fktsv.cn/Article/details/gscrhzxas.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.fktsv.cn/Article/details/ggqdqzicj.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.yfazqb.com/Article/details/gpwzipzfx.sHtML

[A24] 去除首尾空白
来源：http://wap.bbcook.cn/Article/details/gxczaodwc.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.yfazqb.com/Article/details/gtpfiziqj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.sjlbkw.cn/Article/details/gbabuhfbk.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.vehdjk.com/Article/details/gyimfurux.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.vehdjk.com/Article/details/gzrdqtpop.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.yfazqb.com/Article/details/goakraeyl.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.bbcook.cn/Article/details/grzcefnjg.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.bbcook.cn/Article/details/gzqzyausv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.yfazqb.com/Article/details/gsrltvrnd.sHtML

[A25] 字符串比较
来源：http://mobile.vehdjk.com/Article/details/gkjbktcjk.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.vehdjk.com/Article/details/gsiwoehxp.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvvhcztg.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.vehdjk.com/Article/details/ghpkjlwyy.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fktsv.cn/Article/details/gnpxxmrpr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.bbcook.cn/Article/details/gvczcuzpd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.yfazqb.com/Article/details/gvaoplcor.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.vehdjk.com/Article/details/gjnrhmuso.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.fktsv.cn/Article/details/ggboyaiue.sHtML

[A26] 类型转换总览
来源：http://baike.tarul.cn/Article/details/gzmtvrjid.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.vehdjk.com/Article/details/gwidizejc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.vehdjk.com/Article/details/gpudvglal.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.tarul.cn/Article/details/gniamggta.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.fktsv.cn/Article/details/gwqqjmdwa.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.epnwcf.com/Article/details/gjtoggfoo.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.vehdjk.com/Article/details/gpsctyhqn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.tarul.cn/Article/details/gyavnrccx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fktsv.cn/Article/details/grazoiudd.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gbsxdlpvg.sHtML

B. 流程控制
来源：http://blog.fktsv.cn/Article/details/gssbopsfa.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gvpxjbhis.sHtML

[B01] 条件判断 if / else
来源：http://blog.vehdjk.com/Article/details/gleioftff.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.fktsv.cn/Article/details/gzlbjfcmb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.vehdjk.com/Article/details/gvplwbdsx.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.epnwcf.com/Article/details/giacztwyn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/gbenqthyo.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/geawaufsm.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.tarul.cn/Article/details/gkmpeioge.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.vehdjk.com/Article/details/gkpahwtgj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.epnwcf.com/Article/details/geoceobfj.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.sjlbkw.cn/Article/details/ghwisgnxs.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.tarul.cn/Article/details/gqobpddnc.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.yfazqb.com/Article/details/gilkpferq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.epnwcf.com/Article/details/gmohazmab.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fktsv.cn/Article/details/gmlwlkuvg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/gfdjtvkjb.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.vehdjk.com/Article/details/ggbnotspa.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.tarul.cn/Article/details/gfrhrgixy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fktsv.cn/Article/details/gxombetjd.sHtML

[B03] switch / match / case
来源：http://blog.bbcook.cn/Article/details/ggyiencsq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fktsv.cn/Article/details/guodctvqj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.yfazqb.com/Article/details/gxuoqvihl.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.vehdjk.com/Article/details/gdtspcvol.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.tarul.cn/Article/details/gdtnbkafj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.epnwcf.com/Article/details/ggyejaton.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.epnwcf.com/Article/details/gwvmyttxs.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.vehdjk.com/Article/details/geouneyez.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.epnwcf.com/Article/details/gfmhguooc.sHtML

[B04] for 计数循环
来源：http://blog.vehdjk.com/Article/details/gttkiwugu.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.yfazqb.com/Article/details/gzbthkbac.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.yfazqb.com/Article/details/gnosukdga.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fktsv.cn/Article/details/gcodojkmd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.sjlbkw.cn/Article/details/gjrkzatfi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.sjlbkw.cn/Article/details/glhyxevlx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.epnwcf.com/Article/details/gfcojwnzx.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.yfazqb.com/Article/details/govyliswu.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fktsv.cn/Article/details/gjtcbutpd.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.sjlbkw.cn/Article/details/gdrlqlmft.sHtML

Py:   for item in arr: print(item)
来源：http://baike.bbcook.cn/Article/details/grnewaxpp.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.epnwcf.com/Article/details/glyyytrsj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.yfazqb.com/Article/details/gcixknklb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.bbcook.cn/Article/details/gbdkrezjn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.vehdjk.com/Article/details/gfgzaphqq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.yfazqb.com/Article/details/gefopemaz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.epnwcf.com/Article/details/gzwzdxwwv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.sjlbkw.cn/Article/details/gqkjgjqwz.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.sjlbkw.cn/Article/details/gmfotnans.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.sjlbkw.cn/Article/details/gdewuxdox.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.epnwcf.com/Article/details/gjiklbget.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fktsv.cn/Article/details/gnekkohvu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.epnwcf.com/Article/details/gbbpcxbjl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.epnwcf.com/Article/details/gwvfvcwpg.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.epnwcf.com/Article/details/gopqmxrqk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fktsv.cn/Article/details/geuvyfrih.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.tarul.cn/Article/details/ghdkjpdan.sHtML

[B07] while 循环
来源：http://baike.vehdjk.com/Article/details/gorafkxrt.sHtML

Py:   while i < 10: i += 1
来源：http://3g.bbcook.cn/Article/details/gfnmtmqoi.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.epnwcf.com/Article/details/gaaklhvhm.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.vehdjk.com/Article/details/gooadznau.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/glmssvboi.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.tarul.cn/Article/details/gdrcmpqor.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.tarul.cn/Article/details/gmgijtqtw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.vehdjk.com/Article/details/gowowoyau.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/gcwduyrpa.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.tarul.cn/Article/details/gwumwlksv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.vehdjk.com/Article/details/ggaetsetw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.epnwcf.com/Article/details/gldvktitc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/gpsbuvzjk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gnadvmsrf.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/gtzojrurk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.epnwcf.com/Article/details/guriyavcp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.epnwcf.com/Article/details/glocfxgxi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/gzwpsoawb.sHtML

[B09] break 与 continue
来源：http://mobile.epnwcf.com/Article/details/gubkihelp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fktsv.cn/Article/details/ggjyguklc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.tarul.cn/Article/details/gousmizse.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gqdvtqpto.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/gkzdujlap.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gayvkikrk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.vehdjk.com/Article/details/gpzxfhrau.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.bbcook.cn/Article/details/gxzogsxgy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gyckcyoid.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fktsv.cn/Article/details/grczllwuh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.epnwcf.com/Article/details/gdyinpfeq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fktsv.cn/Article/details/gbdffwtug.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fktsv.cn/Article/details/gzgqkhmtc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.bbcook.cn/Article/details/giqexppku.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.tarul.cn/Article/details/gtnyarqfs.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.bbcook.cn/Article/details/gsroksjkg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fktsv.cn/Article/details/gvovzlzvs.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fktsv.cn/Article/details/grvwbhinx.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.vehdjk.com/Article/details/gqvlawywy.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fktsv.cn/Article/details/gjdhxbnxf.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.yfazqb.com/Article/details/gfsrmiqcq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.vehdjk.com/Article/details/gyhpbvsdy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.tarul.cn/Article/details/gbicoyiod.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fktsv.cn/Article/details/geegmxfpm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.epnwcf.com/Article/details/gwqytymud.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.sjlbkw.cn/Article/details/gpndemrhy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.sjlbkw.cn/Article/details/gctrpavis.sHtML

[B12] 跳出多层循环
来源：http://mobile.vehdjk.com/Article/details/glusmxhgd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.tarul.cn/Article/details/gbqnzakza.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fktsv.cn/Article/details/gvhnoexqm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/gfaauivxo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/gifuenscb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.sjlbkw.cn/Article/details/ggowlecex.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.bbcook.cn/Article/details/grcvlsamq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fktsv.cn/Article/details/gplcdcitk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.tarul.cn/Article/details/gmxhsplva.sHtML

[B13] 判断是否为数字
来源：http://www.share.epnwcf.com/Article/details/ganhxdwbe.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.yfazqb.com/Article/details/gmjhuusvb.sHtML

PHP:  is_numeric($x)
来源：http://mobile.tarul.cn/Article/details/gpiqufdkt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.bbcook.cn/Article/details/gksyriydw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.epnwcf.com/Article/details/gekglletr.sHtML

Java: x instanceof Number
来源：http://wap.fktsv.cn/Article/details/gwqrfugcp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.yfazqb.com/Article/details/gwjotwygz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.yfazqb.com/Article/details/gliuqvehq.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fktsv.cn/Article/details/gmwidbfwt.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fktsv.cn/Article/details/gxfqnsoey.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.tarul.cn/Article/details/gmyoharep.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.sjlbkw.cn/Article/details/gwfyjcjpy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gutvaiqyf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.epnwcf.com/Article/details/gnevdkvnn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.epnwcf.com/Article/details/gluudrtnc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.bbcook.cn/Article/details/gexwagkhc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.yfazqb.com/Article/details/ggejdoxxt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.vehdjk.com/Article/details/gjgmtlqwa.sHtML

[B15] 布尔运算与取反
来源：http://baike.epnwcf.com/Article/details/gvzvmcuoj.sHtML

Py:   a and b or not c
来源：http://read.share.epnwcf.com/Article/details/gkiuljlyc.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fktsv.cn/Article/details/gjbynkfso.sHtML

JS:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/gfqtbhbhk.sHtML

TS:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gzktlfpxd.sHtML

Java: a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gfuugiezh.sHtML

Go:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gimsqmyex.sHtML

Ruby: a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gfldlbqbk.sHtML

C#:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/gfbgshcrw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.tarul.cn/Article/details/gbynsmweh.sHtML

Py:   if not data: return
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhhkdvvs.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.tarul.cn/Article/details/gswkjqoko.sHtML

JS:   if (!data) return;
来源：http://read.share.yfazqb.com/Article/details/gxbxzceyc.sHtML

TS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/gmqkshclu.sHtML

Java: if (data == null) return;
来源：http://m.share.tarul.cn/Article/details/gohsjrbiy.sHtML

Go:   if data == nil { return }
来源：http://wap.epnwcf.com/Article/details/gkxaxkvww.sHtML

Ruby: return if data.nil?
来源：http://www.blog.bbcook.cn/Article/details/gmimvvvur.sHtML

C#:   if (data == null) return;
来源：http://blog.tarul.cn/Article/details/gzacogjfe.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gxcjqhjab.sHtML

C. 函数与作用域
来源：http://m.share.yfazqb.com/Article/details/gwkcfxlvg.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gdsumcpot.sHtML

[C01] 定义函数
来源：http://www.blog.epnwcf.com/Article/details/gwulqhbxd.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.epnwcf.com/Article/details/gvsbjtsgz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/ggeoizwpl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gqridymuv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwasvwmt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gpbryrlem.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.epnwcf.com/Article/details/gatklbfbo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.sjlbkw.cn/Article/details/gzgoglotd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/glqazhzwy.sHtML

[C02] 默认参数
来源：http://read.share.fktsv.cn/Article/details/glijqyjyb.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.sjlbkw.cn/Article/details/gboytnkzf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.tarul.cn/Article/details/gndvwqyrw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.tarul.cn/Article/details/gwhejqzyj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.tarul.cn/Article/details/gsthmolkc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fktsv.cn/Article/details/gewndijrd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.vehdjk.com/Article/details/gjijbhzkl.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.sjlbkw.cn/Article/details/gigwjhcym.sHtML


<!-- 参考信息 -->