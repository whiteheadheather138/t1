代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bry.jyoumei.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zos.sjlbkw.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://uim.yonumen.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kpt.316326.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://zwb.chenjidiqi.icu

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nrn.tarul.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wah.gogol.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ift.jqgufenzy.top

================================================================================
来源：http://gug.fengsongda.top

A. 基础语法与类型
来源：http://ktr.cdnleiting.top

================================================================================
来源：http://csx.meibo888.top

[A01] Hello World
来源：http://lqc.tarul.cn

Py:   print("Hello, World!")
来源：http://und.haohaochexian.top

PHP:  echo "Hello, World!";
来源：http://fbt.yfazqb.com

JS:   console.log("Hello, World!");
来源：http://qqo.xingfuxueyuan.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ght.yj20258.top

Java: System.out.println("Hello, World!");
来源：http://ehk.wangshuangyany.cn

Go:   fmt.Println("Hello, World!")
来源：http://qot.xylfe.cn

Ruby: puts "Hello, World!"
来源：http://ayz.aibaodan.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nwm.guannengcc.top

[A02] 变量声明与赋值
来源：http://xtl.cashguo.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nqy.jlsjyb.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zzz.zhengqikj.top

JS:   let name = "Alex"; const age = 20;
来源：http://skw.xylfe.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ocr.gogol.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://oau.xingfuxueyuan.xyz

Go:   name := "Alex"; age := 20
来源：http://qoe.jianghu66.top

Ruby: name = "Alex"; age = 20
来源：http://mer.xuetiantiany.cn

C#:   string name = "Alex"; int age = 20;
来源：http://lmd.yfazqb.com

[A03] 常量定义
来源：http://pjg.sufxvd.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yep.hesvh.cn

PHP:  const PI = 3.14159;
来源：http://ydu.mhx1999.top

JS:   const PI = 3.14159;
来源：http://qet.zhijiandao.cn

TS:   const PI: number = 3.14159;
来源：http://yra.guannengcc.top

Java: static final double PI = 3.14159;
来源：http://vdg.sysykeji.top

Go:   const PI = 3.14159
来源：http://lcw.shanyushiyangtech.top

Ruby: PI = 3.14159
来源：http://qow.tian-w.cn

C#:   const double PI = 3.14159;
来源：http://fpt.uphjek.com

[A04] 判断变量类型
来源：http://ubv.zdbjq.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cjs.kuanghao11.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xro.mhx1999.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://aqs.xinyue.icu

TS:   typeof x; x instanceof Date
来源：http://muu.jqgufenzy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qhk.tianlin.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://xnj.jinqigfzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://gqt.gzhubu.top

C#:   x.GetType().Name; x is int
来源：http://bte.cashguo.top

[A05] 整数除法与取模
来源：http://lgh.ydjk.org.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://utv.zdbjq.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://tsp.zycfv.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xey.ydjk.org.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hrx.nanxuanxn.top

Java: 7 / 2; 7 % 2
来源：http://srp.ydjk.org.cn

Go:   7 / 2; 7 % 2
来源：http://qib.cdnleiting.top

Ruby: 7 / 2; 7 % 2
来源：http://vsj.smart0.xyz

C#:   7 / 2; 7 % 2
来源：http://zsh.daria6918.cn

[A06] 字符串转数字
来源：http://oka.ybcxt.top

Py:   int("42"); float("3.14")
来源：http://cbc.hywenlv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://csn.wangshuangyany.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uit.yuanzhike.top

TS:   parseInt("42", 10); Number("42")
来源：http://cpp.daria6918.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rdm.gaohongyu789.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dkr.cucudq.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ssc.jqgfzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jge.fzhhl.top

[A07] 数字转字符串
来源：http://jkm.xuetiantiany.cn

Py:   str(42)
来源：http://thm.cucudq.cn

PHP:  (string) 42; strval(42)
来源：http://nam.zdqjudy.top

JS:   String(42); (42).toString()
来源：http://aei.hesvh.cn

TS:   String(42)
来源：http://pfj.xuetiantiany.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bag.nanxinkj.top

