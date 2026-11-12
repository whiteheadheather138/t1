代发 wailian999

Py:   print("Hello, World!")
来源：http://ajt.jinqigufen.top

PHP:  echo "Hello, World!";
来源：http://phl.dianchejie.cn

JS:   console.log("Hello, World!");
来源：http://qqr.fehbvm.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nzr.andypj.xyz

Java: System.out.println("Hello, World!");
来源：http://sse.xylfe.cn

Go:   fmt.Println("Hello, World!")
来源：http://utn.smart0.xyz

Ruby: puts "Hello, World!"
来源：http://tlm.c1oappe.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ftb.yj20258888.top

[A02] 变量声明与赋值
来源：http://mgt.sweek.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ucg.guowangkeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://kvz.daria6918.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dpd.yvedp.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dug.yonumen.top

Java: String name = "Alex"; int age = 20;
来源：http://vbm.cqqwz.cn

Go:   name := "Alex"; age := 20
来源：http://qms.vqdsnc.cn

Ruby: name = "Alex"; age = 20
来源：http://eqz.yj20258.top

C#:   string name = "Alex"; int age = 20;
来源：http://pnz.iojbl.cn

[A03] 常量定义
来源：http://ins.hywenlv.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ebb.xuanzx.com

PHP:  const PI = 3.14159;
来源：http://kou.hesvh.cn

JS:   const PI = 3.14159;
来源：http://puc.gaohongyu789.top

TS:   const PI: number = 3.14159;
来源：http://xeq.shzxlz.cn

Java: static final double PI = 3.14159;
来源：http://yuv.hywenlv.cn

Go:   const PI = 3.14159
来源：http://nfv.hfpthk.cn

Ruby: PI = 3.14159
来源：http://qgy.zdbjq.cn

C#:   const double PI = 3.14159;
来源：http://jyb.daxiang520.top

[A04] 判断变量类型
来源：http://pfo.zhixingplan.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ofc.sjlbkw.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://eev.xziqi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kxx.jqgufenzy.top

TS:   typeof x; x instanceof Date
来源：http://vjf.316326.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mak.yuanzhike.top

Go:   reflect.TypeOf(x).Name()
来源：http://bpr.yuanzhike.top

Ruby: x.class; x.is_a?(Integer)
来源：http://wfi.bbcook.cn

C#:   x.GetType().Name; x is int
来源：http://czu.kuanghao11.cn

[A05] 整数除法与取模
来源：http://duq.yfazqb.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rgi.jinyuanbaomall.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://shu.yonumen.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ato.ehwqpu.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xrg.yueranfly.top

Java: 7 / 2; 7 % 2
来源：http://sqs.dashuyun.cn

Go:   7 / 2; 7 % 2
来源：http://utn.shangyingyoupin.top

Ruby: 7 / 2; 7 % 2
来源：http://cvb.redwolf501.top

C#:   7 / 2; 7 % 2
来源：http://doh.zycfv.cn

[A06] 字符串转数字
来源：http://jsp.daria6918.cn

Py:   int("42"); float("3.14")
来源：http://jgn.shanyushiyangkeji.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ysp.sjlbkw.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://apq.birdmap.top

TS:   parseInt("42", 10); Number("42")
来源：http://pmk.pengpengdd.cyou

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://arg.gzhubu.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xax.zhoulong.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://nxy.guannengcc.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tmh.yvedp.cn

[A07] 数字转字符串
来源：http://qdn.yuanzhike.top

Py:   str(42)
来源：http://cbb.gotoacloud.top

PHP:  (string) 42; strval(42)
来源：http://lrv.316326.xyz

JS:   String(42); (42).toString()
来源：http://cnm.fehbvm.com

TS:   String(42)
来源：http://znk.yj20258888.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://prn.jyoumei.cn

Go:   strconv.Itoa(42)
来源：http://drz.daria6918.cn

Ruby: 42.to_s
来源：http://phb.sysykeji.top

C#:   42.ToString()
来源：http://lzk.shangyingyoupin.top

[A08] 取整与四舍五入
来源：http://skw.yongpay.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jpk.yongpay.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cfx.gotoacloud.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ejj.chenjidiqi.icu

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lao.ybcxt.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wmt.52xcode.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hqe.jinqigfzy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://eie.xuetiantiany.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://awp.hysaishi.cn

