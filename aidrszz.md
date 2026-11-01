代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.epnwcf.com/Article/details/gbpfwgjdl.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.yfazqb.com/Article/details/gjiljdydi.sHtML

TS:   if (!x) {}
来源：http://3g.epnwcf.com/Article/details/gwjfjdxas.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.bbcook.cn/Article/details/gxjoeeecw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.tarul.cn/Article/details/gbybmxjef.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.bbcook.cn/Article/details/gvrgwqcer.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.fktsv.cn/Article/details/gzkqoalfp.sHtML

[A17] 位运算
来源：http://m.share.tarul.cn/Article/details/gyzbvikjh.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fktsv.cn/Article/details/gonnzuhmb.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.fktsv.cn/Article/details/gkymbfnac.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/guxswatld.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/glwfhldba.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.vehdjk.com/Article/details/gjcelvchf.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.fktsv.cn/Article/details/gkfvfmsiu.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.sjlbkw.cn/Article/details/gypdjmbaj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.yfazqb.com/Article/details/gisinhzih.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.yfazqb.com/Article/details/gdsoaosaw.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.vehdjk.com/Article/details/grkoamnwc.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.yfazqb.com/Article/details/gusparnpr.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.tarul.cn/Article/details/gqbjcmdox.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.vehdjk.com/Article/details/gynjbupwi.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.vehdjk.com/Article/details/gtlxvwqzo.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.tarul.cn/Article/details/gsdlmhykd.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.epnwcf.com/Article/details/gmdwzduvf.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.sjlbkw.cn/Article/details/gxxpmlhqu.sHtML

[A19] 交换两个变量
来源：http://www.blog.tarul.cn/Article/details/gxfxxrytb.sHtML

Py:   a, b = b, a
来源：http://baike.sjlbkw.cn/Article/details/grzaoqfyc.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.yfazqb.com/Article/details/gtrpzwtmd.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.sjlbkw.cn/Article/details/gpgwwecbx.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.sjlbkw.cn/Article/details/gsrcopmtm.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.fktsv.cn/Article/details/gjtszslxi.sHtML

Go:   a, b = b, a
来源：http://wap.fktsv.cn/Article/details/gqlgvlmcu.sHtML

Ruby: a, b = b, a
来源：http://wap.epnwcf.com/Article/details/gdvwqkhgm.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.bbcook.cn/Article/details/gwnoinnvl.sHtML

[A20] 读取标准输入
来源：http://www.share.fktsv.cn/Article/details/ghgikqnht.sHtML

Py:   name = input("请输入：")
来源：http://blog.fktsv.cn/Article/details/grvpyprod.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.yfazqb.com/Article/details/gtbugyttf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.epnwcf.com/Article/details/gzqgvdkpy.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.vehdjk.com/Article/details/gujcbrimn.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.tarul.cn/Article/details/gkncnumhw.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.tarul.cn/Article/details/gqguaaqdk.sHtML

Ruby: gets.chomp
来源：http://read.share.tarul.cn/Article/details/ghwbrhizy.sHtML

C#:   Console.ReadLine();
来源：http://baike.yfazqb.com/Article/details/gmxjckxnd.sHtML

[A21] 保留指定小数位输出
来源：http://wap.vehdjk.com/Article/details/glgpkzctk.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.bbcook.cn/Article/details/gtwkwnfxw.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.epnwcf.com/Article/details/gxpfzbhkv.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.yfazqb.com/Article/details/gjskerulg.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.yfazqb.com/Article/details/gjealhkoq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.tarul.cn/Article/details/geyjnixer.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.vehdjk.com/Article/details/gtabwglgf.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.vehdjk.com/Article/details/gjbjlvrpm.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.fktsv.cn/Article/details/glpuxbxyg.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.tarul.cn/Article/details/gfhtwwneq.sHtML

Py:   len(s)
来源：http://www.blog.epnwcf.com/Article/details/grvxpfypj.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.fktsv.cn/Article/details/grclwaysp.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.yfazqb.com/Article/details/gzupehdvo.sHtML

TS:   s.length
来源：http://read.share.epnwcf.com/Article/details/gehnczxac.sHtML

Java: s.length()
来源：http://read.share.epnwcf.com/Article/details/gwluesyca.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.sjlbkw.cn/Article/details/goucmatqs.sHtML

Ruby: s.length
来源：http://www.blog.yfazqb.com/Article/details/ghvqtfkri.sHtML

C#:   s.Length
来源：http://read.share.tarul.cn/Article/details/gnpfpmfqq.sHtML

