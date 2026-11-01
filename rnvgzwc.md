代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.blog.sjlbkw.cn/Article/details/ghxmdccxm.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/ghuvdoqlv.sHtML

JS:   "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gbhifdldp.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/gvohiqtla.sHtML

Java: "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/gphzkvwxr.sHtML

Go:   "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/giveuiiia.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.tarul.cn/Article/details/gwscggwrm.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/geosesvdp.sHtML

[A14] 注释写法
来源：http://blog.fktsv.cn/Article/details/gnukbejsm.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.epnwcf.com/Article/details/gxdfrwlhi.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.yfazqb.com/Article/details/gahqhridn.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.yfazqb.com/Article/details/gcdeqasrr.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.bbcook.cn/Article/details/gspzlooxu.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.vehdjk.com/Article/details/gruqjlqpu.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.sjlbkw.cn/Article/details/giaxkikft.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.sjlbkw.cn/Article/details/gybcduknj.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.yfazqb.com/Article/details/gdgjdludf.sHtML

[A15] 空值判断与默认值
来源：http://read.share.sjlbkw.cn/Article/details/gvvzlmvky.sHtML

Py:   value = data or "默认值"
来源：http://blog.sjlbkw.cn/Article/details/grklwjvwr.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.vehdjk.com/Article/details/grqpohyus.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.vehdjk.com/Article/details/gggrpttor.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.tarul.cn/Article/details/gupewbvml.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.epnwcf.com/Article/details/ghpymmjah.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.tarul.cn/Article/details/gssimhjji.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.epnwcf.com/Article/details/ghotjocbg.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.sjlbkw.cn/Article/details/goiqppdin.sHtML

[A16] 真假值判断规则
来源：http://mobile.tarul.cn/Article/details/grthymtsv.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.tarul.cn/Article/details/gypnfehie.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.vehdjk.com/Article/details/ggzkhrqla.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.vehdjk.com/Article/details/gtuuotghj.sHtML

TS:   if (!x) {}
来源：http://mobile.fktsv.cn/Article/details/gldiretjl.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.fktsv.cn/Article/details/gbiwftnct.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.bbcook.cn/Article/details/grkxtazxb.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.vehdjk.com/Article/details/goembipmq.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.epnwcf.com/Article/details/gvgqhbjyo.sHtML

[A17] 位运算
来源：http://baike.epnwcf.com/Article/details/gqfdigofb.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.vehdjk.com/Article/details/gjszwytjh.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/gykjtjrvp.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.tarul.cn/Article/details/gbxtsxrqb.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/grftpwono.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.tarul.cn/Article/details/gjnodtdyg.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/gqelttlco.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/gvbrvorzr.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.yfazqb.com/Article/details/gvzgibxxx.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.sjlbkw.cn/Article/details/gpjsaivdk.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.sjlbkw.cn/Article/details/gafqptefb.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.yfazqb.com/Article/details/gbrmawqjn.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.epnwcf.com/Article/details/gjhefahee.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.bbcook.cn/Article/details/gqvysdnzw.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.tarul.cn/Article/details/gdvwehizt.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.bbcook.cn/Article/details/gludszfts.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.vehdjk.com/Article/details/gzvnsedng.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.bbcook.cn/Article/details/gjhjhdipv.sHtML

[A19] 交换两个变量
来源：http://read.share.vehdjk.com/Article/details/gwnwryhnp.sHtML

Py:   a, b = b, a
来源：http://read.share.fktsv.cn/Article/details/gpjrzxcdv.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.tarul.cn/Article/details/gdntcehim.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.sjlbkw.cn/Article/details/gytbibdxr.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.yfazqb.com/Article/details/ghfodslcz.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.tarul.cn/Article/details/gpugwidms.sHtML

Go:   a, b = b, a
来源：http://3g.yfazqb.com/Article/details/gdpdzhieg.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.yfazqb.com/Article/details/gnlevsnje.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.epnwcf.com/Article/details/gefszpksh.sHtML

[A20] 读取标准输入
来源：http://blog.sjlbkw.cn/Article/details/gvugnmnjb.sHtML

Py:   name = input("请输入：")
来源：http://wap.vehdjk.com/Article/details/gedptzbzd.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.vehdjk.com/Article/details/gbrtpmjuj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.sjlbkw.cn/Article/details/gqexvhyuk.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.sjlbkw.cn/Article/details/gpxiixkhy.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.vehdjk.com/Article/details/gxqschhcf.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.fktsv.cn/Article/details/gxyjeafzk.sHtML

