代发 wailian999

[A02] 变量声明与赋值
来源：http://abp.jlsjyb.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yyw.jinqigfzy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://iom.chenlongwang.top

JS:   let name = "Alex"; const age = 20;
来源：http://pju.feifeiyinyue.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kwi.pycfn.com

Java: String name = "Alex"; int age = 20;
来源：http://xdi.hnxiangtu.top

Go:   name := "Alex"; age := 20
来源：http://jcn.hnxiangtu.top

Ruby: name = "Alex"; age = 20
来源：http://zjd.birdmap.top

C#:   string name = "Alex"; int age = 20;
来源：http://wrp.gogol.net.cn

[A03] 常量定义
来源：http://xwo.c1oappe.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kog.sxryk.cn

PHP:  const PI = 3.14159;
来源：http://vqa.yuxming.cn

JS:   const PI = 3.14159;
来源：http://ohm.vehdjk.com

TS:   const PI: number = 3.14159;
来源：http://baa.iojbl.cn

Java: static final double PI = 3.14159;
来源：http://ams.daxiang520.top

Go:   const PI = 3.14159
来源：http://sdl.nanxinkj.top

Ruby: PI = 3.14159
来源：http://jqw.hfpthk.cn

C#:   const double PI = 3.14159;
来源：http://dxl.wangdashe.top

[A04] 判断变量类型
来源：http://mhn.chenzaomai.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://ios.wangshuangyany.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tov.pengpengdd.cyou

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ijr.hywenlv.cn

TS:   typeof x; x instanceof Date
来源：http://cbk.sjlbkw.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fss.pengpengdd.cyou

Go:   reflect.TypeOf(x).Name()
来源：http://gen.xuetiantiany.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gcw.yj202588.top

C#:   x.GetType().Name; x is int
来源：http://upn.aibaodan.cn

[A05] 整数除法与取模
来源：http://qsc.jqgufenzy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hrv.cheryme.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://lcu.wangshuangyany.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cnm.yvedp.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ynp.jqgfzy.top

Java: 7 / 2; 7 % 2
来源：http://mwk.shuidangran.top

Go:   7 / 2; 7 % 2
来源：http://xwu.xylfe.cn

Ruby: 7 / 2; 7 % 2
来源：http://ikq.zhengqikj.top

C#:   7 / 2; 7 % 2
来源：http://bng.zhengqikj.top

[A06] 字符串转数字
来源：http://yre.fehbvm.com

Py:   int("42"); float("3.14")
来源：http://yce.zhijiandao.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bpc.hammf.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sus.cheryme.top

TS:   parseInt("42", 10); Number("42")
来源：http://bgu.yuanzhike.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kqj.nanxuanxn.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://etp.quarkkingdee.top

Ruby: "42".to_i; "3.14".to_f
来源：http://fsz.ydzc1.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mnk.fehbvm.com

[A07] 数字转字符串
来源：http://wgt.fzhhl.top

Py:   str(42)
来源：http://ivq.ehwqpu.com

PHP:  (string) 42; strval(42)
来源：http://spn.yongpay.top

JS:   String(42); (42).toString()
来源：http://plq.wangshuangyany.cn

TS:   String(42)
来源：http://sby.feifeiyinyue.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ria.havefunace.top

Go:   strconv.Itoa(42)
来源：http://esx.gotoacloud.top

Ruby: 42.to_s
来源：http://bgk.chenzaomai.com

C#:   42.ToString()
来源：http://opi.jqgfzy.top

[A08] 取整与四舍五入
来源：http://hqr.yonumen.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cgz.cashguo.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://sir.xinyue.icu

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://woc.jinghuilouyu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tdl.yuanzhike.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ukm.nwbrower.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pwb.yj20258.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://wna.smart0.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.havefunace.top

[A09] 绝对值与最大最小值
来源：http://zpc.dashuyun.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pzx.jinqigfzy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ltb.hywenlv.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fic.bbcook.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jfx.hywenlv.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://usd.chenjidiqi.icu

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pln.haohaochexian.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kun.sweek.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pfq.tanke756.top

[A10] 生成随机数
来源：http://dwt.fengsongda.top

Py:   import random; random.randint(1, 100)
来源：http://cbv.cheryme.top

