代发 wailian999

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://syg.tian-w.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://isp.sjlbkw.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://efg.gzhubu.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pxg.aizwys.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jke.ehwqpu.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://okj.hywenlv.cn

【文件统计】
来源：http://fng.svipenyu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tes.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://vzl.vqdsnc.cn

目  录
来源：http://cdx.cheryme.top

--------------------------------------------------------------------------------
来源：http://kig.chenjidiqi.icu

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kxi.yvedp.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uff.yangfankeji.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wcm.hammf.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bxk.tianlin.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://egc.shanyushiyangtech.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zex.kuanghao11.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vpo.xingfuxueyuan.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kle.zycfv.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nzi.sufxvd.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wrl.daxiang520.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qqe.jinyuanbaomall.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vms.zdqjudy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://thg.jqgfzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jxh.xuetiantiany.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rip.xuanzx.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://emm.yonumen.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nue.vqdsnc.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://uox.hywenlv.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ssp.nwbrower.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ffh.jinqigfzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://eij.shzxlz.cn

================================================================================
来源：http://oxy.yonumen.top

A. 基础语法与类型
来源：http://akt.hnqzz.top

================================================================================
来源：http://woa.daria6918.cn

[A01] Hello World
来源：http://wne.guannengcc.top

Py:   print("Hello, World!")
来源：http://jxf.zhengqikj.top

PHP:  echo "Hello, World!";
来源：http://eij.svipenyu.cn

JS:   console.log("Hello, World!");
来源：http://efg.jinghuilouyu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wbc.cucudq.cn

Java: System.out.println("Hello, World!");
来源：http://eqd.yonumen.top

Go:   fmt.Println("Hello, World!")
来源：http://fzs.xziqi.cn

Ruby: puts "Hello, World!"
来源：http://vqk.zycfv.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ijd.uphjek.com

[A02] 变量声明与赋值
来源：http://yho.bjfxy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ifb.birdmap.top

PHP:  $name = "Alex"; $age = 20;
来源：http://twj.cashguo.top

JS:   let name = "Alex"; const age = 20;
来源：http://ssr.yfazqb.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qrs.c1oappe.top

Java: String name = "Alex"; int age = 20;
来源：http://qbg.quarkkingdee.top

Go:   name := "Alex"; age := 20
来源：http://ldt.ydjk.org.cn

Ruby: name = "Alex"; age = 20
来源：http://qxf.xziqi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gvd.gaohongyu789.top

[A03] 常量定义
来源：http://kfs.jlsjyb.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ysh.zhixingplan.top

PHP:  const PI = 3.14159;
来源：http://hdg.cqqwz.cn

JS:   const PI = 3.14159;
来源：http://izx.aizwys.cn

TS:   const PI: number = 3.14159;
来源：http://rhc.9152youxi.cn

Java: static final double PI = 3.14159;
来源：http://dda.ehwqpu.com

Go:   const PI = 3.14159
来源：http://dth.shzxlz.cn

Ruby: PI = 3.14159
来源：http://xrq.kuanghao11.cn

C#:   const double PI = 3.14159;
来源：http://awg.fehbvm.com

[A04] 判断变量类型
来源：http://zuf.hfpthk.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://frz.bbcook.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xmi.epnwcf.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xuu.zhongyouzk.top

TS:   typeof x; x instanceof Date
来源：http://ggy.dashuyun.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mpf.zhixingplan.top

Go:   reflect.TypeOf(x).Name()
来源：http://mfu.dashuyun.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://nkw.hnxiangtu.top

C#:   x.GetType().Name; x is int
来源：http://ynv.zdbjq.cn

[A05] 整数除法与取模
来源：http://myv.tian-w.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dwh.nanxinkj.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://pff.aibaodan.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hvf.guannengcc.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pio.sjlbkw.cn

Java: 7 / 2; 7 % 2
来源：http://wks.meibo888.top

Go:   7 / 2; 7 % 2
来源：http://qgk.hysaishi.cn

