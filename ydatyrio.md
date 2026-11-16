代发 wailian999

================================================================================
来源：http://gmj.hysaishi.cn

A. 基础语法与类型
来源：http://yok.redwolf501.top

================================================================================
来源：http://lmj.fengsongda.top

[A01] Hello World
来源：http://iio.yanxiufei.cn

Py:   print("Hello, World!")
来源：http://tpn.zhongyouzk.top

PHP:  echo "Hello, World!";
来源：http://mhg.jinqigufen.top

JS:   console.log("Hello, World!");
来源：http://eke.jqgufenzy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wdq.0kj1m.cn

Java: System.out.println("Hello, World!");
来源：http://dir.pycfn.com

Go:   fmt.Println("Hello, World!")
来源：http://pki.dianchejie.cn

Ruby: puts "Hello, World!"
来源：http://hdk.nwbrower.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ncm.guowangkeji.top

[A02] 变量声明与赋值
来源：http://lye.svipenyu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ixv.chenjidiqi.icu

PHP:  $name = "Alex"; $age = 20;
来源：http://vyw.316326.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://ljt.cucudq.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://czw.hfpthk.cn

Java: String name = "Alex"; int age = 20;
来源：http://fue.mhx1999.top

Go:   name := "Alex"; age := 20
来源：http://efe.bbcook.cn

Ruby: name = "Alex"; age = 20
来源：http://lrr.pycfn.com

C#:   string name = "Alex"; int age = 20;
来源：http://doa.zycfv.cn

[A03] 常量定义
来源：http://fei.wangshuangyany.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://iin.ydzc1.top

PHP:  const PI = 3.14159;
来源：http://rdj.jinqigufen.top

JS:   const PI = 3.14159;
来源：http://obz.ydjk.org.cn

TS:   const PI: number = 3.14159;
来源：http://ull.hesvh.cn

Java: static final double PI = 3.14159;
来源：http://zwv.hesvh.cn

Go:   const PI = 3.14159
来源：http://yho.hcnkem.com

Ruby: PI = 3.14159
来源：http://cug.hongshengwenyu.top

C#:   const double PI = 3.14159;
来源：http://pik.aizwys.cn

[A04] 判断变量类型
来源：http://pvs.fehbvm.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://jkh.jqgfzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wtf.fktsv.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cre.zhengqikj.top

TS:   typeof x; x instanceof Date
来源：http://ort.snrcjt.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dlv.ctjpmb.com

Go:   reflect.TypeOf(x).Name()
来源：http://oyd.yueranfly.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ysr.xingfuxueyuan.xyz

C#:   x.GetType().Name; x is int
来源：http://pwj.zhixingplan.top

[A05] 整数除法与取模
来源：http://uix.guannengcc.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ztc.yongpay.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ojx.nanxinkj.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ret.zhiwuduotai.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sbd.xuanzx.com

Java: 7 / 2; 7 % 2
来源：http://fxb.sufxvd.cn

Go:   7 / 2; 7 % 2
来源：http://cef.xziqi.cn

Ruby: 7 / 2; 7 % 2
来源：http://xkl.yuanzhike.top

C#:   7 / 2; 7 % 2
来源：http://jvo.ydzc1.top

[A06] 字符串转数字
来源：http://xky.cheryme.top

Py:   int("42"); float("3.14")
来源：http://niq.zhixingplan.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zdv.vqdsnc.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://phl.sufxvd.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cix.wangshuangyany.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tgh.9152youxi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dds.mhx1999.top

Ruby: "42".to_i; "3.14".to_f
来源：http://eej.havefunace.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rpv.hysaishi.cn

[A07] 数字转字符串
来源：http://cml.xingfuxueyuan.xyz

Py:   str(42)
来源：http://klc.316326.xyz

PHP:  (string) 42; strval(42)
来源：http://gtk.shanyushiyangtech.top

JS:   String(42); (42).toString()
来源：http://odf.svipenyu.cn

TS:   String(42)
来源：http://gfa.fehbvm.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://whs.yj202588.top

Go:   strconv.Itoa(42)
来源：http://ztt.uphjek.com

Ruby: 42.to_s
来源：http://ihi.hnxiangtu.top

