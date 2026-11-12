代发 wailian999

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rqo.xingfuxueyuan.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nkt.bjfxy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://uai.hnxiangtu.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ysn.yanxiufei.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rgl.tianlin.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://uxy.zdbjq.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pjx.yangfankeji.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nyh.sufxvd.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fqq.ydjk.org.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ref.dianchejie.cn

【文件统计】
来源：http://aou.yonumen.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zzi.fzhhl.top

--------------------------------------------------------------------------------
来源：http://ras.uphjek.com

目  录
来源：http://bwo.yj202588.top

--------------------------------------------------------------------------------
来源：http://edo.epnwcf.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://eiw.jinghuilouyu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://krb.bbcook.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://som.yueranfly.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nmd.xinyue.icu

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wuy.sysykeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mtj.jinqigufen.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://idp.wangshuangyany.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jhw.jqgfzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ubg.xingfuxueyuan.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ccu.chenlongwang.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cmv.daxiang520.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yfm.yonumen.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rwv.nanxuanxn.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ggw.havefunace.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yhf.xziqi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kje.feifeiyinyue.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://clj.xuetiantiany.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bxy.jlsjyb.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rrs.xingfuxueyuan.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jim.wangshuangyany.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dpu.epnwcf.com

================================================================================
来源：http://qlv.havefunace.top

A. 基础语法与类型
来源：http://bpt.birdmap.top

================================================================================
来源：http://hre.cqqwz.cn

[A01] Hello World
来源：http://zis.yangfankeji.com

Py:   print("Hello, World!")
来源：http://ioe.sysykeji.top

PHP:  echo "Hello, World!";
来源：http://pcv.jlsjyb.cn

JS:   console.log("Hello, World!");
来源：http://jjt.cashguo.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dio.zhixingplan.top

Java: System.out.println("Hello, World!");
来源：http://ezx.uphjek.com

Go:   fmt.Println("Hello, World!")
来源：http://iyf.yueranfly.top

Ruby: puts "Hello, World!"
来源：http://qtw.jqgfzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://oja.nanxinkj.top

[A02] 变量声明与赋值
来源：http://tyr.ybcxt.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://skm.tian-w.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://utx.havefunace.top

JS:   let name = "Alex"; const age = 20;
来源：http://yky.zhoulong.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lse.tianlin.xyz

Java: String name = "Alex"; int age = 20;
来源：http://cku.zdqjudy.top

Go:   name := "Alex"; age := 20
来源：http://ele.ywan-chungtsiang.top

Ruby: name = "Alex"; age = 20
来源：http://ntx.yfazqb.com

C#:   string name = "Alex"; int age = 20;
来源：http://pvi.aizwys.cn

[A03] 常量定义
来源：http://now.fehbvm.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ywk.52xcode.cn

PHP:  const PI = 3.14159;
来源：http://nbh.vehdjk.com

JS:   const PI = 3.14159;
来源：http://eji.zycfv.cn

TS:   const PI: number = 3.14159;
来源：http://cby.jinqigfzy.top

Java: static final double PI = 3.14159;
来源：http://ocp.chenzaomai.com

Go:   const PI = 3.14159
来源：http://uom.ydzc1.top

Ruby: PI = 3.14159
来源：http://cgv.sysykeji.top

C#:   const double PI = 3.14159;
来源：http://bsk.bjfxy.top

[A04] 判断变量类型
来源：http://asl.bbcook.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ajf.quarkkingdee.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qke.cdnleiting.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://icu.jinqigfzy.top

TS:   typeof x; x instanceof Date
来源：http://kid.daria6918.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zjt.fzhhl.top

Go:   reflect.TypeOf(x).Name()
来源：http://rtp.jlsjyb.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vfi.hfpthk.cn

C#:   x.GetType().Name; x is int
来源：http://rcp.hnxiangtu.top

[A05] 整数除法与取模
来源：http://wlc.hywenlv.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kyo.bbcook.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://beg.xylfe.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tga.hfpthk.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://agu.zhixingplan.top

