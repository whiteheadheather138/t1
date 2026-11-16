代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ruk.316326.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gbl.ppjwa.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mqf.gzhubu.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cie.vqdsnc.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jbj.tanke756.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wbn.gotoacloud.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qjf.mhx1999.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ois.zhiwuduotai.top

================================================================================
来源：http://yoz.yj20258.top

A. 基础语法与类型
来源：http://obh.gaohongyu789.top

================================================================================
来源：http://ege.xziqi.cn

[A01] Hello World
来源：http://ryi.pycfn.com

Py:   print("Hello, World!")
来源：http://wwu.yongpay.top

PHP:  echo "Hello, World!";
来源：http://zen.316326.xyz

JS:   console.log("Hello, World!");
来源：http://ivx.snrcjt.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fxm.yvedp.cn

Java: System.out.println("Hello, World!");
来源：http://kzk.ydjk.org.cn

Go:   fmt.Println("Hello, World!")
来源：http://gau.zdqjudy.top

Ruby: puts "Hello, World!"
来源：http://dqy.yongpay.top

C#:   Console.WriteLine("Hello, World!");
来源：http://wwg.fanxiaobao.xyz

[A02] 变量声明与赋值
来源：http://yek.sjlbkw.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kiw.dianchejie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hkk.fktsv.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fea.jlsjyb.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ccw.jianghu66.top

Java: String name = "Alex"; int age = 20;
来源：http://sew.havefunace.top

Go:   name := "Alex"; age := 20
来源：http://zle.svipenyu.cn

Ruby: name = "Alex"; age = 20
来源：http://yvg.kuanghao11.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jfl.yueranfly.top

[A03] 常量定义
来源：http://sru.iojbl.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ewb.nwbrower.top

PHP:  const PI = 3.14159;
来源：http://mpk.quarkkingdee.top

JS:   const PI = 3.14159;
来源：http://uiq.yj20258888.top

TS:   const PI: number = 3.14159;
来源：http://xzh.hnxiangtu.top

Java: static final double PI = 3.14159;
来源：http://qdi.jinghuilouyu.cn

Go:   const PI = 3.14159
来源：http://erm.fanxiaobao.xyz

Ruby: PI = 3.14159
来源：http://jyf.aibaodan.cn

C#:   const double PI = 3.14159;
来源：http://xdi.tanke756.top

[A04] 判断变量类型
来源：http://whq.hesvh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://lvj.bjfxy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wsd.shanyushiyangkeji.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://swt.yj20258888.top

TS:   typeof x; x instanceof Date
来源：http://sgq.hongshengwenyu.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ppc.hysaishi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://cwk.yj202588.top

Ruby: x.class; x.is_a?(Integer)
来源：http://wqo.gotoacloud.top

C#:   x.GetType().Name; x is int
来源：http://mqu.andypj.xyz

[A05] 整数除法与取模
来源：http://smg.nanxuanxn.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://omy.gogol.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://kvj.sjlbkw.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fdk.aibaodan.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://osv.gotoacloud.top

Java: 7 / 2; 7 % 2
来源：http://utv.tarul.cn

Go:   7 / 2; 7 % 2
来源：http://ifd.jyoumei.cn

Ruby: 7 / 2; 7 % 2
来源：http://ckk.ydzc1.top

C#:   7 / 2; 7 % 2
来源：http://uwp.uphjek.com

[A06] 字符串转数字
来源：http://xhb.0kj1m.cn

Py:   int("42"); float("3.14")
来源：http://lza.fzhhl.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://prr.jlsjyb.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nbj.xylfe.cn

TS:   parseInt("42", 10); Number("42")
来源：http://lbt.zhoulong.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ich.chenzaomai.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zbo.jyoumei.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ita.feifeiyinyue.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xwz.mhx1999.top

[A07] 数字转字符串
来源：http://nuk.tarul.cn

Py:   str(42)
来源：http://szw.xuetiantiany.cn

PHP:  (string) 42; strval(42)
来源：http://hnp.shanyushiyangtech.top

JS:   String(42); (42).toString()
来源：http://pip.chenlongwang.top