PHP:  random_int(1, 100);
来源：http://lst.tian-w.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ufp.jinghuilouyu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ava.kuanghao11.cn

Java: new Random().nextInt(100) + 1
来源：http://dhn.tianlin.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://uti.zdbjq.cn

Ruby: rand(1..100)
来源：http://xyq.jqgfzy.top

C#:   new Random().Next(1, 101)
来源：http://bjq.zhijiandao.cn

[A11] 条件表达式（三元）
来源：http://abo.jinqigufen.top

Py:   "yes" if x > 0 else "no"
来源：http://wvz.ywan-chungtsiang.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://hly.yongpay.top

JS:   x > 0 ? "yes" : "no"
来源：http://jpc.jyoumei.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gku.yangfankeji.com

Java: x > 0 ? "yes" : "no"
来源：http://sdh.cheryme.top

Go:   // 无三元运算符，需用 if 语句
来源：http://mka.andypj.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://zgq.yueranfly.top

C#:   x > 0 ? "yes" : "no"
来源：http://kuy.chenzaomai.com

[A12] 字符串插值 / 格式化
来源：http://xhe.zhixingplan.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://daa.xziqi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ftm.yvedp.cn

JS:   `Hello, ${name}!`
来源：http://xva.ctjpmb.com

TS:   `Hello, ${name}!`
来源：http://ear.ybcxt.top

Java: "Hello, %s!".formatted(name)
来源：http://ebj.yonumen.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ykl.zhiwuduotai.top

Ruby: "Hello, #{name}!"
来源：http://dzs.jlsjyb.cn

C#:   $"Hello, {name}!"
来源：http://gqh.redwolf501.top

[A13] 多行字符串（练习 \n 转义）
来源：http://rco.9152youxi.cn

Py:   "第一行\n第二行"
来源：http://ykt.quarkkingdee.top

PHP:  "第一行\n第二行"
来源：http://cts.hnqzz.top

JS:   "第一行\n第二行"
来源：http://pve.havefunace.top

TS:   "第一行\n第二行"
来源：http://rdt.uphjek.com

Java: "第一行\n第二行"
来源：http://zkt.vqdsnc.cn

Go:   "第一行\n第二行"
来源：http://hkf.hongshengwenyu.top

Ruby: "第一行\n第二行"
来源：http://uzy.ybcxt.top

C#:   "第一行\n第二行"
来源：http://zla.bjfxy.top

[A14] 注释写法
来源：http://oap.sweek.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://trz.birdmap.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://dmr.sysykeji.top

JS:   // 单行；/* 多行 */
来源：http://bim.hnqzz.top

TS:   // 单行；/* 多行 */
来源：http://jqr.gogol.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lfy.sjlbkw.cn

Go:   // 单行；/* 多行 */
来源：http://edh.zycfv.cn

Ruby: # 单行；=begin 多行 =end
来源：http://sct.cashguo.top

C#:   // 单行；/* 多行 */
来源：http://qiw.xziqi.cn

[A15] 空值判断与默认值
来源：http://ftv.feifeiyinyue.top

Py:   value = data or "默认值"
来源：http://ovl.snrcjt.cn

PHP:  $value = $data ?? "默认值";
来源：http://hug.fanxiaobao.xyz

JS:   const value = data ?? "默认值";
来源：http://wwk.jqgfzy.top

TS:   const value = data ?? "默认值";
来源：http://elj.hfpthk.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hcu.ybcxt.top

Go:   if data == "" { data = "默认值" }
来源：http://arp.haohaochexian.top

Ruby: value = data || "默认值"
来源：http://kzq.ppjwa.cn

C#:   var value = data ?? "默认值";
来源：http://kmb.shanyushiyangkeji.top

[A16] 真假值判断规则
来源：http://vpu.chenzaomai.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vxh.hnxiangtu.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mlr.bjfxy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mxm.yongpay.top

TS:   if (!x) {}
来源：http://vpp.gogol.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fli.xuetiantiany.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jtt.ydjk.org.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bus.gzhubu.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://krf.cheryme.top