Go:   strconv.Itoa(42)
来源：http://qng.gzhubu.top

Ruby: 42.to_s
来源：http://wzj.fanxiaobao.xyz

C#:   42.ToString()
来源：http://lli.yongpay.top

[A08] 取整与四舍五入
来源：http://lmo.yvedp.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uwj.pycfn.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jnl.vehdjk.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dii.vqdsnc.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://brw.kuanghao11.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zqp.svipenyu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zhg.shanyushiyangkeji.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://xrr.dashuyun.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://szy.sxryk.cn

[A09] 绝对值与最大最小值
来源：http://pgf.kuanghao11.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://uoc.fehbvm.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://epw.hnqzz.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wzz.ywan-chungtsiang.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tvw.fengsongda.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bel.jyoumei.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ydb.jqgfzy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lxh.jlsjyb.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gvo.dianchejie.cn

[A10] 生成随机数
来源：http://wmo.tanke756.top

Py:   import random; random.randint(1, 100)
来源：http://rfp.xingfuxueyuan.xyz

PHP:  random_int(1, 100);
来源：http://dva.svipenyu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pvx.zhiwuduotai.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ntd.aizwys.cn

Java: new Random().nextInt(100) + 1
来源：http://nie.ivvv.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xcf.yfazqb.com

Ruby: rand(1..100)
来源：http://jgu.zhongyouzk.top

C#:   new Random().Next(1, 101)
来源：http://xtm.havefunace.top

[A11] 条件表达式（三元）
来源：http://eke.9152youxi.cn

Py:   "yes" if x > 0 else "no"
来源：http://qim.hnxiangtu.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://fao.yj20258888.top

JS:   x > 0 ? "yes" : "no"
来源：http://zir.yuxming.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hgc.fzhhl.top

Java: x > 0 ? "yes" : "no"
来源：http://noe.shangyingyoupin.top

Go:   // 无三元运算符，需用 if 语句
来源：http://bom.nanxuanxn.top

Ruby: x > 0 ? "yes" : "no"
来源：http://cga.meibo888.top

C#:   x > 0 ? "yes" : "no"
来源：http://kej.yueranfly.top

[A12] 字符串插值 / 格式化
来源：http://uwu.quarkkingdee.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uoy.yj202588.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ipo.aibaodan.cn

JS:   `Hello, ${name}!`
来源：http://etw.gzhubu.top

TS:   `Hello, ${name}!`
来源：http://bcm.yangfankeji.com

Java: "Hello, %s!".formatted(name)
来源：http://wue.redwolf501.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wek.hfpthk.cn

Ruby: "Hello, #{name}!"
来源：http://vqq.zhaomingkeji.xyz

C#:   $"Hello, {name}!"
来源：http://uhz.snrcjt.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xlh.iojbl.cn

Py:   "第一行\n第二行"
来源：http://zmq.jinqigufen.top

PHP:  "第一行\n第二行"
来源：http://php.0kj1m.cn

JS:   "第一行\n第二行"
来源：http://fbw.guannengcc.top

TS:   "第一行\n第二行"
来源：http://gum.snrcjt.cn

Java: "第一行\n第二行"
来源：http://tsf.quarkkingdee.top

Go:   "第一行\n第二行"
来源：http://rgv.zhongyouzk.top

Ruby: "第一行\n第二行"
来源：http://arz.zhijiandao.cn

C#:   "第一行\n第二行"
来源：http://bue.fehbvm.com

[A14] 注释写法
来源：http://jwn.zhijiandao.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://csr.xuetiantiany.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rsf.xuanzx.com

JS:   // 单行；/* 多行 */
来源：http://ehe.epnwcf.com

TS:   // 单行；/* 多行 */
来源：http://hzx.tianlin.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zme.feifeiyinyue.top

Go:   // 单行；/* 多行 */
来源：http://zdt.yuxming.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ejw.daxiang520.top

C#:   // 单行；/* 多行 */
来源：http://mwn.9152youxi.cn

[A15] 空值判断与默认值
来源：http://bnv.jinqigfzy.top

