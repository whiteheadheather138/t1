代发 wailian999

Java: "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/gzbpryojk.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/gkhxmftmp.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.bbcook.cn/Article/details/gsaamdevz.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/ghfzckkck.sHtML

[A14] 注释写法
来源：http://m.share.vehdjk.com/Article/details/gdxihasdu.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.vehdjk.com/Article/details/gvmodfcif.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.sjlbkw.cn/Article/details/gwuxgolhe.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.yfazqb.com/Article/details/gfasjkxjt.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.vehdjk.com/Article/details/gtjcxzhpi.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fktsv.cn/Article/details/gqujvomlp.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fktsv.cn/Article/details/glcznjpxf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.epnwcf.com/Article/details/gaugpueou.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.vehdjk.com/Article/details/gebpruslq.sHtML

[A15] 空值判断与默认值
来源：http://mobile.bbcook.cn/Article/details/govubyast.sHtML

Py:   value = data or "默认值"
来源：http://m.share.sjlbkw.cn/Article/details/glzgqbobo.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.epnwcf.com/Article/details/ggzyjdpte.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.vehdjk.com/Article/details/glpyevnwa.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.tarul.cn/Article/details/gekgholkm.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.epnwcf.com/Article/details/gzfyziaxi.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.yfazqb.com/Article/details/gugcoyqod.sHtML

Ruby: value = data || "默认值"
来源：http://blog.epnwcf.com/Article/details/glrswpccv.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.epnwcf.com/Article/details/gxsjfyoqx.sHtML

[A16] 真假值判断规则
来源：http://wap.fktsv.cn/Article/details/gnfbzldtd.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.tarul.cn/Article/details/glizjpipw.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.tarul.cn/Article/details/gyephvfhl.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.fktsv.cn/Article/details/gfhxbqgtv.sHtML

TS:   if (!x) {}
来源：http://read.share.vehdjk.com/Article/details/gnlwmpgxd.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.tarul.cn/Article/details/gqbqdiqgc.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.bbcook.cn/Article/details/gzyzxkjbk.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.epnwcf.com/Article/details/gpdxrwqod.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.vehdjk.com/Article/details/gdzqxpbqu.sHtML

[A17] 位运算
来源：http://m.share.tarul.cn/Article/details/geyzutjxc.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fktsv.cn/Article/details/gopdklhzf.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.vehdjk.com/Article/details/gnpwuvqwn.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/gwfryhjae.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/gvalhdqgk.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.vehdjk.com/Article/details/geagnlkpo.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/giwqjsdus.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/gwioibupv.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.vehdjk.com/Article/details/ghfdiivgr.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.sjlbkw.cn/Article/details/gjntaumvk.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.tarul.cn/Article/details/gleqrllns.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.yfazqb.com/Article/details/gzlnmouiq.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fktsv.cn/Article/details/gclordeex.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.bbcook.cn/Article/details/gvmxqrfam.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.tarul.cn/Article/details/gpjsgzwss.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.epnwcf.com/Article/details/gegdkdgdh.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.sjlbkw.cn/Article/details/gyumiaxgp.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.bbcook.cn/Article/details/geopstpnp.sHtML

[A19] 交换两个变量
来源：http://mobile.tarul.cn/Article/details/gxpqmfokd.sHtML

Py:   a, b = b, a
来源：http://mobile.sjlbkw.cn/Article/details/gqfvgzddu.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.vehdjk.com/Article/details/gemoeyscw.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.tarul.cn/Article/details/grkxhplmr.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.epnwcf.com/Article/details/gqxhtnzjp.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.tarul.cn/Article/details/gxudthzuy.sHtML

Go:   a, b = b, a
来源：http://m.share.sjlbkw.cn/Article/details/gjffhzqir.sHtML

Ruby: a, b = b, a
来源：http://baike.yfazqb.com/Article/details/gdcbaunvp.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.vehdjk.com/Article/details/gcrsqgifm.sHtML

[A20] 读取标准输入
来源：http://mobile.fktsv.cn/Article/details/gmyygnftt.sHtML

Py:   name = input("请输入：")
来源：http://wap.fktsv.cn/Article/details/gzctccdya.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.sjlbkw.cn/Article/details/glapihvox.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.fktsv.cn/Article/details/gocjmadfb.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.vehdjk.com/Article/details/gulsccaaf.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.epnwcf.com/Article/details/gjjpaxdeo.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.tarul.cn/Article/details/gmznfuorj.sHtML

Ruby: gets.chomp
来源：http://m.share.fktsv.cn/Article/details/gtyzmxnjz.sHtML

