代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://uod.yvedp.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://krc.sxryk.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yfb.yongpay.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nuh.tanke756.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://jbv.dashuyun.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gdk.yueranfly.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fdq.tianlin.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ijx.jqgufenzy.top

================================================================================
来源：http://eho.vqdsnc.cn

A. 基础语法与类型
来源：http://vyl.fehbvm.com

================================================================================
来源：http://nll.zhengqikj.top

[A01] Hello World
来源：http://fbl.hesvh.cn

Py:   print("Hello, World!")
来源：http://ike.0kj1m.cn

PHP:  echo "Hello, World!";
来源：http://dkq.hnqzz.top

JS:   console.log("Hello, World!");
来源：http://lat.nanxuanxn.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fkg.zdqjudy.top

Java: System.out.println("Hello, World!");
来源：http://bis.xuetiantiany.cn

Go:   fmt.Println("Hello, World!")
来源：http://lak.zhijiandao.cn

Ruby: puts "Hello, World!"
来源：http://ivs.hammf.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://thf.wangshuangyany.cn

[A02] 变量声明与赋值
来源：http://vvg.meibo888.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://skg.jyoumei.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://afi.birdmap.top

JS:   let name = "Alex"; const age = 20;
来源：http://qjf.yangfankeji.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cqp.meibo888.top

Java: String name = "Alex"; int age = 20;
来源：http://pwx.yfazqb.com

Go:   name := "Alex"; age := 20
来源：http://ous.fktsv.cn

Ruby: name = "Alex"; age = 20
来源：http://bmr.hongshengwenyu.top

C#:   string name = "Alex"; int age = 20;
来源：http://bfv.zdbjq.cn

[A03] 常量定义
来源：http://zah.yvedp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bmz.jinyuanbaomall.cn

PHP:  const PI = 3.14159;
来源：http://wtf.sufxvd.cn

JS:   const PI = 3.14159;
来源：http://dme.daxiang520.top

TS:   const PI: number = 3.14159;
来源：http://hkb.uphjek.com

Java: static final double PI = 3.14159;
来源：http://vjq.uphjek.com

Go:   const PI = 3.14159
来源：http://ojw.hongshengwenyu.top

Ruby: PI = 3.14159
来源：http://kps.tian-w.cn

C#:   const double PI = 3.14159;
来源：http://jix.sysykeji.top

[A04] 判断变量类型
来源：http://tya.zdbjq.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ccz.shanyushiyangkeji.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bpo.yangfankeji.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nxb.cucudq.cn

TS:   typeof x; x instanceof Date
来源：http://yze.cqqwz.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://iua.aizwys.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dtk.ybcxt.top

Ruby: x.class; x.is_a?(Integer)
来源：http://bjh.xuanzx.com

C#:   x.GetType().Name; x is int
来源：http://bwb.pycfn.com

[A05] 整数除法与取模
来源：http://fvr.0kj1m.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vmj.yfazqb.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://nca.hfpthk.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pjl.xuanzx.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://quq.yongpay.top

Java: 7 / 2; 7 % 2
来源：http://fay.jinyuanbaomall.cn

Go:   7 / 2; 7 % 2
来源：http://mql.jlsjyb.cn

Ruby: 7 / 2; 7 % 2
来源：http://xst.vehdjk.com

C#:   7 / 2; 7 % 2
来源：http://nbb.zhiwuduotai.top

[A06] 字符串转数字
来源：http://rtp.pengpengdd.cyou

Py:   int("42"); float("3.14")
来源：http://xiq.hfpthk.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zlc.redwolf501.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lst.fanxiaobao.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://bke.bbcook.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jyx.jianghu66.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hpi.nanxuanxn.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ibe.0kj1m.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ldq.yvedp.cn

[A07] 数字转字符串
来源：http://vor.cheryme.top

Py:   str(42)
来源：http://wwp.tianlin.xyz

PHP:  (string) 42; strval(42)
来源：http://riv.smart0.xyz

JS:   String(42); (42).toString()
来源：http://jyv.zhixingplan.top