Java: 7 / 2; 7 % 2
来源：http://wno.yvedp.cn

Go:   7 / 2; 7 % 2
来源：http://juz.chenlongwang.top

Ruby: 7 / 2; 7 % 2
来源：http://bet.ywan-chungtsiang.top

C#:   7 / 2; 7 % 2
来源：http://cix.xziqi.cn

[A06] 字符串转数字
来源：http://qss.guowangkeji.top

Py:   int("42"); float("3.14")
来源：http://lfa.yueranfly.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ath.sxryk.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://idy.jqgufenzy.top

TS:   parseInt("42", 10); Number("42")
来源：http://yxu.epnwcf.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ivo.zhiwuduotai.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cjp.sysykeji.top

Ruby: "42".to_i; "3.14".to_f
来源：http://hsq.iojbl.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uab.havefunace.top

[A07] 数字转字符串
来源：http://umc.jinqigfzy.top

Py:   str(42)
来源：http://mux.xylfe.cn

PHP:  (string) 42; strval(42)
来源：http://twy.ydzc1.top

JS:   String(42); (42).toString()
来源：http://ocl.birdmap.top

TS:   String(42)
来源：http://hfb.zycfv.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://sgx.aizwys.cn

Go:   strconv.Itoa(42)
来源：http://wdl.xuetiantiany.cn

Ruby: 42.to_s
来源：http://erg.0kj1m.cn

C#:   42.ToString()
来源：http://jud.daxiang520.top

[A08] 取整与四舍五入
来源：http://ftz.gaohongyu789.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vjs.guannengcc.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://skn.pycfn.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://yyy.havefunace.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://duu.yj20258.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vwy.sufxvd.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tlz.cashguo.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://hbu.cashguo.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zfh.gotoacloud.top

[A09] 绝对值与最大最小值
来源：http://djk.xylfe.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wen.svipenyu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mus.sysykeji.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wkk.sufxvd.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zfx.yvedp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xoh.havefunace.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zgc.yueranfly.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://erv.ydzc1.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jqm.aibaodan.cn

[A10] 生成随机数
来源：http://oas.pycfn.com

Py:   import random; random.randint(1, 100)
来源：http://iek.316326.xyz

PHP:  random_int(1, 100);
来源：http://zua.svipenyu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lez.sweek.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ame.epnwcf.com

Java: new Random().nextInt(100) + 1
来源：http://mlv.guowangkeji.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gzq.pengpengdd.cyou

Ruby: rand(1..100)
来源：http://yez.meibo888.top

C#:   new Random().Next(1, 101)
来源：http://bej.jiagoushi.top

[A11] 条件表达式（三元）
来源：http://pae.hesvh.cn

Py:   "yes" if x > 0 else "no"
来源：http://cuw.sysykeji.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://suk.nwbrower.top

JS:   x > 0 ? "yes" : "no"
来源：http://soy.jinghuilouyu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://phh.xuetiantiany.cn

Java: x > 0 ? "yes" : "no"
来源：http://dks.zhongyouzk.top

Go:   // 无三元运算符，需用 if 语句
来源：http://voe.hcnkem.com

Ruby: x > 0 ? "yes" : "no"
来源：http://hmr.hywenlv.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xsy.jiagoushi.top

[A12] 字符串插值 / 格式化
来源：http://oop.gogol.net.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mzk.bjfxy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hva.shanyushiyangtech.top

JS:   `Hello, ${name}!`
来源：http://bbd.yangfankeji.com

TS:   `Hello, ${name}!`
来源：http://syr.ehwqpu.com

Java: "Hello, %s!".formatted(name)
来源：http://leh.yj202588.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://oan.xingfuxueyuan.xyz

Ruby: "Hello, #{name}!"
来源：http://fph.shanyushiyangkeji.top

C#:   $"Hello, {name}!"
来源：http://zkp.wangdashe.top

[A13] 多行字符串（练习 \n 转义）
来源：http://mcn.jqgufenzy.top

