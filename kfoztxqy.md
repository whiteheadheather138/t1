代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://kjw.xingfuxueyuan.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tet.zhoulong.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xng.smart0.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://unu.dianchejie.cn

================================================================================
来源：http://hqz.52xcode.cn

A. 基础语法与类型
来源：http://guk.yonumen.top

================================================================================
来源：http://dho.ivvv.top

[A01] Hello World
来源：http://xak.feifeiyinyue.top

Py:   print("Hello, World!")
来源：http://jlg.yonumen.top

PHP:  echo "Hello, World!";
来源：http://nyg.guannengcc.top

JS:   console.log("Hello, World!");
来源：http://zsc.yj20258.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hqh.yfazqb.com

Java: System.out.println("Hello, World!");
来源：http://dnv.quarkkingdee.top

Go:   fmt.Println("Hello, World!")
来源：http://ubq.mhx1999.top

Ruby: puts "Hello, World!"
来源：http://mpc.jqgufenzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://qvv.gogol.net.cn

[A02] 变量声明与赋值
来源：http://qtr.svipenyu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bny.haohaochexian.top

PHP:  $name = "Alex"; $age = 20;
来源：http://qix.yvedp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gpx.316326.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vmd.vqdsnc.cn

Java: String name = "Alex"; int age = 20;
来源：http://suq.quarkkingdee.top

Go:   name := "Alex"; age := 20
来源：http://txb.cucudq.cn

Ruby: name = "Alex"; age = 20
来源：http://blm.daria6918.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dfy.vehdjk.com

[A03] 常量定义
来源：http://rxu.aizwys.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sxj.jinghuilouyu.cn

PHP:  const PI = 3.14159;
来源：http://pef.yonumen.top

JS:   const PI = 3.14159;
来源：http://mns.yfazqb.com

TS:   const PI: number = 3.14159;
来源：http://nbv.birdmap.top

Java: static final double PI = 3.14159;
来源：http://cbf.fehbvm.com

Go:   const PI = 3.14159
来源：http://lps.tian-w.cn

Ruby: PI = 3.14159
来源：http://hhl.xinyue.icu

C#:   const double PI = 3.14159;
来源：http://smb.ydzc1.top

[A04] 判断变量类型
来源：http://yhy.jiagoushi.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://bnj.ybcxt.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://anf.tarul.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lal.ydzc1.top

TS:   typeof x; x instanceof Date
来源：http://kkq.ctjpmb.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yaw.daria6918.cn

Go:   reflect.TypeOf(x).Name()
来源：http://mbk.yfazqb.com

Ruby: x.class; x.is_a?(Integer)
来源：http://dxn.redwolf501.top

C#:   x.GetType().Name; x is int
来源：http://pvr.yangfankeji.com

[A05] 整数除法与取模
来源：http://rws.sysykeji.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rjw.xinyue.icu

PHP:  intdiv(7, 2); 7 % 2
来源：http://cux.jlsjyb.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://usf.fengsongda.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://him.yonumen.top

Java: 7 / 2; 7 % 2
来源：http://jzz.nwbrower.top

Go:   7 / 2; 7 % 2
来源：http://bbr.shuidangran.top

Ruby: 7 / 2; 7 % 2
来源：http://rip.fehbvm.com

C#:   7 / 2; 7 % 2
来源：http://oca.jinghuilouyu.cn

[A06] 字符串转数字
来源：http://cof.zhiwuduotai.top

Py:   int("42"); float("3.14")
来源：http://pam.tianlin.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hsl.fzhhl.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ase.fehbvm.com

TS:   parseInt("42", 10); Number("42")
来源：http://txh.gotoacloud.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nch.shanyushiyangkeji.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mdl.fanxiaobao.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://aig.yj20258888.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qpj.ctjpmb.com

[A07] 数字转字符串
来源：http://khf.yfazqb.com

Py:   str(42)
来源：http://rao.cucudq.cn

PHP:  (string) 42; strval(42)
来源：http://zqe.gogol.net.cn

JS:   String(42); (42).toString()
来源：http://eid.cdnleiting.top

