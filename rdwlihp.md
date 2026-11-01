代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.m.share.epnwcf.com/Article/details/ggzdmaffu.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gskmuovjl.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/gessrbgpj.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/gpzleshra.sHtML

Java: "第一行\n第二行"
来源：http://m.share.vehdjk.com/Article/details/gukjccyzb.sHtML

Go:   "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/gaxkzbwot.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/gzmlfucvc.sHtML

C#:   "第一行\n第二行"
来源：http://baike.vehdjk.com/Article/details/gbhxcuuhn.sHtML

[A14] 注释写法
来源：http://3g.bbcook.cn/Article/details/gakbacipd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.tarul.cn/Article/details/ggsfyzexe.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.bbcook.cn/Article/details/gnbiqwnst.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.yfazqb.com/Article/details/gmcmmiwqi.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.tarul.cn/Article/details/gktdxdgdf.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.fktsv.cn/Article/details/gvcgxooxd.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.bbcook.cn/Article/details/gxsffmypd.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.tarul.cn/Article/details/gmcoiwqlw.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/gphvuvmuy.sHtML

[A15] 空值判断与默认值
来源：http://3g.bbcook.cn/Article/details/gwrpzhypq.sHtML

Py:   value = data or "默认值"
来源：http://wap.bbcook.cn/Article/details/gvbjyfjzo.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.tarul.cn/Article/details/gbmurryrp.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.bbcook.cn/Article/details/geowgufdk.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.epnwcf.com/Article/details/guaaojvsg.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.bbcook.cn/Article/details/gpmhpikvy.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.sjlbkw.cn/Article/details/gbwjwmeus.sHtML

Ruby: value = data || "默认值"
来源：http://baike.sjlbkw.cn/Article/details/gfdahprrb.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.tarul.cn/Article/details/gexakqllr.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.bbcook.cn/Article/details/gpxmuiqup.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.epnwcf.com/Article/details/gbcruekii.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.epnwcf.com/Article/details/gvmfbnmje.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.fktsv.cn/Article/details/gikwpwdmo.sHtML

TS:   if (!x) {}
来源：http://read.share.epnwcf.com/Article/details/gumatdfoz.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.bbcook.cn/Article/details/gkzxnmxyh.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.vehdjk.com/Article/details/gmmvqimod.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.tarul.cn/Article/details/ghejjybpz.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.yfazqb.com/Article/details/gznjxdcyp.sHtML

[A17] 位运算
来源：http://read.share.bbcook.cn/Article/details/gazlvbivr.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.sjlbkw.cn/Article/details/gtnhthqgr.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.tarul.cn/Article/details/gfmymigky.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.yfazqb.com/Article/details/glaayfquw.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/gokzfuwjx.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/gnkbcxcul.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.bbcook.cn/Article/details/gvunraolq.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.vehdjk.com/Article/details/gdatbanrf.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.bbcook.cn/Article/details/guplbzdaa.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.fktsv.cn/Article/details/gsvsbsxrs.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.sjlbkw.cn/Article/details/glgmpaylk.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.sjlbkw.cn/Article/details/gujponkxd.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.vehdjk.com/Article/details/gaisxotdb.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fktsv.cn/Article/details/gechlsicq.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.fktsv.cn/Article/details/ggsoozqrv.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.yfazqb.com/Article/details/gjkjllgod.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.yfazqb.com/Article/details/gfxnrhdyg.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.yfazqb.com/Article/details/gmzfsbzmi.sHtML

[A19] 交换两个变量
来源：http://blog.yfazqb.com/Article/details/gzfczheuf.sHtML

Py:   a, b = b, a
来源：http://wap.tarul.cn/Article/details/gbjjtwmzz.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.sjlbkw.cn/Article/details/gsmsouauk.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.sjlbkw.cn/Article/details/gjgckxbja.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.epnwcf.com/Article/details/gjkdixcua.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.tarul.cn/Article/details/gvxnzsdmj.sHtML

Go:   a, b = b, a
来源：http://www.blog.sjlbkw.cn/Article/details/gvmeaprcj.sHtML

Ruby: a, b = b, a
来源：http://m.share.sjlbkw.cn/Article/details/gwimunnlk.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.yfazqb.com/Article/details/gdokkdtga.sHtML

[A20] 读取标准输入
来源：http://read.share.yfazqb.com/Article/details/gwwfhoiqt.sHtML

Py:   name = input("请输入：")
来源：http://mobile.vehdjk.com/Article/details/glwvpwkog.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.epnwcf.com/Article/details/grurdyfct.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.fktsv.cn/Article/details/gqkubzcxe.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.vehdjk.com/Article/details/gkyjxeznr.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.tarul.cn/Article/details/gqvwdybjm.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.bbcook.cn/Article/details/gxmtdqhod.sHtML

