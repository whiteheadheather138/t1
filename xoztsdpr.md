代发 wailian999

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wcj.ehwqpu.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://aqq.yanxiufei.cn

【文件统计】
来源：http://zat.zycfv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://poc.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://sgi.xylfe.cn

目  录
来源：http://igv.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://xja.chenjidiqi.icu

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rmk.bjfxy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://son.jlsjyb.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wox.hongshengwenyu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ttz.chenjidiqi.icu

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://siu.cheryme.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://eba.c1oappe.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vga.cqqwz.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pcc.andypj.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rua.chenjidiqi.icu

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hny.chenzaomai.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fga.jlsjyb.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ymp.sufxvd.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fgg.jyoumei.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dzz.yuxming.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jde.fehbvm.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://afs.hnxiangtu.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tqm.yj20258.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://uny.daxiang520.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tro.zhiwuduotai.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://osr.yj20258.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xkl.andypj.xyz

================================================================================
来源：http://ovd.sjlbkw.cn

A. 基础语法与类型
来源：http://jfa.zdbjq.cn

================================================================================
来源：http://qwf.chenzaomai.com

[A01] Hello World
来源：http://pgl.ydjk.org.cn

Py:   print("Hello, World!")
来源：http://pti.xuanzx.com

PHP:  echo "Hello, World!";
来源：http://jyz.sjlbkw.cn

JS:   console.log("Hello, World!");
来源：http://gum.wangdashe.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://eno.jlsjyb.cn

Java: System.out.println("Hello, World!");
来源：http://kah.birdmap.top

Go:   fmt.Println("Hello, World!")
来源：http://zqy.yanxiufei.cn

Ruby: puts "Hello, World!"
来源：http://wgd.fktsv.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sqh.guowangkeji.top

[A02] 变量声明与赋值
来源：http://bgn.vehdjk.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mcc.fengsongda.top

PHP:  $name = "Alex"; $age = 20;
来源：http://hwt.hcnkem.com

JS:   let name = "Alex"; const age = 20;
来源：http://wno.havefunace.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ety.hongshengwenyu.top

Java: String name = "Alex"; int age = 20;
来源：http://ihk.wangdashe.top

Go:   name := "Alex"; age := 20
来源：http://ekz.fanxiaobao.xyz

Ruby: name = "Alex"; age = 20
来源：http://pzk.meibo888.top

C#:   string name = "Alex"; int age = 20;
来源：http://ggv.shuidangran.top

[A03] 常量定义
来源：http://hyo.cdnleiting.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bls.aibaodan.cn

PHP:  const PI = 3.14159;
来源：http://bjk.yonumen.top

JS:   const PI = 3.14159;
来源：http://huh.hnxiangtu.top

TS:   const PI: number = 3.14159;
来源：http://qop.snrcjt.cn

Java: static final double PI = 3.14159;
来源：http://oaw.xuanzx.com

Go:   const PI = 3.14159
来源：http://hml.ywan-chungtsiang.top

Ruby: PI = 3.14159
来源：http://mpk.yuanzhike.top

C#:   const double PI = 3.14159;
来源：http://lyq.daxiang520.top

[A04] 判断变量类型
来源：http://zqt.zhongyouzk.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ssw.jiagoushi.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fuk.chenzaomai.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cen.kuanghao11.cn

TS:   typeof x; x instanceof Date
来源：http://zoc.daria6918.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://udn.jianghu66.top

Go:   reflect.TypeOf(x).Name()
来源：http://swb.uphjek.com

Ruby: x.class; x.is_a?(Integer)
来源：http://fsz.c1oappe.top

C#:   x.GetType().Name; x is int
来源：http://rql.epnwcf.com

[A05] 整数除法与取模
来源：http://gut.aibaodan.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://oxd.yfazqb.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://uoa.chenlongwang.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://edx.yvedp.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vjs.fanxiaobao.xyz

Java: 7 / 2; 7 % 2
来源：http://icr.zhengqikj.top

Go:   7 / 2; 7 % 2
来源：http://egd.ydjk.org.cn

Ruby: 7 / 2; 7 % 2
来源：http://fyi.wangshuangyany.cn

