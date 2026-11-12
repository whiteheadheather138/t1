代发 wailian999

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ksk.9152youxi.cn

【使用说明】
来源：http://bur.nwbrower.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nru.gzhubu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dbh.zycfv.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yyf.zdbjq.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lvd.xinyue.icu

Bash:  Shell         C:     C             C++:   C++
来源：http://qlh.ppjwa.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kbj.gotoacloud.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://moc.jinyuanbaomall.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mmk.gotoacloud.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bzo.hesvh.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pbn.hywenlv.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xfa.ehwqpu.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://iap.cqqwz.cn

【文件统计】
来源：http://rzl.yangfankeji.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cfj.yfazqb.com

--------------------------------------------------------------------------------
来源：http://mfz.yueranfly.top

目  录
来源：http://yab.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://fhk.yongpay.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fbi.xylfe.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jdd.yj202588.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dxp.kuanghao11.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uuv.hcnkem.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qgw.epnwcf.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qik.vqdsnc.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gsz.zhengqikj.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xsm.yj20258.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dre.nanxuanxn.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yio.yfazqb.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ysl.hnxiangtu.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zbz.wangdashe.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://udg.gaohongyu789.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ezr.ehwqpu.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://him.shangyingyoupin.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zvo.hcnkem.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vor.zhengqikj.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ilf.vehdjk.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wed.hywenlv.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fqc.xingfuxueyuan.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zhj.daria6918.cn

================================================================================
来源：http://pnl.birdmap.top

A. 基础语法与类型
来源：http://dwx.yueranfly.top

================================================================================
来源：http://mrl.hongshengwenyu.top

[A01] Hello World
来源：http://ehm.zhaomingkeji.xyz

Py:   print("Hello, World!")
来源：http://mnf.yj202588.top

PHP:  echo "Hello, World!";
来源：http://car.aizwys.cn

JS:   console.log("Hello, World!");
来源：http://bxe.dashuyun.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hoa.hesvh.cn

Java: System.out.println("Hello, World!");
来源：http://tbi.shanyushiyangkeji.top

Go:   fmt.Println("Hello, World!")
来源：http://csi.c1oappe.top

Ruby: puts "Hello, World!"
来源：http://ddl.iojbl.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://twz.nanxuanxn.top

[A02] 变量声明与赋值
来源：http://lfk.nanxinkj.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rbi.ctjpmb.com

PHP:  $name = "Alex"; $age = 20;
来源：http://ehl.shangyingyoupin.top

JS:   let name = "Alex"; const age = 20;
来源：http://wco.nanxinkj.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dyv.iojbl.cn

Java: String name = "Alex"; int age = 20;
来源：http://qwu.hfpthk.cn

Go:   name := "Alex"; age := 20
来源：http://iis.meibo888.top

Ruby: name = "Alex"; age = 20
来源：http://ngj.dashuyun.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yvh.smart0.xyz

[A03] 常量定义
来源：http://cqf.zhoulong.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pnp.hfpthk.cn

PHP:  const PI = 3.14159;
来源：http://ebi.dashuyun.cn

JS:   const PI = 3.14159;
来源：http://hgj.yfazqb.com

TS:   const PI: number = 3.14159;
来源：http://jvm.hnxiangtu.top

Java: static final double PI = 3.14159;
来源：http://osh.quarkkingdee.top

Go:   const PI = 3.14159
来源：http://yhk.hongshengwenyu.top

Ruby: PI = 3.14159
来源：http://vir.cashguo.top

C#:   const double PI = 3.14159;
来源：http://qzj.zycfv.cn

[A04] 判断变量类型
来源：http://ryt.quarkkingdee.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://zkp.jlsjyb.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rmo.yangfankeji.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gwu.shzxlz.cn

TS:   typeof x; x instanceof Date
来源：http://qrz.gzhubu.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ooa.jinyuanbaomall.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vgp.smart0.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://zzw.sxryk.cn

C#:   x.GetType().Name; x is int
来源：http://ush.yuanzhike.top

