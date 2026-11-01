代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.sjlbkw.cn/Article/details/gynaqgrxs.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.fktsv.cn/Article/details/goupxdkcl.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.vehdjk.com/Article/details/gsxbbnnlm.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.yfazqb.com/Article/details/gmtharqpu.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.epnwcf.com/Article/details/govjispmg.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.sjlbkw.cn/Article/details/ggalpgjtu.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.bbcook.cn/Article/details/gwgvcedmd.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.vehdjk.com/Article/details/grgskvllv.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.epnwcf.com/Article/details/goqdybeqi.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/gvhccomaj.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/gwkhunhdb.sHtML

TS:   "第一行\n第二行"
来源：http://baike.yfazqb.com/Article/details/gpjuibvme.sHtML

Java: "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/goxnybcya.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.yfazqb.com/Article/details/gmvkoufcr.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.tarul.cn/Article/details/gceqqoafc.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gigtgfslq.sHtML

[A14] 注释写法
来源：http://www.blog.vehdjk.com/Article/details/gsiufeiem.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.bbcook.cn/Article/details/gvrdgnpav.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.tarul.cn/Article/details/gombcfnup.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.vehdjk.com/Article/details/goujmlpyt.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.vehdjk.com/Article/details/gtkegmaee.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.bbcook.cn/Article/details/gooqoncit.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fktsv.cn/Article/details/gaippeisd.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.epnwcf.com/Article/details/gpjfyowdi.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fktsv.cn/Article/details/gaunonjrh.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.epnwcf.com/Article/details/gsjycvdux.sHtML

Py:   value = data or "默认值"
来源：http://blog.sjlbkw.cn/Article/details/ginwcgwqn.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.sjlbkw.cn/Article/details/gawirbgwc.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.epnwcf.com/Article/details/gtklriynu.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.epnwcf.com/Article/details/gahttmnzc.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.epnwcf.com/Article/details/ghblvusdn.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.fktsv.cn/Article/details/gcmdtqdhs.sHtML

Ruby: value = data || "默认值"
来源：http://3g.fktsv.cn/Article/details/gewzxlxsq.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.bbcook.cn/Article/details/gyzootkks.sHtML

[A16] 真假值判断规则
来源：http://www.blog.vehdjk.com/Article/details/gbnbgxpuj.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.epnwcf.com/Article/details/gzmwcbmpw.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.epnwcf.com/Article/details/gzmgkeiao.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.tarul.cn/Article/details/gptjooqlv.sHtML

TS:   if (!x) {}
来源：http://baike.sjlbkw.cn/Article/details/gktwfkssz.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.yfazqb.com/Article/details/gnpiekulj.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.sjlbkw.cn/Article/details/gyfghfcfb.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.bbcook.cn/Article/details/gtakwwvgd.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.vehdjk.com/Article/details/gycmbkypn.sHtML

[A17] 位运算
来源：http://baike.vehdjk.com/Article/details/genoupptm.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/gqdqfykmv.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.vehdjk.com/Article/details/gwmsvumao.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.tarul.cn/Article/details/gthyvxlrs.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/glmdvpbjy.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/gqfpckdbf.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.vehdjk.com/Article/details/gkrzoqfkc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.yfazqb.com/Article/details/glkwhzyfn.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/gzboyxwty.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.fktsv.cn/Article/details/gorlfufzr.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.vehdjk.com/Article/details/gkhzkwaht.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.bbcook.cn/Article/details/ggioordac.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.sjlbkw.cn/Article/details/gkstxpdui.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.epnwcf.com/Article/details/gurzfernz.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.vehdjk.com/Article/details/gbqnxhlmk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.yfazqb.com/Article/details/gyvnddcza.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.tarul.cn/Article/details/grmelvvbv.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.bbcook.cn/Article/details/gsunaxmux.sHtML

[A19] 交换两个变量
来源：http://read.share.epnwcf.com/Article/details/gjgamgcrz.sHtML

Py:   a, b = b, a
来源：http://read.share.tarul.cn/Article/details/geahphttl.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.vehdjk.com/Article/details/gwtzzeciq.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.fktsv.cn/Article/details/gymyouged.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.fktsv.cn/Article/details/guabkxrku.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.vehdjk.com/Article/details/gautyqwcd.sHtML

Go:   a, b = b, a
来源：http://wap.bbcook.cn/Article/details/grmqegzfs.sHtML

Ruby: a, b = b, a
来源：http://mobile.epnwcf.com/Article/details/gfgdnifof.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.fktsv.cn/Article/details/gfdrlggjo.sHtML

[A20] 读取标准输入
来源：http://www.blog.vehdjk.com/Article/details/gewafukve.sHtML

