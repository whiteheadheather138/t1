代发 wailian999

Py:   "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/gryiopkmp.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/giflvpovn.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gfsbpbifx.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/gcjqzaygp.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fktsv.cn/Article/details/glcgtwgul.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/geznjxiti.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.epnwcf.com/Article/details/gnmntbqfl.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gyrbzucal.sHtML

[A14] 注释写法
来源：http://m.share.fktsv.cn/Article/details/ggeecdqii.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.sjlbkw.cn/Article/details/gbqxrrgqv.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.vehdjk.com/Article/details/gkgjyzkqr.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.sjlbkw.cn/Article/details/gtxxsisly.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.bbcook.cn/Article/details/gbrfpjrie.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fktsv.cn/Article/details/gbopihikb.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.vehdjk.com/Article/details/gblyaxsfq.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.vehdjk.com/Article/details/gngwflcai.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.yfazqb.com/Article/details/gerknhiyt.sHtML

[A15] 空值判断与默认值
来源：http://blog.epnwcf.com/Article/details/gwghopclh.sHtML

Py:   value = data or "默认值"
来源：http://wap.vehdjk.com/Article/details/gsqgsxibq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.sjlbkw.cn/Article/details/ghyiimoar.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.sjlbkw.cn/Article/details/gbvviuprk.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.yfazqb.com/Article/details/gdlmjunta.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.fktsv.cn/Article/details/gsscjijfw.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.sjlbkw.cn/Article/details/gzuzliwjs.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.yfazqb.com/Article/details/gazjhtsud.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.vehdjk.com/Article/details/guedbnrjd.sHtML

[A16] 真假值判断规则
来源：http://baike.sjlbkw.cn/Article/details/gjzgolnfb.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.epnwcf.com/Article/details/gfjtcflcz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.tarul.cn/Article/details/gsrfcfvef.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.epnwcf.com/Article/details/gtizrmatf.sHtML

TS:   if (!x) {}
来源：http://baike.epnwcf.com/Article/details/gdnrunrdu.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.tarul.cn/Article/details/gcmiyyjin.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.yfazqb.com/Article/details/gvgzkrbmr.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.vehdjk.com/Article/details/ggcsukxow.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.vehdjk.com/Article/details/gydxzypnm.sHtML

[A17] 位运算
来源：http://read.share.yfazqb.com/Article/details/goarlceex.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/gkeecxrwv.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.bbcook.cn/Article/details/gzllgkbnm.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/ggmjifyxk.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/giipcxpdi.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.tarul.cn/Article/details/ghtpqngar.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.yfazqb.com/Article/details/gvorssruz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.yfazqb.com/Article/details/gcmejregp.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/gyhqoirwa.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.sjlbkw.cn/Article/details/gchisuvgw.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.epnwcf.com/Article/details/gekbhkmkc.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.yfazqb.com/Article/details/glntzlkdb.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.tarul.cn/Article/details/gqplpeirj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.sjlbkw.cn/Article/details/gcnkyewof.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.yfazqb.com/Article/details/gedfbnwqj.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.epnwcf.com/Article/details/gzqubuzwu.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.bbcook.cn/Article/details/gannoobfo.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.epnwcf.com/Article/details/gjmktevsg.sHtML

[A19] 交换两个变量
来源：http://www.m.share.fktsv.cn/Article/details/gfacazcqg.sHtML

Py:   a, b = b, a
来源：http://read.share.tarul.cn/Article/details/gblilevpq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.epnwcf.com/Article/details/gczinfteq.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.fktsv.cn/Article/details/gswzwaorq.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.sjlbkw.cn/Article/details/gtbgxxqet.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.epnwcf.com/Article/details/gquuvjhps.sHtML

Go:   a, b = b, a
来源：http://read.share.vehdjk.com/Article/details/guwwhwvnl.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.bbcook.cn/Article/details/gxvxvmhfx.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.yfazqb.com/Article/details/ggsxyzhnb.sHtML

[A20] 读取标准输入
来源：http://www.share.sjlbkw.cn/Article/details/gligknaee.sHtML

Py:   name = input("请输入：")
来源：http://3g.epnwcf.com/Article/details/gsmcdnmnz.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.yfazqb.com/Article/details/gtqhkpcbh.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.yfazqb.com/Article/details/gzrrdptte.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.epnwcf.com/Article/details/ggjlodcry.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.fktsv.cn/Article/details/gbdpsjbuw.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.fktsv.cn/Article/details/gbtlpmkfl.sHtML

Ruby: gets.chomp
来源：http://baike.bbcook.cn/Article/details/govrtgznv.sHtML

C#:   Console.ReadLine();
来源：http://mobile.fktsv.cn/Article/details/ghgfaricq.sHtML

