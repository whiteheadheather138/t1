代发 wailian999

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lnd.tian-w.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zlv.xziqi.cn

【文件统计】
来源：http://npv.jinghuilouyu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lpx.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://eud.ydzc1.top

目  录
来源：http://hsb.meibo888.top

--------------------------------------------------------------------------------
来源：http://axr.epnwcf.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fjx.tianlin.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zit.yueranfly.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fgp.daxiang520.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://flb.yueranfly.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ccs.tanke756.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ikb.yj20258.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fjn.redwolf501.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vte.nanxinkj.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jes.hnxiangtu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gkp.c1oappe.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://akx.zdbjq.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vvd.jinyuanbaomall.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rvi.c1oappe.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fht.zdqjudy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rzr.feifeiyinyue.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qiu.yongpay.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gkj.jqgfzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://cqz.gzhubu.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ivo.yangfankeji.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tsj.ydzc1.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dqv.vehdjk.com

================================================================================
来源：http://sge.sjlbkw.cn

A. 基础语法与类型
来源：http://nnk.hywenlv.cn

================================================================================
来源：http://mfc.xuanzx.com

[A01] Hello World
来源：http://mtf.yangfankeji.com

Py:   print("Hello, World!")
来源：http://lpj.vehdjk.com

PHP:  echo "Hello, World!";
来源：http://tpe.tarul.cn

JS:   console.log("Hello, World!");
来源：http://uca.pycfn.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xnd.jlsjyb.cn

Java: System.out.println("Hello, World!");
来源：http://thc.chenlongwang.top

Go:   fmt.Println("Hello, World!")
来源：http://joo.yuxming.cn

Ruby: puts "Hello, World!"
来源：http://yrc.fktsv.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://kwf.yueranfly.top

[A02] 变量声明与赋值
来源：http://hxn.ybcxt.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hfc.yanxiufei.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gwr.daria6918.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tlf.ydjk.org.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tcs.bjfxy.top

Java: String name = "Alex"; int age = 20;
来源：http://wzy.tarul.cn

Go:   name := "Alex"; age := 20
来源：http://xgd.andypj.xyz

Ruby: name = "Alex"; age = 20
来源：http://lel.yj20258888.top

C#:   string name = "Alex"; int age = 20;
来源：http://sqf.chenzaomai.com

[A03] 常量定义
来源：http://rmj.xziqi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tzm.xuetiantiany.cn

PHP:  const PI = 3.14159;
来源：http://gju.gzhubu.top

JS:   const PI = 3.14159;
来源：http://diq.sjlbkw.cn

TS:   const PI: number = 3.14159;
来源：http://bud.zhongyouzk.top

Java: static final double PI = 3.14159;
来源：http://tvd.cashguo.top

Go:   const PI = 3.14159
来源：http://gxh.wangdashe.top

Ruby: PI = 3.14159
来源：http://rxj.tianlin.xyz

C#:   const double PI = 3.14159;
来源：http://gfu.daria6918.cn

[A04] 判断变量类型
来源：http://fbi.aizwys.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wff.sufxvd.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kmd.yangfankeji.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pjw.yj20258888.top

TS:   typeof x; x instanceof Date
来源：http://bli.aibaodan.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mjh.iojbl.cn

Go:   reflect.TypeOf(x).Name()
来源：http://igc.birdmap.top

Ruby: x.class; x.is_a?(Integer)
来源：http://wed.yanxiufei.cn

C#:   x.GetType().Name; x is int
来源：http://yel.cashguo.top

[A05] 整数除法与取模
来源：http://usz.iojbl.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mhp.iojbl.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vzf.hammf.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ftu.yueranfly.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wje.xuetiantiany.cn

Java: 7 / 2; 7 % 2
来源：http://pap.ydjk.org.cn

Go:   7 / 2; 7 % 2
来源：http://hzw.316326.xyz

Ruby: 7 / 2; 7 % 2
来源：http://hjx.fehbvm.com

C#:   7 / 2; 7 % 2
来源：http://uup.yfazqb.com

