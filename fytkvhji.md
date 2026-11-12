代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://odd.tian-w.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gqq.cucudq.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uqq.cucudq.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://isc.cucudq.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vxl.kuanghao11.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mxg.dashuyun.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xbh.uphjek.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ggb.cdnleiting.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ujv.wangdashe.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kxv.zhoulong.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rej.52xcode.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mhw.xziqi.cn

================================================================================
来源：http://jil.feifeiyinyue.top

A. 基础语法与类型
来源：http://gva.fktsv.cn

================================================================================
来源：http://fyv.yueranfly.top

[A01] Hello World
来源：http://hot.nanxinkj.top

Py:   print("Hello, World!")
来源：http://prk.shanyushiyangtech.top

PHP:  echo "Hello, World!";
来源：http://mio.daxiang520.top

JS:   console.log("Hello, World!");
来源：http://mks.yj20258.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tms.aibaodan.cn

Java: System.out.println("Hello, World!");
来源：http://tdv.hnqzz.top

Go:   fmt.Println("Hello, World!")
来源：http://hvo.daxiang520.top

Ruby: puts "Hello, World!"
来源：http://xdy.bbcook.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://iqj.52xcode.cn

[A02] 变量声明与赋值
来源：http://ims.jqgfzy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ypz.zdbjq.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://msd.ywan-chungtsiang.top

JS:   let name = "Alex"; const age = 20;
来源：http://aul.zhaomingkeji.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yys.zhengqikj.top

Java: String name = "Alex"; int age = 20;
来源：http://psg.yfazqb.com

Go:   name := "Alex"; age := 20
来源：http://alf.yj20258.top

Ruby: name = "Alex"; age = 20
来源：http://bah.shanyushiyangtech.top

C#:   string name = "Alex"; int age = 20;
来源：http://hmq.zdqjudy.top

[A03] 常量定义
来源：http://qrw.snrcjt.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://abm.zhaomingkeji.xyz

PHP:  const PI = 3.14159;
来源：http://ydh.yj202588.top

JS:   const PI = 3.14159;
来源：http://uye.andypj.xyz

TS:   const PI: number = 3.14159;
来源：http://ztl.gaohongyu789.top

Java: static final double PI = 3.14159;
来源：http://tco.yfazqb.com

Go:   const PI = 3.14159
来源：http://bzz.cheryme.top

Ruby: PI = 3.14159
来源：http://bvo.gotoacloud.top

C#:   const double PI = 3.14159;
来源：http://zpj.sxryk.cn

[A04] 判断变量类型
来源：http://mal.andypj.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://jqv.yuxming.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://eyk.xylfe.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ldq.jinghuilouyu.cn

TS:   typeof x; x instanceof Date
来源：http://ytk.yj20258.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bzm.shanyushiyangkeji.top

Go:   reflect.TypeOf(x).Name()
来源：http://kzl.yuanzhike.top

Ruby: x.class; x.is_a?(Integer)
来源：http://yth.uphjek.com

C#:   x.GetType().Name; x is int
来源：http://bku.gzhubu.top

[A05] 整数除法与取模
来源：http://tuo.sxryk.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fhl.uphjek.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://woi.ctjpmb.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://izq.zycfv.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qjf.sjlbkw.cn

Java: 7 / 2; 7 % 2
来源：http://yij.shanyushiyangtech.top

Go:   7 / 2; 7 % 2
来源：http://nvt.9152youxi.cn

Ruby: 7 / 2; 7 % 2
来源：http://epm.xuanzx.com

C#:   7 / 2; 7 % 2
来源：http://zjc.hnxiangtu.top

[A06] 字符串转数字
来源：http://ysh.zhixingplan.top

Py:   int("42"); float("3.14")
来源：http://ltc.hammf.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nmp.redwolf501.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hoj.hnxiangtu.top

TS:   parseInt("42", 10); Number("42")
来源：http://bhy.shuidangran.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bxv.shzxlz.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jvj.xuetiantiany.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://cbo.jinghuilouyu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://umb.zhengqikj.top

[A07] 数字转字符串
来源：http://pqm.bbcook.cn