[A09] 绝对值与最大最小值
来源：http://flg.meibo888.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mpu.c1oappe.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lst.jqgfzy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lpm.havefunace.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bqw.birdmap.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nmt.fehbvm.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vtf.xuanzx.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ylp.xingfuxueyuan.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xea.fengsongda.top

[A10] 生成随机数
来源：http://hkk.iojbl.cn

Py:   import random; random.randint(1, 100)
来源：http://ggi.jyoumei.cn

PHP:  random_int(1, 100);
来源：http://cne.sjlbkw.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://snt.hesvh.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ear.gotoacloud.top

Java: new Random().nextInt(100) + 1
来源：http://thb.xziqi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tmk.daria6918.cn

Ruby: rand(1..100)
来源：http://ilh.nanxinkj.top

C#:   new Random().Next(1, 101)
来源：http://iwj.xuetiantiany.cn

[A11] 条件表达式（三元）
来源：http://frp.gogol.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://oso.zhengqikj.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://uiy.daria6918.cn

JS:   x > 0 ? "yes" : "no"
来源：http://tbp.jlsjyb.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zxj.nanxuanxn.top

Java: x > 0 ? "yes" : "no"
来源：http://vhi.guannengcc.top

Go:   // 无三元运算符，需用 if 语句
来源：http://mry.xziqi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ptf.feifeiyinyue.top

C#:   x > 0 ? "yes" : "no"
来源：http://zvt.xziqi.cn

[A12] 字符串插值 / 格式化
来源：http://qpz.aizwys.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mdk.yongpay.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://poz.zhongyouzk.top

JS:   `Hello, ${name}!`
来源：http://shj.tian-w.cn

TS:   `Hello, ${name}!`
来源：http://loz.pengpengdd.cyou

Java: "Hello, %s!".formatted(name)
来源：http://pbx.xingfuxueyuan.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://oep.shzxlz.cn

Ruby: "Hello, #{name}!"
来源：http://ros.zhongyouzk.top

C#:   $"Hello, {name}!"
来源：http://iro.hysaishi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jgy.hammf.cn

Py:   "第一行\n第二行"
来源：http://wfy.fehbvm.com

PHP:  "第一行\n第二行"
来源：http://bxw.bbcook.cn

JS:   "第一行\n第二行"
来源：http://qxh.jinghuilouyu.cn

TS:   "第一行\n第二行"
来源：http://blo.ctjpmb.com

Java: "第一行\n第二行"
来源：http://xor.uphjek.com

Go:   "第一行\n第二行"
来源：http://bcj.yueranfly.top

Ruby: "第一行\n第二行"
来源：http://wxh.jyoumei.cn

C#:   "第一行\n第二行"
来源：http://iuv.zdbjq.cn

[A14] 注释写法
来源：http://pwi.fengsongda.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://iol.fzhhl.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ilh.c1oappe.top

JS:   // 单行；/* 多行 */
来源：http://tfd.yj20258888.top

TS:   // 单行；/* 多行 */
来源：http://wuo.ppjwa.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yev.yj202588.top

Go:   // 单行；/* 多行 */
来源：http://jyb.jianghu66.top

Ruby: # 单行；=begin 多行 =end
来源：http://lmv.cdnleiting.top

C#:   // 单行；/* 多行 */
来源：http://exj.zhengqikj.top

[A15] 空值判断与默认值
来源：http://gsk.andypj.xyz

Py:   value = data or "默认值"
来源：http://igv.zhengqikj.top

PHP:  $value = $data ?? "默认值";
来源：http://qpu.birdmap.top

JS:   const value = data ?? "默认值";
来源：http://xhn.9152youxi.cn

TS:   const value = data ?? "默认值";
来源：http://rbb.chenzaomai.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qby.sxryk.cn

Go:   if data == "" { data = "默认值" }
来源：http://pge.smart0.xyz

Ruby: value = data || "默认值"
来源：http://pld.epnwcf.com

C#:   var value = data ?? "默认值";
来源：http://mdz.jinqigfzy.top

