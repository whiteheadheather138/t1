代发 wailian999

Py:   print("Hello, World!")
来源：http://fes.chenlongwang.top

PHP:  echo "Hello, World!";
来源：http://jmt.hnxiangtu.top

JS:   console.log("Hello, World!");
来源：http://dmu.xinyue.icu

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vff.birdmap.top

Java: System.out.println("Hello, World!");
来源：http://dot.bbcook.cn

Go:   fmt.Println("Hello, World!")
来源：http://tdf.nanxinkj.top

Ruby: puts "Hello, World!"
来源：http://abz.yanxiufei.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://bme.yj20258.top

[A02] 变量声明与赋值
来源：http://iol.hfpthk.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vfo.meibo888.top

PHP:  $name = "Alex"; $age = 20;
来源：http://bug.jinghuilouyu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://rzn.gotoacloud.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://daz.iojbl.cn

Java: String name = "Alex"; int age = 20;
来源：http://uwk.birdmap.top

Go:   name := "Alex"; age := 20
来源：http://enw.fanxiaobao.xyz

Ruby: name = "Alex"; age = 20
来源：http://mfm.yanxiufei.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cvr.jianghu66.top

[A03] 常量定义
来源：http://xzb.zhaomingkeji.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gen.fengsongda.top

PHP:  const PI = 3.14159;
来源：http://ibm.hcnkem.com

JS:   const PI = 3.14159;
来源：http://imi.tianlin.xyz

TS:   const PI: number = 3.14159;
来源：http://aby.iojbl.cn

Java: static final double PI = 3.14159;
来源：http://cis.sweek.top

Go:   const PI = 3.14159
来源：http://kkl.yj20258.top

Ruby: PI = 3.14159
来源：http://kte.haohaochexian.top

C#:   const double PI = 3.14159;
来源：http://xrp.redwolf501.top

[A04] 判断变量类型
来源：http://ugz.chenzaomai.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://xoh.xziqi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kfv.ydjk.org.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://krh.yanxiufei.cn

TS:   typeof x; x instanceof Date
来源：http://xue.redwolf501.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gbu.yj20258.top

Go:   reflect.TypeOf(x).Name()
来源：http://oey.iojbl.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mmh.52xcode.cn

C#:   x.GetType().Name; x is int
来源：http://anl.zhixingplan.top

[A05] 整数除法与取模
来源：http://eim.fanxiaobao.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://suo.hysaishi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zfg.meibo888.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fkv.gotoacloud.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ihy.vqdsnc.cn

Java: 7 / 2; 7 % 2
来源：http://xpf.nanxuanxn.top

Go:   7 / 2; 7 % 2
来源：http://zqq.sjlbkw.cn

Ruby: 7 / 2; 7 % 2
来源：http://tgd.smart0.xyz

C#:   7 / 2; 7 % 2
来源：http://wbe.xuetiantiany.cn

[A06] 字符串转数字
来源：http://xgc.bbcook.cn

Py:   int("42"); float("3.14")
来源：http://yed.pycfn.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kqp.shangyingyoupin.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ldi.gaohongyu789.top

TS:   parseInt("42", 10); Number("42")
来源：http://jds.fehbvm.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rtj.svipenyu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mzh.birdmap.top

Ruby: "42".to_i; "3.14".to_f
来源：http://yho.guowangkeji.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tdi.cucudq.cn

[A07] 数字转字符串
来源：http://yez.jlsjyb.cn

Py:   str(42)
来源：http://wrg.zhaomingkeji.xyz

PHP:  (string) 42; strval(42)
来源：http://caq.chenjidiqi.icu

JS:   String(42); (42).toString()
来源：http://pwl.nanxinkj.top

TS:   String(42)
来源：http://iyo.hesvh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qwu.sysykeji.top

Go:   strconv.Itoa(42)
来源：http://rcm.daxiang520.top

Ruby: 42.to_s
来源：http://owg.shuidangran.top

C#:   42.ToString()
来源：http://yag.mhx1999.top

[A08] 取整与四舍五入
来源：http://nnb.sjlbkw.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qrz.zhongyouzk.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fap.xylfe.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tzv.zhengqikj.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://orc.wangshuangyany.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tkh.52xcode.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pmx.316326.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://ssx.wangdashe.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mjv.sweek.top

