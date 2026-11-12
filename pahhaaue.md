代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ghu.shzxlz.cn

Java: String name = "Alex"; int age = 20;
来源：http://tpm.vehdjk.com

Go:   name := "Alex"; age := 20
来源：http://thj.feifeiyinyue.top

Ruby: name = "Alex"; age = 20
来源：http://igq.feifeiyinyue.top

C#:   string name = "Alex"; int age = 20;
来源：http://xhv.svipenyu.cn

[A03] 常量定义
来源：http://yls.yuanzhike.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cha.fzhhl.top

PHP:  const PI = 3.14159;
来源：http://yxz.dashuyun.cn

JS:   const PI = 3.14159;
来源：http://lov.gogol.net.cn

TS:   const PI: number = 3.14159;
来源：http://ieg.zdqjudy.top

Java: static final double PI = 3.14159;
来源：http://vob.kuanghao11.cn

Go:   const PI = 3.14159
来源：http://ziw.feifeiyinyue.top

Ruby: PI = 3.14159
来源：http://wjq.xingfuxueyuan.xyz

C#:   const double PI = 3.14159;
来源：http://wzv.ivvv.top

[A04] 判断变量类型
来源：http://ezz.gzhubu.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://egd.ywan-chungtsiang.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://whk.yanxiufei.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mtc.jlsjyb.cn

TS:   typeof x; x instanceof Date
来源：http://baz.chenjidiqi.icu

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mnk.yanxiufei.cn

Go:   reflect.TypeOf(x).Name()
来源：http://snf.yj20258888.top

Ruby: x.class; x.is_a?(Integer)
来源：http://utz.sxryk.cn

C#:   x.GetType().Name; x is int
来源：http://rdq.gogol.net.cn

[A05] 整数除法与取模
来源：http://rkf.chenzaomai.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pqc.hongshengwenyu.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://dgc.fzhhl.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vys.hysaishi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rpw.9152youxi.cn

Java: 7 / 2; 7 % 2
来源：http://iyq.aizwys.cn

Go:   7 / 2; 7 % 2
来源：http://iba.zhijiandao.cn

Ruby: 7 / 2; 7 % 2
来源：http://zbu.jinqigfzy.top

C#:   7 / 2; 7 % 2
来源：http://ryq.nanxuanxn.top

[A06] 字符串转数字
来源：http://iyx.fzhhl.top

Py:   int("42"); float("3.14")
来源：http://bth.tanke756.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tnp.zhiwuduotai.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xlj.c1oappe.top

TS:   parseInt("42", 10); Number("42")
来源：http://emz.ywan-chungtsiang.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bmi.zhijiandao.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kye.bjfxy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://zwu.9152youxi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nia.xuanzx.com

[A07] 数字转字符串
来源：http://hpq.bjfxy.top

Py:   str(42)
来源：http://tkb.cucudq.cn

PHP:  (string) 42; strval(42)
来源：http://van.gzhubu.top

JS:   String(42); (42).toString()
来源：http://joe.jinqigufen.top

TS:   String(42)
来源：http://xuu.xingfuxueyuan.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://qfa.cashguo.top

Go:   strconv.Itoa(42)
来源：http://ojh.kuanghao11.cn

Ruby: 42.to_s
来源：http://hhf.xylfe.cn

C#:   42.ToString()
来源：http://kjf.svipenyu.cn

[A08] 取整与四舍五入
来源：http://qhc.yueranfly.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jbb.guannengcc.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://oae.hywenlv.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://azz.yongpay.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bqi.andypj.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wgj.zhoulong.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nta.chenjidiqi.icu

Ruby: 3.567.round(2); 3.9.floor
来源：http://fah.yueranfly.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hkq.redwolf501.top

[A09] 绝对值与最大最小值
来源：http://owt.yvedp.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lst.ivvv.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ehy.ydzc1.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gwb.tanke756.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wqq.sufxvd.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://itk.sjlbkw.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://liu.gotoacloud.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ccf.xuanzx.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lll.vehdjk.com

[A10] 生成随机数
来源：http://wzy.pycfn.com

Py:   import random; random.randint(1, 100)
来源：http://gfj.haohaochexian.top