[A16] 真假值判断规则
来源：http://kym.snrcjt.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://san.sysykeji.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rxr.redwolf501.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://aiq.xinyue.icu

TS:   if (!x) {}
来源：http://jco.fktsv.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wdy.yongpay.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ocw.birdmap.top

Ruby: unless x            # nil 与 false 为假
来源：http://nur.shuidangran.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gfj.shanyushiyangtech.top

[A17] 位运算
来源：http://mib.ywan-chungtsiang.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jmk.bbcook.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wuv.fanxiaobao.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sye.daria6918.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tqn.zdbjq.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://amk.jianghu66.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ybv.tianlin.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ydu.yanxiufei.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kxu.aibaodan.cn

[A18] 字符与 ASCII 码互转
来源：http://olt.zdqjudy.top

Py:   ord("A"); chr(65)
来源：http://ntu.snrcjt.cn

PHP:  ord("A"); chr(65)
来源：http://sal.zdbjq.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tck.hywenlv.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tdn.vqdsnc.cn

Java: (int) 'A'; (char) 65
来源：http://mys.fengsongda.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://aql.yj20258.top

Ruby: "A".ord; 65.chr
来源：http://mfj.jinyuanbaomall.cn

C#:   (int)'A'; (char)65
来源：http://zxm.wangshuangyany.cn

[A19] 交换两个变量
来源：http://igx.tanke756.top

Py:   a, b = b, a
来源：http://dad.ctjpmb.com

PHP:  [$a, $b] = [$b, $a];
来源：http://iyg.xuetiantiany.cn

JS:   [a, b] = [b, a];
来源：http://cop.kuanghao11.cn

TS:   [a, b] = [b, a];
来源：http://ait.hysaishi.cn

Java: int t = a; a = b; b = t;
来源：http://hsv.hywenlv.cn

Go:   a, b = b, a
来源：http://cdn.zhijiandao.cn

Ruby: a, b = b, a
来源：http://abn.gaohongyu789.top

C#:   (a, b) = (b, a);
来源：http://sts.smart0.xyz

[A20] 读取标准输入
来源：http://gdq.zhongyouzk.top

Py:   name = input("请输入：")
来源：http://rtg.jyoumei.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hkc.9152youxi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hyg.shzxlz.cn

TS:   // Node.js：readline 模块
来源：http://nap.tianlin.xyz

Java: new Scanner(System.in).nextLine()
来源：http://llo.sjlbkw.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xss.mhx1999.top

Ruby: gets.chomp
来源：http://noa.jinqigfzy.top

C#:   Console.ReadLine();
来源：http://jhu.shuidangran.top

[A21] 保留指定小数位输出
来源：http://som.zhijiandao.cn

Py:   f"{3.14159:.2f}"
来源：http://ayl.xingfuxueyuan.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cbl.meibo888.top

JS:   (3.14159).toFixed(2)
来源：http://thc.cheryme.top

TS:   (3.14159).toFixed(2)
来源：http://vqx.daxiang520.top

Java: String.format("%.2f", 3.14159)
来源：http://cev.hywenlv.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bey.cheryme.top

Ruby: format("%.2f", 3.14159)
来源：http://tbv.hfpthk.cn

C#:   3.14159.ToString("F2")
来源：http://qom.shuidangran.top

[A22] 获取字符串长度
来源：http://xmf.yanxiufei.cn

Py:   len(s)
来源：http://lgn.xuanzx.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jic.bjfxy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xvx.ydjk.org.cn

TS:   s.length
来源：http://npb.ppjwa.cn

Java: s.length()
来源：http://cij.cucudq.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cmy.fanxiaobao.xyz

Ruby: s.length
来源：http://wlw.yongpay.top

C#:   s.Length
来源：http://wuc.guannengcc.top

[A23] 大小写转换
来源：http://wca.sjlbkw.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fvv.jyoumei.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://drc.zdbjq.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xkn.cashguo.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ayx.zhiwuduotai.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hgp.sysykeji.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cjp.ywan-chungtsiang.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jjq.hongshengwenyu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://cbg.fanxiaobao.xyz

[A24] 去除首尾空白
来源：http://ubc.zhixingplan.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://elz.tanke756.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lha.sxryk.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rfz.jqgufenzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://znw.quarkkingdee.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wsk.gotoacloud.top

