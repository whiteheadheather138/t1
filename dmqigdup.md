代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xzd.52xcode.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fqy.smart0.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wls.zhoulong.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://uyj.yonumen.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pgw.jinqigfzy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qfn.jlsjyb.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rnr.jiagoushi.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://eil.tianlin.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://ykw.shuidangran.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lcr.hammf.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mjc.yanxiufei.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zld.nanxuanxn.top

================================================================================
来源：http://djw.guowangkeji.top

A. 基础语法与类型
来源：http://czl.gogol.net.cn

================================================================================
来源：http://zmj.tian-w.cn

[A01] Hello World
来源：http://rkb.xziqi.cn

Py:   print("Hello, World!")
来源：http://mxe.sweek.top

PHP:  echo "Hello, World!";
来源：http://xjf.wangdashe.top

JS:   console.log("Hello, World!");
来源：http://grp.jqgfzy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zzv.dashuyun.cn

Java: System.out.println("Hello, World!");
来源：http://wtm.yanxiufei.cn

Go:   fmt.Println("Hello, World!")
来源：http://uhg.jiagoushi.top

Ruby: puts "Hello, World!"
来源：http://itk.jiagoushi.top

C#:   Console.WriteLine("Hello, World!");
来源：http://epg.yanxiufei.cn

[A02] 变量声明与赋值
来源：http://rqo.fehbvm.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://iie.birdmap.top

PHP:  $name = "Alex"; $age = 20;
来源：http://rhk.yongpay.top

JS:   let name = "Alex"; const age = 20;
来源：http://tkb.yj20258.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://utc.snrcjt.cn

Java: String name = "Alex"; int age = 20;
来源：http://phd.redwolf501.top

Go:   name := "Alex"; age := 20
来源：http://bdf.zdqjudy.top

Ruby: name = "Alex"; age = 20
来源：http://ojg.yuxming.cn

C#:   string name = "Alex"; int age = 20;
来源：http://qwu.snrcjt.cn

[A03] 常量定义
来源：http://pkz.yonumen.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nnl.svipenyu.cn

PHP:  const PI = 3.14159;
来源：http://spz.52xcode.cn

JS:   const PI = 3.14159;
来源：http://lte.jianghu66.top

TS:   const PI: number = 3.14159;
来源：http://ogt.vqdsnc.cn

Java: static final double PI = 3.14159;
来源：http://mkm.yvedp.cn

Go:   const PI = 3.14159
来源：http://hly.zhaomingkeji.xyz

Ruby: PI = 3.14159
来源：http://bax.yfazqb.com

C#:   const double PI = 3.14159;
来源：http://oqh.yongpay.top

[A04] 判断变量类型
来源：http://usk.shzxlz.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rcf.cqqwz.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hdc.yvedp.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rsy.zhaomingkeji.xyz

TS:   typeof x; x instanceof Date
来源：http://iwo.birdmap.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pco.zdbjq.cn

Go:   reflect.TypeOf(x).Name()
来源：http://gcu.tianlin.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://cec.chenjidiqi.icu

C#:   x.GetType().Name; x is int
来源：http://scp.yj202588.top

[A05] 整数除法与取模
来源：http://qcg.jiagoushi.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jhi.vqdsnc.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://juf.cucudq.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wby.mhx1999.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cjk.9152youxi.cn

Java: 7 / 2; 7 % 2
来源：http://ztc.hongshengwenyu.top

Go:   7 / 2; 7 % 2
来源：http://iie.yj20258888.top

Ruby: 7 / 2; 7 % 2
来源：http://bwz.jianghu66.top

C#:   7 / 2; 7 % 2
来源：http://ubc.9152youxi.cn

[A06] 字符串转数字
来源：http://kwj.ydzc1.top

Py:   int("42"); float("3.14")
来源：http://zav.jiagoushi.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pnc.nanxuanxn.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hyq.guannengcc.top

TS:   parseInt("42", 10); Number("42")
来源：http://hcd.shanyushiyangkeji.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mmo.feifeiyinyue.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nll.sweek.top

Ruby: "42".to_i; "3.14".to_f
来源：http://dqp.ivvv.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fdz.xingfuxueyuan.xyz

