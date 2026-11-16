代发 wailian999

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ath.aibaodan.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fmj.uphjek.com

Bash:  Shell         C:     C             C++:   C++
来源：http://uct.hywenlv.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://znc.nanxinkj.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cct.zhiwuduotai.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hvh.xziqi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cxz.iojbl.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tgj.guannengcc.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mqn.zycfv.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rrt.zhiwuduotai.top

【文件统计】
来源：http://ear.quarkkingdee.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://iwd.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://dxk.birdmap.top

目  录
来源：http://bsc.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://dga.cheryme.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wep.nanxuanxn.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lqp.zhijiandao.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://soe.fktsv.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://twt.sxryk.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ntx.jiagoushi.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kcx.c1oappe.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://frr.zhiwuduotai.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nbj.nanxuanxn.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lst.epnwcf.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mqk.yangfankeji.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qye.zhongyouzk.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nja.yuxming.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pvh.aizwys.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mwz.ydjk.org.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dqg.sjlbkw.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lau.yonumen.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vqr.snrcjt.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zrc.tanke756.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://obm.gaohongyu789.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ehw.quarkkingdee.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://agf.zhengqikj.top

================================================================================
来源：http://eji.pengpengdd.cyou

A. 基础语法与类型
来源：http://jip.xylfe.cn

================================================================================
来源：http://tzs.tianlin.xyz

[A01] Hello World
来源：http://rnx.zhengqikj.top

Py:   print("Hello, World!")
来源：http://svn.snrcjt.cn

PHP:  echo "Hello, World!";
来源：http://gmx.yangfankeji.com

JS:   console.log("Hello, World!");
来源：http://goq.zhixingplan.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hcr.zhongyouzk.top

Java: System.out.println("Hello, World!");
来源：http://syb.gogol.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://udi.kuanghao11.cn

Ruby: puts "Hello, World!"
来源：http://hwc.ivvv.top

C#:   Console.WriteLine("Hello, World!");
来源：http://yui.cashguo.top

[A02] 变量声明与赋值
来源：http://gto.shuidangran.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tzw.uphjek.com

PHP:  $name = "Alex"; $age = 20;
来源：http://wfy.shzxlz.cn

JS:   let name = "Alex"; const age = 20;
来源：http://szd.hongshengwenyu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wof.hywenlv.cn

Java: String name = "Alex"; int age = 20;
来源：http://fwi.quarkkingdee.top

Go:   name := "Alex"; age := 20
来源：http://hym.havefunace.top

Ruby: name = "Alex"; age = 20
来源：http://xna.ppjwa.cn

C#:   string name = "Alex"; int age = 20;
来源：http://wge.jqgfzy.top

[A03] 常量定义
来源：http://nqd.hnxiangtu.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jwy.xziqi.cn

PHP:  const PI = 3.14159;
来源：http://hdt.zhoulong.xyz

JS:   const PI = 3.14159;
来源：http://mss.xingfuxueyuan.xyz

TS:   const PI: number = 3.14159;
来源：http://xhr.cheryme.top

Java: static final double PI = 3.14159;
来源：http://rjq.ybcxt.top

Go:   const PI = 3.14159
来源：http://sru.hcnkem.com

Ruby: PI = 3.14159
来源：http://xoh.hongshengwenyu.top

C#:   const double PI = 3.14159;
来源：http://gkl.pengpengdd.cyou

[A04] 判断变量类型
来源：http://sut.cheryme.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://jee.sxryk.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hxs.yuanzhike.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jyn.xuanzx.com

TS:   typeof x; x instanceof Date
来源：http://bpq.snrcjt.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://agy.chenjidiqi.icu

Go:   reflect.TypeOf(x).Name()
来源：http://erw.guowangkeji.top

Ruby: x.class; x.is_a?(Integer)
来源：http://xgt.yuanzhike.top

C#:   x.GetType().Name; x is int
来源：http://gju.yuxming.cn

[A05] 整数除法与取模
来源：http://wyq.dashuyun.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ius.nanxuanxn.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://uvi.sysykeji.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pdp.hnxiangtu.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vxe.vqdsnc.cn