Ruby: gets.chomp
来源：http://www.share.fktsv.cn/Article/details/gqbphckwk.sHtML

C#:   Console.ReadLine();
来源：http://read.share.sjlbkw.cn/Article/details/grugmrome.sHtML

[A21] 保留指定小数位输出
来源：http://baike.fktsv.cn/Article/details/gdcfbafat.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.fktsv.cn/Article/details/gslgashfz.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.bbcook.cn/Article/details/gwpicwxrc.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.sjlbkw.cn/Article/details/gsdwuygwo.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.bbcook.cn/Article/details/grvnmwhyw.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.vehdjk.com/Article/details/gnrtfaxhs.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.bbcook.cn/Article/details/gmimqowel.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.vehdjk.com/Article/details/ghhxlsmcs.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.fktsv.cn/Article/details/gqpluzfrj.sHtML

[A22] 获取字符串长度
来源：http://www.blog.epnwcf.com/Article/details/gptfbpqwb.sHtML

Py:   len(s)
来源：http://mobile.bbcook.cn/Article/details/gwzoqmqcx.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.tarul.cn/Article/details/gccifahaz.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.sjlbkw.cn/Article/details/ggztgmbti.sHtML

TS:   s.length
来源：http://mobile.vehdjk.com/Article/details/gwzuqkcgs.sHtML

Java: s.length()
来源：http://baike.fktsv.cn/Article/details/gwvblbdfk.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.vehdjk.com/Article/details/ghbgawvab.sHtML

Ruby: s.length
来源：http://read.share.tarul.cn/Article/details/gsqopgwsf.sHtML

C#:   s.Length
来源：http://3g.vehdjk.com/Article/details/gxwscjgbm.sHtML

[A23] 大小写转换
来源：http://mobile.bbcook.cn/Article/details/gauhciwpq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.fktsv.cn/Article/details/gpludnnal.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.epnwcf.com/Article/details/gvgdfkuon.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.vehdjk.com/Article/details/gqdrujboc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fktsv.cn/Article/details/gvqcqvncm.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.bbcook.cn/Article/details/gzirlvzdm.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.epnwcf.com/Article/details/gxqwpxysr.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.sjlbkw.cn/Article/details/guzecpqgp.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.epnwcf.com/Article/details/gncztzlca.sHtML

[A24] 去除首尾空白
来源：http://mobile.sjlbkw.cn/Article/details/gicgvsdct.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.yfazqb.com/Article/details/gsqhpkpij.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.yfazqb.com/Article/details/ggkmwwwlq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fktsv.cn/Article/details/gtkicirhh.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fktsv.cn/Article/details/gtvvohbac.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.epnwcf.com/Article/details/gwbffrsbc.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.vehdjk.com/Article/details/gknajfptl.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.yfazqb.com/Article/details/gxasunrdv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fktsv.cn/Article/details/gurgebtxc.sHtML

[A25] 字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/gcmkzqgva.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.fktsv.cn/Article/details/gcvalubmy.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.yfazqb.com/Article/details/gneyrdcbx.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.epnwcf.com/Article/details/gbyebisvj.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.vehdjk.com/Article/details/gxwbrbaym.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.epnwcf.com/Article/details/giisyzqze.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.fktsv.cn/Article/details/gmlzskxep.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.yfazqb.com/Article/details/gowuubgst.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.sjlbkw.cn/Article/details/gfbqgeypn.sHtML

[A26] 类型转换总览
来源：http://mobile.tarul.cn/Article/details/gfdyvmfek.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fktsv.cn/Article/details/gbtkoplbt.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.fktsv.cn/Article/details/griblytrk.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.tarul.cn/Article/details/ghqwtteaa.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fktsv.cn/Article/details/gobyiwdnz.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.epnwcf.com/Article/details/gpjstwwnz.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.fktsv.cn/Article/details/gokydvqrw.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.fktsv.cn/Article/details/geicwvhea.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.fktsv.cn/Article/details/ganmavhdr.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gclmsardd.sHtML

B. 流程控制
来源：http://baike.fktsv.cn/Article/details/gwdjyfyfs.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/grqbblgyz.sHtML

[B01] 条件判断 if / else
来源：http://3g.bbcook.cn/Article/details/gssvmeybr.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.sjlbkw.cn/Article/details/gkdfpwmri.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gnonirmpi.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gbftdhluq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.yfazqb.com/Article/details/gkulkitwc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fktsv.cn/Article/details/guutzojpk.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.epnwcf.com/Article/details/gotuossir.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.bbcook.cn/Article/details/gnvgbkarp.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.epnwcf.com/Article/details/gzvwagrpz.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.bbcook.cn/Article/details/gdwltjgso.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.epnwcf.com/Article/details/gcupwsigu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.tarul.cn/Article/details/gymhchmuk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/gtwypxenp.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/grqxrbvkd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/gtrqqewsq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.tarul.cn/Article/details/gkkcvhpvn.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.yfazqb.com/Article/details/gjkwymxtm.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.bbcook.cn/Article/details/gnmjkjxmo.sHtML

