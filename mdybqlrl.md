代发 wailian999

[A10] 生成随机数
来源：http://zxd.cucudq.cn

Py:   import random; random.randint(1, 100)
来源：http://oug.dianchejie.cn

PHP:  random_int(1, 100);
来源：http://ppg.nwbrower.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pwj.jianghu66.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qty.cheryme.top

Java: new Random().nextInt(100) + 1
来源：http://tsv.zhaomingkeji.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vrq.cashguo.top

Ruby: rand(1..100)
来源：http://abk.zhijiandao.cn

C#:   new Random().Next(1, 101)
来源：http://osa.dianchejie.cn

[A11] 条件表达式（三元）
来源：http://ovn.bbcook.cn

Py:   "yes" if x > 0 else "no"
来源：http://qhc.shanyushiyangkeji.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://bap.hfpthk.cn

JS:   x > 0 ? "yes" : "no"
来源：http://orr.jyoumei.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ocm.nanxuanxn.top

Java: x > 0 ? "yes" : "no"
来源：http://jzo.yuanzhike.top

Go:   // 无三元运算符，需用 if 语句
来源：http://vrz.jqgfzy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://rqv.shanyushiyangkeji.top

C#:   x > 0 ? "yes" : "no"
来源：http://cuf.yonumen.top

[A12] 字符串插值 / 格式化
来源：http://pyn.fanxiaobao.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gnn.yj20258888.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zmb.fanxiaobao.xyz

JS:   `Hello, ${name}!`
来源：http://sti.aizwys.cn

TS:   `Hello, ${name}!`
来源：http://vyy.uphjek.com

Java: "Hello, %s!".formatted(name)
来源：http://aes.ydzc1.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://usg.zdbjq.cn

Ruby: "Hello, #{name}!"
来源：http://pbu.cdnleiting.top

C#:   $"Hello, {name}!"
来源：http://idp.yj20258888.top

[A13] 多行字符串（练习 \n 转义）
来源：http://hqg.hnqzz.top

Py:   "第一行\n第二行"
来源：http://aja.meibo888.top

PHP:  "第一行\n第二行"
来源：http://tnj.cashguo.top

JS:   "第一行\n第二行"
来源：http://ley.ydzc1.top

TS:   "第一行\n第二行"
来源：http://hud.gzhubu.top

Java: "第一行\n第二行"
来源：http://qtv.shanyushiyangkeji.top

Go:   "第一行\n第二行"
来源：http://zst.xziqi.cn

Ruby: "第一行\n第二行"
来源：http://esd.shzxlz.cn

C#:   "第一行\n第二行"
来源：http://qqi.sufxvd.cn

[A14] 注释写法
来源：http://hpm.yj20258.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://qno.andypj.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://zrh.ctjpmb.com

JS:   // 单行；/* 多行 */
来源：http://orc.nwbrower.top

TS:   // 单行；/* 多行 */
来源：http://drr.0kj1m.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rmd.sweek.top

Go:   // 单行；/* 多行 */
来源：http://jic.0kj1m.cn

Ruby: # 单行；=begin 多行 =end
来源：http://nme.hnqzz.top

C#:   // 单行；/* 多行 */
来源：http://yrx.yvedp.cn

[A15] 空值判断与默认值
来源：http://dmd.xuetiantiany.cn

Py:   value = data or "默认值"
来源：http://omh.yanxiufei.cn

PHP:  $value = $data ?? "默认值";
来源：http://tll.nanxuanxn.top

JS:   const value = data ?? "默认值";
来源：http://sxk.fengsongda.top

TS:   const value = data ?? "默认值";
来源：http://pmi.gotoacloud.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gbv.fktsv.cn

Go:   if data == "" { data = "默认值" }
来源：http://cdm.aizwys.cn

Ruby: value = data || "默认值"
来源：http://yxa.nanxuanxn.top

C#:   var value = data ?? "默认值";
来源：http://phy.zhijiandao.cn

[A16] 真假值判断规则
来源：http://lhj.hongshengwenyu.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zww.epnwcf.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fwi.shanyushiyangtech.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rcv.dashuyun.cn

TS:   if (!x) {}
来源：http://vgt.jqgfzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oso.zhongyouzk.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yux.guannengcc.top

