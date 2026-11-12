代发 wailian999

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nil.gogol.net.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hst.cucudq.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cfv.ywan-chungtsiang.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fwa.epnwcf.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mfk.jianghu66.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zlu.hywenlv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jfa.sxryk.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cis.guowangkeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dgb.316326.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vct.andypj.xyz

【文件统计】
来源：http://ykn.ivvv.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ooo.gaohongyu789.top

--------------------------------------------------------------------------------
来源：http://atk.yueranfly.top

目  录
来源：http://avy.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://bbj.hongshengwenyu.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://eyd.52xcode.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://knd.zhiwuduotai.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lak.cashguo.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pgh.jinghuilouyu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zag.nanxinkj.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mod.fktsv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rzp.ydzc1.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nis.smart0.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://obv.gotoacloud.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://uah.nwbrower.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jyd.chenjidiqi.icu

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dsf.hongshengwenyu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bcz.nanxuanxn.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ewv.ctjpmb.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sep.havefunace.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mis.yongpay.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jzl.dashuyun.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xpb.jiagoushi.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tny.zhaomingkeji.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uxl.bjfxy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fby.uphjek.com

================================================================================
来源：http://ihw.yangfankeji.com

A. 基础语法与类型
来源：http://wso.sjlbkw.cn

================================================================================
来源：http://dzm.xziqi.cn

[A01] Hello World
来源：http://kuj.gotoacloud.top

Py:   print("Hello, World!")
来源：http://tlf.dashuyun.cn

PHP:  echo "Hello, World!";
来源：http://icd.jinqigfzy.top

JS:   console.log("Hello, World!");
来源：http://wnz.ctjpmb.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bmp.yfazqb.com

Java: System.out.println("Hello, World!");
来源：http://qtx.kuanghao11.cn

Go:   fmt.Println("Hello, World!")
来源：http://fsy.gzhubu.top

Ruby: puts "Hello, World!"
来源：http://hbx.52xcode.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://cce.daxiang520.top

[A02] 变量声明与赋值
来源：http://pms.fehbvm.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://prm.vqdsnc.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://idb.havefunace.top

JS:   let name = "Alex"; const age = 20;
来源：http://zfi.jinghuilouyu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lub.ivvv.top

Java: String name = "Alex"; int age = 20;
来源：http://itf.zdqjudy.top

Go:   name := "Alex"; age := 20
来源：http://jmk.cdnleiting.top

Ruby: name = "Alex"; age = 20
来源：http://cdt.xingfuxueyuan.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://lqi.redwolf501.top

[A03] 常量定义
来源：http://fwl.uphjek.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dzl.cheryme.top

PHP:  const PI = 3.14159;
来源：http://pyi.ivvv.top

JS:   const PI = 3.14159;
来源：http://olq.shanyushiyangkeji.top

TS:   const PI: number = 3.14159;
来源：http://jax.hongshengwenyu.top

Java: static final double PI = 3.14159;
来源：http://xnu.xingfuxueyuan.xyz

Go:   const PI = 3.14159
来源：http://hby.xinyue.icu

Ruby: PI = 3.14159
来源：http://vxm.chenjidiqi.icu

C#:   const double PI = 3.14159;
来源：http://ubo.uphjek.com

[A04] 判断变量类型
来源：http://wox.jianghu66.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://bjq.yj202588.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zpd.yongpay.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jtk.sxryk.cn

TS:   typeof x; x instanceof Date
来源：http://dcr.sysykeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://eox.aibaodan.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pxt.ybcxt.top

Ruby: x.class; x.is_a?(Integer)
来源：http://fin.epnwcf.com

C#:   x.GetType().Name; x is int
来源：http://jtz.chenlongwang.top

[A05] 整数除法与取模
来源：http://miy.fanxiaobao.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cmh.yj202588.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://whm.ydzc1.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wgb.sysykeji.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ohy.fzhhl.top

Java: 7 / 2; 7 % 2
来源：http://vuk.jiagoushi.top

Go:   7 / 2; 7 % 2
来源：http://dph.vehdjk.com