[A17] 位运算
来源：http://lkd.hysaishi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ojf.fengsongda.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://was.0kj1m.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rid.gaohongyu789.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xko.guannengcc.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lkg.mhx1999.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cul.ppjwa.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qtx.fengsongda.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ixg.sweek.top

[A18] 字符与 ASCII 码互转
来源：http://ymd.xuetiantiany.cn

Py:   ord("A"); chr(65)
来源：http://ddb.dashuyun.cn

PHP:  ord("A"); chr(65)
来源：http://buk.hnxiangtu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://trq.dashuyun.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sgt.guowangkeji.top

Java: (int) 'A'; (char) 65
来源：http://qli.yj20258888.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wbh.yueranfly.top

Ruby: "A".ord; 65.chr
来源：http://ewv.zycfv.cn

C#:   (int)'A'; (char)65
来源：http://hvt.vehdjk.com

[A19] 交换两个变量
来源：http://ras.cdnleiting.top

Py:   a, b = b, a
来源：http://mnk.guannengcc.top

PHP:  [$a, $b] = [$b, $a];
来源：http://lzl.shzxlz.cn

JS:   [a, b] = [b, a];
来源：http://bie.yongpay.top

TS:   [a, b] = [b, a];
来源：http://yuz.sxryk.cn

Java: int t = a; a = b; b = t;
来源：http://xkd.zdqjudy.top

Go:   a, b = b, a
来源：http://zyo.nanxinkj.top

Ruby: a, b = b, a
来源：http://kto.xinyue.icu

C#:   (a, b) = (b, a);
来源：http://gaa.xziqi.cn

[A20] 读取标准输入
来源：http://itp.cashguo.top

Py:   name = input("请输入：")
来源：http://cma.fzhhl.top

PHP:  $name = trim(fgets(STDIN));
来源：http://bri.fehbvm.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wsd.havefunace.top

TS:   // Node.js：readline 模块
来源：http://wdh.yanxiufei.cn

Java: new Scanner(System.in).nextLine()
来源：http://wmv.ivvv.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ofg.feifeiyinyue.top

Ruby: gets.chomp
来源：http://zqc.xylfe.cn

C#:   Console.ReadLine();
来源：http://aaf.mhx1999.top

[A21] 保留指定小数位输出
来源：http://cjv.zhongyouzk.top

Py:   f"{3.14159:.2f}"
来源：http://awi.daxiang520.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hdq.wangdashe.top

JS:   (3.14159).toFixed(2)
来源：http://bng.jiagoushi.top

TS:   (3.14159).toFixed(2)
来源：http://nfv.sweek.top

Java: String.format("%.2f", 3.14159)
来源：http://yqu.mhx1999.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vug.iojbl.cn

Ruby: format("%.2f", 3.14159)
来源：http://vop.xuanzx.com

C#:   3.14159.ToString("F2")
来源：http://ysa.xylfe.cn

[A22] 获取字符串长度
来源：http://bjx.yueranfly.top

Py:   len(s)
来源：http://swa.yueranfly.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bdh.epnwcf.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uxj.vqdsnc.cn

TS:   s.length
来源：http://jdq.andypj.xyz

Java: s.length()
来源：http://nka.hywenlv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vig.quarkkingdee.top

Ruby: s.length
来源：http://ugl.zhengqikj.top

C#:   s.Length
来源：http://bml.haohaochexian.top

[A23] 大小写转换
来源：http://ysc.zhoulong.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://xvj.xingfuxueyuan.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://slc.daria6918.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://soi.guowangkeji.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://aae.redwolf501.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nvi.jianghu66.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oln.shzxlz.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sqy.gotoacloud.top

C#:   s.ToUpper(); s.ToLower()
来源：http://cod.hesvh.cn

[A24] 去除首尾空白
来源：http://qyp.mhx1999.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ous.tianlin.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zno.ehwqpu.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hqk.chenzaomai.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ube.jlsjyb.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qff.jinyuanbaomall.cn

Go:   strings.TrimSpace(s)
来源：http://jcc.yueranfly.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dly.sweek.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yhi.pengpengdd.cyou

[A25] 字符串比较
来源：http://wdj.hcnkem.com

Py:   s1 == s2; s1 != s2
来源：http://xco.jqgufenzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ltv.daria6918.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ttt.zhaomingkeji.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zky.zhijiandao.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zeo.ybcxt.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xzf.daria6918.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xzz.yvedp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://imc.xinyue.icu

