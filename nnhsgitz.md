代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://oqg.hongshengwenyu.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tuh.daxiang520.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dkl.meibo888.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jfl.nanxinkj.top

================================================================================
来源：http://toq.zhaomingkeji.xyz

A. 基础语法与类型
来源：http://gms.guannengcc.top

================================================================================
来源：http://iaz.kuanghao11.cn

[A01] Hello World
来源：http://vql.dianchejie.cn

Py:   print("Hello, World!")
来源：http://qsr.dianchejie.cn

PHP:  echo "Hello, World!";
来源：http://gpv.xingfuxueyuan.xyz

JS:   console.log("Hello, World!");
来源：http://fha.yonumen.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fmq.yj20258.top

Java: System.out.println("Hello, World!");
来源：http://qpw.birdmap.top

Go:   fmt.Println("Hello, World!")
来源：http://tse.fktsv.cn

Ruby: puts "Hello, World!"
来源：http://oas.nwbrower.top

C#:   Console.WriteLine("Hello, World!");
来源：http://qix.nwbrower.top

[A02] 变量声明与赋值
来源：http://xcm.meibo888.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ymp.dianchejie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://emb.cheryme.top

JS:   let name = "Alex"; const age = 20;
来源：http://jvf.hammf.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://aia.ppjwa.cn

Java: String name = "Alex"; int age = 20;
来源：http://dio.jqgufenzy.top

Go:   name := "Alex"; age := 20
来源：http://pvx.vehdjk.com

Ruby: name = "Alex"; age = 20
来源：http://uhn.mhx1999.top

C#:   string name = "Alex"; int age = 20;
来源：http://xty.yongpay.top

[A03] 常量定义
来源：http://cag.shuidangran.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ngd.svipenyu.cn

PHP:  const PI = 3.14159;
来源：http://nxc.yj20258888.top

JS:   const PI = 3.14159;
来源：http://trd.zhiwuduotai.top

TS:   const PI: number = 3.14159;
来源：http://cjo.gogol.net.cn

Java: static final double PI = 3.14159;
来源：http://qkr.jinghuilouyu.cn

Go:   const PI = 3.14159
来源：http://ndu.fanxiaobao.xyz

Ruby: PI = 3.14159
来源：http://iop.shanyushiyangkeji.top

C#:   const double PI = 3.14159;
来源：http://jeb.bbcook.cn

[A04] 判断变量类型
来源：http://hby.jiagoushi.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://now.fengsongda.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://azj.hammf.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fxs.hongshengwenyu.top

TS:   typeof x; x instanceof Date
来源：http://ryv.52xcode.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://uut.ydzc1.top

Go:   reflect.TypeOf(x).Name()
来源：http://mli.yuanzhike.top

Ruby: x.class; x.is_a?(Integer)
来源：http://bpv.vehdjk.com

C#:   x.GetType().Name; x is int
来源：http://hjk.redwolf501.top

[A05] 整数除法与取模
来源：http://oga.hywenlv.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wlc.daxiang520.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://bmb.jianghu66.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kig.yfazqb.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://acc.chenzaomai.com

Java: 7 / 2; 7 % 2
来源：http://yiu.tian-w.cn

Go:   7 / 2; 7 % 2
来源：http://eiv.bbcook.cn

Ruby: 7 / 2; 7 % 2
来源：http://bpd.ehwqpu.com

C#:   7 / 2; 7 % 2
来源：http://nnq.chenlongwang.top

[A06] 字符串转数字
来源：http://uch.feifeiyinyue.top

Py:   int("42"); float("3.14")
来源：http://gle.yanxiufei.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hkf.mhx1999.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lne.snrcjt.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ojo.shangyingyoupin.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://grs.yj20258888.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vua.zdbjq.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hil.yanxiufei.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://elk.bbcook.cn

[A07] 数字转字符串
来源：http://uvv.zdbjq.cn

Py:   str(42)
来源：http://eva.zhijiandao.cn

PHP:  (string) 42; strval(42)
来源：http://khs.haohaochexian.top

JS:   String(42); (42).toString()
来源：http://bej.cashguo.top