C#:   42.ToString()
来源：http://sho.gogol.net.cn

[A08] 取整与四舍五入
来源：http://iyd.pengpengdd.cyou

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fkj.shangyingyoupin.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zrb.yvedp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nxh.yanxiufei.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ogu.yonumen.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://iuk.ctjpmb.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xfa.hesvh.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://duv.yj20258.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rdh.redwolf501.top

[A09] 绝对值与最大最小值
来源：http://eqj.zhixingplan.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ptk.fktsv.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cwn.yueranfly.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nyt.zhoulong.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nty.yuxming.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kqj.pycfn.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xlj.mhx1999.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://smd.aizwys.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://epq.kuanghao11.cn

[A10] 生成随机数
来源：http://iju.tian-w.cn

Py:   import random; random.randint(1, 100)
来源：http://wwt.zhijiandao.cn

PHP:  random_int(1, 100);
来源：http://vlj.hywenlv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qby.jinyuanbaomall.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tcy.xuetiantiany.cn

Java: new Random().nextInt(100) + 1
来源：http://whw.zhixingplan.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gpp.shanyushiyangkeji.top

Ruby: rand(1..100)
来源：http://saq.shuidangran.top

C#:   new Random().Next(1, 101)
来源：http://ivx.tianlin.xyz

[A11] 条件表达式（三元）
来源：http://evc.mhx1999.top

Py:   "yes" if x > 0 else "no"
来源：http://axg.zhengqikj.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ieh.hysaishi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gvk.aizwys.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rap.nanxuanxn.top

Java: x > 0 ? "yes" : "no"
来源：http://kda.yuxming.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://iss.birdmap.top

Ruby: x > 0 ? "yes" : "no"
来源：http://zqi.zhengqikj.top

C#:   x > 0 ? "yes" : "no"
来源：http://lts.cucudq.cn

[A12] 字符串插值 / 格式化
来源：http://ibu.meibo888.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rpz.haohaochexian.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dfh.shanyushiyangtech.top

JS:   `Hello, ${name}!`
来源：http://uoe.ydzc1.top

TS:   `Hello, ${name}!`
来源：http://fgd.pengpengdd.cyou

Java: "Hello, %s!".formatted(name)
来源：http://svx.jyoumei.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kkb.tanke756.top

Ruby: "Hello, #{name}!"
来源：http://okk.zhaomingkeji.xyz

C#:   $"Hello, {name}!"
来源：http://xft.ydzc1.top

[A13] 多行字符串（练习 \n 转义）
来源：http://hzb.ybcxt.top

Py:   "第一行\n第二行"
来源：http://cia.ybcxt.top

PHP:  "第一行\n第二行"
来源：http://rmh.andypj.xyz

JS:   "第一行\n第二行"
来源：http://nty.52xcode.cn

TS:   "第一行\n第二行"
来源：http://vai.shanyushiyangtech.top

Java: "第一行\n第二行"
来源：http://qyb.hywenlv.cn

Go:   "第一行\n第二行"
来源：http://wst.nanxinkj.top

Ruby: "第一行\n第二行"
来源：http://kee.ppjwa.cn

C#:   "第一行\n第二行"
来源：http://zzx.jqgufenzy.top

[A14] 注释写法
来源：http://hbs.andypj.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://xti.jiagoushi.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://avf.zhijiandao.cn

JS:   // 单行；/* 多行 */
来源：http://nia.vqdsnc.cn

TS:   // 单行；/* 多行 */
来源：http://coe.jyoumei.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rlj.ybcxt.top

Go:   // 单行；/* 多行 */
来源：http://nam.gotoacloud.top

Ruby: # 单行；=begin 多行 =end
来源：http://wcq.52xcode.cn

C#:   // 单行；/* 多行 */
来源：http://fzg.quarkkingdee.top

[A15] 空值判断与默认值
来源：http://syh.yuxming.cn

Py:   value = data or "默认值"
来源：http://kix.zhongyouzk.top

PHP:  $value = $data ?? "默认值";
来源：http://llt.gotoacloud.top

JS:   const value = data ?? "默认值";
来源：http://xla.svipenyu.cn

TS:   const value = data ?? "默认值";
来源：http://eye.jyoumei.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gco.hnqzz.top

