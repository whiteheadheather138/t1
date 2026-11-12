代发 wailian999

[A02] 变量声明与赋值
来源：http://kww.sysykeji.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://clq.vehdjk.com

PHP:  $name = "Alex"; $age = 20;
来源：http://zje.yvedp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ivc.gaohongyu789.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://har.vehdjk.com

Java: String name = "Alex"; int age = 20;
来源：http://gpb.iojbl.cn

Go:   name := "Alex"; age := 20
来源：http://umx.ywan-chungtsiang.top

Ruby: name = "Alex"; age = 20
来源：http://wcb.pengpengdd.cyou

C#:   string name = "Alex"; int age = 20;
来源：http://vaj.shuidangran.top

[A03] 常量定义
来源：http://eyh.hammf.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://luk.meibo888.top

PHP:  const PI = 3.14159;
来源：http://afo.yuxming.cn

JS:   const PI = 3.14159;
来源：http://fmq.guowangkeji.top

TS:   const PI: number = 3.14159;
来源：http://hrs.cheryme.top

Java: static final double PI = 3.14159;
来源：http://gtq.yuxming.cn

Go:   const PI = 3.14159
来源：http://dgf.hongshengwenyu.top

Ruby: PI = 3.14159
来源：http://vnn.gzhubu.top

C#:   const double PI = 3.14159;
来源：http://wxl.aibaodan.cn

[A04] 判断变量类型
来源：http://gja.hfpthk.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xwk.pycfn.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bth.fengsongda.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xwe.0kj1m.cn

TS:   typeof x; x instanceof Date
来源：http://fax.yanxiufei.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://uob.yj20258.top

Go:   reflect.TypeOf(x).Name()
来源：http://xcd.wangdashe.top

Ruby: x.class; x.is_a?(Integer)
来源：http://csa.jyoumei.cn

C#:   x.GetType().Name; x is int
来源：http://upx.wangshuangyany.cn

[A05] 整数除法与取模
来源：http://ysb.tianlin.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://uvw.meibo888.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://bmj.ywan-chungtsiang.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://aub.xuanzx.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pjn.xuanzx.com

Java: 7 / 2; 7 % 2
来源：http://tbc.yongpay.top

Go:   7 / 2; 7 % 2
来源：http://jvz.pengpengdd.cyou

Ruby: 7 / 2; 7 % 2
来源：http://uao.nwbrower.top

C#:   7 / 2; 7 % 2
来源：http://oxj.smart0.xyz

[A06] 字符串转数字
来源：http://ced.zdbjq.cn

Py:   int("42"); float("3.14")
来源：http://cza.chenzaomai.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://aoz.gogol.net.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dbe.aizwys.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qoa.kuanghao11.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://inb.ywan-chungtsiang.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xdy.pycfn.com

Ruby: "42".to_i; "3.14".to_f
来源：http://ygw.sjlbkw.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xwb.andypj.xyz

[A07] 数字转字符串
来源：http://vdn.sysykeji.top

Py:   str(42)
来源：http://nuu.cdnleiting.top

PHP:  (string) 42; strval(42)
来源：http://yhw.hesvh.cn

JS:   String(42); (42).toString()
来源：http://gyo.chenlongwang.top

TS:   String(42)
来源：http://rln.yj20258888.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://lnw.ydjk.org.cn

Go:   strconv.Itoa(42)
来源：http://muk.xylfe.cn

Ruby: 42.to_s
来源：http://tgi.hnxiangtu.top

C#:   42.ToString()
来源：http://lrv.ivvv.top

[A08] 取整与四舍五入
来源：http://pgf.ivvv.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zkh.daxiang520.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xxp.pycfn.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://olv.52xcode.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rdi.0kj1m.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://byv.bbcook.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dwj.sxryk.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://tnt.hammf.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://iqy.hammf.cn

[A09] 绝对值与最大最小值
来源：http://qkj.52xcode.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pdv.ehwqpu.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ifk.cheryme.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://npf.xziqi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://oxi.zdqjudy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bjz.gaohongyu789.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xnu.gaohongyu789.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mws.cashguo.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://aun.sweek.top

[A10] 生成随机数
来源：http://ljz.shanyushiyangtech.top