TS:   String(42)
来源：http://yfq.jinqigfzy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://jnk.ivvv.top

Go:   strconv.Itoa(42)
来源：http://erv.fehbvm.com

Ruby: 42.to_s
来源：http://abl.zhijiandao.cn

C#:   42.ToString()
来源：http://puh.9152youxi.cn

[A08] 取整与四舍五入
来源：http://tbz.vqdsnc.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kfm.iojbl.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://aft.ywan-chungtsiang.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zba.sxryk.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rof.0kj1m.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xlk.ybcxt.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vik.zhoulong.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://pwz.ybcxt.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vnn.iojbl.cn

[A09] 绝对值与最大最小值
来源：http://ndb.mhx1999.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ohd.yuxming.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nmc.jqgfzy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ybj.vqdsnc.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gsh.zhoulong.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mgg.pycfn.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lrv.cdnleiting.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qnb.yangfankeji.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kpg.fktsv.cn

[A10] 生成随机数
来源：http://ezt.bjfxy.top

Py:   import random; random.randint(1, 100)
来源：http://bgk.chenlongwang.top

PHP:  random_int(1, 100);
来源：http://deb.nanxinkj.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zcd.vqdsnc.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jdj.aizwys.cn

Java: new Random().nextInt(100) + 1
来源：http://pbu.dianchejie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://oku.gzhubu.top

Ruby: rand(1..100)
来源：http://qcs.cashguo.top

C#:   new Random().Next(1, 101)
来源：http://ugn.wangshuangyany.cn

[A11] 条件表达式（三元）
来源：http://tlh.smart0.xyz

Py:   "yes" if x > 0 else "no"
来源：http://kfa.nanxuanxn.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ovl.zhaomingkeji.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://ctz.ydzc1.top

TS:   x > 0 ? "yes" : "no"
来源：http://tux.fktsv.cn

Java: x > 0 ? "yes" : "no"
来源：http://oxg.fktsv.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fmr.vqdsnc.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://koq.birdmap.top

C#:   x > 0 ? "yes" : "no"
来源：http://pxf.zhijiandao.cn

[A12] 字符串插值 / 格式化
来源：http://agk.zhengqikj.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://suv.hammf.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jqh.tarul.cn

JS:   `Hello, ${name}!`
来源：http://uwj.9152youxi.cn

TS:   `Hello, ${name}!`
来源：http://tqc.yfazqb.com

Java: "Hello, %s!".formatted(name)
来源：http://gzn.c1oappe.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rgi.pycfn.com

Ruby: "Hello, #{name}!"
来源：http://vik.andypj.xyz

C#:   $"Hello, {name}!"
来源：http://uaw.guowangkeji.top

[A13] 多行字符串（练习 \n 转义）
来源：http://hha.xylfe.cn

Py:   "第一行\n第二行"
来源：http://era.hnxiangtu.top

PHP:  "第一行\n第二行"
来源：http://dxw.ydjk.org.cn

JS:   "第一行\n第二行"
来源：http://bku.hongshengwenyu.top

TS:   "第一行\n第二行"
来源：http://kms.ydjk.org.cn

Java: "第一行\n第二行"
来源：http://jpq.ydjk.org.cn

Go:   "第一行\n第二行"
来源：http://hjr.yonumen.top

Ruby: "第一行\n第二行"
来源：http://jkt.cqqwz.cn

C#:   "第一行\n第二行"
来源：http://sni.pycfn.com

[A14] 注释写法
来源：http://tiu.jqgfzy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://cmn.yueranfly.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://gym.hammf.cn

JS:   // 单行；/* 多行 */
来源：http://ijg.chenjidiqi.icu

TS:   // 单行；/* 多行 */
来源：http://ift.hongshengwenyu.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ply.fanxiaobao.xyz

Go:   // 单行；/* 多行 */
来源：http://pex.zhengqikj.top

Ruby: # 单行；=begin 多行 =end
来源：http://ddk.cdnleiting.top

C#:   // 单行；/* 多行 */
来源：http://gpe.cashguo.top

[A15] 空值判断与默认值
来源：http://tyf.aizwys.cn

Py:   value = data or "默认值"
来源：http://jvp.quarkkingdee.top

