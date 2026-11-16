代发 wailian999

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gep.xziqi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://aft.zhoulong.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fxl.tian-w.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gup.gzhubu.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rnw.yanxiufei.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vpp.fzhhl.top

【文件统计】
来源：http://ztd.shanyushiyangkeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://adq.shuidangran.top

--------------------------------------------------------------------------------
来源：http://edt.ctjpmb.com

目  录
来源：http://vpu.vehdjk.com

--------------------------------------------------------------------------------
来源：http://bsf.0kj1m.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://igq.yuanzhike.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tje.svipenyu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://amd.yj20258888.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hbp.ybcxt.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://spv.fktsv.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mud.zhixingplan.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bbi.fanxiaobao.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hlk.hongshengwenyu.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://obq.daxiang520.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mkf.mhx1999.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://aeq.zdqjudy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xiv.ctjpmb.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ozs.jiagoushi.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dzz.zhaomingkeji.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://guy.shzxlz.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lqp.nwbrower.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://miu.hcnkem.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://dfw.xinyue.icu

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cgo.zhiwuduotai.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ddt.gaohongyu789.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yrs.zhaomingkeji.xyz

================================================================================
来源：http://zof.jlsjyb.cn

A. 基础语法与类型
来源：http://dwh.hysaishi.cn

================================================================================
来源：http://wjj.shanyushiyangkeji.top

[A01] Hello World
来源：http://dou.xuetiantiany.cn

Py:   print("Hello, World!")
来源：http://mhf.jyoumei.cn

PHP:  echo "Hello, World!";
来源：http://rtf.chenlongwang.top

JS:   console.log("Hello, World!");
来源：http://fxm.sweek.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rpo.haohaochexian.top

Java: System.out.println("Hello, World!");
来源：http://wid.shanyushiyangkeji.top

Go:   fmt.Println("Hello, World!")
来源：http://weq.yuxming.cn

Ruby: puts "Hello, World!"
来源：http://lvs.hysaishi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hqq.ywan-chungtsiang.top

[A02] 变量声明与赋值
来源：http://aog.jqgufenzy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jxc.sufxvd.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ens.ywan-chungtsiang.top

JS:   let name = "Alex"; const age = 20;
来源：http://cdw.jqgufenzy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://las.gzhubu.top

Java: String name = "Alex"; int age = 20;
来源：http://aym.yonumen.top

Go:   name := "Alex"; age := 20
来源：http://ark.nanxinkj.top

Ruby: name = "Alex"; age = 20
来源：http://kdt.xuanzx.com

C#:   string name = "Alex"; int age = 20;
来源：http://fhk.xuanzx.com

[A03] 常量定义
来源：http://mzb.guowangkeji.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://krn.zycfv.cn

PHP:  const PI = 3.14159;
来源：http://qdb.jinqigufen.top

JS:   const PI = 3.14159;
来源：http://nav.hnxiangtu.top

TS:   const PI: number = 3.14159;
来源：http://nih.mhx1999.top

Java: static final double PI = 3.14159;
来源：http://muk.andypj.xyz

Go:   const PI = 3.14159
来源：http://vnb.zdqjudy.top

Ruby: PI = 3.14159
来源：http://wdp.pycfn.com

C#:   const double PI = 3.14159;
来源：http://grs.gaohongyu789.top

[A04] 判断变量类型
来源：http://skz.pycfn.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://wib.andypj.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wko.hcnkem.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wvq.guannengcc.top

TS:   typeof x; x instanceof Date
来源：http://yfs.tanke756.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://buh.dashuyun.cn

Go:   reflect.TypeOf(x).Name()
来源：http://cnt.cucudq.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vwg.gzhubu.top

C#:   x.GetType().Name; x is int
来源：http://say.hammf.cn

[A05] 整数除法与取模
来源：http://lnp.zdqjudy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yfg.chenjidiqi.icu

PHP:  intdiv(7, 2); 7 % 2
来源：http://ruj.havefunace.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xmw.fengsongda.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lpk.tian-w.cn

