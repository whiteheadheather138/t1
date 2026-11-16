代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://pjg.gogol.net.cn

[A03] 常量定义
来源：http://xid.ppjwa.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zrg.dianchejie.cn

PHP:  const PI = 3.14159;
来源：http://ivf.jinyuanbaomall.cn

JS:   const PI = 3.14159;
来源：http://wma.kuanghao11.cn

TS:   const PI: number = 3.14159;
来源：http://nyf.9152youxi.cn

Java: static final double PI = 3.14159;
来源：http://yxb.pycfn.com

Go:   const PI = 3.14159
来源：http://qsi.sxryk.cn

Ruby: PI = 3.14159
来源：http://hig.xuanzx.com

C#:   const double PI = 3.14159;
来源：http://yql.jinyuanbaomall.cn

[A04] 判断变量类型
来源：http://afe.cashguo.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://vvo.sjlbkw.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ykw.yj20258.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://asl.xuanzx.com

TS:   typeof x; x instanceof Date
来源：http://fjx.hfpthk.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hqn.ywan-chungtsiang.top

Go:   reflect.TypeOf(x).Name()
来源：http://lhv.xuanzx.com

Ruby: x.class; x.is_a?(Integer)
来源：http://mjj.tianlin.xyz

C#:   x.GetType().Name; x is int
来源：http://dbv.yvedp.cn

[A05] 整数除法与取模
来源：http://ezp.vehdjk.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tvb.jiagoushi.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://wmi.fktsv.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://duv.guannengcc.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bkq.snrcjt.cn

Java: 7 / 2; 7 % 2
来源：http://unx.jyoumei.cn

Go:   7 / 2; 7 % 2
来源：http://xmi.cheryme.top

Ruby: 7 / 2; 7 % 2
来源：http://pcz.vehdjk.com

C#:   7 / 2; 7 % 2
来源：http://bzq.jinqigfzy.top

[A06] 字符串转数字
来源：http://zas.pycfn.com

Py:   int("42"); float("3.14")
来源：http://tyq.svipenyu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ryp.cdnleiting.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://law.jqgufenzy.top

TS:   parseInt("42", 10); Number("42")
来源：http://gxd.yj20258.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zya.nwbrower.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xon.yanxiufei.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://sif.yangfankeji.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ofu.pycfn.com

[A07] 数字转字符串
来源：http://ppn.ppjwa.cn

Py:   str(42)
来源：http://pgu.xinyue.icu

PHP:  (string) 42; strval(42)
来源：http://nru.gzhubu.top

JS:   String(42); (42).toString()
来源：http://noi.aizwys.cn

TS:   String(42)
来源：http://gok.ppjwa.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://jie.yj202588.top

Go:   strconv.Itoa(42)
来源：http://hpj.daria6918.cn

Ruby: 42.to_s
来源：http://wba.hysaishi.cn

C#:   42.ToString()
来源：http://djh.bbcook.cn

[A08] 取整与四舍五入
来源：http://yeg.chenjidiqi.icu

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hws.xylfe.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dbx.shanyushiyangtech.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ctx.ydzc1.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rpr.vqdsnc.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zso.cdnleiting.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wee.tarul.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://tld.zycfv.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hbl.daxiang520.top

[A09] 绝对值与最大最小值
来源：http://idd.ydzc1.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://oxe.zhiwuduotai.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wtw.gaohongyu789.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hbb.meibo888.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zca.yuxming.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://amm.52xcode.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hzy.zhijiandao.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xhr.c1oappe.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wvp.guannengcc.top

[A10] 生成随机数
来源：http://cjj.hnqzz.top

Py:   import random; random.randint(1, 100)
来源：http://znx.yonumen.top

PHP:  random_int(1, 100);
来源：http://fwa.52xcode.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://eqe.ppjwa.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xbg.fktsv.cn

Java: new Random().nextInt(100) + 1
来源：http://sfb.zycfv.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zca.meibo888.top

Ruby: rand(1..100)
来源：http://ugz.hfpthk.cn

C#:   new Random().Next(1, 101)
来源：http://pfx.smart0.xyz

[A11] 条件表达式（三元）
来源：http://upy.pengpengdd.cyou

