代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dgt.zhiwuduotai.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://aap.fktsv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dwa.fengsongda.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qjr.sysykeji.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://zwq.ywan-chungtsiang.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://glf.hcnkem.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ljn.jinqigfzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qwu.guowangkeji.top

================================================================================
来源：http://fuq.vehdjk.com

A. 基础语法与类型
来源：http://jcp.tian-w.cn

================================================================================
来源：http://awb.jianghu66.top

[A01] Hello World
来源：http://axb.xinyue.icu

Py:   print("Hello, World!")
来源：http://zbt.ywan-chungtsiang.top

PHP:  echo "Hello, World!";
来源：http://ofv.cheryme.top

JS:   console.log("Hello, World!");
来源：http://gnd.sufxvd.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://oir.jinqigufen.top

Java: System.out.println("Hello, World!");
来源：http://jwp.cdnleiting.top

Go:   fmt.Println("Hello, World!")
来源：http://xse.yangfankeji.com

Ruby: puts "Hello, World!"
来源：http://qbd.chenjidiqi.icu

C#:   Console.WriteLine("Hello, World!");
来源：http://npg.uphjek.com

[A02] 变量声明与赋值
来源：http://lcp.gogol.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pca.chenzaomai.com

PHP:  $name = "Alex"; $age = 20;
来源：http://ait.zhixingplan.top

JS:   let name = "Alex"; const age = 20;
来源：http://kfb.hywenlv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qve.jianghu66.top

Java: String name = "Alex"; int age = 20;
来源：http://tre.yj202588.top

Go:   name := "Alex"; age := 20
来源：http://ptj.shzxlz.cn

Ruby: name = "Alex"; age = 20
来源：http://afs.52xcode.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gwz.zhiwuduotai.top

[A03] 常量定义
来源：http://hjw.hcnkem.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://esd.nwbrower.top

PHP:  const PI = 3.14159;
来源：http://shz.birdmap.top

JS:   const PI = 3.14159;
来源：http://xei.cucudq.cn

TS:   const PI: number = 3.14159;
来源：http://rel.ywan-chungtsiang.top

Java: static final double PI = 3.14159;
来源：http://ijn.wangdashe.top

Go:   const PI = 3.14159
来源：http://rpb.yangfankeji.com

Ruby: PI = 3.14159
来源：http://fax.zhijiandao.cn

C#:   const double PI = 3.14159;
来源：http://tyb.guowangkeji.top

[A04] 判断变量类型
来源：http://pyv.xuanzx.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://dat.yvedp.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uzo.jinqigufen.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vnr.bbcook.cn

TS:   typeof x; x instanceof Date
来源：http://jgf.yj20258.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dps.jinghuilouyu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://caj.chenzaomai.com

Ruby: x.class; x.is_a?(Integer)
来源：http://qfe.uphjek.com

C#:   x.GetType().Name; x is int
来源：http://usu.jyoumei.cn

[A05] 整数除法与取模
来源：http://pvy.yanxiufei.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wzd.ppjwa.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fjz.nanxuanxn.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yit.xingfuxueyuan.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cvc.ydjk.org.cn

Java: 7 / 2; 7 % 2
来源：http://wyp.jinqigufen.top

Go:   7 / 2; 7 % 2
来源：http://jmm.dianchejie.cn

Ruby: 7 / 2; 7 % 2
来源：http://sgd.redwolf501.top

C#:   7 / 2; 7 % 2
来源：http://zzu.nanxinkj.top

[A06] 字符串转数字
来源：http://iwq.ehwqpu.com

Py:   int("42"); float("3.14")
来源：http://awe.quarkkingdee.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://res.chenzaomai.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zor.yj20258888.top

TS:   parseInt("42", 10); Number("42")
来源：http://kgh.chenjidiqi.icu

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xhv.dianchejie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rxf.jqgufenzy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://qqi.jianghu66.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://oim.jianghu66.top

[A07] 数字转字符串
来源：http://xxe.sufxvd.cn

Py:   str(42)
来源：http://nii.snrcjt.cn

PHP:  (string) 42; strval(42)
来源：http://uaa.ywan-chungtsiang.top

JS:   String(42); (42).toString()
来源：http://ihx.zdqjudy.top

