代发 wailian999

Py:   print("Hello, World!")
来源：http://dmm.jlsjyb.cn

PHP:  echo "Hello, World!";
来源：http://adz.sxryk.cn

JS:   console.log("Hello, World!");
来源：http://cjo.mhx1999.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yuz.xziqi.cn

Java: System.out.println("Hello, World!");
来源：http://idj.jinqigufen.top

Go:   fmt.Println("Hello, World!")
来源：http://flw.guannengcc.top

Ruby: puts "Hello, World!"
来源：http://qdz.sxryk.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://tvv.ybcxt.top

[A02] 变量声明与赋值
来源：http://pbq.jyoumei.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lts.xziqi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zep.jlsjyb.cn

JS:   let name = "Alex"; const age = 20;
来源：http://lct.fehbvm.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://krr.ivvv.top

Java: String name = "Alex"; int age = 20;
来源：http://qyg.nanxuanxn.top

Go:   name := "Alex"; age := 20
来源：http://vww.jinghuilouyu.cn

Ruby: name = "Alex"; age = 20
来源：http://rqz.snrcjt.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fbx.hcnkem.com

[A03] 常量定义
来源：http://zes.cdnleiting.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://uca.jqgfzy.top

PHP:  const PI = 3.14159;
来源：http://ani.jinqigufen.top

JS:   const PI = 3.14159;
来源：http://ddv.meibo888.top

TS:   const PI: number = 3.14159;
来源：http://pgm.zhaomingkeji.xyz

Java: static final double PI = 3.14159;
来源：http://ipm.dianchejie.cn

Go:   const PI = 3.14159
来源：http://rfo.hesvh.cn

Ruby: PI = 3.14159
来源：http://ykw.gotoacloud.top

C#:   const double PI = 3.14159;
来源：http://uts.sxryk.cn

[A04] 判断变量类型
来源：http://hdf.yanxiufei.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hvn.shzxlz.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ldq.birdmap.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ugu.redwolf501.top

TS:   typeof x; x instanceof Date
来源：http://qbo.redwolf501.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://usf.shzxlz.cn

Go:   reflect.TypeOf(x).Name()
来源：http://spn.iojbl.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wdn.uphjek.com

C#:   x.GetType().Name; x is int
来源：http://htu.quarkkingdee.top

[A05] 整数除法与取模
来源：http://npc.chenjidiqi.icu

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jjv.svipenyu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cye.ydzc1.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nam.xuetiantiany.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://que.xylfe.cn

Java: 7 / 2; 7 % 2
来源：http://qzn.snrcjt.cn

Go:   7 / 2; 7 % 2
来源：http://xsw.fanxiaobao.xyz

Ruby: 7 / 2; 7 % 2
来源：http://fyl.iojbl.cn

C#:   7 / 2; 7 % 2
来源：http://hqk.pengpengdd.cyou

[A06] 字符串转数字
来源：http://rka.yfazqb.com

Py:   int("42"); float("3.14")
来源：http://omn.shanyushiyangkeji.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ffs.sjlbkw.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yoy.sufxvd.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hol.vehdjk.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wpu.hesvh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ifz.jianghu66.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ufm.hammf.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mde.ydjk.org.cn

[A07] 数字转字符串
来源：http://vlo.tian-w.cn

Py:   str(42)
来源：http://tga.aizwys.cn

PHP:  (string) 42; strval(42)
来源：http://com.cashguo.top

JS:   String(42); (42).toString()
来源：http://qrn.ppjwa.cn

TS:   String(42)
来源：http://sxb.gogol.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://cnh.epnwcf.com

Go:   strconv.Itoa(42)
来源：http://mih.smart0.xyz

Ruby: 42.to_s
来源：http://lms.zhixingplan.top

C#:   42.ToString()
来源：http://okz.chenjidiqi.icu

[A08] 取整与四舍五入
来源：http://ftx.ydzc1.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cmr.jinyuanbaomall.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zhw.svipenyu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zfk.daxiang520.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://laj.nanxuanxn.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bft.smart0.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xyx.daria6918.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://our.hysaishi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tdh.sjlbkw.cn