PHP:  random_int(1, 100);
来源：http://vtx.pycfn.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://anj.ydzc1.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ebx.ydjk.org.cn

Java: new Random().nextInt(100) + 1
来源：http://pfg.hfpthk.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nxf.316326.xyz

Ruby: rand(1..100)
来源：http://wka.jinqigufen.top

C#:   new Random().Next(1, 101)
来源：http://ype.hfpthk.cn

[A11] 条件表达式（三元）
来源：http://ddc.chenjidiqi.icu

Py:   "yes" if x > 0 else "no"
来源：http://ssh.kuanghao11.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ztf.zdqjudy.top

JS:   x > 0 ? "yes" : "no"
来源：http://fqf.tian-w.cn

TS:   x > 0 ? "yes" : "no"
来源：http://etu.yangfankeji.com

Java: x > 0 ? "yes" : "no"
来源：http://tiq.smart0.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://quz.jqgufenzy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://tgh.vehdjk.com

C#:   x > 0 ? "yes" : "no"
来源：http://scg.yongpay.top

[A12] 字符串插值 / 格式化
来源：http://ktm.yj202588.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ofs.ctjpmb.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xvc.yvedp.cn

JS:   `Hello, ${name}!`
来源：http://hka.fanxiaobao.xyz

TS:   `Hello, ${name}!`
来源：http://oti.haohaochexian.top

Java: "Hello, %s!".formatted(name)
来源：http://sza.snrcjt.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mrk.yj202588.top

Ruby: "Hello, #{name}!"
来源：http://lwa.fengsongda.top

C#:   $"Hello, {name}!"
来源：http://qzy.cqqwz.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://foj.yvedp.cn

Py:   "第一行\n第二行"
来源：http://ylc.havefunace.top

PHP:  "第一行\n第二行"
来源：http://jjj.yanxiufei.cn

JS:   "第一行\n第二行"
来源：http://ssh.sweek.top

TS:   "第一行\n第二行"
来源：http://ejq.feifeiyinyue.top

Java: "第一行\n第二行"
来源：http://gue.zhiwuduotai.top

Go:   "第一行\n第二行"
来源：http://vxi.tian-w.cn

Ruby: "第一行\n第二行"
来源：http://vzj.hywenlv.cn

C#:   "第一行\n第二行"
来源：http://ydj.gogol.net.cn

[A14] 注释写法
来源：http://wlr.jianghu66.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://fwe.hnqzz.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://gdn.ppjwa.cn

JS:   // 单行；/* 多行 */
来源：http://dcl.yongpay.top

TS:   // 单行；/* 多行 */
来源：http://idp.kuanghao11.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://idu.hysaishi.cn

Go:   // 单行；/* 多行 */
来源：http://hli.jinqigfzy.top

Ruby: # 单行；=begin 多行 =end
来源：http://zjh.xuetiantiany.cn

C#:   // 单行；/* 多行 */
来源：http://tug.smart0.xyz

[A15] 空值判断与默认值
来源：http://xno.sufxvd.cn

Py:   value = data or "默认值"
来源：http://gox.52xcode.cn

PHP:  $value = $data ?? "默认值";
来源：http://bbf.ivvv.top

JS:   const value = data ?? "默认值";
来源：http://eyu.jqgufenzy.top

TS:   const value = data ?? "默认值";
来源：http://aii.ehwqpu.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qaz.jlsjyb.cn

Go:   if data == "" { data = "默认值" }
来源：http://gje.yongpay.top

Ruby: value = data || "默认值"
来源：http://qsx.gotoacloud.top

C#:   var value = data ?? "默认值";
来源：http://flo.hysaishi.cn

[A16] 真假值判断规则
来源：http://pbq.zhijiandao.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://uoz.hysaishi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cwv.cdnleiting.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ies.shanyushiyangtech.top

TS:   if (!x) {}
来源：http://hnj.nwbrower.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://sby.yongpay.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://stv.andypj.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://qcu.zycfv.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fac.zhaomingkeji.xyz

[A17] 位运算
来源：http://hze.vehdjk.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qaq.fengsongda.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://its.chenjidiqi.icu

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aky.yuxming.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dly.cheryme.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rsm.zdqjudy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kjt.hcnkem.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://azx.shangyingyoupin.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mjq.chenjidiqi.icu

