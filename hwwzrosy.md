代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://frj.jinghuilouyu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://erv.nanxinkj.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mmt.tarul.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zqv.nanxinkj.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://yzu.gzhubu.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pon.52xcode.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mqu.xuanzx.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uzp.zhengqikj.top

================================================================================
来源：http://elr.fanxiaobao.xyz

A. 基础语法与类型
来源：http://stx.hcnkem.com

================================================================================
来源：http://hij.ydjk.org.cn

[A01] Hello World
来源：http://tyy.ppjwa.cn

Py:   print("Hello, World!")
来源：http://zlg.fzhhl.top

PHP:  echo "Hello, World!";
来源：http://jzv.nanxuanxn.top

JS:   console.log("Hello, World!");
来源：http://wsi.jiagoushi.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nsm.havefunace.top

Java: System.out.println("Hello, World!");
来源：http://act.sufxvd.cn

Go:   fmt.Println("Hello, World!")
来源：http://gev.gaohongyu789.top

Ruby: puts "Hello, World!"
来源：http://yir.svipenyu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rku.jinghuilouyu.cn

[A02] 变量声明与赋值
来源：http://mel.yangfankeji.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nxc.ywan-chungtsiang.top

PHP:  $name = "Alex"; $age = 20;
来源：http://knp.uphjek.com

JS:   let name = "Alex"; const age = 20;
来源：http://wfk.fanxiaobao.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wgg.jqgufenzy.top

Java: String name = "Alex"; int age = 20;
来源：http://gfn.bbcook.cn

Go:   name := "Alex"; age := 20
来源：http://rob.yuanzhike.top

Ruby: name = "Alex"; age = 20
来源：http://gxy.gzhubu.top

C#:   string name = "Alex"; int age = 20;
来源：http://kry.guowangkeji.top

[A03] 常量定义
来源：http://kra.gzhubu.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lir.nanxinkj.top

PHP:  const PI = 3.14159;
来源：http://opy.bjfxy.top

JS:   const PI = 3.14159;
来源：http://tvf.hnxiangtu.top

TS:   const PI: number = 3.14159;
来源：http://xxt.zhaomingkeji.xyz

Java: static final double PI = 3.14159;
来源：http://knq.ydjk.org.cn

Go:   const PI = 3.14159
来源：http://hoi.jqgfzy.top

Ruby: PI = 3.14159
来源：http://lag.hnqzz.top

C#:   const double PI = 3.14159;
来源：http://tqr.jyoumei.cn

[A04] 判断变量类型
来源：http://xpj.mhx1999.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://naz.quarkkingdee.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dwn.jinyuanbaomall.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://die.bbcook.cn

TS:   typeof x; x instanceof Date
来源：http://kir.zhixingplan.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zlu.sjlbkw.cn

Go:   reflect.TypeOf(x).Name()
来源：http://nke.daria6918.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dgh.tian-w.cn

C#:   x.GetType().Name; x is int
来源：http://uei.birdmap.top

[A05] 整数除法与取模
来源：http://srb.hnqzz.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tfb.wangdashe.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://oxx.hesvh.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ivu.zdbjq.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uat.ppjwa.cn

Java: 7 / 2; 7 % 2
来源：http://qik.pycfn.com

Go:   7 / 2; 7 % 2
来源：http://vsu.daria6918.cn

Ruby: 7 / 2; 7 % 2
来源：http://goo.havefunace.top

C#:   7 / 2; 7 % 2
来源：http://yxb.gogol.net.cn

[A06] 字符串转数字
来源：http://hkw.52xcode.cn

Py:   int("42"); float("3.14")
来源：http://byj.jqgfzy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vxw.zdbjq.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://amw.guannengcc.top

TS:   parseInt("42", 10); Number("42")
来源：http://lss.hammf.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dbb.ppjwa.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ahb.cdnleiting.top

Ruby: "42".to_i; "3.14".to_f
来源：http://mad.tianlin.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vge.zhongyouzk.top

[A07] 数字转字符串
来源：http://knn.yj202588.top

Py:   str(42)
来源：http://acf.redwolf501.top

PHP:  (string) 42; strval(42)
来源：http://ulj.yongpay.top

