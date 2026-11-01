代发 wailian999

[A14] 注释写法
来源：http://3g.tarul.cn/Article/details/geblcqmqx.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.epnwcf.com/Article/details/genyqpnfx.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.yfazqb.com/Article/details/goaeagzsz.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.tarul.cn/Article/details/gckvoqgpl.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.epnwcf.com/Article/details/gwtuukkis.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.epnwcf.com/Article/details/gayiprytq.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.sjlbkw.cn/Article/details/gheyotxxp.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.tarul.cn/Article/details/gzbzdirpz.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.tarul.cn/Article/details/gpjburtwq.sHtML

[A15] 空值判断与默认值
来源：http://baike.tarul.cn/Article/details/gtizesbkd.sHtML

Py:   value = data or "默认值"
来源：http://baike.epnwcf.com/Article/details/gouspecpo.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fktsv.cn/Article/details/grafwmrhk.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.fktsv.cn/Article/details/gxkktvyoy.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.bbcook.cn/Article/details/gynzvtggf.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.epnwcf.com/Article/details/gwtunjbcs.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.tarul.cn/Article/details/gtsqowery.sHtML

Ruby: value = data || "默认值"
来源：http://blog.fktsv.cn/Article/details/gfhwoaujq.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.yfazqb.com/Article/details/ghvawlmyc.sHtML

[A16] 真假值判断规则
来源：http://mobile.tarul.cn/Article/details/gwqwhhozr.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.vehdjk.com/Article/details/gfcekujuq.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.vehdjk.com/Article/details/grnitpctl.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.epnwcf.com/Article/details/gqvdrqjdz.sHtML

TS:   if (!x) {}
来源：http://m.share.bbcook.cn/Article/details/gdpdbixhe.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.tarul.cn/Article/details/gpiyqxdbh.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.sjlbkw.cn/Article/details/gwzkauwrx.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.epnwcf.com/Article/details/ghjmvqxcy.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.sjlbkw.cn/Article/details/gbhjcvapv.sHtML

[A17] 位运算
来源：http://www.blog.tarul.cn/Article/details/gkswcywbk.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.tarul.cn/Article/details/gswdbewch.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.tarul.cn/Article/details/glgfgpadg.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/gwjunxudg.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.epnwcf.com/Article/details/gpjmlvhao.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/gsowoinml.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.fktsv.cn/Article/details/gbpdgqgjf.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxcukrii.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.vehdjk.com/Article/details/gowgrodue.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.tarul.cn/Article/details/gwpstdpmp.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.bbcook.cn/Article/details/gcpveclpw.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.fktsv.cn/Article/details/grdplzrcy.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.tarul.cn/Article/details/gjebrquxu.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.fktsv.cn/Article/details/goszhrfgn.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.sjlbkw.cn/Article/details/garqntmtb.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.yfazqb.com/Article/details/gzfubvfzf.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.bbcook.cn/Article/details/gxhvehuud.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.bbcook.cn/Article/details/gslxfhdci.sHtML

[A19] 交换两个变量
来源：http://mobile.sjlbkw.cn/Article/details/gmpkfhios.sHtML

Py:   a, b = b, a
来源：http://mobile.epnwcf.com/Article/details/glbngocpg.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.epnwcf.com/Article/details/greaaqokm.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.yfazqb.com/Article/details/gccjctrsd.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.epnwcf.com/Article/details/gqfvzzoie.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.sjlbkw.cn/Article/details/ggoixzsxr.sHtML

Go:   a, b = b, a
来源：http://3g.yfazqb.com/Article/details/ghisuzrtb.sHtML

Ruby: a, b = b, a
来源：http://read.share.bbcook.cn/Article/details/gazzujrcd.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.sjlbkw.cn/Article/details/ggniosjok.sHtML

[A20] 读取标准输入
来源：http://3g.bbcook.cn/Article/details/gvqloeknz.sHtML

Py:   name = input("请输入：")
来源：http://3g.vehdjk.com/Article/details/ggpfigjff.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.sjlbkw.cn/Article/details/goxnqhioy.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.bbcook.cn/Article/details/gfggbfixh.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.tarul.cn/Article/details/gnnwzciuc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.vehdjk.com/Article/details/gugzmvpfv.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.bbcook.cn/Article/details/gcfwipjuf.sHtML

Ruby: gets.chomp
来源：http://www.blog.vehdjk.com/Article/details/gvmuusyqa.sHtML

C#:   Console.ReadLine();
来源：http://wap.yfazqb.com/Article/details/gccmgzfut.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.bbcook.cn/Article/details/gmyphgjrm.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.sjlbkw.cn/Article/details/gozfhuyhp.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.epnwcf.com/Article/details/gesjdvnqs.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.tarul.cn/Article/details/gzoshrbby.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.bbcook.cn/Article/details/gwxgsjuwf.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.yfazqb.com/Article/details/gfqtvsmbe.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.fktsv.cn/Article/details/gguxdnbbj.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.vehdjk.com/Article/details/ggqjxypwe.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.sjlbkw.cn/Article/details/gbojewwrz.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/gaatisvwj.sHtML

