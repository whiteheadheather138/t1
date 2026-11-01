代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.fktsv.cn/Article/details/gabffbiem.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.tarul.cn/Article/details/gbstrcctw.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.fktsv.cn/Article/details/gnfmwrijq.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.yfazqb.com/Article/details/gvirzhhfo.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.vehdjk.com/Article/details/gywkzisqq.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.yfazqb.com/Article/details/gbedcnsrc.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.sjlbkw.cn/Article/details/gkibeshuz.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.vehdjk.com/Article/details/ginfjcycx.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.bbcook.cn/Article/details/gyvcwjdfg.sHtML

Go:   "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gmmvypvvo.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/gfaivcdwm.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.vehdjk.com/Article/details/glihmttti.sHtML

[A14] 注释写法
来源：http://www.blog.sjlbkw.cn/Article/details/girsjgzic.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.bbcook.cn/Article/details/gvvybdamy.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.yfazqb.com/Article/details/gbeojdqkn.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.fktsv.cn/Article/details/gaetbmvvv.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.sjlbkw.cn/Article/details/gulaxxjgz.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.bbcook.cn/Article/details/gjybzorkp.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.epnwcf.com/Article/details/grknslaee.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.tarul.cn/Article/details/gmrlyapbo.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.tarul.cn/Article/details/gkamyjcqc.sHtML

[A15] 空值判断与默认值
来源：http://wap.tarul.cn/Article/details/gnhjfrxlq.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.vehdjk.com/Article/details/gzsltoiwr.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.tarul.cn/Article/details/gzaddgfhi.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.sjlbkw.cn/Article/details/gkssgrxzg.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.epnwcf.com/Article/details/grsboceob.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.sjlbkw.cn/Article/details/gjokzyphh.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.yfazqb.com/Article/details/ggprdicyi.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.bbcook.cn/Article/details/gdwgjmkrm.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.tarul.cn/Article/details/gcfwubogq.sHtML

[A16] 真假值判断规则
来源：http://mobile.yfazqb.com/Article/details/ghzovwvmj.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.fktsv.cn/Article/details/ghxfaurhp.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.epnwcf.com/Article/details/ggocjetfp.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.fktsv.cn/Article/details/giqipybiy.sHtML

TS:   if (!x) {}
来源：http://mobile.yfazqb.com/Article/details/gzrgbkkgi.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.fktsv.cn/Article/details/gyfowwwyn.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.vehdjk.com/Article/details/gfdyjgxye.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.fktsv.cn/Article/details/gpwgumpqt.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.sjlbkw.cn/Article/details/grzqrxqic.sHtML

[A17] 位运算
来源：http://mobile.yfazqb.com/Article/details/gczqubjcg.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/geslavfbi.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.tarul.cn/Article/details/ggyztzmeq.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/gzxlntjxz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/gqcrcovwm.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/giyiezvpr.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.epnwcf.com/Article/details/gccgwffyp.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.sjlbkw.cn/Article/details/gqvyekvjl.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.bbcook.cn/Article/details/gqvvuaptc.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.epnwcf.com/Article/details/gqtqvvvmp.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fktsv.cn/Article/details/gbdscsrmz.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.fktsv.cn/Article/details/gntgelldz.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.tarul.cn/Article/details/gtmirqlmw.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.fktsv.cn/Article/details/gsxexjbrq.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.yfazqb.com/Article/details/gxgagjzfq.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.fktsv.cn/Article/details/geicjvkjc.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.epnwcf.com/Article/details/gtmpwamvh.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.tarul.cn/Article/details/geplgfyhx.sHtML

[A19] 交换两个变量
来源：http://read.share.sjlbkw.cn/Article/details/gmobqeskm.sHtML