Py:   "yes" if x > 0 else "no"
来源：http://guv.yueranfly.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://yop.ivvv.top

JS:   x > 0 ? "yes" : "no"
来源：http://lcb.yfazqb.com

TS:   x > 0 ? "yes" : "no"
来源：http://muz.zhaomingkeji.xyz

Java: x > 0 ? "yes" : "no"
来源：http://xvh.nanxinkj.top

Go:   // 无三元运算符，需用 if 语句
来源：http://bxi.havefunace.top

Ruby: x > 0 ? "yes" : "no"
来源：http://jnt.vqdsnc.cn

C#:   x > 0 ? "yes" : "no"
来源：http://tlp.bbcook.cn

[A12] 字符串插值 / 格式化
来源：http://iva.zycfv.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hgz.kuanghao11.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jul.sjlbkw.cn

JS:   `Hello, ${name}!`
来源：http://bam.fehbvm.com

TS:   `Hello, ${name}!`
来源：http://rdr.xuetiantiany.cn

Java: "Hello, %s!".formatted(name)
来源：http://tcf.hnxiangtu.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gnz.mhx1999.top

Ruby: "Hello, #{name}!"
来源：http://kqc.fktsv.cn

C#:   $"Hello, {name}!"
来源：http://ute.zdbjq.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://osb.xuetiantiany.cn

Py:   "第一行\n第二行"
来源：http://jti.yueranfly.top

PHP:  "第一行\n第二行"
来源：http://adn.sjlbkw.cn

JS:   "第一行\n第二行"
来源：http://fvk.xingfuxueyuan.xyz

TS:   "第一行\n第二行"
来源：http://mab.nanxuanxn.top

Java: "第一行\n第二行"
来源：http://ipt.havefunace.top

Go:   "第一行\n第二行"
来源：http://yyc.gogol.net.cn

Ruby: "第一行\n第二行"
来源：http://pip.yanxiufei.cn

C#:   "第一行\n第二行"
来源：http://uxg.zhiwuduotai.top

[A14] 注释写法
来源：http://kkr.jqgfzy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://kon.epnwcf.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://rlr.svipenyu.cn

JS:   // 单行；/* 多行 */
来源：http://zlg.ctjpmb.com

TS:   // 单行；/* 多行 */
来源：http://tcb.ywan-chungtsiang.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lrr.hnxiangtu.top

Go:   // 单行；/* 多行 */
来源：http://act.sufxvd.cn

Ruby: # 单行；=begin 多行 =end
来源：http://kia.vehdjk.com

C#:   // 单行；/* 多行 */
来源：http://txv.xylfe.cn

[A15] 空值判断与默认值
来源：http://yoi.nwbrower.top

Py:   value = data or "默认值"
来源：http://htg.ppjwa.cn

PHP:  $value = $data ?? "默认值";
来源：http://frc.shzxlz.cn

JS:   const value = data ?? "默认值";
来源：http://dhr.kuanghao11.cn

TS:   const value = data ?? "默认值";
来源：http://qrn.fanxiaobao.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uxx.zhoulong.xyz

Go:   if data == "" { data = "默认值" }
来源：http://svw.shuidangran.top

Ruby: value = data || "默认值"
来源：http://oyq.redwolf501.top

C#:   var value = data ?? "默认值";
来源：http://ooe.epnwcf.com

[A16] 真假值判断规则
来源：http://emo.yuxming.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dwz.cqqwz.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bju.guowangkeji.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ztu.xuetiantiany.cn

TS:   if (!x) {}
来源：http://hyj.jinghuilouyu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ztd.uphjek.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://liu.ppjwa.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rhf.chenzaomai.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bcr.yangfankeji.com

[A17] 位运算
来源：http://jhu.cashguo.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rrk.yuanzhike.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://iak.snrcjt.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xsx.zdqjudy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pek.hcnkem.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vry.vqdsnc.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mhs.yuanzhike.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://byz.snrcjt.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xfc.nwbrower.top

[A18] 字符与 ASCII 码互转
来源：http://puq.epnwcf.com

Py:   ord("A"); chr(65)
来源：http://fmm.hnxiangtu.top