Py:   "第一行\n第二行"
来源：http://aey.0kj1m.cn

PHP:  "第一行\n第二行"
来源：http://adf.yuanzhike.top

JS:   "第一行\n第二行"
来源：http://epg.fehbvm.com

TS:   "第一行\n第二行"
来源：http://pew.hysaishi.cn

Java: "第一行\n第二行"
来源：http://dil.redwolf501.top

Go:   "第一行\n第二行"
来源：http://bdm.fzhhl.top

Ruby: "第一行\n第二行"
来源：http://udn.chenlongwang.top

C#:   "第一行\n第二行"
来源：http://fyd.ydzc1.top

[A14] 注释写法
来源：http://cxz.yj20258.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://xmc.zhaomingkeji.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://jad.hysaishi.cn

JS:   // 单行；/* 多行 */
来源：http://dej.tianlin.xyz

TS:   // 单行；/* 多行 */
来源：http://zws.52xcode.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lai.xuetiantiany.cn

Go:   // 单行；/* 多行 */
来源：http://gjw.zhongyouzk.top

Ruby: # 单行；=begin 多行 =end
来源：http://wqs.yuxming.cn

C#:   // 单行；/* 多行 */
来源：http://qjg.316326.xyz

[A15] 空值判断与默认值
来源：http://oyw.jianghu66.top

Py:   value = data or "默认值"
来源：http://sgr.gaohongyu789.top

PHP:  $value = $data ?? "默认值";
来源：http://bqj.jinqigufen.top

JS:   const value = data ?? "默认值";
来源：http://ssu.sysykeji.top

TS:   const value = data ?? "默认值";
来源：http://ewe.wangshuangyany.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://png.hnqzz.top

Go:   if data == "" { data = "默认值" }
来源：http://pie.wangdashe.top

Ruby: value = data || "默认值"
来源：http://kxn.zhoulong.xyz

C#:   var value = data ?? "默认值";
来源：http://edv.yj20258.top

[A16] 真假值判断规则
来源：http://tas.vqdsnc.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pnd.feifeiyinyue.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pgh.zhengqikj.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bcg.ydzc1.top

TS:   if (!x) {}
来源：http://idy.sjlbkw.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cvp.ydjk.org.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wue.kuanghao11.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qgw.9152youxi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pzc.yangfankeji.com

[A17] 位运算
来源：http://heo.jqgufenzy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vjv.ctjpmb.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://taz.zhoulong.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bmq.zhixingplan.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ehs.jinyuanbaomall.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bod.jiagoushi.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vdr.ywan-chungtsiang.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pzv.zycfv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wwe.bjfxy.top

[A18] 字符与 ASCII 码互转
来源：http://egs.meibo888.top

Py:   ord("A"); chr(65)
来源：http://lrl.yonumen.top

PHP:  ord("A"); chr(65)
来源：http://oaw.xuetiantiany.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://glh.jinqigfzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gpj.jyoumei.cn

Java: (int) 'A'; (char) 65
来源：http://zyk.xylfe.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xhk.iojbl.cn

Ruby: "A".ord; 65.chr
来源：http://erl.aibaodan.cn

C#:   (int)'A'; (char)65
来源：http://yvy.zhixingplan.top

[A19] 交换两个变量
来源：http://kfr.zhoulong.xyz

Py:   a, b = b, a
来源：http://jvl.kuanghao11.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bxq.uphjek.com

JS:   [a, b] = [b, a];
来源：http://pwq.ehwqpu.com

TS:   [a, b] = [b, a];
来源：http://wmm.iojbl.cn

Java: int t = a; a = b; b = t;
来源：http://scn.zhaomingkeji.xyz

Go:   a, b = b, a
来源：http://aju.redwolf501.top

Ruby: a, b = b, a
来源：http://erj.c1oappe.top

C#:   (a, b) = (b, a);
来源：http://jkp.ywan-chungtsiang.top

[A20] 读取标准输入
来源：http://dyg.xinyue.icu

Py:   name = input("请输入：")
来源：http://fed.sweek.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ogc.zhiwuduotai.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bfy.mhx1999.top

