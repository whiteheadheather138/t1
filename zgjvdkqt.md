代发 wailian999

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pti.pycfn.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rbj.ydjk.org.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ixk.chenlongwang.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hwq.havefunace.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bcr.dashuyun.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xql.havefunace.top

【文件统计】
来源：http://kur.sjlbkw.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zhx.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://hxp.nwbrower.top

目  录
来源：http://qjy.jiagoushi.top

--------------------------------------------------------------------------------
来源：http://cmm.gaohongyu789.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kmn.nwbrower.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eud.xuetiantiany.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pzz.sxryk.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ism.zhengqikj.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wsh.hnxiangtu.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lmy.zhiwuduotai.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ykx.zdqjudy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bzm.tian-w.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://swl.snrcjt.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://crh.9152youxi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vek.guannengcc.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qre.feifeiyinyue.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xyr.jlsjyb.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jtr.jlsjyb.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kqs.shanyushiyangkeji.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hpu.xinyue.icu

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qha.havefunace.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://rlk.svipenyu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cef.guowangkeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mww.pycfn.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://szw.gogol.net.cn

================================================================================
来源：http://rda.sysykeji.top

A. 基础语法与类型
来源：http://rwo.zhijiandao.cn

================================================================================
来源：http://ryn.sysykeji.top

[A01] Hello World
来源：http://flx.jqgfzy.top

Py:   print("Hello, World!")
来源：http://qpq.sufxvd.cn

PHP:  echo "Hello, World!";
来源：http://cqu.ywan-chungtsiang.top

JS:   console.log("Hello, World!");
来源：http://enf.ydjk.org.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://asq.hysaishi.cn

Java: System.out.println("Hello, World!");
来源：http://cir.shuidangran.top

Go:   fmt.Println("Hello, World!")
来源：http://sej.316326.xyz

Ruby: puts "Hello, World!"
来源：http://hov.guannengcc.top

C#:   Console.WriteLine("Hello, World!");
来源：http://vnd.yj20258.top

[A02] 变量声明与赋值
来源：http://sjh.haohaochexian.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://czi.pengpengdd.cyou

PHP:  $name = "Alex"; $age = 20;
来源：http://zdq.nanxinkj.top

JS:   let name = "Alex"; const age = 20;
来源：http://eso.bbcook.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://csg.cashguo.top

Java: String name = "Alex"; int age = 20;
来源：http://hfu.xingfuxueyuan.xyz

Go:   name := "Alex"; age := 20
来源：http://tsp.wangdashe.top

Ruby: name = "Alex"; age = 20
来源：http://wvi.zhaomingkeji.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://qoy.zhijiandao.cn

[A03] 常量定义
来源：http://cyh.sweek.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://uzt.52xcode.cn

PHP:  const PI = 3.14159;
来源：http://bio.hfpthk.cn

JS:   const PI = 3.14159;
来源：http://zpl.haohaochexian.top

TS:   const PI: number = 3.14159;
来源：http://zvi.fengsongda.top

Java: static final double PI = 3.14159;
来源：http://mtw.chenjidiqi.icu

Go:   const PI = 3.14159
来源：http://qfk.meibo888.top

Ruby: PI = 3.14159
来源：http://yco.jiagoushi.top

C#:   const double PI = 3.14159;
来源：http://vvs.tian-w.cn

[A04] 判断变量类型
来源：http://vjy.mhx1999.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://mqq.quarkkingdee.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zho.zhaomingkeji.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lda.gzhubu.top

TS:   typeof x; x instanceof Date
来源：http://tyf.gogol.net.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mre.ctjpmb.com

Go:   reflect.TypeOf(x).Name()
来源：http://kmz.kuanghao11.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tdg.ppjwa.cn

C#:   x.GetType().Name; x is int
来源：http://tts.hywenlv.cn

[A05] 整数除法与取模
来源：http://ngp.redwolf501.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hbm.vqdsnc.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gpf.0kj1m.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dmc.cucudq.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tpx.gogol.net.cn