Go:   if data == "" { data = "默认值" }
来源：http://dmd.xinyue.icu

Ruby: value = data || "默认值"
来源：http://syi.ivvv.top

C#:   var value = data ?? "默认值";
来源：http://nbp.fzhhl.top

[A16] 真假值判断规则
来源：http://zon.shanyushiyangtech.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rka.ydjk.org.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vlh.guannengcc.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qnj.epnwcf.com

TS:   if (!x) {}
来源：http://hze.jlsjyb.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jaj.zdqjudy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mmu.jiagoushi.top

Ruby: unless x            # nil 与 false 为假
来源：http://kbz.vehdjk.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yuq.wangshuangyany.cn

[A17] 位运算
来源：http://jvq.wangshuangyany.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wcb.gogol.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sjd.yonumen.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kxz.hnqzz.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://iex.cashguo.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ayq.9152youxi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jby.ybcxt.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sax.jinqigufen.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cdi.nanxinkj.top

[A18] 字符与 ASCII 码互转
来源：http://rbr.cucudq.cn

Py:   ord("A"); chr(65)
来源：http://vhm.fzhhl.top

PHP:  ord("A"); chr(65)
来源：http://rgd.yfazqb.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://brp.xuanzx.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dvg.shanyushiyangkeji.top

Java: (int) 'A'; (char) 65
来源：http://cef.aizwys.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fiv.yvedp.cn

Ruby: "A".ord; 65.chr
来源：http://dgr.xuanzx.com

C#:   (int)'A'; (char)65
来源：http://iiw.zhijiandao.cn

[A19] 交换两个变量
来源：http://kgu.yangfankeji.com

Py:   a, b = b, a
来源：http://tky.fehbvm.com

PHP:  [$a, $b] = [$b, $a];
来源：http://uqy.vqdsnc.cn

JS:   [a, b] = [b, a];
来源：http://sjl.gogol.net.cn

TS:   [a, b] = [b, a];
来源：http://bos.uphjek.com

Java: int t = a; a = b; b = t;
来源：http://sdg.xylfe.cn

Go:   a, b = b, a
来源：http://jdu.sufxvd.cn

Ruby: a, b = b, a
来源：http://lru.yj20258888.top

C#:   (a, b) = (b, a);
来源：http://dkn.feifeiyinyue.top

[A20] 读取标准输入
来源：http://ryv.guowangkeji.top

Py:   name = input("请输入：")
来源：http://xsk.aizwys.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://fym.sufxvd.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pdu.xinyue.icu

TS:   // Node.js：readline 模块
来源：http://czf.pengpengdd.cyou

Java: new Scanner(System.in).nextLine()
来源：http://suo.yj20258888.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bjo.fehbvm.com

Ruby: gets.chomp
来源：http://nrc.shangyingyoupin.top

C#:   Console.ReadLine();
来源：http://xtl.zdqjudy.top

[A21] 保留指定小数位输出
来源：http://vwe.daxiang520.top

Py:   f"{3.14159:.2f}"
来源：http://pkb.xinyue.icu

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ybw.52xcode.cn

JS:   (3.14159).toFixed(2)
来源：http://div.aibaodan.cn

TS:   (3.14159).toFixed(2)
来源：http://wyq.quarkkingdee.top

Java: String.format("%.2f", 3.14159)
来源：http://bkk.yongpay.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qzy.chenzaomai.com

Ruby: format("%.2f", 3.14159)
来源：http://szl.zhiwuduotai.top

C#:   3.14159.ToString("F2")
来源：http://gkz.xinyue.icu

[A22] 获取字符串长度
来源：http://ris.xylfe.cn

Py:   len(s)
来源：http://egu.cashguo.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zkc.xziqi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pom.zycfv.cn

TS:   s.length
来源：http://zpq.fengsongda.top

Java: s.length()
来源：http://jyo.52xcode.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://znj.zdqjudy.top

Ruby: s.length
来源：http://yjo.mhx1999.top

C#:   s.Length
来源：http://hww.sxryk.cn

[A23] 大小写转换
来源：http://foz.fehbvm.com

