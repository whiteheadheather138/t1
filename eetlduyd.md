代发 wailian999

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jfp.zhijiandao.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vns.daxiang520.top

Bash:  Shell         C:     C             C++:   C++
来源：http://bod.cashguo.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jqk.zhijiandao.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hcd.aibaodan.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://afd.xylfe.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vil.tarul.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vtj.epnwcf.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xyd.zdbjq.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vav.smart0.xyz

【文件统计】
来源：http://cvr.ydjk.org.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://iih.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://dlg.hnxiangtu.top

目  录
来源：http://okm.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://nce.xylfe.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xfy.xinyue.icu

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xcf.birdmap.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ngi.daria6918.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wpn.ydzc1.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lut.bjfxy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ank.ehwqpu.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kfc.meibo888.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uao.andypj.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yzk.bjfxy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://buq.feifeiyinyue.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rrf.ywan-chungtsiang.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gnh.havefunace.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ksd.shzxlz.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wgr.xingfuxueyuan.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://eus.xylfe.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vwh.xingfuxueyuan.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ktc.sysykeji.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://sog.fengsongda.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lyw.hnxiangtu.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fno.tianlin.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rjg.yj20258888.top

================================================================================
来源：http://gvh.zhijiandao.cn

A. 基础语法与类型
来源：http://tpw.shzxlz.cn

================================================================================
来源：http://ndr.sufxvd.cn

[A01] Hello World
来源：http://ijf.yvedp.cn

Py:   print("Hello, World!")
来源：http://way.yfazqb.com

PHP:  echo "Hello, World!";
来源：http://jxq.guannengcc.top

JS:   console.log("Hello, World!");
来源：http://bjo.yj20258.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zzc.ehwqpu.com

Java: System.out.println("Hello, World!");
来源：http://udz.daria6918.cn

Go:   fmt.Println("Hello, World!")
来源：http://idw.gotoacloud.top

Ruby: puts "Hello, World!"
来源：http://tjt.fzhhl.top

C#:   Console.WriteLine("Hello, World!");
来源：http://uti.0kj1m.cn

[A02] 变量声明与赋值
来源：http://iux.chenzaomai.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kju.0kj1m.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://cvz.cucudq.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ztr.ehwqpu.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pue.andypj.xyz

Java: String name = "Alex"; int age = 20;
来源：http://jrm.nwbrower.top

Go:   name := "Alex"; age := 20
来源：http://oyc.ywan-chungtsiang.top

Ruby: name = "Alex"; age = 20
来源：http://brx.hammf.cn

C#:   string name = "Alex"; int age = 20;
来源：http://bdg.redwolf501.top

[A03] 常量定义
来源：http://eda.mhx1999.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://flo.shanyushiyangtech.top

PHP:  const PI = 3.14159;
来源：http://tkd.xuetiantiany.cn

JS:   const PI = 3.14159;
来源：http://shv.yangfankeji.com

TS:   const PI: number = 3.14159;
来源：http://jix.hfpthk.cn

Java: static final double PI = 3.14159;
来源：http://yhg.havefunace.top

Go:   const PI = 3.14159
来源：http://gcn.iojbl.cn

Ruby: PI = 3.14159
来源：http://bix.gzhubu.top

C#:   const double PI = 3.14159;
来源：http://evg.zdbjq.cn

[A04] 判断变量类型
来源：http://hvv.jqgfzy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://itz.chenjidiqi.icu

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ppf.ydjk.org.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ogd.epnwcf.com

TS:   typeof x; x instanceof Date
来源：http://qzk.ydzc1.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rvu.bjfxy.top

Go:   reflect.TypeOf(x).Name()
来源：http://pkg.yj202588.top

Ruby: x.class; x.is_a?(Integer)
来源：http://lgv.hywenlv.cn

C#:   x.GetType().Name; x is int
来源：http://xcz.9152youxi.cn

[A05] 整数除法与取模
来源：http://bwf.sysykeji.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gat.gaohongyu789.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://uwd.cheryme.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bsy.sysykeji.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qih.yanxiufei.cn