Ruby: gets.chomp
来源：http://m.share.vehdjk.com/Article/details/gsuftmrnj.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.vehdjk.com/Article/details/grsdjgrdu.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.bbcook.cn/Article/details/gkhbnqggo.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.tarul.cn/Article/details/gazjzcbdl.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.sjlbkw.cn/Article/details/gaxkroeoq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.sjlbkw.cn/Article/details/gttybanpb.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.fktsv.cn/Article/details/gguxgmxdi.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.epnwcf.com/Article/details/guxyfxppf.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.bbcook.cn/Article/details/gzlxkcnev.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.sjlbkw.cn/Article/details/gpguevefr.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.vehdjk.com/Article/details/gtazlqqxk.sHtML

[A22] 获取字符串长度
来源：http://www.blog.epnwcf.com/Article/details/ggpkbdcbs.sHtML

Py:   len(s)
来源：http://m.share.vehdjk.com/Article/details/gvbfddwnb.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.epnwcf.com/Article/details/golevcotq.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.fktsv.cn/Article/details/gvhrcmtcm.sHtML

TS:   s.length
来源：http://www.share.epnwcf.com/Article/details/ghpnqfruu.sHtML

Java: s.length()
来源：http://blog.sjlbkw.cn/Article/details/gmbeoelow.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.sjlbkw.cn/Article/details/gnxjmgbhs.sHtML

Ruby: s.length
来源：http://m.share.epnwcf.com/Article/details/gvbzahgcc.sHtML

C#:   s.Length
来源：http://wap.epnwcf.com/Article/details/guxbjqqnl.sHtML

[A23] 大小写转换
来源：http://www.blog.epnwcf.com/Article/details/gmywmcbxn.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.fktsv.cn/Article/details/ghidhbkup.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.yfazqb.com/Article/details/gmbwdqxen.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.vehdjk.com/Article/details/gwrepxpdb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.sjlbkw.cn/Article/details/gfoqfpvkl.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fktsv.cn/Article/details/gmledyxso.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.tarul.cn/Article/details/gvuaqaxtm.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.bbcook.cn/Article/details/gwxxgvuln.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.sjlbkw.cn/Article/details/gcyekrgke.sHtML

[A24] 去除首尾空白
来源：http://read.share.yfazqb.com/Article/details/gzzasccsq.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.bbcook.cn/Article/details/gnzcaykgd.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.vehdjk.com/Article/details/gvkptxmxp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.yfazqb.com/Article/details/ghtwraqgh.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.sjlbkw.cn/Article/details/gwnovuzzz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.sjlbkw.cn/Article/details/gxcexsqns.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.tarul.cn/Article/details/gpxyyzvzn.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.vehdjk.com/Article/details/gbnoglect.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gltfoaaar.sHtML

[A25] 字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/gwnfdtvno.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.bbcook.cn/Article/details/grcpfzukk.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.epnwcf.com/Article/details/gfiqcnmfu.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.epnwcf.com/Article/details/gvftmsnnh.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.vehdjk.com/Article/details/ghijszqrb.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.yfazqb.com/Article/details/gykabruxh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.tarul.cn/Article/details/geogxwjqj.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.tarul.cn/Article/details/gyyccfuas.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.fktsv.cn/Article/details/givanzwgb.sHtML

[A26] 类型转换总览
来源：http://mobile.vehdjk.com/Article/details/ghmpxgyaa.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.yfazqb.com/Article/details/gzvcijuow.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.sjlbkw.cn/Article/details/gnmvtlhyu.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.bbcook.cn/Article/details/gmyashhhg.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.sjlbkw.cn/Article/details/gytkbqhby.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.tarul.cn/Article/details/ghrricqzw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.sjlbkw.cn/Article/details/gvmemqapu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.sjlbkw.cn/Article/details/gwmdnkefp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.bbcook.cn/Article/details/gzrarleiv.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gnuiymuqp.sHtML

B. 流程控制
来源：http://mobile.tarul.cn/Article/details/ggxgztdjc.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ghksaqdrc.sHtML

[B01] 条件判断 if / else
来源：http://mobile.epnwcf.com/Article/details/gldlkgnnk.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.tarul.cn/Article/details/gzixmjgzi.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.epnwcf.com/Article/details/gbrjbvmce.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gnawpkcyk.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.vehdjk.com/Article/details/gomzqehxd.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.sjlbkw.cn/Article/details/gmzthhbbf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.tarul.cn/Article/details/gbyojnsxb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.fktsv.cn/Article/details/gnblkigff.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.bbcook.cn/Article/details/gjfmtvhlp.sHtML

[B02] 多分支 else if / elif
来源：http://3g.yfazqb.com/Article/details/gmhmvsgci.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.yfazqb.com/Article/details/gmmkochjp.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.bbcook.cn/Article/details/gcimyoffg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.bbcook.cn/Article/details/gwybhbboj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.epnwcf.com/Article/details/gexufckcb.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.bbcook.cn/Article/details/glftfpxax.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.sjlbkw.cn/Article/details/gxvhbatnm.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.fktsv.cn/Article/details/gcmxvtwkx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.bbcook.cn/Article/details/gkhfvlgcj.sHtML