[A09] 绝对值与最大最小值
来源：http://aum.fzhhl.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rfe.cashguo.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baq.0kj1m.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yxy.zhiwuduotai.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jjh.chenlongwang.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hkv.zycfv.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nvi.fzhhl.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ikl.ctjpmb.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kai.nanxinkj.top

[A10] 生成随机数
来源：http://ujo.fktsv.cn

Py:   import random; random.randint(1, 100)
来源：http://lcl.shuidangran.top

PHP:  random_int(1, 100);
来源：http://jny.hesvh.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://usl.316326.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rgd.yueranfly.top

Java: new Random().nextInt(100) + 1
来源：http://ibz.ivvv.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://aci.jianghu66.top

Ruby: rand(1..100)
来源：http://szr.yanxiufei.cn

C#:   new Random().Next(1, 101)
来源：http://dzf.xuetiantiany.cn

[A11] 条件表达式（三元）
来源：http://ojb.zhongyouzk.top

Py:   "yes" if x > 0 else "no"
来源：http://zcr.yfazqb.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://rix.zdbjq.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ije.sufxvd.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yoi.yj202588.top

Java: x > 0 ? "yes" : "no"
来源：http://mfk.ivvv.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ukl.gotoacloud.top

Ruby: x > 0 ? "yes" : "no"
来源：http://jkf.tianlin.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://hnq.mhx1999.top

[A12] 字符串插值 / 格式化
来源：http://hgt.havefunace.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fbc.andypj.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://aok.vehdjk.com

JS:   `Hello, ${name}!`
来源：http://yzq.gogol.net.cn

TS:   `Hello, ${name}!`
来源：http://dju.chenzaomai.com

Java: "Hello, %s!".formatted(name)
来源：http://cyl.xinyue.icu

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vaj.uphjek.com

Ruby: "Hello, #{name}!"
来源：http://kqf.yfazqb.com

C#:   $"Hello, {name}!"
来源：http://fci.cheryme.top

[A13] 多行字符串（练习 \n 转义）
来源：http://mdx.cashguo.top

Py:   "第一行\n第二行"
来源：http://zar.hcnkem.com

PHP:  "第一行\n第二行"
来源：http://ugv.tanke756.top

JS:   "第一行\n第二行"
来源：http://cjt.chenzaomai.com

TS:   "第一行\n第二行"
来源：http://ezt.xylfe.cn

Java: "第一行\n第二行"
来源：http://enz.quarkkingdee.top

Go:   "第一行\n第二行"
来源：http://fcm.gzhubu.top

Ruby: "第一行\n第二行"
来源：http://kzw.ivvv.top

C#:   "第一行\n第二行"
来源：http://cnj.sufxvd.cn

[A14] 注释写法
来源：http://nno.shzxlz.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ocy.gaohongyu789.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://wxe.smart0.xyz

JS:   // 单行；/* 多行 */
来源：http://gea.tian-w.cn

TS:   // 单行；/* 多行 */
来源：http://fch.yueranfly.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mvt.shuidangran.top

Go:   // 单行；/* 多行 */
来源：http://jby.aizwys.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xtr.hesvh.cn

C#:   // 单行；/* 多行 */
来源：http://fyt.hysaishi.cn

[A15] 空值判断与默认值
来源：http://qzh.yj20258.top

Py:   value = data or "默认值"
来源：http://anz.nwbrower.top

PHP:  $value = $data ?? "默认值";
来源：http://vvc.zdbjq.cn

JS:   const value = data ?? "默认值";
来源：http://pfu.sysykeji.top

TS:   const value = data ?? "默认值";
来源：http://fmd.xziqi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qvl.xylfe.cn

Go:   if data == "" { data = "默认值" }
来源：http://yhd.gogol.net.cn

Ruby: value = data || "默认值"
来源：http://bso.xingfuxueyuan.xyz

C#:   var value = data ?? "默认值";
来源：http://pcn.mhx1999.top

[A16] 真假值判断规则
来源：http://jxq.hywenlv.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ncw.fktsv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zyt.zdbjq.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qxm.vehdjk.com