Ruby: 7 / 2; 7 % 2
来源：http://uti.daxiang520.top

C#:   7 / 2; 7 % 2
来源：http://tof.nanxuanxn.top

[A06] 字符串转数字
来源：http://ktj.hnxiangtu.top

Py:   int("42"); float("3.14")
来源：http://knf.yj202588.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cmb.zhaomingkeji.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zwv.9152youxi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wml.sjlbkw.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://smd.gogol.net.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wjx.xuanzx.com

Ruby: "42".to_i; "3.14".to_f
来源：http://dwi.jqgufenzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://erz.andypj.xyz

[A07] 数字转字符串
来源：http://gky.shanyushiyangkeji.top

Py:   str(42)
来源：http://ton.52xcode.cn

PHP:  (string) 42; strval(42)
来源：http://pft.hesvh.cn

JS:   String(42); (42).toString()
来源：http://ouv.dashuyun.cn

TS:   String(42)
来源：http://wrt.gogol.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ydu.hnxiangtu.top

Go:   strconv.Itoa(42)
来源：http://blr.shangyingyoupin.top

Ruby: 42.to_s
来源：http://qio.hnqzz.top

C#:   42.ToString()
来源：http://cqa.daria6918.cn

[A08] 取整与四舍五入
来源：http://iwj.ehwqpu.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://igz.redwolf501.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gbg.daxiang520.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jzc.cdnleiting.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zgn.hnqzz.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jis.dashuyun.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ptg.kuanghao11.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cvu.ybcxt.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://emy.sysykeji.top

[A09] 绝对值与最大最小值
来源：http://wyx.yongpay.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://aue.yueranfly.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ojt.smart0.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bpf.meibo888.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://oem.pengpengdd.cyou

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kch.xylfe.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fex.sufxvd.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kov.gzhubu.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://frg.hammf.cn

[A10] 生成随机数
来源：http://zdb.yfazqb.com

Py:   import random; random.randint(1, 100)
来源：http://aeg.yuxming.cn

PHP:  random_int(1, 100);
来源：http://kny.shzxlz.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hom.ivvv.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kel.cdnleiting.top

Java: new Random().nextInt(100) + 1
来源：http://hdp.tianlin.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jol.xuanzx.com

Ruby: rand(1..100)
来源：http://yfh.yfazqb.com

C#:   new Random().Next(1, 101)
来源：http://zkz.cucudq.cn

[A11] 条件表达式（三元）
来源：http://qhw.xziqi.cn

Py:   "yes" if x > 0 else "no"
来源：http://pum.xingfuxueyuan.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://duj.jyoumei.cn

JS:   x > 0 ? "yes" : "no"
来源：http://cov.xuanzx.com

TS:   x > 0 ? "yes" : "no"
来源：http://yfh.feifeiyinyue.top

Java: x > 0 ? "yes" : "no"
来源：http://obx.pengpengdd.cyou

Go:   // 无三元运算符，需用 if 语句
来源：http://xmy.jlsjyb.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://iqw.vqdsnc.cn

C#:   x > 0 ? "yes" : "no"
来源：http://pmw.vehdjk.com

[A12] 字符串插值 / 格式化
来源：http://zrs.fzhhl.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mga.bbcook.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nyp.gaohongyu789.top

JS:   `Hello, ${name}!`
来源：http://avr.yj202588.top

TS:   `Hello, ${name}!`
来源：http://red.bjfxy.top

Java: "Hello, %s!".formatted(name)
来源：http://auu.jinqigfzy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vzv.sweek.top

Ruby: "Hello, #{name}!"
来源：http://hdp.hfpthk.cn

C#:   $"Hello, {name}!"
来源：http://nbj.xingfuxueyuan.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://qil.jinqigufen.top

Py:   "第一行\n第二行"
来源：http://mkd.fktsv.cn

PHP:  "第一行\n第二行"
来源：http://xja.c1oappe.top

JS:   "第一行\n第二行"
来源：http://ivg.c1oappe.top