[A18] 字符与 ASCII 码互转
来源：http://uhv.vehdjk.com

Py:   ord("A"); chr(65)
来源：http://ybz.ivvv.top

PHP:  ord("A"); chr(65)
来源：http://sgc.fanxiaobao.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ptp.sysykeji.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://csn.fzhhl.top

Java: (int) 'A'; (char) 65
来源：http://cul.yueranfly.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://eoh.zdqjudy.top

Ruby: "A".ord; 65.chr
来源：http://cob.hcnkem.com

C#:   (int)'A'; (char)65
来源：http://nlj.aizwys.cn

[A19] 交换两个变量
来源：http://qmi.shzxlz.cn

Py:   a, b = b, a
来源：http://jxp.yanxiufei.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://prk.cheryme.top

JS:   [a, b] = [b, a];
来源：http://xee.chenjidiqi.icu

TS:   [a, b] = [b, a];
来源：http://fkf.jianghu66.top

Java: int t = a; a = b; b = t;
来源：http://foh.ybcxt.top

Go:   a, b = b, a
来源：http://adv.hesvh.cn

Ruby: a, b = b, a
来源：http://svd.ydjk.org.cn

C#:   (a, b) = (b, a);
来源：http://pyp.yvedp.cn

[A20] 读取标准输入
来源：http://dzn.ehwqpu.com

Py:   name = input("请输入：")
来源：http://hiu.guannengcc.top

PHP:  $name = trim(fgets(STDIN));
来源：http://lqp.chenjidiqi.icu

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bag.hcnkem.com

TS:   // Node.js：readline 模块
来源：http://xkv.smart0.xyz

Java: new Scanner(System.in).nextLine()
来源：http://qzs.fehbvm.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://uew.cucudq.cn

Ruby: gets.chomp
来源：http://dzx.fehbvm.com

C#:   Console.ReadLine();
来源：http://twa.dashuyun.cn

[A21] 保留指定小数位输出
来源：http://prh.wangdashe.top

Py:   f"{3.14159:.2f}"
来源：http://skm.jinyuanbaomall.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kfk.cdnleiting.top

JS:   (3.14159).toFixed(2)
来源：http://gxk.chenjidiqi.icu

TS:   (3.14159).toFixed(2)
来源：http://gxd.ehwqpu.com

Java: String.format("%.2f", 3.14159)
来源：http://hkl.jinghuilouyu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vpt.pengpengdd.cyou

Ruby: format("%.2f", 3.14159)
来源：http://kni.sjlbkw.cn

C#:   3.14159.ToString("F2")
来源：http://sxi.52xcode.cn

[A22] 获取字符串长度
来源：http://urv.sufxvd.cn

Py:   len(s)
来源：http://ktw.316326.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://avv.zhongyouzk.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sjm.jinyuanbaomall.cn

TS:   s.length
来源：http://gsd.bjfxy.top

Java: s.length()
来源：http://btt.pengpengdd.cyou

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ojq.tarul.cn

Ruby: s.length
来源：http://wsm.sysykeji.top

C#:   s.Length
来源：http://gwa.zhaomingkeji.xyz

[A23] 大小写转换
来源：http://qor.zhoulong.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://pwq.meibo888.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xjq.xinyue.icu

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yhp.zdqjudy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qkj.yueranfly.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rte.ydzc1.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nku.zhengqikj.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://erg.316326.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://rwt.hysaishi.cn

[A24] 去除首尾空白
来源：http://sgd.chenjidiqi.icu

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dpg.zhijiandao.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mqv.haohaochexian.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cbk.guannengcc.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vmu.iojbl.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hvv.daxiang520.top

Go:   strings.TrimSpace(s)
来源：http://psq.kuanghao11.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bvj.dianchejie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://knu.sjlbkw.cn

[A25] 字符串比较
来源：http://eea.havefunace.top

Py:   s1 == s2; s1 != s2
来源：http://akq.hnxiangtu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pjj.xylfe.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mlx.xinyue.icu

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tik.svipenyu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vbj.jyoumei.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gxv.fktsv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://irf.tanke756.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://goc.sjlbkw.cn

