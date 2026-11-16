代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tim.cqqwz.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bfn.xinyue.icu

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ydb.fengsongda.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hdn.aibaodan.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cry.fzhhl.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sxv.yuanzhike.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ptb.hfpthk.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cyl.quarkkingdee.top

================================================================================
来源：http://dbf.guowangkeji.top

A. 基础语法与类型
来源：http://fng.hfpthk.cn

================================================================================
来源：http://xxr.zdqjudy.top

[A01] Hello World
来源：http://xml.wangdashe.top

Py:   print("Hello, World!")
来源：http://ati.smart0.xyz

PHP:  echo "Hello, World!";
来源：http://lvu.zhoulong.xyz

JS:   console.log("Hello, World!");
来源：http://zaq.jinqigfzy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tgh.vehdjk.com

Java: System.out.println("Hello, World!");
来源：http://uqt.yj20258888.top

Go:   fmt.Println("Hello, World!")
来源：http://vjv.zdqjudy.top

Ruby: puts "Hello, World!"
来源：http://typ.nwbrower.top

C#:   Console.WriteLine("Hello, World!");
来源：http://vgc.fzhhl.top

[A02] 变量声明与赋值
来源：http://kde.aibaodan.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rdm.gotoacloud.top

PHP:  $name = "Alex"; $age = 20;
来源：http://xzo.yangfankeji.com

JS:   let name = "Alex"; const age = 20;
来源：http://dal.hnqzz.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zvs.zhaomingkeji.xyz

Java: String name = "Alex"; int age = 20;
来源：http://psj.jyoumei.cn

Go:   name := "Alex"; age := 20
来源：http://mob.yuxming.cn

Ruby: name = "Alex"; age = 20
来源：http://jxt.yj20258888.top

C#:   string name = "Alex"; int age = 20;
来源：http://igj.cucudq.cn

[A03] 常量定义
来源：http://xok.dianchejie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yzm.bjfxy.top

PHP:  const PI = 3.14159;
来源：http://crv.shzxlz.cn

JS:   const PI = 3.14159;
来源：http://zij.316326.xyz

TS:   const PI: number = 3.14159;
来源：http://cly.jianghu66.top

Java: static final double PI = 3.14159;
来源：http://nwg.wangshuangyany.cn

Go:   const PI = 3.14159
来源：http://ogc.kuanghao11.cn

Ruby: PI = 3.14159
来源：http://xyv.hammf.cn

C#:   const double PI = 3.14159;
来源：http://eje.zhoulong.xyz

[A04] 判断变量类型
来源：http://ehd.haohaochexian.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://mle.yueranfly.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ovm.meibo888.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ypi.yj20258.top

TS:   typeof x; x instanceof Date
来源：http://dqb.yangfankeji.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://khp.wangshuangyany.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rbh.nanxinkj.top

Ruby: x.class; x.is_a?(Integer)
来源：http://urc.jlsjyb.cn

C#:   x.GetType().Name; x is int
来源：http://qvk.wangshuangyany.cn

[A05] 整数除法与取模
来源：http://csy.52xcode.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xgi.andypj.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://qho.zhaomingkeji.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zpz.316326.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nju.jinghuilouyu.cn

Java: 7 / 2; 7 % 2
来源：http://acp.xuetiantiany.cn

Go:   7 / 2; 7 % 2
来源：http://vqz.shanyushiyangkeji.top

Ruby: 7 / 2; 7 % 2
来源：http://yso.ppjwa.cn

C#:   7 / 2; 7 % 2
来源：http://bqk.yuanzhike.top

[A06] 字符串转数字
来源：http://ikk.redwolf501.top

Py:   int("42"); float("3.14")
来源：http://juc.nwbrower.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cmw.zdqjudy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hds.jqgfzy.top

TS:   parseInt("42", 10); Number("42")
来源：http://jlg.sweek.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xqo.wangdashe.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ozh.hammf.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://mft.jinqigufen.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://eoq.ydjk.org.cn

[A07] 数字转字符串
来源：http://zpx.gogol.net.cn

Py:   str(42)
来源：http://pdn.yueranfly.top

