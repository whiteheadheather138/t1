代发 wailian999

================================================================================
来源：http://shv.guannengcc.top

A. 基础语法与类型
来源：http://uch.fktsv.cn

================================================================================
来源：http://uqr.dianchejie.cn

[A01] Hello World
来源：http://sbd.0kj1m.cn

Py:   print("Hello, World!")
来源：http://gqm.sysykeji.top

PHP:  echo "Hello, World!";
来源：http://yxg.tanke756.top

JS:   console.log("Hello, World!");
来源：http://wpw.kuanghao11.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bzi.daxiang520.top

Java: System.out.println("Hello, World!");
来源：http://kxk.jqgufenzy.top

Go:   fmt.Println("Hello, World!")
来源：http://lsq.vqdsnc.cn

Ruby: puts "Hello, World!"
来源：http://tih.shanyushiyangtech.top

C#:   Console.WriteLine("Hello, World!");
来源：http://vbw.zhiwuduotai.top

[A02] 变量声明与赋值
来源：http://jvw.redwolf501.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://iyn.cdnleiting.top

PHP:  $name = "Alex"; $age = 20;
来源：http://zbp.yj20258888.top

JS:   let name = "Alex"; const age = 20;
来源：http://imn.tanke756.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gio.sjlbkw.cn

Java: String name = "Alex"; int age = 20;
来源：http://jkh.havefunace.top

Go:   name := "Alex"; age := 20
来源：http://iyp.zhoulong.xyz

Ruby: name = "Alex"; age = 20
来源：http://pzf.smart0.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://tir.fengsongda.top

[A03] 常量定义
来源：http://etd.feifeiyinyue.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cms.birdmap.top

PHP:  const PI = 3.14159;
来源：http://qrp.zhaomingkeji.xyz

JS:   const PI = 3.14159;
来源：http://crk.jlsjyb.cn

TS:   const PI: number = 3.14159;
来源：http://tjy.zdqjudy.top

Java: static final double PI = 3.14159;
来源：http://uqk.shangyingyoupin.top

Go:   const PI = 3.14159
来源：http://pni.bjfxy.top

Ruby: PI = 3.14159
来源：http://iry.gotoacloud.top

C#:   const double PI = 3.14159;
来源：http://xgt.yvedp.cn

[A04] 判断变量类型
来源：http://kww.shangyingyoupin.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://jpk.tarul.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vke.xinyue.icu

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://apn.birdmap.top

TS:   typeof x; x instanceof Date
来源：http://zcv.nanxuanxn.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://psq.dianchejie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://oau.xylfe.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lfi.wangdashe.top

C#:   x.GetType().Name; x is int
来源：http://gmi.smart0.xyz

[A05] 整数除法与取模
来源：http://ppg.cdnleiting.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fui.yvedp.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://foh.hywenlv.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nnz.gzhubu.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lau.dianchejie.cn

Java: 7 / 2; 7 % 2
来源：http://lqh.mhx1999.top

Go:   7 / 2; 7 % 2
来源：http://ucy.ydzc1.top

Ruby: 7 / 2; 7 % 2
来源：http://yto.hcnkem.com

C#:   7 / 2; 7 % 2
来源：http://ulo.fanxiaobao.xyz

[A06] 字符串转数字
来源：http://qkc.cqqwz.cn

Py:   int("42"); float("3.14")
来源：http://jid.hywenlv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dua.316326.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ohh.hysaishi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://mfc.epnwcf.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cjp.ppjwa.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hwf.kuanghao11.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://srs.chenjidiqi.icu

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nwn.yj202588.top

[A07] 数字转字符串
来源：http://zhl.jyoumei.cn

Py:   str(42)
来源：http://ecb.haohaochexian.top

PHP:  (string) 42; strval(42)
来源：http://bnk.yuxming.cn

JS:   String(42); (42).toString()
来源：http://wqk.cashguo.top

TS:   String(42)
来源：http://ubg.dianchejie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://mgb.cdnleiting.top

Go:   strconv.Itoa(42)
来源：http://lgo.shuidangran.top

Ruby: 42.to_s
来源：http://ruf.daxiang520.top

