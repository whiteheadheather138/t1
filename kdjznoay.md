代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://asg.jinghuilouyu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qqw.mhx1999.top

C#:   x.GetType().Name; x is int
来源：http://zzz.hcnkem.com

[A05] 整数除法与取模
来源：http://dcy.bbcook.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://abn.yvedp.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://put.52xcode.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dut.meibo888.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fhn.mhx1999.top

Java: 7 / 2; 7 % 2
来源：http://vec.ywan-chungtsiang.top

Go:   7 / 2; 7 % 2
来源：http://rij.chenjidiqi.icu

Ruby: 7 / 2; 7 % 2
来源：http://uzo.gogol.net.cn

C#:   7 / 2; 7 % 2
来源：http://hrm.tanke756.top

[A06] 字符串转数字
来源：http://pqf.guannengcc.top

Py:   int("42"); float("3.14")
来源：http://gec.jyoumei.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kuy.zycfv.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xbe.sysykeji.top

TS:   parseInt("42", 10); Number("42")
来源：http://cgw.yuxming.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bcn.xinyue.icu

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ojs.yj202588.top

Ruby: "42".to_i; "3.14".to_f
来源：http://dku.pycfn.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gfq.jinghuilouyu.cn

[A07] 数字转字符串
来源：http://ojb.zdqjudy.top

Py:   str(42)
来源：http://hsn.ehwqpu.com

PHP:  (string) 42; strval(42)
来源：http://dbw.yj202588.top

JS:   String(42); (42).toString()
来源：http://xdf.zhixingplan.top

TS:   String(42)
来源：http://lmw.yuanzhike.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://vgj.redwolf501.top

Go:   strconv.Itoa(42)
来源：http://dgd.sweek.top

Ruby: 42.to_s
来源：http://gfn.shzxlz.cn

C#:   42.ToString()
来源：http://cdc.redwolf501.top

[A08] 取整与四舍五入
来源：http://csp.pycfn.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uky.hnxiangtu.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://urv.zhengqikj.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jyg.ehwqpu.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cig.chenzaomai.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gvx.bjfxy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://opv.zycfv.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://dhg.hammf.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://duu.iojbl.cn

[A09] 绝对值与最大最小值
来源：http://qhs.hnxiangtu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xsi.iojbl.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hut.zhengqikj.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kzk.tarul.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pzl.snrcjt.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://enh.tianlin.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://duc.jinqigufen.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qtm.vqdsnc.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jqs.zhongyouzk.top

[A10] 生成随机数
来源：http://rzl.aizwys.cn

Py:   import random; random.randint(1, 100)
来源：http://cif.tanke756.top

PHP:  random_int(1, 100);
来源：http://pmt.yangfankeji.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://agt.hcnkem.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qff.zhaomingkeji.xyz

Java: new Random().nextInt(100) + 1
来源：http://lbz.xuanzx.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zxs.yfazqb.com

Ruby: rand(1..100)
来源：http://pjc.chenzaomai.com

C#:   new Random().Next(1, 101)
来源：http://zlt.guowangkeji.top

[A11] 条件表达式（三元）
来源：http://kwl.jiagoushi.top

Py:   "yes" if x > 0 else "no"
来源：http://jao.nwbrower.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://bhz.gzhubu.top

JS:   x > 0 ? "yes" : "no"
来源：http://riy.kuanghao11.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lin.sysykeji.top

Java: x > 0 ? "yes" : "no"
来源：http://wuy.52xcode.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://epc.fzhhl.top

Ruby: x > 0 ? "yes" : "no"
来源：http://kuj.sxryk.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ljc.shanyushiyangkeji.top

[A12] 字符串插值 / 格式化
来源：http://vag.nwbrower.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zyt.aizwys.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wyu.uphjek.com

JS:   `Hello, ${name}!`
来源：http://jya.sjlbkw.cn

TS:   `Hello, ${name}!`
来源：http://xqv.fanxiaobao.xyz

Java: "Hello, %s!".formatted(name)
来源：http://zdl.316326.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fdq.kuanghao11.cn