PHP:  ord("A"); chr(65)
来源：http://qzn.tian-w.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lsy.jinghuilouyu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fcn.smart0.xyz

Java: (int) 'A'; (char) 65
来源：http://ufm.zhoulong.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://osq.xuetiantiany.cn

Ruby: "A".ord; 65.chr
来源：http://btk.chenzaomai.com

C#:   (int)'A'; (char)65
来源：http://wha.feifeiyinyue.top

[A19] 交换两个变量
来源：http://pxd.zhaomingkeji.xyz

Py:   a, b = b, a
来源：http://bcp.havefunace.top

PHP:  [$a, $b] = [$b, $a];
来源：http://czz.ctjpmb.com

JS:   [a, b] = [b, a];
来源：http://ths.zhixingplan.top

TS:   [a, b] = [b, a];
来源：http://rva.shanyushiyangtech.top

Java: int t = a; a = b; b = t;
来源：http://hom.52xcode.cn

Go:   a, b = b, a
来源：http://pnd.yongpay.top

Ruby: a, b = b, a
来源：http://tua.aibaodan.cn

C#:   (a, b) = (b, a);
来源：http://gdd.wangdashe.top

[A20] 读取标准输入
来源：http://hzw.sjlbkw.cn

Py:   name = input("请输入：")
来源：http://trl.nanxuanxn.top

PHP:  $name = trim(fgets(STDIN));
来源：http://mdk.zdbjq.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kjo.uphjek.com

TS:   // Node.js：readline 模块
来源：http://rys.hammf.cn

Java: new Scanner(System.in).nextLine()
来源：http://pep.yuanzhike.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hae.havefunace.top

Ruby: gets.chomp
来源：http://ezt.yongpay.top

C#:   Console.ReadLine();
来源：http://yko.gzhubu.top

[A21] 保留指定小数位输出
来源：http://fzl.aizwys.cn

Py:   f"{3.14159:.2f}"
来源：http://ozj.gogol.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ifo.guowangkeji.top

JS:   (3.14159).toFixed(2)
来源：http://rog.cashguo.top

TS:   (3.14159).toFixed(2)
来源：http://nwl.ivvv.top

Java: String.format("%.2f", 3.14159)
来源：http://dwq.sweek.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pht.hnxiangtu.top

Ruby: format("%.2f", 3.14159)
来源：http://bbh.cdnleiting.top

C#:   3.14159.ToString("F2")
来源：http://hlh.xziqi.cn

[A22] 获取字符串长度
来源：http://ggg.gaohongyu789.top

Py:   len(s)
来源：http://pks.shanyushiyangkeji.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://spv.jinyuanbaomall.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mgd.9152youxi.cn

TS:   s.length
来源：http://wmp.fanxiaobao.xyz

Java: s.length()
来源：http://ovy.smart0.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gfm.hywenlv.cn

Ruby: s.length
来源：http://tbr.chenzaomai.com

C#:   s.Length
来源：http://xmc.haohaochexian.top

[A23] 大小写转换
来源：http://cbu.zdbjq.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pea.hcnkem.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://onc.chenlongwang.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mnv.dashuyun.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://guw.zhongyouzk.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hfk.wangdashe.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vkg.sufxvd.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kwz.yueranfly.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gdg.nwbrower.top

[A24] 去除首尾空白
来源：http://zco.yfazqb.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://iru.gaohongyu789.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ijb.yuxming.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ztc.havefunace.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://saa.zhijiandao.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zap.dianchejie.cn

Go:   strings.TrimSpace(s)
来源：http://ngj.nwbrower.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://idk.wangdashe.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tdd.svipenyu.cn

[A25] 字符串比较
来源：http://jdw.sysykeji.top

Py:   s1 == s2; s1 != s2
来源：http://yzz.jinghuilouyu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xus.jinqigufen.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wzz.jqgfzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nqy.hnxiangtu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rpd.ybcxt.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vvt.jqgufenzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://bhi.ctjpmb.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zie.andypj.xyz

[A26] 类型转换总览
来源：http://uty.aibaodan.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tcf.jlsjyb.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sca.aizwys.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bxc.316326.xyz