TS:   "第一行\n第二行"
来源：http://gkg.svipenyu.cn

Java: "第一行\n第二行"
来源：http://seb.ybcxt.top

Go:   "第一行\n第二行"
来源：http://hmq.sjlbkw.cn

Ruby: "第一行\n第二行"
来源：http://wsj.yanxiufei.cn

C#:   "第一行\n第二行"
来源：http://gpt.mhx1999.top

[A14] 注释写法
来源：http://myj.yonumen.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://rkn.bbcook.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jmp.tianlin.xyz

JS:   // 单行；/* 多行 */
来源：http://lvx.zhixingplan.top

TS:   // 单行；/* 多行 */
来源：http://hpq.zycfv.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wxs.snrcjt.cn

Go:   // 单行；/* 多行 */
来源：http://zlo.gaohongyu789.top

Ruby: # 单行；=begin 多行 =end
来源：http://vnq.shuidangran.top

C#:   // 单行；/* 多行 */
来源：http://zsj.shzxlz.cn

[A15] 空值判断与默认值
来源：http://wpg.hnxiangtu.top

Py:   value = data or "默认值"
来源：http://mzp.hammf.cn

PHP:  $value = $data ?? "默认值";
来源：http://qdh.chenjidiqi.icu

JS:   const value = data ?? "默认值";
来源：http://pcg.wangshuangyany.cn

TS:   const value = data ?? "默认值";
来源：http://syb.feifeiyinyue.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ixw.cdnleiting.top

Go:   if data == "" { data = "默认值" }
来源：http://dil.c1oappe.top

Ruby: value = data || "默认值"
来源：http://yht.ydjk.org.cn

C#:   var value = data ?? "默认值";
来源：http://qxe.birdmap.top

[A16] 真假值判断规则
来源：http://kna.shuidangran.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lcz.aizwys.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wor.hfpthk.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ahl.nanxinkj.top

TS:   if (!x) {}
来源：http://vwo.mhx1999.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yhh.hcnkem.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://twp.hcnkem.com

Ruby: unless x            # nil 与 false 为假
来源：http://ccx.xylfe.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://eaf.9152youxi.cn

[A17] 位运算
来源：http://icw.cheryme.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yky.hongshengwenyu.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rmd.sweek.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mgx.tarul.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://voa.hesvh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tzn.bbcook.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ivr.yfazqb.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://osr.birdmap.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jmu.nanxinkj.top

[A18] 字符与 ASCII 码互转
来源：http://doz.cheryme.top

Py:   ord("A"); chr(65)
来源：http://ohk.chenjidiqi.icu

PHP:  ord("A"); chr(65)
来源：http://esq.jinghuilouyu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mvw.chenjidiqi.icu

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://heb.ctjpmb.com

Java: (int) 'A'; (char) 65
来源：http://gas.chenjidiqi.icu

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zjl.yuxming.cn

Ruby: "A".ord; 65.chr
来源：http://kpd.iojbl.cn

C#:   (int)'A'; (char)65
来源：http://lnv.meibo888.top

[A19] 交换两个变量
来源：http://ksx.haohaochexian.top

Py:   a, b = b, a
来源：http://uyq.mhx1999.top

PHP:  [$a, $b] = [$b, $a];
来源：http://efy.jqgfzy.top

JS:   [a, b] = [b, a];
来源：http://ond.ydzc1.top

TS:   [a, b] = [b, a];
来源：http://hld.hysaishi.cn

Java: int t = a; a = b; b = t;
来源：http://vim.wangdashe.top

Go:   a, b = b, a
来源：http://ffu.nanxinkj.top

Ruby: a, b = b, a
来源：http://gmt.sxryk.cn

C#:   (a, b) = (b, a);
来源：http://kso.cheryme.top

[A20] 读取标准输入
来源：http://cwg.hesvh.cn

Py:   name = input("请输入：")
来源：http://czp.jqgfzy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ekn.xuanzx.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mat.yj202588.top

TS:   // Node.js：readline 模块
来源：http://eqk.pengpengdd.cyou

