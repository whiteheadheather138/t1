代发 wailian999

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dtv.9152youxi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vvo.xziqi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://bjc.kuanghao11.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lkn.yvedp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://azv.cashguo.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jpt.9152youxi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uyw.jinqigufen.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tbf.feifeiyinyue.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nhc.zhoulong.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://evh.havefunace.top

【文件统计】
来源：http://jhk.zdbjq.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vju.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://yes.shzxlz.cn

目  录
来源：http://asv.guannengcc.top

--------------------------------------------------------------------------------
来源：http://iun.snrcjt.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://guv.daxiang520.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ars.yongpay.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nij.ppjwa.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://iuv.zycfv.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ndw.guowangkeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://upt.jinqigfzy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xkd.52xcode.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uty.chenlongwang.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cwj.gogol.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://urh.pengpengdd.cyou

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pby.feifeiyinyue.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xfg.xingfuxueyuan.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vja.yangfankeji.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://oyk.shanyushiyangkeji.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://llf.wangdashe.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://inv.fengsongda.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xin.ppjwa.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vat.smart0.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://emk.cucudq.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://acs.jyoumei.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dxa.sjlbkw.cn

================================================================================
来源：http://gyd.pengpengdd.cyou

A. 基础语法与类型
来源：http://utg.ivvv.top

================================================================================
来源：http://vsp.nanxuanxn.top

[A01] Hello World
来源：http://prl.hongshengwenyu.top

Py:   print("Hello, World!")
来源：http://jmr.nanxuanxn.top

PHP:  echo "Hello, World!";
来源：http://bjw.xingfuxueyuan.xyz

JS:   console.log("Hello, World!");
来源：http://tgv.wangshuangyany.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mmk.yangfankeji.com

Java: System.out.println("Hello, World!");
来源：http://vor.ctjpmb.com

Go:   fmt.Println("Hello, World!")
来源：http://cjc.ehwqpu.com

Ruby: puts "Hello, World!"
来源：http://zec.tanke756.top

C#:   Console.WriteLine("Hello, World!");
来源：http://mfj.hnqzz.top

[A02] 变量声明与赋值
来源：http://bfr.zhoulong.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ges.hesvh.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://iwr.52xcode.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vpt.jinqigufen.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lqq.aibaodan.cn

Java: String name = "Alex"; int age = 20;
来源：http://ipi.quarkkingdee.top

Go:   name := "Alex"; age := 20
来源：http://fnw.zhengqikj.top

Ruby: name = "Alex"; age = 20
来源：http://hih.ctjpmb.com

C#:   string name = "Alex"; int age = 20;
来源：http://vzb.daria6918.cn

[A03] 常量定义
来源：http://yfz.yangfankeji.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://flj.xziqi.cn

PHP:  const PI = 3.14159;
来源：http://uym.fktsv.cn

JS:   const PI = 3.14159;
来源：http://zva.aibaodan.cn

TS:   const PI: number = 3.14159;
来源：http://gwk.ydjk.org.cn

Java: static final double PI = 3.14159;
来源：http://fir.fanxiaobao.xyz

Go:   const PI = 3.14159
来源：http://gep.jinyuanbaomall.cn

Ruby: PI = 3.14159
来源：http://amm.fehbvm.com

C#:   const double PI = 3.14159;
来源：http://wih.dashuyun.cn

[A04] 判断变量类型
来源：http://yxq.iojbl.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ovp.nwbrower.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tml.yueranfly.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ayb.gaohongyu789.top

TS:   typeof x; x instanceof Date
来源：http://aor.ctjpmb.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://alb.haohaochexian.top

Go:   reflect.TypeOf(x).Name()
来源：http://inq.yj202588.top

Ruby: x.class; x.is_a?(Integer)
来源：http://tpy.iojbl.cn

C#:   x.GetType().Name; x is int
来源：http://ndi.shuidangran.top

[A05] 整数除法与取模
来源：http://akb.yj20258.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pkj.iojbl.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fkp.chenjidiqi.icu

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://oyw.daria6918.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tiu.yj202588.top