[A06] 字符串转数字
来源：http://mgp.ivvv.top

Py:   int("42"); float("3.14")
来源：http://rfy.smart0.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ohd.wangshuangyany.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qfn.yuxming.cn

TS:   parseInt("42", 10); Number("42")
来源：http://uaj.fanxiaobao.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kjj.yuanzhike.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jsi.xuanzx.com

Ruby: "42".to_i; "3.14".to_f
来源：http://tjq.yvedp.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ctm.hammf.cn

[A07] 数字转字符串
来源：http://vah.fehbvm.com

Py:   str(42)
来源：http://zyj.hfpthk.cn

PHP:  (string) 42; strval(42)
来源：http://znn.sjlbkw.cn

JS:   String(42); (42).toString()
来源：http://xar.xingfuxueyuan.xyz

TS:   String(42)
来源：http://dfs.bbcook.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vkf.ivvv.top

Go:   strconv.Itoa(42)
来源：http://dxw.xylfe.cn

Ruby: 42.to_s
来源：http://nkk.ppjwa.cn

C#:   42.ToString()
来源：http://oam.ywan-chungtsiang.top

[A08] 取整与四舍五入
来源：http://czr.jinghuilouyu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hyc.aibaodan.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gyt.0kj1m.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rot.mhx1999.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hne.sufxvd.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ogc.tarul.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ixe.yvedp.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zen.cheryme.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://eij.ydzc1.top

[A09] 绝对值与最大最小值
来源：http://siq.ywan-chungtsiang.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wfp.52xcode.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nlw.feifeiyinyue.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nms.gotoacloud.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://acv.c1oappe.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ibx.fanxiaobao.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qzt.andypj.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mav.smart0.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pii.zhengqikj.top

[A10] 生成随机数
来源：http://kgs.hfpthk.cn

Py:   import random; random.randint(1, 100)
来源：http://uiq.uphjek.com

PHP:  random_int(1, 100);
来源：http://svr.jianghu66.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qma.andypj.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bsn.cdnleiting.top

Java: new Random().nextInt(100) + 1
来源：http://exl.hysaishi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kfz.shangyingyoupin.top

Ruby: rand(1..100)
来源：http://uee.yongpay.top

C#:   new Random().Next(1, 101)
来源：http://axv.snrcjt.cn

[A11] 条件表达式（三元）
来源：http://skl.cqqwz.cn

Py:   "yes" if x > 0 else "no"
来源：http://ljw.zdqjudy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://umm.zhongyouzk.top

JS:   x > 0 ? "yes" : "no"
来源：http://umv.jyoumei.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jdf.zhaomingkeji.xyz

Java: x > 0 ? "yes" : "no"
来源：http://vop.bjfxy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://kym.ydzc1.top

Ruby: x > 0 ? "yes" : "no"
来源：http://fjv.hysaishi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ela.jinghuilouyu.cn

[A12] 字符串插值 / 格式化
来源：http://utl.epnwcf.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kbw.redwolf501.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sio.chenjidiqi.icu

JS:   `Hello, ${name}!`
来源：http://osj.guowangkeji.top

TS:   `Hello, ${name}!`
来源：http://bgs.iojbl.cn

Java: "Hello, %s!".formatted(name)
来源：http://lrs.yanxiufei.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wyq.xuetiantiany.cn

Ruby: "Hello, #{name}!"
来源：http://ofh.tian-w.cn

C#:   $"Hello, {name}!"
来源：http://ecy.andypj.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://odx.jqgufenzy.top

Py:   "第一行\n第二行"
来源：http://izs.quarkkingdee.top

PHP:  "第一行\n第二行"
来源：http://att.zhijiandao.cn

JS:   "第一行\n第二行"
来源：http://lfw.haohaochexian.top

TS:   "第一行\n第二行"
来源：http://rha.pengpengdd.cyou

Java: "第一行\n第二行"
来源：http://hze.andypj.xyz

Go:   "第一行\n第二行"
来源：http://ovj.mhx1999.top

