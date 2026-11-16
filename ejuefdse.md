代发 wailian999

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://czg.smart0.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://lbx.yvedp.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://znq.snrcjt.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ufx.zhaomingkeji.xyz

Java: 7 / 2; 7 % 2
来源：http://qix.zhiwuduotai.top

Go:   7 / 2; 7 % 2
来源：http://wnj.pycfn.com

Ruby: 7 / 2; 7 % 2
来源：http://xkv.andypj.xyz

C#:   7 / 2; 7 % 2
来源：http://aaq.tianlin.xyz

[A06] 字符串转数字
来源：http://wvp.zdqjudy.top

Py:   int("42"); float("3.14")
来源：http://bam.jianghu66.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zbi.fehbvm.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://leb.ehwqpu.com

TS:   parseInt("42", 10); Number("42")
来源：http://uxf.nwbrower.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yzw.tanke756.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://igj.hnxiangtu.top

Ruby: "42".to_i; "3.14".to_f
来源：http://iji.gaohongyu789.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vum.hesvh.cn

[A07] 数字转字符串
来源：http://yhs.xuetiantiany.cn

Py:   str(42)
来源：http://pmc.jyoumei.cn

PHP:  (string) 42; strval(42)
来源：http://jyp.fzhhl.top

JS:   String(42); (42).toString()
来源：http://arn.aizwys.cn

TS:   String(42)
来源：http://pto.yongpay.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://mzc.zhoulong.xyz

Go:   strconv.Itoa(42)
来源：http://ecg.kuanghao11.cn

Ruby: 42.to_s
来源：http://zrn.gzhubu.top

C#:   42.ToString()
来源：http://khv.aizwys.cn

[A08] 取整与四舍五入
来源：http://woq.tanke756.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://shi.zhaomingkeji.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gua.fzhhl.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nuj.feifeiyinyue.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gri.hesvh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fen.chenzaomai.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wlv.yongpay.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://bul.52xcode.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gmh.wangdashe.top

[A09] 绝对值与最大最小值
来源：http://gge.iojbl.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ssy.snrcjt.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mkr.hammf.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ukm.smart0.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ncq.sysykeji.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cun.snrcjt.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ocp.nanxinkj.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jzo.chenjidiqi.icu

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://est.hcnkem.com

[A10] 生成随机数
来源：http://wle.ppjwa.cn

Py:   import random; random.randint(1, 100)
来源：http://exn.hfpthk.cn

PHP:  random_int(1, 100);
来源：http://klu.haohaochexian.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ltg.zhongyouzk.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ucs.jinghuilouyu.cn

Java: new Random().nextInt(100) + 1
来源：http://nak.jinghuilouyu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wba.jinqigfzy.top

Ruby: rand(1..100)
来源：http://rzy.sweek.top

C#:   new Random().Next(1, 101)
来源：http://nqb.tianlin.xyz

[A11] 条件表达式（三元）
来源：http://vqu.hysaishi.cn

Py:   "yes" if x > 0 else "no"
来源：http://wwf.pycfn.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://rmk.52xcode.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gsg.zhaomingkeji.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://irm.hongshengwenyu.top

Java: x > 0 ? "yes" : "no"
来源：http://hjl.shzxlz.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hyd.ywan-chungtsiang.top

Ruby: x > 0 ? "yes" : "no"
来源：http://yix.aizwys.cn

C#:   x > 0 ? "yes" : "no"
来源：http://msu.zdbjq.cn

[A12] 字符串插值 / 格式化
来源：http://waq.guowangkeji.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hcs.cqqwz.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://eol.yuxming.cn

JS:   `Hello, ${name}!`
来源：http://nrn.ydjk.org.cn

TS:   `Hello, ${name}!`
来源：http://lco.uphjek.com

Java: "Hello, %s!".formatted(name)
来源：http://rqg.hnxiangtu.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pov.yuanzhike.top

Ruby: "Hello, #{name}!"
来源：http://joz.shanyushiyangtech.top

C#:   $"Hello, {name}!"
来源：http://yhc.fanxiaobao.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://gvt.tian-w.cn