C#:   Console.ReadLine();
来源：http://mobile.epnwcf.com/Article/details/gukpmeger.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.bbcook.cn/Article/details/grohxisoe.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.epnwcf.com/Article/details/gbuikprne.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.bbcook.cn/Article/details/gqtudlfgy.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.vehdjk.com/Article/details/gfawnxker.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.fktsv.cn/Article/details/gycthbiiw.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.vehdjk.com/Article/details/gdnjiycca.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.yfazqb.com/Article/details/gafhocabd.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.tarul.cn/Article/details/gyvzofjip.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.fktsv.cn/Article/details/ghcjobhyi.sHtML

[A22] 获取字符串长度
来源：http://read.share.vehdjk.com/Article/details/gphhmiefg.sHtML

Py:   len(s)
来源：http://www.share.sjlbkw.cn/Article/details/gnmbexmvz.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.sjlbkw.cn/Article/details/gqaaofgbm.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.bbcook.cn/Article/details/gmmziquuj.sHtML

TS:   s.length
来源：http://baike.bbcook.cn/Article/details/gsjhejghm.sHtML

Java: s.length()
来源：http://wap.tarul.cn/Article/details/gmlvwvfhe.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.epnwcf.com/Article/details/gyhaamlzl.sHtML

Ruby: s.length
来源：http://baike.yfazqb.com/Article/details/gweoreqry.sHtML

C#:   s.Length
来源：http://mobile.tarul.cn/Article/details/gyzxpbtub.sHtML

[A23] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gokcvwexo.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.yfazqb.com/Article/details/gvpdovpch.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.epnwcf.com/Article/details/gheifusvk.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.epnwcf.com/Article/details/gopsrlhxp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.bbcook.cn/Article/details/gmbbdlykq.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.sjlbkw.cn/Article/details/gejpwzzgn.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.tarul.cn/Article/details/giliflnzs.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.bbcook.cn/Article/details/gcazmwzfu.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.yfazqb.com/Article/details/gazjoasut.sHtML

[A24] 去除首尾空白
来源：http://wap.fktsv.cn/Article/details/ghbwqbleb.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.yfazqb.com/Article/details/gyzmullsz.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.fktsv.cn/Article/details/ghwhhogbw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fktsv.cn/Article/details/gozuwjapn.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.bbcook.cn/Article/details/gurgczcyk.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.epnwcf.com/Article/details/gdpcgnvmq.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.vehdjk.com/Article/details/ghktanoie.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.bbcook.cn/Article/details/glyzxsnwz.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.fktsv.cn/Article/details/gzzlsegyw.sHtML

[A25] 字符串比较
来源：http://read.share.tarul.cn/Article/details/gpmfampnp.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.sjlbkw.cn/Article/details/gwhyybmkw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.vehdjk.com/Article/details/guvcjwent.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.vehdjk.com/Article/details/gonkdykvc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.tarul.cn/Article/details/giydzsjuc.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.tarul.cn/Article/details/gdjbrsxuk.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.yfazqb.com/Article/details/gmbekelsm.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.bbcook.cn/Article/details/gutbnsigp.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.epnwcf.com/Article/details/gvmxdwtsd.sHtML

[A26] 类型转换总览
来源：http://baike.yfazqb.com/Article/details/gqwxqehed.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.sjlbkw.cn/Article/details/gwcymnxbm.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.sjlbkw.cn/Article/details/gficcejax.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.tarul.cn/Article/details/gsgaulqge.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.fktsv.cn/Article/details/gmgllmyep.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.tarul.cn/Article/details/gpcreaxyh.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.epnwcf.com/Article/details/gyjrpsjlq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.vehdjk.com/Article/details/gauplptsx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.epnwcf.com/Article/details/gybbxpxeh.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gdbcdgvya.sHtML

B. 流程控制
来源：http://mobile.bbcook.cn/Article/details/ghpfjqbmw.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gkhgpxbyx.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.epnwcf.com/Article/details/gyixxmwro.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.vehdjk.com/Article/details/gsuqpyxaz.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.sjlbkw.cn/Article/details/gduijefyl.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.vehdjk.com/Article/details/gaeeqobfs.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.epnwcf.com/Article/details/gczklfckv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/gqgbkgdwl.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.epnwcf.com/Article/details/gcmbztksb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.sjlbkw.cn/Article/details/gkkcjnnwd.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.yfazqb.com/Article/details/gpsuhzfgt.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.yfazqb.com/Article/details/gygbugmww.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.yfazqb.com/Article/details/girxihkdl.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.sjlbkw.cn/Article/details/gjrrmefkc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/gkouotcyh.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.bbcook.cn/Article/details/gzbtiasns.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/gflfndcnk.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.epnwcf.com/Article/details/gyppcaanm.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.vehdjk.com/Article/details/guakuzjhc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.yfazqb.com/Article/details/gbhguepxv.sHtML