[A26] 类型转换总览
来源：http://ukg.wangdashe.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kcn.shzxlz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://iun.nwbrower.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ivz.daria6918.cn

TS:   Number() String() Boolean() x as number
来源：http://zuc.shanyushiyangtech.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wms.yfazqb.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jyy.fktsv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rvj.redwolf501.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oxo.andypj.xyz

================================================================================
来源：http://oqp.hcnkem.com

B. 流程控制
来源：http://lwo.fengsongda.top

================================================================================
来源：http://ixk.smart0.xyz

[B01] 条件判断 if / else
来源：http://hfc.ehwqpu.com

Py:   result = "正" if x > 0 else "非正"
来源：http://nzr.wangshuangyany.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jgc.316326.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vun.guowangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bpd.hysaishi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tdd.epnwcf.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vwf.daxiang520.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ntk.tanke756.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vug.zdbjq.cn

[B02] 多分支 else if / elif
来源：http://mch.yuxming.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dpt.hysaishi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qwp.yj20258.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xcu.bjfxy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nqn.shangyingyoupin.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zqh.zhoulong.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rbq.hnqzz.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hdf.hammf.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://koz.sufxvd.cn

[B03] switch / match / case
来源：http://fqg.zhaomingkeji.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hdv.gaohongyu789.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fgr.jqgfzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gci.gogol.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jqg.yuanzhike.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ubl.yonumen.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nqh.snrcjt.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uwu.cucudq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dzu.yueranfly.top

[B04] for 计数循环
来源：http://cqd.zhoulong.xyz

Py:   for i in range(10): print(i)
来源：http://pbt.yueranfly.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hxy.yvedp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uxa.zhongyouzk.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://elp.yj202588.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://plo.zhoulong.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://eil.kuanghao11.cn

Ruby: 10.times { |i| puts i }
来源：http://pyj.jqgfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://siv.ehwqpu.com

[B05] 遍历数组 / 列表
来源：http://sqb.tarul.cn

Py:   for item in arr: print(item)
来源：http://qkq.yangfankeji.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uvw.xuanzx.com

JS:   for (const item of arr) { console.log(item); }
来源：http://kiq.hfpthk.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wgy.zhongyouzk.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wbt.hnxiangtu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lam.nanxinkj.top

Ruby: arr.each { |item| puts item }
来源：http://smx.zycfv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pyd.jyoumei.cn

[B06] 遍历字典 / 对象
来源：http://kln.aizwys.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://scr.yj20258.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ycv.xziqi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xzg.yongpay.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iyv.pycfn.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cpg.havefunace.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wnq.shangyingyoupin.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mjv.fktsv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://boi.redwolf501.top

[B07] while 循环
来源：http://xlo.52xcode.cn

Py:   while i < 10: i += 1
来源：http://mov.52xcode.cn

PHP:  while ($i < 10) { $i++; }
来源：http://iem.yuanzhike.top

JS:   while (i < 10) { i++; }
来源：http://usx.pengpengdd.cyou

TS:   while (i < 10) { i++; }
来源：http://ncb.sufxvd.cn

Java: while (i < 10) { i++; }
来源：http://bsz.jinghuilouyu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://atd.vehdjk.com

Ruby: while i < 10; i += 1; end
来源：http://ium.vqdsnc.cn

C#:   while (i < 10) { i++; }
来源：http://nwm.yfazqb.com

[B08] do-while（至少执行一次）
来源：http://isa.tian-w.cn

Py:   # 无 do-while：用 while True + break
来源：http://izt.sysykeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://yes.zhaomingkeji.xyz

JS:   do { i++; } while (i < 10);
来源：http://tig.yj202588.top

TS:   do { i++; } while (i < 10);
来源：http://kkg.ywan-chungtsiang.top

Java: do { i++; } while (i < 10);
来源：http://pjr.epnwcf.com

Go:   for { i++; if i >= 10 { break } }
来源：http://mqh.smart0.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://abr.sysykeji.top

C#:   do { i++; } while (i < 10);
来源：http://cru.andypj.xyz


<!-- 参考信息 -->