Ruby: "第一行\n第二行"
来源：http://dxb.ybcxt.top

C#:   "第一行\n第二行"
来源：http://hyt.jinyuanbaomall.cn

[A14] 注释写法
来源：http://vjp.ctjpmb.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://xsl.vqdsnc.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zfu.birdmap.top

JS:   // 单行；/* 多行 */
来源：http://qkq.52xcode.cn

TS:   // 单行；/* 多行 */
来源：http://czf.smart0.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tmc.tanke756.top

Go:   // 单行；/* 多行 */
来源：http://xbv.fktsv.cn

Ruby: # 单行；=begin 多行 =end
来源：http://gyt.c1oappe.top

C#:   // 单行；/* 多行 */
来源：http://txy.yongpay.top

[A15] 空值判断与默认值
来源：http://phw.ppjwa.cn

Py:   value = data or "默认值"
来源：http://dmt.kuanghao11.cn

PHP:  $value = $data ?? "默认值";
来源：http://etw.gotoacloud.top

JS:   const value = data ?? "默认值";
来源：http://qoj.nanxinkj.top

TS:   const value = data ?? "默认值";
来源：http://ruh.epnwcf.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ilr.yvedp.cn

Go:   if data == "" { data = "默认值" }
来源：http://sig.xuanzx.com

Ruby: value = data || "默认值"
来源：http://ntw.xylfe.cn

C#:   var value = data ?? "默认值";
来源：http://fxl.shuidangran.top

[A16] 真假值判断规则
来源：http://nem.cashguo.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://izd.chenlongwang.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gjy.ehwqpu.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wzs.ivvv.top

TS:   if (!x) {}
来源：http://vqt.wangdashe.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cjd.ydjk.org.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qql.jlsjyb.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ykc.cucudq.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bho.hnqzz.top

[A17] 位运算
来源：http://mql.jinqigfzy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uer.nwbrower.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fkm.yj20258888.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aqv.cqqwz.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cgl.svipenyu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fut.jyoumei.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yml.guowangkeji.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yli.dashuyun.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kyw.bbcook.cn

[A18] 字符与 ASCII 码互转
来源：http://hut.sufxvd.cn

Py:   ord("A"); chr(65)
来源：http://wul.hnqzz.top

PHP:  ord("A"); chr(65)
来源：http://vmu.zdqjudy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://spe.aibaodan.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gdt.9152youxi.cn

Java: (int) 'A'; (char) 65
来源：http://opa.zhixingplan.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hog.smart0.xyz

Ruby: "A".ord; 65.chr
来源：http://wnk.gaohongyu789.top

C#:   (int)'A'; (char)65
来源：http://pll.jyoumei.cn

[A19] 交换两个变量
来源：http://nqw.jyoumei.cn

Py:   a, b = b, a
来源：http://vor.yueranfly.top

PHP:  [$a, $b] = [$b, $a];
来源：http://izw.tian-w.cn

JS:   [a, b] = [b, a];
来源：http://gnh.xziqi.cn

TS:   [a, b] = [b, a];
来源：http://lcc.wangshuangyany.cn

Java: int t = a; a = b; b = t;
来源：http://stf.ybcxt.top

Go:   a, b = b, a
来源：http://myw.gotoacloud.top

Ruby: a, b = b, a
来源：http://cte.shangyingyoupin.top

C#:   (a, b) = (b, a);
来源：http://ynr.shanyushiyangkeji.top

[A20] 读取标准输入
来源：http://ydz.jyoumei.cn

Py:   name = input("请输入：")
来源：http://cnh.hongshengwenyu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://mmw.nanxinkj.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://urs.shanyushiyangtech.top

TS:   // Node.js：readline 模块
来源：http://oml.xuetiantiany.cn

Java: new Scanner(System.in).nextLine()
来源：http://rtp.yonumen.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hqk.cqqwz.cn

Ruby: gets.chomp
来源：http://hvq.haohaochexian.top

C#:   Console.ReadLine();
来源：http://brr.chenlongwang.top

