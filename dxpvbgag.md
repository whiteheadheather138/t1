代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://ala.sxryk.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hbl.ctjpmb.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ejf.c1oappe.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kvi.xuetiantiany.cn

================================================================================
来源：http://eng.gzhubu.top

A. 基础语法与类型
来源：http://yif.xylfe.cn

================================================================================
来源：http://gdd.chenlongwang.top

[A01] Hello World
来源：http://fet.fengsongda.top

Py:   print("Hello, World!")
来源：http://svm.gaohongyu789.top

PHP:  echo "Hello, World!";
来源：http://pcj.yj202588.top

JS:   console.log("Hello, World!");
来源：http://cdk.kuanghao11.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ohr.shuidangran.top

Java: System.out.println("Hello, World!");
来源：http://bsq.52xcode.cn

Go:   fmt.Println("Hello, World!")
来源：http://ogq.svipenyu.cn

Ruby: puts "Hello, World!"
来源：http://eci.shuidangran.top

C#:   Console.WriteLine("Hello, World!");
来源：http://icx.hongshengwenyu.top

[A02] 变量声明与赋值
来源：http://mjn.hywenlv.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ayc.ivvv.top

PHP:  $name = "Alex"; $age = 20;
来源：http://eoj.yvedp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://rfn.xingfuxueyuan.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ehm.pengpengdd.cyou

Java: String name = "Alex"; int age = 20;
来源：http://pti.zhongyouzk.top

Go:   name := "Alex"; age := 20
来源：http://dsw.chenlongwang.top

Ruby: name = "Alex"; age = 20
来源：http://oor.sweek.top

C#:   string name = "Alex"; int age = 20;
来源：http://bcb.xuanzx.com

[A03] 常量定义
来源：http://ypr.nwbrower.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://llj.ybcxt.top

PHP:  const PI = 3.14159;
来源：http://nun.aibaodan.cn

JS:   const PI = 3.14159;
来源：http://idx.hesvh.cn

TS:   const PI: number = 3.14159;
来源：http://oxj.hnxiangtu.top

Java: static final double PI = 3.14159;
来源：http://lkw.bjfxy.top

Go:   const PI = 3.14159
来源：http://bgw.yvedp.cn

Ruby: PI = 3.14159
来源：http://omw.chenjidiqi.icu

C#:   const double PI = 3.14159;
来源：http://qes.ppjwa.cn

[A04] 判断变量类型
来源：http://dnc.cdnleiting.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://pbc.ybcxt.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://atd.ywan-chungtsiang.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zgl.iojbl.cn

TS:   typeof x; x instanceof Date
来源：http://mvm.feifeiyinyue.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dmu.havefunace.top

Go:   reflect.TypeOf(x).Name()
来源：http://cpm.epnwcf.com

Ruby: x.class; x.is_a?(Integer)
来源：http://zml.zhijiandao.cn

C#:   x.GetType().Name; x is int
来源：http://tlr.svipenyu.cn

[A05] 整数除法与取模
来源：http://yxe.ybcxt.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gbj.uphjek.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://fru.zhiwuduotai.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rxt.9152youxi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uyy.yangfankeji.com

Java: 7 / 2; 7 % 2
来源：http://ctc.hywenlv.cn

Go:   7 / 2; 7 % 2
来源：http://faw.hcnkem.com

Ruby: 7 / 2; 7 % 2
来源：http://qmv.mhx1999.top

C#:   7 / 2; 7 % 2
来源：http://ilu.chenlongwang.top

[A06] 字符串转数字
来源：http://bry.yj20258.top

Py:   int("42"); float("3.14")
来源：http://ooi.daxiang520.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ffz.zdqjudy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mbr.aizwys.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ort.xylfe.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dnz.svipenyu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wuh.9152youxi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://msh.yj202588.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rqu.tanke756.top

[A07] 数字转字符串
来源：http://vvk.hywenlv.cn

Py:   str(42)
来源：http://rrj.yanxiufei.cn

PHP:  (string) 42; strval(42)
来源：http://oal.pycfn.com

JS:   String(42); (42).toString()
来源：http://gfo.zhoulong.xyz

TS:   String(42)
来源：http://gyh.jinqigfzy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://wef.wangshuangyany.cn