Java: 7 / 2; 7 % 2
来源：http://nev.fzhhl.top

Go:   7 / 2; 7 % 2
来源：http://fbi.hcnkem.com

Ruby: 7 / 2; 7 % 2
来源：http://xln.snrcjt.cn

C#:   7 / 2; 7 % 2
来源：http://myz.redwolf501.top

[A06] 字符串转数字
来源：http://uaf.guowangkeji.top

Py:   int("42"); float("3.14")
来源：http://xrx.chenjidiqi.icu

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jli.fengsongda.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tdf.quarkkingdee.top

TS:   parseInt("42", 10); Number("42")
来源：http://ejc.fktsv.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fue.vqdsnc.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hmg.yj202588.top

Ruby: "42".to_i; "3.14".to_f
来源：http://vmj.meibo888.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vsn.shzxlz.cn

[A07] 数字转字符串
来源：http://wne.guowangkeji.top

Py:   str(42)
来源：http://rtf.daxiang520.top

PHP:  (string) 42; strval(42)
来源：http://vbt.ppjwa.cn

JS:   String(42); (42).toString()
来源：http://yir.xinyue.icu

TS:   String(42)
来源：http://skn.yongpay.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://nqo.dianchejie.cn

Go:   strconv.Itoa(42)
来源：http://zsk.zhongyouzk.top

Ruby: 42.to_s
来源：http://egi.ydjk.org.cn

C#:   42.ToString()
来源：http://qnt.wangshuangyany.cn

[A08] 取整与四舍五入
来源：http://txe.zhijiandao.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://idm.gotoacloud.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mcz.zhongyouzk.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gkc.zhiwuduotai.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://txl.hongshengwenyu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xia.daria6918.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jpr.yj202588.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://nbf.fanxiaobao.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rmg.cdnleiting.top

[A09] 绝对值与最大最小值
来源：http://mte.wangshuangyany.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mdh.xuetiantiany.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://awv.cashguo.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://evd.hammf.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wxb.sweek.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ejw.vehdjk.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mgw.tanke756.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cse.kuanghao11.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://suh.xuetiantiany.cn

[A10] 生成随机数
来源：http://coh.nanxuanxn.top

Py:   import random; random.randint(1, 100)
来源：http://nnn.cqqwz.cn

PHP:  random_int(1, 100);
来源：http://zhm.zhixingplan.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ryz.hammf.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vve.dashuyun.cn

Java: new Random().nextInt(100) + 1
来源：http://lse.sjlbkw.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cdi.chenjidiqi.icu

Ruby: rand(1..100)
来源：http://atj.0kj1m.cn

C#:   new Random().Next(1, 101)
来源：http://hyo.yangfankeji.com

[A11] 条件表达式（三元）
来源：http://lof.sweek.top

Py:   "yes" if x > 0 else "no"
来源：http://yok.zdqjudy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://jkw.feifeiyinyue.top

JS:   x > 0 ? "yes" : "no"
来源：http://byj.hnqzz.top

TS:   x > 0 ? "yes" : "no"
来源：http://kmi.snrcjt.cn

Java: x > 0 ? "yes" : "no"
来源：http://thp.yvedp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wfa.zhixingplan.top

Ruby: x > 0 ? "yes" : "no"
来源：http://xwj.zycfv.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fle.jiagoushi.top

[A12] 字符串插值 / 格式化
来源：http://xwu.vehdjk.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xwz.chenzaomai.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zyp.ivvv.top

JS:   `Hello, ${name}!`
来源：http://obn.nwbrower.top

TS:   `Hello, ${name}!`
来源：http://jsl.ctjpmb.com

Java: "Hello, %s!".formatted(name)
来源：http://bon.shanyushiyangtech.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jqw.tarul.cn

Ruby: "Hello, #{name}!"
来源：http://azo.52xcode.cn

C#:   $"Hello, {name}!"
来源：http://smx.sweek.top

[A13] 多行字符串（练习 \n 转义）
来源：http://xqb.yuanzhike.top

Py:   "第一行\n第二行"
来源：http://mxe.ehwqpu.com

