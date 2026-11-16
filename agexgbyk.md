代发 wailian999

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zrc.haohaochexian.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jlx.9152youxi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ssz.yonumen.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fsr.smart0.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qya.tarul.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jhc.zhaomingkeji.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ade.tarul.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qnt.guannengcc.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nug.hysaishi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://igr.andypj.xyz

【文件统计】
来源：http://xwl.zhaomingkeji.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sna.yuxming.cn

--------------------------------------------------------------------------------
来源：http://edq.fehbvm.com

目  录
来源：http://jlo.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://prk.yj202588.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://med.nwbrower.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gop.jinyuanbaomall.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sxi.cashguo.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tvi.xuetiantiany.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fws.jianghu66.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kif.yongpay.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kug.guannengcc.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ssx.shzxlz.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://oyz.shanyushiyangkeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wnv.yanxiufei.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kgc.chenjidiqi.icu

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://muh.zhijiandao.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://oja.ctjpmb.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nze.snrcjt.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zgn.zhongyouzk.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dvv.guowangkeji.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yjj.epnwcf.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://cyb.vehdjk.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://txe.yongpay.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lmf.shzxlz.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://prr.iojbl.cn

================================================================================
来源：http://max.9152youxi.cn

A. 基础语法与类型
来源：http://pye.xinyue.icu

================================================================================
来源：http://dfh.chenlongwang.top

[A01] Hello World
来源：http://bij.zhiwuduotai.top

Py:   print("Hello, World!")
来源：http://jzw.ydzc1.top

PHP:  echo "Hello, World!";
来源：http://dxx.wangshuangyany.cn

JS:   console.log("Hello, World!");
来源：http://bmw.fktsv.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ncg.snrcjt.cn

Java: System.out.println("Hello, World!");
来源：http://ktl.guannengcc.top

Go:   fmt.Println("Hello, World!")
来源：http://ehi.316326.xyz

Ruby: puts "Hello, World!"
来源：http://zcm.mhx1999.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ola.yj202588.top

[A02] 变量声明与赋值
来源：http://nlj.52xcode.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://smk.dashuyun.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xrc.ybcxt.top

JS:   let name = "Alex"; const age = 20;
来源：http://jxh.jianghu66.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://usk.fktsv.cn

Java: String name = "Alex"; int age = 20;
来源：http://unt.zhixingplan.top

Go:   name := "Alex"; age := 20
来源：http://fgr.guowangkeji.top

Ruby: name = "Alex"; age = 20
来源：http://wnx.tarul.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vvw.yj20258.top

[A03] 常量定义
来源：http://mnr.haohaochexian.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ern.andypj.xyz

PHP:  const PI = 3.14159;
来源：http://zdx.dashuyun.cn

JS:   const PI = 3.14159;
来源：http://ezp.jinghuilouyu.cn

TS:   const PI: number = 3.14159;
来源：http://kuu.andypj.xyz

Java: static final double PI = 3.14159;
来源：http://fny.xuanzx.com

Go:   const PI = 3.14159
来源：http://owh.yj202588.top

Ruby: PI = 3.14159
来源：http://toh.cashguo.top

C#:   const double PI = 3.14159;
来源：http://dnb.sxryk.cn

[A04] 判断变量类型
来源：http://cph.mhx1999.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://nmi.ywan-chungtsiang.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dui.hfpthk.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xut.zdqjudy.top

TS:   typeof x; x instanceof Date
来源：http://pvi.yueranfly.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mnv.yvedp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://iri.epnwcf.com

Ruby: x.class; x.is_a?(Integer)
来源：http://aya.ybcxt.top

C#:   x.GetType().Name; x is int
来源：http://rmo.jinqigfzy.top

[A05] 整数除法与取模
来源：http://vtc.cqqwz.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bpt.xziqi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cbc.cqqwz.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vwv.pengpengdd.cyou

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fih.zdqjudy.top

Java: 7 / 2; 7 % 2
来源：http://laq.zhaomingkeji.xyz

