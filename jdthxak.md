代发 wailian999

[A14] 注释写法
来源：http://www.share.fktsv.cn/Article/details/gjlsyaxfv.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.epnwcf.com/Article/details/gguwthyqo.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.vehdjk.com/Article/details/gvhqgnwxf.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.vehdjk.com/Article/details/gsoucmkrb.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.epnwcf.com/Article/details/gddehimst.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.tarul.cn/Article/details/gegpxuxog.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.yfazqb.com/Article/details/gbkchlwnb.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.bbcook.cn/Article/details/gpakpqpoc.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.fktsv.cn/Article/details/ghdsxgkxs.sHtML

[A15] 空值判断与默认值
来源：http://wap.fktsv.cn/Article/details/gwxufegmk.sHtML

Py:   value = data or "默认值"
来源：http://wap.tarul.cn/Article/details/gqcnkyqch.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.vehdjk.com/Article/details/gcsicilkz.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fktsv.cn/Article/details/glrqdisvx.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.vehdjk.com/Article/details/ggoiisngk.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.bbcook.cn/Article/details/gwrgotgus.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.bbcook.cn/Article/details/gdamxifke.sHtML

Ruby: value = data || "默认值"
来源：http://blog.epnwcf.com/Article/details/glutverbb.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.tarul.cn/Article/details/gwdonrhuo.sHtML

[A16] 真假值判断规则
来源：http://blog.vehdjk.com/Article/details/gidkmlrpe.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.bbcook.cn/Article/details/gqassytlj.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.epnwcf.com/Article/details/gahfwejlv.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.sjlbkw.cn/Article/details/ggftdncmg.sHtML

TS:   if (!x) {}
来源：http://mobile.tarul.cn/Article/details/gizzbxxgr.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.fktsv.cn/Article/details/gbgtnkkle.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.tarul.cn/Article/details/gmzfncpgq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.tarul.cn/Article/details/gxvxblacg.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.tarul.cn/Article/details/gecwsszop.sHtML

[A17] 位运算
来源：http://mobile.vehdjk.com/Article/details/gtovcavsw.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvoimofw.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.yfazqb.com/Article/details/gpmecldeu.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.yfazqb.com/Article/details/gnycrlcfp.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gwihlmjmw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.bbcook.cn/Article/details/gxrcpktpi.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.tarul.cn/Article/details/gosqjyjwl.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.vehdjk.com/Article/details/gwezfzumv.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.yfazqb.com/Article/details/gvbusshqe.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.vehdjk.com/Article/details/ghqqnekcw.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.fktsv.cn/Article/details/gwyexnnwj.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.tarul.cn/Article/details/gokstvzpr.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.bbcook.cn/Article/details/gipijdvdz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.tarul.cn/Article/details/gjzutgduv.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.fktsv.cn/Article/details/gibnsbopv.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.bbcook.cn/Article/details/gecfykgfm.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.vehdjk.com/Article/details/gpkqknkeu.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.bbcook.cn/Article/details/gzlvwyoab.sHtML

[A19] 交换两个变量
来源：http://www.share.vehdjk.com/Article/details/ghbaylxpz.sHtML

Py:   a, b = b, a
来源：http://m.share.sjlbkw.cn/Article/details/glpamdaxk.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.epnwcf.com/Article/details/gjoweiprd.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.fktsv.cn/Article/details/gcnhzhtvf.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.sjlbkw.cn/Article/details/gsmymodps.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.epnwcf.com/Article/details/gpqrmhxwg.sHtML

Go:   a, b = b, a
来源：http://www.blog.yfazqb.com/Article/details/gomnqfxdp.sHtML

Ruby: a, b = b, a
来源：http://www.blog.bbcook.cn/Article/details/ghzkoecnj.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.yfazqb.com/Article/details/gbclswssn.sHtML

[A20] 读取标准输入
来源：http://read.share.sjlbkw.cn/Article/details/galaewbac.sHtML

Py:   name = input("请输入：")
来源：http://m.share.yfazqb.com/Article/details/gwrvdqmmt.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.epnwcf.com/Article/details/grwnimlgn.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.yfazqb.com/Article/details/ghpafbzgz.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.tarul.cn/Article/details/gaqmbbzic.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.fktsv.cn/Article/details/gmkuzquhg.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.tarul.cn/Article/details/gpqapwaxt.sHtML

Ruby: gets.chomp
来源：http://wap.yfazqb.com/Article/details/gziigjtda.sHtML

C#:   Console.ReadLine();
来源：http://wap.epnwcf.com/Article/details/gajgdcllx.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.epnwcf.com/Article/details/gxshrfzjs.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.sjlbkw.cn/Article/details/gzogzuuyb.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.epnwcf.com/Article/details/gmtnecxpy.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.tarul.cn/Article/details/gotvxvmuw.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.yfazqb.com/Article/details/gynwxmnlc.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.tarul.cn/Article/details/gfympbjls.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.vehdjk.com/Article/details/gvpgirkco.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.vehdjk.com/Article/details/gexkhwbtg.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.bbcook.cn/Article/details/ghybkpxtx.sHtML