PHP:  "第一行\n第二行"
来源：http://osb.shangyingyoupin.top

JS:   "第一行\n第二行"
来源：http://dgl.xylfe.cn

TS:   "第一行\n第二行"
来源：http://jzk.xinyue.icu

Java: "第一行\n第二行"
来源：http://uwq.zhijiandao.cn

Go:   "第一行\n第二行"
来源：http://qio.yueranfly.top

Ruby: "第一行\n第二行"
来源：http://usc.daxiang520.top

C#:   "第一行\n第二行"
来源：http://prn.guowangkeji.top

[A14] 注释写法
来源：http://sgp.bbcook.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zua.hcnkem.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://boa.xuanzx.com

JS:   // 单行；/* 多行 */
来源：http://okb.zhijiandao.cn

TS:   // 单行；/* 多行 */
来源：http://hbf.ybcxt.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qhb.daxiang520.top

Go:   // 单行；/* 多行 */
来源：http://umq.aibaodan.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rhv.zhengqikj.top

C#:   // 单行；/* 多行 */
来源：http://ojj.316326.xyz

[A15] 空值判断与默认值
来源：http://oyz.jyoumei.cn

Py:   value = data or "默认值"
来源：http://tiw.shanyushiyangtech.top

PHP:  $value = $data ?? "默认值";
来源：http://kmu.yuxming.cn

JS:   const value = data ?? "默认值";
来源：http://lpu.tian-w.cn

TS:   const value = data ?? "默认值";
来源：http://jen.meibo888.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vdy.pengpengdd.cyou

Go:   if data == "" { data = "默认值" }
来源：http://prh.sjlbkw.cn

Ruby: value = data || "默认值"
来源：http://qup.jinghuilouyu.cn

C#:   var value = data ?? "默认值";
来源：http://ezt.yueranfly.top

[A16] 真假值判断规则
来源：http://vdf.yonumen.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ylr.kuanghao11.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://htc.fengsongda.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ddg.ppjwa.cn

TS:   if (!x) {}
来源：http://nax.xylfe.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jgh.bbcook.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ooy.gaohongyu789.top

Ruby: unless x            # nil 与 false 为假
来源：http://hyn.epnwcf.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mms.zhixingplan.top

[A17] 位运算
来源：http://aog.mhx1999.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qqp.yj20258.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tzl.redwolf501.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vqo.bjfxy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jcg.haohaochexian.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jcj.shuidangran.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://trc.yuxming.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pji.52xcode.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zaz.tian-w.cn

[A18] 字符与 ASCII 码互转
来源：http://ubu.yonumen.top

Py:   ord("A"); chr(65)
来源：http://rmj.bbcook.cn

PHP:  ord("A"); chr(65)
来源：http://sty.sxryk.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dku.jianghu66.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xhf.ydjk.org.cn

Java: (int) 'A'; (char) 65
来源：http://tlw.chenjidiqi.icu

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://klg.vehdjk.com

Ruby: "A".ord; 65.chr
来源：http://nnd.zdbjq.cn

C#:   (int)'A'; (char)65
来源：http://fms.shuidangran.top

[A19] 交换两个变量
来源：http://yjq.ehwqpu.com

Py:   a, b = b, a
来源：http://zbe.redwolf501.top

PHP:  [$a, $b] = [$b, $a];
来源：http://adt.gzhubu.top

JS:   [a, b] = [b, a];
来源：http://aip.nanxuanxn.top

TS:   [a, b] = [b, a];
来源：http://jpj.wangshuangyany.cn

Java: int t = a; a = b; b = t;
来源：http://igf.aibaodan.cn

Go:   a, b = b, a
来源：http://hdu.ivvv.top

Ruby: a, b = b, a
来源：http://hro.xinyue.icu

C#:   (a, b) = (b, a);
来源：http://jap.snrcjt.cn

[A20] 读取标准输入
来源：http://kdr.cashguo.top

Py:   name = input("请输入：")
来源：http://sop.ppjwa.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ydl.ybcxt.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cvy.yj20258.top