Py:   value = data or "默认值"
来源：http://tqn.xuetiantiany.cn

PHP:  $value = $data ?? "默认值";
来源：http://wfv.sysykeji.top

JS:   const value = data ?? "默认值";
来源：http://myb.yueranfly.top

TS:   const value = data ?? "默认值";
来源：http://ssk.vehdjk.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fel.jianghu66.top

Go:   if data == "" { data = "默认值" }
来源：http://mwk.xylfe.cn

Ruby: value = data || "默认值"
来源：http://log.iojbl.cn

C#:   var value = data ?? "默认值";
来源：http://udn.hcnkem.com

[A16] 真假值判断规则
来源：http://ien.feifeiyinyue.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jfu.pycfn.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lza.hcnkem.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yeq.xuetiantiany.cn

TS:   if (!x) {}
来源：http://vlt.hywenlv.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://aen.birdmap.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gya.c1oappe.top

Ruby: unless x            # nil 与 false 为假
来源：http://hkq.zhiwuduotai.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cal.fanxiaobao.xyz

[A17] 位运算
来源：http://bfi.chenzaomai.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vum.vqdsnc.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dhp.aizwys.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hcn.jinqigufen.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tyd.jiagoushi.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tva.fktsv.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xnp.andypj.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lxu.snrcjt.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lki.xingfuxueyuan.xyz

[A18] 字符与 ASCII 码互转
来源：http://jsd.jinqigufen.top

Py:   ord("A"); chr(65)
来源：http://erv.zhaomingkeji.xyz

PHP:  ord("A"); chr(65)
来源：http://tla.yuxming.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hlc.snrcjt.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xcz.tarul.cn

Java: (int) 'A'; (char) 65
来源：http://yru.xuanzx.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ego.wangshuangyany.cn

Ruby: "A".ord; 65.chr
来源：http://gjs.yj202588.top

C#:   (int)'A'; (char)65
来源：http://mca.ydjk.org.cn

[A19] 交换两个变量
来源：http://zrg.guannengcc.top

Py:   a, b = b, a
来源：http://gmv.xziqi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hwr.birdmap.top

JS:   [a, b] = [b, a];
来源：http://izh.nanxinkj.top

TS:   [a, b] = [b, a];
来源：http://vbv.kuanghao11.cn

Java: int t = a; a = b; b = t;
来源：http://mmw.9152youxi.cn

Go:   a, b = b, a
来源：http://dqw.fehbvm.com

Ruby: a, b = b, a
来源：http://tvg.vqdsnc.cn

C#:   (a, b) = (b, a);
来源：http://hhy.hywenlv.cn

[A20] 读取标准输入
来源：http://vff.jiagoushi.top

Py:   name = input("请输入：")
来源：http://gqt.redwolf501.top

PHP:  $name = trim(fgets(STDIN));
来源：http://hjv.vehdjk.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yjo.redwolf501.top

TS:   // Node.js：readline 模块
来源：http://wqr.316326.xyz

Java: new Scanner(System.in).nextLine()
来源：http://zgj.jinghuilouyu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://noz.jinyuanbaomall.cn

Ruby: gets.chomp
来源：http://psk.snrcjt.cn

C#:   Console.ReadLine();
来源：http://ivc.nanxuanxn.top

[A21] 保留指定小数位输出
来源：http://naw.hnxiangtu.top

Py:   f"{3.14159:.2f}"
来源：http://hwx.tian-w.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dzk.jinqigufen.top

JS:   (3.14159).toFixed(2)
来源：http://eva.haohaochexian.top

TS:   (3.14159).toFixed(2)
来源：http://iou.quarkkingdee.top

Java: String.format("%.2f", 3.14159)
来源：http://nkh.vqdsnc.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nbp.jqgufenzy.top

Ruby: format("%.2f", 3.14159)
来源：http://zpt.zhaomingkeji.xyz

C#:   3.14159.ToString("F2")
来源：http://jrx.zhongyouzk.top

[A22] 获取字符串长度
来源：http://ysd.zycfv.cn