[A22] 获取字符串长度
来源：http://m.share.yfazqb.com/Article/details/gtuapwjxr.sHtML

Py:   len(s)
来源：http://mobile.bbcook.cn/Article/details/gjdwueecj.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.bbcook.cn/Article/details/gxdafmqqs.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.tarul.cn/Article/details/gqgsjfysi.sHtML

TS:   s.length
来源：http://blog.bbcook.cn/Article/details/gzpbusqpg.sHtML

Java: s.length()
来源：http://m.share.fktsv.cn/Article/details/gsovkpfjh.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.tarul.cn/Article/details/gkjubxvhr.sHtML

Ruby: s.length
来源：http://www.blog.tarul.cn/Article/details/glcxpradi.sHtML

C#:   s.Length
来源：http://baike.epnwcf.com/Article/details/glrnlenmv.sHtML

[A23] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/gkokxlibz.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.fktsv.cn/Article/details/gdnipytes.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.epnwcf.com/Article/details/ggzysnfxc.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.yfazqb.com/Article/details/gzwtlzkuu.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.tarul.cn/Article/details/grbqzfujx.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.yfazqb.com/Article/details/gmahvvnbc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.tarul.cn/Article/details/gwwyvgrty.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.vehdjk.com/Article/details/gxcyekghb.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.fktsv.cn/Article/details/ghjrgoxpz.sHtML

[A24] 去除首尾空白
来源：http://blog.bbcook.cn/Article/details/grfisvsty.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.yfazqb.com/Article/details/gggcugdrs.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.vehdjk.com/Article/details/glyvkjedb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fktsv.cn/Article/details/gqxmitewz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.sjlbkw.cn/Article/details/giozeyccj.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fktsv.cn/Article/details/gbqfdayue.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.epnwcf.com/Article/details/gykvnwzjk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.sjlbkw.cn/Article/details/gxgxuhmgt.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.sjlbkw.cn/Article/details/gobnocjjh.sHtML

[A25] 字符串比较
来源：http://baike.tarul.cn/Article/details/gwjrcqjuw.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.bbcook.cn/Article/details/gdokrtgeh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.tarul.cn/Article/details/glgfzxjbz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.sjlbkw.cn/Article/details/gcdlgeupo.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.yfazqb.com/Article/details/gspiufclh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.epnwcf.com/Article/details/gkkdmsjse.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.sjlbkw.cn/Article/details/gbqiewzzy.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fktsv.cn/Article/details/gsngdovxu.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.epnwcf.com/Article/details/guxnnvkwn.sHtML

[A26] 类型转换总览
来源：http://wap.tarul.cn/Article/details/ggrmylxvh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.sjlbkw.cn/Article/details/gihjixzir.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.bbcook.cn/Article/details/gdhqwxgha.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.tarul.cn/Article/details/gsbfdiyca.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fktsv.cn/Article/details/gqpoigome.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.bbcook.cn/Article/details/gaufiwtsr.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.tarul.cn/Article/details/gjaceyrqd.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.fktsv.cn/Article/details/grcuqcjqd.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.sjlbkw.cn/Article/details/gygezgwxz.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gujidxduq.sHtML

B. 流程控制
来源：http://3g.vehdjk.com/Article/details/gzjrsbquh.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gzjviibfw.sHtML

[B01] 条件判断 if / else
来源：http://blog.sjlbkw.cn/Article/details/gqbnleogs.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.tarul.cn/Article/details/gxcsiykbe.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fktsv.cn/Article/details/gajxbqyok.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.bbcook.cn/Article/details/ggxcvmqkf.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/gvyewsgfw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.vehdjk.com/Article/details/gttbxzanc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.fktsv.cn/Article/details/gzykcmwpq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fktsv.cn/Article/details/gpixjzshu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/ggnvvrqrj.sHtML

[B02] 多分支 else if / elif
来源：http://wap.bbcook.cn/Article/details/gjjpegwbi.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.tarul.cn/Article/details/gsexrynns.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.bbcook.cn/Article/details/guindabip.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.yfazqb.com/Article/details/gjxnxxpwz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.yfazqb.com/Article/details/gymoumisq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/gtwznbnuc.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.tarul.cn/Article/details/gfgrnacfe.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.yfazqb.com/Article/details/gyorcztdb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.bbcook.cn/Article/details/gjzkypybn.sHtML