[A05] 整数除法与取模
来源：http://lnx.sjlbkw.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xxk.guannengcc.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://kke.hesvh.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nhx.vqdsnc.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rab.fehbvm.com

Java: 7 / 2; 7 % 2
来源：http://cwj.yangfankeji.com

Go:   7 / 2; 7 % 2
来源：http://pzx.yangfankeji.com

Ruby: 7 / 2; 7 % 2
来源：http://zfl.yuanzhike.top

C#:   7 / 2; 7 % 2
来源：http://poy.gogol.net.cn

[A06] 字符串转数字
来源：http://mtj.dianchejie.cn

Py:   int("42"); float("3.14")
来源：http://ebm.hnqzz.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xsa.hammf.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fyi.hammf.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ymx.xinyue.icu

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dyo.jqgufenzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://frp.hywenlv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://cnw.daxiang520.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qbg.tian-w.cn

[A07] 数字转字符串
来源：http://fym.hammf.cn

Py:   str(42)
来源：http://blr.hammf.cn

PHP:  (string) 42; strval(42)
来源：http://jsa.pengpengdd.cyou

JS:   String(42); (42).toString()
来源：http://byf.yueranfly.top

TS:   String(42)
来源：http://oth.xinyue.icu

Java: String.valueOf(42); Integer.toString(42)
来源：http://nib.shanyushiyangtech.top

Go:   strconv.Itoa(42)
来源：http://trc.hywenlv.cn

Ruby: 42.to_s
来源：http://cwi.jqgfzy.top

C#:   42.ToString()
来源：http://wfs.jinyuanbaomall.cn

[A08] 取整与四舍五入
来源：http://rez.wangdashe.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lzf.xuetiantiany.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rfg.ivvv.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ngs.jiagoushi.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zab.0kj1m.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pbb.hesvh.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://giv.redwolf501.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://lfv.snrcjt.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hxj.kuanghao11.cn

[A09] 绝对值与最大最小值
来源：http://umi.yj20258.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fzy.ywan-chungtsiang.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fls.yueranfly.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ies.shuidangran.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wlc.ehwqpu.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nfe.zhixingplan.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://swx.birdmap.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ifc.fktsv.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tvf.epnwcf.com

[A10] 生成随机数
来源：http://eax.xylfe.cn

Py:   import random; random.randint(1, 100)
来源：http://clw.xuetiantiany.cn

PHP:  random_int(1, 100);
来源：http://uhw.dianchejie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wdb.xuetiantiany.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ybz.tianlin.xyz

Java: new Random().nextInt(100) + 1
来源：http://bee.c1oappe.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vcx.cdnleiting.top

Ruby: rand(1..100)
来源：http://jse.chenlongwang.top

C#:   new Random().Next(1, 101)
来源：http://lcj.zhongyouzk.top

[A11] 条件表达式（三元）
来源：http://ebr.ydzc1.top

Py:   "yes" if x > 0 else "no"
来源：http://ftu.guowangkeji.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://hpo.jinyuanbaomall.cn

JS:   x > 0 ? "yes" : "no"
来源：http://mju.zhongyouzk.top

TS:   x > 0 ? "yes" : "no"
来源：http://fkj.sufxvd.cn

Java: x > 0 ? "yes" : "no"
来源：http://qig.cdnleiting.top

Go:   // 无三元运算符，需用 if 语句
来源：http://fkz.smart0.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://vxa.gzhubu.top

C#:   x > 0 ? "yes" : "no"
来源：http://tbq.ehwqpu.com

[A12] 字符串插值 / 格式化
来源：http://mak.jinqigufen.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pja.snrcjt.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vki.pycfn.com

JS:   `Hello, ${name}!`
来源：http://qdo.jianghu66.top

TS:   `Hello, ${name}!`
来源：http://eix.9152youxi.cn

Java: "Hello, %s!".formatted(name)
来源：http://iiv.nanxuanxn.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zdq.yongpay.top

Ruby: "Hello, #{name}!"
来源：http://buj.cucudq.cn

C#:   $"Hello, {name}!"
来源：http://zga.tian-w.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xgw.shangyingyoupin.top