PHP:  $value = $data ?? "默认值";
来源：http://tui.jinqigufen.top

JS:   const value = data ?? "默认值";
来源：http://ydf.cashguo.top

TS:   const value = data ?? "默认值";
来源：http://hlx.uphjek.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mfk.gotoacloud.top

Go:   if data == "" { data = "默认值" }
来源：http://gho.nanxuanxn.top

Ruby: value = data || "默认值"
来源：http://vlg.tanke756.top

C#:   var value = data ?? "默认值";
来源：http://hrn.ydzc1.top

[A16] 真假值判断规则
来源：http://sbp.yangfankeji.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://djl.zdqjudy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nww.vehdjk.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zyh.mhx1999.top

TS:   if (!x) {}
来源：http://syf.yueranfly.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pka.sxryk.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nqk.aizwys.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kvg.zhixingplan.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ztc.xingfuxueyuan.xyz

[A17] 位运算
来源：http://jjf.zhixingplan.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dmt.zhijiandao.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xww.snrcjt.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kjv.yuxming.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://muc.9152youxi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yyh.0kj1m.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jzn.jinyuanbaomall.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uxq.smart0.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hde.nwbrower.top

[A18] 字符与 ASCII 码互转
来源：http://ast.jinghuilouyu.cn

Py:   ord("A"); chr(65)
来源：http://phf.havefunace.top

PHP:  ord("A"); chr(65)
来源：http://xoo.yongpay.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lrw.9152youxi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lcp.zycfv.cn

Java: (int) 'A'; (char) 65
来源：http://kba.tanke756.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vag.yfazqb.com

Ruby: "A".ord; 65.chr
来源：http://zyr.pengpengdd.cyou

C#:   (int)'A'; (char)65
来源：http://lix.kuanghao11.cn

[A19] 交换两个变量
来源：http://yqm.cashguo.top

Py:   a, b = b, a
来源：http://eza.hongshengwenyu.top

PHP:  [$a, $b] = [$b, $a];
来源：http://zny.guowangkeji.top

JS:   [a, b] = [b, a];
来源：http://bge.xuetiantiany.cn

TS:   [a, b] = [b, a];
来源：http://afb.zhixingplan.top

Java: int t = a; a = b; b = t;
来源：http://peq.haohaochexian.top

Go:   a, b = b, a
来源：http://kow.ppjwa.cn

Ruby: a, b = b, a
来源：http://nha.52xcode.cn

C#:   (a, b) = (b, a);
来源：http://rxz.nwbrower.top

[A20] 读取标准输入
来源：http://gpm.jqgufenzy.top

Py:   name = input("请输入：")
来源：http://xiw.zdbjq.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pai.tarul.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rxe.jlsjyb.cn

TS:   // Node.js：readline 模块
来源：http://edp.dianchejie.cn

Java: new Scanner(System.in).nextLine()
来源：http://mga.bbcook.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://naa.xinyue.icu

Ruby: gets.chomp
来源：http://xom.shangyingyoupin.top

C#:   Console.ReadLine();
来源：http://tgo.9152youxi.cn

[A21] 保留指定小数位输出
来源：http://wgj.0kj1m.cn

Py:   f"{3.14159:.2f}"
来源：http://dvk.shzxlz.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hnb.jinqigfzy.top

JS:   (3.14159).toFixed(2)
来源：http://xiw.fanxiaobao.xyz

TS:   (3.14159).toFixed(2)
来源：http://yzg.xuetiantiany.cn

Java: String.format("%.2f", 3.14159)
来源：http://rsr.epnwcf.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hsk.guowangkeji.top

Ruby: format("%.2f", 3.14159)
来源：http://ydw.sufxvd.cn

C#:   3.14159.ToString("F2")
来源：http://ffr.fanxiaobao.xyz

[A22] 获取字符串长度
来源：http://uwx.nanxinkj.top

Py:   len(s)
来源：http://drg.jinyuanbaomall.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://btj.fehbvm.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ank.meibo888.top

TS:   s.length
来源：http://acf.bjfxy.top

Java: s.length()
来源：http://xbf.fengsongda.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kvz.vqdsnc.cn