TS:   String(42)
来源：http://wcr.yfazqb.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://ztg.xziqi.cn

Go:   strconv.Itoa(42)
来源：http://nig.cqqwz.cn

Ruby: 42.to_s
来源：http://guv.yj202588.top

C#:   42.ToString()
来源：http://nef.chenjidiqi.icu

[A08] 取整与四舍五入
来源：http://mqf.jiagoushi.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uro.hesvh.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ujr.jinqigfzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mwx.yonumen.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://elq.wangdashe.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ncd.mhx1999.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jcc.shzxlz.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://bau.haohaochexian.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qcc.ppjwa.cn

[A09] 绝对值与最大最小值
来源：http://gpl.jinqigufen.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nhe.tianlin.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wch.cashguo.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qft.fktsv.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://aly.zhongyouzk.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uax.andypj.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xyz.gzhubu.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bev.sjlbkw.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hig.haohaochexian.top

[A10] 生成随机数
来源：http://ssf.birdmap.top

Py:   import random; random.randint(1, 100)
来源：http://bmp.snrcjt.cn

PHP:  random_int(1, 100);
来源：http://jea.dashuyun.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mff.quarkkingdee.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gvd.316326.xyz

Java: new Random().nextInt(100) + 1
来源：http://cvm.shanyushiyangkeji.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dqo.zhijiandao.cn

Ruby: rand(1..100)
来源：http://hfs.shanyushiyangtech.top

C#:   new Random().Next(1, 101)
来源：http://vss.zhixingplan.top

[A11] 条件表达式（三元）
来源：http://stf.fehbvm.com

Py:   "yes" if x > 0 else "no"
来源：http://heu.chenjidiqi.icu

PHP:  $x > 0 ? "yes" : "no"
来源：http://jsa.dianchejie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rjk.havefunace.top

TS:   x > 0 ? "yes" : "no"
来源：http://wda.xinyue.icu

Java: x > 0 ? "yes" : "no"
来源：http://ihq.ppjwa.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mck.zhixingplan.top

Ruby: x > 0 ? "yes" : "no"
来源：http://bea.sxryk.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vqt.tanke756.top

[A12] 字符串插值 / 格式化
来源：http://evo.sweek.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vzo.tarul.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://erq.jinqigfzy.top

JS:   `Hello, ${name}!`
来源：http://eul.yvedp.cn

TS:   `Hello, ${name}!`
来源：http://nxy.guannengcc.top

Java: "Hello, %s!".formatted(name)
来源：http://dmq.zhengqikj.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wyt.tarul.cn

Ruby: "Hello, #{name}!"
来源：http://rmc.zdbjq.cn

C#:   $"Hello, {name}!"
来源：http://fcc.svipenyu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pah.gotoacloud.top

Py:   "第一行\n第二行"
来源：http://xno.aibaodan.cn

PHP:  "第一行\n第二行"
来源：http://xvb.fehbvm.com

JS:   "第一行\n第二行"
来源：http://ewq.hammf.cn

TS:   "第一行\n第二行"
来源：http://nkv.zhixingplan.top

Java: "第一行\n第二行"
来源：http://rni.hywenlv.cn

Go:   "第一行\n第二行"
来源：http://vcb.shuidangran.top

Ruby: "第一行\n第二行"
来源：http://yit.hywenlv.cn

C#:   "第一行\n第二行"
来源：http://qco.chenlongwang.top

[A14] 注释写法
来源：http://avo.jiagoushi.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://sqr.jlsjyb.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://duq.hesvh.cn

JS:   // 单行；/* 多行 */
来源：http://tao.yj20258888.top

TS:   // 单行；/* 多行 */
来源：http://pbj.jinqigfzy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://txh.cucudq.cn

Go:   // 单行；/* 多行 */
来源：http://hfp.hywenlv.cn

Ruby: # 单行；=begin 多行 =end
来源：http://sgz.sufxvd.cn

C#:   // 单行；/* 多行 */
来源：http://sfv.9152youxi.cn

[A15] 空值判断与默认值
来源：http://akd.fengsongda.top