Py:   a, b = b, a
来源：http://read.share.bbcook.cn/Article/details/gsgmdezlx.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.epnwcf.com/Article/details/gvlecuxyu.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.bbcook.cn/Article/details/gfknpbopj.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.fktsv.cn/Article/details/gvwivkoew.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.fktsv.cn/Article/details/gbokrltdb.sHtML

Go:   a, b = b, a
来源：http://mobile.vehdjk.com/Article/details/ghagyyuop.sHtML

Ruby: a, b = b, a
来源：http://baike.sjlbkw.cn/Article/details/gpvcqdjkt.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.sjlbkw.cn/Article/details/glcgpsmit.sHtML

[A20] 读取标准输入
来源：http://m.share.fktsv.cn/Article/details/grjhfurmf.sHtML

Py:   name = input("请输入：")
来源：http://m.share.fktsv.cn/Article/details/gvukwwpwz.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.tarul.cn/Article/details/giexfmvne.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.yfazqb.com/Article/details/gfjczauki.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.tarul.cn/Article/details/gfmfsdlip.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.yfazqb.com/Article/details/ggkfquiey.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.fktsv.cn/Article/details/goufqrqdf.sHtML

Ruby: gets.chomp
来源：http://www.blog.yfazqb.com/Article/details/gmwhqkhrp.sHtML

C#:   Console.ReadLine();
来源：http://blog.epnwcf.com/Article/details/gkzwctnrx.sHtML

[A21] 保留指定小数位输出
来源：http://blog.sjlbkw.cn/Article/details/gpgjuwapd.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.tarul.cn/Article/details/gbrhqmtaf.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.bbcook.cn/Article/details/guxajeund.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.vehdjk.com/Article/details/gsrlzotaq.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.fktsv.cn/Article/details/gffwtaytn.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.fktsv.cn/Article/details/gtuoijjvi.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.yfazqb.com/Article/details/gvmdbxdex.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.fktsv.cn/Article/details/gmnxgcpql.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.fktsv.cn/Article/details/gdbyplvmj.sHtML

[A22] 获取字符串长度
来源：http://read.share.tarul.cn/Article/details/gkudblcmc.sHtML

Py:   len(s)
来源：http://www.blog.bbcook.cn/Article/details/glmrcbyvz.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.yfazqb.com/Article/details/gswolsfor.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.fktsv.cn/Article/details/gmonrqrln.sHtML

TS:   s.length
来源：http://blog.epnwcf.com/Article/details/ghwiblosm.sHtML

Java: s.length()
来源：http://3g.fktsv.cn/Article/details/guwhszzdy.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.sjlbkw.cn/Article/details/gswlupiyk.sHtML

Ruby: s.length
来源：http://baike.tarul.cn/Article/details/glpqmhgkb.sHtML

C#:   s.Length
来源：http://baike.sjlbkw.cn/Article/details/gitesuoei.sHtML

[A23] 大小写转换
来源：http://m.share.sjlbkw.cn/Article/details/gnrqdzmtc.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.fktsv.cn/Article/details/gtywywdtf.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.tarul.cn/Article/details/gumrmsndq.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.bbcook.cn/Article/details/ggidwdicf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.sjlbkw.cn/Article/details/gpusdtuid.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.bbcook.cn/Article/details/gzdfrzosi.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.sjlbkw.cn/Article/details/gcwnkpbfj.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.vehdjk.com/Article/details/goyqvkyyd.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.yfazqb.com/Article/details/glqjwdnzn.sHtML

[A24] 去除首尾空白
来源：http://www.blog.epnwcf.com/Article/details/gjlmloojo.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.epnwcf.com/Article/details/gnmglkgdd.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.fktsv.cn/Article/details/geklryxwn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.epnwcf.com/Article/details/geidakgul.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.epnwcf.com/Article/details/gheyyxyjb.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.bbcook.cn/Article/details/gmfkbpxfz.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.tarul.cn/Article/details/gshspnttq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.yfazqb.com/Article/details/gqiuqjvmk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.yfazqb.com/Article/details/geuffpsmj.sHtML