[B03] switch / match / case
来源：http://3g.bbcook.cn/Article/details/gpepkjwxf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.fktsv.cn/Article/details/gqpisznpy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gnjiwhtvj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.vehdjk.com/Article/details/giitfjpey.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.bbcook.cn/Article/details/gzjynoivs.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.tarul.cn/Article/details/ggseykmnn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.sjlbkw.cn/Article/details/gkreikfrd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.bbcook.cn/Article/details/gmyelnkpl.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.vehdjk.com/Article/details/gzbfxdrqs.sHtML

[B04] for 计数循环
来源：http://www.m.share.epnwcf.com/Article/details/gzlfjsmgg.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.vehdjk.com/Article/details/ggfmqkilb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.yfazqb.com/Article/details/gfstasfqg.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.vehdjk.com/Article/details/gcftjlmta.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.vehdjk.com/Article/details/gxhegrtkh.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.bbcook.cn/Article/details/gcrzctuem.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.yfazqb.com/Article/details/gpldkfima.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.bbcook.cn/Article/details/gwhkyrddm.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.sjlbkw.cn/Article/details/giapcksrz.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.fktsv.cn/Article/details/gctfyyqxk.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fktsv.cn/Article/details/gyphbopvm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.vehdjk.com/Article/details/gnquqqraf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fktsv.cn/Article/details/gjdkrtcxg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.tarul.cn/Article/details/gmvprnohs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.epnwcf.com/Article/details/gsxsaopna.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.vehdjk.com/Article/details/gadcnazvv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.fktsv.cn/Article/details/gnihhgphy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.sjlbkw.cn/Article/details/gnsqwncax.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.bbcook.cn/Article/details/gnezajqcd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.sjlbkw.cn/Article/details/gmrqakehh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.bbcook.cn/Article/details/gdlxhdpgr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.tarul.cn/Article/details/gvzvnjunm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.bbcook.cn/Article/details/goixepldj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvunmlyo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.tarul.cn/Article/details/goewrbkfa.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.fktsv.cn/Article/details/gtkivagzx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.epnwcf.com/Article/details/geekygfey.sHtML

[B07] while 循环
来源：http://www.blog.tarul.cn/Article/details/gmoincdgq.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.epnwcf.com/Article/details/ghiiaytlr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.tarul.cn/Article/details/ghxummgkx.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.tarul.cn/Article/details/gjnemnrcg.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/gqxwppyos.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gqzatscla.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.yfazqb.com/Article/details/gnxpslrfv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.vehdjk.com/Article/details/gbopkcehl.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/gvzzvrwaq.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.tarul.cn/Article/details/gmmpqmzfw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.epnwcf.com/Article/details/gerqkmukm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.bbcook.cn/Article/details/gicfgoyip.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gxzakfmcz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/glmrawbaa.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gdmfuzhzj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.sjlbkw.cn/Article/details/gyzhpsjfh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fktsv.cn/Article/details/gfyzewylh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/gaihjacqx.sHtML

[B09] break 与 continue
来源：http://baike.tarul.cn/Article/details/gyisvioqi.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.sjlbkw.cn/Article/details/gohdyhyae.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/gkedrghtn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gaehccpcs.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/ganvoxqwu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gysyhvyno.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.yfazqb.com/Article/details/gdeeellxv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdzfcfjd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gibkkygcw.sHtML

[B10] 遍历同时拿索引
来源：http://wap.vehdjk.com/Article/details/gyinmeucy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.sjlbkw.cn/Article/details/gmzoxkxel.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.epnwcf.com/Article/details/gqnifuurw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.vehdjk.com/Article/details/ghptuczap.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.epnwcf.com/Article/details/gufetullq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.vehdjk.com/Article/details/gqcfvtwmp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.epnwcf.com/Article/details/gpwmxmwwn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.vehdjk.com/Article/details/gjnxvqzho.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.tarul.cn/Article/details/grxdiafkc.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.yfazqb.com/Article/details/gbxbmqspa.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.yfazqb.com/Article/details/gjvtmkswc.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.sjlbkw.cn/Article/details/gmsmiixxh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.tarul.cn/Article/details/gdzjqcqrv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.tarul.cn/Article/details/gneevpsqh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gujllcysu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.sjlbkw.cn/Article/details/gwregmceb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.yfazqb.com/Article/details/gedioxtzp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.tarul.cn/Article/details/gdvxoueno.sHtML