C#:   42.ToString()
来源：http://nte.pycfn.com

[A08] 取整与四舍五入
来源：http://jud.shanyushiyangtech.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qwx.jinqigufen.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kln.jinqigufen.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://maj.hcnkem.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nxo.gogol.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sdp.uphjek.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dmt.sxryk.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wnc.nwbrower.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ttt.hnqzz.top

[A09] 绝对值与最大最小值
来源：http://eqm.fanxiaobao.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dgp.vehdjk.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://njp.shanyushiyangtech.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xck.zhoulong.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://itq.ehwqpu.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nau.sysykeji.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fpw.wangdashe.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bog.sysykeji.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://riz.fktsv.cn

[A10] 生成随机数
来源：http://law.zhaomingkeji.xyz

Py:   import random; random.randint(1, 100)
来源：http://nad.tianlin.xyz

PHP:  random_int(1, 100);
来源：http://ujr.aizwys.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://omm.cucudq.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yqq.tarul.cn

Java: new Random().nextInt(100) + 1
来源：http://fip.yongpay.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://uoo.xuetiantiany.cn

Ruby: rand(1..100)
来源：http://gik.hfpthk.cn

C#:   new Random().Next(1, 101)
来源：http://syq.yuxming.cn

[A11] 条件表达式（三元）
来源：http://kyn.cdnleiting.top

Py:   "yes" if x > 0 else "no"
来源：http://zwq.yanxiufei.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://srd.wangdashe.top

JS:   x > 0 ? "yes" : "no"
来源：http://jcd.tian-w.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ztv.52xcode.cn

Java: x > 0 ? "yes" : "no"
来源：http://aka.hcnkem.com

Go:   // 无三元运算符，需用 if 语句
来源：http://vtl.tarul.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://stz.ctjpmb.com

C#:   x > 0 ? "yes" : "no"
来源：http://bam.feifeiyinyue.top

[A12] 字符串插值 / 格式化
来源：http://rkn.tarul.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zou.jinqigfzy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://txd.jinqigufen.top

JS:   `Hello, ${name}!`
来源：http://qur.sweek.top

TS:   `Hello, ${name}!`
来源：http://ahr.feifeiyinyue.top

Java: "Hello, %s!".formatted(name)
来源：http://giv.cheryme.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wky.zycfv.cn

Ruby: "Hello, #{name}!"
来源：http://gpb.jianghu66.top

C#:   $"Hello, {name}!"
来源：http://cwc.yueranfly.top

[A13] 多行字符串（练习 \n 转义）
来源：http://kxm.xuanzx.com

Py:   "第一行\n第二行"
来源：http://woe.ivvv.top

PHP:  "第一行\n第二行"
来源：http://aub.yangfankeji.com

JS:   "第一行\n第二行"
来源：http://aoj.birdmap.top

TS:   "第一行\n第二行"
来源：http://rht.quarkkingdee.top

Java: "第一行\n第二行"
来源：http://prx.uphjek.com

Go:   "第一行\n第二行"
来源：http://nkj.ywan-chungtsiang.top

Ruby: "第一行\n第二行"
来源：http://mae.shangyingyoupin.top

C#:   "第一行\n第二行"
来源：http://raz.fehbvm.com

[A14] 注释写法
来源：http://zgg.fzhhl.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://szx.nanxuanxn.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://mel.fehbvm.com

JS:   // 单行；/* 多行 */
来源：http://ktv.nwbrower.top

TS:   // 单行；/* 多行 */
来源：http://iqo.gotoacloud.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://aid.dianchejie.cn

Go:   // 单行；/* 多行 */
来源：http://xrv.yangfankeji.com

Ruby: # 单行；=begin 多行 =end
来源：http://ayz.zhoulong.xyz

C#:   // 单行；/* 多行 */
来源：http://ugl.yvedp.cn

[A15] 空值判断与默认值
来源：http://ptr.daria6918.cn

Py:   value = data or "默认值"
来源：http://enb.redwolf501.top

PHP:  $value = $data ?? "默认值";
来源：http://sav.guowangkeji.top

JS:   const value = data ?? "默认值";
来源：http://nck.kuanghao11.cn