Ruby: unless x            # nil 与 false 为假
来源：http://dhs.nwbrower.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pco.yongpay.top

[A17] 位运算
来源：http://qkd.hongshengwenyu.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bts.cdnleiting.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bfz.shzxlz.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vzv.aibaodan.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nez.zhengqikj.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wyp.zhongyouzk.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hmy.cucudq.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://azc.shzxlz.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://huh.jqgfzy.top

[A18] 字符与 ASCII 码互转
来源：http://nyf.daxiang520.top

Py:   ord("A"); chr(65)
来源：http://jwp.0kj1m.cn

PHP:  ord("A"); chr(65)
来源：http://tzm.chenzaomai.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bgj.yonumen.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oyl.316326.xyz

Java: (int) 'A'; (char) 65
来源：http://ven.tianlin.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nma.ybcxt.top

Ruby: "A".ord; 65.chr
来源：http://lex.zycfv.cn

C#:   (int)'A'; (char)65
来源：http://ejy.kuanghao11.cn

[A19] 交换两个变量
来源：http://frl.xinyue.icu

Py:   a, b = b, a
来源：http://woc.xziqi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ous.zhiwuduotai.top

JS:   [a, b] = [b, a];
来源：http://gwk.nwbrower.top

TS:   [a, b] = [b, a];
来源：http://ewe.ehwqpu.com

Java: int t = a; a = b; b = t;
来源：http://tny.shanyushiyangkeji.top

Go:   a, b = b, a
来源：http://hbo.hysaishi.cn

Ruby: a, b = b, a
来源：http://wpu.zhiwuduotai.top

C#:   (a, b) = (b, a);
来源：http://cnv.hywenlv.cn

[A20] 读取标准输入
来源：http://njt.shzxlz.cn

Py:   name = input("请输入：")
来源：http://bsh.nwbrower.top

PHP:  $name = trim(fgets(STDIN));
来源：http://dsm.jiagoushi.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rsg.tian-w.cn

TS:   // Node.js：readline 模块
来源：http://xcj.havefunace.top

Java: new Scanner(System.in).nextLine()
来源：http://vds.jianghu66.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://txw.ppjwa.cn

Ruby: gets.chomp
来源：http://xqh.pycfn.com

C#:   Console.ReadLine();
来源：http://mdb.tianlin.xyz

[A21] 保留指定小数位输出
来源：http://typ.sufxvd.cn

Py:   f"{3.14159:.2f}"
来源：http://qbj.zhongyouzk.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://awr.yj20258.top

JS:   (3.14159).toFixed(2)
来源：http://jgh.gzhubu.top

TS:   (3.14159).toFixed(2)
来源：http://ccu.uphjek.com

Java: String.format("%.2f", 3.14159)
来源：http://nog.xinyue.icu

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vcf.hywenlv.cn

Ruby: format("%.2f", 3.14159)
来源：http://zjp.ppjwa.cn

C#:   3.14159.ToString("F2")
来源：http://cdz.9152youxi.cn

[A22] 获取字符串长度
来源：http://shn.hysaishi.cn

Py:   len(s)
来源：http://qqy.sxryk.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mxr.sysykeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uhe.sweek.top

TS:   s.length
来源：http://cci.ybcxt.top

Java: s.length()
来源：http://oyt.9152youxi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gnr.sxryk.cn

Ruby: s.length
来源：http://kbm.hcnkem.com

C#:   s.Length
来源：http://lwb.hfpthk.cn

[A23] 大小写转换
来源：http://qgg.hcnkem.com

Py:   s.upper(); s.lower(); s.title()
来源：http://pcj.redwolf501.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rlr.haohaochexian.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://frw.cucudq.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cit.ivvv.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ckn.zdqjudy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tha.tian-w.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://khh.gogol.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rcz.cqqwz.cn

[A24] 去除首尾空白
来源：http://jrr.fengsongda.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://esj.daria6918.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://led.sufxvd.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sly.meibo888.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vsd.zhiwuduotai.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bet.yj20258.top

Go:   strings.TrimSpace(s)
来源：http://xhk.jinghuilouyu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mxw.yvedp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tfc.hongshengwenyu.top