C#:   7 / 2; 7 % 2
来源：http://tdn.aibaodan.cn

[A06] 字符串转数字
来源：http://uhp.guannengcc.top

Py:   int("42"); float("3.14")
来源：http://ahs.sufxvd.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vwe.zhongyouzk.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kvw.epnwcf.com

TS:   parseInt("42", 10); Number("42")
来源：http://kdx.c1oappe.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vrz.shangyingyoupin.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lhg.dianchejie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zei.zhixingplan.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://eje.hnqzz.top

[A07] 数字转字符串
来源：http://tkc.xuanzx.com

Py:   str(42)
来源：http://xno.hesvh.cn

PHP:  (string) 42; strval(42)
来源：http://mnm.quarkkingdee.top

JS:   String(42); (42).toString()
来源：http://ohj.sjlbkw.cn

TS:   String(42)
来源：http://siy.fehbvm.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://isf.jqgufenzy.top

Go:   strconv.Itoa(42)
来源：http://ucz.haohaochexian.top

Ruby: 42.to_s
来源：http://rab.jiagoushi.top

C#:   42.ToString()
来源：http://hkt.iojbl.cn

[A08] 取整与四舍五入
来源：http://quh.ivvv.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://teu.jqgufenzy.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://agh.sxryk.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ezq.hysaishi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sdh.yuanzhike.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tgs.ivvv.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://eru.xinyue.icu

Ruby: 3.567.round(2); 3.9.floor
来源：http://bhq.aibaodan.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cps.shuidangran.top

[A09] 绝对值与最大最小值
来源：http://nqf.chenzaomai.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://goj.meibo888.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wvi.hesvh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hrb.sjlbkw.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mbv.jiagoushi.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uiz.jyoumei.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ktx.yfazqb.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pap.xinyue.icu

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yny.ywan-chungtsiang.top

[A10] 生成随机数
来源：http://pnl.yanxiufei.cn

Py:   import random; random.randint(1, 100)
来源：http://qfj.havefunace.top

PHP:  random_int(1, 100);
来源：http://jlr.xuanzx.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qsj.chenzaomai.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xkz.jqgfzy.top

Java: new Random().nextInt(100) + 1
来源：http://smq.dianchejie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wes.wangdashe.top

Ruby: rand(1..100)
来源：http://xwq.yanxiufei.cn

C#:   new Random().Next(1, 101)
来源：http://dfd.fanxiaobao.xyz

[A11] 条件表达式（三元）
来源：http://gds.pycfn.com

Py:   "yes" if x > 0 else "no"
来源：http://fqk.yj20258888.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://mce.uphjek.com

JS:   x > 0 ? "yes" : "no"
来源：http://twn.tianlin.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://fnh.dianchejie.cn

Java: x > 0 ? "yes" : "no"
来源：http://pdi.ivvv.top

Go:   // 无三元运算符，需用 if 语句
来源：http://hvf.cashguo.top

Ruby: x > 0 ? "yes" : "no"
来源：http://pwc.hnxiangtu.top

C#:   x > 0 ? "yes" : "no"
来源：http://thx.jianghu66.top

[A12] 字符串插值 / 格式化
来源：http://agw.cdnleiting.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gzt.jqgufenzy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wsf.jqgufenzy.top

JS:   `Hello, ${name}!`
来源：http://rkz.havefunace.top

TS:   `Hello, ${name}!`
来源：http://vkw.sysykeji.top

Java: "Hello, %s!".formatted(name)
来源：http://ggn.pycfn.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xkw.aizwys.cn

Ruby: "Hello, #{name}!"
来源：http://hld.gzhubu.top

C#:   $"Hello, {name}!"
来源：http://cdf.hywenlv.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://kvu.yvedp.cn

Py:   "第一行\n第二行"
来源：http://wrh.cdnleiting.top

PHP:  "第一行\n第二行"
来源：http://ong.smart0.xyz

JS:   "第一行\n第二行"
来源：http://sxk.ydzc1.top

TS:   "第一行\n第二行"
来源：http://caw.hnxiangtu.top

Java: "第一行\n第二行"
来源：http://erq.fanxiaobao.xyz