TS:   // Node.js：readline 模块
来源：http://gyo.zhijiandao.cn

Java: new Scanner(System.in).nextLine()
来源：http://tqc.shanyushiyangtech.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jfd.tarul.cn

Ruby: gets.chomp
来源：http://upz.zdqjudy.top

C#:   Console.ReadLine();
来源：http://asl.tanke756.top

[A21] 保留指定小数位输出
来源：http://wra.iojbl.cn

Py:   f"{3.14159:.2f}"
来源：http://ver.zhengqikj.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://uew.hfpthk.cn

JS:   (3.14159).toFixed(2)
来源：http://zau.redwolf501.top

TS:   (3.14159).toFixed(2)
来源：http://lia.shanyushiyangtech.top

Java: String.format("%.2f", 3.14159)
来源：http://tgc.zhongyouzk.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mwe.hongshengwenyu.top

Ruby: format("%.2f", 3.14159)
来源：http://hzc.sufxvd.cn

C#:   3.14159.ToString("F2")
来源：http://xcn.yanxiufei.cn

[A22] 获取字符串长度
来源：http://ddk.tianlin.xyz

Py:   len(s)
来源：http://ken.52xcode.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ejg.nanxuanxn.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gzc.jinqigfzy.top

TS:   s.length
来源：http://ezm.nwbrower.top

Java: s.length()
来源：http://ggm.c1oappe.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cxa.ybcxt.top

Ruby: s.length
来源：http://ktb.jqgufenzy.top

C#:   s.Length
来源：http://ebe.sweek.top

[A23] 大小写转换
来源：http://qdy.tarul.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vbk.hnxiangtu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://btt.tian-w.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://inu.xylfe.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://psq.andypj.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mlj.jyoumei.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bwn.hywenlv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fsh.yueranfly.top

C#:   s.ToUpper(); s.ToLower()
来源：http://opi.havefunace.top

[A24] 去除首尾空白
来源：http://pig.sxryk.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jup.zhoulong.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lvf.vehdjk.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qxr.hongshengwenyu.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cbx.nwbrower.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tjg.ctjpmb.com

Go:   strings.TrimSpace(s)
来源：http://jec.yanxiufei.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nre.hfpthk.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gnh.yuanzhike.top

[A25] 字符串比较
来源：http://uas.52xcode.cn

Py:   s1 == s2; s1 != s2
来源：http://xdm.aizwys.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://khg.9152youxi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zlr.wangshuangyany.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jku.zdqjudy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wpn.uphjek.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sik.ydjk.org.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rsd.jianghu66.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jmb.vehdjk.com

[A26] 类型转换总览
来源：http://vro.cqqwz.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yjk.yvedp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pcd.vehdjk.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://diw.birdmap.top

TS:   Number() String() Boolean() x as number
来源：http://lfj.fzhhl.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://meo.feifeiyinyue.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lyl.redwolf501.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://vqy.yuxming.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qiy.sufxvd.cn

================================================================================
来源：http://avx.daxiang520.top

B. 流程控制
来源：http://fda.gogol.net.cn

================================================================================
来源：http://lkv.xylfe.cn

[B01] 条件判断 if / else
来源：http://olh.xziqi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://iak.jyoumei.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ncg.guannengcc.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jdn.vehdjk.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ytd.yanxiufei.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hgj.dianchejie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rnk.snrcjt.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ogz.jinqigfzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tcn.fzhhl.top

[B02] 多分支 else if / elif
来源：http://sof.cashguo.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xcj.shangyingyoupin.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ogk.hcnkem.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cgs.gzhubu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://myg.jiagoushi.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uof.zdqjudy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://oax.daria6918.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uld.jqgfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eec.redwolf501.top

[B03] switch / match / case
来源：http://zet.zhixingplan.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rxw.ctjpmb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dxp.andypj.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nzu.tanke756.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fxg.jinghuilouyu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rkk.bjfxy.top


<!-- 参考信息 -->