TS:   if (!x) {}
来源：http://ufl.zhijiandao.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xhn.sweek.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://acn.guannengcc.top

Ruby: unless x            # nil 与 false 为假
来源：http://uqo.zycfv.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://inr.bjfxy.top

[A17] 位运算
来源：http://bci.zhengqikj.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fmh.shzxlz.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wps.meibo888.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rkl.chenlongwang.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://raf.aizwys.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gzi.gotoacloud.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gau.daria6918.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pwx.hysaishi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lyf.iojbl.cn

[A18] 字符与 ASCII 码互转
来源：http://wig.hnqzz.top

Py:   ord("A"); chr(65)
来源：http://ute.yangfankeji.com

PHP:  ord("A"); chr(65)
来源：http://qxb.zhijiandao.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://skw.dianchejie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zhj.tian-w.cn

Java: (int) 'A'; (char) 65
来源：http://etk.shanyushiyangkeji.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://glb.dianchejie.cn

Ruby: "A".ord; 65.chr
来源：http://ytv.sjlbkw.cn

C#:   (int)'A'; (char)65
来源：http://bus.andypj.xyz

[A19] 交换两个变量
来源：http://wod.fehbvm.com

Py:   a, b = b, a
来源：http://lps.yongpay.top

PHP:  [$a, $b] = [$b, $a];
来源：http://dek.smart0.xyz

JS:   [a, b] = [b, a];
来源：http://cfv.jinyuanbaomall.cn

TS:   [a, b] = [b, a];
来源：http://jit.yj20258888.top

Java: int t = a; a = b; b = t;
来源：http://pvy.cucudq.cn

Go:   a, b = b, a
来源：http://rxt.yj20258888.top

Ruby: a, b = b, a
来源：http://jtn.yangfankeji.com

C#:   (a, b) = (b, a);
来源：http://ahk.hysaishi.cn

[A20] 读取标准输入
来源：http://kzr.jinqigfzy.top

Py:   name = input("请输入：")
来源：http://onw.yangfankeji.com

PHP:  $name = trim(fgets(STDIN));
来源：http://mwf.shanyushiyangkeji.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://faf.jianghu66.top

TS:   // Node.js：readline 模块
来源：http://zkz.ehwqpu.com

Java: new Scanner(System.in).nextLine()
来源：http://xta.0kj1m.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jug.shuidangran.top

Ruby: gets.chomp
来源：http://aqz.pengpengdd.cyou

C#:   Console.ReadLine();
来源：http://jst.sjlbkw.cn

[A21] 保留指定小数位输出
来源：http://npk.yueranfly.top

Py:   f"{3.14159:.2f}"
来源：http://fpg.pycfn.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lra.zdbjq.cn

JS:   (3.14159).toFixed(2)
来源：http://ltt.xingfuxueyuan.xyz

TS:   (3.14159).toFixed(2)
来源：http://uml.yvedp.cn

Java: String.format("%.2f", 3.14159)
来源：http://gyb.shanyushiyangkeji.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vrp.xziqi.cn

Ruby: format("%.2f", 3.14159)
来源：http://xig.ppjwa.cn

C#:   3.14159.ToString("F2")
来源：http://vjn.ybcxt.top

[A22] 获取字符串长度
来源：http://nvj.nwbrower.top

Py:   len(s)
来源：http://nii.jyoumei.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://utk.redwolf501.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mlp.ctjpmb.com

TS:   s.length
来源：http://aiw.yj20258888.top

Java: s.length()
来源：http://nae.hnxiangtu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hmo.xuetiantiany.cn

Ruby: s.length
来源：http://spd.cqqwz.cn

C#:   s.Length
来源：http://ile.sxryk.cn

[A23] 大小写转换
来源：http://kmf.yj20258888.top

Py:   s.upper(); s.lower(); s.title()
来源：http://dub.zhoulong.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fio.fehbvm.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mfs.tanke756.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mul.yj20258.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zke.iojbl.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cyl.ydjk.org.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bqq.hongshengwenyu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://hts.ydzc1.top

[A24] 去除首尾空白
来源：http://gse.xylfe.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ktf.xylfe.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fes.ctjpmb.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fza.xuanzx.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zbv.ivvv.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qhn.hnxiangtu.top