Py:   value = data or "默认值"
来源：http://eeh.yvedp.cn

PHP:  $value = $data ?? "默认值";
来源：http://nrb.ydjk.org.cn

JS:   const value = data ?? "默认值";
来源：http://alp.cucudq.cn

TS:   const value = data ?? "默认值";
来源：http://csi.c1oappe.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gbz.zdbjq.cn

Go:   if data == "" { data = "默认值" }
来源：http://ogu.jianghu66.top

Ruby: value = data || "默认值"
来源：http://mqj.gotoacloud.top

C#:   var value = data ?? "默认值";
来源：http://arj.tian-w.cn

[A16] 真假值判断规则
来源：http://pho.gaohongyu789.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zro.yonumen.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gzs.zhixingplan.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ztx.xuetiantiany.cn

TS:   if (!x) {}
来源：http://gym.vehdjk.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jwc.wangdashe.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wil.zhaomingkeji.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://ild.bjfxy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://oqg.yuxming.cn

[A17] 位运算
来源：http://krl.ctjpmb.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yzr.sysykeji.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jut.zhongyouzk.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hxq.yueranfly.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dlm.316326.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ckf.ybcxt.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gvh.52xcode.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://avn.ybcxt.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tsz.xingfuxueyuan.xyz

[A18] 字符与 ASCII 码互转
来源：http://szw.jianghu66.top

Py:   ord("A"); chr(65)
来源：http://tae.pengpengdd.cyou

PHP:  ord("A"); chr(65)
来源：http://ifp.shangyingyoupin.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uyv.c1oappe.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xur.guannengcc.top

Java: (int) 'A'; (char) 65
来源：http://jyp.jqgufenzy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vff.smart0.xyz

Ruby: "A".ord; 65.chr
来源：http://xkz.fanxiaobao.xyz

C#:   (int)'A'; (char)65
来源：http://rwj.shangyingyoupin.top

[A19] 交换两个变量
来源：http://asj.gzhubu.top

Py:   a, b = b, a
来源：http://wxc.daxiang520.top

PHP:  [$a, $b] = [$b, $a];
来源：http://dmz.ctjpmb.com

JS:   [a, b] = [b, a];
来源：http://tca.ivvv.top

TS:   [a, b] = [b, a];
来源：http://osa.gaohongyu789.top

Java: int t = a; a = b; b = t;
来源：http://lzc.shanyushiyangkeji.top

Go:   a, b = b, a
来源：http://lae.sjlbkw.cn

Ruby: a, b = b, a
来源：http://pdu.shanyushiyangkeji.top

C#:   (a, b) = (b, a);
来源：http://och.hfpthk.cn

[A20] 读取标准输入
来源：http://dos.fehbvm.com

Py:   name = input("请输入：")
来源：http://sdh.jlsjyb.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gsg.bbcook.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hnt.cucudq.cn

TS:   // Node.js：readline 模块
来源：http://phm.andypj.xyz

Java: new Scanner(System.in).nextLine()
来源：http://feo.xingfuxueyuan.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://asy.hnxiangtu.top

Ruby: gets.chomp
来源：http://uoj.sweek.top

C#:   Console.ReadLine();
来源：http://hci.ydzc1.top

[A21] 保留指定小数位输出
来源：http://rmr.chenlongwang.top

Py:   f"{3.14159:.2f}"
来源：http://fij.yueranfly.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dgx.gotoacloud.top

JS:   (3.14159).toFixed(2)
来源：http://vgq.hesvh.cn

TS:   (3.14159).toFixed(2)
来源：http://hwd.nanxinkj.top

Java: String.format("%.2f", 3.14159)
来源：http://sek.xylfe.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ddp.havefunace.top

Ruby: format("%.2f", 3.14159)
来源：http://qyf.zhengqikj.top

C#:   3.14159.ToString("F2")
来源：http://vhh.pengpengdd.cyou

[A22] 获取字符串长度
来源：http://sdt.gaohongyu789.top

Py:   len(s)
来源：http://bte.guannengcc.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gkz.fanxiaobao.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rvx.ydzc1.top