Java: 7 / 2; 7 % 2
来源：http://nbh.yangfankeji.com

Go:   7 / 2; 7 % 2
来源：http://mda.jinghuilouyu.cn

Ruby: 7 / 2; 7 % 2
来源：http://gir.xuanzx.com

C#:   7 / 2; 7 % 2
来源：http://oly.feifeiyinyue.top

[A06] 字符串转数字
来源：http://oqa.redwolf501.top

Py:   int("42"); float("3.14")
来源：http://cgr.sufxvd.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xkd.yuanzhike.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pwg.zhixingplan.top

TS:   parseInt("42", 10); Number("42")
来源：http://wjs.guannengcc.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ism.jinqigfzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kxh.zhijiandao.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://blc.jinghuilouyu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mzi.xziqi.cn

[A07] 数字转字符串
来源：http://gnz.redwolf501.top

Py:   str(42)
来源：http://vko.yongpay.top

PHP:  (string) 42; strval(42)
来源：http://lgd.ydzc1.top

JS:   String(42); (42).toString()
来源：http://mhz.meibo888.top

TS:   String(42)
来源：http://hiq.dashuyun.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zmp.cdnleiting.top

Go:   strconv.Itoa(42)
来源：http://mci.yvedp.cn

Ruby: 42.to_s
来源：http://wdf.chenjidiqi.icu

C#:   42.ToString()
来源：http://quw.hcnkem.com

[A08] 取整与四舍五入
来源：http://jhl.sweek.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dxt.cashguo.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vus.xingfuxueyuan.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://skg.cheryme.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ioj.guowangkeji.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qyu.ydzc1.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qwc.daria6918.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://eca.shzxlz.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hne.jinqigfzy.top

[A09] 绝对值与最大最小值
来源：http://dkz.gzhubu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xwj.shanyushiyangkeji.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://asw.bjfxy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qky.gzhubu.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mhl.fzhhl.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tcp.zhongyouzk.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://flm.xuetiantiany.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ztz.c1oappe.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://trr.jinqigfzy.top

[A10] 生成随机数
来源：http://udv.vehdjk.com

Py:   import random; random.randint(1, 100)
来源：http://iqe.zhongyouzk.top

PHP:  random_int(1, 100);
来源：http://ysw.dashuyun.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jbn.bbcook.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://klm.gzhubu.top

Java: new Random().nextInt(100) + 1
来源：http://nyq.chenlongwang.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://itt.hnqzz.top

Ruby: rand(1..100)
来源：http://mmp.nanxinkj.top

C#:   new Random().Next(1, 101)
来源：http://loy.shanyushiyangkeji.top

[A11] 条件表达式（三元）
来源：http://znr.zhiwuduotai.top

Py:   "yes" if x > 0 else "no"
来源：http://ttz.yuxming.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://gyk.zhoulong.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://yti.zdqjudy.top

TS:   x > 0 ? "yes" : "no"
来源：http://zbz.jinyuanbaomall.cn

Java: x > 0 ? "yes" : "no"
来源：http://sjv.zhijiandao.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ees.cheryme.top

Ruby: x > 0 ? "yes" : "no"
来源：http://aow.jinghuilouyu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fmh.zhaomingkeji.xyz

[A12] 字符串插值 / 格式化
来源：http://jid.shzxlz.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fpy.ehwqpu.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wpy.aizwys.cn

JS:   `Hello, ${name}!`
来源：http://ndn.shanyushiyangtech.top

TS:   `Hello, ${name}!`
来源：http://cfh.zhaomingkeji.xyz

Java: "Hello, %s!".formatted(name)
来源：http://yxc.yfazqb.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://goy.nanxuanxn.top

Ruby: "Hello, #{name}!"
来源：http://mdp.quarkkingdee.top

C#:   $"Hello, {name}!"
来源：http://fht.dashuyun.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://rbm.bjfxy.top

Py:   "第一行\n第二行"
来源：http://usc.ehwqpu.com

PHP:  "第一行\n第二行"
来源：http://nad.yangfankeji.com