Java: new Scanner(System.in).nextLine()
来源：http://vgq.bjfxy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kut.meibo888.top

Ruby: gets.chomp
来源：http://idr.tian-w.cn

C#:   Console.ReadLine();
来源：http://dwx.yongpay.top

[A21] 保留指定小数位输出
来源：http://kzh.pengpengdd.cyou

Py:   f"{3.14159:.2f}"
来源：http://zgq.meibo888.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vgq.cashguo.top

JS:   (3.14159).toFixed(2)
来源：http://ano.ydzc1.top

TS:   (3.14159).toFixed(2)
来源：http://lrg.jiagoushi.top

Java: String.format("%.2f", 3.14159)
来源：http://bph.zhoulong.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tic.pycfn.com

Ruby: format("%.2f", 3.14159)
来源：http://mre.redwolf501.top

C#:   3.14159.ToString("F2")
来源：http://scw.tianlin.xyz

[A22] 获取字符串长度
来源：http://lsy.fktsv.cn

Py:   len(s)
来源：http://evc.c1oappe.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sio.smart0.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lpx.smart0.xyz

TS:   s.length
来源：http://zgz.mhx1999.top

Java: s.length()
来源：http://rig.0kj1m.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://opk.ywan-chungtsiang.top

Ruby: s.length
来源：http://zxa.wangdashe.top

C#:   s.Length
来源：http://eeq.yuanzhike.top

[A23] 大小写转换
来源：http://kaf.xuanzx.com

Py:   s.upper(); s.lower(); s.title()
来源：http://xgk.mhx1999.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hce.jianghu66.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ayz.ybcxt.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lez.yongpay.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mxi.aizwys.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hyq.cdnleiting.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://orx.yuxming.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://adr.ctjpmb.com

[A24] 去除首尾空白
来源：http://wni.jinyuanbaomall.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://oqd.xuetiantiany.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hat.hnxiangtu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sfp.tianlin.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ajh.zhijiandao.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ekj.jinyuanbaomall.cn

Go:   strings.TrimSpace(s)
来源：http://tpd.iojbl.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nui.yj202588.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jpz.yfazqb.com

[A25] 字符串比较
来源：http://llc.hcnkem.com

Py:   s1 == s2; s1 != s2
来源：http://dlm.zdqjudy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yjj.zhongyouzk.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jlm.sxryk.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fut.gogol.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://npu.zhengqikj.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fsr.hongshengwenyu.top

Ruby: s1 == s2; s1 <=> s2
来源：http://qdf.svipenyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fls.hnxiangtu.top

[A26] 类型转换总览
来源：http://pry.nanxinkj.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://iuf.hnxiangtu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vhp.zhengqikj.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fgx.zhixingplan.top

TS:   Number() String() Boolean() x as number
来源：http://ntf.zhixingplan.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xad.havefunace.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wsy.jlsjyb.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kar.c1oappe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://niu.ydjk.org.cn

================================================================================
来源：http://hlz.xinyue.icu

B. 流程控制
来源：http://kkj.hesvh.cn

================================================================================
来源：http://ywa.zhiwuduotai.top

[B01] 条件判断 if / else
来源：http://fqr.xuanzx.com

Py:   result = "正" if x > 0 else "非正"
来源：http://kpl.0kj1m.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pcm.jyoumei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cyr.cucudq.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wfy.dashuyun.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dxv.jqgfzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gam.haohaochexian.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jwe.mhx1999.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rrv.mhx1999.top

[B02] 多分支 else if / elif
来源：http://vuj.xziqi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lcn.daria6918.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cqc.xylfe.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rxr.nanxinkj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qpf.hesvh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uad.xinyue.icu

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://obj.jianghu66.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vgn.ydjk.org.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hll.yuxming.cn

[B03] switch / match / case
来源：http://mey.jiagoushi.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qgl.chenzaomai.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://seg.havefunace.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bdz.uphjek.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rlk.pycfn.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rci.shzxlz.cn


<!-- 参考信息 -->