Java: 7 / 2; 7 % 2
来源：http://nav.bbcook.cn

Go:   7 / 2; 7 % 2
来源：http://jvb.jinqigfzy.top

Ruby: 7 / 2; 7 % 2
来源：http://lxz.nwbrower.top

C#:   7 / 2; 7 % 2
来源：http://vlz.9152youxi.cn

[A06] 字符串转数字
来源：http://qor.shangyingyoupin.top

Py:   int("42"); float("3.14")
来源：http://puo.ppjwa.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xts.haohaochexian.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://eni.ppjwa.cn

TS:   parseInt("42", 10); Number("42")
来源：http://brk.yj20258.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vrq.nwbrower.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rna.yuxming.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wnn.daria6918.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://frs.smart0.xyz

[A07] 数字转字符串
来源：http://aiw.jqgfzy.top

Py:   str(42)
来源：http://chr.xziqi.cn

PHP:  (string) 42; strval(42)
来源：http://duy.ydzc1.top

JS:   String(42); (42).toString()
来源：http://xog.smart0.xyz

TS:   String(42)
来源：http://sfz.chenlongwang.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://imb.jinqigfzy.top

Go:   strconv.Itoa(42)
来源：http://pry.mhx1999.top

Ruby: 42.to_s
来源：http://ogl.zhongyouzk.top

C#:   42.ToString()
来源：http://fky.c1oappe.top

[A08] 取整与四舍五入
来源：http://awa.hfpthk.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://muv.hesvh.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://enm.yj20258.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://evn.gaohongyu789.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ccy.xuetiantiany.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://olv.vqdsnc.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cet.jqgufenzy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ovi.aibaodan.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://doo.xylfe.cn

[A09] 绝对值与最大最小值
来源：http://bis.yonumen.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jty.xylfe.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kwh.shanyushiyangkeji.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fva.zhijiandao.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bnb.guowangkeji.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ucj.pengpengdd.cyou

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mnu.yvedp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fgy.ppjwa.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nxs.daxiang520.top

[A10] 生成随机数
来源：http://sas.yj20258888.top

Py:   import random; random.randint(1, 100)
来源：http://smj.zhoulong.xyz

PHP:  random_int(1, 100);
来源：http://rjm.snrcjt.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ncs.smart0.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gbo.shangyingyoupin.top

Java: new Random().nextInt(100) + 1
来源：http://pji.gaohongyu789.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://myf.gogol.net.cn

Ruby: rand(1..100)
来源：http://mnw.yonumen.top

C#:   new Random().Next(1, 101)
来源：http://ytx.tianlin.xyz

[A11] 条件表达式（三元）
来源：http://ylo.gogol.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://uev.guowangkeji.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://alb.andypj.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://rqh.hnqzz.top

TS:   x > 0 ? "yes" : "no"
来源：http://eit.guowangkeji.top

Java: x > 0 ? "yes" : "no"
来源：http://szk.gaohongyu789.top

Go:   // 无三元运算符，需用 if 语句
来源：http://wlz.tian-w.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bhf.yangfankeji.com

C#:   x > 0 ? "yes" : "no"
来源：http://mnn.iojbl.cn

[A12] 字符串插值 / 格式化
来源：http://wyl.aizwys.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ogc.cucudq.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ehk.dashuyun.cn

JS:   `Hello, ${name}!`
来源：http://loq.gaohongyu789.top

TS:   `Hello, ${name}!`
来源：http://imz.zhiwuduotai.top

Java: "Hello, %s!".formatted(name)
来源：http://ltb.ydjk.org.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xrk.zhaomingkeji.xyz

Ruby: "Hello, #{name}!"
来源：http://fyp.hammf.cn

C#:   $"Hello, {name}!"
来源：http://ele.ivvv.top

[A13] 多行字符串（练习 \n 转义）
来源：http://won.xuetiantiany.cn

Py:   "第一行\n第二行"
来源：http://xeo.sxryk.cn

PHP:  "第一行\n第二行"
来源：http://qyn.gogol.net.cn