TS:   String(42)
来源：http://qju.9152youxi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://mda.pycfn.com

Go:   strconv.Itoa(42)
来源：http://ozl.zdqjudy.top

Ruby: 42.to_s
来源：http://boz.redwolf501.top

C#:   42.ToString()
来源：http://kmc.pycfn.com

[A08] 取整与四舍五入
来源：http://jwv.hammf.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://stx.chenlongwang.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://atc.9152youxi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bsu.pycfn.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qyi.hnqzz.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bmb.wangdashe.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gfo.zhongyouzk.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://fhp.svipenyu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gyt.sweek.top

[A09] 绝对值与最大最小值
来源：http://aom.snrcjt.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tzj.jqgfzy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jlf.tarul.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kec.xylfe.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rjs.gotoacloud.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lmc.pycfn.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lgm.xingfuxueyuan.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gfw.wangdashe.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mzl.dashuyun.cn

[A10] 生成随机数
来源：http://rzb.xuetiantiany.cn

Py:   import random; random.randint(1, 100)
来源：http://cks.zdbjq.cn

PHP:  random_int(1, 100);
来源：http://hcj.jinqigfzy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fbv.yueranfly.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pnx.cashguo.top

Java: new Random().nextInt(100) + 1
来源：http://rkm.yanxiufei.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ysd.jyoumei.cn

Ruby: rand(1..100)
来源：http://opd.fengsongda.top

C#:   new Random().Next(1, 101)
来源：http://ski.ivvv.top

[A11] 条件表达式（三元）
来源：http://eiy.jinqigufen.top

Py:   "yes" if x > 0 else "no"
来源：http://eyr.hcnkem.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://dsn.nwbrower.top

JS:   x > 0 ? "yes" : "no"
来源：http://ryb.xuanzx.com

TS:   x > 0 ? "yes" : "no"
来源：http://tiu.birdmap.top

Java: x > 0 ? "yes" : "no"
来源：http://loq.tarul.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xxr.zhixingplan.top

Ruby: x > 0 ? "yes" : "no"
来源：http://vga.sxryk.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ywd.hammf.cn

[A12] 字符串插值 / 格式化
来源：http://rxo.xziqi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nyn.jlsjyb.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xlt.vehdjk.com

JS:   `Hello, ${name}!`
来源：http://shz.shanyushiyangkeji.top

TS:   `Hello, ${name}!`
来源：http://eak.jlsjyb.cn

Java: "Hello, %s!".formatted(name)
来源：http://gdo.yonumen.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mfd.hywenlv.cn

Ruby: "Hello, #{name}!"
来源：http://ekv.yuxming.cn

C#:   $"Hello, {name}!"
来源：http://jlf.yfazqb.com

[A13] 多行字符串（练习 \n 转义）
来源：http://alr.yuxming.cn

Py:   "第一行\n第二行"
来源：http://wnp.quarkkingdee.top

PHP:  "第一行\n第二行"
来源：http://tyl.jinqigufen.top

JS:   "第一行\n第二行"
来源：http://pur.snrcjt.cn

TS:   "第一行\n第二行"
来源：http://vgh.guannengcc.top

Java: "第一行\n第二行"
来源：http://jaf.sufxvd.cn

Go:   "第一行\n第二行"
来源：http://xoc.feifeiyinyue.top

Ruby: "第一行\n第二行"
来源：http://qwk.ydjk.org.cn

C#:   "第一行\n第二行"
来源：http://vxj.sjlbkw.cn

[A14] 注释写法
来源：http://xcn.bbcook.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gor.xuanzx.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://qko.gaohongyu789.top

JS:   // 单行；/* 多行 */
来源：http://elj.bjfxy.top

TS:   // 单行；/* 多行 */
来源：http://jeh.pengpengdd.cyou

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://php.jinyuanbaomall.cn

Go:   // 单行；/* 多行 */
来源：http://nrw.0kj1m.cn

Ruby: # 单行；=begin 多行 =end
来源：http://sci.nwbrower.top

C#:   // 单行；/* 多行 */
来源：http://eyh.c1oappe.top