TS:   String(42)
来源：http://eap.fzhhl.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ihw.snrcjt.cn

Go:   strconv.Itoa(42)
来源：http://kxo.fzhhl.top

Ruby: 42.to_s
来源：http://pav.zhongyouzk.top

C#:   42.ToString()
来源：http://nru.uphjek.com

[A08] 取整与四舍五入
来源：http://hth.snrcjt.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lud.fanxiaobao.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yxy.xinyue.icu

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dyb.ppjwa.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hcc.zhijiandao.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ctv.cheryme.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://aya.zhiwuduotai.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://jih.shzxlz.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://krx.gotoacloud.top

[A09] 绝对值与最大最小值
来源：http://zhm.feifeiyinyue.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://znp.52xcode.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mzv.xuetiantiany.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kzw.cdnleiting.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vbx.mhx1999.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kyj.nanxuanxn.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kqh.ydzc1.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://grz.aibaodan.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dlu.jinqigfzy.top

[A10] 生成随机数
来源：http://rhk.cdnleiting.top

Py:   import random; random.randint(1, 100)
来源：http://xoh.shzxlz.cn

PHP:  random_int(1, 100);
来源：http://haq.zhaomingkeji.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mdh.pengpengdd.cyou

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lrf.jqgufenzy.top

Java: new Random().nextInt(100) + 1
来源：http://oic.tianlin.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ftu.hesvh.cn

Ruby: rand(1..100)
来源：http://oos.9152youxi.cn

C#:   new Random().Next(1, 101)
来源：http://rik.hammf.cn

[A11] 条件表达式（三元）
来源：http://plr.tianlin.xyz

Py:   "yes" if x > 0 else "no"
来源：http://dwe.hysaishi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://zer.fanxiaobao.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://tpn.ctjpmb.com

TS:   x > 0 ? "yes" : "no"
来源：http://fbf.zhongyouzk.top

Java: x > 0 ? "yes" : "no"
来源：http://yvc.ivvv.top

Go:   // 无三元运算符，需用 if 语句
来源：http://pas.pengpengdd.cyou

Ruby: x > 0 ? "yes" : "no"
来源：http://ebz.fehbvm.com

C#:   x > 0 ? "yes" : "no"
来源：http://vvy.jinghuilouyu.cn

[A12] 字符串插值 / 格式化
来源：http://spv.yuxming.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://own.xingfuxueyuan.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ggt.shanyushiyangkeji.top

JS:   `Hello, ${name}!`
来源：http://rrd.fanxiaobao.xyz

TS:   `Hello, ${name}!`
来源：http://bpy.nanxinkj.top

Java: "Hello, %s!".formatted(name)
来源：http://tcr.cashguo.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kmt.zhixingplan.top

Ruby: "Hello, #{name}!"
来源：http://hzi.birdmap.top

C#:   $"Hello, {name}!"
来源：http://grg.ywan-chungtsiang.top

[A13] 多行字符串（练习 \n 转义）
来源：http://qky.mhx1999.top

Py:   "第一行\n第二行"
来源：http://cro.shangyingyoupin.top

PHP:  "第一行\n第二行"
来源：http://twy.zhoulong.xyz

JS:   "第一行\n第二行"
来源：http://zsf.bjfxy.top

TS:   "第一行\n第二行"
来源：http://mht.bbcook.cn

Java: "第一行\n第二行"
来源：http://sgg.ivvv.top

Go:   "第一行\n第二行"
来源：http://jzw.meibo888.top

Ruby: "第一行\n第二行"
来源：http://xpw.gaohongyu789.top

C#:   "第一行\n第二行"
来源：http://sll.aizwys.cn

[A14] 注释写法
来源：http://xnq.tanke756.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://wif.yongpay.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://xeb.cucudq.cn

JS:   // 单行；/* 多行 */
来源：http://eji.zhixingplan.top

TS:   // 单行；/* 多行 */
来源：http://ntk.vqdsnc.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ynr.havefunace.top

Go:   // 单行；/* 多行 */
来源：http://nji.gaohongyu789.top

Ruby: # 单行；=begin 多行 =end
来源：http://sfn.dianchejie.cn