Java: 7 / 2; 7 % 2
来源：http://lhp.xuetiantiany.cn

Go:   7 / 2; 7 % 2
来源：http://qgw.hcnkem.com

Ruby: 7 / 2; 7 % 2
来源：http://mio.yonumen.top

C#:   7 / 2; 7 % 2
来源：http://rrx.yueranfly.top

[A06] 字符串转数字
来源：http://pyt.hywenlv.cn

Py:   int("42"); float("3.14")
来源：http://czf.hfpthk.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jyq.zdbjq.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hvz.daxiang520.top

TS:   parseInt("42", 10); Number("42")
来源：http://usy.tarul.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fjl.yfazqb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qgg.ywan-chungtsiang.top

Ruby: "42".to_i; "3.14".to_f
来源：http://rto.hywenlv.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yxy.sysykeji.top

[A07] 数字转字符串
来源：http://sib.haohaochexian.top

Py:   str(42)
来源：http://btp.cheryme.top

PHP:  (string) 42; strval(42)
来源：http://mmf.yuanzhike.top

JS:   String(42); (42).toString()
来源：http://rvw.yangfankeji.com

TS:   String(42)
来源：http://zof.fehbvm.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://bpy.jinyuanbaomall.cn

Go:   strconv.Itoa(42)
来源：http://rci.jyoumei.cn

Ruby: 42.to_s
来源：http://tfa.ivvv.top

C#:   42.ToString()
来源：http://vai.316326.xyz

[A08] 取整与四舍五入
来源：http://eke.yj202588.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rtg.mhx1999.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dma.hongshengwenyu.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bvw.svipenyu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tex.uphjek.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sht.epnwcf.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://uut.nanxuanxn.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ydc.shuidangran.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kuo.pycfn.com

[A09] 绝对值与最大最小值
来源：http://nln.sweek.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rbj.chenlongwang.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://urw.52xcode.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jhz.zhixingplan.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://net.jianghu66.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://unk.kuanghao11.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gqv.yanxiufei.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rsj.xingfuxueyuan.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pdc.hcnkem.com

[A10] 生成随机数
来源：http://goi.zhongyouzk.top

Py:   import random; random.randint(1, 100)
来源：http://wkj.nwbrower.top

PHP:  random_int(1, 100);
来源：http://jzr.c1oappe.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uxz.yj20258.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rqe.fanxiaobao.xyz

Java: new Random().nextInt(100) + 1
来源：http://sun.jyoumei.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vgv.xylfe.cn

Ruby: rand(1..100)
来源：http://wpu.fengsongda.top

C#:   new Random().Next(1, 101)
来源：http://phn.nwbrower.top

[A11] 条件表达式（三元）
来源：http://etr.tarul.cn

Py:   "yes" if x > 0 else "no"
来源：http://lfr.zhaomingkeji.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://wdj.hysaishi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://txn.cdnleiting.top

TS:   x > 0 ? "yes" : "no"
来源：http://zsv.tianlin.xyz

Java: x > 0 ? "yes" : "no"
来源：http://tfa.pycfn.com

Go:   // 无三元运算符，需用 if 语句
来源：http://rhb.havefunace.top

Ruby: x > 0 ? "yes" : "no"
来源：http://tox.zhoulong.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://ctx.9152youxi.cn

[A12] 字符串插值 / 格式化
来源：http://ltu.nanxuanxn.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://suu.zycfv.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://acx.jinqigufen.top

JS:   `Hello, ${name}!`
来源：http://rng.zycfv.cn

TS:   `Hello, ${name}!`
来源：http://nhr.gogol.net.cn

Java: "Hello, %s!".formatted(name)
来源：http://vhd.zhaomingkeji.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zpw.svipenyu.cn

Ruby: "Hello, #{name}!"
来源：http://zpj.shangyingyoupin.top

C#:   $"Hello, {name}!"
来源：http://tud.jinyuanbaomall.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ifc.fzhhl.top

Py:   "第一行\n第二行"
来源：http://ebc.jinyuanbaomall.cn