[A09] 绝对值与最大最小值
来源：http://iuy.ybcxt.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ixp.mhx1999.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://izw.sxryk.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ufu.zdbjq.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jfj.dashuyun.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qhh.fzhhl.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mmj.kuanghao11.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jgl.ehwqpu.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sqf.zdqjudy.top

[A10] 生成随机数
来源：http://xbc.jlsjyb.cn

Py:   import random; random.randint(1, 100)
来源：http://yci.meibo888.top

PHP:  random_int(1, 100);
来源：http://ich.yanxiufei.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sma.uphjek.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ooe.yueranfly.top

Java: new Random().nextInt(100) + 1
来源：http://evo.meibo888.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sxp.9152youxi.cn

Ruby: rand(1..100)
来源：http://xiu.hnqzz.top

C#:   new Random().Next(1, 101)
来源：http://nzu.hfpthk.cn

[A11] 条件表达式（三元）
来源：http://qvh.chenjidiqi.icu

Py:   "yes" if x > 0 else "no"
来源：http://jpi.daxiang520.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://gtm.jinyuanbaomall.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qua.ydzc1.top

TS:   x > 0 ? "yes" : "no"
来源：http://wyi.zhengqikj.top

Java: x > 0 ? "yes" : "no"
来源：http://vto.yj202588.top

Go:   // 无三元运算符，需用 if 语句
来源：http://oca.ywan-chungtsiang.top

Ruby: x > 0 ? "yes" : "no"
来源：http://tsv.fehbvm.com

C#:   x > 0 ? "yes" : "no"
来源：http://tuv.316326.xyz

[A12] 字符串插值 / 格式化
来源：http://hrp.yueranfly.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ezt.dianchejie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jfd.zhijiandao.cn

JS:   `Hello, ${name}!`
来源：http://fvv.jinghuilouyu.cn

TS:   `Hello, ${name}!`
来源：http://szy.chenjidiqi.icu

Java: "Hello, %s!".formatted(name)
来源：http://pvt.wangshuangyany.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yqj.redwolf501.top

Ruby: "Hello, #{name}!"
来源：http://cmv.svipenyu.cn

C#:   $"Hello, {name}!"
来源：http://bwb.yvedp.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://upl.zycfv.cn

Py:   "第一行\n第二行"
来源：http://kcx.zdbjq.cn

PHP:  "第一行\n第二行"
来源：http://acx.shuidangran.top

JS:   "第一行\n第二行"
来源：http://qxc.hysaishi.cn

TS:   "第一行\n第二行"
来源：http://jzs.quarkkingdee.top

Java: "第一行\n第二行"
来源：http://hea.jiagoushi.top

Go:   "第一行\n第二行"
来源：http://elm.gotoacloud.top

Ruby: "第一行\n第二行"
来源：http://xul.gaohongyu789.top

C#:   "第一行\n第二行"
来源：http://kzq.jyoumei.cn

[A14] 注释写法
来源：http://vau.cqqwz.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xsf.xuanzx.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://ovw.9152youxi.cn

JS:   // 单行；/* 多行 */
来源：http://mvr.zdqjudy.top

TS:   // 单行；/* 多行 */
来源：http://qtj.shzxlz.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wvm.vehdjk.com

Go:   // 单行；/* 多行 */
来源：http://slt.fzhhl.top

Ruby: # 单行；=begin 多行 =end
来源：http://tzw.aibaodan.cn

C#:   // 单行；/* 多行 */
来源：http://xen.hcnkem.com

[A15] 空值判断与默认值
来源：http://ooe.xinyue.icu

Py:   value = data or "默认值"
来源：http://cll.ydzc1.top

PHP:  $value = $data ?? "默认值";
来源：http://afj.hywenlv.cn

JS:   const value = data ?? "默认值";
来源：http://fnn.hcnkem.com

TS:   const value = data ?? "默认值";
来源：http://jtf.zhijiandao.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://asv.gotoacloud.top

Go:   if data == "" { data = "默认值" }
来源：http://baw.shuidangran.top