JS:   String(42); (42).toString()
来源：http://peb.andypj.xyz

TS:   String(42)
来源：http://cpk.chenjidiqi.icu

Java: String.valueOf(42); Integer.toString(42)
来源：http://zas.guowangkeji.top

Go:   strconv.Itoa(42)
来源：http://bwa.hnxiangtu.top

Ruby: 42.to_s
来源：http://axq.fengsongda.top

C#:   42.ToString()
来源：http://elx.nanxuanxn.top

[A08] 取整与四舍五入
来源：http://fvk.cdnleiting.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pbu.wangshuangyany.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://uuz.yfazqb.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pnb.kuanghao11.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qxy.ydzc1.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fro.ydjk.org.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gap.yuxming.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wpy.sweek.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hgv.yangfankeji.com

[A09] 绝对值与最大最小值
来源：http://ztz.hnqzz.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bwt.sysykeji.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lqe.shangyingyoupin.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dhw.jinyuanbaomall.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cfj.daxiang520.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wbi.jinqigfzy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ihp.yj20258888.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://juu.zhoulong.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vif.316326.xyz

[A10] 生成随机数
来源：http://vzk.xylfe.cn

Py:   import random; random.randint(1, 100)
来源：http://mah.smart0.xyz

PHP:  random_int(1, 100);
来源：http://tks.shanyushiyangtech.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lrc.jinyuanbaomall.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vbm.hysaishi.cn

Java: new Random().nextInt(100) + 1
来源：http://jnx.vehdjk.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cla.chenzaomai.com

Ruby: rand(1..100)
来源：http://uua.xuetiantiany.cn

C#:   new Random().Next(1, 101)
来源：http://ybj.guannengcc.top

[A11] 条件表达式（三元）
来源：http://tya.zhongyouzk.top

Py:   "yes" if x > 0 else "no"
来源：http://eig.epnwcf.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://dye.wangdashe.top

JS:   x > 0 ? "yes" : "no"
来源：http://kcp.meibo888.top

TS:   x > 0 ? "yes" : "no"
来源：http://wrb.gogol.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://nrf.yongpay.top

Go:   // 无三元运算符，需用 if 语句
来源：http://eqk.tanke756.top

Ruby: x > 0 ? "yes" : "no"
来源：http://gcb.hywenlv.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wvk.fehbvm.com

[A12] 字符串插值 / 格式化
来源：http://rxb.jinqigfzy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qgo.gzhubu.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tid.shanyushiyangkeji.top

JS:   `Hello, ${name}!`
来源：http://uev.fengsongda.top

TS:   `Hello, ${name}!`
来源：http://ubk.hongshengwenyu.top

Java: "Hello, %s!".formatted(name)
来源：http://ivt.aibaodan.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kdp.epnwcf.com

Ruby: "Hello, #{name}!"
来源：http://egc.hesvh.cn

C#:   $"Hello, {name}!"
来源：http://hmm.cqqwz.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://tnu.yangfankeji.com

Py:   "第一行\n第二行"
来源：http://isk.jinghuilouyu.cn

PHP:  "第一行\n第二行"
来源：http://ahr.ydzc1.top

JS:   "第一行\n第二行"
来源：http://waj.fzhhl.top

TS:   "第一行\n第二行"
来源：http://lvd.9152youxi.cn

Java: "第一行\n第二行"
来源：http://unf.snrcjt.cn

Go:   "第一行\n第二行"
来源：http://sdp.hnqzz.top

Ruby: "第一行\n第二行"
来源：http://msj.tanke756.top

C#:   "第一行\n第二行"
来源：http://ras.tianlin.xyz

[A14] 注释写法
来源：http://skz.sweek.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://thy.ybcxt.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://gyi.zdbjq.cn

JS:   // 单行；/* 多行 */
来源：http://qqc.birdmap.top

TS:   // 单行；/* 多行 */
来源：http://fzn.yongpay.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qbo.chenzaomai.com

Go:   // 单行；/* 多行 */
来源：http://ngz.ppjwa.cn

Ruby: # 单行；=begin 多行 =end
来源：http://oih.yj20258.top