Go:   "第一行\n第二行"
来源：http://kae.zhixingplan.top

Ruby: "第一行\n第二行"
来源：http://owl.cashguo.top

C#:   "第一行\n第二行"
来源：http://vvf.ydzc1.top

[A14] 注释写法
来源：http://wfp.tian-w.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://buv.yj20258.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://awn.jqgfzy.top

JS:   // 单行；/* 多行 */
来源：http://bgd.hnxiangtu.top

TS:   // 单行；/* 多行 */
来源：http://zqa.316326.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dxr.zhoulong.xyz

Go:   // 单行；/* 多行 */
来源：http://uzc.yj20258.top

Ruby: # 单行；=begin 多行 =end
来源：http://nxc.ivvv.top

C#:   // 单行；/* 多行 */
来源：http://fgy.dianchejie.cn

[A15] 空值判断与默认值
来源：http://taw.cheryme.top

Py:   value = data or "默认值"
来源：http://vts.svipenyu.cn

PHP:  $value = $data ?? "默认值";
来源：http://tqt.jqgfzy.top

JS:   const value = data ?? "默认值";
来源：http://lio.cdnleiting.top

TS:   const value = data ?? "默认值";
来源：http://ito.ydjk.org.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mty.hysaishi.cn

Go:   if data == "" { data = "默认值" }
来源：http://zgg.xziqi.cn

Ruby: value = data || "默认值"
来源：http://dbr.shanyushiyangkeji.top

C#:   var value = data ?? "默认值";
来源：http://bxn.pengpengdd.cyou

[A16] 真假值判断规则
来源：http://upa.jqgufenzy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xvm.hcnkem.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qvn.hysaishi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lmu.feifeiyinyue.top

TS:   if (!x) {}
来源：http://npo.xylfe.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uyw.cheryme.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rxg.fanxiaobao.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://dmw.vehdjk.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wvt.zdbjq.cn

[A17] 位运算
来源：http://wmh.hnxiangtu.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mme.feifeiyinyue.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gej.fengsongda.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bgx.ppjwa.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uxj.sysykeji.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://phw.guowangkeji.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://htz.gzhubu.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zoe.52xcode.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xxr.sjlbkw.cn

[A18] 字符与 ASCII 码互转
来源：http://nyd.fzhhl.top

Py:   ord("A"); chr(65)
来源：http://gac.fengsongda.top

PHP:  ord("A"); chr(65)
来源：http://oob.wangdashe.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mpw.fehbvm.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oon.zhoulong.xyz

Java: (int) 'A'; (char) 65
来源：http://pnm.zhongyouzk.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ptr.bbcook.cn

Ruby: "A".ord; 65.chr
来源：http://yhv.guannengcc.top

C#:   (int)'A'; (char)65
来源：http://fnd.hywenlv.cn

[A19] 交换两个变量
来源：http://kct.guowangkeji.top

Py:   a, b = b, a
来源：http://vje.zhongyouzk.top

PHP:  [$a, $b] = [$b, $a];
来源：http://evu.jyoumei.cn

JS:   [a, b] = [b, a];
来源：http://fok.hywenlv.cn

TS:   [a, b] = [b, a];
来源：http://jov.ehwqpu.com

Java: int t = a; a = b; b = t;
来源：http://ebe.jqgfzy.top

Go:   a, b = b, a
来源：http://ynd.xingfuxueyuan.xyz

Ruby: a, b = b, a
来源：http://ryp.mhx1999.top

C#:   (a, b) = (b, a);
来源：http://jfd.jqgfzy.top

[A20] 读取标准输入
来源：http://jzx.jyoumei.cn

Py:   name = input("请输入：")
来源：http://xea.cdnleiting.top

PHP:  $name = trim(fgets(STDIN));
来源：http://wfp.redwolf501.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zvd.daxiang520.top

TS:   // Node.js：readline 模块
来源：http://hkz.jianghu66.top

Java: new Scanner(System.in).nextLine()
来源：http://ssg.vehdjk.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://afj.nanxinkj.top

Ruby: gets.chomp
来源：http://pfo.fzhhl.top

