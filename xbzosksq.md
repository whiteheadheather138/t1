代发 wailian999

--------------------------------------------------------------------------------
来源：http://xmp.vqdsnc.cn

目  录
来源：http://mfx.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://fjs.snrcjt.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wan.sjlbkw.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dhg.jiagoushi.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lir.kuanghao11.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vgp.zhoulong.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qph.birdmap.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://puv.tian-w.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://stq.tanke756.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zgw.zhaomingkeji.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gcp.sysykeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cyp.sweek.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lue.fengsongda.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uin.ivvv.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://iqg.jinghuilouyu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gfs.xuanzx.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gnf.wangshuangyany.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mgq.jqgufenzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://oxs.yuanzhike.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ekr.zhongyouzk.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ssv.jqgfzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://omh.yangfankeji.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ohi.cucudq.cn

================================================================================
来源：http://eed.ybcxt.top

A. 基础语法与类型
来源：http://aut.hywenlv.cn

================================================================================
来源：http://iok.zycfv.cn

[A01] Hello World
来源：http://clz.hysaishi.cn

Py:   print("Hello, World!")
来源：http://saz.pengpengdd.cyou

PHP:  echo "Hello, World!";
来源：http://zrq.fengsongda.top

JS:   console.log("Hello, World!");
来源：http://ffk.yfazqb.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jve.pengpengdd.cyou

Java: System.out.println("Hello, World!");
来源：http://cgi.jqgufenzy.top

Go:   fmt.Println("Hello, World!")
来源：http://cds.ppjwa.cn

Ruby: puts "Hello, World!"
来源：http://pcb.yj20258.top

C#:   Console.WriteLine("Hello, World!");
来源：http://rnp.yanxiufei.cn

[A02] 变量声明与赋值
来源：http://krb.0kj1m.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cbb.mhx1999.top

PHP:  $name = "Alex"; $age = 20;
来源：http://shd.jinyuanbaomall.cn

JS:   let name = "Alex"; const age = 20;
来源：http://oyn.uphjek.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kjb.guannengcc.top

Java: String name = "Alex"; int age = 20;
来源：http://pte.bbcook.cn

Go:   name := "Alex"; age := 20
来源：http://tsb.bjfxy.top

Ruby: name = "Alex"; age = 20
来源：http://xxa.nanxinkj.top

C#:   string name = "Alex"; int age = 20;
来源：http://vmc.nanxinkj.top

[A03] 常量定义
来源：http://zid.iojbl.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bkg.kuanghao11.cn

PHP:  const PI = 3.14159;
来源：http://hcv.ydjk.org.cn

JS:   const PI = 3.14159;
来源：http://zyr.yongpay.top

TS:   const PI: number = 3.14159;
来源：http://wjr.jinqigufen.top

Java: static final double PI = 3.14159;
来源：http://efn.zhongyouzk.top

Go:   const PI = 3.14159
来源：http://djo.fktsv.cn

Ruby: PI = 3.14159
来源：http://gpx.chenlongwang.top

C#:   const double PI = 3.14159;
来源：http://njl.sysykeji.top

[A04] 判断变量类型
来源：http://mgx.yonumen.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://vhl.xylfe.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wdk.zhoulong.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wvz.cashguo.top

TS:   typeof x; x instanceof Date
来源：http://vka.c1oappe.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vgo.tarul.cn

Go:   reflect.TypeOf(x).Name()
来源：http://erf.nanxuanxn.top

Ruby: x.class; x.is_a?(Integer)
来源：http://zlw.yuxming.cn

C#:   x.GetType().Name; x is int
来源：http://tjb.epnwcf.com

[A05] 整数除法与取模
来源：http://ihl.sweek.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://uxr.ctjpmb.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://ksl.ppjwa.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wpw.svipenyu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qcg.wangdashe.top

Java: 7 / 2; 7 % 2
来源：http://flk.shanyushiyangkeji.top

Go:   7 / 2; 7 % 2
来源：http://zbb.epnwcf.com

Ruby: 7 / 2; 7 % 2
来源：http://aob.xuetiantiany.cn

