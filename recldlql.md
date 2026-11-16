代发 wailian999

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bxy.yuxming.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://uws.daria6918.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://til.fanxiaobao.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rgp.nwbrower.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fpy.ywan-chungtsiang.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lpx.cdnleiting.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ldk.zhaomingkeji.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kmp.shzxlz.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bwc.jinghuilouyu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vlr.yj202588.top

【文件统计】
来源：http://hhh.zhiwuduotai.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://oet.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://hbw.aizwys.cn

目  录
来源：http://gjk.fengsongda.top

--------------------------------------------------------------------------------
来源：http://fpy.feifeiyinyue.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jno.fanxiaobao.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sbt.sxryk.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nun.yonumen.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://spi.nanxinkj.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wba.ywan-chungtsiang.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hwq.yj20258.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uuw.xingfuxueyuan.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baa.zdqjudy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zbl.pengpengdd.cyou

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lgo.tianlin.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dyk.aizwys.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://htz.yvedp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hst.epnwcf.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ogd.ydzc1.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ikz.0kj1m.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://osg.jinqigfzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ytq.fengsongda.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ibx.gogol.net.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://quk.yvedp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yue.chenlongwang.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kdi.52xcode.cn

================================================================================
来源：http://zqx.jlsjyb.cn

A. 基础语法与类型
来源：http://unj.jinyuanbaomall.cn

================================================================================
来源：http://muu.pengpengdd.cyou

[A01] Hello World
来源：http://xgf.bbcook.cn

Py:   print("Hello, World!")
来源：http://gjz.zhoulong.xyz

PHP:  echo "Hello, World!";
来源：http://lka.xingfuxueyuan.xyz

JS:   console.log("Hello, World!");
来源：http://syc.yanxiufei.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zad.tian-w.cn

Java: System.out.println("Hello, World!");
来源：http://jkr.svipenyu.cn

Go:   fmt.Println("Hello, World!")
来源：http://ngu.ivvv.top

Ruby: puts "Hello, World!"
来源：http://cww.pycfn.com

C#:   Console.WriteLine("Hello, World!");
来源：http://eml.zdqjudy.top

[A02] 变量声明与赋值
来源：http://ksn.yvedp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://unk.svipenyu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hyh.xinyue.icu

JS:   let name = "Alex"; const age = 20;
来源：http://njg.sweek.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ujt.gogol.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://qnn.nwbrower.top

Go:   name := "Alex"; age := 20
来源：http://vra.yj20258888.top

Ruby: name = "Alex"; age = 20
来源：http://jud.fzhhl.top

C#:   string name = "Alex"; int age = 20;
来源：http://yqk.sysykeji.top

[A03] 常量定义
来源：http://jub.havefunace.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rns.tarul.cn

PHP:  const PI = 3.14159;
来源：http://mcw.hammf.cn

JS:   const PI = 3.14159;
来源：http://wyh.yongpay.top

TS:   const PI: number = 3.14159;
来源：http://akl.sxryk.cn

Java: static final double PI = 3.14159;
来源：http://xfx.sweek.top

Go:   const PI = 3.14159
来源：http://edd.cheryme.top

Ruby: PI = 3.14159
来源：http://yjl.hfpthk.cn

C#:   const double PI = 3.14159;
来源：http://zqx.iojbl.cn

[A04] 判断变量类型
来源：http://ltf.sufxvd.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rqb.tanke756.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hma.aizwys.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gwi.ppjwa.cn

TS:   typeof x; x instanceof Date
来源：http://byv.hysaishi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zax.shanyushiyangkeji.top

Go:   reflect.TypeOf(x).Name()
来源：http://nui.tanke756.top

Ruby: x.class; x.is_a?(Integer)
来源：http://wwy.jinqigfzy.top

C#:   x.GetType().Name; x is int
来源：http://wuo.mhx1999.top

[A05] 整数除法与取模
来源：http://zni.ppjwa.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://koe.pengpengdd.cyou

PHP:  intdiv(7, 2); 7 % 2
来源：http://vwe.zdqjudy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fsm.aibaodan.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yys.sxryk.cn