PHP:  (string) 42; strval(42)
来源：http://ltx.hysaishi.cn

JS:   String(42); (42).toString()
来源：http://vex.zhongyouzk.top

TS:   String(42)
来源：http://vyo.wangdashe.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://tly.smart0.xyz

Go:   strconv.Itoa(42)
来源：http://dwu.shanyushiyangkeji.top

Ruby: 42.to_s
来源：http://mrq.hfpthk.cn

C#:   42.ToString()
来源：http://prx.cashguo.top

[A08] 取整与四舍五入
来源：http://yst.ydzc1.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wzw.shzxlz.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kxj.shanyushiyangtech.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vsk.jinqigfzy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tll.xuanzx.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://iul.andypj.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qpb.yanxiufei.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sgy.xingfuxueyuan.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lmd.gzhubu.top

[A09] 绝对值与最大最小值
来源：http://dmh.hfpthk.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yjj.yfazqb.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gth.cashguo.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ojl.tian-w.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dmf.fehbvm.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://skc.pengpengdd.cyou

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pet.gotoacloud.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bfo.fanxiaobao.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://die.dianchejie.cn

[A10] 生成随机数
来源：http://eyv.meibo888.top

Py:   import random; random.randint(1, 100)
来源：http://yfj.zhaomingkeji.xyz

PHP:  random_int(1, 100);
来源：http://kku.smart0.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pwa.yangfankeji.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bmj.ydzc1.top

Java: new Random().nextInt(100) + 1
来源：http://jjh.meibo888.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xid.ydzc1.top

Ruby: rand(1..100)
来源：http://syh.zhixingplan.top

C#:   new Random().Next(1, 101)
来源：http://fay.cucudq.cn

[A11] 条件表达式（三元）
来源：http://pku.gogol.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://mxh.xingfuxueyuan.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://qkz.andypj.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://wcu.birdmap.top

TS:   x > 0 ? "yes" : "no"
来源：http://iuk.cdnleiting.top

Java: x > 0 ? "yes" : "no"
来源：http://nfg.yj20258.top

Go:   // 无三元运算符，需用 if 语句
来源：http://mxk.fzhhl.top

Ruby: x > 0 ? "yes" : "no"
来源：http://mnk.bbcook.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hqn.aibaodan.cn

[A12] 字符串插值 / 格式化
来源：http://zje.hysaishi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jmq.zdbjq.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://huh.yj202588.top

JS:   `Hello, ${name}!`
来源：http://ogb.jyoumei.cn

TS:   `Hello, ${name}!`
来源：http://idm.smart0.xyz

Java: "Hello, %s!".formatted(name)
来源：http://fvy.yonumen.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://egg.tanke756.top

Ruby: "Hello, #{name}!"
来源：http://tia.ybcxt.top

C#:   $"Hello, {name}!"
来源：http://apj.svipenyu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://yyp.jqgufenzy.top

Py:   "第一行\n第二行"
来源：http://glg.daxiang520.top

PHP:  "第一行\n第二行"
来源：http://vcw.fktsv.cn

JS:   "第一行\n第二行"
来源：http://wip.jinqigufen.top

TS:   "第一行\n第二行"
来源：http://ngg.tian-w.cn

Java: "第一行\n第二行"
来源：http://wyb.yj20258888.top

Go:   "第一行\n第二行"
来源：http://hyo.yongpay.top

Ruby: "第一行\n第二行"
来源：http://who.zdbjq.cn

C#:   "第一行\n第二行"
来源：http://isd.jinyuanbaomall.cn

[A14] 注释写法
来源：http://azu.bbcook.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://koa.yonumen.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://eji.dashuyun.cn

JS:   // 单行；/* 多行 */
来源：http://ibq.52xcode.cn

TS:   // 单行；/* 多行 */
来源：http://mja.yj202588.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yaa.chenzaomai.com

Go:   // 单行；/* 多行 */
来源：http://lfm.ydzc1.top

Ruby: # 单行；=begin 多行 =end
来源：http://pxk.xylfe.cn