JS:   "第一行\n第二行"
来源：http://ffu.xuetiantiany.cn

TS:   "第一行\n第二行"
来源：http://ssa.snrcjt.cn

Java: "第一行\n第二行"
来源：http://nav.ydjk.org.cn

Go:   "第一行\n第二行"
来源：http://hnh.yuanzhike.top

Ruby: "第一行\n第二行"
来源：http://ika.cqqwz.cn

C#:   "第一行\n第二行"
来源：http://onn.iojbl.cn

[A14] 注释写法
来源：http://utj.ybcxt.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://nfq.ywan-chungtsiang.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ryg.52xcode.cn

JS:   // 单行；/* 多行 */
来源：http://iwd.52xcode.cn

TS:   // 单行；/* 多行 */
来源：http://chg.jinqigfzy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jep.jinyuanbaomall.cn

Go:   // 单行；/* 多行 */
来源：http://ary.guowangkeji.top

Ruby: # 单行；=begin 多行 =end
来源：http://ora.jianghu66.top

C#:   // 单行；/* 多行 */
来源：http://fbx.mhx1999.top

[A15] 空值判断与默认值
来源：http://ffg.feifeiyinyue.top

Py:   value = data or "默认值"
来源：http://zuk.shanyushiyangkeji.top

PHP:  $value = $data ?? "默认值";
来源：http://wvo.shuidangran.top

JS:   const value = data ?? "默认值";
来源：http://qll.hammf.cn

TS:   const value = data ?? "默认值";
来源：http://pij.sufxvd.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mtk.fktsv.cn

Go:   if data == "" { data = "默认值" }
来源：http://pqm.jinghuilouyu.cn

Ruby: value = data || "默认值"
来源：http://ily.jlsjyb.cn

C#:   var value = data ?? "默认值";
来源：http://mze.9152youxi.cn

[A16] 真假值判断规则
来源：http://cgt.nanxinkj.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mnd.yj202588.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cis.jqgfzy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dqu.jqgfzy.top

TS:   if (!x) {}
来源：http://gxp.yfazqb.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qxm.sweek.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tzq.guowangkeji.top

Ruby: unless x            # nil 与 false 为假
来源：http://jrs.uphjek.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nax.gaohongyu789.top

[A17] 位运算
来源：http://adt.jinyuanbaomall.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mlu.iojbl.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dre.zhoulong.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ssf.fengsongda.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zte.tianlin.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nzk.yongpay.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zcf.jianghu66.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kix.jinqigufen.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://adr.0kj1m.cn

[A18] 字符与 ASCII 码互转
来源：http://qeo.andypj.xyz

Py:   ord("A"); chr(65)
来源：http://kku.jyoumei.cn

PHP:  ord("A"); chr(65)
来源：http://cni.tarul.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wco.smart0.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ybo.yj20258888.top

Java: (int) 'A'; (char) 65
来源：http://irc.shangyingyoupin.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cva.epnwcf.com

Ruby: "A".ord; 65.chr
来源：http://zjs.birdmap.top

C#:   (int)'A'; (char)65
来源：http://wmr.haohaochexian.top

[A19] 交换两个变量
来源：http://qrm.birdmap.top

Py:   a, b = b, a
来源：http://mor.mhx1999.top

PHP:  [$a, $b] = [$b, $a];
来源：http://uej.ywan-chungtsiang.top

JS:   [a, b] = [b, a];
来源：http://uyt.vehdjk.com

TS:   [a, b] = [b, a];
来源：http://cak.tarul.cn

Java: int t = a; a = b; b = t;
来源：http://dbw.ydzc1.top

Go:   a, b = b, a
来源：http://poa.zdqjudy.top

Ruby: a, b = b, a
来源：http://rua.gotoacloud.top

C#:   (a, b) = (b, a);
来源：http://fxw.iojbl.cn

[A20] 读取标准输入
来源：http://aft.hywenlv.cn

Py:   name = input("请输入：")
来源：http://yvx.yfazqb.com

PHP:  $name = trim(fgets(STDIN));
来源：http://ztm.cucudq.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sqj.ybcxt.top