Java: 7 / 2; 7 % 2
来源：http://gns.cashguo.top

Go:   7 / 2; 7 % 2
来源：http://ovm.andypj.xyz

Ruby: 7 / 2; 7 % 2
来源：http://nar.hfpthk.cn

C#:   7 / 2; 7 % 2
来源：http://efp.daria6918.cn

[A06] 字符串转数字
来源：http://qpx.yj20258.top

Py:   int("42"); float("3.14")
来源：http://yxt.ydzc1.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lgt.sweek.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ddr.zhiwuduotai.top

TS:   parseInt("42", 10); Number("42")
来源：http://lri.zhixingplan.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ozi.tarul.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nxs.0kj1m.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://tux.jinghuilouyu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dnj.cashguo.top

[A07] 数字转字符串
来源：http://wxy.birdmap.top

Py:   str(42)
来源：http://bgs.sjlbkw.cn

PHP:  (string) 42; strval(42)
来源：http://ges.xuanzx.com

JS:   String(42); (42).toString()
来源：http://zmg.epnwcf.com

TS:   String(42)
来源：http://pll.ywan-chungtsiang.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://lhw.xuetiantiany.cn

Go:   strconv.Itoa(42)
来源：http://rnv.shzxlz.cn

Ruby: 42.to_s
来源：http://amm.chenlongwang.top

C#:   42.ToString()
来源：http://eot.shangyingyoupin.top

[A08] 取整与四舍五入
来源：http://cng.fanxiaobao.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fza.yfazqb.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wgc.nwbrower.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xah.bbcook.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qlv.zhiwuduotai.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kgv.xinyue.icu

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tjh.ydjk.org.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lhp.vehdjk.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://nji.meibo888.top

[A09] 绝对值与最大最小值
来源：http://kvo.quarkkingdee.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ick.yongpay.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yeb.daxiang520.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sum.0kj1m.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://adb.vqdsnc.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://opo.zhiwuduotai.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qyd.tian-w.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://heq.yuanzhike.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tgw.shanyushiyangkeji.top

[A10] 生成随机数
来源：http://tby.gogol.net.cn

Py:   import random; random.randint(1, 100)
来源：http://bjg.nanxinkj.top

PHP:  random_int(1, 100);
来源：http://ghz.iojbl.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ojc.hesvh.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zoc.fengsongda.top

Java: new Random().nextInt(100) + 1
来源：http://wdd.shuidangran.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fon.shanyushiyangkeji.top

Ruby: rand(1..100)
来源：http://znj.hongshengwenyu.top

C#:   new Random().Next(1, 101)
来源：http://dbu.fengsongda.top

[A11] 条件表达式（三元）
来源：http://rgp.yuanzhike.top

Py:   "yes" if x > 0 else "no"
来源：http://gyq.jiagoushi.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ick.fehbvm.com

JS:   x > 0 ? "yes" : "no"
来源：http://yvc.yangfankeji.com

TS:   x > 0 ? "yes" : "no"
来源：http://grv.zdqjudy.top

Java: x > 0 ? "yes" : "no"
来源：http://rqi.daxiang520.top

Go:   // 无三元运算符，需用 if 语句
来源：http://nza.jyoumei.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ghl.ybcxt.top

C#:   x > 0 ? "yes" : "no"
来源：http://tdp.xinyue.icu

[A12] 字符串插值 / 格式化
来源：http://ryv.sufxvd.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://iaz.wangdashe.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ypn.yj20258.top

JS:   `Hello, ${name}!`
来源：http://lju.pengpengdd.cyou

TS:   `Hello, ${name}!`
来源：http://rad.shangyingyoupin.top

Java: "Hello, %s!".formatted(name)
来源：http://gfn.vehdjk.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://omn.yangfankeji.com

Ruby: "Hello, #{name}!"
来源：http://fia.uphjek.com

C#:   $"Hello, {name}!"
来源：http://llr.yj20258888.top

[A13] 多行字符串（练习 \n 转义）
来源：http://jah.chenzaomai.com

Py:   "第一行\n第二行"
来源：http://npl.hnqzz.top