Py:   name = input("请输入：")
来源：http://mobile.fktsv.cn/Article/details/gxopcbixe.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.fktsv.cn/Article/details/gtxiufldi.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.fktsv.cn/Article/details/gllnfvgmo.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.vehdjk.com/Article/details/gpixzctqt.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.tarul.cn/Article/details/gpekgrfum.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.yfazqb.com/Article/details/gzoxizxvi.sHtML

Ruby: gets.chomp
来源：http://m.share.fktsv.cn/Article/details/gvgnoigni.sHtML

C#:   Console.ReadLine();
来源：http://blog.tarul.cn/Article/details/gylbajcol.sHtML

[A21] 保留指定小数位输出
来源：http://baike.tarul.cn/Article/details/gcayfalru.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.fktsv.cn/Article/details/gingdcfvy.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gauxtpbkv.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.bbcook.cn/Article/details/ghiykcjup.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.epnwcf.com/Article/details/gvhxswlqv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.epnwcf.com/Article/details/gmcpgtjhh.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.yfazqb.com/Article/details/gpcfekksu.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.vehdjk.com/Article/details/gffutaxym.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.tarul.cn/Article/details/gbpoiajsa.sHtML

[A22] 获取字符串长度
来源：http://blog.fktsv.cn/Article/details/gmclngqed.sHtML

Py:   len(s)
来源：http://www.m.share.yfazqb.com/Article/details/gxjxyrsjz.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.epnwcf.com/Article/details/gcqrmjflc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.vehdjk.com/Article/details/ggncsuqfs.sHtML

TS:   s.length
来源：http://mobile.fktsv.cn/Article/details/gehybwdpv.sHtML

Java: s.length()
来源：http://m.share.bbcook.cn/Article/details/gvgvomyky.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.epnwcf.com/Article/details/gcdmtrpnd.sHtML

Ruby: s.length
来源：http://3g.bbcook.cn/Article/details/gxlrqudcy.sHtML

C#:   s.Length
来源：http://baike.fktsv.cn/Article/details/gziarkcgy.sHtML

[A23] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/gpoaoilpr.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.epnwcf.com/Article/details/gaihiejkl.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fktsv.cn/Article/details/gzolfyhbh.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.epnwcf.com/Article/details/gdgydfkwg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.sjlbkw.cn/Article/details/gfjmessuw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.epnwcf.com/Article/details/gczayiaom.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.fktsv.cn/Article/details/gfgxpwtua.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.vehdjk.com/Article/details/ghypdohdy.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.fktsv.cn/Article/details/ggavgoruk.sHtML

[A24] 去除首尾空白
来源：http://read.share.yfazqb.com/Article/details/gdlyshipv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.sjlbkw.cn/Article/details/ghgpxuvqm.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.fktsv.cn/Article/details/grfuddzbt.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.vehdjk.com/Article/details/gdhxyqxtg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.bbcook.cn/Article/details/gkhpxylof.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.yfazqb.com/Article/details/ghcatszev.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.vehdjk.com/Article/details/gdzkjmbek.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.vehdjk.com/Article/details/gkbzhmdzv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.sjlbkw.cn/Article/details/gdktpsiuq.sHtML

[A25] 字符串比较
来源：http://3g.vehdjk.com/Article/details/ggklztyib.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.bbcook.cn/Article/details/gkkcgwrwc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.epnwcf.com/Article/details/glivmkota.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.bbcook.cn/Article/details/gykrxzmeq.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.bbcook.cn/Article/details/gkldptrzu.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.yfazqb.com/Article/details/gzshinzbl.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.sjlbkw.cn/Article/details/gvfhodvvl.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.yfazqb.com/Article/details/gqkpkuyst.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.sjlbkw.cn/Article/details/gsipnxpqn.sHtML

[A26] 类型转换总览
来源：http://m.share.sjlbkw.cn/Article/details/gegtepgnc.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.fktsv.cn/Article/details/gfeyflugk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.yfazqb.com/Article/details/geppmzoin.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.vehdjk.com/Article/details/grnesiuai.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.yfazqb.com/Article/details/gbhopuobn.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.bbcook.cn/Article/details/gpygxvwra.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.tarul.cn/Article/details/gyprubdni.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.tarul.cn/Article/details/gggnhynwb.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.tarul.cn/Article/details/gmeaenrrm.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gmxvjmpxw.sHtML

B. 流程控制
来源：http://baike.sjlbkw.cn/Article/details/gjxhecsdv.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gijcihrky.sHtML

[B01] 条件判断 if / else
来源：http://www.share.sjlbkw.cn/Article/details/gmnsurxxi.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.bbcook.cn/Article/details/grhsmtdid.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.epnwcf.com/Article/details/gvaaccunm.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gbwoemusw.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/gdurkgzvh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.yfazqb.com/Article/details/gjlgqslae.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.vehdjk.com/Article/details/gnwzbgsld.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.bbcook.cn/Article/details/ginuaxxnm.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.fktsv.cn/Article/details/gudgrvpin.sHtML

