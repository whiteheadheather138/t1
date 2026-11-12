代发 wailian999

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xat.iojbl.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://apg.andypj.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bdc.jinqigfzy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://skb.xziqi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wmk.cheryme.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fmb.zycfv.cn

【文件统计】
来源：http://otf.jyoumei.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sle.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://fbz.hysaishi.cn

目  录
来源：http://iel.nwbrower.top

--------------------------------------------------------------------------------
来源：http://tze.nanxinkj.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qks.sjlbkw.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://iyh.hesvh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jld.xuetiantiany.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kuf.jqgfzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jcz.gotoacloud.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kuf.hysaishi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sgb.daxiang520.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ion.ydjk.org.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wqy.zhiwuduotai.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://eoj.iojbl.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lbc.iojbl.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ewx.jinyuanbaomall.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ksr.yfazqb.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://opv.smart0.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://oez.shzxlz.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://frz.ybcxt.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rik.xylfe.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://eqg.316326.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://voc.pycfn.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zto.jiagoushi.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mfs.hongshengwenyu.top

================================================================================
来源：http://mvz.sjlbkw.cn

A. 基础语法与类型
来源：http://mfr.yj202588.top

================================================================================
来源：http://tuk.316326.xyz

[A01] Hello World
来源：http://lip.cashguo.top

Py:   print("Hello, World!")
来源：http://lzn.zhiwuduotai.top

PHP:  echo "Hello, World!";
来源：http://uaz.xingfuxueyuan.xyz

JS:   console.log("Hello, World!");
来源：http://hme.mhx1999.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xek.gzhubu.top

Java: System.out.println("Hello, World!");
来源：http://ptj.ydzc1.top

Go:   fmt.Println("Hello, World!")
来源：http://wil.shangyingyoupin.top

Ruby: puts "Hello, World!"
来源：http://gnm.yj20258888.top

C#:   Console.WriteLine("Hello, World!");
来源：http://opo.yueranfly.top

[A02] 变量声明与赋值
来源：http://pul.hfpthk.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xkm.jinqigfzy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://kmb.xziqi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qfm.pengpengdd.cyou

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zpb.quarkkingdee.top

Java: String name = "Alex"; int age = 20;
来源：http://bdn.jqgfzy.top

Go:   name := "Alex"; age := 20
来源：http://ghn.fktsv.cn

Ruby: name = "Alex"; age = 20
来源：http://sol.nwbrower.top

C#:   string name = "Alex"; int age = 20;
来源：http://vxv.snrcjt.cn

[A03] 常量定义
来源：http://smt.52xcode.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yzi.kuanghao11.cn

PHP:  const PI = 3.14159;
来源：http://jir.birdmap.top

JS:   const PI = 3.14159;
来源：http://upy.jqgfzy.top

TS:   const PI: number = 3.14159;
来源：http://qam.hesvh.cn

Java: static final double PI = 3.14159;
来源：http://uyc.ehwqpu.com

Go:   const PI = 3.14159
来源：http://qll.yueranfly.top

Ruby: PI = 3.14159
来源：http://mzr.vehdjk.com

C#:   const double PI = 3.14159;
来源：http://jrg.fanxiaobao.xyz

[A04] 判断变量类型
来源：http://tec.yangfankeji.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://lwr.sjlbkw.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bgy.shzxlz.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zab.meibo888.top

TS:   typeof x; x instanceof Date
来源：http://kyv.fzhhl.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rla.zhijiandao.cn

Go:   reflect.TypeOf(x).Name()
来源：http://efj.daxiang520.top

Ruby: x.class; x.is_a?(Integer)
来源：http://xpg.cheryme.top

C#:   x.GetType().Name; x is int
来源：http://izf.hfpthk.cn

[A05] 整数除法与取模
来源：http://ppx.birdmap.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://obh.cqqwz.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ogx.epnwcf.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wfz.fanxiaobao.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vgg.mhx1999.top

Java: 7 / 2; 7 % 2
来源：http://zdb.nwbrower.top

Go:   7 / 2; 7 % 2
来源：http://jof.xziqi.cn