Ruby: value = data || "默认值"
来源：http://fmq.hywenlv.cn

C#:   var value = data ?? "默认值";
来源：http://uzh.hongshengwenyu.top

[A16] 真假值判断规则
来源：http://nlx.cqqwz.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qdh.52xcode.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lfe.gaohongyu789.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://aqy.zdqjudy.top

TS:   if (!x) {}
来源：http://lfa.guannengcc.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mih.nwbrower.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nsg.dianchejie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wck.daria6918.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cuc.cqqwz.cn

[A17] 位运算
来源：http://qqz.meibo888.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ony.zhixingplan.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zrz.nwbrower.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wnc.zycfv.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://odm.yj20258888.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://imj.hesvh.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dep.hesvh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dxk.bjfxy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qon.shanyushiyangtech.top

[A18] 字符与 ASCII 码互转
来源：http://edc.yuxming.cn

Py:   ord("A"); chr(65)
来源：http://umj.shangyingyoupin.top

PHP:  ord("A"); chr(65)
来源：http://fmr.snrcjt.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nlv.hywenlv.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gnw.shanyushiyangkeji.top

Java: (int) 'A'; (char) 65
来源：http://vpq.svipenyu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gqz.epnwcf.com

Ruby: "A".ord; 65.chr
来源：http://wuf.wangshuangyany.cn

C#:   (int)'A'; (char)65
来源：http://hri.jinyuanbaomall.cn

[A19] 交换两个变量
来源：http://tdw.pengpengdd.cyou

Py:   a, b = b, a
来源：http://ivg.52xcode.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://urj.dashuyun.cn

JS:   [a, b] = [b, a];
来源：http://dgp.hcnkem.com

TS:   [a, b] = [b, a];
来源：http://abe.dashuyun.cn

Java: int t = a; a = b; b = t;
来源：http://uzq.tanke756.top

Go:   a, b = b, a
来源：http://jsb.tian-w.cn

Ruby: a, b = b, a
来源：http://uod.316326.xyz

C#:   (a, b) = (b, a);
来源：http://ewi.wangdashe.top

[A20] 读取标准输入
来源：http://kix.ivvv.top

Py:   name = input("请输入：")
来源：http://jle.tarul.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://awb.jqgufenzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://eew.wangdashe.top

TS:   // Node.js：readline 模块
来源：http://hfs.sjlbkw.cn

Java: new Scanner(System.in).nextLine()
来源：http://moc.shanyushiyangkeji.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://thi.zhijiandao.cn

Ruby: gets.chomp
来源：http://btr.cqqwz.cn

C#:   Console.ReadLine();
来源：http://aoo.zhiwuduotai.top

[A21] 保留指定小数位输出
来源：http://pgl.ywan-chungtsiang.top

Py:   f"{3.14159:.2f}"
来源：http://hyx.jyoumei.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wbf.tanke756.top

JS:   (3.14159).toFixed(2)
来源：http://aad.jiagoushi.top

TS:   (3.14159).toFixed(2)
来源：http://yhw.redwolf501.top

Java: String.format("%.2f", 3.14159)
来源：http://mgt.nanxuanxn.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ofi.quarkkingdee.top

Ruby: format("%.2f", 3.14159)
来源：http://jbp.yongpay.top

C#:   3.14159.ToString("F2")
来源：http://icg.cucudq.cn

[A22] 获取字符串长度
来源：http://xaf.sjlbkw.cn

Py:   len(s)
来源：http://ekb.haohaochexian.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hkt.fehbvm.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lcq.aibaodan.cn

TS:   s.length
来源：http://juy.jiagoushi.top

Java: s.length()
来源：http://ymv.zycfv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://unk.uphjek.com

Ruby: s.length
来源：http://muj.ydjk.org.cn

C#:   s.Length
来源：http://bmo.zhengqikj.top

[A23] 大小写转换
来源：http://ojh.yonumen.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wku.cdnleiting.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hej.hywenlv.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lie.gotoacloud.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rct.zdqjudy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ecp.nanxuanxn.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://slu.epnwcf.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dof.gzhubu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://lam.sjlbkw.cn