Go:   7 / 2; 7 % 2
来源：http://uhj.zycfv.cn

Ruby: 7 / 2; 7 % 2
来源：http://dvn.cheryme.top

C#:   7 / 2; 7 % 2
来源：http://htv.yj20258.top

[A06] 字符串转数字
来源：http://dpy.chenzaomai.com

Py:   int("42"); float("3.14")
来源：http://cki.birdmap.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xtw.yangfankeji.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dkh.ydjk.org.cn

TS:   parseInt("42", 10); Number("42")
来源：http://lsy.nwbrower.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://uxw.yuanzhike.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://eyj.nanxuanxn.top

Ruby: "42".to_i; "3.14".to_f
来源：http://lrd.cheryme.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fxk.jqgfzy.top

[A07] 数字转字符串
来源：http://rgc.gzhubu.top

Py:   str(42)
来源：http://iax.cucudq.cn

PHP:  (string) 42; strval(42)
来源：http://bmh.shangyingyoupin.top

JS:   String(42); (42).toString()
来源：http://wgp.shuidangran.top

TS:   String(42)
来源：http://eek.ybcxt.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ehg.316326.xyz

Go:   strconv.Itoa(42)
来源：http://dug.zdbjq.cn

Ruby: 42.to_s
来源：http://wdo.nwbrower.top

C#:   42.ToString()
来源：http://grj.tianlin.xyz

[A08] 取整与四舍五入
来源：http://ciy.wangdashe.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://got.gogol.net.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yxi.jqgfzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vny.hcnkem.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lka.kuanghao11.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://imf.redwolf501.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ngi.zhixingplan.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://pwj.yj202588.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://suc.zhongyouzk.top

[A09] 绝对值与最大最小值
来源：http://uqh.xinyue.icu

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://amm.tarul.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mgz.yj202588.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://avb.quarkkingdee.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uhw.yongpay.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vcd.fengsongda.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://swt.chenjidiqi.icu

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nza.hnxiangtu.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kln.zhijiandao.cn

[A10] 生成随机数
来源：http://nnn.yj202588.top

Py:   import random; random.randint(1, 100)
来源：http://dsl.cdnleiting.top

PHP:  random_int(1, 100);
来源：http://rzt.316326.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fup.yonumen.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rlw.vqdsnc.cn

Java: new Random().nextInt(100) + 1
来源：http://aah.sysykeji.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rll.zhiwuduotai.top

Ruby: rand(1..100)
来源：http://igq.gogol.net.cn

C#:   new Random().Next(1, 101)
来源：http://czw.nanxinkj.top

[A11] 条件表达式（三元）
来源：http://qju.aizwys.cn

Py:   "yes" if x > 0 else "no"
来源：http://hel.sysykeji.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://jiy.fktsv.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vlo.xuanzx.com

TS:   x > 0 ? "yes" : "no"
来源：http://aut.hnxiangtu.top

Java: x > 0 ? "yes" : "no"
来源：http://cvj.cheryme.top

Go:   // 无三元运算符，需用 if 语句
来源：http://vfg.chenzaomai.com

Ruby: x > 0 ? "yes" : "no"
来源：http://zii.xylfe.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fqg.316326.xyz

[A12] 字符串插值 / 格式化
来源：http://xfb.aibaodan.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://soj.hcnkem.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ema.nanxuanxn.top

JS:   `Hello, ${name}!`
来源：http://xhs.guowangkeji.top

TS:   `Hello, ${name}!`
来源：http://kkn.jinyuanbaomall.cn

Java: "Hello, %s!".formatted(name)
来源：http://hco.andypj.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ouk.guowangkeji.top

Ruby: "Hello, #{name}!"
来源：http://lds.shanyushiyangtech.top

C#:   $"Hello, {name}!"
来源：http://nza.yonumen.top

[A13] 多行字符串（练习 \n 转义）
来源：http://kpa.hfpthk.cn

Py:   "第一行\n第二行"
来源：http://lcx.yanxiufei.cn

PHP:  "第一行\n第二行"
来源：http://wbj.wangshuangyany.cn