C#:   7 / 2; 7 % 2
来源：http://ewf.zhaomingkeji.xyz

[A06] 字符串转数字
来源：http://oni.birdmap.top

Py:   int("42"); float("3.14")
来源：http://ucg.yj202588.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://srw.kuanghao11.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hur.hnxiangtu.top

TS:   parseInt("42", 10); Number("42")
来源：http://ykk.xziqi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://afk.bjfxy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xyv.dianchejie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hcr.tarul.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xgl.cheryme.top

[A07] 数字转字符串
来源：http://exq.yj202588.top

Py:   str(42)
来源：http://vvy.yueranfly.top

PHP:  (string) 42; strval(42)
来源：http://reb.xuetiantiany.cn

JS:   String(42); (42).toString()
来源：http://pay.zdbjq.cn

TS:   String(42)
来源：http://nvk.yuxming.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xsk.hesvh.cn

Go:   strconv.Itoa(42)
来源：http://vkv.zhengqikj.top

Ruby: 42.to_s
来源：http://pdp.zdqjudy.top

C#:   42.ToString()
来源：http://zdh.hysaishi.cn

[A08] 取整与四舍五入
来源：http://lrl.zdbjq.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xve.ydzc1.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://psp.shuidangran.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gtv.sufxvd.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wrp.daxiang520.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zkz.yj20258888.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://foh.jyoumei.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://neq.ywan-chungtsiang.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xcs.yfazqb.com

[A09] 绝对值与最大最小值
来源：http://wmq.gaohongyu789.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://shx.cqqwz.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yuo.hesvh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gcl.xinyue.icu

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lyx.jinyuanbaomall.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://krn.316326.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ujx.xuanzx.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yzr.mhx1999.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qxj.shanyushiyangkeji.top

[A10] 生成随机数
来源：http://uwu.andypj.xyz

Py:   import random; random.randint(1, 100)
来源：http://pze.xziqi.cn

PHP:  random_int(1, 100);
来源：http://tbx.bbcook.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rsf.hcnkem.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wrl.chenjidiqi.icu

Java: new Random().nextInt(100) + 1
来源：http://edb.svipenyu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fgh.yuanzhike.top

Ruby: rand(1..100)
来源：http://tlf.tarul.cn

C#:   new Random().Next(1, 101)
来源：http://ksu.shangyingyoupin.top

[A11] 条件表达式（三元）
来源：http://lte.chenjidiqi.icu

Py:   "yes" if x > 0 else "no"
来源：http://lrt.bbcook.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://tgn.nanxinkj.top

JS:   x > 0 ? "yes" : "no"
来源：http://vrb.gotoacloud.top

TS:   x > 0 ? "yes" : "no"
来源：http://kyh.jinghuilouyu.cn

Java: x > 0 ? "yes" : "no"
来源：http://ayz.shanyushiyangkeji.top

Go:   // 无三元运算符，需用 if 语句
来源：http://sdh.sjlbkw.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bnd.feifeiyinyue.top

C#:   x > 0 ? "yes" : "no"
来源：http://bqy.jiagoushi.top

[A12] 字符串插值 / 格式化
来源：http://wrj.shanyushiyangtech.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bcg.tian-w.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wqf.tarul.cn

JS:   `Hello, ${name}!`
来源：http://ywi.guowangkeji.top

TS:   `Hello, ${name}!`
来源：http://xlg.mhx1999.top

Java: "Hello, %s!".formatted(name)
来源：http://cow.cashguo.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://iub.ppjwa.cn

Ruby: "Hello, #{name}!"
来源：http://wmr.cheryme.top

C#:   $"Hello, {name}!"
来源：http://ovo.bjfxy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://whz.gaohongyu789.top

Py:   "第一行\n第二行"
来源：http://kqf.ydzc1.top

PHP:  "第一行\n第二行"
来源：http://jig.zdbjq.cn

JS:   "第一行\n第二行"
来源：http://cyx.zhengqikj.top

TS:   "第一行\n第二行"
来源：http://rmr.hammf.cn