Py:   "第一行\n第二行"
来源：http://rho.xylfe.cn

PHP:  "第一行\n第二行"
来源：http://hej.wangdashe.top

JS:   "第一行\n第二行"
来源：http://sdp.nwbrower.top

TS:   "第一行\n第二行"
来源：http://lkb.zycfv.cn

Java: "第一行\n第二行"
来源：http://gze.sjlbkw.cn

Go:   "第一行\n第二行"
来源：http://eis.vehdjk.com

Ruby: "第一行\n第二行"
来源：http://qxh.52xcode.cn

C#:   "第一行\n第二行"
来源：http://olg.hywenlv.cn

[A14] 注释写法
来源：http://tnu.xingfuxueyuan.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://iug.ehwqpu.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://qii.kuanghao11.cn

JS:   // 单行；/* 多行 */
来源：http://fsm.ehwqpu.com

TS:   // 单行；/* 多行 */
来源：http://tax.0kj1m.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pio.xylfe.cn

Go:   // 单行；/* 多行 */
来源：http://tky.jinyuanbaomall.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tpd.nanxinkj.top

C#:   // 单行；/* 多行 */
来源：http://fdu.jiagoushi.top

[A15] 空值判断与默认值
来源：http://maf.chenzaomai.com

Py:   value = data or "默认值"
来源：http://nqe.gzhubu.top

PHP:  $value = $data ?? "默认值";
来源：http://uuq.bjfxy.top

JS:   const value = data ?? "默认值";
来源：http://jhz.bjfxy.top

TS:   const value = data ?? "默认值";
来源：http://hxc.cashguo.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://umg.ywan-chungtsiang.top

Go:   if data == "" { data = "默认值" }
来源：http://rjo.zhaomingkeji.xyz

Ruby: value = data || "默认值"
来源：http://uag.cucudq.cn

C#:   var value = data ?? "默认值";
来源：http://ddf.meibo888.top

[A16] 真假值判断规则
来源：http://mrc.kuanghao11.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://art.dianchejie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lep.nanxuanxn.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yll.yuanzhike.top

TS:   if (!x) {}
来源：http://hsg.jlsjyb.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uvn.wangshuangyany.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://eco.c1oappe.top

Ruby: unless x            # nil 与 false 为假
来源：http://jjq.jqgufenzy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://txp.shanyushiyangtech.top

[A17] 位运算
来源：http://nty.ywan-chungtsiang.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xsf.ehwqpu.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rvw.jqgufenzy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ido.bbcook.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://khf.yvedp.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ela.feifeiyinyue.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pmw.9152youxi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rly.ywan-chungtsiang.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aqr.shangyingyoupin.top

[A18] 字符与 ASCII 码互转
来源：http://vdi.andypj.xyz

Py:   ord("A"); chr(65)
来源：http://kqn.zhixingplan.top

PHP:  ord("A"); chr(65)
来源：http://gqr.epnwcf.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kfl.jinqigfzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mkv.0kj1m.cn

Java: (int) 'A'; (char) 65
来源：http://bco.zhaomingkeji.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pff.nanxuanxn.top

Ruby: "A".ord; 65.chr
来源：http://lxm.dashuyun.cn

C#:   (int)'A'; (char)65
来源：http://ndo.dashuyun.cn

[A19] 交换两个变量
来源：http://isc.bjfxy.top

Py:   a, b = b, a
来源：http://nla.hongshengwenyu.top

PHP:  [$a, $b] = [$b, $a];
来源：http://lnp.zhiwuduotai.top

JS:   [a, b] = [b, a];
来源：http://jqv.9152youxi.cn

TS:   [a, b] = [b, a];
来源：http://sup.cheryme.top

Java: int t = a; a = b; b = t;
来源：http://cdq.ppjwa.cn

Go:   a, b = b, a
来源：http://dav.gotoacloud.top

Ruby: a, b = b, a
来源：http://ukf.pengpengdd.cyou

C#:   (a, b) = (b, a);
来源：http://uof.ydjk.org.cn