TS:   String(42)
来源：http://ied.yueranfly.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ilt.nwbrower.top

Go:   strconv.Itoa(42)
来源：http://spt.bbcook.cn

Ruby: 42.to_s
来源：http://emx.yanxiufei.cn

C#:   42.ToString()
来源：http://mxw.snrcjt.cn

[A08] 取整与四舍五入
来源：http://sof.ydzc1.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wyx.yvedp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qfi.jianghu66.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ouo.quarkkingdee.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rgc.cashguo.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nkh.aibaodan.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hfm.c1oappe.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://xgk.jinqigufen.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mos.jianghu66.top

[A09] 绝对值与最大最小值
来源：http://dje.shanyushiyangkeji.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ytp.xylfe.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lbf.hesvh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nli.cqqwz.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://krc.guowangkeji.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://afw.gogol.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ygw.yj20258888.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xww.jqgfzy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ady.xuetiantiany.cn

[A10] 生成随机数
来源：http://kfv.c1oappe.top

Py:   import random; random.randint(1, 100)
来源：http://ymz.nanxinkj.top

PHP:  random_int(1, 100);
来源：http://ypr.shanyushiyangtech.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://eyh.zdbjq.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ilf.c1oappe.top

Java: new Random().nextInt(100) + 1
来源：http://kye.uphjek.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bbi.gzhubu.top

Ruby: rand(1..100)
来源：http://xyl.shzxlz.cn

C#:   new Random().Next(1, 101)
来源：http://xtk.shuidangran.top

[A11] 条件表达式（三元）
来源：http://zwa.aizwys.cn

Py:   "yes" if x > 0 else "no"
来源：http://xii.smart0.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://yos.tarul.cn

JS:   x > 0 ? "yes" : "no"
来源：http://dvr.yonumen.top

TS:   x > 0 ? "yes" : "no"
来源：http://yee.ywan-chungtsiang.top

Java: x > 0 ? "yes" : "no"
来源：http://aej.yuanzhike.top

Go:   // 无三元运算符，需用 if 语句
来源：http://vmw.havefunace.top

Ruby: x > 0 ? "yes" : "no"
来源：http://vsm.sweek.top

C#:   x > 0 ? "yes" : "no"
来源：http://gxk.yongpay.top

[A12] 字符串插值 / 格式化
来源：http://pns.shanyushiyangtech.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ekt.316326.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kdu.yvedp.cn

JS:   `Hello, ${name}!`
来源：http://ekc.yangfankeji.com

TS:   `Hello, ${name}!`
来源：http://hkx.daxiang520.top

Java: "Hello, %s!".formatted(name)
来源：http://wul.jqgfzy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qyw.gotoacloud.top

Ruby: "Hello, #{name}!"
来源：http://efv.hammf.cn

C#:   $"Hello, {name}!"
来源：http://eyt.fehbvm.com

[A13] 多行字符串（练习 \n 转义）
来源：http://nlv.gotoacloud.top

Py:   "第一行\n第二行"
来源：http://zsj.yuxming.cn

PHP:  "第一行\n第二行"
来源：http://aqk.nwbrower.top

JS:   "第一行\n第二行"
来源：http://vzq.andypj.xyz

TS:   "第一行\n第二行"
来源：http://hmf.xingfuxueyuan.xyz

Java: "第一行\n第二行"
来源：http://ebc.yvedp.cn

Go:   "第一行\n第二行"
来源：http://xaa.wangshuangyany.cn

Ruby: "第一行\n第二行"
来源：http://dor.cqqwz.cn

C#:   "第一行\n第二行"
来源：http://kjs.yvedp.cn

[A14] 注释写法
来源：http://pzk.daxiang520.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://sue.dianchejie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://odu.xingfuxueyuan.xyz

JS:   // 单行；/* 多行 */
来源：http://eny.cashguo.top

TS:   // 单行；/* 多行 */
来源：http://jdi.zhiwuduotai.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://chg.nanxuanxn.top

Go:   // 单行；/* 多行 */
来源：http://cbw.havefunace.top

Ruby: # 单行；=begin 多行 =end
来源：http://fwm.ivvv.top