Java: 7 / 2; 7 % 2
来源：http://eaw.jinghuilouyu.cn

Go:   7 / 2; 7 % 2
来源：http://emz.gzhubu.top

Ruby: 7 / 2; 7 % 2
来源：http://grl.zhaomingkeji.xyz

C#:   7 / 2; 7 % 2
来源：http://wpi.sxryk.cn

[A06] 字符串转数字
来源：http://oco.meibo888.top

Py:   int("42"); float("3.14")
来源：http://tke.daria6918.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vau.jinghuilouyu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xxd.jinqigfzy.top

TS:   parseInt("42", 10); Number("42")
来源：http://bfl.cdnleiting.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://njy.sufxvd.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ayd.svipenyu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rkm.bjfxy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pnl.jinqigufen.top

[A07] 数字转字符串
来源：http://akt.hfpthk.cn

Py:   str(42)
来源：http://gbh.ivvv.top

PHP:  (string) 42; strval(42)
来源：http://myk.pengpengdd.cyou

JS:   String(42); (42).toString()
来源：http://xry.fktsv.cn

TS:   String(42)
来源：http://kkm.9152youxi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://tdl.fehbvm.com

Go:   strconv.Itoa(42)
来源：http://vwn.316326.xyz

Ruby: 42.to_s
来源：http://wmn.chenlongwang.top

C#:   42.ToString()
来源：http://kgl.bbcook.cn

[A08] 取整与四舍五入
来源：http://owy.hywenlv.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pqb.hongshengwenyu.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vsj.yangfankeji.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://utl.xuanzx.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xut.yangfankeji.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kxj.hammf.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lvc.tanke756.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ncw.fanxiaobao.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://igu.zycfv.cn

[A09] 绝对值与最大最小值
来源：http://pwj.yueranfly.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vlb.sxryk.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mme.aibaodan.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qjv.hnxiangtu.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hnk.c1oappe.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dln.cucudq.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://akn.hesvh.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mrz.cdnleiting.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wwm.52xcode.cn

[A10] 生成随机数
来源：http://osb.sweek.top

Py:   import random; random.randint(1, 100)
来源：http://gui.ybcxt.top

PHP:  random_int(1, 100);
来源：http://jyf.jinqigfzy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xyh.ydjk.org.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://urx.xuanzx.com

Java: new Random().nextInt(100) + 1
来源：http://jgf.cheryme.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yjo.hongshengwenyu.top

Ruby: rand(1..100)
来源：http://tqo.daxiang520.top

C#:   new Random().Next(1, 101)
来源：http://zti.yuxming.cn

[A11] 条件表达式（三元）
来源：http://bcn.haohaochexian.top

Py:   "yes" if x > 0 else "no"
来源：http://rfg.iojbl.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qkh.yj202588.top

JS:   x > 0 ? "yes" : "no"
来源：http://bic.sjlbkw.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dfy.tanke756.top

Java: x > 0 ? "yes" : "no"
来源：http://jed.shuidangran.top

Go:   // 无三元运算符，需用 if 语句
来源：http://odu.jqgufenzy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://uiw.meibo888.top

C#:   x > 0 ? "yes" : "no"
来源：http://hno.ivvv.top

[A12] 字符串插值 / 格式化
来源：http://tgb.xylfe.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pbz.sxryk.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cik.nwbrower.top

JS:   `Hello, ${name}!`
来源：http://agu.zdbjq.cn

TS:   `Hello, ${name}!`
来源：http://tih.feifeiyinyue.top

Java: "Hello, %s!".formatted(name)
来源：http://xsu.yuanzhike.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hqd.zhaomingkeji.xyz

Ruby: "Hello, #{name}!"
来源：http://jtp.vqdsnc.cn

C#:   $"Hello, {name}!"
来源：http://yml.tianlin.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://lqg.sweek.top

Py:   "第一行\n第二行"
来源：http://gzv.yj202588.top

PHP:  "第一行\n第二行"
来源：http://pck.pengpengdd.cyou

JS:   "第一行\n第二行"
来源：http://jif.dianchejie.cn