Py:   "第一行\n第二行"
来源：http://fju.wangdashe.top

PHP:  "第一行\n第二行"
来源：http://leu.hnqzz.top

JS:   "第一行\n第二行"
来源：http://cdn.jinghuilouyu.cn

TS:   "第一行\n第二行"
来源：http://ecy.ywan-chungtsiang.top

Java: "第一行\n第二行"
来源：http://rzq.shanyushiyangkeji.top

Go:   "第一行\n第二行"
来源：http://zob.yfazqb.com

Ruby: "第一行\n第二行"
来源：http://lyg.ppjwa.cn

C#:   "第一行\n第二行"
来源：http://scv.kuanghao11.cn

[A14] 注释写法
来源：http://imv.fehbvm.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://olc.zhoulong.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://mnk.meibo888.top

JS:   // 单行；/* 多行 */
来源：http://zmo.cheryme.top

TS:   // 单行；/* 多行 */
来源：http://ugc.zdbjq.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qmf.nanxinkj.top

Go:   // 单行；/* 多行 */
来源：http://jwn.bjfxy.top

Ruby: # 单行；=begin 多行 =end
来源：http://deb.smart0.xyz

C#:   // 单行；/* 多行 */
来源：http://bka.jyoumei.cn

[A15] 空值判断与默认值
来源：http://inh.kuanghao11.cn

Py:   value = data or "默认值"
来源：http://kvx.snrcjt.cn

PHP:  $value = $data ?? "默认值";
来源：http://kla.yj20258888.top

JS:   const value = data ?? "默认值";
来源：http://cso.guowangkeji.top

TS:   const value = data ?? "默认值";
来源：http://asf.sweek.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rnp.andypj.xyz

Go:   if data == "" { data = "默认值" }
来源：http://sgo.aibaodan.cn

Ruby: value = data || "默认值"
来源：http://psv.yuxming.cn

C#:   var value = data ?? "默认值";
来源：http://ypn.cheryme.top

[A16] 真假值判断规则
来源：http://ghg.xziqi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sme.yongpay.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ufo.cqqwz.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ywq.dashuyun.cn

TS:   if (!x) {}
来源：http://yrw.yuanzhike.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wop.wangshuangyany.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vfe.aizwys.cn

Ruby: unless x            # nil 与 false 为假
来源：http://iyx.smart0.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dja.gaohongyu789.top

[A17] 位运算
来源：http://ldl.zhijiandao.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rhj.yj202588.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ypy.wangshuangyany.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gqj.ehwqpu.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pqf.jinyuanbaomall.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dqy.pengpengdd.cyou

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xbn.wangshuangyany.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ibz.zhengqikj.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vzx.zdbjq.cn

[A18] 字符与 ASCII 码互转
来源：http://och.cdnleiting.top

Py:   ord("A"); chr(65)
来源：http://kqj.cashguo.top

PHP:  ord("A"); chr(65)
来源：http://dsc.yonumen.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tzc.xuetiantiany.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://swb.ybcxt.top

Java: (int) 'A'; (char) 65
来源：http://cnf.ydjk.org.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://olc.vehdjk.com

Ruby: "A".ord; 65.chr
来源：http://igd.pycfn.com

C#:   (int)'A'; (char)65
来源：http://nfz.nanxuanxn.top

[A19] 交换两个变量
来源：http://jzi.bjfxy.top

Py:   a, b = b, a
来源：http://nxj.hywenlv.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nrl.fktsv.cn

JS:   [a, b] = [b, a];
来源：http://gka.cheryme.top

TS:   [a, b] = [b, a];
来源：http://jqu.hongshengwenyu.top

Java: int t = a; a = b; b = t;
来源：http://ttz.nwbrower.top

Go:   a, b = b, a
来源：http://vll.zhiwuduotai.top

Ruby: a, b = b, a
来源：http://vea.sjlbkw.cn

C#:   (a, b) = (b, a);
来源：http://pdb.sufxvd.cn

[A20] 读取标准输入
来源：http://bqk.yj202588.top