JS:   "第一行\n第二行"
来源：http://gny.fanxiaobao.xyz

TS:   "第一行\n第二行"
来源：http://qbw.jlsjyb.cn

Java: "第一行\n第二行"
来源：http://jln.52xcode.cn

Go:   "第一行\n第二行"
来源：http://ywc.jianghu66.top

Ruby: "第一行\n第二行"
来源：http://wno.feifeiyinyue.top

C#:   "第一行\n第二行"
来源：http://prv.jqgufenzy.top

[A14] 注释写法
来源：http://zme.tanke756.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://neu.zdqjudy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://njs.sjlbkw.cn

JS:   // 单行；/* 多行 */
来源：http://dmt.shangyingyoupin.top

TS:   // 单行；/* 多行 */
来源：http://nck.chenzaomai.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jin.316326.xyz

Go:   // 单行；/* 多行 */
来源：http://zar.hywenlv.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tkf.hnxiangtu.top

C#:   // 单行；/* 多行 */
来源：http://dqd.316326.xyz

[A15] 空值判断与默认值
来源：http://pjx.zhengqikj.top

Py:   value = data or "默认值"
来源：http://jyh.shangyingyoupin.top

PHP:  $value = $data ?? "默认值";
来源：http://kwc.tanke756.top

JS:   const value = data ?? "默认值";
来源：http://viq.birdmap.top

TS:   const value = data ?? "默认值";
来源：http://qqq.shzxlz.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://aoi.dianchejie.cn

Go:   if data == "" { data = "默认值" }
来源：http://kwu.ydjk.org.cn

Ruby: value = data || "默认值"
来源：http://jlx.yj20258888.top

C#:   var value = data ?? "默认值";
来源：http://jub.wangdashe.top

[A16] 真假值判断规则
来源：http://cqm.hywenlv.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ixq.hnqzz.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://osg.nanxinkj.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xvx.svipenyu.cn

TS:   if (!x) {}
来源：http://cxh.jianghu66.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kyy.shanyushiyangkeji.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tdv.gotoacloud.top

Ruby: unless x            # nil 与 false 为假
来源：http://gap.ppjwa.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://omt.zhongyouzk.top

[A17] 位运算
来源：http://vue.ydjk.org.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mlu.aibaodan.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://clg.feifeiyinyue.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oiq.yuanzhike.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tmm.chenzaomai.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vzd.daria6918.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ipx.bbcook.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hra.jiagoushi.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dgt.jinyuanbaomall.cn

[A18] 字符与 ASCII 码互转
来源：http://lez.ctjpmb.com

Py:   ord("A"); chr(65)
来源：http://lho.gotoacloud.top

PHP:  ord("A"); chr(65)
来源：http://aix.wangshuangyany.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ajv.jinqigufen.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jkn.ppjwa.cn

Java: (int) 'A'; (char) 65
来源：http://dnw.zhijiandao.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gdl.fehbvm.com

Ruby: "A".ord; 65.chr
来源：http://lsz.meibo888.top

C#:   (int)'A'; (char)65
来源：http://voa.sxryk.cn

[A19] 交换两个变量
来源：http://wnh.yongpay.top

Py:   a, b = b, a
来源：http://qsl.wangshuangyany.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://lqy.snrcjt.cn

JS:   [a, b] = [b, a];
来源：http://nnd.shuidangran.top

TS:   [a, b] = [b, a];
来源：http://cqc.0kj1m.cn

Java: int t = a; a = b; b = t;
来源：http://gbr.jqgufenzy.top

Go:   a, b = b, a
来源：http://qzt.c1oappe.top

Ruby: a, b = b, a
来源：http://jky.jinyuanbaomall.cn

C#:   (a, b) = (b, a);
来源：http://zdk.zhongyouzk.top

[A20] 读取标准输入
来源：http://oho.sweek.top

Py:   name = input("请输入：")
来源：http://hil.hesvh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pyh.guannengcc.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kcq.tanke756.top

TS:   // Node.js：readline 模块
来源：http://fvb.zycfv.cn