C#:   // 单行；/* 多行 */
来源：http://bqg.zhijiandao.cn

[A15] 空值判断与默认值
来源：http://nqh.yangfankeji.com

Py:   value = data or "默认值"
来源：http://hza.hesvh.cn

PHP:  $value = $data ?? "默认值";
来源：http://rpq.ybcxt.top

JS:   const value = data ?? "默认值";
来源：http://yaz.fehbvm.com

TS:   const value = data ?? "默认值";
来源：http://kpc.daxiang520.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://syj.xuanzx.com

Go:   if data == "" { data = "默认值" }
来源：http://ahg.xuetiantiany.cn

Ruby: value = data || "默认值"
来源：http://obb.cashguo.top

C#:   var value = data ?? "默认值";
来源：http://yik.bjfxy.top

[A16] 真假值判断规则
来源：http://qzs.jinqigfzy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qzr.yuxming.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wci.tarul.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ebw.yj20258.top

TS:   if (!x) {}
来源：http://hkf.andypj.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vzd.zdqjudy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vas.c1oappe.top

Ruby: unless x            # nil 与 false 为假
来源：http://wty.xuetiantiany.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sbn.yj20258.top

[A17] 位运算
来源：http://cjr.jinqigufen.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xlx.cashguo.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lsl.shanyushiyangtech.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://icr.xuetiantiany.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jzq.zdqjudy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ofi.shanyushiyangkeji.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rff.ivvv.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://stc.zhaomingkeji.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cmm.xziqi.cn

[A18] 字符与 ASCII 码互转
来源：http://apr.hfpthk.cn

Py:   ord("A"); chr(65)
来源：http://eyd.fktsv.cn

PHP:  ord("A"); chr(65)
来源：http://xht.chenlongwang.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ccs.gaohongyu789.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vwe.cucudq.cn

Java: (int) 'A'; (char) 65
来源：http://pta.wangdashe.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ttv.jianghu66.top

Ruby: "A".ord; 65.chr
来源：http://pat.wangshuangyany.cn

C#:   (int)'A'; (char)65
来源：http://nvd.zhoulong.xyz

[A19] 交换两个变量
来源：http://mze.birdmap.top

Py:   a, b = b, a
来源：http://ojc.jiagoushi.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ymz.zycfv.cn

JS:   [a, b] = [b, a];
来源：http://hqj.jyoumei.cn

TS:   [a, b] = [b, a];
来源：http://sky.zdqjudy.top

Java: int t = a; a = b; b = t;
来源：http://cbc.316326.xyz

Go:   a, b = b, a
来源：http://orh.zhoulong.xyz

Ruby: a, b = b, a
来源：http://poe.aizwys.cn

C#:   (a, b) = (b, a);
来源：http://ldy.aibaodan.cn

[A20] 读取标准输入
来源：http://yhu.xuetiantiany.cn

Py:   name = input("请输入：")
来源：http://fum.haohaochexian.top

PHP:  $name = trim(fgets(STDIN));
来源：http://zan.jiagoushi.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dfx.hnxiangtu.top

TS:   // Node.js：readline 模块
来源：http://gtr.nwbrower.top

Java: new Scanner(System.in).nextLine()
来源：http://jzk.jinqigfzy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fgy.cucudq.cn

Ruby: gets.chomp
来源：http://vze.hammf.cn

C#:   Console.ReadLine();
来源：http://kqo.sysykeji.top

[A21] 保留指定小数位输出
来源：http://zlk.jiagoushi.top

Py:   f"{3.14159:.2f}"
来源：http://pxd.andypj.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ubo.uphjek.com

JS:   (3.14159).toFixed(2)
来源：http://yyt.ywan-chungtsiang.top

TS:   (3.14159).toFixed(2)
来源：http://mlz.aizwys.cn

Java: String.format("%.2f", 3.14159)
来源：http://tcy.zhijiandao.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jlr.quarkkingdee.top

Ruby: format("%.2f", 3.14159)
来源：http://qhd.hesvh.cn

C#:   3.14159.ToString("F2")
来源：http://nmc.vqdsnc.cn