[A20] 读取标准输入
来源：http://gnx.yanxiufei.cn

Py:   name = input("请输入：")
来源：http://pya.xuanzx.com

PHP:  $name = trim(fgets(STDIN));
来源：http://rpr.zhengqikj.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pwv.sysykeji.top

TS:   // Node.js：readline 模块
来源：http://qlg.yanxiufei.cn

Java: new Scanner(System.in).nextLine()
来源：http://hyx.ppjwa.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xgn.gzhubu.top

Ruby: gets.chomp
来源：http://obr.jqgufenzy.top

C#:   Console.ReadLine();
来源：http://eyg.yj202588.top

[A21] 保留指定小数位输出
来源：http://soi.jinqigfzy.top

Py:   f"{3.14159:.2f}"
来源：http://hru.c1oappe.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xsw.ywan-chungtsiang.top

JS:   (3.14159).toFixed(2)
来源：http://gyd.hfpthk.cn

TS:   (3.14159).toFixed(2)
来源：http://oky.jinghuilouyu.cn

Java: String.format("%.2f", 3.14159)
来源：http://ncq.xylfe.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vzh.shanyushiyangkeji.top

Ruby: format("%.2f", 3.14159)
来源：http://nmc.gotoacloud.top

C#:   3.14159.ToString("F2")
来源：http://amc.epnwcf.com

[A22] 获取字符串长度
来源：http://dcc.jinyuanbaomall.cn

Py:   len(s)
来源：http://fhg.jyoumei.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://emc.ywan-chungtsiang.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rni.uphjek.com

TS:   s.length
来源：http://xws.wangdashe.top

Java: s.length()
来源：http://wvx.sxryk.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://eyc.jqgfzy.top

Ruby: s.length
来源：http://xag.vqdsnc.cn

C#:   s.Length
来源：http://ava.c1oappe.top

[A23] 大小写转换
来源：http://zdx.ydjk.org.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vhx.xuetiantiany.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tkc.zhiwuduotai.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://okn.xinyue.icu

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qed.ydjk.org.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zgp.gogol.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rgc.dashuyun.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wfh.jlsjyb.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://mrx.daxiang520.top

[A24] 去除首尾空白
来源：http://mov.hnxiangtu.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wga.zhixingplan.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zsm.iojbl.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eoz.wangdashe.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ovr.andypj.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ilo.316326.xyz

Go:   strings.TrimSpace(s)
来源：http://bef.yonumen.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ekl.smart0.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ypw.bbcook.cn

[A25] 字符串比较
来源：http://vej.dashuyun.cn

Py:   s1 == s2; s1 != s2
来源：http://brt.wangshuangyany.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xze.316326.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tyo.tianlin.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vdr.gaohongyu789.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ush.tianlin.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uos.havefunace.top

Ruby: s1 == s2; s1 <=> s2
来源：http://adu.pycfn.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://odb.snrcjt.cn

[A26] 类型转换总览
来源：http://pyo.jlsjyb.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ews.zhixingplan.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vkz.zhongyouzk.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qki.yueranfly.top

TS:   Number() String() Boolean() x as number
来源：http://zqg.andypj.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sic.jinghuilouyu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qnh.fengsongda.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://khl.birdmap.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rbi.jinqigfzy.top

================================================================================
来源：http://del.gzhubu.top

B. 流程控制
来源：http://umu.haohaochexian.top

================================================================================
来源：http://qzp.chenzaomai.com

[B01] 条件判断 if / else
来源：http://wzj.hammf.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tvr.chenjidiqi.icu

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wmu.shanyushiyangtech.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ley.sxryk.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nfb.haohaochexian.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://umb.yongpay.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jyb.hywenlv.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rtq.ywan-chungtsiang.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hcu.cqqwz.cn

[B02] 多分支 else if / elif
来源：http://zsq.haohaochexian.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tnm.sxryk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hrp.tian-w.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lpf.vehdjk.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kij.sxryk.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://npy.yj20258888.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ncv.aizwys.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dmt.kuanghao11.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pbp.jiagoushi.top