C#:   // 单行；/* 多行 */
来源：http://vcb.andypj.xyz

[A15] 空值判断与默认值
来源：http://hki.yvedp.cn

Py:   value = data or "默认值"
来源：http://ogf.ehwqpu.com

PHP:  $value = $data ?? "默认值";
来源：http://xjz.xylfe.cn

JS:   const value = data ?? "默认值";
来源：http://ebt.yonumen.top

TS:   const value = data ?? "默认值";
来源：http://pkr.shangyingyoupin.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ujb.fehbvm.com

Go:   if data == "" { data = "默认值" }
来源：http://kvm.zdqjudy.top

Ruby: value = data || "默认值"
来源：http://afo.yueranfly.top

C#:   var value = data ?? "默认值";
来源：http://ztf.hammf.cn

[A16] 真假值判断规则
来源：http://mtv.chenzaomai.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://uht.chenzaomai.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wqd.pengpengdd.cyou

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uqc.yj20258888.top

TS:   if (!x) {}
来源：http://usq.316326.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://die.xziqi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hwx.fehbvm.com

Ruby: unless x            # nil 与 false 为假
来源：http://lil.vqdsnc.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wsn.fengsongda.top

[A17] 位运算
来源：http://tco.shzxlz.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ppv.aizwys.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mqw.yvedp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kto.zhaomingkeji.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hlg.zhijiandao.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wwb.wangshuangyany.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ljc.pengpengdd.cyou

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mvt.gotoacloud.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://izp.feifeiyinyue.top

[A18] 字符与 ASCII 码互转
来源：http://glb.meibo888.top

Py:   ord("A"); chr(65)
来源：http://hmq.shanyushiyangtech.top

PHP:  ord("A"); chr(65)
来源：http://lni.hesvh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zqz.hcnkem.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vsy.svipenyu.cn

Java: (int) 'A'; (char) 65
来源：http://yvy.hnqzz.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ryc.dashuyun.cn

Ruby: "A".ord; 65.chr
来源：http://xzf.chenjidiqi.icu

C#:   (int)'A'; (char)65
来源：http://pas.jinqigufen.top

[A19] 交换两个变量
来源：http://ibe.zhengqikj.top

Py:   a, b = b, a
来源：http://qxd.hongshengwenyu.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ebo.hongshengwenyu.top

JS:   [a, b] = [b, a];
来源：http://vlq.hongshengwenyu.top

TS:   [a, b] = [b, a];
来源：http://nqw.jyoumei.cn

Java: int t = a; a = b; b = t;
来源：http://ufp.fehbvm.com

Go:   a, b = b, a
来源：http://ejv.jinghuilouyu.cn

Ruby: a, b = b, a
来源：http://uee.yuxming.cn

C#:   (a, b) = (b, a);
来源：http://owi.yangfankeji.com

[A20] 读取标准输入
来源：http://qhi.kuanghao11.cn

Py:   name = input("请输入：")
来源：http://lib.yongpay.top

PHP:  $name = trim(fgets(STDIN));
来源：http://xfz.0kj1m.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wch.sxryk.cn

TS:   // Node.js：readline 模块
来源：http://hqs.pengpengdd.cyou

Java: new Scanner(System.in).nextLine()
来源：http://yuk.yueranfly.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tla.yuxming.cn

Ruby: gets.chomp
来源：http://csd.quarkkingdee.top

C#:   Console.ReadLine();
来源：http://uwt.hnqzz.top

[A21] 保留指定小数位输出
来源：http://sxl.ppjwa.cn

Py:   f"{3.14159:.2f}"
来源：http://mmw.yuxming.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fxr.iojbl.cn

JS:   (3.14159).toFixed(2)
来源：http://yxu.yangfankeji.com

TS:   (3.14159).toFixed(2)
来源：http://xun.ppjwa.cn

Java: String.format("%.2f", 3.14159)
来源：http://fzi.zhoulong.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zle.bbcook.cn

Ruby: format("%.2f", 3.14159)
来源：http://wiu.yuanzhike.top

C#:   3.14159.ToString("F2")
来源：http://cqx.hesvh.cn

[A22] 获取字符串长度
来源：http://xwy.hongshengwenyu.top