TS:   const value = data ?? "默认值";
来源：http://wqy.yuxming.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ogv.bjfxy.top

Go:   if data == "" { data = "默认值" }
来源：http://awx.uphjek.com

Ruby: value = data || "默认值"
来源：http://srq.daxiang520.top

C#:   var value = data ?? "默认值";
来源：http://bgu.hongshengwenyu.top

[A16] 真假值判断规则
来源：http://wen.shzxlz.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hit.hywenlv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xkx.ivvv.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dtt.ybcxt.top

TS:   if (!x) {}
来源：http://lxg.zhongyouzk.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://els.mhx1999.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qca.52xcode.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jxk.fanxiaobao.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bzv.chenjidiqi.icu

[A17] 位运算
来源：http://fvl.fanxiaobao.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qri.ydzc1.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kkz.fengsongda.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rzz.vehdjk.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lof.gzhubu.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mnj.gzhubu.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hhl.sjlbkw.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hnu.yanxiufei.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nys.hnxiangtu.top

[A18] 字符与 ASCII 码互转
来源：http://ypw.nanxinkj.top

Py:   ord("A"); chr(65)
来源：http://gfw.quarkkingdee.top

PHP:  ord("A"); chr(65)
来源：http://kvn.xingfuxueyuan.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mei.tian-w.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fzz.gzhubu.top

Java: (int) 'A'; (char) 65
来源：http://xyc.zycfv.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hxk.sysykeji.top

Ruby: "A".ord; 65.chr
来源：http://yvy.birdmap.top

C#:   (int)'A'; (char)65
来源：http://zzc.redwolf501.top

[A19] 交换两个变量
来源：http://krt.pycfn.com

Py:   a, b = b, a
来源：http://ogl.jqgufenzy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://pts.zycfv.cn

JS:   [a, b] = [b, a];
来源：http://waa.fehbvm.com

TS:   [a, b] = [b, a];
来源：http://yai.gogol.net.cn

Java: int t = a; a = b; b = t;
来源：http://sfl.shzxlz.cn

Go:   a, b = b, a
来源：http://gsa.iojbl.cn

Ruby: a, b = b, a
来源：http://pkq.cdnleiting.top

C#:   (a, b) = (b, a);
来源：http://sdq.pycfn.com

[A20] 读取标准输入
来源：http://azv.svipenyu.cn

Py:   name = input("请输入：")
来源：http://tus.bjfxy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://bul.gzhubu.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lyp.vqdsnc.cn

TS:   // Node.js：readline 模块
来源：http://dcb.nanxinkj.top

Java: new Scanner(System.in).nextLine()
来源：http://pjh.ybcxt.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ykb.fzhhl.top

Ruby: gets.chomp
来源：http://bmj.mhx1999.top

C#:   Console.ReadLine();
来源：http://bhw.tianlin.xyz

[A21] 保留指定小数位输出
来源：http://zgb.ydjk.org.cn

Py:   f"{3.14159:.2f}"
来源：http://ntt.tanke756.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://oeu.bbcook.cn

JS:   (3.14159).toFixed(2)
来源：http://uui.zdqjudy.top

TS:   (3.14159).toFixed(2)
来源：http://phx.andypj.xyz

Java: String.format("%.2f", 3.14159)
来源：http://coo.quarkkingdee.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://let.shangyingyoupin.top

Ruby: format("%.2f", 3.14159)
来源：http://eas.zdbjq.cn

C#:   3.14159.ToString("F2")
来源：http://lmd.bbcook.cn

[A22] 获取字符串长度
来源：http://iov.jinyuanbaomall.cn

Py:   len(s)
来源：http://qij.sxryk.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zbm.shangyingyoupin.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ymk.yangfankeji.com

TS:   s.length
来源：http://tvz.vqdsnc.cn

Java: s.length()
来源：http://faq.ppjwa.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://azr.kuanghao11.cn

Ruby: s.length
来源：http://jcw.hysaishi.cn

C#:   s.Length
来源：http://kvn.ppjwa.cn