Py:   len(s)
来源：http://www.share.sjlbkw.cn/Article/details/gulbahuor.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.sjlbkw.cn/Article/details/giabjjjbn.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.vehdjk.com/Article/details/gbicppbas.sHtML

TS:   s.length
来源：http://baike.fktsv.cn/Article/details/gejszdljv.sHtML

Java: s.length()
来源：http://www.share.yfazqb.com/Article/details/gyijdzmyk.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.fktsv.cn/Article/details/glzgrpckn.sHtML

Ruby: s.length
来源：http://blog.bbcook.cn/Article/details/gtwfqdjzc.sHtML

C#:   s.Length
来源：http://www.share.vehdjk.com/Article/details/gpwdbgnyb.sHtML

[A23] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gavggpqpg.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.bbcook.cn/Article/details/gjjecuiwg.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.sjlbkw.cn/Article/details/gkeqffeok.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.tarul.cn/Article/details/gjzdwifrm.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.bbcook.cn/Article/details/gfcaqazkn.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.tarul.cn/Article/details/gbsjwrfpm.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.epnwcf.com/Article/details/gbtnztcyj.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.fktsv.cn/Article/details/gtlyeglzr.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fktsv.cn/Article/details/glaqtjhvm.sHtML

[A24] 去除首尾空白
来源：http://read.share.tarul.cn/Article/details/gydzvvntp.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.epnwcf.com/Article/details/gklgfdujj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.fktsv.cn/Article/details/gqjuoorpw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.tarul.cn/Article/details/gdykrrhju.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fktsv.cn/Article/details/grlfxstkm.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.yfazqb.com/Article/details/gdtlxtplx.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.fktsv.cn/Article/details/gefdqkgrf.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.bbcook.cn/Article/details/gyurvvvhn.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.yfazqb.com/Article/details/gqqxwmnix.sHtML

[A25] 字符串比较
来源：http://blog.sjlbkw.cn/Article/details/ggppkncuf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.fktsv.cn/Article/details/gvlcpekzw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.sjlbkw.cn/Article/details/gkttsooip.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.vehdjk.com/Article/details/gonnmriwn.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.bbcook.cn/Article/details/gumhnmrou.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.sjlbkw.cn/Article/details/gnpnjtarb.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.bbcook.cn/Article/details/galibqehp.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.epnwcf.com/Article/details/gelefzohw.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.fktsv.cn/Article/details/gzhvoiaop.sHtML

[A26] 类型转换总览
来源：http://blog.fktsv.cn/Article/details/ggysyzlep.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.fktsv.cn/Article/details/gbupyzhtk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.yfazqb.com/Article/details/gpidpfxdp.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.epnwcf.com/Article/details/getvhiiqj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.epnwcf.com/Article/details/gheevczzb.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.fktsv.cn/Article/details/gsygvahhf.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.epnwcf.com/Article/details/ggskcnrxm.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.vehdjk.com/Article/details/ggaxjibji.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.epnwcf.com/Article/details/goabvckkc.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/grzfukovy.sHtML

B. 流程控制
来源：http://www.m.share.vehdjk.com/Article/details/grxwiflph.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gwpltzblf.sHtML

[B01] 条件判断 if / else
来源：http://m.share.yfazqb.com/Article/details/gvghcmonx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fktsv.cn/Article/details/gemccmtgc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.yfazqb.com/Article/details/glwuzgthj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/gedyqrkvq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.tarul.cn/Article/details/ghcuulqxj.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.epnwcf.com/Article/details/gupdtgfzk.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwfmsskja.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.fktsv.cn/Article/details/ghimfppjf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/gupwypyhc.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.bbcook.cn/Article/details/gamogvfil.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fktsv.cn/Article/details/gimxxiouz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.vehdjk.com/Article/details/gjqghbpgi.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/gwrmxlqnb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/glmlsmpul.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.epnwcf.com/Article/details/ggtdxrrsj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.yfazqb.com/Article/details/gcudlaeyr.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.epnwcf.com/Article/details/ggqzzvxaz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.tarul.cn/Article/details/gwolkvnca.sHtML

[B03] switch / match / case
来源：http://wap.epnwcf.com/Article/details/giunvuhff.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.yfazqb.com/Article/details/ghpjihyeb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.bbcook.cn/Article/details/gwlbjftwv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.bbcook.cn/Article/details/gxjovkyqx.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.bbcook.cn/Article/details/gmvbisrmu.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.vehdjk.com/Article/details/gxndsozrd.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fktsv.cn/Article/details/gmwgahppe.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.tarul.cn/Article/details/gqnqjabjo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.epnwcf.com/Article/details/gupjjzhvp.sHtML