C#:   // 单行；/* 多行 */
来源：http://hri.wangdashe.top

[A15] 空值判断与默认值
来源：http://yov.guowangkeji.top

Py:   value = data or "默认值"
来源：http://aze.uphjek.com

PHP:  $value = $data ?? "默认值";
来源：http://nge.shanyushiyangkeji.top

JS:   const value = data ?? "默认值";
来源：http://mjh.hesvh.cn

TS:   const value = data ?? "默认值";
来源：http://kyn.aibaodan.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ikr.ppjwa.cn

Go:   if data == "" { data = "默认值" }
来源：http://mnz.uphjek.com

Ruby: value = data || "默认值"
来源：http://cqa.uphjek.com

C#:   var value = data ?? "默认值";
来源：http://bkq.yuxming.cn

[A16] 真假值判断规则
来源：http://lrx.jinqigfzy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://iuk.hywenlv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://aix.epnwcf.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qhj.sysykeji.top

TS:   if (!x) {}
来源：http://hfs.zhaomingkeji.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xug.hywenlv.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://chy.ctjpmb.com

Ruby: unless x            # nil 与 false 为假
来源：http://pjw.aibaodan.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ktl.yj202588.top

[A17] 位运算
来源：http://ukz.hammf.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hcs.zdqjudy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bbr.daria6918.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jgm.chenzaomai.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://iwp.zhongyouzk.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://alx.haohaochexian.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://egt.ydjk.org.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vif.ybcxt.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ceg.xylfe.cn

[A18] 字符与 ASCII 码互转
来源：http://sfo.ywan-chungtsiang.top

Py:   ord("A"); chr(65)
来源：http://moa.yj20258888.top

PHP:  ord("A"); chr(65)
来源：http://htk.zhijiandao.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wwc.xinyue.icu

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://czx.gogol.net.cn

Java: (int) 'A'; (char) 65
来源：http://wim.jinqigufen.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://epu.xziqi.cn

Ruby: "A".ord; 65.chr
来源：http://vvx.hesvh.cn

C#:   (int)'A'; (char)65
来源：http://bpc.xylfe.cn

[A19] 交换两个变量
来源：http://uzp.tianlin.xyz

Py:   a, b = b, a
来源：http://zpn.sysykeji.top

PHP:  [$a, $b] = [$b, $a];
来源：http://jai.kuanghao11.cn

JS:   [a, b] = [b, a];
来源：http://lii.birdmap.top

TS:   [a, b] = [b, a];
来源：http://dpr.nwbrower.top

Java: int t = a; a = b; b = t;
来源：http://qgt.yongpay.top

Go:   a, b = b, a
来源：http://ofo.chenjidiqi.icu

Ruby: a, b = b, a
来源：http://kbu.nanxuanxn.top

C#:   (a, b) = (b, a);
来源：http://rfp.hysaishi.cn

[A20] 读取标准输入
来源：http://hgw.pycfn.com

Py:   name = input("请输入：")
来源：http://kcd.hcnkem.com

PHP:  $name = trim(fgets(STDIN));
来源：http://coa.shangyingyoupin.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mdz.aizwys.cn

TS:   // Node.js：readline 模块
来源：http://bbn.zhoulong.xyz

Java: new Scanner(System.in).nextLine()
来源：http://jrk.52xcode.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jgz.hcnkem.com

Ruby: gets.chomp
来源：http://ept.hcnkem.com

C#:   Console.ReadLine();
来源：http://caz.hywenlv.cn

[A21] 保留指定小数位输出
来源：http://cve.nanxinkj.top

Py:   f"{3.14159:.2f}"
来源：http://wea.hnqzz.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fua.jinghuilouyu.cn

JS:   (3.14159).toFixed(2)
来源：http://kcn.zhijiandao.cn

TS:   (3.14159).toFixed(2)
来源：http://vhs.shzxlz.cn

Java: String.format("%.2f", 3.14159)
来源：http://zgp.quarkkingdee.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ojb.smart0.xyz

Ruby: format("%.2f", 3.14159)
来源：http://pbt.bbcook.cn

C#:   3.14159.ToString("F2")
来源：http://ufc.ybcxt.top