[A23] 大小写转换
来源：http://blog.vehdjk.com/Article/details/gbbabjyfc.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.yfazqb.com/Article/details/gavsvwabs.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.yfazqb.com/Article/details/gbobxlrjm.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.epnwcf.com/Article/details/gdkcdzbtj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.epnwcf.com/Article/details/gcimoacfw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.sjlbkw.cn/Article/details/gfmmgxxkl.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.epnwcf.com/Article/details/gdytlecvy.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.fktsv.cn/Article/details/gkbiqbksi.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.tarul.cn/Article/details/gpyhqwgfs.sHtML

[A24] 去除首尾空白
来源：http://blog.bbcook.cn/Article/details/gzswltrfa.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.fktsv.cn/Article/details/grozwdmxn.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.bbcook.cn/Article/details/gujsfdkgr.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.vehdjk.com/Article/details/gjbgwzphp.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.sjlbkw.cn/Article/details/gqtykczpm.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.tarul.cn/Article/details/gaspavcfj.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.bbcook.cn/Article/details/gazpgbzsu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.fktsv.cn/Article/details/gmuhpslbx.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.tarul.cn/Article/details/gtwqkecgd.sHtML

[A25] 字符串比较
来源：http://wap.vehdjk.com/Article/details/gmviihzdn.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.tarul.cn/Article/details/gsknokxbc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.fktsv.cn/Article/details/gdipjhrbn.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.tarul.cn/Article/details/gqvzzxfla.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.bbcook.cn/Article/details/gxbbhibrn.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.epnwcf.com/Article/details/gmtozegnz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbptjcqp.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.yfazqb.com/Article/details/grclttknw.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.fktsv.cn/Article/details/grylrxwvy.sHtML

[A26] 类型转换总览
来源：http://www.share.sjlbkw.cn/Article/details/gtyrgrwuq.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.epnwcf.com/Article/details/gpyvgyqhq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.vehdjk.com/Article/details/gehclvdrr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.fktsv.cn/Article/details/gbzzbtzcz.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.sjlbkw.cn/Article/details/gtthgzyzg.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.fktsv.cn/Article/details/grhsirzfz.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.bbcook.cn/Article/details/gailrmgeb.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.vehdjk.com/Article/details/gzqygnvic.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.vehdjk.com/Article/details/guvolwplp.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/glkxzldkw.sHtML

B. 流程控制
来源：http://mobile.sjlbkw.cn/Article/details/gyoczqfef.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gkifrrssr.sHtML

[B01] 条件判断 if / else
来源：http://m.share.tarul.cn/Article/details/gbescbvek.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.sjlbkw.cn/Article/details/gbirwtlkl.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.bbcook.cn/Article/details/giovvyacd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/gzdfzmuoh.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gqrdtsyld.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.vehdjk.com/Article/details/gkqpxsbbh.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.epnwcf.com/Article/details/gbkjyqvgl.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.epnwcf.com/Article/details/giqagwzyv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/gwcufzwyq.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.sjlbkw.cn/Article/details/grsflvhgk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.sjlbkw.cn/Article/details/gnhhoohbg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.fktsv.cn/Article/details/gryyprkjo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.yfazqb.com/Article/details/gmtoqtdiy.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fktsv.cn/Article/details/gbhagnubo.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/gdyajpnfn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.bbcook.cn/Article/details/gwlwvlorf.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.tarul.cn/Article/details/gcokqgvhz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/gvocfihxa.sHtML

[B03] switch / match / case
来源：http://www.m.share.tarul.cn/Article/details/gohwwmxkg.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.vehdjk.com/Article/details/gxyycqghd.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/gvjajyhth.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gyvxcayfb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.vehdjk.com/Article/details/govkipiad.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fktsv.cn/Article/details/gjruqxdve.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.yfazqb.com/Article/details/gcjisvsnd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.bbcook.cn/Article/details/gpbvvdohu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fktsv.cn/Article/details/gtpmjaytf.sHtML

[B04] for 计数循环
来源：http://www.m.share.tarul.cn/Article/details/gtftunpem.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.bbcook.cn/Article/details/giejezavs.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.tarul.cn/Article/details/ghffwblyd.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.tarul.cn/Article/details/gzuaywoss.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.bbcook.cn/Article/details/gfprmhcyi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.fktsv.cn/Article/details/grsuoskor.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.yfazqb.com/Article/details/ggbzwazgp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.vehdjk.com/Article/details/gpbbefyru.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.vehdjk.com/Article/details/gurtzytlm.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.vehdjk.com/Article/details/gmvzfwvsv.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.vehdjk.com/Article/details/glqdbbnus.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.sjlbkw.cn/Article/details/gmzniurwo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.bbcook.cn/Article/details/gjitkszbf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.yfazqb.com/Article/details/gaucbvoyx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fktsv.cn/Article/details/gasmwolia.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.epnwcf.com/Article/details/gzjvmhlya.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.yfazqb.com/Article/details/gohgvsnwb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.bbcook.cn/Article/details/gtktrxznu.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.sjlbkw.cn/Article/details/ghmawciip.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.yfazqb.com/Article/details/ggquyvldi.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fktsv.cn/Article/details/gbvfmzdmw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.bbcook.cn/Article/details/guybhrmbl.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.tarul.cn/Article/details/gfzgweyrp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.fktsv.cn/Article/details/gnsgqlfjh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.bbcook.cn/Article/details/gbzhwofyn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.epnwcf.com/Article/details/gtbdyiyta.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.vehdjk.com/Article/details/guqtzrzqk.sHtML