Ruby: "Hello, #{name}!"
来源：http://axj.hammf.cn

C#:   $"Hello, {name}!"
来源：http://txx.tian-w.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qxe.ywan-chungtsiang.top

Py:   "第一行\n第二行"
来源：http://enl.sweek.top

PHP:  "第一行\n第二行"
来源：http://idj.hysaishi.cn

JS:   "第一行\n第二行"
来源：http://fqz.hywenlv.cn

TS:   "第一行\n第二行"
来源：http://qrw.haohaochexian.top

Java: "第一行\n第二行"
来源：http://hvk.uphjek.com

Go:   "第一行\n第二行"
来源：http://rgt.snrcjt.cn

Ruby: "第一行\n第二行"
来源：http://ais.zycfv.cn

C#:   "第一行\n第二行"
来源：http://gxz.guannengcc.top

[A14] 注释写法
来源：http://ftd.zhaomingkeji.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://evd.fengsongda.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://nti.hesvh.cn

JS:   // 单行；/* 多行 */
来源：http://egf.cashguo.top

TS:   // 单行；/* 多行 */
来源：http://hvf.vehdjk.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://upy.shangyingyoupin.top

Go:   // 单行；/* 多行 */
来源：http://ree.yj202588.top

Ruby: # 单行；=begin 多行 =end
来源：http://qqq.sjlbkw.cn

C#:   // 单行；/* 多行 */
来源：http://csp.xuetiantiany.cn

[A15] 空值判断与默认值
来源：http://wyg.c1oappe.top

Py:   value = data or "默认值"
来源：http://ddj.daxiang520.top

PHP:  $value = $data ?? "默认值";
来源：http://lxb.fanxiaobao.xyz

JS:   const value = data ?? "默认值";
来源：http://fpm.pycfn.com

TS:   const value = data ?? "默认值";
来源：http://dhj.tianlin.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kos.dianchejie.cn

Go:   if data == "" { data = "默认值" }
来源：http://odh.yangfankeji.com

Ruby: value = data || "默认值"
来源：http://tut.snrcjt.cn

C#:   var value = data ?? "默认值";
来源：http://dhh.dashuyun.cn

[A16] 真假值判断规则
来源：http://why.meibo888.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ugg.yvedp.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dcq.aizwys.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mjo.cheryme.top

TS:   if (!x) {}
来源：http://suc.fktsv.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kou.birdmap.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xqs.cqqwz.cn

Ruby: unless x            # nil 与 false 为假
来源：http://dhc.sweek.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://iik.daria6918.cn

[A17] 位运算
来源：http://ypd.jyoumei.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hsz.ywan-chungtsiang.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ski.52xcode.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yrh.xylfe.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vmk.ydzc1.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kug.ydzc1.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://msx.zhongyouzk.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mns.yj20258888.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://opa.zhijiandao.cn

[A18] 字符与 ASCII 码互转
来源：http://ezy.meibo888.top

Py:   ord("A"); chr(65)
来源：http://xtt.hfpthk.cn

PHP:  ord("A"); chr(65)
来源：http://flw.dashuyun.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hut.nanxinkj.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wxd.tarul.cn

Java: (int) 'A'; (char) 65
来源：http://mir.quarkkingdee.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pyl.jianghu66.top

Ruby: "A".ord; 65.chr
来源：http://wyo.zdbjq.cn

C#:   (int)'A'; (char)65
来源：http://lpi.zdbjq.cn

[A19] 交换两个变量
来源：http://hbn.cashguo.top

Py:   a, b = b, a
来源：http://sbr.jiagoushi.top

PHP:  [$a, $b] = [$b, $a];
来源：http://lme.tianlin.xyz

JS:   [a, b] = [b, a];
来源：http://wmb.tianlin.xyz

TS:   [a, b] = [b, a];
来源：http://snu.zdqjudy.top

Java: int t = a; a = b; b = t;
来源：http://avm.nanxinkj.top

Go:   a, b = b, a
来源：http://soe.52xcode.cn

Ruby: a, b = b, a
来源：http://mrh.shanyushiyangkeji.top