[B03] switch / match / case
来源：http://www.blog.bbcook.cn/Article/details/gdncgxdjq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.epnwcf.com/Article/details/gwwzbvjhk.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/gdeciinxz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gywvrbszv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/ggnvejdgz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.epnwcf.com/Article/details/gledxrhtx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.yfazqb.com/Article/details/ggtburpvf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.bbcook.cn/Article/details/gtwjwlcwc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.yfazqb.com/Article/details/gjxaopheq.sHtML

[B04] for 计数循环
来源：http://mobile.tarul.cn/Article/details/gscgpovvf.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.fktsv.cn/Article/details/giopagwkh.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.bbcook.cn/Article/details/gnqukafzj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.bbcook.cn/Article/details/gfvkosipf.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fktsv.cn/Article/details/gifxowxpy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.bbcook.cn/Article/details/gankzrlai.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.bbcook.cn/Article/details/gpczyjorx.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.fktsv.cn/Article/details/gviqsuqqu.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fktsv.cn/Article/details/gwgmogjkz.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.epnwcf.com/Article/details/gyztekovu.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.epnwcf.com/Article/details/gwvveodim.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.fktsv.cn/Article/details/goliypjab.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.epnwcf.com/Article/details/gmwowgpka.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.vehdjk.com/Article/details/gztwqbiou.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.vehdjk.com/Article/details/gpvanupni.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.vehdjk.com/Article/details/ggyquttlt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.vehdjk.com/Article/details/gfrwenogm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.tarul.cn/Article/details/gxegmopgz.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.vehdjk.com/Article/details/gksvxqkzz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.epnwcf.com/Article/details/gjcnvbaay.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.sjlbkw.cn/Article/details/gemmgdsnp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.vehdjk.com/Article/details/gxztsfxvx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.bbcook.cn/Article/details/gtugaajcs.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.epnwcf.com/Article/details/gerkwvjhy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fktsv.cn/Article/details/gkqmrosrw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.vehdjk.com/Article/details/gcfvywmjj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.sjlbkw.cn/Article/details/guflttcso.sHtML

[B07] while 循环
来源：http://baike.yfazqb.com/Article/details/gzklpdyyb.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.epnwcf.com/Article/details/gayglihou.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.yfazqb.com/Article/details/gwbsfcvrv.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gcdxmgfan.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gcjbxenui.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.vehdjk.com/Article/details/gbnmkvyzy.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fktsv.cn/Article/details/gymutbhzd.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.sjlbkw.cn/Article/details/givevlhmu.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gpfivwbvv.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.epnwcf.com/Article/details/gbmccpbxu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.sjlbkw.cn/Article/details/gwngoupgn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.yfazqb.com/Article/details/glyapjwgf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gftlpsmlq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fktsv.cn/Article/details/gzukyyilp.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gresowlcw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.epnwcf.com/Article/details/gcngmzuoi.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fktsv.cn/Article/details/gjmkxbjdo.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/gjrvbgmvx.sHtML

[B09] break 与 continue
来源：http://wap.epnwcf.com/Article/details/gngssurdy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.epnwcf.com/Article/details/gkunbyfeb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gslgqarxv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gvjrwavtx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gjvvjsvna.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/gxzkrtoru.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.fktsv.cn/Article/details/gheebgahr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.vehdjk.com/Article/details/gfgxvmuyz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gwormbqyc.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.yfazqb.com/Article/details/gzpeojxtu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.bbcook.cn/Article/details/gikubpcmw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.bbcook.cn/Article/details/gycsxpzzw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.bbcook.cn/Article/details/gghbycwyb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.vehdjk.com/Article/details/gznhcyosi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.bbcook.cn/Article/details/geodbbcke.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.bbcook.cn/Article/details/gvfrcuvat.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.epnwcf.com/Article/details/gpanacxai.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.bbcook.cn/Article/details/grobzsawu.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.yfazqb.com/Article/details/gafrjoooa.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.sjlbkw.cn/Article/details/gmmjxboah.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.yfazqb.com/Article/details/gdwivlcjb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.sjlbkw.cn/Article/details/gupaznlef.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.sjlbkw.cn/Article/details/gjtedkimd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.epnwcf.com/Article/details/gmouyoygc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.vehdjk.com/Article/details/gmpwhnvhy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.bbcook.cn/Article/details/gckjtjngk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.yfazqb.com/Article/details/goujyybpg.sHtML