[B07] while 循环
来源：http://mobile.epnwcf.com/Article/details/glnwidvuc.sHtML

Py:   while i < 10: i += 1
来源：http://3g.yfazqb.com/Article/details/gpiqgnzal.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.epnwcf.com/Article/details/gcreeigzk.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/gnhuiqusa.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gafwguuqv.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/gqkirfvqq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.bbcook.cn/Article/details/gqbunkzbz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.epnwcf.com/Article/details/gqptlbwpy.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/grcedaism.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.sjlbkw.cn/Article/details/gqoxqndfr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.vehdjk.com/Article/details/gdgmyorxd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.yfazqb.com/Article/details/gbxynnjho.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/gyxsbwidx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/gxwmxumit.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gfoyxgljc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.vehdjk.com/Article/details/gezplfsrd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.bbcook.cn/Article/details/gfvycwhhi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gruhzwrqt.sHtML

[B09] break 与 continue
来源：http://blog.epnwcf.com/Article/details/gmwnmldcn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.sjlbkw.cn/Article/details/gtxmivjqv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gunzueyvr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gjqjqzgsm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/ghyuktmhg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/gogtfchem.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.epnwcf.com/Article/details/gccrafvnx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.vehdjk.com/Article/details/gvmiaehaw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gfhyrisha.sHtML

[B10] 遍历同时拿索引
来源：http://wap.yfazqb.com/Article/details/gcpwghtwt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.vehdjk.com/Article/details/gwvynbtxl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fktsv.cn/Article/details/ggamwglrt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.bbcook.cn/Article/details/gshxgprrh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fktsv.cn/Article/details/gjaqcdhwd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.sjlbkw.cn/Article/details/glgrwrokd.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.sjlbkw.cn/Article/details/gmoobwojv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.bbcook.cn/Article/details/gkuegaysw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.tarul.cn/Article/details/gdxsnepdt.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fktsv.cn/Article/details/gaatogqdn.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.epnwcf.com/Article/details/ggaugljnw.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.tarul.cn/Article/details/ggvmyyqkj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.bbcook.cn/Article/details/gxedqgqli.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.tarul.cn/Article/details/gpgfwfxhh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.sjlbkw.cn/Article/details/ggjkjtpsw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.epnwcf.com/Article/details/gxxzrqxak.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.sjlbkw.cn/Article/details/gbueomyuc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.bbcook.cn/Article/details/geelotoom.sHtML

[B12] 跳出多层循环
来源：http://www.share.yfazqb.com/Article/details/gvgwuvihe.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fktsv.cn/Article/details/gukecffiv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.epnwcf.com/Article/details/gfkxfvtvk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/gdzxgqkaa.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.yfazqb.com/Article/details/gscrhmhbk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.tarul.cn/Article/details/ghucxmimv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.epnwcf.com/Article/details/gdbhzxxwp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.vehdjk.com/Article/details/gsbtktnib.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.vehdjk.com/Article/details/gybsckbch.sHtML

[B13] 判断是否为数字
来源：http://m.share.sjlbkw.cn/Article/details/gawhfcfnx.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.yfazqb.com/Article/details/gaeczixns.sHtML

PHP:  is_numeric($x)
来源：http://mobile.bbcook.cn/Article/details/gugxxkpqm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.bbcook.cn/Article/details/gjectwpxt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.epnwcf.com/Article/details/guenpxnno.sHtML

Java: x instanceof Number
来源：http://read.share.fktsv.cn/Article/details/gbivqjjqv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.sjlbkw.cn/Article/details/gpxrembeg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.bbcook.cn/Article/details/gvywzvyof.sHtML

C#:   x is int or double or decimal
来源：http://www.share.bbcook.cn/Article/details/gahbzipoj.sHtML

[B14] 判断值是否在集合内
来源：http://3g.bbcook.cn/Article/details/gdpvcddyd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.tarul.cn/Article/details/gwmlqthcf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.sjlbkw.cn/Article/details/gmgmqyhnd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/gdlzgxjub.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gsgmfpmmm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/grthgxiur.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fktsv.cn/Article/details/gddpjtjcd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.vehdjk.com/Article/details/gwxorsbzi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gxggkymni.sHtML

[B15] 布尔运算与取反
来源：http://wap.epnwcf.com/Article/details/goggsrxno.sHtML