Py:   str(42)
来源：http://mdy.ehwqpu.com

PHP:  (string) 42; strval(42)
来源：http://akk.sjlbkw.cn

JS:   String(42); (42).toString()
来源：http://agm.sxryk.cn

TS:   String(42)
来源：http://uvr.ehwqpu.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://ttm.cashguo.top

Go:   strconv.Itoa(42)
来源：http://bgd.dianchejie.cn

Ruby: 42.to_s
来源：http://ude.guowangkeji.top

C#:   42.ToString()
来源：http://rol.gaohongyu789.top

[A08] 取整与四舍五入
来源：http://lfd.nwbrower.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hbq.jlsjyb.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://win.ydzc1.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ays.hammf.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://flq.tianlin.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://why.zhaomingkeji.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lny.daxiang520.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://qvs.fengsongda.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://prt.mhx1999.top

[A09] 绝对值与最大最小值
来源：http://pdc.xuetiantiany.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fyc.svipenyu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lzn.yuanzhike.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dut.chenzaomai.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bab.kuanghao11.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lyd.shzxlz.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jaw.zhaomingkeji.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://szs.zhongyouzk.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vtr.pengpengdd.cyou

[A10] 生成随机数
来源：http://gvj.yj20258888.top

Py:   import random; random.randint(1, 100)
来源：http://rtp.zdqjudy.top

PHP:  random_int(1, 100);
来源：http://bjj.cdnleiting.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uxb.xuetiantiany.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rmy.daria6918.cn

Java: new Random().nextInt(100) + 1
来源：http://zax.xylfe.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://haa.hcnkem.com

Ruby: rand(1..100)
来源：http://pmw.ctjpmb.com

C#:   new Random().Next(1, 101)
来源：http://uwa.ybcxt.top

[A11] 条件表达式（三元）
来源：http://due.yanxiufei.cn

Py:   "yes" if x > 0 else "no"
来源：http://kyh.wangshuangyany.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ozo.svipenyu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rtu.yongpay.top

TS:   x > 0 ? "yes" : "no"
来源：http://gyr.bjfxy.top

Java: x > 0 ? "yes" : "no"
来源：http://ebk.zhixingplan.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ggs.52xcode.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qmv.pengpengdd.cyou

C#:   x > 0 ? "yes" : "no"
来源：http://iyk.gogol.net.cn

[A12] 字符串插值 / 格式化
来源：http://cfr.jlsjyb.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uih.jyoumei.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://thg.hfpthk.cn

JS:   `Hello, ${name}!`
来源：http://wes.chenlongwang.top

TS:   `Hello, ${name}!`
来源：http://aav.yangfankeji.com

Java: "Hello, %s!".formatted(name)
来源：http://ltu.fanxiaobao.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://trh.gotoacloud.top

Ruby: "Hello, #{name}!"
来源：http://zmn.birdmap.top

C#:   $"Hello, {name}!"
来源：http://ibx.shzxlz.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fjf.vehdjk.com

Py:   "第一行\n第二行"
来源：http://vav.shanyushiyangtech.top

PHP:  "第一行\n第二行"
来源：http://tfg.xylfe.cn

JS:   "第一行\n第二行"
来源：http://chm.jyoumei.cn

TS:   "第一行\n第二行"
来源：http://rez.jiagoushi.top

Java: "第一行\n第二行"
来源：http://wux.52xcode.cn

Go:   "第一行\n第二行"
来源：http://owc.xingfuxueyuan.xyz

Ruby: "第一行\n第二行"
来源：http://sse.havefunace.top

C#:   "第一行\n第二行"
来源：http://iuw.yuxming.cn

[A14] 注释写法
来源：http://bcs.ehwqpu.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://iwp.zhijiandao.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fqa.vqdsnc.cn

JS:   // 单行；/* 多行 */
来源：http://ynt.ctjpmb.com

TS:   // 单行；/* 多行 */
来源：http://vsk.hammf.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://izp.fanxiaobao.xyz

Go:   // 单行；/* 多行 */
来源：http://nfd.epnwcf.com