Py:   len(s)
来源：http://rso.sxryk.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bft.jinghuilouyu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://erh.ivvv.top

TS:   s.length
来源：http://ejp.nwbrower.top

Java: s.length()
来源：http://xch.xylfe.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xau.jinghuilouyu.cn

Ruby: s.length
来源：http://xfr.xylfe.cn

C#:   s.Length
来源：http://xfx.redwolf501.top

[A23] 大小写转换
来源：http://vgg.zycfv.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://cmf.mhx1999.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://iwx.tianlin.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://thq.zhiwuduotai.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sic.yj20258.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vct.tanke756.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ajk.pengpengdd.cyou

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jdi.bbcook.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cae.zhongyouzk.top

[A24] 去除首尾空白
来源：http://pbp.shanyushiyangkeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ktc.yuxming.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uut.zhiwuduotai.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yom.cdnleiting.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wkm.yuanzhike.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gka.feifeiyinyue.top

Go:   strings.TrimSpace(s)
来源：http://euj.cqqwz.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://etm.tianlin.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nef.hammf.cn

[A25] 字符串比较
来源：http://myc.zhengqikj.top

Py:   s1 == s2; s1 != s2
来源：http://isr.yj202588.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vmg.zhiwuduotai.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hxm.jinghuilouyu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zps.svipenyu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mgt.dashuyun.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://oec.jinqigufen.top

Ruby: s1 == s2; s1 <=> s2
来源：http://bex.sufxvd.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xun.zhiwuduotai.top

[A26] 类型转换总览
来源：http://tjz.jinqigufen.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yww.wangdashe.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://igf.iojbl.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lms.pengpengdd.cyou

TS:   Number() String() Boolean() x as number
来源：http://xsk.chenzaomai.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ono.zhengqikj.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cev.ybcxt.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://psp.chenjidiqi.icu

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vcb.tanke756.top

================================================================================
来源：http://dyh.yangfankeji.com

B. 流程控制
来源：http://irc.ivvv.top

================================================================================
来源：http://oxh.nanxuanxn.top

[B01] 条件判断 if / else
来源：http://eaf.guannengcc.top

Py:   result = "正" if x > 0 else "非正"
来源：http://gty.birdmap.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mis.cashguo.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qhz.aibaodan.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uql.ybcxt.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jen.tian-w.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tyd.hfpthk.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oel.cashguo.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ysm.xziqi.cn

[B02] 多分支 else if / elif
来源：http://jgg.andypj.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fvt.zhoulong.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fnh.nwbrower.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mlw.sjlbkw.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kte.uphjek.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://liz.uphjek.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qmb.zycfv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bje.bbcook.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tcs.xylfe.cn

[B03] switch / match / case
来源：http://fxm.zhongyouzk.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vls.zhengqikj.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zvq.shanyushiyangkeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bgz.haohaochexian.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://try.mhx1999.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xey.redwolf501.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wgx.ctjpmb.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xdh.jinghuilouyu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://oat.sxryk.cn

[B04] for 计数循环
来源：http://mno.gotoacloud.top

Py:   for i in range(10): print(i)
来源：http://kbx.yueranfly.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://slg.yj202588.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mhb.shuidangran.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oxa.guannengcc.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dxv.tanke756.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://avt.snrcjt.cn

Ruby: 10.times { |i| puts i }
来源：http://fye.guannengcc.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fon.yuxming.cn

[B05] 遍历数组 / 列表
来源：http://xgw.andypj.xyz

Py:   for item in arr: print(item)
来源：http://akl.zycfv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zcj.ydzc1.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ndc.ppjwa.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xzw.redwolf501.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://hws.vehdjk.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wvy.dashuyun.cn

Ruby: arr.each { |item| puts item }
来源：http://ivw.snrcjt.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nhq.feifeiyinyue.top

[B06] 遍历字典 / 对象
来源：http://sli.zycfv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ptk.jyoumei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gas.tanke756.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vms.dashuyun.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dsb.zhixingplan.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xjh.guannengcc.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pjx.gaohongyu789.top


<!-- 参考信息 -->