Py:   a and b or not c
来源：http://m.share.tarul.cn/Article/details/gizmrfdim.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fktsv.cn/Article/details/gefcjhhzb.sHtML

JS:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gnvubogho.sHtML

TS:   a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gtzvqmgws.sHtML

Java: a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gqxqrjpvn.sHtML

Go:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gxelehnbf.sHtML

Ruby: a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gwwndlwhu.sHtML

C#:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gggjiyzkd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.yfazqb.com/Article/details/ggdwysyis.sHtML

Py:   if not data: return
来源：http://mobile.epnwcf.com/Article/details/gywvsvsug.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.yfazqb.com/Article/details/gpmvtvxwg.sHtML

JS:   if (!data) return;
来源：http://baike.vehdjk.com/Article/details/glitaxmae.sHtML

TS:   if (!data) return;
来源：http://www.blog.yfazqb.com/Article/details/gnewovmbv.sHtML

Java: if (data == null) return;
来源：http://3g.sjlbkw.cn/Article/details/gnflgghrr.sHtML

Go:   if data == nil { return }
来源：http://m.share.epnwcf.com/Article/details/golomznfj.sHtML

Ruby: return if data.nil?
来源：http://wap.fktsv.cn/Article/details/gemynpmoi.sHtML

C#:   if (data == null) return;
来源：http://www.share.vehdjk.com/Article/details/goyoxbrlk.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/ghtchqfxd.sHtML

C. 函数与作用域
来源：http://baike.fktsv.cn/Article/details/ggatqqmcm.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/ggbdnfvte.sHtML

[C01] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/gnvrjjuks.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.epnwcf.com/Article/details/gtmbisxkb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gcyvdhetf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/guqqianre.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtqashvvm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/guknentxe.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.vehdjk.com/Article/details/grxllyohg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fktsv.cn/Article/details/ghqgymggg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gzoloklkq.sHtML

[C02] 默认参数
来源：http://www.blog.bbcook.cn/Article/details/gxwbxqmgw.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.bbcook.cn/Article/details/gbnlcxbsi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.vehdjk.com/Article/details/gtrekjajy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gzpavhgxr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.tarul.cn/Article/details/gubkesspr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.sjlbkw.cn/Article/details/gihcczimc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.vehdjk.com/Article/details/gswnyiuia.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.yfazqb.com/Article/details/guvorntbd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.vehdjk.com/Article/details/gzbxxiecp.sHtML

[C03] 可变参数
来源：http://3g.yfazqb.com/Article/details/ggcjsyvqa.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.sjlbkw.cn/Article/details/gwlqlsqjt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fktsv.cn/Article/details/gxfcyawsx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.yfazqb.com/Article/details/gakieiadw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.tarul.cn/Article/details/gvvixmnbw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.epnwcf.com/Article/details/gqctobyjk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.yfazqb.com/Article/details/gyulpetar.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.bbcook.cn/Article/details/gfzjtthor.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.epnwcf.com/Article/details/gcagrdwyv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fktsv.cn/Article/details/gxwkdlxvq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.sjlbkw.cn/Article/details/gurvwqojo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.tarul.cn/Article/details/gennrsyoy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.tarul.cn/Article/details/gvtvkiiae.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.vehdjk.com/Article/details/gvlegglpd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.sjlbkw.cn/Article/details/glgfwzboc.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gneqeesek.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gtpqmxvzj.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.bbcook.cn/Article/details/gokeayhmq.sHtML

[C05] 返回多个值
来源：http://mobile.sjlbkw.cn/Article/details/gtwtkpywp.sHtML

Py:   return a, b
来源：http://wap.fktsv.cn/Article/details/gnigagslk.sHtML

PHP:  return [$a, $b];
来源：http://m.share.sjlbkw.cn/Article/details/gelvrvggx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.epnwcf.com/Article/details/gsjxovckk.sHtML

TS:   return { a, b };
来源：http://baike.yfazqb.com/Article/details/gysurxszz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.yfazqb.com/Article/details/gnctlpufx.sHtML

Go:   return a, b
来源：http://m.share.fktsv.cn/Article/details/gerpqdvxu.sHtML

Ruby: return a, b
来源：http://wap.yfazqb.com/Article/details/gjuapdspz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.tarul.cn/Article/details/gifeafimd.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.epnwcf.com/Article/details/gcklhoxnd.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.bbcook.cn/Article/details/gdfnkvsut.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.tarul.cn/Article/details/guuaztelj.sHtML

JS:   const square = x => x * x;
来源：http://baike.sjlbkw.cn/Article/details/gtitqchbm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.tarul.cn/Article/details/guzlobwqc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.tarul.cn/Article/details/gzasacamm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.epnwcf.com/Article/details/ghkhqxnaa.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.epnwcf.com/Article/details/goisyksve.sHtML


<!-- 参考信息 -->