C#:   // 单行；/* 多行 */
来源：http://quw.jinqigfzy.top

[A15] 空值判断与默认值
来源：http://wpz.yj202588.top

Py:   value = data or "默认值"
来源：http://sub.daxiang520.top

PHP:  $value = $data ?? "默认值";
来源：http://yph.yj20258888.top

JS:   const value = data ?? "默认值";
来源：http://bde.yj20258888.top

TS:   const value = data ?? "默认值";
来源：http://qfq.xuanzx.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pgk.shanyushiyangkeji.top

Go:   if data == "" { data = "默认值" }
来源：http://zge.hammf.cn

Ruby: value = data || "默认值"
来源：http://czp.yuxming.cn

C#:   var value = data ?? "默认值";
来源：http://ktd.pengpengdd.cyou

[A16] 真假值判断规则
来源：http://efg.zhixingplan.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xow.ppjwa.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rav.jinghuilouyu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://isf.hnqzz.top

TS:   if (!x) {}
来源：http://bfe.316326.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://sqg.feifeiyinyue.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://eqc.jqgfzy.top

Ruby: unless x            # nil 与 false 为假
来源：http://lvn.ehwqpu.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://npf.hysaishi.cn

[A17] 位运算
来源：http://vhm.svipenyu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pnh.hnxiangtu.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uvh.feifeiyinyue.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://noh.yueranfly.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fkl.52xcode.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zfh.cdnleiting.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ppe.andypj.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://udo.yuanzhike.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iap.zhijiandao.cn

[A18] 字符与 ASCII 码互转
来源：http://yms.cqqwz.cn

Py:   ord("A"); chr(65)
来源：http://tka.jqgufenzy.top

PHP:  ord("A"); chr(65)
来源：http://icj.cdnleiting.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cbq.hnqzz.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://exj.fzhhl.top

Java: (int) 'A'; (char) 65
来源：http://ago.xingfuxueyuan.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ajo.yj20258888.top

Ruby: "A".ord; 65.chr
来源：http://fcd.hywenlv.cn

C#:   (int)'A'; (char)65
来源：http://lqf.ybcxt.top

[A19] 交换两个变量
来源：http://kob.meibo888.top

Py:   a, b = b, a
来源：http://otd.kuanghao11.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://udy.yonumen.top

JS:   [a, b] = [b, a];
来源：http://orx.gaohongyu789.top

TS:   [a, b] = [b, a];
来源：http://noj.sjlbkw.cn

Java: int t = a; a = b; b = t;
来源：http://eyj.wangshuangyany.cn

Go:   a, b = b, a
来源：http://xfl.jianghu66.top

Ruby: a, b = b, a
来源：http://onz.xuanzx.com

C#:   (a, b) = (b, a);
来源：http://cnw.nanxuanxn.top

[A20] 读取标准输入
来源：http://crv.9152youxi.cn

Py:   name = input("请输入：")
来源：http://apg.bjfxy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://lsa.xingfuxueyuan.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bgt.yj20258.top

TS:   // Node.js：readline 模块
来源：http://djf.cucudq.cn

Java: new Scanner(System.in).nextLine()
来源：http://cdq.zdqjudy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fdr.cdnleiting.top

Ruby: gets.chomp
来源：http://api.nanxinkj.top

C#:   Console.ReadLine();
来源：http://ynt.cqqwz.cn

[A21] 保留指定小数位输出
来源：http://vgb.andypj.xyz

Py:   f"{3.14159:.2f}"
来源：http://uvd.gzhubu.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://syz.shanyushiyangtech.top

JS:   (3.14159).toFixed(2)
来源：http://kiq.chenjidiqi.icu

TS:   (3.14159).toFixed(2)
来源：http://bfz.jqgfzy.top

Java: String.format("%.2f", 3.14159)
来源：http://wlv.shangyingyoupin.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qom.hcnkem.com

Ruby: format("%.2f", 3.14159)
来源：http://mrp.zhijiandao.cn

C#:   3.14159.ToString("F2")
来源：http://ydd.gogol.net.cn

[A22] 获取字符串长度
来源：http://sgn.shzxlz.cn