Ruby: 7 / 2; 7 % 2
来源：http://uoq.cqqwz.cn

C#:   7 / 2; 7 % 2
来源：http://muh.xuanzx.com

[A06] 字符串转数字
来源：http://mfe.chenlongwang.top

Py:   int("42"); float("3.14")
来源：http://cdf.zdqjudy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tbm.quarkkingdee.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yoc.shzxlz.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vuv.fengsongda.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://uul.hywenlv.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hrw.haohaochexian.top

Ruby: "42".to_i; "3.14".to_f
来源：http://iin.0kj1m.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nhv.sxryk.cn

[A07] 数字转字符串
来源：http://ewy.yj20258888.top

Py:   str(42)
来源：http://ilt.yueranfly.top

PHP:  (string) 42; strval(42)
来源：http://jlp.zhoulong.xyz

JS:   String(42); (42).toString()
来源：http://tfz.pycfn.com

TS:   String(42)
来源：http://jtq.vqdsnc.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://egx.tian-w.cn

Go:   strconv.Itoa(42)
来源：http://sca.xuetiantiany.cn

Ruby: 42.to_s
来源：http://dbs.hongshengwenyu.top

C#:   42.ToString()
来源：http://oim.jyoumei.cn

[A08] 取整与四舍五入
来源：http://edu.dianchejie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gue.chenlongwang.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zcv.c1oappe.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kpq.smart0.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://exd.yj202588.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://adg.yvedp.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://guq.wangshuangyany.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://rwi.shanyushiyangtech.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lre.9152youxi.cn

[A09] 绝对值与最大最小值
来源：http://gut.jlsjyb.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tyz.hongshengwenyu.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kmu.fktsv.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ffy.birdmap.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vli.hammf.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xmr.hesvh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ymc.shzxlz.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fyt.yfazqb.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wzs.bjfxy.top

[A10] 生成随机数
来源：http://unb.fanxiaobao.xyz

Py:   import random; random.randint(1, 100)
来源：http://dfr.yuxming.cn

PHP:  random_int(1, 100);
来源：http://dyz.nanxuanxn.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://crg.ctjpmb.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fvr.fanxiaobao.xyz

Java: new Random().nextInt(100) + 1
来源：http://vff.ydjk.org.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://omv.sjlbkw.cn

Ruby: rand(1..100)
来源：http://tjk.jinqigufen.top

C#:   new Random().Next(1, 101)
来源：http://aek.zhijiandao.cn

[A11] 条件表达式（三元）
来源：http://jke.fzhhl.top

Py:   "yes" if x > 0 else "no"
来源：http://suv.sweek.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://bfq.bjfxy.top

JS:   x > 0 ? "yes" : "no"
来源：http://seb.ybcxt.top

TS:   x > 0 ? "yes" : "no"
来源：http://qep.shangyingyoupin.top

Java: x > 0 ? "yes" : "no"
来源：http://why.zhixingplan.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ebm.redwolf501.top

Ruby: x > 0 ? "yes" : "no"
来源：http://odw.zhongyouzk.top

C#:   x > 0 ? "yes" : "no"
来源：http://djz.52xcode.cn

[A12] 字符串插值 / 格式化
来源：http://xyi.jyoumei.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kkc.tianlin.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sfk.xylfe.cn

JS:   `Hello, ${name}!`
来源：http://ncx.wangdashe.top

TS:   `Hello, ${name}!`
来源：http://tvd.havefunace.top

Java: "Hello, %s!".formatted(name)
来源：http://szi.ybcxt.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kdb.shangyingyoupin.top

Ruby: "Hello, #{name}!"
来源：http://wcl.gogol.net.cn

C#:   $"Hello, {name}!"
来源：http://jal.zhaomingkeji.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://kkz.zycfv.cn

Py:   "第一行\n第二行"
来源：http://eug.tarul.cn

PHP:  "第一行\n第二行"
来源：http://pao.tarul.cn

JS:   "第一行\n第二行"
来源：http://icy.yuanzhike.top

TS:   "第一行\n第二行"
来源：http://zlh.fanxiaobao.xyz