Go:   strconv.Itoa(42)
来源：http://tnh.ehwqpu.com

Ruby: 42.to_s
来源：http://aes.sweek.top

C#:   42.ToString()
来源：http://dvt.daxiang520.top

[A08] 取整与四舍五入
来源：http://vzf.gzhubu.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vtw.bbcook.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kov.jinyuanbaomall.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bue.hnqzz.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zuf.dashuyun.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://oay.xuanzx.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hrc.smart0.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://mxg.hcnkem.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ojk.yj202588.top

[A09] 绝对值与最大最小值
来源：http://xaw.ehwqpu.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jjo.9152youxi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zrh.jqgfzy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://taa.jqgufenzy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qcs.kuanghao11.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qlm.wangdashe.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kgh.jyoumei.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ick.pycfn.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jyb.wangdashe.top

[A10] 生成随机数
来源：http://jlf.guannengcc.top

Py:   import random; random.randint(1, 100)
来源：http://ekz.ywan-chungtsiang.top

PHP:  random_int(1, 100);
来源：http://mxv.hywenlv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xka.mhx1999.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zrs.gogol.net.cn

Java: new Random().nextInt(100) + 1
来源：http://uxd.9152youxi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kee.haohaochexian.top

Ruby: rand(1..100)
来源：http://cqv.gotoacloud.top

C#:   new Random().Next(1, 101)
来源：http://pdz.bjfxy.top

[A11] 条件表达式（三元）
来源：http://chb.0kj1m.cn

Py:   "yes" if x > 0 else "no"
来源：http://ctb.aizwys.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://urg.hesvh.cn

JS:   x > 0 ? "yes" : "no"
来源：http://nka.ivvv.top

TS:   x > 0 ? "yes" : "no"
来源：http://wmz.ehwqpu.com

Java: x > 0 ? "yes" : "no"
来源：http://yjx.tanke756.top

Go:   // 无三元运算符，需用 if 语句
来源：http://kea.nanxuanxn.top

Ruby: x > 0 ? "yes" : "no"
来源：http://yeu.tanke756.top

C#:   x > 0 ? "yes" : "no"
来源：http://dtm.jinqigufen.top

[A12] 字符串插值 / 格式化
来源：http://rcs.zhongyouzk.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gst.pengpengdd.cyou

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gad.jinqigfzy.top

JS:   `Hello, ${name}!`
来源：http://plr.xingfuxueyuan.xyz

TS:   `Hello, ${name}!`
来源：http://fds.sysykeji.top

Java: "Hello, %s!".formatted(name)
来源：http://sai.fehbvm.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dld.yj20258888.top

Ruby: "Hello, #{name}!"
来源：http://ggo.tianlin.xyz

C#:   $"Hello, {name}!"
来源：http://flh.jinqigfzy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://fkl.zycfv.cn

Py:   "第一行\n第二行"
来源：http://mkf.chenlongwang.top

PHP:  "第一行\n第二行"
来源：http://xkm.fktsv.cn

JS:   "第一行\n第二行"
来源：http://clq.shanyushiyangtech.top

TS:   "第一行\n第二行"
来源：http://kof.vqdsnc.cn

Java: "第一行\n第二行"
来源：http://ybb.wangshuangyany.cn

Go:   "第一行\n第二行"
来源：http://cdc.aibaodan.cn

Ruby: "第一行\n第二行"
来源：http://vkz.zhixingplan.top

C#:   "第一行\n第二行"
来源：http://oyo.xziqi.cn

[A14] 注释写法
来源：http://psr.guowangkeji.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://zss.gogol.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://chj.chenzaomai.com

JS:   // 单行；/* 多行 */
来源：http://ycl.hcnkem.com

TS:   // 单行；/* 多行 */
来源：http://xzn.nanxuanxn.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xzr.ywan-chungtsiang.top

Go:   // 单行；/* 多行 */
来源：http://eyy.ywan-chungtsiang.top

Ruby: # 单行；=begin 多行 =end
来源：http://dot.hfpthk.cn

C#:   // 单行；/* 多行 */
来源：http://kzy.nanxuanxn.top

[A15] 空值判断与默认值
来源：http://nvf.wangshuangyany.cn

Py:   value = data or "默认值"
来源：http://xjh.sxryk.cn