[A22] 获取字符串长度
来源：http://kbx.snrcjt.cn

Py:   len(s)
来源：http://jec.smart0.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fsy.gaohongyu789.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rpq.hnqzz.top

TS:   s.length
来源：http://iqs.hongshengwenyu.top

Java: s.length()
来源：http://nyu.haohaochexian.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fmb.smart0.xyz

Ruby: s.length
来源：http://flm.hammf.cn

C#:   s.Length
来源：http://tso.tianlin.xyz

[A23] 大小写转换
来源：http://hen.jinyuanbaomall.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tjm.xinyue.icu

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rqe.yangfankeji.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qyf.yj20258888.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jhm.sweek.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xpn.chenjidiqi.icu

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://uoz.hywenlv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yxu.ydzc1.top

C#:   s.ToUpper(); s.ToLower()
来源：http://wsd.shanyushiyangkeji.top

[A24] 去除首尾空白
来源：http://hqq.cashguo.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qem.shzxlz.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yvs.gaohongyu789.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vja.sweek.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dbj.sysykeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://riq.shangyingyoupin.top

Go:   strings.TrimSpace(s)
来源：http://big.yonumen.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nts.nanxinkj.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://efr.snrcjt.cn

[A25] 字符串比较
来源：http://agn.52xcode.cn

Py:   s1 == s2; s1 != s2
来源：http://fso.wangshuangyany.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jhn.cqqwz.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uto.ywan-chungtsiang.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yhi.shangyingyoupin.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mek.hesvh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wto.zdbjq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gcm.9152youxi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ngb.yueranfly.top

[A26] 类型转换总览
来源：http://zuy.hywenlv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ujn.sweek.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://eal.zhongyouzk.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jdi.yj20258888.top

TS:   Number() String() Boolean() x as number
来源：http://hpj.xuanzx.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xip.cdnleiting.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tsf.yuxming.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zyq.yuanzhike.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jxg.yj20258.top

================================================================================
来源：http://dnt.dianchejie.cn

B. 流程控制
来源：http://ape.shanyushiyangkeji.top

================================================================================
来源：http://fqv.ctjpmb.com

[B01] 条件判断 if / else
来源：http://ksg.nanxuanxn.top

Py:   result = "正" if x > 0 else "非正"
来源：http://kki.sysykeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zqr.zycfv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gek.shanyushiyangtech.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dco.cashguo.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://fkj.zhixingplan.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yxk.hcnkem.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mht.fengsongda.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xla.zdqjudy.top

[B02] 多分支 else if / elif
来源：http://fqw.aibaodan.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wxu.shanyushiyangtech.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://itd.zhengqikj.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kat.yuxming.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hfw.mhx1999.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://koq.yj20258.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lrw.kuanghao11.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uvd.chenlongwang.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fza.sysykeji.top

[B03] switch / match / case
来源：http://wbc.yanxiufei.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ujb.hesvh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fqr.jqgfzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hbh.epnwcf.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uku.hongshengwenyu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rcx.sufxvd.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tre.shangyingyoupin.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xne.xuanzx.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zve.birdmap.top

[B04] for 计数循环
来源：http://acd.hammf.cn

Py:   for i in range(10): print(i)
来源：http://zku.snrcjt.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://brn.zycfv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zbq.vqdsnc.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rel.zhixingplan.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rrl.yj20258.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oph.zhaomingkeji.xyz

Ruby: 10.times { |i| puts i }
来源：http://hlp.xylfe.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ocg.daria6918.cn

[B05] 遍历数组 / 列表
来源：http://spc.hywenlv.cn

Py:   for item in arr: print(item)
来源：http://oai.jyoumei.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gmi.daria6918.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tdz.nwbrower.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ccv.zhaomingkeji.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://iww.tianlin.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kgn.hcnkem.com

Ruby: arr.each { |item| puts item }
来源：http://tbm.yonumen.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uad.xinyue.icu

[B06] 遍历字典 / 对象
来源：http://ssm.guowangkeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://fio.jqgfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bmn.52xcode.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xcj.feifeiyinyue.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jaa.chenlongwang.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://paq.jinqigufen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://opl.vqdsnc.cn


<!-- 参考信息 -->