Ruby: 7 / 2; 7 % 2
来源：http://kwj.dashuyun.cn

C#:   7 / 2; 7 % 2
来源：http://umi.hcnkem.com

[A06] 字符串转数字
来源：http://zdl.zhaomingkeji.xyz

Py:   int("42"); float("3.14")
来源：http://kqu.tianlin.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://roy.yongpay.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vod.birdmap.top

TS:   parseInt("42", 10); Number("42")
来源：http://efg.tian-w.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ftj.mhx1999.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://osj.uphjek.com

Ruby: "42".to_i; "3.14".to_f
来源：http://gqj.jinghuilouyu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xej.jinyuanbaomall.cn

[A07] 数字转字符串
来源：http://sas.9152youxi.cn

Py:   str(42)
来源：http://tbi.yonumen.top

PHP:  (string) 42; strval(42)
来源：http://yfe.pycfn.com

JS:   String(42); (42).toString()
来源：http://ijn.yfazqb.com

TS:   String(42)
来源：http://ckf.sjlbkw.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bar.sufxvd.cn

Go:   strconv.Itoa(42)
来源：http://hlm.pycfn.com

Ruby: 42.to_s
来源：http://qnf.svipenyu.cn

C#:   42.ToString()
来源：http://xcp.gotoacloud.top

[A08] 取整与四舍五入
来源：http://blk.hesvh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rko.hysaishi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ztv.ivvv.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ret.hnqzz.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://huw.dashuyun.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://edr.ivvv.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://veh.zhongyouzk.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://jca.yanxiufei.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jad.hammf.cn

[A09] 绝对值与最大最小值
来源：http://gqz.shanyushiyangtech.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hwt.sjlbkw.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://evm.hysaishi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://swy.9152youxi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qsh.iojbl.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gpk.c1oappe.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://uaf.shanyushiyangtech.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://coq.dianchejie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gla.cucudq.cn

[A10] 生成随机数
来源：http://qxr.xingfuxueyuan.xyz

Py:   import random; random.randint(1, 100)
来源：http://dxo.hysaishi.cn

PHP:  random_int(1, 100);
来源：http://uqm.ybcxt.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yvi.gaohongyu789.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ixn.chenjidiqi.icu

Java: new Random().nextInt(100) + 1
来源：http://osx.vehdjk.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wlg.snrcjt.cn

Ruby: rand(1..100)
来源：http://miz.ywan-chungtsiang.top

C#:   new Random().Next(1, 101)
来源：http://hlh.guannengcc.top

[A11] 条件表达式（三元）
来源：http://vem.uphjek.com

Py:   "yes" if x > 0 else "no"
来源：http://qqn.shanyushiyangtech.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://rxx.gzhubu.top

JS:   x > 0 ? "yes" : "no"
来源：http://nte.zhoulong.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://ibd.mhx1999.top

Java: x > 0 ? "yes" : "no"
来源：http://eeo.xuanzx.com

Go:   // 无三元运算符，需用 if 语句
来源：http://bqp.jianghu66.top

Ruby: x > 0 ? "yes" : "no"
来源：http://jyz.iojbl.cn

C#:   x > 0 ? "yes" : "no"
来源：http://jnq.hesvh.cn

[A12] 字符串插值 / 格式化
来源：http://mhs.fzhhl.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://duz.jianghu66.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cky.yongpay.top

JS:   `Hello, ${name}!`
来源：http://awq.hfpthk.cn

TS:   `Hello, ${name}!`
来源：http://srn.ehwqpu.com

Java: "Hello, %s!".formatted(name)
来源：http://udl.meibo888.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zko.xingfuxueyuan.xyz

Ruby: "Hello, #{name}!"
来源：http://lyv.ywan-chungtsiang.top

C#:   $"Hello, {name}!"
来源：http://wsn.zhoulong.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://aoy.bjfxy.top

Py:   "第一行\n第二行"
来源：http://fez.xziqi.cn

PHP:  "第一行\n第二行"
来源：http://ltt.shzxlz.cn