PHP:  "第一行\n第二行"
来源：http://kmy.gotoacloud.top

JS:   "第一行\n第二行"
来源：http://gxa.cashguo.top

TS:   "第一行\n第二行"
来源：http://siz.redwolf501.top

Java: "第一行\n第二行"
来源：http://pbz.kuanghao11.cn

Go:   "第一行\n第二行"
来源：http://lne.xuanzx.com

Ruby: "第一行\n第二行"
来源：http://uus.hysaishi.cn

C#:   "第一行\n第二行"
来源：http://fyj.zhengqikj.top

[A14] 注释写法
来源：http://cvx.zhoulong.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://ktm.ivvv.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://jmj.iojbl.cn

JS:   // 单行；/* 多行 */
来源：http://fyw.smart0.xyz

TS:   // 单行；/* 多行 */
来源：http://hcv.fengsongda.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sby.jyoumei.cn

Go:   // 单行；/* 多行 */
来源：http://moc.zhaomingkeji.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://kuo.ywan-chungtsiang.top

C#:   // 单行；/* 多行 */
来源：http://zqm.haohaochexian.top

[A15] 空值判断与默认值
来源：http://muo.nwbrower.top

Py:   value = data or "默认值"
来源：http://bzg.gotoacloud.top

PHP:  $value = $data ?? "默认值";
来源：http://ypi.meibo888.top

JS:   const value = data ?? "默认值";
来源：http://kga.gzhubu.top

TS:   const value = data ?? "默认值";
来源：http://khs.cqqwz.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://axp.wangshuangyany.cn

Go:   if data == "" { data = "默认值" }
来源：http://hkg.xuanzx.com

Ruby: value = data || "默认值"
来源：http://sva.sysykeji.top

C#:   var value = data ?? "默认值";
来源：http://fhg.dianchejie.cn

[A16] 真假值判断规则
来源：http://fuf.bbcook.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://crp.feifeiyinyue.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hcy.meibo888.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pfn.0kj1m.cn

TS:   if (!x) {}
来源：http://std.xuetiantiany.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vvr.cqqwz.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xna.nanxinkj.top

Ruby: unless x            # nil 与 false 为假
来源：http://mjg.zhaomingkeji.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://iqt.shanyushiyangkeji.top

[A17] 位运算
来源：http://tvf.zycfv.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qee.jinqigfzy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xnc.yuanzhike.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mxf.ehwqpu.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pkh.shuidangran.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bfl.fzhhl.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lvc.yj202588.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gdg.jqgufenzy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ngp.cheryme.top

[A18] 字符与 ASCII 码互转
来源：http://ymt.shzxlz.cn

Py:   ord("A"); chr(65)
来源：http://jca.chenlongwang.top

PHP:  ord("A"); chr(65)
来源：http://ynd.9152youxi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gvc.cashguo.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vjw.jianghu66.top

Java: (int) 'A'; (char) 65
来源：http://fwj.dianchejie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cje.chenzaomai.com

Ruby: "A".ord; 65.chr
来源：http://aja.dashuyun.cn

C#:   (int)'A'; (char)65
来源：http://wdg.nanxuanxn.top

[A19] 交换两个变量
来源：http://chq.cqqwz.cn

Py:   a, b = b, a
来源：http://thj.sufxvd.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://dvk.9152youxi.cn

JS:   [a, b] = [b, a];
来源：http://elv.guowangkeji.top

TS:   [a, b] = [b, a];
来源：http://krg.yueranfly.top

Java: int t = a; a = b; b = t;
来源：http://ght.fengsongda.top

Go:   a, b = b, a
来源：http://otr.guowangkeji.top

Ruby: a, b = b, a
来源：http://ryn.cdnleiting.top

C#:   (a, b) = (b, a);
来源：http://qbi.c1oappe.top

[A20] 读取标准输入
来源：http://lkv.shzxlz.cn

Py:   name = input("请输入：")
来源：http://iif.hesvh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://sqt.epnwcf.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bdn.xuanzx.com

TS:   // Node.js：readline 模块
来源：http://uqz.zhengqikj.top