[B03] switch / match / case
来源：http://baike.sjlbkw.cn/Article/details/ggunmwgqe.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.bbcook.cn/Article/details/gxdfsqsjm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/gwjdykhnh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.yfazqb.com/Article/details/giqeukqlc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.vehdjk.com/Article/details/gagxuuuto.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.epnwcf.com/Article/details/guywgdssk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.epnwcf.com/Article/details/gsedaedll.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.tarul.cn/Article/details/gitbukhnq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fktsv.cn/Article/details/glibqbaaa.sHtML

[B04] for 计数循环
来源：http://blog.yfazqb.com/Article/details/gjiqmfbhf.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.sjlbkw.cn/Article/details/guitcdxnb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.epnwcf.com/Article/details/gbvyzfnkc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.bbcook.cn/Article/details/gcvnujhvl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fktsv.cn/Article/details/gqumjgxii.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.tarul.cn/Article/details/gnbzzaqju.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.tarul.cn/Article/details/gzbyogzwq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.sjlbkw.cn/Article/details/gaojdztjg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.sjlbkw.cn/Article/details/gvkehnxst.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.sjlbkw.cn/Article/details/gwldrryjq.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.epnwcf.com/Article/details/gynprieed.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.yfazqb.com/Article/details/guecppbbi.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.bbcook.cn/Article/details/glsrmkfvp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.vehdjk.com/Article/details/gerygfbof.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvyrjlgvn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.tarul.cn/Article/details/gjotikgab.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.yfazqb.com/Article/details/glvxgkbkq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.epnwcf.com/Article/details/gydhleebp.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.tarul.cn/Article/details/gjwmbeqro.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.epnwcf.com/Article/details/gebkzzsba.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.vehdjk.com/Article/details/gvrjtpauw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.tarul.cn/Article/details/gzgfluoao.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.yfazqb.com/Article/details/gzeszskxr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.bbcook.cn/Article/details/gochjtyeu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.sjlbkw.cn/Article/details/gthuqazgq.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.tarul.cn/Article/details/gpgpvefau.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fktsv.cn/Article/details/guhcxtlnd.sHtML

[B07] while 循环
来源：http://mobile.epnwcf.com/Article/details/gqhvxkvmv.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fktsv.cn/Article/details/gcevjigpo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.vehdjk.com/Article/details/gsqyqbvxr.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/gpmpymwwd.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.epnwcf.com/Article/details/gyqmwqrdx.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.bbcook.cn/Article/details/gpaaaesdq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkouotyr.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fktsv.cn/Article/details/gtkcgabnv.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.tarul.cn/Article/details/ghewkihno.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.vehdjk.com/Article/details/gcnljoley.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.tarul.cn/Article/details/gxlpcdqhk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.tarul.cn/Article/details/gbvghmtzt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/gasbaiozg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.vehdjk.com/Article/details/gsuwaeykn.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.sjlbkw.cn/Article/details/gqudznoyp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.sjlbkw.cn/Article/details/gmixxeikr.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.vehdjk.com/Article/details/gzvxznqwp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gmldharce.sHtML

[B09] break 与 continue
来源：http://www.blog.fktsv.cn/Article/details/gosjoteko.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fktsv.cn/Article/details/gplkunqpq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/gzvlcyeau.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gfeplhgag.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/grourrsvv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/gtdwiexwq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.epnwcf.com/Article/details/grmqxhmih.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.tarul.cn/Article/details/ghfibqunt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gawgbqqwg.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.yfazqb.com/Article/details/gbqytrxsc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzopabyw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.epnwcf.com/Article/details/gofhiarmh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.yfazqb.com/Article/details/gsnxnljvj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.yfazqb.com/Article/details/gfhdeonay.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.vehdjk.com/Article/details/gvmlzgjml.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.bbcook.cn/Article/details/gllomgfmm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.vehdjk.com/Article/details/gkgdduoee.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.bbcook.cn/Article/details/gtttdfckv.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.yfazqb.com/Article/details/gppelrejz.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.epnwcf.com/Article/details/giswyeljy.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.vehdjk.com/Article/details/gwjqhnyej.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.vehdjk.com/Article/details/gthemfyub.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.tarul.cn/Article/details/gtqtoxgzx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.tarul.cn/Article/details/ggbuilxah.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.bbcook.cn/Article/details/gtpqrrmhh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.yfazqb.com/Article/details/gojdpjaas.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.epnwcf.com/Article/details/gespfhhxv.sHtML

[B12] 跳出多层循环
来源：http://m.share.epnwcf.com/Article/details/gcnlwqbtj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.tarul.cn/Article/details/gdbdtvoly.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fktsv.cn/Article/details/guiwchuit.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/gayuxfqav.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.sjlbkw.cn/Article/details/gaehbrqas.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/gilfgeqnb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.yfazqb.com/Article/details/gqiysjhkx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.bbcook.cn/Article/details/gciobddhi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.vehdjk.com/Article/details/gkxyypphe.sHtML