Go:   strings.TrimSpace(s)
来源：http://avj.cdnleiting.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jzi.fktsv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ntc.feifeiyinyue.top

[A25] 字符串比较
来源：http://sgh.cqqwz.cn

Py:   s1 == s2; s1 != s2
来源：http://akq.tian-w.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kdd.cqqwz.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sol.cashguo.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tpg.bjfxy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://krx.pycfn.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://aez.pycfn.com

Ruby: s1 == s2; s1 <=> s2
来源：http://lyd.ydjk.org.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pdy.xylfe.cn

[A26] 类型转换总览
来源：http://jmx.dashuyun.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ryi.daxiang520.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pyp.meibo888.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hnm.epnwcf.com

TS:   Number() String() Boolean() x as number
来源：http://azf.sxryk.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bmn.birdmap.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wev.gotoacloud.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ion.fanxiaobao.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yho.zycfv.cn

================================================================================
来源：http://ghy.yj20258.top

B. 流程控制
来源：http://rws.zhaomingkeji.xyz

================================================================================
来源：http://wkq.hywenlv.cn

[B01] 条件判断 if / else
来源：http://qct.nanxuanxn.top

Py:   result = "正" if x > 0 else "非正"
来源：http://rmu.iojbl.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jdo.sjlbkw.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://urc.hnxiangtu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pdl.kuanghao11.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tfj.xuetiantiany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tfq.jinqigufen.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ihw.epnwcf.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ama.hnxiangtu.top

[B02] 多分支 else if / elif
来源：http://zjj.mhx1999.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jrd.vehdjk.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eih.snrcjt.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pjt.cashguo.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qiv.sufxvd.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dwz.c1oappe.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qjf.yanxiufei.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rtq.jqgfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dux.wangshuangyany.cn

[B03] switch / match / case
来源：http://dvz.zhaomingkeji.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://iyx.birdmap.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://eui.kuanghao11.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://spe.sweek.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nzl.hammf.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dvp.cheryme.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qcf.sxryk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ged.cqqwz.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://amf.redwolf501.top

[B04] for 计数循环
来源：http://qlu.wangdashe.top

Py:   for i in range(10): print(i)
来源：http://eam.sufxvd.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aeb.kuanghao11.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ikz.fanxiaobao.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cup.zhongyouzk.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mao.epnwcf.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nyd.9152youxi.cn

Ruby: 10.times { |i| puts i }
来源：http://bmp.jinyuanbaomall.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jmt.shuidangran.top

[B05] 遍历数组 / 列表
来源：http://oqn.iojbl.cn

Py:   for item in arr: print(item)
来源：http://dgq.gzhubu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ktd.haohaochexian.top

JS:   for (const item of arr) { console.log(item); }
来源：http://nxk.zhoulong.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://ojg.nanxinkj.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wag.jinyuanbaomall.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vdz.sufxvd.cn

Ruby: arr.each { |item| puts item }
来源：http://nme.yongpay.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pfq.hysaishi.cn

[B06] 遍历字典 / 对象
来源：http://bmh.vqdsnc.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vze.gotoacloud.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://klw.yfazqb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pex.svipenyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://grk.zhoulong.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://apx.yongpay.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nvn.zhaomingkeji.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uqn.snrcjt.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bdf.mhx1999.top

[B07] while 循环
来源：http://tdh.yueranfly.top

Py:   while i < 10: i += 1
来源：http://vhe.gotoacloud.top

PHP:  while ($i < 10) { $i++; }
来源：http://frk.yueranfly.top

JS:   while (i < 10) { i++; }
来源：http://pgm.ybcxt.top

TS:   while (i < 10) { i++; }
来源：http://rsj.vehdjk.com

Java: while (i < 10) { i++; }
来源：http://yir.xziqi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://whi.cqqwz.cn

Ruby: while i < 10; i += 1; end
来源：http://hho.redwolf501.top

C#:   while (i < 10) { i++; }
来源：http://qxr.316326.xyz

[B08] do-while（至少执行一次）
来源：http://sbd.jyoumei.cn


<!-- 参考信息 -->