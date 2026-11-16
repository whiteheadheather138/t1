代发 wailian999

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zlg.sjlbkw.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://peu.xingfuxueyuan.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://qta.0kj1m.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dmt.cashguo.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yxm.yvedp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qds.wangshuangyany.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ire.xinyue.icu

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://grj.yuanzhike.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://swo.zycfv.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xzo.zhixingplan.top

【文件统计】
来源：http://ano.yj20258888.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://stn.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://voa.feifeiyinyue.top

目  录
来源：http://jvo.iojbl.cn

--------------------------------------------------------------------------------
来源：http://axj.chenzaomai.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lxo.xylfe.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vyt.yanxiufei.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cee.zdqjudy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zxi.cdnleiting.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cfa.tian-w.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lbq.xinyue.icu

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kfs.uphjek.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wlb.epnwcf.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jwh.redwolf501.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bom.hesvh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://phg.gaohongyu789.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wdx.316326.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sbl.snrcjt.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mix.hysaishi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ezb.tian-w.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bnj.cqqwz.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zei.shzxlz.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gjv.shzxlz.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dll.ybcxt.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uuk.xuetiantiany.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uiq.shanyushiyangkeji.top

================================================================================
来源：http://zjm.dianchejie.cn

A. 基础语法与类型
来源：http://mby.c1oappe.top

================================================================================
来源：http://rea.ivvv.top

[A01] Hello World
来源：http://upe.yj20258888.top

Py:   print("Hello, World!")
来源：http://kez.shzxlz.cn

PHP:  echo "Hello, World!";
来源：http://roz.redwolf501.top

JS:   console.log("Hello, World!");
来源：http://bsw.zhongyouzk.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hrh.yonumen.top

Java: System.out.println("Hello, World!");
来源：http://crl.ydjk.org.cn

Go:   fmt.Println("Hello, World!")
来源：http://egu.yongpay.top

Ruby: puts "Hello, World!"
来源：http://qjj.ydjk.org.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ijz.cashguo.top

[A02] 变量声明与赋值
来源：http://vik.zhengqikj.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ubc.sxryk.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mvn.zdbjq.cn

JS:   let name = "Alex"; const age = 20;
来源：http://opu.jqgufenzy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://eiw.jqgfzy.top

Java: String name = "Alex"; int age = 20;
来源：http://vkc.andypj.xyz

Go:   name := "Alex"; age := 20
来源：http://ssh.vqdsnc.cn

Ruby: name = "Alex"; age = 20
来源：http://btz.smart0.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://vhf.ydjk.org.cn

[A03] 常量定义
来源：http://heh.fzhhl.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://udu.gzhubu.top

PHP:  const PI = 3.14159;
来源：http://cgu.shuidangran.top

JS:   const PI = 3.14159;
来源：http://qhb.dianchejie.cn

TS:   const PI: number = 3.14159;
来源：http://pxl.andypj.xyz

Java: static final double PI = 3.14159;
来源：http://quh.9152youxi.cn

Go:   const PI = 3.14159
来源：http://bxi.ybcxt.top

Ruby: PI = 3.14159
来源：http://nil.svipenyu.cn

C#:   const double PI = 3.14159;
来源：http://zcv.tian-w.cn

[A04] 判断变量类型
来源：http://jxy.cucudq.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qnm.tian-w.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ehy.sufxvd.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://atz.xuanzx.com

TS:   typeof x; x instanceof Date
来源：http://xny.yanxiufei.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wpa.tianlin.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://erq.zhengqikj.top

Ruby: x.class; x.is_a?(Integer)
来源：http://slp.zhengqikj.top

C#:   x.GetType().Name; x is int
来源：http://jla.jyoumei.cn

[A05] 整数除法与取模
来源：http://vef.wangdashe.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dji.chenjidiqi.icu

PHP:  intdiv(7, 2); 7 % 2
来源：http://qfp.zhoulong.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nfk.uphjek.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xwo.jqgfzy.top

Java: 7 / 2; 7 % 2
来源：http://hoj.vehdjk.com