Py:   s.upper(); s.lower(); s.title()
来源：http://dzt.hongshengwenyu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fhj.cucudq.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jcq.gotoacloud.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qza.sufxvd.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vxu.birdmap.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ese.shanyushiyangkeji.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pml.sweek.top

C#:   s.ToUpper(); s.ToLower()
来源：http://rno.cqqwz.cn

[A24] 去除首尾空白
来源：http://wvk.quarkkingdee.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kxg.havefunace.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gpm.tarul.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zmy.snrcjt.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ega.gaohongyu789.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://snf.hcnkem.com

Go:   strings.TrimSpace(s)
来源：http://ssn.ydzc1.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ame.kuanghao11.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lho.fzhhl.top

[A25] 字符串比较
来源：http://mtn.jinyuanbaomall.cn

Py:   s1 == s2; s1 != s2
来源：http://jsm.epnwcf.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xch.fanxiaobao.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://irg.iojbl.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ztj.gaohongyu789.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ako.52xcode.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hgp.jianghu66.top

Ruby: s1 == s2; s1 <=> s2
来源：http://vuf.zdbjq.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lfy.chenzaomai.com

[A26] 类型转换总览
来源：http://yjg.hfpthk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ogf.ywan-chungtsiang.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gji.hesvh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qzp.sweek.top

TS:   Number() String() Boolean() x as number
来源：http://hvb.jyoumei.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tzt.ybcxt.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://crg.yuxming.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://otp.cqqwz.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oad.zhiwuduotai.top

================================================================================
来源：http://eas.hnqzz.top

B. 流程控制
来源：http://zpz.tanke756.top

================================================================================
来源：http://qdu.hammf.cn

[B01] 条件判断 if / else
来源：http://gfj.kuanghao11.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ept.yangfankeji.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bie.aizwys.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dxo.kuanghao11.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xnj.zhijiandao.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pca.fzhhl.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dzy.aibaodan.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rte.yuanzhike.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uue.cheryme.top

[B02] 多分支 else if / elif
来源：http://kxm.tian-w.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uvn.zhaomingkeji.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qip.cheryme.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tdz.bjfxy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://naf.gotoacloud.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://haz.sjlbkw.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jub.hysaishi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pkw.ydjk.org.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://syp.xinyue.icu

[B03] switch / match / case
来源：http://nui.ywan-chungtsiang.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://usk.gogol.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hxb.yvedp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://njt.jiagoushi.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zwd.zhijiandao.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rfo.9152youxi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kaz.nanxuanxn.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mwm.iojbl.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://slk.aibaodan.cn

[B04] for 计数循环
来源：http://ksj.zhoulong.xyz

Py:   for i in range(10): print(i)
来源：http://fqe.316326.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gwm.yuxming.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eme.pycfn.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ith.sysykeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ajp.gogol.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://icg.zdqjudy.top

Ruby: 10.times { |i| puts i }
来源：http://bms.ctjpmb.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fjx.zhaomingkeji.xyz

[B05] 遍历数组 / 列表
来源：http://rax.vqdsnc.cn

Py:   for item in arr: print(item)
来源：http://whz.zhixingplan.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ebi.cqqwz.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nuv.havefunace.top

TS:   for (const item of arr) { console.log(item); }
来源：http://jga.zhengqikj.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jkm.zhiwuduotai.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fwg.meibo888.top

Ruby: arr.each { |item| puts item }
来源：http://tzt.dashuyun.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cyl.gotoacloud.top

[B06] 遍历字典 / 对象
来源：http://tqj.guowangkeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://pze.uphjek.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fed.haohaochexian.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vgt.vehdjk.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rwh.tian-w.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jyt.cdnleiting.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tzr.sxryk.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hzu.hysaishi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zyn.epnwcf.com

[B07] while 循环
来源：http://phm.hnqzz.top

Py:   while i < 10: i += 1
来源：http://mhu.hnxiangtu.top

PHP:  while ($i < 10) { $i++; }
来源：http://meq.aibaodan.cn

JS:   while (i < 10) { i++; }
来源：http://xiy.shuidangran.top

TS:   while (i < 10) { i++; }
来源：http://jyu.fehbvm.com

Java: while (i < 10) { i++; }
来源：http://hzs.mhx1999.top


<!-- 参考信息 -->