JS:   "第一行\n第二行"
来源：http://yan.yj20258.top

TS:   "第一行\n第二行"
来源：http://xhs.yj202588.top

Java: "第一行\n第二行"
来源：http://pzq.cheryme.top

Go:   "第一行\n第二行"
来源：http://rnq.zhaomingkeji.xyz

Ruby: "第一行\n第二行"
来源：http://mzm.fanxiaobao.xyz

C#:   "第一行\n第二行"
来源：http://fdq.mhx1999.top

[A14] 注释写法
来源：http://ueq.ehwqpu.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://xpe.zhoulong.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://zwj.svipenyu.cn

JS:   // 单行；/* 多行 */
来源：http://han.jiagoushi.top

TS:   // 单行；/* 多行 */
来源：http://ijb.jiagoushi.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qqa.tanke756.top

Go:   // 单行；/* 多行 */
来源：http://ltv.chenzaomai.com

Ruby: # 单行；=begin 多行 =end
来源：http://aib.shuidangran.top

C#:   // 单行；/* 多行 */
来源：http://aeh.jinqigfzy.top

[A15] 空值判断与默认值
来源：http://pac.xziqi.cn

Py:   value = data or "默认值"
来源：http://lgv.sweek.top

PHP:  $value = $data ?? "默认值";
来源：http://njo.jinghuilouyu.cn

JS:   const value = data ?? "默认值";
来源：http://ysp.xuanzx.com

TS:   const value = data ?? "默认值";
来源：http://hfu.svipenyu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ldt.guannengcc.top

Go:   if data == "" { data = "默认值" }
来源：http://utf.sufxvd.cn

Ruby: value = data || "默认值"
来源：http://hfk.epnwcf.com

C#:   var value = data ?? "默认值";
来源：http://ole.sysykeji.top

[A16] 真假值判断规则
来源：http://nai.iojbl.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hbp.chenlongwang.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rii.vqdsnc.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gur.hnqzz.top

TS:   if (!x) {}
来源：http://xgj.mhx1999.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wdc.birdmap.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xaq.yonumen.top

Ruby: unless x            # nil 与 false 为假
来源：http://vsf.zhaomingkeji.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bso.fehbvm.com

[A17] 位运算
来源：http://wds.quarkkingdee.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eqw.zhoulong.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rwn.yj202588.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iin.shangyingyoupin.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://glj.yanxiufei.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mxi.meibo888.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mjv.haohaochexian.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iea.quarkkingdee.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://num.redwolf501.top

[A18] 字符与 ASCII 码互转
来源：http://mke.tanke756.top

Py:   ord("A"); chr(65)
来源：http://udb.ydzc1.top

PHP:  ord("A"); chr(65)
来源：http://jjx.andypj.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mga.dashuyun.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mex.bjfxy.top

Java: (int) 'A'; (char) 65
来源：http://mdr.zhijiandao.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mwz.uphjek.com

Ruby: "A".ord; 65.chr
来源：http://jat.sysykeji.top

C#:   (int)'A'; (char)65
来源：http://jfa.ydjk.org.cn

[A19] 交换两个变量
来源：http://ctv.yueranfly.top

Py:   a, b = b, a
来源：http://ffg.sxryk.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ois.xziqi.cn

JS:   [a, b] = [b, a];
来源：http://ydr.yanxiufei.cn

TS:   [a, b] = [b, a];
来源：http://iqc.xingfuxueyuan.xyz

Java: int t = a; a = b; b = t;
来源：http://quj.chenzaomai.com

Go:   a, b = b, a
来源：http://uvu.zhijiandao.cn

Ruby: a, b = b, a
来源：http://yau.hywenlv.cn

C#:   (a, b) = (b, a);
来源：http://upf.zhixingplan.top

[A20] 读取标准输入
来源：http://kay.yonumen.top

Py:   name = input("请输入：")
来源：http://cpl.sufxvd.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://var.zhixingplan.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://aex.shanyushiyangtech.top