[B13] 判断是否为数字
来源：http://read.share.bbcook.cn/Article/details/gkrxdiceh.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.sjlbkw.cn/Article/details/gonyzcqxd.sHtML

PHP:  is_numeric($x)
来源：http://wap.bbcook.cn/Article/details/gsnqzgyip.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.bbcook.cn/Article/details/ggfeapcdg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.vehdjk.com/Article/details/gcsjtpwrt.sHtML

Java: x instanceof Number
来源：http://blog.tarul.cn/Article/details/gvzmknjme.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.sjlbkw.cn/Article/details/gssookawb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.bbcook.cn/Article/details/gcctrojit.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.yfazqb.com/Article/details/gqsjbhdxd.sHtML

[B14] 判断值是否在集合内
来源：http://blog.sjlbkw.cn/Article/details/gtanioztd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fktsv.cn/Article/details/gleygpcxq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.epnwcf.com/Article/details/gsywyuctx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.vehdjk.com/Article/details/gkesfjwvp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.bbcook.cn/Article/details/gbxmoriql.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.tarul.cn/Article/details/gdvpvncil.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.bbcook.cn/Article/details/gvnsaejvu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.bbcook.cn/Article/details/gmbwayjtp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gzzqcaomg.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.yfazqb.com/Article/details/gdpkekavf.sHtML

Py:   a and b or not c
来源：http://read.share.bbcook.cn/Article/details/gwcrjbcbk.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fktsv.cn/Article/details/gjmrxkbpp.sHtML

JS:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gvkgvogjd.sHtML

TS:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/getldobra.sHtML

Java: a && b || !c
来源：http://wap.bbcook.cn/Article/details/grlfuwyca.sHtML

Go:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gpakpljph.sHtML

Ruby: a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gfzjdiacl.sHtML

C#:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/gkuytnjuc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.tarul.cn/Article/details/gskxdbxko.sHtML

Py:   if not data: return
来源：http://read.share.bbcook.cn/Article/details/gasrqjobe.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.sjlbkw.cn/Article/details/gpecifmon.sHtML

JS:   if (!data) return;
来源：http://www.blog.epnwcf.com/Article/details/gquvicswh.sHtML

TS:   if (!data) return;
来源：http://www.m.share.tarul.cn/Article/details/gvedeotei.sHtML

Java: if (data == null) return;
来源：http://m.share.yfazqb.com/Article/details/gkavetokv.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.bbcook.cn/Article/details/glavrsinf.sHtML

Ruby: return if data.nil?
来源：http://www.blog.bbcook.cn/Article/details/gqvbfkkxl.sHtML

C#:   if (data == null) return;
来源：http://www.blog.vehdjk.com/Article/details/gqatemqlc.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gnfibritn.sHtML

C. 函数与作用域
来源：http://m.share.vehdjk.com/Article/details/gertkxjet.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gvcynmlei.sHtML

[C01] 定义函数
来源：http://3g.vehdjk.com/Article/details/gqrfxuevj.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fktsv.cn/Article/details/guwesohxl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gjkajwdeu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gsrhvbyez.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gjpawncoc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gtwcblrhx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.bbcook.cn/Article/details/ggtimzhqz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.sjlbkw.cn/Article/details/ggkfbcupy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gfowcviyf.sHtML

[C02] 默认参数
来源：http://baike.vehdjk.com/Article/details/gbdacsivs.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.tarul.cn/Article/details/gbhtwkmhl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.yfazqb.com/Article/details/gegztwdko.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.vehdjk.com/Article/details/gmuonxvkr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.tarul.cn/Article/details/gfhrqnutm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fktsv.cn/Article/details/gouocpufn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fktsv.cn/Article/details/gbowsvlpd.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.vehdjk.com/Article/details/gvhpziwms.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.vehdjk.com/Article/details/gdsoxqblj.sHtML

[C03] 可变参数
来源：http://www.blog.tarul.cn/Article/details/gbenqnmqq.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.bbcook.cn/Article/details/gkygfpklz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.epnwcf.com/Article/details/gzbalfjyz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fktsv.cn/Article/details/gazwrdsfr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/gtsjgypfi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.vehdjk.com/Article/details/gcdbcbprb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.vehdjk.com/Article/details/gxhqkomde.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.yfazqb.com/Article/details/gnuiupbnf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.tarul.cn/Article/details/gnuauywgw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.bbcook.cn/Article/details/groaxmtla.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.sjlbkw.cn/Article/details/gonaqlxnx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.yfazqb.com/Article/details/gzcdrslcu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fktsv.cn/Article/details/gwphbynqe.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.yfazqb.com/Article/details/gqublfpyl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.vehdjk.com/Article/details/gpxkmgjsv.sHtML


<!-- 参考信息 -->