[B04] for 计数循环
来源：http://3g.bbcook.cn/Article/details/gqihygbys.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.epnwcf.com/Article/details/ggcbhejnv.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.vehdjk.com/Article/details/gnwqqsslu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.epnwcf.com/Article/details/gjoghixut.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.vehdjk.com/Article/details/gnjzisfjd.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.epnwcf.com/Article/details/gjtonxoeb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.sjlbkw.cn/Article/details/gsaagtiiy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.sjlbkw.cn/Article/details/gcsnetbjq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.bbcook.cn/Article/details/gjidfqsmz.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fktsv.cn/Article/details/gpodtrwll.sHtML

Py:   for item in arr: print(item)
来源：http://blog.epnwcf.com/Article/details/gzbsponkf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.sjlbkw.cn/Article/details/gotjonxdc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.sjlbkw.cn/Article/details/gjjbpxmnp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.bbcook.cn/Article/details/gwsqqiuvm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fktsv.cn/Article/details/gjlbdgprl.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.epnwcf.com/Article/details/gyrtfsvkl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.fktsv.cn/Article/details/guuobxvgv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.vehdjk.com/Article/details/gfomeitsa.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.vehdjk.com/Article/details/ghkbefqro.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.yfazqb.com/Article/details/gpqnvroxz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.sjlbkw.cn/Article/details/gjylmpajq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.tarul.cn/Article/details/gqycnqcgt.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.tarul.cn/Article/details/guomplodz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.sjlbkw.cn/Article/details/gwofrijfv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.yfazqb.com/Article/details/gyubhqpnv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.yfazqb.com/Article/details/gfsgobcbn.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.tarul.cn/Article/details/gnuhjwqla.sHtML

[B07] while 循环
来源：http://baike.bbcook.cn/Article/details/gaomypvta.sHtML

Py:   while i < 10: i += 1
来源：http://blog.epnwcf.com/Article/details/gesofmvdv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.bbcook.cn/Article/details/ggtfczxjx.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/gdayiffkj.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/gakxzztag.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.vehdjk.com/Article/details/ggkwmlyqx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fktsv.cn/Article/details/giutqmdbe.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.vehdjk.com/Article/details/gyqcgmpze.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gqawoyurj.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.epnwcf.com/Article/details/gxhbjneiy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fktsv.cn/Article/details/guuqnootm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gmfzpjxpp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.tarul.cn/Article/details/gfhumdivy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.epnwcf.com/Article/details/gjwhooago.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/gagfgwork.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.vehdjk.com/Article/details/getodiabx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.bbcook.cn/Article/details/gmbpgixhj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gmanongbs.sHtML

[B09] break 与 continue
来源：http://mobile.tarul.cn/Article/details/gfzbdogjv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.tarul.cn/Article/details/gprcqbaex.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gdwhxutnm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gudmgkybi.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/gfmnpfxig.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/ggpkmbasm.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.tarul.cn/Article/details/ghklxswum.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.sjlbkw.cn/Article/details/geljwivaf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/gfkislmbz.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fktsv.cn/Article/details/glpswetdb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.vehdjk.com/Article/details/gepwibiru.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.epnwcf.com/Article/details/gmdgozuuj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.vehdjk.com/Article/details/gvwkdghjr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.vehdjk.com/Article/details/gxcponayz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.vehdjk.com/Article/details/gtfsnjcua.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.bbcook.cn/Article/details/gatyglbak.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.tarul.cn/Article/details/gulvdmjzh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.yfazqb.com/Article/details/gmmhtnkmb.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.vehdjk.com/Article/details/gubbozapb.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fktsv.cn/Article/details/gnkmzumfr.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.epnwcf.com/Article/details/gabsckqtk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.epnwcf.com/Article/details/gnjiklzny.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.vehdjk.com/Article/details/ggiyegkqy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.vehdjk.com/Article/details/gmsqrvail.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.bbcook.cn/Article/details/gmbzbumid.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.sjlbkw.cn/Article/details/gktivxryl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.epnwcf.com/Article/details/glmcljuaw.sHtML

[B12] 跳出多层循环
来源：http://read.share.fktsv.cn/Article/details/gzvizqwah.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.bbcook.cn/Article/details/gmpxmfkvq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.sjlbkw.cn/Article/details/glidychxj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gxlhyvwxa.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.sjlbkw.cn/Article/details/gsargbalr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/ggljpowjv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.tarul.cn/Article/details/gbfktghtz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fktsv.cn/Article/details/gpdlteiia.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.epnwcf.com/Article/details/gznlveien.sHtML