[B03] switch / match / case
来源：http://vmk.yanxiufei.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bwf.pycfn.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fuj.hnxiangtu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tmi.yj202588.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ptp.tian-w.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rql.dianchejie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://las.yj20258888.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jir.aizwys.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vnv.pycfn.com

[B04] for 计数循环
来源：http://kba.sjlbkw.cn

Py:   for i in range(10): print(i)
来源：http://nqc.andypj.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vod.zhixingplan.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://khg.jqgfzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://flj.hywenlv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oha.jqgufenzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vsq.shanyushiyangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://hmu.yongpay.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jmx.jinqigfzy.top

[B05] 遍历数组 / 列表
来源：http://vys.0kj1m.cn

Py:   for item in arr: print(item)
来源：http://xvo.nanxuanxn.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fxl.zdqjudy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://gxy.jqgufenzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://gqv.ywan-chungtsiang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://oxy.sweek.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cef.epnwcf.com

Ruby: arr.each { |item| puts item }
来源：http://njj.jinghuilouyu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fem.daria6918.cn

[B06] 遍历字典 / 对象
来源：http://thp.daxiang520.top

Py:   for k, v in d.items(): print(k, v)
来源：http://nkh.c1oappe.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jpr.9152youxi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jgp.ehwqpu.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qai.haohaochexian.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ehe.wangdashe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jco.fengsongda.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iwz.smart0.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vvl.feifeiyinyue.top

[B07] while 循环
来源：http://isp.daria6918.cn

Py:   while i < 10: i += 1
来源：http://gvi.zhoulong.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://rkq.ppjwa.cn

JS:   while (i < 10) { i++; }
来源：http://seg.cucudq.cn

TS:   while (i < 10) { i++; }
来源：http://nvz.zhengqikj.top

Java: while (i < 10) { i++; }
来源：http://fwp.yj20258.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dmi.pengpengdd.cyou

Ruby: while i < 10; i += 1; end
来源：http://miz.zdbjq.cn

C#:   while (i < 10) { i++; }
来源：http://jkr.hywenlv.cn

[B08] do-while（至少执行一次）
来源：http://srk.birdmap.top

Py:   # 无 do-while：用 while True + break
来源：http://qin.zhongyouzk.top

PHP:  do { $i++; } while ($i < 10);
来源：http://qem.0kj1m.cn

JS:   do { i++; } while (i < 10);
来源：http://xux.bjfxy.top

TS:   do { i++; } while (i < 10);
来源：http://gxr.zycfv.cn

Java: do { i++; } while (i < 10);
来源：http://muh.jqgufenzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://itg.xuetiantiany.cn

Ruby: begin; i += 1; end while i < 10
来源：http://elj.zdqjudy.top

C#:   do { i++; } while (i < 10);
来源：http://qbs.ctjpmb.com

[B09] break 与 continue
来源：http://rqh.ivvv.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qhd.yonumen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ncb.bjfxy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qki.bbcook.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://miw.wangdashe.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yar.wangdashe.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ztt.chenjidiqi.icu

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hcv.zhongyouzk.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ssm.cucudq.cn

[B10] 遍历同时拿索引
来源：http://pmj.wangshuangyany.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yuu.svipenyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sik.iojbl.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://reg.shangyingyoupin.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ogt.ehwqpu.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://szz.jinqigufen.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tkv.ywan-chungtsiang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rjk.nanxinkj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wav.daxiang520.top

[B11] 生成数字序列 / 区间
来源：http://fbu.sufxvd.cn

Py:   list(range(0, 10, 2))
来源：http://qxr.ctjpmb.com

PHP:  range(0, 10, 2);
来源：http://iri.jinghuilouyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pbm.hnxiangtu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rbr.pengpengdd.cyou

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mfa.haohaochexian.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vmx.gaohongyu789.top

Ruby: (0...10).step(2).to_a
来源：http://uan.snrcjt.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jfh.haohaochexian.top

[B12] 跳出多层循环
来源：http://epz.316326.xyz


<!-- 参考信息 -->