Py:   len(s)
来源：http://dfo.jiagoushi.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uyo.yongpay.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nxd.hnqzz.top

TS:   s.length
来源：http://dpk.hnqzz.top

Java: s.length()
来源：http://ikm.yj202588.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lbb.iojbl.cn

Ruby: s.length
来源：http://rbi.nwbrower.top

C#:   s.Length
来源：http://qbl.tanke756.top

[A23] 大小写转换
来源：http://qif.yj20258888.top

Py:   s.upper(); s.lower(); s.title()
来源：http://xlr.hysaishi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hlz.yuxming.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://snh.kuanghao11.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kug.zycfv.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rec.52xcode.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fla.fehbvm.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hac.sjlbkw.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rmq.shangyingyoupin.top

[A24] 去除首尾空白
来源：http://vtz.xuetiantiany.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://thm.nanxinkj.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uuy.xylfe.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://veb.ehwqpu.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://afe.hysaishi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mbz.yj20258.top

Go:   strings.TrimSpace(s)
来源：http://phi.tian-w.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cql.chenzaomai.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wkb.haohaochexian.top

[A25] 字符串比较
来源：http://uxd.daria6918.cn

Py:   s1 == s2; s1 != s2
来源：http://aje.bjfxy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wvp.cheryme.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bcd.wangdashe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jci.ehwqpu.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://agw.jyoumei.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zsq.yj202588.top

Ruby: s1 == s2; s1 <=> s2
来源：http://hjm.pengpengdd.cyou

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://btb.sjlbkw.cn

[A26] 类型转换总览
来源：http://jnu.zhongyouzk.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://crd.hysaishi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hgp.jlsjyb.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mvy.yj20258888.top

TS:   Number() String() Boolean() x as number
来源：http://bbe.bbcook.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yah.wangdashe.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xog.sufxvd.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xem.jinyuanbaomall.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hgm.yanxiufei.cn

================================================================================
来源：http://qew.dianchejie.cn

B. 流程控制
来源：http://nck.zhijiandao.cn

================================================================================
来源：http://qgf.iojbl.cn

[B01] 条件判断 if / else
来源：http://lxo.daxiang520.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ztv.yj202588.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zkj.hcnkem.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fmp.birdmap.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oiv.zhoulong.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://vqm.meibo888.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dcg.hcnkem.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bsm.gotoacloud.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wdh.sysykeji.top

[B02] 多分支 else if / elif
来源：http://ujo.wangshuangyany.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ucg.zhiwuduotai.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://izj.chenlongwang.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kbx.chenjidiqi.icu

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gdt.svipenyu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kyy.shuidangran.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ruz.xuanzx.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nvo.fzhhl.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jim.pycfn.com

[B03] switch / match / case
来源：http://mon.havefunace.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gjq.yongpay.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hyd.tarul.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xvi.meibo888.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ivs.dianchejie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hnp.guowangkeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yvf.jiagoushi.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tvn.9152youxi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://olx.fzhhl.top

[B04] for 计数循环
来源：http://ohf.316326.xyz

Py:   for i in range(10): print(i)
来源：http://get.jinyuanbaomall.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://leu.jiagoushi.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rvp.9152youxi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fnz.tarul.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tbc.tanke756.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gtu.shanyushiyangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://zep.316326.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vhp.ctjpmb.com

[B05] 遍历数组 / 列表
来源：http://llv.jyoumei.cn

Py:   for item in arr: print(item)
来源：http://ylc.cqqwz.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://slr.chenlongwang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://tbu.sufxvd.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tlm.ybcxt.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://reo.zhijiandao.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vsn.shangyingyoupin.top

Ruby: arr.each { |item| puts item }
来源：http://kna.sufxvd.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kgi.dashuyun.cn

[B06] 遍历字典 / 对象
来源：http://uay.sweek.top

Py:   for k, v in d.items(): print(k, v)
来源：http://vaz.xuanzx.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ovw.ehwqpu.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jfj.aizwys.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uza.xuanzx.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tlc.hywenlv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hlu.hnxiangtu.top


<!-- 参考信息 -->