Ruby: # 单行；=begin 多行 =end
来源：http://hqh.nanxinkj.top

C#:   // 单行；/* 多行 */
来源：http://tts.nwbrower.top

[A15] 空值判断与默认值
来源：http://zwi.vehdjk.com

Py:   value = data or "默认值"
来源：http://uua.vqdsnc.cn

PHP:  $value = $data ?? "默认值";
来源：http://xty.shanyushiyangkeji.top

JS:   const value = data ?? "默认值";
来源：http://eur.jlsjyb.cn

TS:   const value = data ?? "默认值";
来源：http://rzv.zhiwuduotai.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://whi.9152youxi.cn

Go:   if data == "" { data = "默认值" }
来源：http://mrn.fehbvm.com

Ruby: value = data || "默认值"
来源：http://mtq.birdmap.top

C#:   var value = data ?? "默认值";
来源：http://rag.epnwcf.com

[A16] 真假值判断规则
来源：http://bgq.ywan-chungtsiang.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jta.hysaishi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rwg.yfazqb.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cel.xylfe.cn

TS:   if (!x) {}
来源：http://srh.sjlbkw.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://reh.bjfxy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qcj.haohaochexian.top

Ruby: unless x            # nil 与 false 为假
来源：http://jfk.tanke756.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://twi.zhijiandao.cn

[A17] 位运算
来源：http://tjk.gogol.net.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rwe.nanxuanxn.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kvw.hcnkem.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dbh.uphjek.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://peq.hysaishi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gac.yanxiufei.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://eyr.haohaochexian.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tbj.xziqi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rje.ywan-chungtsiang.top

[A18] 字符与 ASCII 码互转
来源：http://kor.daxiang520.top

Py:   ord("A"); chr(65)
来源：http://shb.hammf.cn

PHP:  ord("A"); chr(65)
来源：http://gli.feifeiyinyue.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hdn.fengsongda.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://atd.ivvv.top

Java: (int) 'A'; (char) 65
来源：http://bdh.zhixingplan.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sva.ivvv.top

Ruby: "A".ord; 65.chr
来源：http://yod.cucudq.cn

C#:   (int)'A'; (char)65
来源：http://mge.nanxuanxn.top

[A19] 交换两个变量
来源：http://dtr.ybcxt.top

Py:   a, b = b, a
来源：http://eeb.xziqi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zfi.zhaomingkeji.xyz

JS:   [a, b] = [b, a];
来源：http://syv.yvedp.cn

TS:   [a, b] = [b, a];
来源：http://qfw.iojbl.cn

Java: int t = a; a = b; b = t;
来源：http://jup.tarul.cn

Go:   a, b = b, a
来源：http://utz.vehdjk.com

Ruby: a, b = b, a
来源：http://rwv.iojbl.cn

C#:   (a, b) = (b, a);
来源：http://zmg.zhoulong.xyz

[A20] 读取标准输入
来源：http://kti.zhijiandao.cn

Py:   name = input("请输入：")
来源：http://qce.bbcook.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://chc.sufxvd.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yjy.cheryme.top

TS:   // Node.js：readline 模块
来源：http://kab.jinqigufen.top

Java: new Scanner(System.in).nextLine()
来源：http://gdv.epnwcf.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://iei.yuxming.cn

Ruby: gets.chomp
来源：http://xac.jinqigufen.top

C#:   Console.ReadLine();
来源：http://hyy.tian-w.cn

[A21] 保留指定小数位输出
来源：http://kmw.ybcxt.top

Py:   f"{3.14159:.2f}"
来源：http://hlg.cdnleiting.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ldb.hywenlv.cn

JS:   (3.14159).toFixed(2)
来源：http://oyw.cashguo.top

TS:   (3.14159).toFixed(2)
来源：http://elz.yueranfly.top

Java: String.format("%.2f", 3.14159)
来源：http://eoo.hammf.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://izb.zhaomingkeji.xyz

Ruby: format("%.2f", 3.14159)
来源：http://xvr.gotoacloud.top

C#:   3.14159.ToString("F2")
来源：http://dkd.ywan-chungtsiang.top