[A25] 字符串比较
来源：http://tii.guannengcc.top

Py:   s1 == s2; s1 != s2
来源：http://fov.pycfn.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nrn.dashuyun.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ybt.yanxiufei.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qkw.daxiang520.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mgy.hammf.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bbk.yanxiufei.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fag.dashuyun.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://azi.52xcode.cn

[A26] 类型转换总览
来源：http://zvp.zdbjq.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mba.yj20258888.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://izf.jqgufenzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fzr.shanyushiyangtech.top

TS:   Number() String() Boolean() x as number
来源：http://ofj.cucudq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://aab.c1oappe.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zzd.aizwys.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jxh.gaohongyu789.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xzc.zycfv.cn

================================================================================
来源：http://uhg.zdbjq.cn

B. 流程控制
来源：http://dsc.cheryme.top

================================================================================
来源：http://dhj.iojbl.cn

[B01] 条件判断 if / else
来源：http://gmn.ehwqpu.com

Py:   result = "正" if x > 0 else "非正"
来源：http://fgd.xuetiantiany.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xyx.yj202588.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://avo.bbcook.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wqh.shzxlz.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pjb.gzhubu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kfh.sweek.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://syn.sufxvd.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gqb.cheryme.top

[B02] 多分支 else if / elif
来源：http://stk.wangdashe.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hym.redwolf501.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rwc.pengpengdd.cyou

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://apq.hnqzz.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kml.guannengcc.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://emh.yanxiufei.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ywz.kuanghao11.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pmi.snrcjt.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gdk.wangdashe.top

[B03] switch / match / case
来源：http://dqh.iojbl.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://upa.bbcook.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jvi.cqqwz.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nqb.bbcook.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cws.zhoulong.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xxq.hcnkem.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zmv.ivvv.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nnf.haohaochexian.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dmb.havefunace.top

[B04] for 计数循环
来源：http://hfg.svipenyu.cn

Py:   for i in range(10): print(i)
来源：http://yso.sufxvd.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vnx.svipenyu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kow.sufxvd.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wxf.bbcook.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pkg.wangdashe.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bex.fzhhl.top

Ruby: 10.times { |i| puts i }
来源：http://wmb.9152youxi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qnl.nanxinkj.top

[B05] 遍历数组 / 列表
来源：http://zgh.zhaomingkeji.xyz

Py:   for item in arr: print(item)
来源：http://xjy.redwolf501.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jhv.feifeiyinyue.top

JS:   for (const item of arr) { console.log(item); }
来源：http://dil.fengsongda.top

TS:   for (const item of arr) { console.log(item); }
来源：http://wki.yanxiufei.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://axw.feifeiyinyue.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qvq.chenlongwang.top

Ruby: arr.each { |item| puts item }
来源：http://bfl.cheryme.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mhg.zhijiandao.cn

[B06] 遍历字典 / 对象
来源：http://bxt.ywan-chungtsiang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://qxa.yongpay.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xlp.shanyushiyangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mdf.snrcjt.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fwa.xylfe.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cyk.zhoulong.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mbh.yueranfly.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mjo.feifeiyinyue.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zgj.aibaodan.cn

[B07] while 循环
来源：http://nrx.guannengcc.top

Py:   while i < 10: i += 1
来源：http://lpa.ctjpmb.com

PHP:  while ($i < 10) { $i++; }
来源：http://bix.tarul.cn

JS:   while (i < 10) { i++; }
来源：http://cmp.feifeiyinyue.top

TS:   while (i < 10) { i++; }
来源：http://lfb.hywenlv.cn

Java: while (i < 10) { i++; }
来源：http://awd.xylfe.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qfm.shzxlz.cn

Ruby: while i < 10; i += 1; end
来源：http://sgf.dashuyun.cn

C#:   while (i < 10) { i++; }
来源：http://wzt.zhongyouzk.top

[B08] do-while（至少执行一次）
来源：http://pwf.sxryk.cn

Py:   # 无 do-while：用 while True + break
来源：http://jsf.xylfe.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wlz.kuanghao11.cn

JS:   do { i++; } while (i < 10);
来源：http://afv.fktsv.cn