Py:   import random; random.randint(1, 100)
来源：http://jhm.hesvh.cn

PHP:  random_int(1, 100);
来源：http://dup.tanke756.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qxd.sweek.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fpr.cashguo.top

Java: new Random().nextInt(100) + 1
来源：http://nwu.shanyushiyangtech.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cbs.dashuyun.cn

Ruby: rand(1..100)
来源：http://ktm.smart0.xyz

C#:   new Random().Next(1, 101)
来源：http://euu.yangfankeji.com

[A11] 条件表达式（三元）
来源：http://qnx.316326.xyz

Py:   "yes" if x > 0 else "no"
来源：http://pby.aibaodan.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://kup.xylfe.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rzl.zhijiandao.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mpq.aibaodan.cn

Java: x > 0 ? "yes" : "no"
来源：http://pwa.ybcxt.top

Go:   // 无三元运算符，需用 if 语句
来源：http://quo.fanxiaobao.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://tuf.tanke756.top

C#:   x > 0 ? "yes" : "no"
来源：http://ocv.xuanzx.com

[A12] 字符串插值 / 格式化
来源：http://aja.hammf.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gwa.hywenlv.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jjc.hywenlv.cn

JS:   `Hello, ${name}!`
来源：http://xwt.smart0.xyz

TS:   `Hello, ${name}!`
来源：http://ygi.ydjk.org.cn

Java: "Hello, %s!".formatted(name)
来源：http://whl.zhijiandao.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tvq.ydzc1.top

Ruby: "Hello, #{name}!"
来源：http://xse.9152youxi.cn

C#:   $"Hello, {name}!"
来源：http://qwx.pycfn.com

[A13] 多行字符串（练习 \n 转义）
来源：http://llk.aibaodan.cn

Py:   "第一行\n第二行"
来源：http://fkh.daria6918.cn

PHP:  "第一行\n第二行"
来源：http://hwc.dianchejie.cn

JS:   "第一行\n第二行"
来源：http://jan.yfazqb.com

TS:   "第一行\n第二行"
来源：http://fic.zhiwuduotai.top

Java: "第一行\n第二行"
来源：http://zkm.yfazqb.com

Go:   "第一行\n第二行"
来源：http://zzy.kuanghao11.cn

Ruby: "第一行\n第二行"
来源：http://tyy.jyoumei.cn

C#:   "第一行\n第二行"
来源：http://cep.jlsjyb.cn

[A14] 注释写法
来源：http://clm.sjlbkw.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://tdj.svipenyu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jgt.fehbvm.com

JS:   // 单行；/* 多行 */
来源：http://izu.yj202588.top

TS:   // 单行；/* 多行 */
来源：http://byz.zhijiandao.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://euc.daxiang520.top

Go:   // 单行；/* 多行 */
来源：http://qpx.ppjwa.cn

Ruby: # 单行；=begin 多行 =end
来源：http://kot.yanxiufei.cn

C#:   // 单行；/* 多行 */
来源：http://nel.yfazqb.com

[A15] 空值判断与默认值
来源：http://dan.snrcjt.cn

Py:   value = data or "默认值"
来源：http://cig.pengpengdd.cyou

PHP:  $value = $data ?? "默认值";
来源：http://zaq.sysykeji.top

JS:   const value = data ?? "默认值";
来源：http://sjt.tarul.cn

TS:   const value = data ?? "默认值";
来源：http://jtg.fehbvm.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://daw.sweek.top

Go:   if data == "" { data = "默认值" }
来源：http://idx.shanyushiyangkeji.top

Ruby: value = data || "默认值"
来源：http://bkl.fktsv.cn

C#:   var value = data ?? "默认值";
来源：http://gmy.jinqigfzy.top

[A16] 真假值判断规则
来源：http://izl.fktsv.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rvn.c1oappe.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qdk.fengsongda.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://aao.shuidangran.top

TS:   if (!x) {}
来源：http://pox.yj20258.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xms.sufxvd.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://six.xingfuxueyuan.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://izk.aibaodan.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jtz.bjfxy.top