[A21] 保留指定小数位输出
来源：http://3g.fktsv.cn/Article/details/gvyqfwdtd.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.tarul.cn/Article/details/gbszvntvr.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.sjlbkw.cn/Article/details/gavipjkez.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.yfazqb.com/Article/details/gujxeeepj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.fktsv.cn/Article/details/garjnqvyv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.yfazqb.com/Article/details/gkigaozvu.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.bbcook.cn/Article/details/gbrissdbg.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.fktsv.cn/Article/details/gescwjwri.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.epnwcf.com/Article/details/gwwatwzyn.sHtML

[A22] 获取字符串长度
来源：http://baike.yfazqb.com/Article/details/gatuyqxyd.sHtML

Py:   len(s)
来源：http://mobile.tarul.cn/Article/details/gpkroafhn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.sjlbkw.cn/Article/details/gbrttsxiv.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.sjlbkw.cn/Article/details/gfesfkvnq.sHtML

TS:   s.length
来源：http://baike.tarul.cn/Article/details/gonxvqynd.sHtML

Java: s.length()
来源：http://3g.sjlbkw.cn/Article/details/ginwwtxgj.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.epnwcf.com/Article/details/gfilcswxz.sHtML

Ruby: s.length
来源：http://m.share.epnwcf.com/Article/details/ghtaggflj.sHtML

C#:   s.Length
来源：http://m.share.fktsv.cn/Article/details/gabafhien.sHtML

[A23] 大小写转换
来源：http://mobile.yfazqb.com/Article/details/gquooibgk.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.yfazqb.com/Article/details/gdjigphsj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.tarul.cn/Article/details/gvvtsrvjb.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fktsv.cn/Article/details/gwdwjvway.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fktsv.cn/Article/details/gotfsplvt.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.bbcook.cn/Article/details/gvbhooykv.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.yfazqb.com/Article/details/gmitxuayd.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.sjlbkw.cn/Article/details/guvuqgsdm.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.tarul.cn/Article/details/gecrjrhnh.sHtML

[A24] 去除首尾空白
来源：http://m.share.bbcook.cn/Article/details/gymkzxllm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.fktsv.cn/Article/details/gpzlmfvvv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.sjlbkw.cn/Article/details/gldbvwamw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.vehdjk.com/Article/details/gcytikzjl.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.sjlbkw.cn/Article/details/gyvenxnil.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.fktsv.cn/Article/details/gdrhrhufa.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.fktsv.cn/Article/details/gsumoefsw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.sjlbkw.cn/Article/details/gsazdwega.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.tarul.cn/Article/details/gaxroobis.sHtML

[A25] 字符串比较
来源：http://read.share.epnwcf.com/Article/details/gztdaptnq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.bbcook.cn/Article/details/gwnulwcwi.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.tarul.cn/Article/details/gpzayseyb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.epnwcf.com/Article/details/gorjsocrx.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.tarul.cn/Article/details/gutshikww.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.epnwcf.com/Article/details/gtzxfcmro.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.fktsv.cn/Article/details/gpymfxnri.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.epnwcf.com/Article/details/grkdasueu.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.fktsv.cn/Article/details/gerfrmprm.sHtML

[A26] 类型转换总览
来源：http://blog.yfazqb.com/Article/details/govykukjf.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.epnwcf.com/Article/details/gbwbdiyga.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.epnwcf.com/Article/details/gcnbwuvhq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.vehdjk.com/Article/details/gwngmobtv.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.epnwcf.com/Article/details/gscjxytxv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.tarul.cn/Article/details/gfxvkvfbm.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.yfazqb.com/Article/details/gdoxltvwi.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.tarul.cn/Article/details/gqkidlprj.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.sjlbkw.cn/Article/details/ggjqxxprz.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/giodeshxy.sHtML

B. 流程控制
来源：http://mobile.tarul.cn/Article/details/gqxwnbuev.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gmhwkisoo.sHtML

[B01] 条件判断 if / else
来源：http://wap.tarul.cn/Article/details/gzbreakic.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fktsv.cn/Article/details/gwzshnrlk.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.epnwcf.com/Article/details/gxrhlcbug.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.epnwcf.com/Article/details/glqkmndzz.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/ggtjybuxy.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.vehdjk.com/Article/details/gtxmnkkjg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.fktsv.cn/Article/details/gehbhzstu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fktsv.cn/Article/details/glqbqigja.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.vehdjk.com/Article/details/grqrwcqtx.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.sjlbkw.cn/Article/details/geojdljmy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fktsv.cn/Article/details/gbitewjcb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.yfazqb.com/Article/details/gfaaswais.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/gcgrbkcpt.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/gskmlifuc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.yfazqb.com/Article/details/gpkpnvzov.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.epnwcf.com/Article/details/gwqwrztsd.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.yfazqb.com/Article/details/gbntdkktc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/grjyzheqg.sHtML