[B12] 跳出多层循环
来源：http://blog.epnwcf.com/Article/details/gzniuinkx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.vehdjk.com/Article/details/gufwbbukn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.epnwcf.com/Article/details/gsrfzyxmw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.epnwcf.com/Article/details/gucspbwoc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.yfazqb.com/Article/details/gzsrclofd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/gqxanmlhu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.vehdjk.com/Article/details/gvcykever.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.sjlbkw.cn/Article/details/ghykwyuse.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.sjlbkw.cn/Article/details/gjbldhkqk.sHtML

[B13] 判断是否为数字
来源：http://m.share.vehdjk.com/Article/details/ggduvfmwr.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.tarul.cn/Article/details/gjbskxooa.sHtML

PHP:  is_numeric($x)
来源：http://baike.epnwcf.com/Article/details/gwrlpkbgy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.yfazqb.com/Article/details/gajotrwzo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.sjlbkw.cn/Article/details/gbmcvlwiz.sHtML

Java: x instanceof Number
来源：http://www.m.share.vehdjk.com/Article/details/gdnlrsfaw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.vehdjk.com/Article/details/gikyobkgy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.epnwcf.com/Article/details/gcexrzseq.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.bbcook.cn/Article/details/gpvbptahs.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.bbcook.cn/Article/details/gbmhgjzwb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.sjlbkw.cn/Article/details/glxptqjkr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.vehdjk.com/Article/details/gvjfrthvi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/ghvstgcbj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.epnwcf.com/Article/details/gdyezsjdk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fktsv.cn/Article/details/ggvvvrblj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.vehdjk.com/Article/details/gcrqeizhw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gensukhmv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.yfazqb.com/Article/details/gtyuoiqwg.sHtML

[B15] 布尔运算与取反
来源：http://mobile.yfazqb.com/Article/details/gpqsyqhyb.sHtML

Py:   a and b or not c
来源：http://m.share.epnwcf.com/Article/details/guettrvlw.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fktsv.cn/Article/details/gnstyowau.sHtML

JS:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gcxfvzkto.sHtML

TS:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gilupkuft.sHtML

Java: a && b || !c
来源：http://blog.bbcook.cn/Article/details/gniaxuqxc.sHtML

Go:   a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gxfwqqztn.sHtML

Ruby: a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gqdfanjox.sHtML

C#:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gmzsdywck.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.tarul.cn/Article/details/grobvwbym.sHtML

Py:   if not data: return
来源：http://mobile.bbcook.cn/Article/details/gcqprisix.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.epnwcf.com/Article/details/gueappdrd.sHtML

JS:   if (!data) return;
来源：http://m.share.sjlbkw.cn/Article/details/guvhbtgyh.sHtML

TS:   if (!data) return;
来源：http://m.share.bbcook.cn/Article/details/gagfbnhxa.sHtML

Java: if (data == null) return;
来源：http://www.blog.fktsv.cn/Article/details/geqjujqoh.sHtML

Go:   if data == nil { return }
来源：http://www.blog.tarul.cn/Article/details/gzqeutptv.sHtML

Ruby: return if data.nil?
来源：http://blog.fktsv.cn/Article/details/gmfaddifp.sHtML

C#:   if (data == null) return;
来源：http://www.blog.bbcook.cn/Article/details/gichdppmb.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gxoiqhooa.sHtML

C. 函数与作用域
来源：http://www.m.share.epnwcf.com/Article/details/ghisbvbrz.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gzmmovpju.sHtML

[C01] 定义函数
来源：http://blog.epnwcf.com/Article/details/genzbitpc.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.bbcook.cn/Article/details/gsvpgcayt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/ggttpxwsp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gxtyyfdfv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/grlyhjxdd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gllhwdion.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.sjlbkw.cn/Article/details/gefllxtnn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.vehdjk.com/Article/details/gewtdcxel.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gvofivdok.sHtML

[C02] 默认参数
来源：http://mobile.tarul.cn/Article/details/gwslejiud.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.bbcook.cn/Article/details/gstnrbltg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.epnwcf.com/Article/details/gunzjbopq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gujnhzyzg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.tarul.cn/Article/details/gqgbhgjer.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.epnwcf.com/Article/details/gznqmftku.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fktsv.cn/Article/details/grbzvixdy.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.sjlbkw.cn/Article/details/gbmrspbkh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.vehdjk.com/Article/details/gtjilmcnq.sHtML

[C03] 可变参数
来源：http://www.blog.tarul.cn/Article/details/grlfqwfam.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.epnwcf.com/Article/details/geqysnsej.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.sjlbkw.cn/Article/details/gbigorgrr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fktsv.cn/Article/details/gnfmwnmju.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.yfazqb.com/Article/details/ggpviqavn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.tarul.cn/Article/details/gxhqsaskt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.epnwcf.com/Article/details/gnimoilwi.sHtML


<!-- 参考信息 -->