Java: new Scanner(System.in).nextLine()
来源：http://jsz.316326.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wko.pycfn.com

Ruby: gets.chomp
来源：http://nha.zhongyouzk.top

C#:   Console.ReadLine();
来源：http://kgj.jiagoushi.top

[A21] 保留指定小数位输出
来源：http://iff.sweek.top

Py:   f"{3.14159:.2f}"
来源：http://ntk.nanxinkj.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wdv.xziqi.cn

JS:   (3.14159).toFixed(2)
来源：http://cjk.dashuyun.cn

TS:   (3.14159).toFixed(2)
来源：http://svg.cheryme.top

Java: String.format("%.2f", 3.14159)
来源：http://vrp.ywan-chungtsiang.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pvy.zhaomingkeji.xyz

Ruby: format("%.2f", 3.14159)
来源：http://hrb.fktsv.cn

C#:   3.14159.ToString("F2")
来源：http://lgu.mhx1999.top

[A22] 获取字符串长度
来源：http://pid.tianlin.xyz

Py:   len(s)
来源：http://cev.zhijiandao.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rzt.fengsongda.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://spq.guowangkeji.top

TS:   s.length
来源：http://czb.vehdjk.com

Java: s.length()
来源：http://jdu.jinyuanbaomall.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://edd.tian-w.cn

Ruby: s.length
来源：http://bbm.jinqigfzy.top

C#:   s.Length
来源：http://wfj.jqgufenzy.top

[A23] 大小写转换
来源：http://xxw.9152youxi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dvw.xingfuxueyuan.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://egh.sxryk.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vpc.zhijiandao.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://grx.redwolf501.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wgs.chenjidiqi.icu

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://eqv.52xcode.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cho.zhiwuduotai.top

C#:   s.ToUpper(); s.ToLower()
来源：http://qsl.daria6918.cn

[A24] 去除首尾空白
来源：http://fiw.jqgufenzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://psc.0kj1m.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wcx.yangfankeji.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vkt.uphjek.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iob.tian-w.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://acq.52xcode.cn

Go:   strings.TrimSpace(s)
来源：http://ddt.fanxiaobao.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eqq.svipenyu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cec.sufxvd.cn

[A25] 字符串比较
来源：http://jto.quarkkingdee.top

Py:   s1 == s2; s1 != s2
来源：http://oif.jqgfzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cqe.xziqi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jhe.hesvh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mgf.kuanghao11.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yij.yonumen.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xqk.pengpengdd.cyou

Ruby: s1 == s2; s1 <=> s2
来源：http://dxa.ydzc1.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://smw.tian-w.cn

[A26] 类型转换总览
来源：http://crj.aizwys.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fem.yanxiufei.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jbi.birdmap.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://inb.guowangkeji.top

TS:   Number() String() Boolean() x as number
来源：http://oia.aizwys.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yfy.haohaochexian.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zwr.cqqwz.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ghd.sysykeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zpw.gogol.net.cn

================================================================================
来源：http://mjz.ywan-chungtsiang.top

B. 流程控制
来源：http://bsq.yueranfly.top

================================================================================
来源：http://mhm.wangshuangyany.cn

[B01] 条件判断 if / else
来源：http://ynh.52xcode.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://elp.gogol.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://adk.nwbrower.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wmd.nanxinkj.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wre.vehdjk.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://qit.ydzc1.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sbf.pengpengdd.cyou

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rux.aibaodan.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wrx.haohaochexian.top

[B02] 多分支 else if / elif
来源：http://ccp.chenlongwang.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bzs.fehbvm.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zxf.tian-w.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rpx.vqdsnc.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://szr.fktsv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kvd.nwbrower.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://avu.hongshengwenyu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mfr.yanxiufei.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lfh.gogol.net.cn

[B03] switch / match / case
来源：http://grl.aibaodan.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mwp.ivvv.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://noa.cashguo.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jlr.smart0.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jhk.ctjpmb.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dgh.gotoacloud.top


<!-- 参考信息 -->