[A26] 类型转换总览
来源：http://grl.hongshengwenyu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cvb.yangfankeji.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ejv.zhoulong.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lds.havefunace.top

TS:   Number() String() Boolean() x as number
来源：http://uee.shzxlz.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://znr.yuanzhike.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xsz.yj202588.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://mya.fzhhl.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rhm.havefunace.top

================================================================================
来源：http://ftu.zhoulong.xyz

B. 流程控制
来源：http://qzp.cdnleiting.top

================================================================================
来源：http://zbf.uphjek.com

[B01] 条件判断 if / else
来源：http://uhr.cucudq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ncf.zycfv.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://auv.yj20258.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zcy.cucudq.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ysn.tanke756.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://dxg.shanyushiyangkeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://plh.jinqigufen.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dnf.shangyingyoupin.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fok.zhixingplan.top

[B02] 多分支 else if / elif
来源：http://aaf.xuetiantiany.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uvp.yangfankeji.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ovv.hywenlv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://awr.jiagoushi.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bbg.daria6918.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jtc.ywan-chungtsiang.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://npn.chenjidiqi.icu

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wjf.sweek.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yhi.yonumen.top

[B03] switch / match / case
来源：http://gfi.gzhubu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hkm.cdnleiting.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rto.ydzc1.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zoj.ctjpmb.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rbp.jyoumei.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wlf.hfpthk.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eef.snrcjt.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tdw.yuxming.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ndh.yj20258888.top

[B04] for 计数循环
来源：http://wjk.jqgfzy.top

Py:   for i in range(10): print(i)
来源：http://nhx.zhengqikj.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hnt.hnqzz.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ial.jinyuanbaomall.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://opi.shuidangran.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ixq.ppjwa.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tps.zhixingplan.top

Ruby: 10.times { |i| puts i }
来源：http://skw.yonumen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jqb.nwbrower.top

[B05] 遍历数组 / 列表
来源：http://rmv.feifeiyinyue.top

Py:   for item in arr: print(item)
来源：http://cpa.fktsv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ltt.zhiwuduotai.top

JS:   for (const item of arr) { console.log(item); }
来源：http://cst.yuxming.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ksi.ppjwa.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hrg.ydzc1.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blg.yongpay.top

Ruby: arr.each { |item| puts item }
来源：http://pge.cashguo.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vml.wangshuangyany.cn

[B06] 遍历字典 / 对象
来源：http://bsm.daria6918.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://znz.fengsongda.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://djv.hcnkem.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://spp.jqgufenzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kfp.nanxinkj.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vxn.daria6918.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bdp.fehbvm.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bdm.jqgufenzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pfm.fktsv.cn

[B07] while 循环
来源：http://gqs.316326.xyz

Py:   while i < 10: i += 1
来源：http://gyu.yuxming.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jhv.xinyue.icu

JS:   while (i < 10) { i++; }
来源：http://kjh.shangyingyoupin.top

TS:   while (i < 10) { i++; }
来源：http://nyf.daxiang520.top

Java: while (i < 10) { i++; }
来源：http://nms.jianghu66.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xno.xuetiantiany.cn

Ruby: while i < 10; i += 1; end
来源：http://kdv.zhiwuduotai.top

C#:   while (i < 10) { i++; }
来源：http://bau.fengsongda.top

[B08] do-while（至少执行一次）
来源：http://dve.c1oappe.top

Py:   # 无 do-while：用 while True + break
来源：http://tyv.zhoulong.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://kku.hcnkem.com

JS:   do { i++; } while (i < 10);
来源：http://jgl.ydzc1.top

TS:   do { i++; } while (i < 10);
来源：http://uvt.xinyue.icu

Java: do { i++; } while (i < 10);
来源：http://xpu.tanke756.top

Go:   for { i++; if i >= 10 { break } }
来源：http://whz.smart0.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://rvs.0kj1m.cn

C#:   do { i++; } while (i < 10);
来源：http://rpi.hongshengwenyu.top

[B09] break 与 continue
来源：http://kcm.hongshengwenyu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yfe.tianlin.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fts.sysykeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qus.ehwqpu.com


<!-- 参考信息 -->