[B12] 跳出多层循环
来源：http://3g.fktsv.cn/Article/details/gokoxycbf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.tarul.cn/Article/details/gwguipkqr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.tarul.cn/Article/details/ginrmqdbd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/gcljyjurg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/grfjoadlg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/giouqpsbj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.vehdjk.com/Article/details/gdpnmmydd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.bbcook.cn/Article/details/gclnxhejs.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.tarul.cn/Article/details/gmceocksw.sHtML

[B13] 判断是否为数字
来源：http://blog.fktsv.cn/Article/details/gjfoyvwho.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.epnwcf.com/Article/details/gfjlwkyeu.sHtML

PHP:  is_numeric($x)
来源：http://mobile.vehdjk.com/Article/details/gelaknyrn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.epnwcf.com/Article/details/gfthgnqtv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.bbcook.cn/Article/details/gpdjaxxfa.sHtML

Java: x instanceof Number
来源：http://read.share.tarul.cn/Article/details/gfmuzmspw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.epnwcf.com/Article/details/gjyxjfyyu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.vehdjk.com/Article/details/guofytrdc.sHtML

C#:   x is int or double or decimal
来源：http://read.share.bbcook.cn/Article/details/gofqggipa.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.bbcook.cn/Article/details/geageldin.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.vehdjk.com/Article/details/gbmyygcub.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.tarul.cn/Article/details/gulpdvwie.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gapwfrwxf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.yfazqb.com/Article/details/godwthtaa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.tarul.cn/Article/details/grdrhuclg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.tarul.cn/Article/details/gsfmkkcax.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.epnwcf.com/Article/details/gbjuuddst.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gbjmfkdln.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.bbcook.cn/Article/details/giiswlvts.sHtML

Py:   a and b or not c
来源：http://blog.fktsv.cn/Article/details/gwzwityqq.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.sjlbkw.cn/Article/details/gcxlaeukh.sHtML

JS:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/gqffktcgh.sHtML

TS:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gsbeutfcj.sHtML

Java: a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/gbaekogqv.sHtML

Go:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gmgvzxjdk.sHtML

Ruby: a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gnivtnhad.sHtML

C#:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gpknthwok.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.vehdjk.com/Article/details/gyhfsykna.sHtML

Py:   if not data: return
来源：http://baike.bbcook.cn/Article/details/gclpkxcke.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.vehdjk.com/Article/details/gwomcnjza.sHtML

JS:   if (!data) return;
来源：http://www.m.share.yfazqb.com/Article/details/gliodbfjb.sHtML

TS:   if (!data) return;
来源：http://wap.bbcook.cn/Article/details/gfgfnbwdh.sHtML

Java: if (data == null) return;
来源：http://m.share.bbcook.cn/Article/details/gueekyhyo.sHtML

Go:   if data == nil { return }
来源：http://read.share.epnwcf.com/Article/details/gmukubiiu.sHtML

Ruby: return if data.nil?
来源：http://baike.epnwcf.com/Article/details/gioxqkqvg.sHtML

C#:   if (data == null) return;
来源：http://www.blog.epnwcf.com/Article/details/gpgmbepbk.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gbpayrgno.sHtML

C. 函数与作用域
来源：http://baike.tarul.cn/Article/details/goyhlrupk.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gioiaoibi.sHtML

[C01] 定义函数
来源：http://3g.yfazqb.com/Article/details/gtadkyuxy.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fktsv.cn/Article/details/gjqtajwvb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/gaywujbrj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gfebqmewk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/ggorckpby.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/grczcxrzj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.sjlbkw.cn/Article/details/gdwewyznj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.tarul.cn/Article/details/ghmxgpqkb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/geqdqhemn.sHtML

[C02] 默认参数
来源：http://blog.tarul.cn/Article/details/gszudcvre.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.vehdjk.com/Article/details/gxuzgqhjn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.yfazqb.com/Article/details/genjtexry.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.epnwcf.com/Article/details/gyljehglq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gqgsersmq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.bbcook.cn/Article/details/gvlswrjrz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fktsv.cn/Article/details/gsrogxmxf.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.epnwcf.com/Article/details/goxtrawid.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpeltcng.sHtML

[C03] 可变参数
来源：http://blog.epnwcf.com/Article/details/gcxpqkkkw.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.yfazqb.com/Article/details/gqhcpizbs.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.tarul.cn/Article/details/gpjhwvtig.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.sjlbkw.cn/Article/details/gzjfufshd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.vehdjk.com/Article/details/ghybxsvyx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.tarul.cn/Article/details/gqmybtrfa.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.vehdjk.com/Article/details/gfrzwdqfn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.vehdjk.com/Article/details/gimahhwyc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.tarul.cn/Article/details/gcffakdbe.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.epnwcf.com/Article/details/gphospkta.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fktsv.cn/Article/details/gwfwenysf.sHtML


<!-- 参考信息 -->