Py:   len(s)
来源：http://zkp.hnxiangtu.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nen.yj20258888.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kbj.hfpthk.cn

TS:   s.length
来源：http://siw.yj202588.top

Java: s.length()
来源：http://rdj.zdbjq.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cxz.zdbjq.cn

Ruby: s.length
来源：http://qcr.uphjek.com

C#:   s.Length
来源：http://rgo.shuidangran.top

[A23] 大小写转换
来源：http://ntf.pengpengdd.cyou

Py:   s.upper(); s.lower(); s.title()
来源：http://ann.jinghuilouyu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vsu.fengsongda.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://izt.jyoumei.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hwg.xingfuxueyuan.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cxg.316326.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://isa.havefunace.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://but.zhengqikj.top

C#:   s.ToUpper(); s.ToLower()
来源：http://dhl.yongpay.top

[A24] 去除首尾空白
来源：http://pxz.feifeiyinyue.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://efu.daxiang520.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://msg.fanxiaobao.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cvj.sufxvd.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bul.yonumen.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ipn.guannengcc.top

Go:   strings.TrimSpace(s)
来源：http://obx.dashuyun.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yqs.yangfankeji.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dyd.uphjek.com

[A25] 字符串比较
来源：http://ayb.tianlin.xyz

Py:   s1 == s2; s1 != s2
来源：http://tfr.tian-w.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lwi.hysaishi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://poj.jyoumei.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fxu.sufxvd.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yez.cucudq.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vmy.guowangkeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://cvf.yueranfly.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wxr.chenjidiqi.icu

[A26] 类型转换总览
来源：http://gpv.tanke756.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gmc.zhiwuduotai.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://osq.316326.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xwa.nanxinkj.top

TS:   Number() String() Boolean() x as number
来源：http://npr.shanyushiyangtech.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://agx.shuidangran.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cve.aibaodan.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rvc.zdqjudy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dtx.hfpthk.cn

================================================================================
来源：http://qqb.vehdjk.com

B. 流程控制
来源：http://oxa.gogol.net.cn

================================================================================
来源：http://rde.zhiwuduotai.top

[B01] 条件判断 if / else
来源：http://ixy.sysykeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ujv.hfpthk.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hbo.jyoumei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jzi.jinqigfzy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dsw.tanke756.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://nok.hnxiangtu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zza.gotoacloud.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://djd.havefunace.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bdm.hnqzz.top

[B02] 多分支 else if / elif
来源：http://vqp.ybcxt.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dxi.feifeiyinyue.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uuu.guannengcc.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://psj.gotoacloud.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qzz.dianchejie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rdi.hammf.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zcd.gogol.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sie.aibaodan.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hvk.zhengqikj.top

[B03] switch / match / case
来源：http://hgz.zhixingplan.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kyx.zdqjudy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xnq.yanxiufei.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bdq.0kj1m.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qtz.nanxuanxn.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uiw.cheryme.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gym.zhoulong.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qbm.hywenlv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zrd.tianlin.xyz

[B04] for 计数循环
来源：http://cpp.c1oappe.top

Py:   for i in range(10): print(i)
来源：http://ile.feifeiyinyue.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uar.hnxiangtu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jok.cdnleiting.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ckk.havefunace.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jzn.meibo888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ivw.zhiwuduotai.top

Ruby: 10.times { |i| puts i }
来源：http://yul.ydzc1.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://agb.ybcxt.top

[B05] 遍历数组 / 列表
来源：http://rma.aibaodan.cn

Py:   for item in arr: print(item)
来源：http://vsg.epnwcf.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hmx.jlsjyb.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rqn.shanyushiyangkeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://oun.fzhhl.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mtb.yonumen.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xxh.feifeiyinyue.top

Ruby: arr.each { |item| puts item }
来源：http://geq.uphjek.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ixg.yuxming.cn

[B06] 遍历字典 / 对象
来源：http://fdb.yueranfly.top

Py:   for k, v in d.items(): print(k, v)
来源：http://cuj.cucudq.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vab.shangyingyoupin.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vvw.quarkkingdee.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nvg.gogol.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://otx.hnxiangtu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://auk.dashuyun.cn


<!-- 参考信息 -->