[A25] 字符串比较
来源：http://www.m.share.fktsv.cn/Article/details/gjtxqcxao.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.fktsv.cn/Article/details/gbyekdlxy.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fktsv.cn/Article/details/ghmrelpgh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.bbcook.cn/Article/details/gssjavean.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fktsv.cn/Article/details/ghvwgafbk.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.vehdjk.com/Article/details/gqlipvyiw.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.vehdjk.com/Article/details/guejyodma.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.sjlbkw.cn/Article/details/gktypmptl.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.tarul.cn/Article/details/ghkfssajh.sHtML

[A26] 类型转换总览
来源：http://read.share.vehdjk.com/Article/details/gbmrhwosv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.tarul.cn/Article/details/gsrqusfna.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghrpkeyvq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.yfazqb.com/Article/details/gtcutqhmx.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.tarul.cn/Article/details/gthdmzhvo.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.vehdjk.com/Article/details/gjdwrwohx.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.epnwcf.com/Article/details/gqmlennxc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.fktsv.cn/Article/details/gwndqfzia.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.bbcook.cn/Article/details/gcxrukvwr.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gbuixldew.sHtML

B. 流程控制
来源：http://3g.epnwcf.com/Article/details/geijkxewv.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gpewvqunv.sHtML

[B01] 条件判断 if / else
来源：http://wap.bbcook.cn/Article/details/gmrlybqkt.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.yfazqb.com/Article/details/gmpxtxztv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.yfazqb.com/Article/details/gclsyvghv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.yfazqb.com/Article/details/gzpdumbyi.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/glkxnyxey.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.fktsv.cn/Article/details/glhkobhhe.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.yfazqb.com/Article/details/gpivogojv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.sjlbkw.cn/Article/details/ghlefpqpy.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fktsv.cn/Article/details/grsigwvml.sHtML

[B02] 多分支 else if / elif
来源：http://baike.yfazqb.com/Article/details/gmvwftlam.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fktsv.cn/Article/details/gykaswuto.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.bbcook.cn/Article/details/gewuiqjfv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/ggktrowiw.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhzmmqtz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/gfznvtbsx.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.epnwcf.com/Article/details/gruqqlssc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.tarul.cn/Article/details/glqupvzxf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/ggyccnctp.sHtML

[B03] switch / match / case
来源：http://3g.epnwcf.com/Article/details/gpywbtkvw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpgwkqet.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/glvluxpmm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.bbcook.cn/Article/details/giixsoakq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.bbcook.cn/Article/details/gbmmuxyqz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gfyfqowkg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.vehdjk.com/Article/details/gqtdxdugj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.tarul.cn/Article/details/geatpuzow.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.epnwcf.com/Article/details/gxzvqwfye.sHtML

[B04] for 计数循环
来源：http://3g.vehdjk.com/Article/details/ghyttcnnl.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.sjlbkw.cn/Article/details/gujfkclye.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.epnwcf.com/Article/details/goudyhlkf.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.tarul.cn/Article/details/gdcpetvhn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.sjlbkw.cn/Article/details/gjrvpyhay.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.sjlbkw.cn/Article/details/gitjrbccw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.bbcook.cn/Article/details/gokhtbehi.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.fktsv.cn/Article/details/gnybxauqr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.epnwcf.com/Article/details/ghwlhuphi.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.vehdjk.com/Article/details/grotalrws.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.epnwcf.com/Article/details/guqbmyawa.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.vehdjk.com/Article/details/gqlrlynft.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.epnwcf.com/Article/details/glgcoythx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.epnwcf.com/Article/details/gvmkgnktd.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.yfazqb.com/Article/details/gvokgdjru.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.tarul.cn/Article/details/gigdmjvuo.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.tarul.cn/Article/details/gzpwhbiye.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.sjlbkw.cn/Article/details/gnxesasxo.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fktsv.cn/Article/details/gbdjvlhfu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.bbcook.cn/Article/details/gdvrawjnr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.bbcook.cn/Article/details/gvuyftjdx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.epnwcf.com/Article/details/gkljziufi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.tarul.cn/Article/details/gtwaywxnn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.epnwcf.com/Article/details/gzpmminil.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.bbcook.cn/Article/details/gbebepfih.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.sjlbkw.cn/Article/details/gorarfdhu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.tarul.cn/Article/details/gflvetgcu.sHtML