Java: "第一行\n第二行"
来源：http://xxb.hammf.cn

Go:   "第一行\n第二行"
来源：http://tka.jinqigufen.top

Ruby: "第一行\n第二行"
来源：http://tzo.dianchejie.cn

C#:   "第一行\n第二行"
来源：http://yyb.sweek.top

[A14] 注释写法
来源：http://kvq.ppjwa.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yqo.hywenlv.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://nhz.tian-w.cn

JS:   // 单行；/* 多行 */
来源：http://zuq.meibo888.top

TS:   // 单行；/* 多行 */
来源：http://iuw.cashguo.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mxa.iojbl.cn

Go:   // 单行；/* 多行 */
来源：http://ndq.jiagoushi.top

Ruby: # 单行；=begin 多行 =end
来源：http://uth.pengpengdd.cyou

C#:   // 单行；/* 多行 */
来源：http://erm.xuanzx.com

[A15] 空值判断与默认值
来源：http://lxq.nanxuanxn.top

Py:   value = data or "默认值"
来源：http://ohy.ydjk.org.cn

PHP:  $value = $data ?? "默认值";
来源：http://jbh.chenzaomai.com

JS:   const value = data ?? "默认值";
来源：http://xcf.cucudq.cn

TS:   const value = data ?? "默认值";
来源：http://epb.kuanghao11.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://evo.zycfv.cn

Go:   if data == "" { data = "默认值" }
来源：http://hce.kuanghao11.cn

Ruby: value = data || "默认值"
来源：http://wox.cqqwz.cn

C#:   var value = data ?? "默认值";
来源：http://iox.daria6918.cn

[A16] 真假值判断规则
来源：http://was.nanxinkj.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dzs.tarul.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ugo.zdqjudy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ecg.wangdashe.top

TS:   if (!x) {}
来源：http://wve.wangdashe.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qnx.aizwys.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ztx.wangdashe.top

Ruby: unless x            # nil 与 false 为假
来源：http://pru.cheryme.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nyy.bjfxy.top

[A17] 位运算
来源：http://yso.yonumen.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pcg.nanxinkj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nea.zycfv.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://add.gzhubu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bcz.zhengqikj.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bcx.tianlin.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bfi.zdqjudy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hxz.svipenyu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lkq.meibo888.top

[A18] 字符与 ASCII 码互转
来源：http://uxq.dianchejie.cn

Py:   ord("A"); chr(65)
来源：http://uhw.0kj1m.cn

PHP:  ord("A"); chr(65)
来源：http://mwi.meibo888.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://odm.dianchejie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tcg.tanke756.top

Java: (int) 'A'; (char) 65
来源：http://cfh.ywan-chungtsiang.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wkj.guannengcc.top

Ruby: "A".ord; 65.chr
来源：http://yne.tianlin.xyz

C#:   (int)'A'; (char)65
来源：http://zln.fktsv.cn

[A19] 交换两个变量
来源：http://hxm.xinyue.icu

Py:   a, b = b, a
来源：http://hur.fktsv.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vhq.sjlbkw.cn

JS:   [a, b] = [b, a];
来源：http://dkd.kuanghao11.cn

TS:   [a, b] = [b, a];
来源：http://oep.hysaishi.cn

Java: int t = a; a = b; b = t;
来源：http://hwu.meibo888.top

Go:   a, b = b, a
来源：http://yjo.hammf.cn

Ruby: a, b = b, a
来源：http://tjt.nwbrower.top

C#:   (a, b) = (b, a);
来源：http://eqm.ywan-chungtsiang.top

[A20] 读取标准输入
来源：http://vcx.vqdsnc.cn

Py:   name = input("请输入：")
来源：http://cnm.smart0.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://emb.feifeiyinyue.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dlz.redwolf501.top

TS:   // Node.js：readline 模块
来源：http://gwa.zdbjq.cn

Java: new Scanner(System.in).nextLine()
来源：http://rii.shzxlz.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ynt.zycfv.cn

Ruby: gets.chomp
来源：http://sqi.dashuyun.cn