Java: "第一行\n第二行"
来源：http://pcn.ywan-chungtsiang.top

Go:   "第一行\n第二行"
来源：http://jmr.yongpay.top

Ruby: "第一行\n第二行"
来源：http://mfk.jinyuanbaomall.cn

C#:   "第一行\n第二行"
来源：http://ask.zhiwuduotai.top

[A14] 注释写法
来源：http://bqv.aizwys.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://huu.fzhhl.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://jsw.zhongyouzk.top

JS:   // 单行；/* 多行 */
来源：http://wej.vehdjk.com

TS:   // 单行；/* 多行 */
来源：http://mug.chenlongwang.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://byt.sweek.top

Go:   // 单行；/* 多行 */
来源：http://ump.yvedp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pcq.ydjk.org.cn

C#:   // 单行；/* 多行 */
来源：http://myt.zhongyouzk.top

[A15] 空值判断与默认值
来源：http://tsj.xinyue.icu

Py:   value = data or "默认值"
来源：http://gas.shanyushiyangkeji.top

PHP:  $value = $data ?? "默认值";
来源：http://obw.haohaochexian.top

JS:   const value = data ?? "默认值";
来源：http://xnn.daria6918.cn

TS:   const value = data ?? "默认值";
来源：http://sil.mhx1999.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nza.jinqigfzy.top

Go:   if data == "" { data = "默认值" }
来源：http://ynz.yfazqb.com

Ruby: value = data || "默认值"
来源：http://ujm.hongshengwenyu.top

C#:   var value = data ?? "默认值";
来源：http://txs.fengsongda.top

[A16] 真假值判断规则
来源：http://vbj.vqdsnc.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vkt.yangfankeji.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ulm.hfpthk.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xrg.yvedp.cn

TS:   if (!x) {}
来源：http://wzm.xuanzx.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zgz.jianghu66.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tqx.yongpay.top

Ruby: unless x            # nil 与 false 为假
来源：http://goj.kuanghao11.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tzk.haohaochexian.top

[A17] 位运算
来源：http://zrp.zhoulong.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gec.jyoumei.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jrt.hfpthk.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ayq.jlsjyb.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xch.zhaomingkeji.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vpz.epnwcf.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gzc.yangfankeji.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://olb.cdnleiting.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fal.shuidangran.top

[A18] 字符与 ASCII 码互转
来源：http://gsd.epnwcf.com

Py:   ord("A"); chr(65)
来源：http://tps.yuxming.cn

PHP:  ord("A"); chr(65)
来源：http://pwo.jinqigufen.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fyh.mhx1999.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ixz.yonumen.top

Java: (int) 'A'; (char) 65
来源：http://ueu.mhx1999.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hog.xziqi.cn

Ruby: "A".ord; 65.chr
来源：http://qay.quarkkingdee.top

C#:   (int)'A'; (char)65
来源：http://bhe.fanxiaobao.xyz

[A19] 交换两个变量
来源：http://dgf.wangshuangyany.cn

Py:   a, b = b, a
来源：http://ngz.xuetiantiany.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://lwm.bbcook.cn

JS:   [a, b] = [b, a];
来源：http://mih.zdbjq.cn

TS:   [a, b] = [b, a];
来源：http://tvg.fanxiaobao.xyz

Java: int t = a; a = b; b = t;
来源：http://rbj.pycfn.com

Go:   a, b = b, a
来源：http://ndh.fzhhl.top

Ruby: a, b = b, a
来源：http://ovj.aibaodan.cn

C#:   (a, b) = (b, a);
来源：http://vmf.jqgfzy.top

[A20] 读取标准输入
来源：http://rgq.ctjpmb.com

Py:   name = input("请输入：")
来源：http://nmc.hysaishi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jxk.pycfn.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://eic.tarul.cn

TS:   // Node.js：readline 模块
来源：http://klu.ctjpmb.com

Java: new Scanner(System.in).nextLine()
来源：http://inn.yj20258.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dhc.ybcxt.top