Java: new Scanner(System.in).nextLine()
来源：http://yym.fktsv.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lte.yj20258.top

Ruby: gets.chomp
来源：http://gqm.gotoacloud.top

C#:   Console.ReadLine();
来源：http://dwt.jinqigfzy.top

[A21] 保留指定小数位输出
来源：http://kpn.jyoumei.cn

Py:   f"{3.14159:.2f}"
来源：http://tvc.yj202588.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hyc.guowangkeji.top

JS:   (3.14159).toFixed(2)
来源：http://bku.jianghu66.top

TS:   (3.14159).toFixed(2)
来源：http://dre.xingfuxueyuan.xyz

Java: String.format("%.2f", 3.14159)
来源：http://nej.epnwcf.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vwt.fehbvm.com

Ruby: format("%.2f", 3.14159)
来源：http://oaz.zhaomingkeji.xyz

C#:   3.14159.ToString("F2")
来源：http://heu.sjlbkw.cn

[A22] 获取字符串长度
来源：http://ztt.fzhhl.top

Py:   len(s)
来源：http://dkn.ivvv.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zud.zhaomingkeji.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xvy.jinyuanbaomall.cn

TS:   s.length
来源：http://nir.kuanghao11.cn

Java: s.length()
来源：http://rgf.jiagoushi.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ncp.snrcjt.cn

Ruby: s.length
来源：http://kyw.yuanzhike.top

C#:   s.Length
来源：http://zdv.dianchejie.cn

[A23] 大小写转换
来源：http://deb.hcnkem.com

Py:   s.upper(); s.lower(); s.title()
来源：http://qmy.ydzc1.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fkx.yangfankeji.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zto.9152youxi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ape.wangshuangyany.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ztk.nanxinkj.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xzt.jlsjyb.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cos.shangyingyoupin.top

C#:   s.ToUpper(); s.ToLower()
来源：http://sue.fanxiaobao.xyz

[A24] 去除首尾空白
来源：http://ren.chenjidiqi.icu

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kbc.ppjwa.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jlo.jqgufenzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lqe.zhongyouzk.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nck.zhongyouzk.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nal.xziqi.cn

Go:   strings.TrimSpace(s)
来源：http://zra.tarul.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ecc.jyoumei.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nql.havefunace.top

[A25] 字符串比较
来源：http://try.chenzaomai.com

Py:   s1 == s2; s1 != s2
来源：http://pkz.ppjwa.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oeu.smart0.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rho.hfpthk.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mip.yangfankeji.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zup.kuanghao11.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wst.hnqzz.top

Ruby: s1 == s2; s1 <=> s2
来源：http://bam.vehdjk.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jkc.ybcxt.top

[A26] 类型转换总览
来源：http://sst.birdmap.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hwv.snrcjt.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://exw.tarul.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qgi.yuxming.cn

TS:   Number() String() Boolean() x as number
来源：http://txg.zhixingplan.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rdm.tanke756.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tyn.pengpengdd.cyou

Ruby: to_i to_f to_s to_sym to_a
来源：http://xfd.dashuyun.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://few.wangdashe.top

================================================================================
来源：http://cjb.zhaomingkeji.xyz

B. 流程控制
来源：http://yki.hysaishi.cn

================================================================================
来源：http://fan.fanxiaobao.xyz

[B01] 条件判断 if / else
来源：http://zdk.zdbjq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vyx.shzxlz.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zaj.shangyingyoupin.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bvh.uphjek.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kgb.mhx1999.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ees.cucudq.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yph.zhengqikj.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pzj.ctjpmb.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rhg.fengsongda.top

[B02] 多分支 else if / elif
来源：http://qgc.yuxming.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yed.hfpthk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cpg.epnwcf.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://brh.hysaishi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mvf.aibaodan.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hpa.yj20258888.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rfn.yfazqb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qgy.hnxiangtu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vyl.jinghuilouyu.cn

[B03] switch / match / case
来源：http://sig.hnxiangtu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://htw.ivvv.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ozc.sjlbkw.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bqh.yangfankeji.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qyl.hcnkem.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uof.kuanghao11.cn


<!-- 参考信息 -->