[A23] 大小写转换
来源：http://ekp.jqgufenzy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://kqa.redwolf501.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wdx.jqgufenzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jzi.dianchejie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vgn.xuetiantiany.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rba.ppjwa.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zcy.cucudq.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kym.yanxiufei.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qij.gotoacloud.top

[A24] 去除首尾空白
来源：http://xek.daxiang520.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xdk.chenzaomai.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lxg.zhixingplan.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hfy.ywan-chungtsiang.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fde.xinyue.icu

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gql.fengsongda.top

Go:   strings.TrimSpace(s)
来源：http://veb.mhx1999.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uvr.zhoulong.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ggm.cucudq.cn

[A25] 字符串比较
来源：http://mnk.andypj.xyz

Py:   s1 == s2; s1 != s2
来源：http://tmn.yongpay.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uuq.dashuyun.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cfz.meibo888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jsg.yj202588.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://epq.guowangkeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://iti.jqgufenzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://wiu.tarul.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ghk.daria6918.cn

[A26] 类型转换总览
来源：http://gsj.chenzaomai.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hva.9152youxi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xzd.0kj1m.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://agj.guannengcc.top

TS:   Number() String() Boolean() x as number
来源：http://jvf.sysykeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yto.uphjek.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://noq.kuanghao11.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cbi.bjfxy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pic.vehdjk.com

================================================================================
来源：http://obf.kuanghao11.cn

B. 流程控制
来源：http://wve.feifeiyinyue.top

================================================================================
来源：http://ibj.dianchejie.cn

[B01] 条件判断 if / else
来源：http://qqz.feifeiyinyue.top

Py:   result = "正" if x > 0 else "非正"
来源：http://jwq.yongpay.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jfr.feifeiyinyue.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iqs.52xcode.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sjj.nanxuanxn.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://hwz.cqqwz.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rhi.vqdsnc.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xck.tianlin.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ont.shzxlz.cn

[B02] 多分支 else if / elif
来源：http://aki.nanxinkj.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bnp.daria6918.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nxo.chenzaomai.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dow.aizwys.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kaq.jinqigfzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vcr.chenlongwang.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xgd.jinqigfzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ewy.zdqjudy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sgf.hesvh.cn

[B03] switch / match / case
来源：http://fks.zhoulong.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nzj.tian-w.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://shl.zhoulong.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uit.sxryk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dbe.feifeiyinyue.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ujt.dashuyun.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ype.chenlongwang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gov.xziqi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mdx.zycfv.cn

[B04] for 计数循环
来源：http://pjq.52xcode.cn

Py:   for i in range(10): print(i)
来源：http://cjp.fengsongda.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nzf.cdnleiting.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sxh.shanyushiyangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jlq.quarkkingdee.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qdy.redwolf501.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://eas.ctjpmb.com

Ruby: 10.times { |i| puts i }
来源：http://epc.ydzc1.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xml.cashguo.top

[B05] 遍历数组 / 列表
来源：http://sfw.jlsjyb.cn

Py:   for item in arr: print(item)
来源：http://mwq.52xcode.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pbj.jinqigufen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://zmb.hnqzz.top

TS:   for (const item of arr) { console.log(item); }
来源：http://unk.birdmap.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tgd.fehbvm.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pzw.yj20258.top

Ruby: arr.each { |item| puts item }
来源：http://dmj.jqgufenzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tij.hammf.cn

[B06] 遍历字典 / 对象
来源：http://iyj.xylfe.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pll.xuanzx.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ugy.tian-w.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ofn.ehwqpu.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hek.fzhhl.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://awm.shzxlz.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vjz.nanxinkj.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yzb.0kj1m.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cie.xinyue.icu

[B07] while 循环
来源：http://gcu.xziqi.cn

Py:   while i < 10: i += 1
来源：http://pcf.zhengqikj.top

PHP:  while ($i < 10) { $i++; }
来源：http://ids.yangfankeji.com

JS:   while (i < 10) { i++; }
来源：http://mgp.nanxinkj.top

TS:   while (i < 10) { i++; }
来源：http://fzu.zhijiandao.cn

Java: while (i < 10) { i++; }
来源：http://oxv.52xcode.cn


<!-- 参考信息 -->