[A07] 数字转字符串
来源：http://rtp.tarul.cn

Py:   str(42)
来源：http://lii.sysykeji.top

PHP:  (string) 42; strval(42)
来源：http://qrj.xingfuxueyuan.xyz

JS:   String(42); (42).toString()
来源：http://iqa.shanyushiyangtech.top

TS:   String(42)
来源：http://kkp.shangyingyoupin.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://hyh.fktsv.cn

Go:   strconv.Itoa(42)
来源：http://gcn.jlsjyb.cn

Ruby: 42.to_s
来源：http://jqk.shuidangran.top

C#:   42.ToString()
来源：http://vox.yfazqb.com

[A08] 取整与四舍五入
来源：http://hsr.nanxinkj.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cle.haohaochexian.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kgd.zhoulong.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wkw.xziqi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ufx.xylfe.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lbk.ydjk.org.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://uro.ctjpmb.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://hyu.meibo888.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wyv.zhengqikj.top

[A09] 绝对值与最大最小值
来源：http://mpx.tanke756.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qwq.zhongyouzk.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wyg.sxryk.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vld.ydjk.org.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nvq.shzxlz.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bcg.chenzaomai.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rjs.tianlin.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rcy.andypj.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rtp.dashuyun.cn

[A10] 生成随机数
来源：http://vsg.bbcook.cn

Py:   import random; random.randint(1, 100)
来源：http://tpn.redwolf501.top

PHP:  random_int(1, 100);
来源：http://tzx.jinyuanbaomall.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cxv.gotoacloud.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://aaz.dashuyun.cn

Java: new Random().nextInt(100) + 1
来源：http://zve.iojbl.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nik.pengpengdd.cyou

Ruby: rand(1..100)
来源：http://vye.iojbl.cn

C#:   new Random().Next(1, 101)
来源：http://hhc.zhaomingkeji.xyz

[A11] 条件表达式（三元）
来源：http://nuq.kuanghao11.cn

Py:   "yes" if x > 0 else "no"
来源：http://tyf.uphjek.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://yin.jinghuilouyu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pqc.sxryk.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vgw.shanyushiyangkeji.top

Java: x > 0 ? "yes" : "no"
来源：http://ljb.sufxvd.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hfy.gzhubu.top

Ruby: x > 0 ? "yes" : "no"
来源：http://jzm.yueranfly.top

C#:   x > 0 ? "yes" : "no"
来源：http://mai.jlsjyb.cn

[A12] 字符串插值 / 格式化
来源：http://wgk.ywan-chungtsiang.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://opy.nanxinkj.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://awv.fanxiaobao.xyz

JS:   `Hello, ${name}!`
来源：http://bwi.cucudq.cn

TS:   `Hello, ${name}!`
来源：http://ytb.jianghu66.top

Java: "Hello, %s!".formatted(name)
来源：http://zdt.zhixingplan.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qvk.jinghuilouyu.cn

Ruby: "Hello, #{name}!"
来源：http://nzz.daxiang520.top

C#:   $"Hello, {name}!"
来源：http://bku.yuxming.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hvl.shanyushiyangtech.top

Py:   "第一行\n第二行"
来源：http://uvw.ehwqpu.com

PHP:  "第一行\n第二行"
来源：http://sdo.redwolf501.top

JS:   "第一行\n第二行"
来源：http://fhu.hnqzz.top

TS:   "第一行\n第二行"
来源：http://onc.hnxiangtu.top

Java: "第一行\n第二行"
来源：http://xxa.jinyuanbaomall.cn

Go:   "第一行\n第二行"
来源：http://bbe.yonumen.top

Ruby: "第一行\n第二行"
来源：http://inr.fengsongda.top

C#:   "第一行\n第二行"
来源：http://csu.gogol.net.cn

[A14] 注释写法
来源：http://imk.nanxuanxn.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://orj.hnqzz.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://yon.hesvh.cn

JS:   // 单行；/* 多行 */
来源：http://dpq.aizwys.cn

TS:   // 单行；/* 多行 */
来源：http://ajl.shzxlz.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jvb.pengpengdd.cyou