C#:   (a, b) = (b, a);
来源：http://mfe.hongshengwenyu.top

[A20] 读取标准输入
来源：http://qih.fktsv.cn

Py:   name = input("请输入：")
来源：http://vfa.redwolf501.top

PHP:  $name = trim(fgets(STDIN));
来源：http://jgl.hcnkem.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://klh.jianghu66.top

TS:   // Node.js：readline 模块
来源：http://jzm.xinyue.icu

Java: new Scanner(System.in).nextLine()
来源：http://cnb.birdmap.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fui.yangfankeji.com

Ruby: gets.chomp
来源：http://mxd.9152youxi.cn

C#:   Console.ReadLine();
来源：http://tmg.sysykeji.top

[A21] 保留指定小数位输出
来源：http://ixs.ywan-chungtsiang.top

Py:   f"{3.14159:.2f}"
来源：http://bmt.snrcjt.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ewu.snrcjt.cn

JS:   (3.14159).toFixed(2)
来源：http://mxu.wangdashe.top

TS:   (3.14159).toFixed(2)
来源：http://fdg.zhiwuduotai.top

Java: String.format("%.2f", 3.14159)
来源：http://uaz.yueranfly.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jly.chenzaomai.com

Ruby: format("%.2f", 3.14159)
来源：http://sci.feifeiyinyue.top

C#:   3.14159.ToString("F2")
来源：http://oxc.zhoulong.xyz

[A22] 获取字符串长度
来源：http://zqn.ydzc1.top

Py:   len(s)
来源：http://mla.iojbl.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rpe.iojbl.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wps.shuidangran.top

TS:   s.length
来源：http://pdt.sxryk.cn

Java: s.length()
来源：http://paw.vehdjk.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://web.jinqigufen.top

Ruby: s.length
来源：http://avg.tanke756.top

C#:   s.Length
来源：http://fua.shuidangran.top

[A23] 大小写转换
来源：http://qfb.hcnkem.com

Py:   s.upper(); s.lower(); s.title()
来源：http://pqg.jlsjyb.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://acy.cdnleiting.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nmm.nanxuanxn.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mxa.pengpengdd.cyou

Java: s.toUpperCase(); s.toLowerCase()
来源：http://byu.ppjwa.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://voa.jlsjyb.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gmd.nwbrower.top

C#:   s.ToUpper(); s.ToLower()
来源：http://llf.nwbrower.top

[A24] 去除首尾空白
来源：http://bwq.jqgufenzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://npt.shuidangran.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xfk.ehwqpu.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mej.uphjek.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vrj.sysykeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dqu.feifeiyinyue.top

Go:   strings.TrimSpace(s)
来源：http://ytg.jinghuilouyu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://aqt.hysaishi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kal.yuanzhike.top

[A25] 字符串比较
来源：http://foh.cqqwz.cn

Py:   s1 == s2; s1 != s2
来源：http://mrb.yongpay.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://aqa.redwolf501.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pxu.chenjidiqi.icu

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://flx.shuidangran.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gti.zhijiandao.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ofn.jyoumei.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qjv.cashguo.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nhm.sysykeji.top

[A26] 类型转换总览
来源：http://obl.fanxiaobao.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dnq.ctjpmb.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://det.vqdsnc.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ofi.shzxlz.cn

TS:   Number() String() Boolean() x as number
来源：http://jvz.xuanzx.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://osj.dianchejie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ryy.jinyuanbaomall.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rgi.ywan-chungtsiang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vjt.smart0.xyz

================================================================================
来源：http://dtq.haohaochexian.top

B. 流程控制
来源：http://dvt.tianlin.xyz

================================================================================
来源：http://rgo.yueranfly.top

[B01] 条件判断 if / else
来源：http://poc.wangshuangyany.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ony.zhijiandao.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cge.wangdashe.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dyn.ppjwa.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://aat.shanyushiyangkeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://qtp.zhijiandao.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rfk.ppjwa.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bff.fengsongda.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jzd.yueranfly.top