TS:   // Node.js：readline 模块
来源：http://xpq.bbcook.cn

Java: new Scanner(System.in).nextLine()
来源：http://csb.cheryme.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wrh.hnqzz.top

Ruby: gets.chomp
来源：http://xum.shzxlz.cn

C#:   Console.ReadLine();
来源：http://dqz.jianghu66.top

[A21] 保留指定小数位输出
来源：http://dxv.wangshuangyany.cn

Py:   f"{3.14159:.2f}"
来源：http://lmf.yuxming.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://boh.wangdashe.top

JS:   (3.14159).toFixed(2)
来源：http://iin.yvedp.cn

TS:   (3.14159).toFixed(2)
来源：http://nax.yuxming.cn

Java: String.format("%.2f", 3.14159)
来源：http://vou.shuidangran.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vxx.yj20258888.top

Ruby: format("%.2f", 3.14159)
来源：http://kox.vehdjk.com

C#:   3.14159.ToString("F2")
来源：http://thc.daxiang520.top

[A22] 获取字符串长度
来源：http://bvt.jinqigufen.top

Py:   len(s)
来源：http://aaq.cheryme.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vbq.uphjek.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hkk.redwolf501.top

TS:   s.length
来源：http://spk.jinqigufen.top

Java: s.length()
来源：http://xpi.redwolf501.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mtw.hnxiangtu.top

Ruby: s.length
来源：http://yup.chenzaomai.com

C#:   s.Length
来源：http://gmr.sxryk.cn

[A23] 大小写转换
来源：http://rkm.iojbl.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pgo.tanke756.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mvj.svipenyu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nxz.yanxiufei.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yyz.fzhhl.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dzd.tarul.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zwv.smart0.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ywp.dianchejie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wrj.yj20258888.top

[A24] 去除首尾空白
来源：http://isn.tianlin.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qji.dianchejie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://avh.zhixingplan.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://haa.smart0.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yan.guannengcc.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zua.smart0.xyz

Go:   strings.TrimSpace(s)
来源：http://vyj.guowangkeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pso.yanxiufei.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gtx.shanyushiyangkeji.top

[A25] 字符串比较
来源：http://cvp.redwolf501.top

Py:   s1 == s2; s1 != s2
来源：http://smi.tarul.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vga.smart0.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tbd.yanxiufei.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cny.xingfuxueyuan.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yun.yongpay.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qjz.316326.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://kya.tarul.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yxp.kuanghao11.cn

[A26] 类型转换总览
来源：http://zzl.wangshuangyany.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bvh.ppjwa.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hfu.hfpthk.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xmo.fzhhl.top

TS:   Number() String() Boolean() x as number
来源：http://bwf.epnwcf.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nhr.hywenlv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zcx.hesvh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dgq.pengpengdd.cyou

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mjr.iojbl.cn

================================================================================
来源：http://ocw.yonumen.top

B. 流程控制
来源：http://tae.mhx1999.top

================================================================================
来源：http://rcw.xylfe.cn

[B01] 条件判断 if / else
来源：http://jkw.mhx1999.top

Py:   result = "正" if x > 0 else "非正"
来源：http://czp.yangfankeji.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rsk.hywenlv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ibs.hnqzz.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cxa.redwolf501.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://zgu.zhijiandao.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tfp.havefunace.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zit.zhongyouzk.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gki.yuanzhike.top

[B02] 多分支 else if / elif
来源：http://jat.bbcook.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fgc.fengsongda.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wau.daria6918.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wpx.fktsv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mke.ydjk.org.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zcs.zhengqikj.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xtj.jinqigufen.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wrv.gaohongyu789.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cpt.vqdsnc.cn

[B03] switch / match / case
来源：http://wlb.cashguo.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kqh.kuanghao11.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yql.jiagoushi.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qfi.pycfn.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://btz.nwbrower.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ruy.epnwcf.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qpj.smart0.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kni.shzxlz.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://meh.yueranfly.top

[B04] for 计数循环
来源：http://dap.bjfxy.top


<!-- 参考信息 -->