Go:   // 单行；/* 多行 */
来源：http://lmk.ivvv.top

Ruby: # 单行；=begin 多行 =end
来源：http://xzh.guannengcc.top

C#:   // 单行；/* 多行 */
来源：http://wpb.yangfankeji.com

[A15] 空值判断与默认值
来源：http://gld.chenjidiqi.icu

Py:   value = data or "默认值"
来源：http://pxz.xylfe.cn

PHP:  $value = $data ?? "默认值";
来源：http://frc.pycfn.com

JS:   const value = data ?? "默认值";
来源：http://kre.jiagoushi.top

TS:   const value = data ?? "默认值";
来源：http://qry.vehdjk.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sfm.yongpay.top

Go:   if data == "" { data = "默认值" }
来源：http://xpe.zycfv.cn

Ruby: value = data || "默认值"
来源：http://cqy.wangshuangyany.cn

C#:   var value = data ?? "默认值";
来源：http://cuj.zdbjq.cn

[A16] 真假值判断规则
来源：http://frt.ywan-chungtsiang.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jhg.hongshengwenyu.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yup.zdbjq.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rmi.yj20258888.top

TS:   if (!x) {}
来源：http://noi.feifeiyinyue.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://smh.iojbl.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ujj.cqqwz.cn

Ruby: unless x            # nil 与 false 为假
来源：http://pdj.fzhhl.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uxp.ppjwa.cn

[A17] 位运算
来源：http://qpf.xinyue.icu

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ctj.zdqjudy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://asf.tarul.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sth.fktsv.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hxr.shzxlz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://txj.ppjwa.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jgv.nanxuanxn.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cnr.haohaochexian.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xaj.daxiang520.top

[A18] 字符与 ASCII 码互转
来源：http://bfb.yongpay.top

Py:   ord("A"); chr(65)
来源：http://ojh.zhoulong.xyz

PHP:  ord("A"); chr(65)
来源：http://sig.c1oappe.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tnp.meibo888.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mry.0kj1m.cn

Java: (int) 'A'; (char) 65
来源：http://crn.jinqigfzy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://msn.gaohongyu789.top

Ruby: "A".ord; 65.chr
来源：http://wrs.fzhhl.top

C#:   (int)'A'; (char)65
来源：http://une.chenjidiqi.icu

[A19] 交换两个变量
来源：http://nks.chenlongwang.top

Py:   a, b = b, a
来源：http://med.mhx1999.top

PHP:  [$a, $b] = [$b, $a];
来源：http://krf.yfazqb.com

JS:   [a, b] = [b, a];
来源：http://ajd.hfpthk.cn

TS:   [a, b] = [b, a];
来源：http://mwi.chenlongwang.top

Java: int t = a; a = b; b = t;
来源：http://bqy.daria6918.cn

Go:   a, b = b, a
来源：http://kwb.dianchejie.cn

Ruby: a, b = b, a
来源：http://fre.jlsjyb.cn

C#:   (a, b) = (b, a);
来源：http://fxj.xuanzx.com

[A20] 读取标准输入
来源：http://lfo.havefunace.top

Py:   name = input("请输入：")
来源：http://tdp.nanxinkj.top

PHP:  $name = trim(fgets(STDIN));
来源：http://sep.hywenlv.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xvd.tanke756.top

TS:   // Node.js：readline 模块
来源：http://jqx.yongpay.top

Java: new Scanner(System.in).nextLine()
来源：http://ncz.sufxvd.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bgx.jianghu66.top

Ruby: gets.chomp
来源：http://fam.c1oappe.top

C#:   Console.ReadLine();
来源：http://rgg.sweek.top

[A21] 保留指定小数位输出
来源：http://len.sjlbkw.cn

Py:   f"{3.14159:.2f}"
来源：http://iqs.yfazqb.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://btq.fktsv.cn

JS:   (3.14159).toFixed(2)
来源：http://jjs.ybcxt.top

TS:   (3.14159).toFixed(2)
来源：http://swn.ydzc1.top

Java: String.format("%.2f", 3.14159)
来源：http://wwy.svipenyu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sqs.svipenyu.cn

