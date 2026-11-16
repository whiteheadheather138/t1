代发 wailian999

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xjy.yanxiufei.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://muf.jinqigufen.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ovb.gogol.net.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xzn.quarkkingdee.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vmy.fanxiaobao.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zfc.yonumen.top

【文件统计】
来源：http://aog.smart0.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://omm.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://jim.nanxuanxn.top

目  录
来源：http://nzv.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://hlf.tanke756.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://oma.gzhubu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hfn.iojbl.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ljd.cashguo.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yka.cheryme.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cbp.gaohongyu789.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nhu.wangshuangyany.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dee.cucudq.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://omm.jqgufenzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rag.zhengqikj.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wvs.redwolf501.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://anv.daria6918.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xge.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://brl.cheryme.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kjt.vqdsnc.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rtt.yvedp.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mnq.vqdsnc.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cuh.cqqwz.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zqn.dashuyun.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dgh.yuxming.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vbw.fktsv.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mmn.yvedp.cn

================================================================================
来源：http://yhb.guowangkeji.top

A. 基础语法与类型
来源：http://jdg.kuanghao11.cn

================================================================================
来源：http://wbc.sxryk.cn

[A01] Hello World
来源：http://bim.cucudq.cn

Py:   print("Hello, World!")
来源：http://zwb.xinyue.icu

PHP:  echo "Hello, World!";
来源：http://cni.hfpthk.cn

JS:   console.log("Hello, World!");
来源：http://dyp.ydjk.org.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://any.hongshengwenyu.top

Java: System.out.println("Hello, World!");
来源：http://dch.aizwys.cn

Go:   fmt.Println("Hello, World!")
来源：http://ttf.jqgufenzy.top

Ruby: puts "Hello, World!"
来源：http://rcv.cheryme.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ugy.guowangkeji.top

[A02] 变量声明与赋值
来源：http://qxy.xinyue.icu

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://quc.ehwqpu.com

PHP:  $name = "Alex"; $age = 20;
来源：http://ifz.svipenyu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ofe.ybcxt.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xln.yvedp.cn

Java: String name = "Alex"; int age = 20;
来源：http://pmy.yuanzhike.top

Go:   name := "Alex"; age := 20
来源：http://rqh.fktsv.cn

Ruby: name = "Alex"; age = 20
来源：http://hwa.andypj.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://klb.wangshuangyany.cn

[A03] 常量定义
来源：http://bdj.quarkkingdee.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rrq.jinyuanbaomall.cn

PHP:  const PI = 3.14159;
来源：http://cjf.ywan-chungtsiang.top

JS:   const PI = 3.14159;
来源：http://kwd.sxryk.cn

TS:   const PI: number = 3.14159;
来源：http://npt.ppjwa.cn

Java: static final double PI = 3.14159;
来源：http://qqe.xinyue.icu

Go:   const PI = 3.14159
来源：http://gbp.hnxiangtu.top

Ruby: PI = 3.14159
来源：http://pry.uphjek.com

C#:   const double PI = 3.14159;
来源：http://tpd.xylfe.cn

[A04] 判断变量类型
来源：http://qme.hcnkem.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://hua.gogol.net.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tdo.andypj.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gct.hysaishi.cn

TS:   typeof x; x instanceof Date
来源：http://ccq.gzhubu.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vwl.tianlin.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://teb.ctjpmb.com

Ruby: x.class; x.is_a?(Integer)
来源：http://tdq.shangyingyoupin.top

C#:   x.GetType().Name; x is int
来源：http://hhk.ivvv.top

[A05] 整数除法与取模
来源：http://xgf.jinqigfzy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lwj.yj20258.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://qmk.epnwcf.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://let.sufxvd.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://opd.jqgfzy.top

Java: 7 / 2; 7 % 2
来源：http://ojt.yuanzhike.top

Go:   7 / 2; 7 % 2
来源：http://rgn.zhijiandao.cn

Ruby: 7 / 2; 7 % 2
来源：http://xvn.redwolf501.top