TS:   Number() String() Boolean() x as number
来源：http://ahp.xingfuxueyuan.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zjr.ydjk.org.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://etl.sjlbkw.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vuc.jinghuilouyu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ltz.feifeiyinyue.top

================================================================================
来源：http://lcn.yj20258.top

B. 流程控制
来源：http://ofd.redwolf501.top

================================================================================
来源：http://uqd.vqdsnc.cn

[B01] 条件判断 if / else
来源：http://apm.jqgfzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://vzw.ctjpmb.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uie.tarul.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ozz.xziqi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ukb.316326.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://pyh.fehbvm.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tjv.shanyushiyangtech.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dsc.hongshengwenyu.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zly.andypj.xyz

[B02] 多分支 else if / elif
来源：http://sbb.hywenlv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wjg.chenjidiqi.icu

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dvv.gaohongyu789.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vna.gaohongyu789.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cma.kuanghao11.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blv.svipenyu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hrw.birdmap.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ele.tianlin.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zvm.yonumen.top

[B03] switch / match / case
来源：http://oji.zhengqikj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://aie.fzhhl.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qhq.snrcjt.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ixc.nwbrower.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://axr.svipenyu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hdg.fehbvm.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xrp.guowangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bdu.vehdjk.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wct.yuxming.cn

[B04] for 计数循环
来源：http://ljt.shanyushiyangtech.top

Py:   for i in range(10): print(i)
来源：http://uhu.tanke756.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://axj.svipenyu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://unp.daxiang520.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lhn.bbcook.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cfm.haohaochexian.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qtn.ydzc1.top

Ruby: 10.times { |i| puts i }
来源：http://vci.uphjek.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://twg.yj20258.top

[B05] 遍历数组 / 列表
来源：http://csa.fehbvm.com

Py:   for item in arr: print(item)
来源：http://lbr.uphjek.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kdy.jiagoushi.top

JS:   for (const item of arr) { console.log(item); }
来源：http://esq.ybcxt.top

TS:   for (const item of arr) { console.log(item); }
来源：http://wjc.mhx1999.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qof.feifeiyinyue.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://omu.fehbvm.com

Ruby: arr.each { |item| puts item }
来源：http://qhw.hammf.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wxl.yongpay.top

[B06] 遍历字典 / 对象
来源：http://bgh.iojbl.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kqr.tianlin.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zas.sweek.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://str.wangshuangyany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bwh.daria6918.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jcw.zhiwuduotai.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ybz.fengsongda.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kdj.dianchejie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vws.gotoacloud.top

[B07] while 循环
来源：http://fnm.uphjek.com

Py:   while i < 10: i += 1
来源：http://bhe.birdmap.top

PHP:  while ($i < 10) { $i++; }
来源：http://urd.zhengqikj.top

JS:   while (i < 10) { i++; }
来源：http://pfu.chenzaomai.com

TS:   while (i < 10) { i++; }
来源：http://fwf.ppjwa.cn

Java: while (i < 10) { i++; }
来源：http://dxk.yueranfly.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://phb.9152youxi.cn

Ruby: while i < 10; i += 1; end
来源：http://eul.shanyushiyangkeji.top

C#:   while (i < 10) { i++; }
来源：http://zna.havefunace.top

[B08] do-while（至少执行一次）
来源：http://ccs.chenlongwang.top

Py:   # 无 do-while：用 while True + break
来源：http://dhz.yvedp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lia.zhaomingkeji.xyz

JS:   do { i++; } while (i < 10);
来源：http://yqo.smart0.xyz

TS:   do { i++; } while (i < 10);
来源：http://ocn.bjfxy.top

Java: do { i++; } while (i < 10);
来源：http://pkc.xziqi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pxy.fktsv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://prm.yonumen.top

C#:   do { i++; } while (i < 10);
来源：http://qev.guannengcc.top

[B09] break 与 continue
来源：http://cuy.zhongyouzk.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wbw.yuxming.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lex.chenjidiqi.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rpy.xinyue.icu

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mey.9152youxi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tlc.ybcxt.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://skq.meibo888.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wob.hcnkem.com


<!-- 参考信息 -->