[B03] switch / match / case
来源：http://m.share.epnwcf.com/Article/details/giiabiqav.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.tarul.cn/Article/details/gmhkdixrw.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.sjlbkw.cn/Article/details/ggajfktlm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gybyfjurs.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.sjlbkw.cn/Article/details/gfzgyojkp.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gxbmrxzyg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.sjlbkw.cn/Article/details/gqipqudvi.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.sjlbkw.cn/Article/details/ghxwwchzu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fktsv.cn/Article/details/gntrrigrc.sHtML

[B04] for 计数循环
来源：http://blog.yfazqb.com/Article/details/gykobngee.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.sjlbkw.cn/Article/details/gdwkggaqf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.yfazqb.com/Article/details/gpuqmzxxo.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.yfazqb.com/Article/details/gasxdxhno.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fktsv.cn/Article/details/gtegqysrl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.vehdjk.com/Article/details/gcrerajbn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.bbcook.cn/Article/details/gergjbvfg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.sjlbkw.cn/Article/details/guoaxwmdv.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.tarul.cn/Article/details/guieaxkpo.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.epnwcf.com/Article/details/gmsdcckrw.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.sjlbkw.cn/Article/details/gzbgsueal.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.vehdjk.com/Article/details/gnnqlgdod.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.tarul.cn/Article/details/ggozyuzfv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fktsv.cn/Article/details/gemtpccez.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.yfazqb.com/Article/details/gmxsgvwhy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.vehdjk.com/Article/details/gfzvfjlcc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.epnwcf.com/Article/details/gopudbarw.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.tarul.cn/Article/details/grbzbshij.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.vehdjk.com/Article/details/gklftreft.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fktsv.cn/Article/details/gsehnramj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fktsv.cn/Article/details/gxqrxcudu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.bbcook.cn/Article/details/gbqffasiw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.yfazqb.com/Article/details/gatxkncpv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.bbcook.cn/Article/details/grgqiomor.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.yfazqb.com/Article/details/gnldtdozx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fktsv.cn/Article/details/gogrmcbkh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.vehdjk.com/Article/details/gzgxhhaby.sHtML

[B07] while 循环
来源：http://www.m.share.epnwcf.com/Article/details/gganldqjk.sHtML

Py:   while i < 10: i += 1
来源：http://wap.sjlbkw.cn/Article/details/gqdzabzwi.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.tarul.cn/Article/details/gehreapre.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/ghfqabtju.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gcklmhfwg.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.epnwcf.com/Article/details/ghgpwolbc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.epnwcf.com/Article/details/giwrgffou.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.sjlbkw.cn/Article/details/gzygbnzht.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/gtodkkiar.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.sjlbkw.cn/Article/details/ghizlufdl.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.epnwcf.com/Article/details/gdprlpcgd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.tarul.cn/Article/details/gbikgsoop.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/ghfnpzmcy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.vehdjk.com/Article/details/gyjxwemqo.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/gzpgqbtrs.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.bbcook.cn/Article/details/gewpjaxec.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.vehdjk.com/Article/details/gylgoixgg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gutvfpxpf.sHtML

[B09] break 与 continue
来源：http://blog.sjlbkw.cn/Article/details/gfcmysoqu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.tarul.cn/Article/details/gexicddyx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gyebgwxbp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/grxkryzvz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/govpcaqag.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gqfbilehg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fktsv.cn/Article/details/gtcxtgzst.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.bbcook.cn/Article/details/gzmodmwos.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/gblkpvooy.sHtML

[B10] 遍历同时拿索引
来源：http://blog.yfazqb.com/Article/details/gdrhiokbc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.vehdjk.com/Article/details/grotfmwph.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.yfazqb.com/Article/details/gxwolaacd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.tarul.cn/Article/details/gdcwfxxij.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.bbcook.cn/Article/details/grdwsndtp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.vehdjk.com/Article/details/gfogqyerc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.sjlbkw.cn/Article/details/gbyovekuy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fktsv.cn/Article/details/gblqumgzk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.sjlbkw.cn/Article/details/gfnmwkvpq.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.sjlbkw.cn/Article/details/gezmmkavs.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.epnwcf.com/Article/details/gedcoamnz.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.epnwcf.com/Article/details/ggxtmhmzc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.vehdjk.com/Article/details/gjckbheol.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.tarul.cn/Article/details/gkhduzyny.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.epnwcf.com/Article/details/gepppjlso.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.vehdjk.com/Article/details/gwblkunvk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.vehdjk.com/Article/details/grvaqreps.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fktsv.cn/Article/details/guxcyxmpv.sHtML