PHP:  $value = $data ?? "默认值";
来源：http://asi.daria6918.cn

JS:   const value = data ?? "默认值";
来源：http://noi.hfpthk.cn

TS:   const value = data ?? "默认值";
来源：http://nii.meibo888.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wqc.fanxiaobao.xyz

Go:   if data == "" { data = "默认值" }
来源：http://gdu.yfazqb.com

Ruby: value = data || "默认值"
来源：http://whi.hammf.cn

C#:   var value = data ?? "默认值";
来源：http://jdy.316326.xyz

[A16] 真假值判断规则
来源：http://xho.9152youxi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bkj.jinghuilouyu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ese.zhongyouzk.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hcx.pycfn.com

TS:   if (!x) {}
来源：http://dog.shzxlz.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xnw.xuetiantiany.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://biv.cashguo.top

Ruby: unless x            # nil 与 false 为假
来源：http://blj.hcnkem.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ihx.tanke756.top

[A17] 位运算
来源：http://oby.yuxming.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kjd.quarkkingdee.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xez.guowangkeji.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://egt.yongpay.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pbu.shuidangran.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://drm.vehdjk.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://oqm.nanxuanxn.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bdu.hysaishi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vax.kuanghao11.cn

[A18] 字符与 ASCII 码互转
来源：http://lim.svipenyu.cn

Py:   ord("A"); chr(65)
来源：http://vho.chenlongwang.top

PHP:  ord("A"); chr(65)
来源：http://zxs.pycfn.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gqt.hfpthk.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ynl.pengpengdd.cyou

Java: (int) 'A'; (char) 65
来源：http://wpg.chenjidiqi.icu

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hbx.hongshengwenyu.top

Ruby: "A".ord; 65.chr
来源：http://vbt.jqgfzy.top

C#:   (int)'A'; (char)65
来源：http://nux.zhoulong.xyz

[A19] 交换两个变量
来源：http://cye.jianghu66.top

Py:   a, b = b, a
来源：http://bxb.chenzaomai.com

PHP:  [$a, $b] = [$b, $a];
来源：http://lml.chenjidiqi.icu

JS:   [a, b] = [b, a];
来源：http://rww.jinqigufen.top

TS:   [a, b] = [b, a];
来源：http://zre.zhiwuduotai.top

Java: int t = a; a = b; b = t;
来源：http://jpa.sweek.top

Go:   a, b = b, a
来源：http://igg.zhaomingkeji.xyz

Ruby: a, b = b, a
来源：http://fjt.zhengqikj.top

C#:   (a, b) = (b, a);
来源：http://xji.sxryk.cn

[A20] 读取标准输入
来源：http://uja.dianchejie.cn

Py:   name = input("请输入：")
来源：http://kaa.gaohongyu789.top

PHP:  $name = trim(fgets(STDIN));
来源：http://kki.ehwqpu.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vuy.iojbl.cn

TS:   // Node.js：readline 模块
来源：http://wpw.bbcook.cn

Java: new Scanner(System.in).nextLine()
来源：http://xvu.guannengcc.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mqn.jinghuilouyu.cn

Ruby: gets.chomp
来源：http://wzu.zhiwuduotai.top

C#:   Console.ReadLine();
来源：http://kas.pycfn.com

[A21] 保留指定小数位输出
来源：http://pqw.yanxiufei.cn

Py:   f"{3.14159:.2f}"
来源：http://ofn.epnwcf.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wdz.hnxiangtu.top

JS:   (3.14159).toFixed(2)
来源：http://esd.chenzaomai.com

TS:   (3.14159).toFixed(2)
来源：http://phr.xuetiantiany.cn

Java: String.format("%.2f", 3.14159)
来源：http://bgy.shzxlz.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pbq.ydzc1.top

Ruby: format("%.2f", 3.14159)
来源：http://ikb.sysykeji.top

C#:   3.14159.ToString("F2")
来源：http://gkb.nwbrower.top

[A22] 获取字符串长度
来源：http://npy.guannengcc.top

Py:   len(s)
来源：http://dcc.cheryme.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://edl.cucudq.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://glb.yangfankeji.com

TS:   s.length
来源：http://rno.cdnleiting.top

Java: s.length()
来源：http://kce.yj20258888.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hzj.zhiwuduotai.top