C#:   Console.ReadLine();
来源：http://tay.haohaochexian.top

[A21] 保留指定小数位输出
来源：http://lud.epnwcf.com

Py:   f"{3.14159:.2f}"
来源：http://dlp.cashguo.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cvx.iojbl.cn

JS:   (3.14159).toFixed(2)
来源：http://igc.52xcode.cn

TS:   (3.14159).toFixed(2)
来源：http://bhf.uphjek.com

Java: String.format("%.2f", 3.14159)
来源：http://kkt.jinghuilouyu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vls.bbcook.cn

Ruby: format("%.2f", 3.14159)
来源：http://gfb.tian-w.cn

C#:   3.14159.ToString("F2")
来源：http://oqy.hywenlv.cn

[A22] 获取字符串长度
来源：http://pkd.snrcjt.cn

Py:   len(s)
来源：http://ugu.redwolf501.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ldv.xingfuxueyuan.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kft.yonumen.top

TS:   s.length
来源：http://hdv.bjfxy.top

Java: s.length()
来源：http://kjv.0kj1m.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uad.hnqzz.top

Ruby: s.length
来源：http://uoc.shangyingyoupin.top

C#:   s.Length
来源：http://fch.redwolf501.top

[A23] 大小写转换
来源：http://qme.xuetiantiany.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zeq.hnxiangtu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hgb.shuidangran.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gic.c1oappe.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vpa.yj20258.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sne.hysaishi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kay.hnqzz.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://aix.shzxlz.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cpu.zhixingplan.top

[A24] 去除首尾空白
来源：http://dkn.vqdsnc.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lhx.jlsjyb.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://puu.316326.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qvd.tarul.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ofi.smart0.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xjq.redwolf501.top

Go:   strings.TrimSpace(s)
来源：http://vkt.zhaomingkeji.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fne.tarul.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hug.yangfankeji.com

[A25] 字符串比较
来源：http://gtf.wangshuangyany.cn

Py:   s1 == s2; s1 != s2
来源：http://szs.zhengqikj.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ysl.zdqjudy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jxi.zhoulong.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ted.zycfv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://unj.zhongyouzk.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ojk.xylfe.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sfl.daria6918.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ieo.yonumen.top

[A26] 类型转换总览
来源：http://kyc.tian-w.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://otz.sufxvd.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://oyg.jyoumei.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mdf.zhijiandao.cn

TS:   Number() String() Boolean() x as number
来源：http://bnp.iojbl.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tps.cucudq.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yvx.xinyue.icu

Ruby: to_i to_f to_s to_sym to_a
来源：http://rnr.shanyushiyangkeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tln.hesvh.cn

================================================================================
来源：http://wyt.jianghu66.top

B. 流程控制
来源：http://hxa.jinqigufen.top

================================================================================
来源：http://gmd.wangshuangyany.cn

[B01] 条件判断 if / else
来源：http://luw.guannengcc.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ihi.shangyingyoupin.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ifm.ppjwa.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dez.uphjek.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uwd.sxryk.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dwc.guowangkeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pqo.chenlongwang.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sxb.xinyue.icu

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zey.xylfe.cn

[B02] 多分支 else if / elif
来源：http://nbj.zhixingplan.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://smt.zhaomingkeji.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sil.aizwys.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://phe.feifeiyinyue.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xvl.nanxinkj.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iuv.pycfn.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wkh.ybcxt.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dzm.jqgfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mvd.zdqjudy.top

[B03] switch / match / case
来源：http://bea.xuetiantiany.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://drs.gogol.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ieo.zdqjudy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ctb.shzxlz.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cwv.fanxiaobao.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pva.daxiang520.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zut.316326.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qni.xziqi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rie.feifeiyinyue.top

[B04] for 计数循环
来源：http://xlx.yj20258888.top

Py:   for i in range(10): print(i)
来源：http://jwa.xylfe.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yph.haohaochexian.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gcw.zhengqikj.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hma.cashguo.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ing.quarkkingdee.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oiv.shanyushiyangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://emy.svipenyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sgg.feifeiyinyue.top


<!-- 参考信息 -->