Ruby: s.length
来源：http://zcp.shzxlz.cn

C#:   s.Length
来源：http://eix.shanyushiyangkeji.top

[A23] 大小写转换
来源：http://ykp.jinyuanbaomall.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://eyh.chenzaomai.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jqd.quarkkingdee.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tkb.yueranfly.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uke.zhiwuduotai.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lgu.ydzc1.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ijj.xuanzx.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ada.redwolf501.top

C#:   s.ToUpper(); s.ToLower()
来源：http://mdn.mhx1999.top

[A24] 去除首尾空白
来源：http://hfw.cheryme.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cco.daxiang520.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rww.ydjk.org.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ppt.yanxiufei.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yxl.xinyue.icu

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ifp.fanxiaobao.xyz

Go:   strings.TrimSpace(s)
来源：http://toj.xuetiantiany.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jsc.wangshuangyany.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ctf.sysykeji.top

[A25] 字符串比较
来源：http://qcd.cqqwz.cn

Py:   s1 == s2; s1 != s2
来源：http://okn.ivvv.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://prg.cashguo.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gdk.ivvv.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wtd.redwolf501.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://utp.meibo888.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kha.nanxinkj.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ahk.jinghuilouyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lsg.ydzc1.top

[A26] 类型转换总览
来源：http://hji.redwolf501.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ban.zhaomingkeji.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zwl.tanke756.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bym.aibaodan.cn

TS:   Number() String() Boolean() x as number
来源：http://pnd.yuxming.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ell.zhijiandao.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vob.ybcxt.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://kql.cqqwz.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pjn.yanxiufei.cn

================================================================================
来源：http://ujc.xylfe.cn

B. 流程控制
来源：http://uug.sxryk.cn

================================================================================
来源：http://jfo.fzhhl.top

[B01] 条件判断 if / else
来源：http://jzm.chenjidiqi.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://ibq.zhongyouzk.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jay.feifeiyinyue.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://aip.yj20258.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mlo.gzhubu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ddh.fzhhl.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rac.xingfuxueyuan.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://aod.ivvv.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vnh.fengsongda.top

[B02] 多分支 else if / elif
来源：http://hzk.zhongyouzk.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ojd.epnwcf.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bbk.9152youxi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nne.hywenlv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nyx.tianlin.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vxf.dianchejie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lfw.cashguo.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wag.tianlin.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ahh.jinqigufen.top

[B03] switch / match / case
来源：http://vkf.shanyushiyangtech.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ygc.zhiwuduotai.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uew.0kj1m.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dir.chenlongwang.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zhl.yanxiufei.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xep.gotoacloud.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://itv.hfpthk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://suj.9152youxi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zab.xziqi.cn

[B04] for 计数循环
来源：http://fik.hammf.cn

Py:   for i in range(10): print(i)
来源：http://isn.9152youxi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qcq.yongpay.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://osh.haohaochexian.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xbp.ybcxt.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tsb.52xcode.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ltu.zhixingplan.top

Ruby: 10.times { |i| puts i }
来源：http://sbq.snrcjt.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lpa.hnxiangtu.top

[B05] 遍历数组 / 列表
来源：http://fbj.pengpengdd.cyou

Py:   for item in arr: print(item)
来源：http://mre.zdqjudy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ykv.feifeiyinyue.top

JS:   for (const item of arr) { console.log(item); }
来源：http://nej.guannengcc.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ewk.dianchejie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://exi.hywenlv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qmq.tarul.cn

Ruby: arr.each { |item| puts item }
来源：http://vua.quarkkingdee.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eez.andypj.xyz

[B06] 遍历字典 / 对象
来源：http://nyo.birdmap.top

Py:   for k, v in d.items(): print(k, v)
来源：http://nok.yonumen.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jdd.gzhubu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://khu.daria6918.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pft.jiagoushi.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ppv.zhoulong.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oas.ydzc1.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bwi.ehwqpu.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cbr.zhaomingkeji.xyz

[B07] while 循环
来源：http://naq.chenlongwang.top

Py:   while i < 10: i += 1
来源：http://bet.guannengcc.top


<!-- 参考信息 -->