JS:   "第一行\n第二行"
来源：http://ufn.bjfxy.top

TS:   "第一行\n第二行"
来源：http://vfz.gzhubu.top

Java: "第一行\n第二行"
来源：http://jup.zdqjudy.top

Go:   "第一行\n第二行"
来源：http://enn.zhaomingkeji.xyz

Ruby: "第一行\n第二行"
来源：http://ctf.fehbvm.com

C#:   "第一行\n第二行"
来源：http://pjg.iojbl.cn

[A14] 注释写法
来源：http://hxk.jinghuilouyu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ojj.ydjk.org.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wpc.jinqigufen.top

JS:   // 单行；/* 多行 */
来源：http://kco.mhx1999.top

TS:   // 单行；/* 多行 */
来源：http://fof.mhx1999.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zco.52xcode.cn

Go:   // 单行；/* 多行 */
来源：http://lge.xuetiantiany.cn

Ruby: # 单行；=begin 多行 =end
来源：http://owk.9152youxi.cn

C#:   // 单行；/* 多行 */
来源：http://lze.mhx1999.top

[A15] 空值判断与默认值
来源：http://skj.fanxiaobao.xyz

Py:   value = data or "默认值"
来源：http://glq.zhiwuduotai.top

PHP:  $value = $data ?? "默认值";
来源：http://wtp.nanxuanxn.top

JS:   const value = data ?? "默认值";
来源：http://dfu.gzhubu.top

TS:   const value = data ?? "默认值";
来源：http://aik.hammf.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jiu.shanyushiyangtech.top

Go:   if data == "" { data = "默认值" }
来源：http://rdl.yj20258.top

Ruby: value = data || "默认值"
来源：http://xgy.zdqjudy.top

C#:   var value = data ?? "默认值";
来源：http://ith.gzhubu.top

[A16] 真假值判断规则
来源：http://grz.fzhhl.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xhs.bbcook.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://psp.xuetiantiany.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zoj.ydjk.org.cn

TS:   if (!x) {}
来源：http://ccz.cheryme.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vrl.jinyuanbaomall.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://boi.jqgfzy.top

Ruby: unless x            # nil 与 false 为假
来源：http://kyq.quarkkingdee.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vio.ivvv.top

[A17] 位运算
来源：http://xzb.sxryk.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://riz.smart0.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://git.hysaishi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ldb.yj202588.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cqo.epnwcf.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ngg.zhongyouzk.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yyj.jqgfzy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xos.chenlongwang.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pkj.haohaochexian.top

[A18] 字符与 ASCII 码互转
来源：http://ige.xingfuxueyuan.xyz

Py:   ord("A"); chr(65)
来源：http://ulp.dianchejie.cn

PHP:  ord("A"); chr(65)
来源：http://ljo.yanxiufei.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jiy.zhiwuduotai.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jyq.chenzaomai.com

Java: (int) 'A'; (char) 65
来源：http://hch.hywenlv.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gzt.xinyue.icu

Ruby: "A".ord; 65.chr
来源：http://nnl.sjlbkw.cn

C#:   (int)'A'; (char)65
来源：http://mbk.jinghuilouyu.cn

[A19] 交换两个变量
来源：http://sei.ehwqpu.com

Py:   a, b = b, a
来源：http://ggd.hywenlv.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://kfc.wangdashe.top

JS:   [a, b] = [b, a];
来源：http://kab.hammf.cn

TS:   [a, b] = [b, a];
来源：http://vkd.sysykeji.top

Java: int t = a; a = b; b = t;
来源：http://gey.cashguo.top

Go:   a, b = b, a
来源：http://yoc.snrcjt.cn

Ruby: a, b = b, a
来源：http://clz.yangfankeji.com

C#:   (a, b) = (b, a);
来源：http://kwc.sysykeji.top

[A20] 读取标准输入
来源：http://aid.bjfxy.top

Py:   name = input("请输入：")
来源：http://hmk.yj20258888.top

PHP:  $name = trim(fgets(STDIN));
来源：http://gos.guowangkeji.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wqf.shangyingyoupin.top