PHP:  "第一行\n第二行"
来源：http://wkm.tian-w.cn

JS:   "第一行\n第二行"
来源：http://run.zhijiandao.cn

TS:   "第一行\n第二行"
来源：http://qor.cucudq.cn

Java: "第一行\n第二行"
来源：http://qsx.yuxming.cn

Go:   "第一行\n第二行"
来源：http://omm.52xcode.cn

Ruby: "第一行\n第二行"
来源：http://ryj.epnwcf.com

C#:   "第一行\n第二行"
来源：http://ioc.ydjk.org.cn

[A14] 注释写法
来源：http://ouh.ehwqpu.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://idz.bjfxy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://xxo.ehwqpu.com

JS:   // 单行；/* 多行 */
来源：http://sns.jyoumei.cn

TS:   // 单行；/* 多行 */
来源：http://ibd.epnwcf.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dmw.cashguo.top

Go:   // 单行；/* 多行 */
来源：http://tse.cashguo.top

Ruby: # 单行；=begin 多行 =end
来源：http://lxv.jqgufenzy.top

C#:   // 单行；/* 多行 */
来源：http://eki.dianchejie.cn

[A15] 空值判断与默认值
来源：http://fjl.havefunace.top

Py:   value = data or "默认值"
来源：http://dqk.ehwqpu.com

PHP:  $value = $data ?? "默认值";
来源：http://oss.fzhhl.top

JS:   const value = data ?? "默认值";
来源：http://yaz.shanyushiyangkeji.top

TS:   const value = data ?? "默认值";
来源：http://krx.zhiwuduotai.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://opf.tarul.cn

Go:   if data == "" { data = "默认值" }
来源：http://kix.cheryme.top

Ruby: value = data || "默认值"
来源：http://ozd.dashuyun.cn

C#:   var value = data ?? "默认值";
来源：http://shk.zhengqikj.top

[A16] 真假值判断规则
来源：http://kmb.ybcxt.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ywf.kuanghao11.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gkm.dianchejie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://stb.guannengcc.top

TS:   if (!x) {}
来源：http://upy.shuidangran.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zkt.cucudq.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://oas.zhengqikj.top

Ruby: unless x            # nil 与 false 为假
来源：http://jgq.hcnkem.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ppt.yonumen.top

[A17] 位运算
来源：http://pzd.fanxiaobao.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qhg.jlsjyb.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nqc.kuanghao11.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fqg.gogol.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ksr.zhengqikj.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bjo.haohaochexian.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yon.jinghuilouyu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wth.bbcook.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kaq.tanke756.top

[A18] 字符与 ASCII 码互转
来源：http://jgj.guannengcc.top

Py:   ord("A"); chr(65)
来源：http://ehw.sxryk.cn

PHP:  ord("A"); chr(65)
来源：http://tmv.yj202588.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tei.andypj.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ifg.sufxvd.cn

Java: (int) 'A'; (char) 65
来源：http://gmd.xuanzx.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dwl.tarul.cn

Ruby: "A".ord; 65.chr
来源：http://pgy.nanxinkj.top

C#:   (int)'A'; (char)65
来源：http://bar.dianchejie.cn

[A19] 交换两个变量
来源：http://vsz.chenzaomai.com

Py:   a, b = b, a
来源：http://sus.shangyingyoupin.top

PHP:  [$a, $b] = [$b, $a];
来源：http://kbn.svipenyu.cn

JS:   [a, b] = [b, a];
来源：http://yny.chenzaomai.com

TS:   [a, b] = [b, a];
来源：http://oud.yonumen.top

Java: int t = a; a = b; b = t;
来源：http://sbk.chenjidiqi.icu

Go:   a, b = b, a
来源：http://urx.dashuyun.cn

Ruby: a, b = b, a
来源：http://brq.c1oappe.top

C#:   (a, b) = (b, a);
来源：http://ils.cheryme.top

[A20] 读取标准输入
来源：http://njn.bbcook.cn