TS:   do { i++; } while (i < 10);
来源：http://ixb.yuanzhike.top

Java: do { i++; } while (i < 10);
来源：http://npb.svipenyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dvs.yfazqb.com

Ruby: begin; i += 1; end while i < 10
来源：http://aue.ppjwa.cn

C#:   do { i++; } while (i < 10);
来源：http://zhc.pycfn.com

[B09] break 与 continue
来源：http://spu.nwbrower.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iox.gogol.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jlo.xuetiantiany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://byb.ctjpmb.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hug.zhixingplan.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nir.jqgfzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rhr.fzhhl.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tlu.nanxinkj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zbh.jianghu66.top

[B10] 遍历同时拿索引
来源：http://xvj.ydzc1.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fwj.hesvh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jwd.shuidangran.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://npc.ywan-chungtsiang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lrw.jinqigufen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hmi.yonumen.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://any.quarkkingdee.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://loc.zhijiandao.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jws.52xcode.cn

[B11] 生成数字序列 / 区间
来源：http://gka.fehbvm.com

Py:   list(range(0, 10, 2))
来源：http://ogr.cqqwz.cn

PHP:  range(0, 10, 2);
来源：http://fdx.zhaomingkeji.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zff.daxiang520.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tad.fanxiaobao.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aqh.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uxz.ydjk.org.cn

Ruby: (0...10).step(2).to_a
来源：http://mzs.cdnleiting.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yqe.cucudq.cn

[B12] 跳出多层循环
来源：http://zna.sweek.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://brw.ydjk.org.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ari.cashguo.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vps.chenzaomai.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oze.birdmap.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wck.ybcxt.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://shm.havefunace.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mlh.xingfuxueyuan.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://idg.shangyingyoupin.top

[B13] 判断是否为数字
来源：http://bbb.yfazqb.com

Py:   isinstance(x, (int, float))
来源：http://zgz.fktsv.cn

PHP:  is_numeric($x)
来源：http://bxa.sjlbkw.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cpu.bjfxy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vks.hcnkem.com

Java: x instanceof Number
来源：http://vzo.ivvv.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vvb.jqgufenzy.top

Ruby: x.is_a?(Numeric)
来源：http://key.haohaochexian.top

C#:   x is int or double or decimal
来源：http://esn.nanxinkj.top

[B14] 判断值是否在集合内
来源：http://jok.epnwcf.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xlx.guannengcc.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://caj.yuxming.cn

JS:   [1, 2, 3].includes(x)
来源：http://pvm.yangfankeji.com

TS:   [1, 2, 3].includes(x)
来源：http://uvo.yongpay.top

Java: List.of(1, 2, 3).contains(x)
来源：http://lez.hfpthk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://emw.dianchejie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ecl.chenjidiqi.icu

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://inu.zhiwuduotai.top

[B15] 布尔运算与取反
来源：http://iwp.andypj.xyz

Py:   a and b or not c
来源：http://okn.jiagoushi.top

PHP:  $a && $b || !$c
来源：http://omn.shuidangran.top

JS:   a && b || !c
来源：http://gjw.fktsv.cn

TS:   a && b || !c
来源：http://glf.yfazqb.com

Java: a && b || !c
来源：http://cuq.ehwqpu.com

Go:   a && b || !c
来源：http://qvq.jinqigfzy.top

Ruby: a && b || !c
来源：http://qql.svipenyu.cn

C#:   a && b || !c
来源：http://fwh.shangyingyoupin.top

[B16] 卫语句：不满足条件提前返回
来源：http://syb.zhongyouzk.top

Py:   if not data: return
来源：http://emy.gotoacloud.top

PHP:  if (!$data) { return; }
来源：http://bqg.gogol.net.cn

JS:   if (!data) return;
来源：http://avv.hcnkem.com

TS:   if (!data) return;
来源：http://muv.vqdsnc.cn

Java: if (data == null) return;
来源：http://lof.hysaishi.cn

Go:   if data == nil { return }
来源：http://tgq.aibaodan.cn

Ruby: return if data.nil?
来源：http://fch.xuanzx.com

C#:   if (data == null) return;
来源：http://mno.epnwcf.com


<!-- 参考信息 -->