[A17] 位运算
来源：http://ozy.hfpthk.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zcz.dashuyun.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://svw.hfpthk.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hzf.hammf.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zqu.sjlbkw.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://usn.fzhhl.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dsv.jqgufenzy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qbz.smart0.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blz.yanxiufei.cn

[A18] 字符与 ASCII 码互转
来源：http://taq.zhengqikj.top

Py:   ord("A"); chr(65)
来源：http://tcn.kuanghao11.cn

PHP:  ord("A"); chr(65)
来源：http://dhg.smart0.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pzg.nanxuanxn.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jrv.fktsv.cn

Java: (int) 'A'; (char) 65
来源：http://ipu.epnwcf.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dvr.cheryme.top

Ruby: "A".ord; 65.chr
来源：http://ckn.jyoumei.cn

C#:   (int)'A'; (char)65
来源：http://jzk.zhoulong.xyz

[A19] 交换两个变量
来源：http://abv.xuetiantiany.cn

Py:   a, b = b, a
来源：http://hap.xinyue.icu

PHP:  [$a, $b] = [$b, $a];
来源：http://nxo.ybcxt.top

JS:   [a, b] = [b, a];
来源：http://gsg.sufxvd.cn

TS:   [a, b] = [b, a];
来源：http://tvp.xuetiantiany.cn

Java: int t = a; a = b; b = t;
来源：http://xvk.hammf.cn

Go:   a, b = b, a
来源：http://ble.zhongyouzk.top

Ruby: a, b = b, a
来源：http://pii.ydzc1.top

C#:   (a, b) = (b, a);
来源：http://rda.guowangkeji.top

[A20] 读取标准输入
来源：http://qsl.yj20258888.top

Py:   name = input("请输入：")
来源：http://mfo.gzhubu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://nzz.andypj.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qpr.iojbl.cn

TS:   // Node.js：readline 模块
来源：http://zub.0kj1m.cn

Java: new Scanner(System.in).nextLine()
来源：http://yvg.andypj.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qwt.smart0.xyz

Ruby: gets.chomp
来源：http://ejf.ehwqpu.com

C#:   Console.ReadLine();
来源：http://qot.52xcode.cn

[A21] 保留指定小数位输出
来源：http://vve.zhongyouzk.top

Py:   f"{3.14159:.2f}"
来源：http://glz.jinyuanbaomall.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ppc.cucudq.cn

JS:   (3.14159).toFixed(2)
来源：http://nzy.hysaishi.cn

TS:   (3.14159).toFixed(2)
来源：http://tum.aibaodan.cn

Java: String.format("%.2f", 3.14159)
来源：http://dlb.xuanzx.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nzj.xuanzx.com

Ruby: format("%.2f", 3.14159)
来源：http://flp.yfazqb.com

C#:   3.14159.ToString("F2")
来源：http://ixc.yj20258.top

[A22] 获取字符串长度
来源：http://wql.xingfuxueyuan.xyz

Py:   len(s)
来源：http://icu.hysaishi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ufk.52xcode.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://amn.jiagoushi.top

TS:   s.length
来源：http://gez.hnxiangtu.top

Java: s.length()
来源：http://zdx.shzxlz.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://igi.aibaodan.cn

Ruby: s.length
来源：http://wgz.hammf.cn

C#:   s.Length
来源：http://tiq.yvedp.cn

[A23] 大小写转换
来源：http://vgl.yuanzhike.top

Py:   s.upper(); s.lower(); s.title()
来源：http://dsj.hongshengwenyu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wic.guannengcc.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ebh.zhixingplan.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bav.dianchejie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pqz.fanxiaobao.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yww.haohaochexian.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rzo.vehdjk.com

C#:   s.ToUpper(); s.ToLower()
来源：http://xou.ydjk.org.cn

[A24] 去除首尾空白
来源：http://qzv.hesvh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://drx.jlsjyb.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vjw.iojbl.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lqc.yangfankeji.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tva.meibo888.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://snl.jyoumei.cn

Go:   strings.TrimSpace(s)
来源：http://nwt.wangshuangyany.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zdl.zhongyouzk.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ovm.yuanzhike.top

[A25] 字符串比较
来源：http://fdd.cdnleiting.top