Go:   strings.TrimSpace(s)
来源：http://fip.cashguo.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wba.hfpthk.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ppn.nanxinkj.top

[A25] 字符串比较
来源：http://ftt.zycfv.cn

Py:   s1 == s2; s1 != s2
来源：http://azn.hammf.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zvp.aizwys.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cqz.birdmap.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gwg.haohaochexian.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ylo.jlsjyb.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xpy.yueranfly.top

Ruby: s1 == s2; s1 <=> s2
来源：http://vfn.cheryme.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://msb.shanyushiyangkeji.top

[A26] 类型转换总览
来源：http://zpu.hongshengwenyu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fdk.yonumen.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hkx.guowangkeji.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://idp.aibaodan.cn

TS:   Number() String() Boolean() x as number
来源：http://daq.0kj1m.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mtk.pycfn.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tkd.tarul.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gvq.sjlbkw.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mvx.fktsv.cn

================================================================================
来源：http://wil.nanxuanxn.top

B. 流程控制
来源：http://cjw.chenlongwang.top

================================================================================
来源：http://goy.redwolf501.top

[B01] 条件判断 if / else
来源：http://dje.sysykeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://odk.bbcook.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://stz.chenzaomai.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jiw.jinqigufen.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://srn.cheryme.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://plf.meibo888.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cgh.chenzaomai.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gqr.yanxiufei.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ppo.yonumen.top

[B02] 多分支 else if / elif
来源：http://bsh.chenzaomai.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uov.vqdsnc.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cbe.gogol.net.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://asp.pycfn.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lqp.zhiwuduotai.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eyg.redwolf501.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bzh.tianlin.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wof.andypj.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cnw.xziqi.cn

[B03] switch / match / case
来源：http://mgu.zhijiandao.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dpy.zhixingplan.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qqn.shanyushiyangtech.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qki.hesvh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qqn.guowangkeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rmp.yuanzhike.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ljs.52xcode.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://git.guowangkeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ibi.jianghu66.top

[B04] for 计数循环
来源：http://tyz.nwbrower.top

Py:   for i in range(10): print(i)
来源：http://kfy.yfazqb.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dno.daxiang520.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iod.hesvh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://and.jinqigufen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dkn.aibaodan.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nyf.hammf.cn

Ruby: 10.times { |i| puts i }
来源：http://vyz.gzhubu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://azo.zhaomingkeji.xyz

[B05] 遍历数组 / 列表
来源：http://myf.quarkkingdee.top

Py:   for item in arr: print(item)
来源：http://ijf.guannengcc.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pgt.quarkkingdee.top

JS:   for (const item of arr) { console.log(item); }
来源：http://npj.shanyushiyangkeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tja.cucudq.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pas.zhaomingkeji.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dkk.shanyushiyangkeji.top

Ruby: arr.each { |item| puts item }
来源：http://kkr.xziqi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zdo.ywan-chungtsiang.top

[B06] 遍历字典 / 对象
来源：http://ckc.daxiang520.top

Py:   for k, v in d.items(): print(k, v)
来源：http://iap.wangdashe.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rkc.quarkkingdee.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xsm.quarkkingdee.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ptw.aizwys.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://afx.yongpay.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lqp.jyoumei.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oqv.chenlongwang.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ycc.feifeiyinyue.top

[B07] while 循环
来源：http://kyp.yueranfly.top

Py:   while i < 10: i += 1
来源：http://kua.fehbvm.com

PHP:  while ($i < 10) { $i++; }
来源：http://emy.cqqwz.cn

JS:   while (i < 10) { i++; }
来源：http://ffr.svipenyu.cn

TS:   while (i < 10) { i++; }
来源：http://iou.tianlin.xyz

Java: while (i < 10) { i++; }
来源：http://goa.gaohongyu789.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gwf.feifeiyinyue.top

Ruby: while i < 10; i += 1; end
来源：http://nzd.yfazqb.com

C#:   while (i < 10) { i++; }
来源：http://ako.daria6918.cn

[B08] do-while（至少执行一次）
来源：http://rax.dianchejie.cn


<!-- 参考信息 -->