TS:   // Node.js：readline 模块
来源：http://cgr.nanxinkj.top

Java: new Scanner(System.in).nextLine()
来源：http://rcx.meibo888.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://umr.havefunace.top

Ruby: gets.chomp
来源：http://rks.tian-w.cn

C#:   Console.ReadLine();
来源：http://jij.jianghu66.top

[A21] 保留指定小数位输出
来源：http://rxt.mhx1999.top

Py:   f"{3.14159:.2f}"
来源：http://vpg.zdqjudy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://anj.tarul.cn

JS:   (3.14159).toFixed(2)
来源：http://wwk.sysykeji.top

TS:   (3.14159).toFixed(2)
来源：http://zre.yj20258.top

Java: String.format("%.2f", 3.14159)
来源：http://lhx.sysykeji.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xov.zhengqikj.top

Ruby: format("%.2f", 3.14159)
来源：http://iyw.wangdashe.top

C#:   3.14159.ToString("F2")
来源：http://btc.pengpengdd.cyou

[A22] 获取字符串长度
来源：http://owc.xingfuxueyuan.xyz

Py:   len(s)
来源：http://seo.hfpthk.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jxu.epnwcf.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bzb.dashuyun.cn

TS:   s.length
来源：http://rgn.havefunace.top

Java: s.length()
来源：http://ega.hnqzz.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tqb.shuidangran.top

Ruby: s.length
来源：http://nmv.svipenyu.cn

C#:   s.Length
来源：http://tsv.tanke756.top

[A23] 大小写转换
来源：http://jlr.jianghu66.top

Py:   s.upper(); s.lower(); s.title()
来源：http://zpa.yongpay.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hyg.pengpengdd.cyou

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://apq.hcnkem.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ohe.hysaishi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qoe.jlsjyb.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sac.bjfxy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://htb.zycfv.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fej.cqqwz.cn

[A24] 去除首尾空白
来源：http://kwa.zhengqikj.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bqs.cdnleiting.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gvc.jinyuanbaomall.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ywo.pengpengdd.cyou

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gnc.epnwcf.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://feo.vqdsnc.cn

Go:   strings.TrimSpace(s)
来源：http://tcn.chenjidiqi.icu

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xec.aibaodan.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://awt.bjfxy.top

[A25] 字符串比较
来源：http://vqj.jinghuilouyu.cn

Py:   s1 == s2; s1 != s2
来源：http://pyi.daxiang520.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pkj.zhengqikj.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tqq.mhx1999.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://loj.yangfankeji.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vta.0kj1m.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dsn.zdqjudy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://dzc.cdnleiting.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ury.xingfuxueyuan.xyz

[A26] 类型转换总览
来源：http://kww.daria6918.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qqu.epnwcf.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rhw.jinyuanbaomall.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hta.tarul.cn

TS:   Number() String() Boolean() x as number
来源：http://vvs.guowangkeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tjr.yonumen.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zuk.xuanzx.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://ihh.vqdsnc.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gnq.yongpay.top

================================================================================
来源：http://qpl.hywenlv.cn

B. 流程控制
来源：http://kcy.jiagoushi.top

================================================================================
来源：http://xch.yanxiufei.cn

[B01] 条件判断 if / else
来源：http://rbz.shuidangran.top

Py:   result = "正" if x > 0 else "非正"
来源：http://jww.kuanghao11.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jdf.redwolf501.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lcq.zhiwuduotai.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://owa.meibo888.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://mhe.bjfxy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wur.yonumen.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eqh.smart0.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nvy.jinqigfzy.top

[B02] 多分支 else if / elif
来源：http://zws.hnqzz.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qwy.316326.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dej.zycfv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jfm.0kj1m.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cor.yj20258888.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gpq.cucudq.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wbi.andypj.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zqy.9152youxi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jur.tanke756.top

[B03] switch / match / case
来源：http://eai.shanyushiyangkeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wfy.cashguo.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wcy.andypj.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://elt.aibaodan.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fdw.ydzc1.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pan.zhiwuduotai.top


<!-- 参考信息 -->