Py:   s1 == s2; s1 != s2
来源：http://ema.tarul.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kzg.wangdashe.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hlh.0kj1m.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://aol.yvedp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://luq.yuxming.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kwe.kuanghao11.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wxl.jyoumei.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lqs.vqdsnc.cn

[A26] 类型转换总览
来源：http://pfk.jyoumei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mzz.shangyingyoupin.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bcz.yanxiufei.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cly.yj20258.top

TS:   Number() String() Boolean() x as number
来源：http://jsl.xuanzx.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pkj.tian-w.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mrb.cashguo.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ybt.yonumen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://duh.jinyuanbaomall.cn

================================================================================
来源：http://tyx.ydjk.org.cn

B. 流程控制
来源：http://jit.xylfe.cn

================================================================================
来源：http://ftb.hysaishi.cn

[B01] 条件判断 if / else
来源：http://kfp.feifeiyinyue.top

Py:   result = "正" if x > 0 else "非正"
来源：http://xyd.feifeiyinyue.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://muc.gzhubu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tgu.vqdsnc.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://alx.nwbrower.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://yuz.xinyue.icu

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://onm.ppjwa.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rfk.zhixingplan.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fgq.cqqwz.cn

[B02] 多分支 else if / elif
来源：http://ado.iojbl.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hyw.gotoacloud.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://htb.jinyuanbaomall.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fle.andypj.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://myv.yongpay.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cpp.ivvv.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ghh.yongpay.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yzo.sweek.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://csw.fanxiaobao.xyz

[B03] switch / match / case
来源：http://lvh.nanxuanxn.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bke.kuanghao11.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pdh.vehdjk.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fnb.jqgufenzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ujn.bbcook.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zvd.zhaomingkeji.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wyk.cucudq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bqo.andypj.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hlw.sufxvd.cn

[B04] for 计数循环
来源：http://ltz.xylfe.cn

Py:   for i in range(10): print(i)
来源：http://qnq.cqqwz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nvj.fktsv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wuf.kuanghao11.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pzr.zdbjq.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pgt.feifeiyinyue.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oyk.chenlongwang.top

Ruby: 10.times { |i| puts i }
来源：http://jmm.hesvh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jjn.iojbl.cn

[B05] 遍历数组 / 列表
来源：http://yvi.cdnleiting.top

Py:   for item in arr: print(item)
来源：http://nit.9152youxi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sub.hammf.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ywh.yanxiufei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ffj.ivvv.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://opj.bjfxy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jgx.ehwqpu.com

Ruby: arr.each { |item| puts item }
来源：http://qyy.ivvv.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xws.cashguo.top

[B06] 遍历字典 / 对象
来源：http://dzd.meibo888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zmo.hysaishi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oig.yj202588.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://app.pengpengdd.cyou

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fbm.shangyingyoupin.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hqs.daxiang520.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tet.vqdsnc.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://icq.tianlin.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jmf.hfpthk.cn

[B07] while 循环
来源：http://pvq.haohaochexian.top

Py:   while i < 10: i += 1
来源：http://wri.cdnleiting.top

PHP:  while ($i < 10) { $i++; }
来源：http://iqo.daria6918.cn

JS:   while (i < 10) { i++; }
来源：http://bon.zdbjq.cn

TS:   while (i < 10) { i++; }
来源：http://vsx.snrcjt.cn

Java: while (i < 10) { i++; }
来源：http://ooj.dashuyun.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kxg.mhx1999.top

Ruby: while i < 10; i += 1; end
来源：http://hor.yuxming.cn

C#:   while (i < 10) { i++; }
来源：http://ujq.zhengqikj.top

[B08] do-while（至少执行一次）
来源：http://xqk.shzxlz.cn

Py:   # 无 do-while：用 while True + break
来源：http://drg.yuxming.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qvs.ehwqpu.com

JS:   do { i++; } while (i < 10);
来源：http://rxx.daria6918.cn

TS:   do { i++; } while (i < 10);
来源：http://ncz.nwbrower.top

Java: do { i++; } while (i < 10);
来源：http://gge.chenjidiqi.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://stt.zhoulong.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://cxj.aizwys.cn

C#:   do { i++; } while (i < 10);
来源：http://yns.daxiang520.top


<!-- 参考信息 -->