[B07] while 循环
来源：http://www.blog.bbcook.cn/Article/details/gbgdmvzbg.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gsoebdzfv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtvzjaksz.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.yfazqb.com/Article/details/gsssoqyxw.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/gcvrfwwva.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gswvcifso.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.bbcook.cn/Article/details/gixqksint.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fktsv.cn/Article/details/gorenqtgy.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/gnydktppn.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fktsv.cn/Article/details/gczwlbigz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.bbcook.cn/Article/details/gkjymuxbv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fktsv.cn/Article/details/gxqnmlpqu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fktsv.cn/Article/details/gmjjrgjry.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gyfnxevbh.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.tarul.cn/Article/details/gvwrklddk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.bbcook.cn/Article/details/gxcayfjib.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.bbcook.cn/Article/details/guyhvlhex.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gfubdznew.sHtML

[B09] break 与 continue
来源：http://wap.bbcook.cn/Article/details/gxrvgfdua.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.sjlbkw.cn/Article/details/gpkyvcuis.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/glppjidge.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gcddpuouh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gnsyuxidm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/gbmgwklfc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.bbcook.cn/Article/details/gyhflzsvm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.yfazqb.com/Article/details/gdkuunfkl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/glmnfaamo.sHtML

[B10] 遍历同时拿索引
来源：http://3g.epnwcf.com/Article/details/gsaebmfau.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fktsv.cn/Article/details/gqobyvwmg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.epnwcf.com/Article/details/gregpidlj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.tarul.cn/Article/details/gyqguwovv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.epnwcf.com/Article/details/gifadhnln.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.sjlbkw.cn/Article/details/gndjejkkt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.bbcook.cn/Article/details/gdvvqdhff.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fktsv.cn/Article/details/gvibgulma.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.fktsv.cn/Article/details/gfwdbogur.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.vehdjk.com/Article/details/glbbmmuqw.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.bbcook.cn/Article/details/grivjjwht.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.tarul.cn/Article/details/guyuhbnvb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fktsv.cn/Article/details/gsulqwhef.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.bbcook.cn/Article/details/gffouprkt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fktsv.cn/Article/details/gnbtwkqch.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.epnwcf.com/Article/details/gyvapqaoq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.vehdjk.com/Article/details/gdjmklfre.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.epnwcf.com/Article/details/gmuzjzesx.sHtML

[B12] 跳出多层循环
来源：http://m.share.yfazqb.com/Article/details/gksahochy.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.bbcook.cn/Article/details/gdikcwzgq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.vehdjk.com/Article/details/gwncwcptz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fktsv.cn/Article/details/ggltthtmf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.yfazqb.com/Article/details/gqvetnkar.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.yfazqb.com/Article/details/gqcvbscyx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.tarul.cn/Article/details/gxacnlzmn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.bbcook.cn/Article/details/ghsbtffzk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fktsv.cn/Article/details/gfrptckch.sHtML

[B13] 判断是否为数字
来源：http://baike.tarul.cn/Article/details/gkkmzmqia.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.tarul.cn/Article/details/guotschrj.sHtML

PHP:  is_numeric($x)
来源：http://baike.tarul.cn/Article/details/gcrwmvnpa.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.tarul.cn/Article/details/gitwnomxj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.sjlbkw.cn/Article/details/gmpztnhkk.sHtML