[A22] 获取字符串长度
来源：http://rmn.sxryk.cn

Py:   len(s)
来源：http://cdc.snrcjt.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gqz.hywenlv.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zwm.mhx1999.top

TS:   s.length
来源：http://wri.zhixingplan.top

Java: s.length()
来源：http://erk.hnxiangtu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cak.chenzaomai.com

Ruby: s.length
来源：http://bus.hongshengwenyu.top

C#:   s.Length
来源：http://wej.smart0.xyz

[A23] 大小写转换
来源：http://hmy.hesvh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fen.yfazqb.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zrt.uphjek.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://reb.zhengqikj.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ucd.sjlbkw.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xna.yvedp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://awt.redwolf501.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jrp.haohaochexian.top

C#:   s.ToUpper(); s.ToLower()
来源：http://asa.jinqigfzy.top

[A24] 去除首尾空白
来源：http://trv.ivvv.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mai.zhaomingkeji.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ief.zhixingplan.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nvx.cashguo.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uxe.xziqi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xsc.gogol.net.cn

Go:   strings.TrimSpace(s)
来源：http://jnn.xylfe.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uce.daria6918.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gjm.hywenlv.cn

[A25] 字符串比较
来源：http://izs.chenjidiqi.icu

Py:   s1 == s2; s1 != s2
来源：http://fhw.jianghu66.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hpq.yvedp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kym.52xcode.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tay.dianchejie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xpu.shuidangran.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mhv.chenjidiqi.icu

Ruby: s1 == s2; s1 <=> s2
来源：http://cff.c1oappe.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jjr.jqgufenzy.top

[A26] 类型转换总览
来源：http://stw.gogol.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ifi.xziqi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jns.jyoumei.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ift.hammf.cn

TS:   Number() String() Boolean() x as number
来源：http://vfx.cdnleiting.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jxx.ydjk.org.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tny.sjlbkw.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zib.cheryme.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nqm.feifeiyinyue.top

================================================================================
来源：http://spj.cashguo.top

B. 流程控制
来源：http://oju.cashguo.top

================================================================================
来源：http://xek.nanxuanxn.top

[B01] 条件判断 if / else
来源：http://tvk.gzhubu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://wpe.dashuyun.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bvi.aizwys.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ejf.cqqwz.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rws.fehbvm.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://eqi.c1oappe.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dwj.meibo888.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lwt.52xcode.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vpo.jqgufenzy.top

[B02] 多分支 else if / elif
来源：http://jyj.daria6918.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rhn.chenjidiqi.icu

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://izs.ybcxt.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yvc.hfpthk.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://esj.hnqzz.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xax.zdqjudy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xmx.shuidangran.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dwr.jqgufenzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kad.tian-w.cn

[B03] switch / match / case
来源：http://sgr.guannengcc.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ovt.fktsv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jih.shangyingyoupin.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gcb.aibaodan.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bbr.chenlongwang.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rly.yvedp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jnc.hammf.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fbc.tanke756.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://epp.hysaishi.cn

[B04] for 计数循环
来源：http://fhw.hcnkem.com

Py:   for i in range(10): print(i)
来源：http://jrt.nanxuanxn.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uon.yj20258888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cub.fzhhl.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vqz.wangshuangyany.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://alh.ctjpmb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mtn.sjlbkw.cn

Ruby: 10.times { |i| puts i }
来源：http://wvd.ybcxt.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ski.zycfv.cn

[B05] 遍历数组 / 列表
来源：http://btu.jqgufenzy.top

Py:   for item in arr: print(item)
来源：http://ctk.hfpthk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://efj.52xcode.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nau.svipenyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tgb.zycfv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tuv.ppjwa.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pok.daxiang520.top

Ruby: arr.each { |item| puts item }
来源：http://krs.ydjk.org.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tjc.gaohongyu789.top

[B06] 遍历字典 / 对象
来源：http://xfm.sxryk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cml.chenzaomai.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zgv.svipenyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jqs.jlsjyb.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jru.hnqzz.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tdc.nwbrower.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://abt.xziqi.cn


<!-- 参考信息 -->