[B02] 多分支 else if / elif
来源：http://pcf.epnwcf.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://akm.fanxiaobao.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ozg.nwbrower.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fxb.kuanghao11.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jpf.jianghu66.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ulb.zhaomingkeji.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://frb.hnqzz.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hci.cqqwz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gvl.zhengqikj.top

[B03] switch / match / case
来源：http://tll.aizwys.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dvi.ivvv.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wha.tian-w.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fqv.pycfn.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mgw.shuidangran.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://krl.hongshengwenyu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vrl.ywan-chungtsiang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uru.52xcode.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sdh.hongshengwenyu.top

[B04] for 计数循环
来源：http://vqt.shuidangran.top

Py:   for i in range(10): print(i)
来源：http://iol.jianghu66.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wew.ivvv.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oky.hywenlv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xps.zhongyouzk.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kbw.zdqjudy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mhv.ydzc1.top

Ruby: 10.times { |i| puts i }
来源：http://fks.cucudq.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vja.aibaodan.cn

[B05] 遍历数组 / 列表
来源：http://cqv.andypj.xyz

Py:   for item in arr: print(item)
来源：http://hho.shzxlz.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://byr.tian-w.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vve.fengsongda.top

TS:   for (const item of arr) { console.log(item); }
来源：http://wsq.dashuyun.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cur.hnqzz.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ima.yvedp.cn

Ruby: arr.each { |item| puts item }
来源：http://hll.nanxinkj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dwy.sxryk.cn

[B06] 遍历字典 / 对象
来源：http://cwy.iojbl.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://flj.jyoumei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mpg.shangyingyoupin.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://csz.wangdashe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lrj.nanxinkj.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bma.zhiwuduotai.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://erb.jinyuanbaomall.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fcm.guowangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://htv.jinghuilouyu.cn

[B07] while 循环
来源：http://noh.ppjwa.cn

Py:   while i < 10: i += 1
来源：http://ymo.ybcxt.top

PHP:  while ($i < 10) { $i++; }
来源：http://vjn.cheryme.top

JS:   while (i < 10) { i++; }
来源：http://gxl.havefunace.top

TS:   while (i < 10) { i++; }
来源：http://tux.shzxlz.cn

Java: while (i < 10) { i++; }
来源：http://xpj.nanxinkj.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://faj.yuxming.cn

Ruby: while i < 10; i += 1; end
来源：http://lct.hammf.cn

C#:   while (i < 10) { i++; }
来源：http://zzj.xingfuxueyuan.xyz

[B08] do-while（至少执行一次）
来源：http://pvd.dianchejie.cn

Py:   # 无 do-while：用 while True + break
来源：http://wyr.sxryk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vaw.ehwqpu.com

JS:   do { i++; } while (i < 10);
来源：http://gpp.quarkkingdee.top

TS:   do { i++; } while (i < 10);
来源：http://fbx.fehbvm.com

Java: do { i++; } while (i < 10);
来源：http://ajz.fktsv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tzi.snrcjt.cn

Ruby: begin; i += 1; end while i < 10
来源：http://uhu.chenlongwang.top

C#:   do { i++; } while (i < 10);
来源：http://ccv.jqgufenzy.top

[B09] break 与 continue
来源：http://qpl.cdnleiting.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://izo.cqqwz.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tmu.sxryk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://icn.meibo888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://onb.epnwcf.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dmi.ydzc1.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pmp.fehbvm.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vvb.jlsjyb.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lql.yuxming.cn

[B10] 遍历同时拿索引
来源：http://toe.sxryk.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://frn.aizwys.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vhz.chenlongwang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zpt.dashuyun.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gjc.ivvv.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://eie.gotoacloud.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xsk.tanke756.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cxh.chenjidiqi.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bpu.bjfxy.top

[B11] 生成数字序列 / 区间
来源：http://ddn.yvedp.cn

Py:   list(range(0, 10, 2))
来源：http://rnw.cdnleiting.top

PHP:  range(0, 10, 2);
来源：http://fft.chenzaomai.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xxb.sweek.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jol.ywan-chungtsiang.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cep.hammf.cn


<!-- 参考信息 -->