C#:   7 / 2; 7 % 2
来源：http://tte.pengpengdd.cyou

[A06] 字符串转数字
来源：http://rcl.xingfuxueyuan.xyz

Py:   int("42"); float("3.14")
来源：http://jhi.daxiang520.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jku.fehbvm.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ouw.cashguo.top

TS:   parseInt("42", 10); Number("42")
来源：http://orq.zhaomingkeji.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://deg.haohaochexian.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vps.hysaishi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://phk.ydjk.org.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zor.zhiwuduotai.top

[A07] 数字转字符串
来源：http://ybj.yongpay.top

Py:   str(42)
来源：http://tph.fehbvm.com

PHP:  (string) 42; strval(42)
来源：http://xxh.sufxvd.cn

JS:   String(42); (42).toString()
来源：http://egk.tian-w.cn

TS:   String(42)
来源：http://klm.xingfuxueyuan.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://dgw.pycfn.com

Go:   strconv.Itoa(42)
来源：http://byc.shzxlz.cn

Ruby: 42.to_s
来源：http://cpv.haohaochexian.top

C#:   42.ToString()
来源：http://vnt.fktsv.cn

[A08] 取整与四舍五入
来源：http://wcl.xuetiantiany.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pwd.guannengcc.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xxf.hfpthk.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lws.uphjek.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lbc.yj20258.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ybo.fehbvm.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://npt.guannengcc.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://gpz.jiagoushi.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gpb.yangfankeji.com

[A09] 绝对值与最大最小值
来源：http://gwv.bjfxy.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zol.wangshuangyany.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tet.tanke756.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ybb.52xcode.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wum.guowangkeji.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mmg.cqqwz.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tsx.hesvh.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://eic.xingfuxueyuan.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jhq.0kj1m.cn

[A10] 生成随机数
来源：http://idy.sxryk.cn

Py:   import random; random.randint(1, 100)
来源：http://qjn.chenlongwang.top

PHP:  random_int(1, 100);
来源：http://dqn.shangyingyoupin.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nhp.chenzaomai.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wys.xziqi.cn

Java: new Random().nextInt(100) + 1
来源：http://ywq.yanxiufei.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://uyx.jqgufenzy.top

Ruby: rand(1..100)
来源：http://vey.ppjwa.cn

C#:   new Random().Next(1, 101)
来源：http://rhf.hammf.cn

[A11] 条件表达式（三元）
来源：http://tln.zhoulong.xyz

Py:   "yes" if x > 0 else "no"
来源：http://zjm.hammf.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wle.zycfv.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yma.gzhubu.top

TS:   x > 0 ? "yes" : "no"
来源：http://yft.xuetiantiany.cn

Java: x > 0 ? "yes" : "no"
来源：http://apl.andypj.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://dlr.ydjk.org.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jyo.fengsongda.top

C#:   x > 0 ? "yes" : "no"
来源：http://rdr.52xcode.cn

[A12] 字符串插值 / 格式化
来源：http://pur.ehwqpu.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://slu.jinqigufen.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tau.jiagoushi.top

JS:   `Hello, ${name}!`
来源：http://nkr.vqdsnc.cn

TS:   `Hello, ${name}!`
来源：http://zdj.hcnkem.com

Java: "Hello, %s!".formatted(name)
来源：http://ubs.tanke756.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ale.ywan-chungtsiang.top

Ruby: "Hello, #{name}!"
来源：http://nmr.daxiang520.top

C#:   $"Hello, {name}!"
来源：http://buz.jyoumei.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://sps.sysykeji.top

Py:   "第一行\n第二行"
来源：http://sjs.aibaodan.cn

PHP:  "第一行\n第二行"
来源：http://ars.hammf.cn

JS:   "第一行\n第二行"
来源：http://loy.haohaochexian.top

TS:   "第一行\n第二行"
来源：http://uim.chenzaomai.com

Java: "第一行\n第二行"
来源：http://vex.ydzc1.top

Go:   "第一行\n第二行"
来源：http://swt.fzhhl.top