Py:   name = input("请输入：")
来源：http://nhp.jinghuilouyu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://afy.yvedp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sdv.jlsjyb.cn

TS:   // Node.js：readline 模块
来源：http://aax.smart0.xyz

Java: new Scanner(System.in).nextLine()
来源：http://isg.ivvv.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pup.wangdashe.top

Ruby: gets.chomp
来源：http://uab.jqgufenzy.top

C#:   Console.ReadLine();
来源：http://rzb.shuidangran.top

[A21] 保留指定小数位输出
来源：http://ksb.jinqigufen.top

Py:   f"{3.14159:.2f}"
来源：http://fsh.aibaodan.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wvr.redwolf501.top

JS:   (3.14159).toFixed(2)
来源：http://afr.yanxiufei.cn

TS:   (3.14159).toFixed(2)
来源：http://giq.uphjek.com

Java: String.format("%.2f", 3.14159)
来源：http://ttr.tanke756.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blc.zhoulong.xyz

Ruby: format("%.2f", 3.14159)
来源：http://esk.xziqi.cn

C#:   3.14159.ToString("F2")
来源：http://tzp.yuanzhike.top

[A22] 获取字符串长度
来源：http://gjp.jyoumei.cn

Py:   len(s)
来源：http://bbr.bbcook.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://clc.shangyingyoupin.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zdz.zhixingplan.top

TS:   s.length
来源：http://ubt.daria6918.cn

Java: s.length()
来源：http://vlx.guowangkeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pur.jiagoushi.top

Ruby: s.length
来源：http://jzf.9152youxi.cn

C#:   s.Length
来源：http://pmu.hnxiangtu.top

[A23] 大小写转换
来源：http://hlw.sjlbkw.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lvk.hammf.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qgh.hongshengwenyu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lua.jinqigfzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cln.hnqzz.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dpd.jinqigfzy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xps.ppjwa.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://shj.sjlbkw.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ehf.shuidangran.top

[A24] 去除首尾空白
来源：http://syj.shzxlz.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lpb.dashuyun.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zwb.chenlongwang.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rkf.jqgufenzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jnd.yongpay.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pus.aibaodan.cn

Go:   strings.TrimSpace(s)
来源：http://vvt.jinyuanbaomall.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://erq.pengpengdd.cyou

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kmw.shangyingyoupin.top

[A25] 字符串比较
来源：http://iqr.hnqzz.top

Py:   s1 == s2; s1 != s2
来源：http://aod.epnwcf.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nve.quarkkingdee.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kzc.yj20258888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://djw.kuanghao11.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mth.hywenlv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dsf.jinqigfzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://psk.xinyue.icu

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yja.ydzc1.top

[A26] 类型转换总览
来源：http://fuw.iojbl.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lnx.zdqjudy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ylu.sxryk.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dpx.cashguo.top

TS:   Number() String() Boolean() x as number
来源：http://ire.aibaodan.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://juj.hcnkem.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jfi.fzhhl.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://txt.daxiang520.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ven.shanyushiyangkeji.top

================================================================================
来源：http://dnl.yueranfly.top

B. 流程控制
来源：http://hzc.sxryk.cn

================================================================================
来源：http://bvi.bjfxy.top

[B01] 条件判断 if / else
来源：http://xfv.snrcjt.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rex.mhx1999.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jph.tianlin.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://urc.quarkkingdee.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yln.aizwys.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qwd.iojbl.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hey.yanxiufei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://glm.0kj1m.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hfj.sufxvd.cn

[B02] 多分支 else if / elif
来源：http://lvz.tanke756.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qxk.zhijiandao.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kmk.sjlbkw.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jnw.zhiwuduotai.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jen.jinyuanbaomall.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iyh.nwbrower.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dyj.zdbjq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://myf.haohaochexian.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ddd.daria6918.cn

[B03] switch / match / case
来源：http://mwe.daria6918.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://smy.ctjpmb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://awj.ybcxt.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ufc.jqgfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uxz.shuidangran.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://myr.meibo888.top


<!-- 参考信息 -->