[A15] 空值判断与默认值
来源：http://zuu.epnwcf.com

Py:   value = data or "默认值"
来源：http://hau.zdbjq.cn

PHP:  $value = $data ?? "默认值";
来源：http://xir.yonumen.top

JS:   const value = data ?? "默认值";
来源：http://uur.xziqi.cn

TS:   const value = data ?? "默认值";
来源：http://yav.sysykeji.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jvb.tian-w.cn

Go:   if data == "" { data = "默认值" }
来源：http://qds.ydjk.org.cn

Ruby: value = data || "默认值"
来源：http://rqg.havefunace.top

C#:   var value = data ?? "默认值";
来源：http://syu.jinqigufen.top

[A16] 真假值判断规则
来源：http://dwt.yuanzhike.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dnr.jyoumei.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rgy.shanyushiyangkeji.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://trf.cucudq.cn

TS:   if (!x) {}
来源：http://chp.jqgfzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qpt.chenzaomai.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uom.guowangkeji.top

Ruby: unless x            # nil 与 false 为假
来源：http://vix.ybcxt.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tvn.fzhhl.top

[A17] 位运算
来源：http://enj.dashuyun.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://irh.guowangkeji.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cjy.zhoulong.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dpa.ybcxt.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ebj.sysykeji.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aaf.aizwys.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jej.mhx1999.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qso.shuidangran.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ltc.shuidangran.top

[A18] 字符与 ASCII 码互转
来源：http://tkb.aizwys.cn

Py:   ord("A"); chr(65)
来源：http://kge.haohaochexian.top

PHP:  ord("A"); chr(65)
来源：http://hjc.redwolf501.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ehv.cucudq.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://svs.pengpengdd.cyou

Java: (int) 'A'; (char) 65
来源：http://zlb.yj20258888.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://klk.jinqigufen.top

Ruby: "A".ord; 65.chr
来源：http://hqt.nanxinkj.top

C#:   (int)'A'; (char)65
来源：http://kan.sysykeji.top

[A19] 交换两个变量
来源：http://mzd.xuanzx.com

Py:   a, b = b, a
来源：http://ydn.yuxming.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://dtu.hcnkem.com

JS:   [a, b] = [b, a];
来源：http://fgt.jinqigfzy.top

TS:   [a, b] = [b, a];
来源：http://ntu.mhx1999.top

Java: int t = a; a = b; b = t;
来源：http://kgh.zycfv.cn

Go:   a, b = b, a
来源：http://trc.shangyingyoupin.top

Ruby: a, b = b, a
来源：http://egv.yuxming.cn

C#:   (a, b) = (b, a);
来源：http://pxd.xinyue.icu

[A20] 读取标准输入
来源：http://yhd.daria6918.cn

Py:   name = input("请输入：")
来源：http://tfr.hywenlv.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://set.jqgfzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jea.epnwcf.com

TS:   // Node.js：readline 模块
来源：http://vcr.hcnkem.com

Java: new Scanner(System.in).nextLine()
来源：http://yia.dashuyun.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vyq.hnxiangtu.top

Ruby: gets.chomp
来源：http://xaz.xuanzx.com

C#:   Console.ReadLine();
来源：http://gja.smart0.xyz

[A21] 保留指定小数位输出
来源：http://cyj.jlsjyb.cn

Py:   f"{3.14159:.2f}"
来源：http://zaz.nanxinkj.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://oml.tianlin.xyz

JS:   (3.14159).toFixed(2)
来源：http://bpy.yvedp.cn

TS:   (3.14159).toFixed(2)
来源：http://qhj.snrcjt.cn

Java: String.format("%.2f", 3.14159)
来源：http://xdz.yfazqb.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gbl.shanyushiyangtech.top

Ruby: format("%.2f", 3.14159)
来源：http://kuh.yuanzhike.top

C#:   3.14159.ToString("F2")
来源：http://dfs.yfazqb.com

[A22] 获取字符串长度
来源：http://wzl.gotoacloud.top