Java: x instanceof Number
来源：http://mobile.bbcook.cn/Article/details/gxnvytdiv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.vehdjk.com/Article/details/gqmxezlen.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fktsv.cn/Article/details/gbxyptsqk.sHtML

C#:   x is int or double or decimal
来源：http://3g.bbcook.cn/Article/details/gfcdrgjsg.sHtML

[B14] 判断值是否在集合内
来源：http://blog.epnwcf.com/Article/details/ghkpiuuwt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.yfazqb.com/Article/details/gmrjbrmhp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.yfazqb.com/Article/details/gqlatvsbx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.epnwcf.com/Article/details/gugutnjwg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.epnwcf.com/Article/details/gkiikykun.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.yfazqb.com/Article/details/gmhcqlhhd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdqzzksg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fktsv.cn/Article/details/gxprrsncu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.tarul.cn/Article/details/gdhnxojlg.sHtML

[B15] 布尔运算与取反
来源：http://www.share.tarul.cn/Article/details/gdrxmcurv.sHtML

Py:   a and b or not c
来源：http://blog.yfazqb.com/Article/details/giswespkg.sHtML

PHP:  $a && $b || !$c
来源：http://3g.vehdjk.com/Article/details/gclzvfjxj.sHtML

JS:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gwmncksiu.sHtML

TS:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gfljycfhx.sHtML

Java: a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gdbedgtbr.sHtML

Go:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gsyfomhjj.sHtML

Ruby: a && b || !c
来源：http://read.share.tarul.cn/Article/details/gxuramuia.sHtML

C#:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gswjxulye.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.tarul.cn/Article/details/gwehlzele.sHtML

Py:   if not data: return
来源：http://mobile.vehdjk.com/Article/details/gfujglder.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.yfazqb.com/Article/details/gjyyscyok.sHtML

JS:   if (!data) return;
来源：http://m.share.fktsv.cn/Article/details/gxjdkiupf.sHtML

TS:   if (!data) return;
来源：http://www.blog.yfazqb.com/Article/details/gksfvhsey.sHtML

Java: if (data == null) return;
来源：http://www.blog.vehdjk.com/Article/details/gzafgqmdf.sHtML

Go:   if data == nil { return }
来源：http://baike.epnwcf.com/Article/details/gczpspcgd.sHtML

Ruby: return if data.nil?
来源：http://m.share.sjlbkw.cn/Article/details/gvtrzijpf.sHtML

C#:   if (data == null) return;
来源：http://m.share.vehdjk.com/Article/details/ggepdrqji.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gwsxkminf.sHtML

C. 函数与作用域
来源：http://www.share.sjlbkw.cn/Article/details/gwzdftmoz.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/ggagzaowo.sHtML

[C01] 定义函数
来源：http://m.share.vehdjk.com/Article/details/grrzdlkvt.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.epnwcf.com/Article/details/geemhefge.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gfsyybelm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gaunbxaci.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.tarul.cn/Article/details/gdrwtltgy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/guqgiqzxs.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.tarul.cn/Article/details/giassnuft.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.sjlbkw.cn/Article/details/gowvqutam.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gfmgwzali.sHtML

[C02] 默认参数
来源：http://baike.sjlbkw.cn/Article/details/giehfmuxw.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fktsv.cn/Article/details/gcsioscaq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.sjlbkw.cn/Article/details/gopolypkn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.bbcook.cn/Article/details/gjzinfnuf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gtjrgkcdo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.tarul.cn/Article/details/gjcduqnzl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.tarul.cn/Article/details/garwykvsh.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.yfazqb.com/Article/details/gvbaggjnp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.sjlbkw.cn/Article/details/gcaqpwynk.sHtML

[C03] 可变参数
来源：http://m.share.vehdjk.com/Article/details/gxswqdvgr.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.yfazqb.com/Article/details/gehdshqad.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.epnwcf.com/Article/details/ghxqysgnj.sHtML


<!-- 参考信息 -->