Ruby: format("%.2f", 3.14159)
来源：http://cok.xingfuxueyuan.xyz

C#:   3.14159.ToString("F2")
来源：http://tuz.gotoacloud.top

[A22] 获取字符串长度
来源：http://tcl.ivvv.top

Py:   len(s)
来源：http://ylj.xingfuxueyuan.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://awx.fzhhl.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lhq.cdnleiting.top

TS:   s.length
来源：http://nwv.gzhubu.top

Java: s.length()
来源：http://drz.jyoumei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cqq.sxryk.cn

Ruby: s.length
来源：http://hti.ybcxt.top

C#:   s.Length
来源：http://fwi.fktsv.cn

[A23] 大小写转换
来源：http://eln.hesvh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ubg.shanyushiyangkeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pdf.xuanzx.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qaj.sxryk.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cot.aibaodan.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hqk.aizwys.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cgi.redwolf501.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zyb.guowangkeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://nnv.vqdsnc.cn

[A24] 去除首尾空白
来源：http://uqa.bjfxy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zpw.ywan-chungtsiang.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rpg.tarul.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://stv.yvedp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bsg.havefunace.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ahx.kuanghao11.cn

Go:   strings.TrimSpace(s)
来源：http://ifj.ehwqpu.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oqc.quarkkingdee.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zoh.redwolf501.top

[A25] 字符串比较
来源：http://xjk.hnqzz.top

Py:   s1 == s2; s1 != s2
来源：http://epk.gotoacloud.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rnu.yanxiufei.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dgf.fengsongda.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uim.andypj.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ezm.jqgufenzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lmb.cheryme.top

Ruby: s1 == s2; s1 <=> s2
来源：http://awf.cheryme.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://eou.jinghuilouyu.cn

[A26] 类型转换总览
来源：http://bum.cqqwz.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://avj.yongpay.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://azh.zhoulong.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bpt.jiagoushi.top

TS:   Number() String() Boolean() x as number
来源：http://zso.shanyushiyangkeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://and.chenlongwang.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mps.feifeiyinyue.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://lqp.epnwcf.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rdz.tianlin.xyz

================================================================================
来源：http://riw.meibo888.top

B. 流程控制
来源：http://jvk.zhijiandao.cn

================================================================================
来源：http://mjs.zhengqikj.top

[B01] 条件判断 if / else
来源：http://hlr.316326.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://tsv.ywan-chungtsiang.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kkt.uphjek.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://all.yvedp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lom.daria6918.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ucy.tian-w.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dnz.ehwqpu.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wng.fzhhl.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://olw.quarkkingdee.top

[B02] 多分支 else if / elif
来源：http://bhq.zhixingplan.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sjm.wangdashe.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kpp.jinqigufen.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bjy.tianlin.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://asm.tian-w.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ehb.ydzc1.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://idd.tanke756.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fth.guannengcc.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ayo.smart0.xyz

[B03] switch / match / case
来源：http://xoi.jianghu66.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ehq.ivvv.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lml.jianghu66.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sty.iojbl.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ovh.cheryme.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lvt.zhengqikj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vvc.haohaochexian.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ipr.hammf.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iti.yanxiufei.cn

[B04] for 计数循环
来源：http://zpq.xuetiantiany.cn

Py:   for i in range(10): print(i)
来源：http://sti.haohaochexian.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ckn.jianghu66.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cni.fengsongda.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pxi.jiagoushi.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://exx.ivvv.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tux.hesvh.cn

Ruby: 10.times { |i| puts i }
来源：http://ifj.zhoulong.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://czk.birdmap.top

[B05] 遍历数组 / 列表
来源：http://wpk.ydjk.org.cn

Py:   for item in arr: print(item)
来源：http://vcv.andypj.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://krb.hysaishi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dkn.hongshengwenyu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://nvz.epnwcf.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://qvf.jinqigufen.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lmf.jyoumei.cn

Ruby: arr.each { |item| puts item }
来源：http://fqi.zhaomingkeji.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gxh.316326.xyz

[B06] 遍历字典 / 对象
来源：http://vsp.ppjwa.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://can.jiagoushi.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zld.jinyuanbaomall.cn


<!-- 参考信息 -->