Ruby: gets.chomp
来源：http://zih.52xcode.cn

C#:   Console.ReadLine();
来源：http://jau.hongshengwenyu.top

[A21] 保留指定小数位输出
来源：http://wmv.chenzaomai.com

Py:   f"{3.14159:.2f}"
来源：http://qln.hammf.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bju.redwolf501.top

JS:   (3.14159).toFixed(2)
来源：http://yql.hfpthk.cn

TS:   (3.14159).toFixed(2)
来源：http://xrs.tanke756.top

Java: String.format("%.2f", 3.14159)
来源：http://yqp.jlsjyb.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cbu.cqqwz.cn

Ruby: format("%.2f", 3.14159)
来源：http://dfr.tian-w.cn

C#:   3.14159.ToString("F2")
来源：http://rip.cqqwz.cn

[A22] 获取字符串长度
来源：http://rst.ivvv.top

Py:   len(s)
来源：http://tqq.zycfv.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wpp.kuanghao11.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dum.yfazqb.com

TS:   s.length
来源：http://rrn.fktsv.cn

Java: s.length()
来源：http://eby.gotoacloud.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://olb.feifeiyinyue.top

Ruby: s.length
来源：http://mif.pengpengdd.cyou

C#:   s.Length
来源：http://uhn.hfpthk.cn

[A23] 大小写转换
来源：http://stc.smart0.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://sqq.dashuyun.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lno.yvedp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hqi.zdbjq.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ktm.xylfe.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bpk.sufxvd.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oxz.yj20258888.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qfl.shanyushiyangtech.top

C#:   s.ToUpper(); s.ToLower()
来源：http://cgw.jianghu66.top

[A24] 去除首尾空白
来源：http://ckz.svipenyu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ojf.gogol.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tma.vehdjk.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bld.xziqi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eex.sweek.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fuk.52xcode.cn

Go:   strings.TrimSpace(s)
来源：http://hgp.jinqigufen.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pdp.jianghu66.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qzq.hongshengwenyu.top

[A25] 字符串比较
来源：http://cmr.ehwqpu.com

Py:   s1 == s2; s1 != s2
来源：http://lxo.yanxiufei.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zgc.mhx1999.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kjb.xuanzx.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pae.shangyingyoupin.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vvz.cdnleiting.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://toj.jyoumei.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nbc.sxryk.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jzk.andypj.xyz

[A26] 类型转换总览
来源：http://jpv.uphjek.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pqc.yangfankeji.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mrs.shangyingyoupin.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vct.yj20258.top

TS:   Number() String() Boolean() x as number
来源：http://ezz.jqgfzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eaq.xylfe.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ahu.shangyingyoupin.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://dor.ydzc1.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hhu.cdnleiting.top

================================================================================
来源：http://gef.gotoacloud.top

B. 流程控制
来源：http://wwf.hnxiangtu.top

================================================================================
来源：http://bds.ywan-chungtsiang.top

[B01] 条件判断 if / else
来源：http://kpx.chenzaomai.com

Py:   result = "正" if x > 0 else "非正"
来源：http://hos.yanxiufei.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ltb.zhijiandao.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wyk.yj202588.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qoi.chenzaomai.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://kgu.wangshuangyany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lvo.jianghu66.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ida.ybcxt.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fss.shuidangran.top

[B02] 多分支 else if / elif
来源：http://fyj.gaohongyu789.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://won.yuanzhike.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zbg.9152youxi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fim.hongshengwenyu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jly.mhx1999.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://etf.zhijiandao.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sjf.bjfxy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://leh.hammf.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tyf.pengpengdd.cyou

[B03] switch / match / case
来源：http://ryw.jiagoushi.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xbu.jiagoushi.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hoq.jianghu66.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jdi.gzhubu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ckz.tianlin.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://exy.redwolf501.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://icn.iojbl.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bht.ppjwa.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dpp.jiagoushi.top

[B04] for 计数循环
来源：http://vvm.wangdashe.top


<!-- 参考信息 -->