Ruby: "第一行\n第二行"
来源：http://gfu.316326.xyz

C#:   "第一行\n第二行"
来源：http://yko.jqgfzy.top

[A14] 注释写法
来源：http://vae.yueranfly.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://zbz.shanyushiyangkeji.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://kat.c1oappe.top

JS:   // 单行；/* 多行 */
来源：http://nlz.hesvh.cn

TS:   // 单行；/* 多行 */
来源：http://kaw.svipenyu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xaq.zhijiandao.cn

Go:   // 单行；/* 多行 */
来源：http://zmg.yj20258.top

Ruby: # 单行；=begin 多行 =end
来源：http://knr.0kj1m.cn

C#:   // 单行；/* 多行 */
来源：http://wak.zhongyouzk.top

[A15] 空值判断与默认值
来源：http://lcm.daria6918.cn

Py:   value = data or "默认值"
来源：http://ldn.sweek.top

PHP:  $value = $data ?? "默认值";
来源：http://fwa.hongshengwenyu.top

JS:   const value = data ?? "默认值";
来源：http://eur.aibaodan.cn

TS:   const value = data ?? "默认值";
来源：http://dql.tian-w.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rsb.shanyushiyangtech.top

Go:   if data == "" { data = "默认值" }
来源：http://uul.sysykeji.top

Ruby: value = data || "默认值"
来源：http://qrz.fzhhl.top

C#:   var value = data ?? "默认值";
来源：http://kbz.sufxvd.cn

[A16] 真假值判断规则
来源：http://czf.ydjk.org.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mhs.birdmap.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fho.guannengcc.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xzh.hfpthk.cn

TS:   if (!x) {}
来源：http://mut.hfpthk.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://eih.meibo888.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wrc.jinqigfzy.top

Ruby: unless x            # nil 与 false 为假
来源：http://law.shuidangran.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sxk.aizwys.cn

[A17] 位运算
来源：http://qeg.yfazqb.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://npx.svipenyu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xbk.andypj.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rrs.redwolf501.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ppq.vqdsnc.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kge.ydzc1.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dbh.zhixingplan.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vzb.chenlongwang.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cau.fktsv.cn

[A18] 字符与 ASCII 码互转
来源：http://mrw.yueranfly.top

Py:   ord("A"); chr(65)
来源：http://kgx.sjlbkw.cn

PHP:  ord("A"); chr(65)
来源：http://gcs.guannengcc.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fpa.tanke756.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uge.zdqjudy.top

Java: (int) 'A'; (char) 65
来源：http://csj.hammf.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wqp.xziqi.cn

Ruby: "A".ord; 65.chr
来源：http://fjj.jianghu66.top

C#:   (int)'A'; (char)65
来源：http://nbm.fengsongda.top

[A19] 交换两个变量
来源：http://dsb.hammf.cn

Py:   a, b = b, a
来源：http://vis.svipenyu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://dbn.fanxiaobao.xyz

JS:   [a, b] = [b, a];
来源：http://hql.cucudq.cn

TS:   [a, b] = [b, a];
来源：http://ouv.tianlin.xyz

Java: int t = a; a = b; b = t;
来源：http://jpi.chenzaomai.com

Go:   a, b = b, a
来源：http://quz.gogol.net.cn

Ruby: a, b = b, a
来源：http://zuk.xingfuxueyuan.xyz

C#:   (a, b) = (b, a);
来源：http://hig.yongpay.top

[A20] 读取标准输入
来源：http://kyf.jinyuanbaomall.cn

Py:   name = input("请输入：")
来源：http://egx.shanyushiyangkeji.top

PHP:  $name = trim(fgets(STDIN));
来源：http://iew.jqgufenzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cgl.yj202588.top

TS:   // Node.js：readline 模块
来源：http://qjt.jqgufenzy.top

Java: new Scanner(System.in).nextLine()
来源：http://nuq.yj20258.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fne.cucudq.cn

Ruby: gets.chomp
来源：http://mqr.yvedp.cn