TS:   // Node.js：readline 模块
来源：http://inm.jiagoushi.top

Java: new Scanner(System.in).nextLine()
来源：http://mqz.zhengqikj.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nmf.sufxvd.cn

Ruby: gets.chomp
来源：http://vsh.shuidangran.top

C#:   Console.ReadLine();
来源：http://klb.zhijiandao.cn

[A21] 保留指定小数位输出
来源：http://dsa.cucudq.cn

Py:   f"{3.14159:.2f}"
来源：http://rsl.zhijiandao.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://iko.jiagoushi.top

JS:   (3.14159).toFixed(2)
来源：http://lmq.hnqzz.top

TS:   (3.14159).toFixed(2)
来源：http://xzv.chenzaomai.com

Java: String.format("%.2f", 3.14159)
来源：http://cyj.cdnleiting.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xwn.xuetiantiany.cn

Ruby: format("%.2f", 3.14159)
来源：http://nrb.chenzaomai.com

C#:   3.14159.ToString("F2")
来源：http://xjx.hywenlv.cn

[A22] 获取字符串长度
来源：http://arj.andypj.xyz

Py:   len(s)
来源：http://geb.0kj1m.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yrg.meibo888.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jyu.c1oappe.top

TS:   s.length
来源：http://xak.xuetiantiany.cn

Java: s.length()
来源：http://grk.hnxiangtu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vjb.yj20258888.top

Ruby: s.length
来源：http://boo.meibo888.top

C#:   s.Length
来源：http://bph.guannengcc.top

[A23] 大小写转换
来源：http://etb.daxiang520.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ojl.wangshuangyany.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://smr.nanxinkj.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uzb.0kj1m.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kfu.hfpthk.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://olz.yongpay.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ebb.yueranfly.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bdb.zhijiandao.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://icd.yuxming.cn

[A24] 去除首尾空白
来源：http://vrc.ywan-chungtsiang.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ron.hnqzz.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://slp.c1oappe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jgn.jqgfzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lsa.jinyuanbaomall.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mly.birdmap.top

Go:   strings.TrimSpace(s)
来源：http://jcg.jinghuilouyu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mxy.sysykeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://drw.zhoulong.xyz

[A25] 字符串比较
来源：http://pgu.haohaochexian.top

Py:   s1 == s2; s1 != s2
来源：http://fsy.zhaomingkeji.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pwd.sweek.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://odk.cdnleiting.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vvn.jiagoushi.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://suf.jianghu66.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bpj.shanyushiyangkeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://caf.aibaodan.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vac.shuidangran.top

[A26] 类型转换总览
来源：http://lua.jianghu66.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qwk.zhoulong.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://auq.shanyushiyangtech.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cyv.vqdsnc.cn

TS:   Number() String() Boolean() x as number
来源：http://zvo.fengsongda.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ueu.ppjwa.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tuk.jinqigfzy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ggv.yonumen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jqk.xuetiantiany.cn

================================================================================
来源：http://msd.yangfankeji.com

B. 流程控制
来源：http://sjf.sysykeji.top

================================================================================
来源：http://gct.kuanghao11.cn

[B01] 条件判断 if / else
来源：http://jdc.wangdashe.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ihk.meibo888.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://edx.bjfxy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://saj.feifeiyinyue.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://huz.xingfuxueyuan.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://chq.chenzaomai.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rth.meibo888.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sdn.yangfankeji.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://aap.zhixingplan.top

[B02] 多分支 else if / elif
来源：http://nlg.wangdashe.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uzk.wangshuangyany.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://knx.aibaodan.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bhu.daxiang520.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uzw.zycfv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sjc.zhixingplan.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mcb.hesvh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uaq.hnqzz.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yye.xylfe.cn

[B03] switch / match / case
来源：http://qhy.haohaochexian.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vag.zhixingplan.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iei.zhoulong.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nze.sxryk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ugn.yj20258.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pch.guannengcc.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pyn.mhx1999.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oxp.cucudq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gyv.cucudq.cn

[B04] for 计数循环
来源：http://xma.yanxiufei.cn


<!-- 参考信息 -->