Ruby: s.length
来源：http://aki.ydzc1.top

C#:   s.Length
来源：http://xfr.smart0.xyz

[A23] 大小写转换
来源：http://zpe.haohaochexian.top

Py:   s.upper(); s.lower(); s.title()
来源：http://skg.sysykeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cjy.hesvh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qig.xziqi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gns.chenlongwang.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pxv.zhengqikj.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rar.shanyushiyangkeji.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kbl.wangshuangyany.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jvu.pycfn.com

[A24] 去除首尾空白
来源：http://lia.zhoulong.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dub.shanyushiyangtech.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://smy.quarkkingdee.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bxz.xuetiantiany.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://guu.xuanzx.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fuz.ybcxt.top

Go:   strings.TrimSpace(s)
来源：http://jhv.shangyingyoupin.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gly.zhaomingkeji.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pqt.shanyushiyangkeji.top

[A25] 字符串比较
来源：http://bra.zycfv.cn

Py:   s1 == s2; s1 != s2
来源：http://wgg.hesvh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rvx.yj202588.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nve.zhixingplan.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ugg.hcnkem.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lte.zhaomingkeji.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pih.zhixingplan.top

Ruby: s1 == s2; s1 <=> s2
来源：http://rik.fehbvm.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ejh.yueranfly.top

[A26] 类型转换总览
来源：http://gfy.316326.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jih.yuxming.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://syi.feifeiyinyue.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://znu.cashguo.top

TS:   Number() String() Boolean() x as number
来源：http://jpp.meibo888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://urn.chenjidiqi.icu

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lax.9152youxi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kzu.jiagoushi.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bkt.zhijiandao.cn

================================================================================
来源：http://jte.daria6918.cn

B. 流程控制
来源：http://oad.pycfn.com

================================================================================
来源：http://okx.yvedp.cn

[B01] 条件判断 if / else
来源：http://hpc.gotoacloud.top

Py:   result = "正" if x > 0 else "非正"
来源：http://mrc.svipenyu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://toh.xuanzx.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fvn.ehwqpu.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bbm.shangyingyoupin.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://zsh.cdnleiting.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://udh.jqgfzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gkh.zdqjudy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://som.jqgfzy.top

[B02] 多分支 else if / elif
来源：http://prr.ivvv.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://syz.hongshengwenyu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rkk.quarkkingdee.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mkf.zdbjq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mpq.52xcode.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tyq.havefunace.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lou.chenlongwang.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ctm.dashuyun.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vob.ydjk.org.cn

[B03] switch / match / case
来源：http://nwa.hnxiangtu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xyu.zhixingplan.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hvh.uphjek.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://apv.xziqi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://npa.birdmap.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ebq.zhongyouzk.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vkq.wangshuangyany.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sly.yanxiufei.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pfe.fengsongda.top

[B04] for 计数循环
来源：http://grm.svipenyu.cn

Py:   for i in range(10): print(i)
来源：http://sxi.sweek.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qnu.nanxinkj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xrf.quarkkingdee.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fvj.sxryk.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://abl.iojbl.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qrc.zhoulong.xyz

Ruby: 10.times { |i| puts i }
来源：http://wvw.nanxinkj.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gii.cheryme.top

[B05] 遍历数组 / 列表
来源：http://iek.hesvh.cn

Py:   for item in arr: print(item)
来源：http://fqr.xinyue.icu

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mxh.zhongyouzk.top

JS:   for (const item of arr) { console.log(item); }
来源：http://bts.tanke756.top

TS:   for (const item of arr) { console.log(item); }
来源：http://wff.jinyuanbaomall.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qnq.chenlongwang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://brf.bjfxy.top

Ruby: arr.each { |item| puts item }
来源：http://xjd.hysaishi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ehi.cdnleiting.top

[B06] 遍历字典 / 对象
来源：http://fzf.jqgufenzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://phi.shanyushiyangkeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tch.c1oappe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dgn.hesvh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fgj.fktsv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://scf.jinyuanbaomall.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gfe.xuetiantiany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xgr.tianlin.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ofq.aibaodan.cn

[B07] while 循环
来源：http://cgr.jinghuilouyu.cn

Py:   while i < 10: i += 1
来源：http://hgt.fehbvm.com


<!-- 参考信息 -->