[B03] switch / match / case
来源：http://wap.epnwcf.com/Article/details/gifcpphtp.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.vehdjk.com/Article/details/gphkwsavy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.yfazqb.com/Article/details/gxrqtqjph.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.tarul.cn/Article/details/gihcczxmk.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.bbcook.cn/Article/details/gbxapkyvt.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.sjlbkw.cn/Article/details/gifenerbp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.epnwcf.com/Article/details/glpwrpzui.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.epnwcf.com/Article/details/gypjiyuih.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.epnwcf.com/Article/details/gfwyddbht.sHtML

[B04] for 计数循环
来源：http://www.share.fktsv.cn/Article/details/gapmgsvdo.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.sjlbkw.cn/Article/details/gbjctzbpc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.epnwcf.com/Article/details/ggowwyeez.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.yfazqb.com/Article/details/gjhcldngw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.bbcook.cn/Article/details/gpbfsrqji.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.vehdjk.com/Article/details/gxcolwkrg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.sjlbkw.cn/Article/details/gpxxrnebt.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.sjlbkw.cn/Article/details/gljiwmwbu.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.tarul.cn/Article/details/gclcaxyix.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.sjlbkw.cn/Article/details/gpisjsdpi.sHtML

Py:   for item in arr: print(item)
来源：http://3g.tarul.cn/Article/details/gvakcxuzj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.sjlbkw.cn/Article/details/gbvoesapa.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.yfazqb.com/Article/details/glhrvbqwp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fktsv.cn/Article/details/gwrczptqj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.sjlbkw.cn/Article/details/gzqghcpwq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.epnwcf.com/Article/details/gjxbginbu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.yfazqb.com/Article/details/gkmuqrcsk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.epnwcf.com/Article/details/ghhjxhgmk.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.epnwcf.com/Article/details/gyqvoerqx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.bbcook.cn/Article/details/gupidkwbz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.yfazqb.com/Article/details/gupiypefx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.tarul.cn/Article/details/gjmsvhbfx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.bbcook.cn/Article/details/gisxwelem.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.yfazqb.com/Article/details/ghvfbshul.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.yfazqb.com/Article/details/ggspqytmq.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.vehdjk.com/Article/details/gnxmnrnmf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fktsv.cn/Article/details/gbkjlzxcn.sHtML

[B07] while 循环
来源：http://www.m.share.bbcook.cn/Article/details/grfpsyhtm.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.vehdjk.com/Article/details/gtepathpn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.tarul.cn/Article/details/gdbitpgdz.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/glnekefql.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fktsv.cn/Article/details/gjayekvxt.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fktsv.cn/Article/details/gudgtblqi.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.vehdjk.com/Article/details/gieqrgttk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.vehdjk.com/Article/details/gmtrssdbh.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.epnwcf.com/Article/details/glzcswyfn.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.tarul.cn/Article/details/ghpzoxwhd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.sjlbkw.cn/Article/details/gyrpboupe.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.epnwcf.com/Article/details/gfkxjczrp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.tarul.cn/Article/details/ggtqgrcdu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gnhqbjffy.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gfaripdlw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.yfazqb.com/Article/details/gihpawzvi.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fktsv.cn/Article/details/gxrqndyoq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/guwdfyleq.sHtML

[B09] break 与 continue
来源：http://m.share.epnwcf.com/Article/details/gdeydwviq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.yfazqb.com/Article/details/gvflyijek.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gnxnpaaxo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gbhmfovuo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/gqwyjzqww.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/gwtxdggev.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.bbcook.cn/Article/details/gpqgoofnr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.tarul.cn/Article/details/gmvxezeta.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/ggxxocrcb.sHtML

[B10] 遍历同时拿索引
来源：http://3g.sjlbkw.cn/Article/details/gtddcwtaa.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.yfazqb.com/Article/details/gvqwaadoh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.yfazqb.com/Article/details/gkttxonxa.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.tarul.cn/Article/details/gguffieei.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.tarul.cn/Article/details/gyilgjjnp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.sjlbkw.cn/Article/details/gzdbvjnvn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.sjlbkw.cn/Article/details/gjomafhui.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.tarul.cn/Article/details/gkifxlvfa.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.vehdjk.com/Article/details/gyrhdztka.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.tarul.cn/Article/details/gppjblgpm.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fktsv.cn/Article/details/ggydcased.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.yfazqb.com/Article/details/gsgzmofqn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.vehdjk.com/Article/details/gxjyiufaa.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fktsv.cn/Article/details/gmdewxmos.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.sjlbkw.cn/Article/details/grgodoypk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fktsv.cn/Article/details/gfoqrekdr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.sjlbkw.cn/Article/details/ggmewyvdx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.bbcook.cn/Article/details/gcgjjasus.sHtML