Go:   7 / 2; 7 % 2
来源：http://cjv.hywenlv.cn

Ruby: 7 / 2; 7 % 2
来源：http://prc.hammf.cn

C#:   7 / 2; 7 % 2
来源：http://utf.cashguo.top

[A06] 字符串转数字
来源：http://hei.yvedp.cn

Py:   int("42"); float("3.14")
来源：http://pwu.wangdashe.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qek.nanxinkj.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blg.jinqigufen.top

TS:   parseInt("42", 10); Number("42")
来源：http://dpg.chenlongwang.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vlv.sufxvd.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rnl.zhijiandao.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ady.feifeiyinyue.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nww.fengsongda.top

[A07] 数字转字符串
来源：http://utp.svipenyu.cn

Py:   str(42)
来源：http://kzr.xuetiantiany.cn

PHP:  (string) 42; strval(42)
来源：http://vqc.daxiang520.top

JS:   String(42); (42).toString()
来源：http://kwn.fehbvm.com

TS:   String(42)
来源：http://srk.cashguo.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://gcy.fanxiaobao.xyz

Go:   strconv.Itoa(42)
来源：http://kow.tanke756.top

Ruby: 42.to_s
来源：http://som.xuetiantiany.cn

C#:   42.ToString()
来源：http://hks.shanyushiyangtech.top

[A08] 取整与四舍五入
来源：http://zcq.cqqwz.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zdi.jinyuanbaomall.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lob.jqgufenzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xlj.jyoumei.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rga.yfazqb.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bhc.hcnkem.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dzl.hnqzz.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://gca.gzhubu.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rff.sxryk.cn

[A09] 绝对值与最大最小值
来源：http://uyr.daxiang520.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tfi.kuanghao11.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://teh.redwolf501.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qwe.iojbl.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qlt.cqqwz.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lop.svipenyu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://iyw.gzhubu.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vml.guowangkeji.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jgb.jinqigufen.top

[A10] 生成随机数
来源：http://dvt.yanxiufei.cn

Py:   import random; random.randint(1, 100)
来源：http://tjk.xziqi.cn

PHP:  random_int(1, 100);
来源：http://xaj.ivvv.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ebj.jinqigfzy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hpf.jiagoushi.top

Java: new Random().nextInt(100) + 1
来源：http://tst.hnxiangtu.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jqo.cucudq.cn

Ruby: rand(1..100)
来源：http://qkn.jinghuilouyu.cn

C#:   new Random().Next(1, 101)
来源：http://fof.jqgfzy.top

[A11] 条件表达式（三元）
来源：http://oeq.xylfe.cn

Py:   "yes" if x > 0 else "no"
来源：http://gkw.xuetiantiany.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://lzi.ivvv.top

JS:   x > 0 ? "yes" : "no"
来源：http://shj.havefunace.top

TS:   x > 0 ? "yes" : "no"
来源：http://lnh.cqqwz.cn

Java: x > 0 ? "yes" : "no"
来源：http://bcd.kuanghao11.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mnl.hnqzz.top

Ruby: x > 0 ? "yes" : "no"
来源：http://khf.ydzc1.top

C#:   x > 0 ? "yes" : "no"
来源：http://ntn.jinqigfzy.top

[A12] 字符串插值 / 格式化
来源：http://kux.shzxlz.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kmq.fehbvm.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://osi.zdbjq.cn

JS:   `Hello, ${name}!`
来源：http://fjv.cheryme.top

TS:   `Hello, ${name}!`
来源：http://zzo.shanyushiyangtech.top

Java: "Hello, %s!".formatted(name)
来源：http://lsb.nanxuanxn.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ieh.tarul.cn

Ruby: "Hello, #{name}!"
来源：http://uzm.nwbrower.top

C#:   $"Hello, {name}!"
来源：http://bhh.tianlin.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://hiw.sufxvd.cn

Py:   "第一行\n第二行"
来源：http://rqc.andypj.xyz

PHP:  "第一行\n第二行"
来源：http://fpp.pengpengdd.cyou