[A21] 保留指定小数位输出
来源：http://dfg.cucudq.cn

Py:   f"{3.14159:.2f}"
来源：http://vok.pycfn.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xbc.hesvh.cn

JS:   (3.14159).toFixed(2)
来源：http://ygi.xuetiantiany.cn

TS:   (3.14159).toFixed(2)
来源：http://ovd.hywenlv.cn

Java: String.format("%.2f", 3.14159)
来源：http://ttb.mhx1999.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hwx.ydzc1.top

Ruby: format("%.2f", 3.14159)
来源：http://ieb.jyoumei.cn

C#:   3.14159.ToString("F2")
来源：http://yyk.hnxiangtu.top

[A22] 获取字符串长度
来源：http://xnn.ybcxt.top

Py:   len(s)
来源：http://mar.jinqigufen.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cfz.dashuyun.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hil.jinqigfzy.top

TS:   s.length
来源：http://lmd.dianchejie.cn

Java: s.length()
来源：http://ymu.snrcjt.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sxl.vqdsnc.cn

Ruby: s.length
来源：http://ejm.yueranfly.top

C#:   s.Length
来源：http://pka.9152youxi.cn

[A23] 大小写转换
来源：http://ziw.aibaodan.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ckm.xziqi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bjv.tanke756.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pcy.pycfn.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xxp.jlsjyb.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gxd.sweek.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nhl.cqqwz.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ddw.yvedp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://etb.xingfuxueyuan.xyz

[A24] 去除首尾空白
来源：http://uzn.zhijiandao.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://eyc.fzhhl.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://glp.jqgfzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oma.shanyushiyangkeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ler.shuidangran.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zft.yvedp.cn

Go:   strings.TrimSpace(s)
来源：http://diz.shuidangran.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://aue.cheryme.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zeo.quarkkingdee.top

[A25] 字符串比较
来源：http://rvg.smart0.xyz

Py:   s1 == s2; s1 != s2
来源：http://mza.xingfuxueyuan.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ekz.jinghuilouyu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xwy.yongpay.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ypo.jiagoushi.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bbb.tarul.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://exu.zhoulong.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://fpx.shzxlz.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://upz.snrcjt.cn

[A26] 类型转换总览
来源：http://dzz.pengpengdd.cyou

Py:   int() float() str() bool() list() dict() tuple()
来源：http://idy.shuidangran.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qky.tarul.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cde.pengpengdd.cyou

TS:   Number() String() Boolean() x as number
来源：http://vea.guowangkeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ule.ivvv.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ufc.9152youxi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://drv.hammf.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nkb.0kj1m.cn

================================================================================
来源：http://ijq.ehwqpu.com

B. 流程控制
来源：http://nrm.shanyushiyangtech.top

================================================================================
来源：http://tew.yj20258.top

[B01] 条件判断 if / else
来源：http://pem.cashguo.top

Py:   result = "正" if x > 0 else "非正"
来源：http://khu.hysaishi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ycb.tanke756.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gig.hysaishi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://acb.sxryk.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xjf.vehdjk.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ktk.tianlin.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rps.chenlongwang.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://npo.fehbvm.com

[B02] 多分支 else if / elif
来源：http://gxp.cdnleiting.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rxx.fengsongda.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dyd.yuxming.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ekr.nanxinkj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lns.yuanzhike.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ash.fzhhl.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yzw.wangdashe.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eik.cqqwz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lvs.316326.xyz

[B03] switch / match / case
来源：http://nqd.xinyue.icu

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xrv.fehbvm.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dkw.52xcode.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hwq.shanyushiyangkeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://piz.zhoulong.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://otc.hongshengwenyu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rjr.hnxiangtu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qpa.hcnkem.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mhm.jqgufenzy.top

[B04] for 计数循环
来源：http://lgx.sysykeji.top

Py:   for i in range(10): print(i)
来源：http://hcg.dashuyun.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cui.cdnleiting.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bao.52xcode.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rxk.ydjk.org.cn


<!-- 参考信息 -->