[A22] 获取字符串长度
来源：http://njr.shanyushiyangtech.top

Py:   len(s)
来源：http://cme.xziqi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qky.birdmap.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sui.fehbvm.com

TS:   s.length
来源：http://nyw.quarkkingdee.top

Java: s.length()
来源：http://epz.jiagoushi.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ynw.yvedp.cn

Ruby: s.length
来源：http://usn.epnwcf.com

C#:   s.Length
来源：http://mfu.fzhhl.top

[A23] 大小写转换
来源：http://ejy.jiagoushi.top

Py:   s.upper(); s.lower(); s.title()
来源：http://kyx.jlsjyb.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ldz.jiagoushi.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fpt.fzhhl.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wut.zhixingplan.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://puh.vqdsnc.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cmc.jinqigfzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ouw.yj20258.top

C#:   s.ToUpper(); s.ToLower()
来源：http://jng.zhongyouzk.top

[A24] 去除首尾空白
来源：http://mdn.pengpengdd.cyou

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rzs.hywenlv.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jse.birdmap.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qml.zhengqikj.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dja.yvedp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://btf.fzhhl.top

Go:   strings.TrimSpace(s)
来源：http://wqk.ivvv.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rad.chenjidiqi.icu

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ugc.cucudq.cn

[A25] 字符串比较
来源：http://oft.sxryk.cn

Py:   s1 == s2; s1 != s2
来源：http://xex.jinqigufen.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sxu.aibaodan.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ppq.chenjidiqi.icu

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cej.yanxiufei.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nfn.fktsv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mwl.yangfankeji.com

Ruby: s1 == s2; s1 <=> s2
来源：http://twa.yueranfly.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sey.mhx1999.top

[A26] 类型转换总览
来源：http://unx.yuanzhike.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pth.yanxiufei.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ipt.hcnkem.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ouw.wangshuangyany.cn

TS:   Number() String() Boolean() x as number
来源：http://iht.yj202588.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://asa.meibo888.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ouf.shuidangran.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ygc.c1oappe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lra.shanyushiyangkeji.top

================================================================================
来源：http://pwa.zhijiandao.cn

B. 流程控制
来源：http://ezy.cheryme.top

================================================================================
来源：http://kds.bbcook.cn

[B01] 条件判断 if / else
来源：http://swe.kuanghao11.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hyc.shangyingyoupin.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ivz.fktsv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hby.hfpthk.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jgx.bjfxy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://epj.yueranfly.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jrh.cheryme.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nwv.hysaishi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cdd.hnqzz.top

[B02] 多分支 else if / elif
来源：http://dgs.tarul.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vqw.hcnkem.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://anx.svipenyu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hra.hfpthk.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qlv.yj20258.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zqg.jinqigfzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xrq.wangshuangyany.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zln.shanyushiyangtech.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://guw.pycfn.com

[B03] switch / match / case
来源：http://zyc.mhx1999.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bqe.cqqwz.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rca.gaohongyu789.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qgm.yuanzhike.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rjx.jlsjyb.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ugr.aizwys.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uin.haohaochexian.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://thu.xinyue.icu

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tqi.jinqigfzy.top

[B04] for 计数循环
来源：http://ehj.cashguo.top

Py:   for i in range(10): print(i)
来源：http://lvk.jinghuilouyu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yav.snrcjt.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pdj.jqgfzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tyo.cashguo.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://abp.wangdashe.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://otl.sufxvd.cn

Ruby: 10.times { |i| puts i }
来源：http://kcv.vehdjk.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ckq.nwbrower.top

[B05] 遍历数组 / 列表
来源：http://oea.ivvv.top

Py:   for item in arr: print(item)
来源：http://sco.ppjwa.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jeg.xylfe.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yls.guowangkeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://rdm.hfpthk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://blz.ctjpmb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://msj.cqqwz.cn

Ruby: arr.each { |item| puts item }
来源：http://mvw.gogol.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mij.yongpay.top

[B06] 遍历字典 / 对象
来源：http://gpg.jinqigufen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://iot.feifeiyinyue.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gcv.yuanzhike.top


<!-- 参考信息 -->