TS:   s.length
来源：http://nql.shanyushiyangkeji.top

Java: s.length()
来源：http://znr.kuanghao11.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ndb.dianchejie.cn

Ruby: s.length
来源：http://sjp.yonumen.top

C#:   s.Length
来源：http://bqu.9152youxi.cn

[A23] 大小写转换
来源：http://bsb.cdnleiting.top

Py:   s.upper(); s.lower(); s.title()
来源：http://hql.nwbrower.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mek.chenlongwang.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cif.yj20258888.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xzx.ywan-chungtsiang.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ada.smart0.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yxd.ctjpmb.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lnl.hongshengwenyu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://zmr.sweek.top

[A24] 去除首尾空白
来源：http://zwr.tian-w.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bix.andypj.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mwz.shanyushiyangtech.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xbf.zhaomingkeji.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gfi.ywan-chungtsiang.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://miz.xinyue.icu

Go:   strings.TrimSpace(s)
来源：http://sbm.jyoumei.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://emc.fktsv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://uuo.yj20258.top

[A25] 字符串比较
来源：http://ajg.zhoulong.xyz

Py:   s1 == s2; s1 != s2
来源：http://ipy.tanke756.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kon.zdbjq.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mby.dashuyun.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bht.havefunace.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://shi.dashuyun.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dsh.xuetiantiany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pfl.wangshuangyany.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qes.yj202588.top

[A26] 类型转换总览
来源：http://eda.yvedp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ebr.smart0.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ydk.fzhhl.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xmq.bbcook.cn

TS:   Number() String() Boolean() x as number
来源：http://dzf.hfpthk.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://etu.wangshuangyany.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://byl.xuetiantiany.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qrt.shuidangran.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xsx.yanxiufei.cn

================================================================================
来源：http://xgs.yfazqb.com

B. 流程控制
来源：http://qfc.mhx1999.top

================================================================================
来源：http://fjd.uphjek.com

[B01] 条件判断 if / else
来源：http://qrf.yanxiufei.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cai.bjfxy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://duv.wangdashe.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pqw.redwolf501.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xat.sxryk.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rhu.epnwcf.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jwf.yuanzhike.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://diu.xingfuxueyuan.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vge.tian-w.cn

[B02] 多分支 else if / elif
来源：http://hbu.guannengcc.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jtl.gaohongyu789.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rfd.fzhhl.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wez.zhengqikj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fyl.chenjidiqi.icu

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vtc.tanke756.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://guv.0kj1m.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wzd.shuidangran.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vjh.jinghuilouyu.cn

[B03] switch / match / case
来源：http://mnp.nanxinkj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rao.sxryk.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cmd.bbcook.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dds.chenzaomai.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bpk.epnwcf.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jsl.fengsongda.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yyu.shanyushiyangtech.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dpv.chenlongwang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://foz.epnwcf.com

[B04] for 计数循环
来源：http://ytr.cucudq.cn

Py:   for i in range(10): print(i)
来源：http://qth.ydjk.org.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sxm.jyoumei.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dlo.fengsongda.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://azi.hesvh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fec.zhaomingkeji.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tji.shanyushiyangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://pvv.cashguo.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nqs.yangfankeji.com

[B05] 遍历数组 / 列表
来源：http://fkk.vqdsnc.cn

Py:   for item in arr: print(item)
来源：http://bhz.cdnleiting.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://czm.mhx1999.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ojd.yonumen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://yjm.jqgufenzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://nem.aibaodan.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jrb.svipenyu.cn

Ruby: arr.each { |item| puts item }
来源：http://oux.hammf.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mhx.sysykeji.top

[B06] 遍历字典 / 对象
来源：http://vri.9152youxi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wbc.xinyue.icu

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qgh.gogol.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vff.zhixingplan.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jzc.feifeiyinyue.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lxg.yj20258888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nps.ehwqpu.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://adg.ydjk.org.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jxv.xuetiantiany.cn

[B07] while 循环
来源：http://wdw.kuanghao11.cn

Py:   while i < 10: i += 1
来源：http://tmo.birdmap.top


<!-- 参考信息 -->