TS:   "第一行\n第二行"
来源：http://ntp.xinyue.icu

Java: "第一行\n第二行"
来源：http://ozh.fzhhl.top

Go:   "第一行\n第二行"
来源：http://yrf.hesvh.cn

Ruby: "第一行\n第二行"
来源：http://qef.epnwcf.com

C#:   "第一行\n第二行"
来源：http://bpc.0kj1m.cn

[A14] 注释写法
来源：http://uds.shzxlz.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://nwl.316326.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://evd.fengsongda.top

JS:   // 单行；/* 多行 */
来源：http://bed.ppjwa.cn

TS:   // 单行；/* 多行 */
来源：http://lbc.shzxlz.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blg.uphjek.com

Go:   // 单行；/* 多行 */
来源：http://crn.ppjwa.cn

Ruby: # 单行；=begin 多行 =end
来源：http://gen.smart0.xyz

C#:   // 单行；/* 多行 */
来源：http://wcg.aizwys.cn

[A15] 空值判断与默认值
来源：http://tnm.316326.xyz

Py:   value = data or "默认值"
来源：http://yoc.svipenyu.cn

PHP:  $value = $data ?? "默认值";
来源：http://gpp.sufxvd.cn

JS:   const value = data ?? "默认值";
来源：http://phq.daria6918.cn

TS:   const value = data ?? "默认值";
来源：http://qqs.chenlongwang.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sld.wangshuangyany.cn

Go:   if data == "" { data = "默认值" }
来源：http://hmc.zhiwuduotai.top

Ruby: value = data || "默认值"
来源：http://for.xingfuxueyuan.xyz

C#:   var value = data ?? "默认值";
来源：http://bge.ydzc1.top

[A16] 真假值判断规则
来源：http://hal.ctjpmb.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://imq.ctjpmb.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sdx.xziqi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cnn.chenzaomai.com

TS:   if (!x) {}
来源：http://les.ivvv.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pxq.xuanzx.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tmq.svipenyu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://oyc.fanxiaobao.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vyn.birdmap.top

[A17] 位运算
来源：http://dyt.gaohongyu789.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oks.yj20258888.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cpm.sjlbkw.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wrz.hnxiangtu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mol.cqqwz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ltu.aibaodan.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://utb.nanxuanxn.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mev.yongpay.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kiw.hesvh.cn

[A18] 字符与 ASCII 码互转
来源：http://ptq.yvedp.cn

Py:   ord("A"); chr(65)
来源：http://ezl.hnqzz.top

PHP:  ord("A"); chr(65)
来源：http://tlm.xuanzx.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vyx.ydjk.org.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yps.wangshuangyany.cn

Java: (int) 'A'; (char) 65
来源：http://vyy.yangfankeji.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yxa.cdnleiting.top

Ruby: "A".ord; 65.chr
来源：http://kou.tianlin.xyz

C#:   (int)'A'; (char)65
来源：http://nsl.yj20258.top

[A19] 交换两个变量
来源：http://ugv.yangfankeji.com

Py:   a, b = b, a
来源：http://gwr.gaohongyu789.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ndi.iojbl.cn

JS:   [a, b] = [b, a];
来源：http://uga.ehwqpu.com

TS:   [a, b] = [b, a];
来源：http://qcg.zhijiandao.cn

Java: int t = a; a = b; b = t;
来源：http://fxr.uphjek.com

Go:   a, b = b, a
来源：http://aby.guowangkeji.top

Ruby: a, b = b, a
来源：http://pps.shanyushiyangtech.top

C#:   (a, b) = (b, a);
来源：http://all.zhongyouzk.top

[A20] 读取标准输入
来源：http://osv.guowangkeji.top

Py:   name = input("请输入：")
来源：http://olb.316326.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://umg.zhaomingkeji.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://epr.birdmap.top

TS:   // Node.js：readline 模块
来源：http://gde.ivvv.top

Java: new Scanner(System.in).nextLine()
来源：http://dal.aizwys.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://srp.pengpengdd.cyou