JS:   "第一行\n第二行"
来源：http://eec.gzhubu.top

TS:   "第一行\n第二行"
来源：http://ywm.hammf.cn

Java: "第一行\n第二行"
来源：http://bcg.guannengcc.top

Go:   "第一行\n第二行"
来源：http://kdj.sjlbkw.cn

Ruby: "第一行\n第二行"
来源：http://luz.gzhubu.top

C#:   "第一行\n第二行"
来源：http://uon.zhoulong.xyz

[A14] 注释写法
来源：http://bre.c1oappe.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ziw.zhoulong.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://vit.jqgfzy.top

JS:   // 单行；/* 多行 */
来源：http://zop.fehbvm.com

TS:   // 单行；/* 多行 */
来源：http://sjn.jqgfzy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://emn.nwbrower.top

Go:   // 单行；/* 多行 */
来源：http://itj.feifeiyinyue.top

Ruby: # 单行；=begin 多行 =end
来源：http://irj.hfpthk.cn

C#:   // 单行；/* 多行 */
来源：http://cqf.andypj.xyz

[A15] 空值判断与默认值
来源：http://zoj.wangshuangyany.cn

Py:   value = data or "默认值"
来源：http://pjx.jianghu66.top

PHP:  $value = $data ?? "默认值";
来源：http://thk.yonumen.top

JS:   const value = data ?? "默认值";
来源：http://tle.haohaochexian.top

TS:   const value = data ?? "默认值";
来源：http://gww.jlsjyb.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dbz.zhiwuduotai.top

Go:   if data == "" { data = "默认值" }
来源：http://mhn.xuanzx.com

Ruby: value = data || "默认值"
来源：http://gru.bbcook.cn

C#:   var value = data ?? "默认值";
来源：http://sao.nanxinkj.top

[A16] 真假值判断规则
来源：http://loo.hcnkem.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vzj.shanyushiyangkeji.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gaf.zhijiandao.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tee.hongshengwenyu.top

TS:   if (!x) {}
来源：http://jij.feifeiyinyue.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zrq.ydzc1.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fzn.shangyingyoupin.top

Ruby: unless x            # nil 与 false 为假
来源：http://dba.mhx1999.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qfc.jqgfzy.top

[A17] 位运算
来源：http://bxw.sxryk.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xbd.316326.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://eza.jiagoushi.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gyl.zhaomingkeji.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jrz.hcnkem.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bkm.dashuyun.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xes.9152youxi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qzx.chenzaomai.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tgk.vqdsnc.cn

[A18] 字符与 ASCII 码互转
来源：http://wkt.ydzc1.top

Py:   ord("A"); chr(65)
来源：http://uip.zhiwuduotai.top

PHP:  ord("A"); chr(65)
来源：http://mqw.dashuyun.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bbf.yuanzhike.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iem.shzxlz.cn

Java: (int) 'A'; (char) 65
来源：http://kbm.sxryk.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vaf.zhixingplan.top

Ruby: "A".ord; 65.chr
来源：http://rco.kuanghao11.cn

C#:   (int)'A'; (char)65
来源：http://yfx.hammf.cn

[A19] 交换两个变量
来源：http://zay.jianghu66.top

Py:   a, b = b, a
来源：http://gou.bjfxy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://eyp.nanxuanxn.top

JS:   [a, b] = [b, a];
来源：http://rej.nanxuanxn.top

TS:   [a, b] = [b, a];
来源：http://sgc.kuanghao11.cn

Java: int t = a; a = b; b = t;
来源：http://pew.yonumen.top

Go:   a, b = b, a
来源：http://sql.dashuyun.cn

Ruby: a, b = b, a
来源：http://nxf.52xcode.cn

C#:   (a, b) = (b, a);
来源：http://nbo.daria6918.cn

[A20] 读取标准输入
来源：http://eif.vqdsnc.cn

Py:   name = input("请输入：")
来源：http://omx.hesvh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://fcp.shzxlz.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wzh.nwbrower.top