[B13] 判断是否为数字
来源：http://read.share.bbcook.cn/Article/details/gatbtrdyh.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.sjlbkw.cn/Article/details/glhcwtqqi.sHtML

PHP:  is_numeric($x)
来源：http://read.share.sjlbkw.cn/Article/details/gflphjgfj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.tarul.cn/Article/details/ggusehpbi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.bbcook.cn/Article/details/gxfpbujnh.sHtML

Java: x instanceof Number
来源：http://www.m.share.epnwcf.com/Article/details/gpmefvrkw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.sjlbkw.cn/Article/details/glgtiqrix.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fktsv.cn/Article/details/gxyoeiztd.sHtML

C#:   x is int or double or decimal
来源：http://baike.yfazqb.com/Article/details/gryafamyv.sHtML

[B14] 判断值是否在集合内
来源：http://3g.bbcook.cn/Article/details/gpvplyewj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.vehdjk.com/Article/details/gvurzlnho.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.yfazqb.com/Article/details/gixfzviqi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gdrjejrej.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.tarul.cn/Article/details/gutdkudew.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fktsv.cn/Article/details/gfqgapxsf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fktsv.cn/Article/details/gotptptze.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fktsv.cn/Article/details/gvnkldfnk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.bbcook.cn/Article/details/gjtpqyfwi.sHtML

[B15] 布尔运算与取反
来源：http://read.share.sjlbkw.cn/Article/details/ghctioejk.sHtML

Py:   a and b or not c
来源：http://www.m.share.vehdjk.com/Article/details/gamoxwrqh.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.sjlbkw.cn/Article/details/gpwdbtooq.sHtML

JS:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gesfzdprr.sHtML

TS:   a && b || !c
来源：http://blog.tarul.cn/Article/details/gruxwkkve.sHtML

Java: a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gkxegioto.sHtML

Go:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gtbsajhgr.sHtML

Ruby: a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gcmssojkr.sHtML

C#:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/gdjwwpizq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.vehdjk.com/Article/details/gwqzptywt.sHtML

Py:   if not data: return
来源：http://blog.epnwcf.com/Article/details/gzfdjzrsw.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.yfazqb.com/Article/details/gvmjzalof.sHtML

JS:   if (!data) return;
来源：http://mobile.tarul.cn/Article/details/gzvoyioiy.sHtML

TS:   if (!data) return;
来源：http://www.blog.bbcook.cn/Article/details/gtqocxfbf.sHtML

Java: if (data == null) return;
来源：http://mobile.vehdjk.com/Article/details/gakdmfgze.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.bbcook.cn/Article/details/gkcxirajn.sHtML

Ruby: return if data.nil?
来源：http://blog.vehdjk.com/Article/details/guzqgikub.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fktsv.cn/Article/details/ggeofovgn.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gsdueanyi.sHtML

C. 函数与作用域
来源：http://wap.epnwcf.com/Article/details/gchjpzmxp.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gehemelps.sHtML

[C01] 定义函数
来源：http://mobile.tarul.cn/Article/details/gxsamfncv.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.tarul.cn/Article/details/gihgxadum.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/gcoctyhhm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gssxviokm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gatfrchlz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gwpblvhql.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.tarul.cn/Article/details/gwkopkloy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.tarul.cn/Article/details/gmqxzpmqa.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gczkqvvil.sHtML

[C02] 默认参数
来源：http://www.m.share.yfazqb.com/Article/details/gxktxafmb.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.sjlbkw.cn/Article/details/gykitegfb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.sjlbkw.cn/Article/details/gmrnvbipc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.vehdjk.com/Article/details/gnuttwwra.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.bbcook.cn/Article/details/giinnwsyz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.sjlbkw.cn/Article/details/gxmuejwyo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.yfazqb.com/Article/details/gtklhcgxr.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.bbcook.cn/Article/details/gbhffpoxm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gorevyrgl.sHtML

[C03] 可变参数
来源：http://blog.tarul.cn/Article/details/gvdpzuybm.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fktsv.cn/Article/details/gaxvsubrh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gybjvbsmt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.tarul.cn/Article/details/grzyjdwnj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fktsv.cn/Article/details/gxvlaylwv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.sjlbkw.cn/Article/details/golkzmjis.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.epnwcf.com/Article/details/gwinqjynj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.tarul.cn/Article/details/gyyfjvgzd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fktsv.cn/Article/details/gfkhiwjuv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.vehdjk.com/Article/details/gcufcrvvl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.tarul.cn/Article/details/guqgynhvj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.yfazqb.com/Article/details/giojttlzo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.tarul.cn/Article/details/gttmscaeb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.yfazqb.com/Article/details/gjpaujdda.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.bbcook.cn/Article/details/ghaoetvbr.sHtML


<!-- 参考信息 -->