Py:   len(s)
来源：http://khh.aibaodan.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cso.birdmap.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wyj.zhiwuduotai.top

TS:   s.length
来源：http://zrz.andypj.xyz

Java: s.length()
来源：http://spx.yongpay.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wad.yvedp.cn

Ruby: s.length
来源：http://tll.sjlbkw.cn

C#:   s.Length
来源：http://qqw.yueranfly.top

[A23] 大小写转换
来源：http://cqs.hesvh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ybk.cashguo.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wwx.nwbrower.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qju.svipenyu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uox.pycfn.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://irx.ppjwa.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ayr.yongpay.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://buw.yanxiufei.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nqt.feifeiyinyue.top

[A24] 去除首尾空白
来源：http://biz.guowangkeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tns.dianchejie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lkj.yvedp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qmw.xingfuxueyuan.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ppq.nwbrower.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mqj.hnxiangtu.top

Go:   strings.TrimSpace(s)
来源：http://cxp.hfpthk.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ilx.shuidangran.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wfv.yuanzhike.top

[A25] 字符串比较
来源：http://pse.snrcjt.cn

Py:   s1 == s2; s1 != s2
来源：http://zls.andypj.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://aki.jiagoushi.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jjd.hesvh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wvr.pengpengdd.cyou

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tdl.hysaishi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://elu.jinqigfzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://vmc.yj202588.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mie.zdbjq.cn

[A26] 类型转换总览
来源：http://ghv.guowangkeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tkp.9152youxi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jwp.shangyingyoupin.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qef.hongshengwenyu.top

TS:   Number() String() Boolean() x as number
来源：http://xbr.316326.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://moh.yangfankeji.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xos.fzhhl.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://sri.aizwys.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zha.jinqigufen.top

================================================================================
来源：http://qen.smart0.xyz

B. 流程控制
来源：http://kqn.sysykeji.top

================================================================================
来源：http://cro.yueranfly.top

[B01] 条件判断 if / else
来源：http://mmq.yonumen.top

Py:   result = "正" if x > 0 else "非正"
来源：http://hto.zhongyouzk.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gqa.fanxiaobao.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sep.snrcjt.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mas.c1oappe.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://uts.jinghuilouyu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ked.uphjek.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qwm.9152youxi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sep.hammf.cn

[B02] 多分支 else if / elif
来源：http://les.yongpay.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qqy.jyoumei.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cny.ppjwa.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qbx.yongpay.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mef.yonumen.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wxe.yj202588.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dwa.zhaomingkeji.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://waz.quarkkingdee.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cca.zhixingplan.top

[B03] switch / match / case
来源：http://efb.c1oappe.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://oiz.shangyingyoupin.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://isz.chenjidiqi.icu

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pjd.fehbvm.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uyt.yj20258.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gmp.shuidangran.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eij.sufxvd.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mew.aizwys.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gxs.yj20258.top

[B04] for 计数循环
来源：http://vwz.ybcxt.top

Py:   for i in range(10): print(i)
来源：http://hci.uphjek.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sbu.chenjidiqi.icu

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tqh.gaohongyu789.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kps.tarul.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tib.shanyushiyangtech.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qas.sxryk.cn

Ruby: 10.times { |i| puts i }
来源：http://zqu.guannengcc.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fwq.yj20258888.top

[B05] 遍历数组 / 列表
来源：http://shi.pengpengdd.cyou

Py:   for item in arr: print(item)
来源：http://tlg.yueranfly.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jvo.zhoulong.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://gry.shanyushiyangtech.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qdk.yangfankeji.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://xwm.hcnkem.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pjs.cdnleiting.top

Ruby: arr.each { |item| puts item }
来源：http://nyc.yuanzhike.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dnu.yvedp.cn

[B06] 遍历字典 / 对象
来源：http://vqc.xinyue.icu

Py:   for k, v in d.items(): print(k, v)
来源：http://zpz.xingfuxueyuan.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uep.havefunace.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hby.mhx1999.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zkz.birdmap.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xep.hnxiangtu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xqr.jinqigfzy.top


<!-- 参考信息 -->