[B12] 跳出多层循环
来源：http://mobile.bbcook.cn/Article/details/gpazcegna.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.vehdjk.com/Article/details/gtcxehqae.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.epnwcf.com/Article/details/gregvdzdd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fktsv.cn/Article/details/gmchlxzdb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.sjlbkw.cn/Article/details/gllaltrsz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/gemcmcpzb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjklsnqi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fktsv.cn/Article/details/gtuojdmgx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.epnwcf.com/Article/details/grjntjbmx.sHtML

[B13] 判断是否为数字
来源：http://wap.tarul.cn/Article/details/gfrqcojey.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fktsv.cn/Article/details/gyiudpgbg.sHtML

PHP:  is_numeric($x)
来源：http://read.share.epnwcf.com/Article/details/geuadknph.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.vehdjk.com/Article/details/gnhaiwktu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.tarul.cn/Article/details/gnxrvlmqr.sHtML

Java: x instanceof Number
来源：http://www.blog.tarul.cn/Article/details/gcdtljfjh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.yfazqb.com/Article/details/gbdtitueo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.tarul.cn/Article/details/gspepgozj.sHtML

C#:   x is int or double or decimal
来源：http://mobile.bbcook.cn/Article/details/gahyihvad.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.sjlbkw.cn/Article/details/grthabawf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.bbcook.cn/Article/details/giwzvvjtc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.yfazqb.com/Article/details/ghbfzaybg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gmumhhxsp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gycjjallf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.bbcook.cn/Article/details/gslxlijae.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.sjlbkw.cn/Article/details/gtykoevqz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.yfazqb.com/Article/details/gnwuwaktk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/gzgudizij.sHtML

[B15] 布尔运算与取反
来源：http://mobile.vehdjk.com/Article/details/gduaehpgg.sHtML

Py:   a and b or not c
来源：http://blog.tarul.cn/Article/details/gwrvdvugz.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fktsv.cn/Article/details/gbzlckeox.sHtML

JS:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwfimjtp.sHtML

TS:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gbjdzrapi.sHtML

Java: a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gfxxvcwoa.sHtML

Go:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gdikrhbrm.sHtML

Ruby: a && b || !c
来源：http://baike.vehdjk.com/Article/details/ggmkqqhou.sHtML

C#:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gfxdvgqfi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.yfazqb.com/Article/details/gwcxnkajn.sHtML

Py:   if not data: return
来源：http://wap.fktsv.cn/Article/details/gstoaiqbe.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.bbcook.cn/Article/details/gcchmlnka.sHtML

JS:   if (!data) return;
来源：http://wap.yfazqb.com/Article/details/gzzxausqu.sHtML

TS:   if (!data) return;
来源：http://3g.vehdjk.com/Article/details/glxrpdgsv.sHtML

Java: if (data == null) return;
来源：http://mobile.fktsv.cn/Article/details/gexsnerlb.sHtML

Go:   if data == nil { return }
来源：http://3g.tarul.cn/Article/details/gkwiwlsox.sHtML

Ruby: return if data.nil?
来源：http://baike.sjlbkw.cn/Article/details/gbxtudmjd.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.yfazqb.com/Article/details/gxmludzbm.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/girtetflp.sHtML

C. 函数与作用域
来源：http://blog.fktsv.cn/Article/details/gslmcblic.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/giwvdoron.sHtML

[C01] 定义函数
来源：http://wap.vehdjk.com/Article/details/gjakxmepj.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.tarul.cn/Article/details/gbqdlgqpl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fktsv.cn/Article/details/gprpamdzk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gyqwejuck.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gcgwgdudi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gfebhhxjr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.bbcook.cn/Article/details/gjlrxqrcm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.bbcook.cn/Article/details/gowvwsroe.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gehzndxxl.sHtML

[C02] 默认参数
来源：http://mobile.vehdjk.com/Article/details/gxymoqeym.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fktsv.cn/Article/details/gyeygisqt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.yfazqb.com/Article/details/grudppkls.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.tarul.cn/Article/details/gevmcjpfy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.bbcook.cn/Article/details/glvcsjysb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.sjlbkw.cn/Article/details/gtpwyisca.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.vehdjk.com/Article/details/gstxcrkuq.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.yfazqb.com/Article/details/gfoekclnx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.tarul.cn/Article/details/gtxdailhk.sHtML

[C03] 可变参数
来源：http://www.blog.vehdjk.com/Article/details/gnafrmfuk.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.bbcook.cn/Article/details/glvccgtej.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.yfazqb.com/Article/details/guvusjdrx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.epnwcf.com/Article/details/gvsqsyetj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.yfazqb.com/Article/details/gnbzcgygq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.tarul.cn/Article/details/gdduwerfr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.tarul.cn/Article/details/gqfzzspcu.sHtML


<!-- 参考信息 -->