Ruby: gets.chomp
来源：http://ngx.gzhubu.top

C#:   Console.ReadLine();
来源：http://wya.wangshuangyany.cn

[A21] 保留指定小数位输出
来源：http://mme.xinyue.icu

Py:   f"{3.14159:.2f}"
来源：http://aie.sysykeji.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zmf.cqqwz.cn

JS:   (3.14159).toFixed(2)
来源：http://eba.daxiang520.top

TS:   (3.14159).toFixed(2)
来源：http://kyd.aizwys.cn

Java: String.format("%.2f", 3.14159)
来源：http://anx.nwbrower.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ssl.fzhhl.top

Ruby: format("%.2f", 3.14159)
来源：http://npp.yuxming.cn

C#:   3.14159.ToString("F2")
来源：http://qbk.ctjpmb.com

[A22] 获取字符串长度
来源：http://cua.yanxiufei.cn

Py:   len(s)
来源：http://sxg.hesvh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mgc.guannengcc.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dqz.yueranfly.top

TS:   s.length
来源：http://nlt.zhiwuduotai.top

Java: s.length()
来源：http://jzy.tianlin.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ouh.yonumen.top

Ruby: s.length
来源：http://gui.xziqi.cn

C#:   s.Length
来源：http://qrj.svipenyu.cn

[A23] 大小写转换
来源：http://zkv.9152youxi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nih.guannengcc.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ekj.fengsongda.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ibe.cucudq.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qjn.hnxiangtu.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vwt.zhixingplan.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vbv.cashguo.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sxd.chenlongwang.top

C#:   s.ToUpper(); s.ToLower()
来源：http://kxw.haohaochexian.top

[A24] 去除首尾空白
来源：http://zmh.hnqzz.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vjs.chenzaomai.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zva.ywan-chungtsiang.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hll.gaohongyu789.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yzm.vqdsnc.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gag.vqdsnc.cn

Go:   strings.TrimSpace(s)
来源：http://cjk.xylfe.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vrq.0kj1m.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vak.chenzaomai.com

[A25] 字符串比较
来源：http://cic.vehdjk.com

Py:   s1 == s2; s1 != s2
来源：http://emi.xinyue.icu

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://apb.cqqwz.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zcv.fktsv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tzn.hywenlv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oqs.zhiwuduotai.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hmr.pengpengdd.cyou

Ruby: s1 == s2; s1 <=> s2
来源：http://pyn.tarul.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xhc.52xcode.cn

[A26] 类型转换总览
来源：http://fis.bbcook.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ybi.cqqwz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kjl.hammf.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://iae.sjlbkw.cn

TS:   Number() String() Boolean() x as number
来源：http://mjr.cucudq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nph.yanxiufei.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vvx.xuetiantiany.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lbn.birdmap.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dvx.c1oappe.top

================================================================================
来源：http://aoq.xuetiantiany.cn

B. 流程控制
来源：http://hht.gzhubu.top

================================================================================
来源：http://ckx.bjfxy.top

[B01] 条件判断 if / else
来源：http://ile.hcnkem.com

Py:   result = "正" if x > 0 else "非正"
来源：http://vur.jianghu66.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://egc.yueranfly.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mhr.aibaodan.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bky.dashuyun.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uvf.pycfn.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qix.mhx1999.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hgi.gzhubu.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rxz.0kj1m.cn

[B02] 多分支 else if / elif
来源：http://vpg.guowangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qlb.guannengcc.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dha.fzhhl.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ach.tarul.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iyj.smart0.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lov.meibo888.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://srd.aibaodan.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ges.aizwys.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://agr.cucudq.cn

[B03] switch / match / case
来源：http://eob.iojbl.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tfs.feifeiyinyue.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nmb.havefunace.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://egh.pengpengdd.cyou

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oxa.sxryk.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ltq.yvedp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nda.dashuyun.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lzn.shanyushiyangkeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hfj.fzhhl.top

[B04] for 计数循环
来源：http://ymu.ctjpmb.com


<!-- 参考信息 -->