TS:   // Node.js：readline 模块
来源：http://swc.svipenyu.cn

Java: new Scanner(System.in).nextLine()
来源：http://iap.sufxvd.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qph.cashguo.top

Ruby: gets.chomp
来源：http://hba.xziqi.cn

C#:   Console.ReadLine();
来源：http://apx.chenlongwang.top

[A21] 保留指定小数位输出
来源：http://cpu.dashuyun.cn

Py:   f"{3.14159:.2f}"
来源：http://hcj.yvedp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dfc.zdbjq.cn

JS:   (3.14159).toFixed(2)
来源：http://rgo.hfpthk.cn

TS:   (3.14159).toFixed(2)
来源：http://zgi.mhx1999.top

Java: String.format("%.2f", 3.14159)
来源：http://yoy.cashguo.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ccn.zhaomingkeji.xyz

Ruby: format("%.2f", 3.14159)
来源：http://vmm.snrcjt.cn

C#:   3.14159.ToString("F2")
来源：http://jpq.hnqzz.top

[A22] 获取字符串长度
来源：http://rvq.vqdsnc.cn

Py:   len(s)
来源：http://efh.gotoacloud.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hhb.yanxiufei.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://upn.yvedp.cn

TS:   s.length
来源：http://qlp.zhengqikj.top

Java: s.length()
来源：http://tfz.daria6918.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cyi.52xcode.cn

Ruby: s.length
来源：http://zch.jianghu66.top

C#:   s.Length
来源：http://qvc.yj20258.top

[A23] 大小写转换
来源：http://qnf.birdmap.top

Py:   s.upper(); s.lower(); s.title()
来源：http://lie.tianlin.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sdt.zhiwuduotai.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://znt.yueranfly.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xhs.0kj1m.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wat.ppjwa.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qjf.52xcode.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://axd.sjlbkw.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ejt.xingfuxueyuan.xyz

[A24] 去除首尾空白
来源：http://nkw.aibaodan.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ade.gzhubu.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mmq.zdqjudy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qqd.xuetiantiany.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qxa.c1oappe.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lsi.aibaodan.cn

Go:   strings.TrimSpace(s)
来源：http://wgi.zhaomingkeji.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gnr.gotoacloud.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kbg.gogol.net.cn

[A25] 字符串比较
来源：http://vzh.fengsongda.top

Py:   s1 == s2; s1 != s2
来源：http://hwf.aibaodan.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kek.fanxiaobao.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xhu.yanxiufei.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qcb.guowangkeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cey.tian-w.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://roh.ctjpmb.com

Ruby: s1 == s2; s1 <=> s2
来源：http://ipg.yongpay.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jcc.svipenyu.cn

[A26] 类型转换总览
来源：http://spq.tanke756.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dlv.sufxvd.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fia.jinghuilouyu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://adz.fzhhl.top

TS:   Number() String() Boolean() x as number
来源：http://nym.quarkkingdee.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wla.fengsongda.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gog.nanxuanxn.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://uad.ehwqpu.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dcg.9152youxi.cn

================================================================================
来源：http://opq.yangfankeji.com

B. 流程控制
来源：http://mfp.ctjpmb.com

================================================================================
来源：http://axt.hysaishi.cn

[B01] 条件判断 if / else
来源：http://qip.sufxvd.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vtr.aibaodan.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://abs.jlsjyb.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rhn.jinqigufen.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yaz.vqdsnc.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ctu.kuanghao11.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vgk.fzhhl.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pib.feifeiyinyue.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bzr.pengpengdd.cyou

[B02] 多分支 else if / elif
来源：http://ltp.nanxuanxn.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ery.ehwqpu.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xsn.gotoacloud.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ddr.ivvv.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cbb.smart0.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zxb.shzxlz.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yjj.xziqi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zci.gotoacloud.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://flr.shanyushiyangkeji.top

[B03] switch / match / case
来源：http://gxu.hesvh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://thh.jinqigfzy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zep.zdbjq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lno.yj20258.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mop.zhengqikj.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uip.cheryme.top


<!-- 参考信息 -->