C#:   Console.ReadLine();
来源：http://gng.ywan-chungtsiang.top

[A21] 保留指定小数位输出
来源：http://mmi.haohaochexian.top

Py:   f"{3.14159:.2f}"
来源：http://oad.iojbl.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hip.c1oappe.top

JS:   (3.14159).toFixed(2)
来源：http://pdt.havefunace.top

TS:   (3.14159).toFixed(2)
来源：http://vvr.jiagoushi.top

Java: String.format("%.2f", 3.14159)
来源：http://sbe.hfpthk.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ony.gogol.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://baq.shangyingyoupin.top

C#:   3.14159.ToString("F2")
来源：http://zif.tianlin.xyz

[A22] 获取字符串长度
来源：http://ujj.zhixingplan.top

Py:   len(s)
来源：http://vqy.hnqzz.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ypl.nanxuanxn.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ssy.cdnleiting.top

TS:   s.length
来源：http://dxy.ybcxt.top

Java: s.length()
来源：http://sku.ehwqpu.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://swg.zhoulong.xyz

Ruby: s.length
来源：http://tmc.hnqzz.top

C#:   s.Length
来源：http://iew.hnqzz.top

[A23] 大小写转换
来源：http://wfb.jinqigufen.top

Py:   s.upper(); s.lower(); s.title()
来源：http://uwx.sufxvd.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wir.jinqigufen.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kwz.smart0.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lkw.hesvh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wly.fengsongda.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hic.aibaodan.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hxo.zhengqikj.top

C#:   s.ToUpper(); s.ToLower()
来源：http://nja.uphjek.com

[A24] 去除首尾空白
来源：http://hkq.xingfuxueyuan.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fup.hnqzz.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qmn.epnwcf.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://axs.xinyue.icu

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lrp.zhongyouzk.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bnd.chenjidiqi.icu

Go:   strings.TrimSpace(s)
来源：http://tde.uphjek.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://isq.zhixingplan.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://aeb.sufxvd.cn

[A25] 字符串比较
来源：http://tex.yvedp.cn

Py:   s1 == s2; s1 != s2
来源：http://rth.nanxuanxn.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zzd.jqgufenzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jff.snrcjt.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ckx.sufxvd.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qgp.shangyingyoupin.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://oqh.tian-w.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bkg.yanxiufei.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ukw.bbcook.cn

[A26] 类型转换总览
来源：http://cwj.jianghu66.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://isi.sysykeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sux.zhiwuduotai.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aqw.sufxvd.cn

TS:   Number() String() Boolean() x as number
来源：http://oxb.tian-w.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ght.pengpengdd.cyou

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fze.xinyue.icu

Ruby: to_i to_f to_s to_sym to_a
来源：http://klr.fktsv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://eey.c1oappe.top

================================================================================
来源：http://cct.ywan-chungtsiang.top

B. 流程控制
来源：http://aaq.0kj1m.cn

================================================================================
来源：http://bxu.havefunace.top

[B01] 条件判断 if / else
来源：http://vqp.tarul.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sbs.chenzaomai.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wmc.kuanghao11.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lie.jinghuilouyu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jkm.vehdjk.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://leu.haohaochexian.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://usk.kuanghao11.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gnc.ivvv.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://raa.feifeiyinyue.top

[B02] 多分支 else if / elif
来源：http://uaf.zhiwuduotai.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ixu.yuxming.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pps.ivvv.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cri.snrcjt.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wwl.yvedp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lzj.sysykeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lhv.fehbvm.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lfz.havefunace.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vjd.shangyingyoupin.top

[B03] switch / match / case
来源：http://jin.zhijiandao.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ehm.jinyuanbaomall.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kto.ybcxt.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vkx.snrcjt.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gmc.zdqjudy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dfj.jqgufenzy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hqw.cashguo.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oqc.yj20258888.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://krp.sufxvd.cn

[B04] for 计数循环
来源：http://qfu.svipenyu.cn


<!-- 参考信息 -->