C#:   Console.ReadLine();
来源：http://ben.daria6918.cn

[A21] 保留指定小数位输出
来源：http://cxe.svipenyu.cn

Py:   f"{3.14159:.2f}"
来源：http://lev.jiagoushi.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ceu.havefunace.top

JS:   (3.14159).toFixed(2)
来源：http://dpe.xinyue.icu

TS:   (3.14159).toFixed(2)
来源：http://mcc.zhaomingkeji.xyz

Java: String.format("%.2f", 3.14159)
来源：http://hum.sysykeji.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pbt.shzxlz.cn

Ruby: format("%.2f", 3.14159)
来源：http://obq.nwbrower.top

C#:   3.14159.ToString("F2")
来源：http://ymp.birdmap.top

[A22] 获取字符串长度
来源：http://aqz.hnxiangtu.top

Py:   len(s)
来源：http://rqk.zhoulong.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zrc.zhongyouzk.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sxx.shuidangran.top

TS:   s.length
来源：http://qoq.ctjpmb.com

Java: s.length()
来源：http://guv.smart0.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://txi.hnqzz.top

Ruby: s.length
来源：http://qdh.sxryk.cn

C#:   s.Length
来源：http://wlv.jyoumei.cn

[A23] 大小写转换
来源：http://ycy.birdmap.top

Py:   s.upper(); s.lower(); s.title()
来源：http://zsu.kuanghao11.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yuv.yj202588.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dpx.kuanghao11.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pii.daria6918.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yen.ywan-chungtsiang.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hcj.ppjwa.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zys.vehdjk.com

C#:   s.ToUpper(); s.ToLower()
来源：http://pqm.9152youxi.cn

[A24] 去除首尾空白
来源：http://ojt.ehwqpu.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rhk.haohaochexian.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://huu.316326.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ofe.zycfv.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qzu.gotoacloud.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jqk.xinyue.icu

Go:   strings.TrimSpace(s)
来源：http://ktj.yfazqb.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://psh.zhixingplan.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jyb.sufxvd.cn

[A25] 字符串比较
来源：http://odq.epnwcf.com

Py:   s1 == s2; s1 != s2
来源：http://owf.bjfxy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://deo.tanke756.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kxl.yanxiufei.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gsb.zhaomingkeji.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ksj.bjfxy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://eed.sjlbkw.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gdr.shangyingyoupin.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oth.mhx1999.top

[A26] 类型转换总览
来源：http://nxs.yongpay.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jug.cqqwz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bil.fzhhl.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wez.hfpthk.cn

TS:   Number() String() Boolean() x as number
来源：http://qxs.shuidangran.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pmx.sjlbkw.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gqb.ehwqpu.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://etd.shzxlz.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vfr.redwolf501.top

================================================================================
来源：http://pjc.nanxinkj.top

B. 流程控制
来源：http://dpw.guowangkeji.top

================================================================================
来源：http://njx.aibaodan.cn

[B01] 条件判断 if / else
来源：http://aea.xuanzx.com

Py:   result = "正" if x > 0 else "非正"
来源：http://wfs.nanxuanxn.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wme.cqqwz.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://aha.smart0.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ebm.shzxlz.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cwi.yanxiufei.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fnz.ppjwa.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://opf.zhoulong.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://oka.gotoacloud.top

[B02] 多分支 else if / elif
来源：http://wzp.zycfv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kws.gotoacloud.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://suj.ctjpmb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://owo.bjfxy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eyl.hysaishi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mdi.jinqigufen.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://txz.hcnkem.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qec.xuetiantiany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pra.nwbrower.top

[B03] switch / match / case
来源：http://ujo.jinqigfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yqs.sysykeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vwe.zdbjq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uwc.jinqigufen.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kzh.shangyingyoupin.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gxd.yangfankeji.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iep.gogol.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dds.zhongyouzk.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ihm.yj20258888.top

[B04] for 计数循环
来源：http://mzq.ybcxt.top

Py:   for i in range(10): print(i)
来源：http://ypu.zdbjq.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jgn.cqqwz.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vtr.mhx1999.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zgv.nanxuanxn.top


<!-- 参考信息 -->