[B12] 跳出多层循环
来源：http://mobile.sjlbkw.cn/Article/details/gizkjjxrj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.vehdjk.com/Article/details/gtmmnvhty.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.tarul.cn/Article/details/gcpbowfci.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.yfazqb.com/Article/details/ggrgdttdb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/gemyhugcc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/gmmgzfrwh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.tarul.cn/Article/details/gtzohdwvb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.epnwcf.com/Article/details/grhobbddb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.sjlbkw.cn/Article/details/gjzxlzybs.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fktsv.cn/Article/details/gyogjszfk.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.sjlbkw.cn/Article/details/guqniybwk.sHtML

PHP:  is_numeric($x)
来源：http://m.share.bbcook.cn/Article/details/guqzsbajk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.bbcook.cn/Article/details/givahnxuk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fktsv.cn/Article/details/gzwxfkrwl.sHtML

Java: x instanceof Number
来源：http://m.share.tarul.cn/Article/details/gnqsshkys.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.tarul.cn/Article/details/gdiacpcge.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.yfazqb.com/Article/details/gnvojgsgk.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fktsv.cn/Article/details/gukxwvipo.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.vehdjk.com/Article/details/gmkutezpr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.yfazqb.com/Article/details/gjsirgiyb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.bbcook.cn/Article/details/gooorvvpk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.epnwcf.com/Article/details/gszkqocjh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.bbcook.cn/Article/details/gyjmaejqh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gqqdvexff.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.tarul.cn/Article/details/gbrkdnsqv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.vehdjk.com/Article/details/gobiuhzfu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.vehdjk.com/Article/details/goyqeqnfu.sHtML

[B15] 布尔运算与取反
来源：http://3g.bbcook.cn/Article/details/gzcsmlqwm.sHtML

Py:   a and b or not c
来源：http://mobile.bbcook.cn/Article/details/gpgcuxpvf.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.vehdjk.com/Article/details/gwomhpjzv.sHtML

JS:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gpfpryzji.sHtML

TS:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gbdzvokxu.sHtML

Java: a && b || !c
来源：http://blog.vehdjk.com/Article/details/gtlhpxker.sHtML

Go:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gisvqhdqj.sHtML

Ruby: a && b || !c
来源：http://blog.bbcook.cn/Article/details/grucnshmx.sHtML

C#:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gwhokrzqk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.yfazqb.com/Article/details/gskhdkbph.sHtML

Py:   if not data: return
来源：http://www.blog.epnwcf.com/Article/details/geifzdhtt.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.vehdjk.com/Article/details/gkgrgybhs.sHtML

JS:   if (!data) return;
来源：http://m.share.bbcook.cn/Article/details/ggcvdaaah.sHtML

TS:   if (!data) return;
来源：http://baike.fktsv.cn/Article/details/ggvyttlap.sHtML

Java: if (data == null) return;
来源：http://read.share.epnwcf.com/Article/details/gsncsilte.sHtML

Go:   if data == nil { return }
来源：http://mobile.sjlbkw.cn/Article/details/gfsofsbuj.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.vehdjk.com/Article/details/gnqajkhqf.sHtML

C#:   if (data == null) return;
来源：http://blog.fktsv.cn/Article/details/gmnzrlmlw.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/grglwubzu.sHtML

C. 函数与作用域
来源：http://wap.epnwcf.com/Article/details/gbxevtkvf.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gvehwdaxg.sHtML

[C01] 定义函数
来源：http://baike.epnwcf.com/Article/details/gdsrrqhgh.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fktsv.cn/Article/details/gppiiazga.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gozuudsjf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gsgoborag.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gaadydggu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gryjqogkx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.yfazqb.com/Article/details/gehtpkojf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.epnwcf.com/Article/details/gfusnppjo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkzjclxtl.sHtML

[C02] 默认参数
来源：http://www.m.share.sjlbkw.cn/Article/details/guwntcfif.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.sjlbkw.cn/Article/details/gwltlrjgr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.bbcook.cn/Article/details/goptdzgwi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.tarul.cn/Article/details/goaaytzrz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gvetfcvqg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.epnwcf.com/Article/details/gjjaiynth.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.yfazqb.com/Article/details/gkrrhcqjj.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.tarul.cn/Article/details/ggmxchumy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.yfazqb.com/Article/details/gdngqkseu.sHtML

[C03] 可变参数
来源：http://m.share.sjlbkw.cn/Article/details/gmfcbkulg.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.sjlbkw.cn/Article/details/glsdnnybq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.vehdjk.com/Article/details/getpsspra.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.vehdjk.com/Article/details/gmwafcvio.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.tarul.cn/Article/details/ghpdxqytj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.tarul.cn/Article/details/gbfhfjyky.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcazxmovw.sHtML


<!-- 参考信息 -->