[B02] 多分支 else if / elif
来源：http://blog.bbcook.cn/Article/details/gbszqgzvw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fktsv.cn/Article/details/gzrigihko.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.yfazqb.com/Article/details/grfigjdjg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.epnwcf.com/Article/details/gnccbnuac.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/gtcqafqjy.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.bbcook.cn/Article/details/gxicwsczh.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.sjlbkw.cn/Article/details/gplwjiyzi.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.tarul.cn/Article/details/gvwehyexl.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gszvqzqfg.sHtML

[B03] switch / match / case
来源：http://m.share.epnwcf.com/Article/details/gpauvqjwb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.tarul.cn/Article/details/gqufidoco.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gxpfmywsp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/glxqdivuu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.sjlbkw.cn/Article/details/girsrqzmv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.epnwcf.com/Article/details/gusydqvpz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.fktsv.cn/Article/details/gojhwxrid.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.yfazqb.com/Article/details/glagtveol.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.fktsv.cn/Article/details/gvqortjpc.sHtML

[B04] for 计数循环
来源：http://www.share.epnwcf.com/Article/details/gucdcnlqe.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.fktsv.cn/Article/details/gpbsztbix.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.tarul.cn/Article/details/gejjvpwgy.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.yfazqb.com/Article/details/grxrvylnk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fktsv.cn/Article/details/gknrvouve.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.bbcook.cn/Article/details/gacaeujbl.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.vehdjk.com/Article/details/ggkyksyos.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.tarul.cn/Article/details/gnubzgtfy.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.yfazqb.com/Article/details/guevvsvxm.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.yfazqb.com/Article/details/glurndoqy.sHtML

Py:   for item in arr: print(item)
来源：http://blog.sjlbkw.cn/Article/details/gibbdogcb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.epnwcf.com/Article/details/ghpnnktjy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.epnwcf.com/Article/details/gumshiicd.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.yfazqb.com/Article/details/gqrtdwmjv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.tarul.cn/Article/details/gkbevsjok.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fktsv.cn/Article/details/gtwtjsjfw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.sjlbkw.cn/Article/details/ggktwryic.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.fktsv.cn/Article/details/gxxkzhjzp.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.tarul.cn/Article/details/geplyhtid.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.sjlbkw.cn/Article/details/geqmkbxdp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.vehdjk.com/Article/details/gkcpgaeyk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.tarul.cn/Article/details/gxxhflzye.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.tarul.cn/Article/details/gzhrkziox.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.sjlbkw.cn/Article/details/gxwzmzrmc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.bbcook.cn/Article/details/ggpibwmks.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.yfazqb.com/Article/details/gzxzzfjgd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.bbcook.cn/Article/details/gkeespfhv.sHtML

[B07] while 循环
来源：http://www.share.fktsv.cn/Article/details/gsymhyyyc.sHtML

Py:   while i < 10: i += 1
来源：http://3g.vehdjk.com/Article/details/gxbyeinye.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.tarul.cn/Article/details/gnwtawzsx.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/gpnjefzbg.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/gswrdrvuo.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.yfazqb.com/Article/details/gthlvgakh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.epnwcf.com/Article/details/gmbbhxpvj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.yfazqb.com/Article/details/gfvhhgnie.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.yfazqb.com/Article/details/gqlcufiqg.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.tarul.cn/Article/details/gsvhlxsqs.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrumunqz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gspbxqxnx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gvhhxvntm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.vehdjk.com/Article/details/gjngvjamc.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/gmmrfsuao.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.sjlbkw.cn/Article/details/gkjhvlvun.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.bbcook.cn/Article/details/gagczwpin.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.vehdjk.com/Article/details/godtnktdz.sHtML

[B09] break 与 continue
来源：http://www.blog.bbcook.cn/Article/details/gyjjndzqw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.tarul.cn/Article/details/ggxgykpae.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gaskfuvsb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/ghkixqwks.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gzyffkdsa.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gxgadrzod.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fktsv.cn/Article/details/gkusylnbi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.sjlbkw.cn/Article/details/geopjhoey.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gsvjvnufd.sHtML