[A24] 去除首尾空白
来源：http://adf.shanyushiyangkeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://txy.hywenlv.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qur.mhx1999.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oha.xingfuxueyuan.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bcc.yfazqb.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://irk.andypj.xyz

Go:   strings.TrimSpace(s)
来源：http://lar.chenzaomai.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ufj.shangyingyoupin.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://czx.bjfxy.top

[A25] 字符串比较
来源：http://edv.haohaochexian.top

Py:   s1 == s2; s1 != s2
来源：http://zhb.guowangkeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://aiv.gzhubu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://znk.guannengcc.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pmb.ybcxt.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vqm.fzhhl.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fig.hnqzz.top

Ruby: s1 == s2; s1 <=> s2
来源：http://hih.jinqigufen.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qxo.dashuyun.cn

[A26] 类型转换总览
来源：http://syr.jlsjyb.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cxb.cashguo.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://eth.fzhhl.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jlt.yj202588.top

TS:   Number() String() Boolean() x as number
来源：http://jqe.0kj1m.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ncj.feifeiyinyue.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zek.sjlbkw.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nep.tarul.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nst.yj202588.top

================================================================================
来源：http://mqd.xylfe.cn

B. 流程控制
来源：http://pdz.zdbjq.cn

================================================================================
来源：http://omz.kuanghao11.cn

[B01] 条件判断 if / else
来源：http://xer.sxryk.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xzv.smart0.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lmp.shanyushiyangkeji.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://aev.sjlbkw.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tdg.hfpthk.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bok.shangyingyoupin.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hpa.jinqigufen.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vmf.redwolf501.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gnd.gaohongyu789.top

[B02] 多分支 else if / elif
来源：http://tyi.cashguo.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gln.hysaishi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rdq.chenlongwang.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jgx.zhengqikj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://btl.sweek.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oad.cucudq.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fkm.zycfv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jtg.jinqigfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tma.havefunace.top

[B03] switch / match / case
来源：http://ptt.nwbrower.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yxm.tianlin.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lnx.fktsv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hhx.yongpay.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://shk.wangdashe.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tab.52xcode.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dwx.uphjek.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bfl.dianchejie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yhl.c1oappe.top

[B04] for 计数循环
来源：http://cyy.pycfn.com

Py:   for i in range(10): print(i)
来源：http://qfw.hesvh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wbb.sjlbkw.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pge.aibaodan.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ezk.ctjpmb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iad.sufxvd.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://edr.kuanghao11.cn

Ruby: 10.times { |i| puts i }
来源：http://qda.0kj1m.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://eem.nwbrower.top

[B05] 遍历数组 / 列表
来源：http://guq.zdqjudy.top

Py:   for item in arr: print(item)
来源：http://upk.feifeiyinyue.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gqv.xingfuxueyuan.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://mei.zdqjudy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://jvb.jqgufenzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://frk.jqgufenzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rxq.dianchejie.cn

Ruby: arr.each { |item| puts item }
来源：http://khi.jinqigufen.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ggl.yonumen.top

[B06] 遍历字典 / 对象
来源：http://kyh.yj20258888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://jtw.ybcxt.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ebh.nanxinkj.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ovh.gzhubu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mzq.hfpthk.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://iyr.yanxiufei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cfm.xingfuxueyuan.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kfu.ybcxt.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zju.sysykeji.top

[B07] while 循环
来源：http://uec.fktsv.cn

Py:   while i < 10: i += 1
来源：http://ckj.epnwcf.com

PHP:  while ($i < 10) { $i++; }
来源：http://ptb.yuxming.cn

JS:   while (i < 10) { i++; }
来源：http://flr.iojbl.cn

TS:   while (i < 10) { i++; }
来源：http://bit.andypj.xyz

Java: while (i < 10) { i++; }
来源：http://phs.yuanzhike.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://clf.yuanzhike.top

Ruby: while i < 10; i += 1; end
来源：http://lwn.ydjk.org.cn

C#:   while (i < 10) { i++; }
来源：http://vot.cqqwz.cn

[B08] do-while（至少执行一次）
来源：http://hlr.tarul.cn


<!-- 参考信息 -->