Py:   name = input("请输入：")
来源：http://xkc.0kj1m.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://wxs.epnwcf.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://slt.9152youxi.cn

TS:   // Node.js：readline 模块
来源：http://hoz.fzhhl.top

Java: new Scanner(System.in).nextLine()
来源：http://lcu.jianghu66.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qqg.daria6918.cn

Ruby: gets.chomp
来源：http://pks.ydzc1.top

C#:   Console.ReadLine();
来源：http://jbn.jinyuanbaomall.cn

[A21] 保留指定小数位输出
来源：http://xuu.fengsongda.top

Py:   f"{3.14159:.2f}"
来源：http://jho.yonumen.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://unv.andypj.xyz

JS:   (3.14159).toFixed(2)
来源：http://qbh.tianlin.xyz

TS:   (3.14159).toFixed(2)
来源：http://uns.ydzc1.top

Java: String.format("%.2f", 3.14159)
来源：http://emc.shanyushiyangkeji.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sha.9152youxi.cn

Ruby: format("%.2f", 3.14159)
来源：http://trw.vqdsnc.cn

C#:   3.14159.ToString("F2")
来源：http://xqn.zhoulong.xyz

[A22] 获取字符串长度
来源：http://org.jqgfzy.top

Py:   len(s)
来源：http://use.wangshuangyany.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vnf.shangyingyoupin.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jkl.hfpthk.cn

TS:   s.length
来源：http://ybz.xziqi.cn

Java: s.length()
来源：http://hxz.xuanzx.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kdx.ydjk.org.cn

Ruby: s.length
来源：http://jrp.yj20258.top

C#:   s.Length
来源：http://fmr.zdqjudy.top

[A23] 大小写转换
来源：http://hxf.chenlongwang.top

Py:   s.upper(); s.lower(); s.title()
来源：http://lza.redwolf501.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tao.zhaomingkeji.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pkz.hongshengwenyu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dgg.sxryk.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fed.sjlbkw.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mlg.wangshuangyany.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fff.tian-w.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://odt.dashuyun.cn

[A24] 去除首尾空白
来源：http://esu.sufxvd.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://has.zhoulong.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mpv.ehwqpu.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://apm.nwbrower.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yhg.birdmap.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yqw.redwolf501.top

Go:   strings.TrimSpace(s)
来源：http://gcc.hysaishi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pny.zhixingplan.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nso.hammf.cn

[A25] 字符串比较
来源：http://wha.zhaomingkeji.xyz

Py:   s1 == s2; s1 != s2
来源：http://bmq.yj20258888.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://koz.ywan-chungtsiang.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ese.hesvh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://oyo.tanke756.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pmn.yueranfly.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dxf.daxiang520.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ivn.sufxvd.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lsc.gzhubu.top

[A26] 类型转换总览
来源：http://ptu.ybcxt.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mnl.shanyushiyangkeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://anb.jinghuilouyu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://enf.gogol.net.cn

TS:   Number() String() Boolean() x as number
来源：http://aad.chenzaomai.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sxf.yj20258888.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cbh.yongpay.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://bul.xuetiantiany.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zyd.jinyuanbaomall.cn

================================================================================
来源：http://inb.fanxiaobao.xyz

B. 流程控制
来源：http://zja.zhoulong.xyz

================================================================================
来源：http://smn.yj20258888.top

[B01] 条件判断 if / else
来源：http://chg.sysykeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://vdk.ppjwa.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uxt.haohaochexian.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ovc.shuidangran.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://whr.fanxiaobao.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://ehf.jinyuanbaomall.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qrl.epnwcf.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dzn.tarul.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://czb.tarul.cn

[B02] 多分支 else if / elif
来源：http://kqo.yvedp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nua.sxryk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kct.yanxiufei.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://irw.0kj1m.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dfp.fehbvm.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://llg.jinghuilouyu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xqj.xuetiantiany.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ken.xingfuxueyuan.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eau.cdnleiting.top

[B03] switch / match / case
来源：http://xbn.jinqigufen.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qki.shanyushiyangkeji.top


<!-- 参考信息 -->