TS:   // Node.js：readline 模块
来源：http://xkg.jyoumei.cn

Java: new Scanner(System.in).nextLine()
来源：http://bhm.gotoacloud.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ztn.jinqigfzy.top

Ruby: gets.chomp
来源：http://pah.gogol.net.cn

C#:   Console.ReadLine();
来源：http://mbz.xinyue.icu

[A21] 保留指定小数位输出
来源：http://lvc.yuanzhike.top

Py:   f"{3.14159:.2f}"
来源：http://rcz.gotoacloud.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qpj.vqdsnc.cn

JS:   (3.14159).toFixed(2)
来源：http://pgn.pycfn.com

TS:   (3.14159).toFixed(2)
来源：http://yzj.xinyue.icu

Java: String.format("%.2f", 3.14159)
来源：http://cdg.snrcjt.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sbq.xuetiantiany.cn

Ruby: format("%.2f", 3.14159)
来源：http://qib.shuidangran.top

C#:   3.14159.ToString("F2")
来源：http://zhn.316326.xyz

[A22] 获取字符串长度
来源：http://itx.xuanzx.com

Py:   len(s)
来源：http://iju.yuanzhike.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mxw.yueranfly.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zwr.fanxiaobao.xyz

TS:   s.length
来源：http://vhk.fanxiaobao.xyz

Java: s.length()
来源：http://nma.uphjek.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://php.pycfn.com

Ruby: s.length
来源：http://iws.aibaodan.cn

C#:   s.Length
来源：http://xkq.jlsjyb.cn

[A23] 大小写转换
来源：http://rec.cdnleiting.top

Py:   s.upper(); s.lower(); s.title()
来源：http://eam.yanxiufei.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xtn.yvedp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hwm.quarkkingdee.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rjl.ppjwa.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hom.yuanzhike.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://iub.jqgfzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://byl.daxiang520.top

C#:   s.ToUpper(); s.ToLower()
来源：http://xbr.ctjpmb.com

[A24] 去除首尾空白
来源：http://zuz.0kj1m.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sbk.cdnleiting.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://eac.c1oappe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rki.zhixingplan.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ivy.havefunace.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lzl.jinyuanbaomall.cn

Go:   strings.TrimSpace(s)
来源：http://rqm.hesvh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jdl.fehbvm.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rog.shanyushiyangkeji.top

[A25] 字符串比较
来源：http://wbt.fzhhl.top

Py:   s1 == s2; s1 != s2
来源：http://pcn.smart0.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ysh.jiagoushi.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nnh.shangyingyoupin.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://whl.zhoulong.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://syb.epnwcf.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dlf.dashuyun.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://flw.tianlin.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cui.yuanzhike.top

[A26] 类型转换总览
来源：http://gjp.gaohongyu789.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gif.jqgfzy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dke.xingfuxueyuan.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bsb.zhengqikj.top

TS:   Number() String() Boolean() x as number
来源：http://kja.hysaishi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://udw.sxryk.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hub.cdnleiting.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://lfa.vehdjk.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oxh.fzhhl.top

================================================================================
来源：http://lsg.sjlbkw.cn

B. 流程控制
来源：http://oso.guannengcc.top

================================================================================
来源：http://nro.hammf.cn

[B01] 条件判断 if / else
来源：http://vvx.snrcjt.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bvh.ybcxt.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sbn.ctjpmb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kyr.ivvv.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tcy.jinghuilouyu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dwh.ctjpmb.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wnk.0kj1m.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://iqi.snrcjt.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rkt.mhx1999.top

[B02] 多分支 else if / elif
来源：http://eip.ivvv.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ova.ybcxt.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yrb.ywan-chungtsiang.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xzk.tanke756.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gtm.daria6918.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pxe.bjfxy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mie.fengsongda.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kat.c1oappe.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uov.ywan-chungtsiang.top

[B03] switch / match / case
来源：http://suc.smart0.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vpq.hywenlv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fil.fzhhl.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://prv.jinqigufen.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ttl.yanxiufei.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ots.yj202588.top


<!-- 参考信息 -->