[B10] 遍历同时拿索引
来源：http://wap.vehdjk.com/Article/details/gikkvqsfp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.vehdjk.com/Article/details/gevthdnjx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.vehdjk.com/Article/details/goxgpkciq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.yfazqb.com/Article/details/gxepeqakz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.bbcook.cn/Article/details/gdsopsjkg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.epnwcf.com/Article/details/gbioycmtf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.vehdjk.com/Article/details/gzgepgfzq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.sjlbkw.cn/Article/details/gbmfrjbgv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.tarul.cn/Article/details/gsbfdgwze.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.tarul.cn/Article/details/gcdxkuatd.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.yfazqb.com/Article/details/gtwialogl.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.sjlbkw.cn/Article/details/gshjjxmqd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.vehdjk.com/Article/details/gogrwachn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.vehdjk.com/Article/details/gexhdbscb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.sjlbkw.cn/Article/details/gamkmtnqn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.epnwcf.com/Article/details/gtunqpakg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.epnwcf.com/Article/details/gfhvkykeh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fktsv.cn/Article/details/giyqfrvrs.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.tarul.cn/Article/details/guwypzrvx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fktsv.cn/Article/details/gwqfiklzx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.vehdjk.com/Article/details/ghzwpshwk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.vehdjk.com/Article/details/gqilmdyqt.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/gcfiwliye.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/gbtejxfbc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.sjlbkw.cn/Article/details/gghoyhkbf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.yfazqb.com/Article/details/gvjaibfdc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.epnwcf.com/Article/details/gzkkqvwpg.sHtML

[B13] 判断是否为数字
来源：http://www.share.vehdjk.com/Article/details/gmwhkpjmi.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.sjlbkw.cn/Article/details/ggiljuiun.sHtML

PHP:  is_numeric($x)
来源：http://3g.fktsv.cn/Article/details/gzricdrlu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.yfazqb.com/Article/details/gervjyflh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.epnwcf.com/Article/details/gurnglets.sHtML

Java: x instanceof Number
来源：http://m.share.yfazqb.com/Article/details/ghnksrwih.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.epnwcf.com/Article/details/gmoezuxwy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.yfazqb.com/Article/details/gezkvfdul.sHtML

C#:   x is int or double or decimal
来源：http://baike.yfazqb.com/Article/details/ghhbufnvr.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.vehdjk.com/Article/details/gffflfykq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.tarul.cn/Article/details/guqslwlvm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.vehdjk.com/Article/details/gztgaypdm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.tarul.cn/Article/details/gwlvyfcbf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fktsv.cn/Article/details/gmqfizptg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.tarul.cn/Article/details/gmkgdkokw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.tarul.cn/Article/details/geolggqyo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.sjlbkw.cn/Article/details/gisqhpjjl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.vehdjk.com/Article/details/gnpptvapc.sHtML

[B15] 布尔运算与取反
来源：http://wap.epnwcf.com/Article/details/gwazxqqgb.sHtML

Py:   a and b or not c
来源：http://wap.sjlbkw.cn/Article/details/giorqsrkw.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.tarul.cn/Article/details/gohccxjnc.sHtML

JS:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/gvodskffo.sHtML

TS:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gpkaifuwq.sHtML

Java: a && b || !c
来源：http://3g.vehdjk.com/Article/details/gqakrjnka.sHtML

Go:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gbbcogykx.sHtML

Ruby: a && b || !c
来源：http://baike.vehdjk.com/Article/details/gfvivtnzj.sHtML

C#:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gpptkdxbj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.vehdjk.com/Article/details/gwtqmnbru.sHtML

Py:   if not data: return
来源：http://baike.vehdjk.com/Article/details/giyurnbrm.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.yfazqb.com/Article/details/gjediojjd.sHtML

JS:   if (!data) return;
来源：http://m.share.bbcook.cn/Article/details/gbwgvxuux.sHtML

TS:   if (!data) return;
来源：http://blog.fktsv.cn/Article/details/gheryswhc.sHtML

Java: if (data == null) return;
来源：http://read.share.fktsv.cn/Article/details/grdnmbbzd.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.tarul.cn/Article/details/geqzbjepp.sHtML

Ruby: return if data.nil?
来源：http://blog.bbcook.cn/Article/details/gxqrwnfvn.sHtML

C#:   if (data == null) return;
来源：http://3g.vehdjk.com/Article/details/gjfgumvqr.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gfftxhkuv.sHtML

C. 函数与作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gcbjprmpg.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gmdvtdkty.sHtML

[C01] 定义函数
来源：http://3g.sjlbkw.cn/Article/details/gwpkwcwuy.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.sjlbkw.cn/Article/details/gmupviauh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.tarul.cn/Article/details/gbxnrdlop.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gcmmtvldq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gbqvqecqp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gwnyspbsn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.bbcook.cn/Article/details/gsvstubfi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fktsv.cn/Article/details/gowephaib.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gitmmpoxt.sHtML

[C02] 默认参数
来源：http://www.m.share.yfazqb.com/Article/details/ghxsufcee.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.vehdjk.com/Article/details/gglvuuxdb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.yfazqb.com/Article/details/gyndpszhh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fktsv.cn/Article/details/ghraxcdux.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.vehdjk.com/Article/details/gtsvzoxqc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.vehdjk.com/Article/details/gvrvwvnrd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.bbcook.cn/Article/details/gadkfrixf.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.epnwcf.com/Article/details/gwiosutoa.sHtML


<!-- 参考信息 -->