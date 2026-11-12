代发 wailian999

[A02] 变量声明与赋值
来源：http://abp.fehbvm.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wlo.aizwys.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://djp.gzhubu.top

JS:   let name = "Alex"; const age = 20;
来源：http://hdf.haohaochexian.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cti.cashguo.top

Java: String name = "Alex"; int age = 20;
来源：http://gro.haohaochexian.top

Go:   name := "Alex"; age := 20
来源：http://yaf.fehbvm.com

Ruby: name = "Alex"; age = 20
来源：http://ouc.shuidangran.top

C#:   string name = "Alex"; int age = 20;
来源：http://yvk.xuetiantiany.cn

[A03] 常量定义
来源：http://hih.jqgfzy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gcj.zhongyouzk.top

PHP:  const PI = 3.14159;
来源：http://nzf.uphjek.com

JS:   const PI = 3.14159;
来源：http://yya.hesvh.cn

TS:   const PI: number = 3.14159;
来源：http://lbd.cqqwz.cn

Java: static final double PI = 3.14159;
来源：http://xhb.yuxming.cn

Go:   const PI = 3.14159
来源：http://pti.ppjwa.cn

Ruby: PI = 3.14159
来源：http://vdm.jianghu66.top

C#:   const double PI = 3.14159;
来源：http://rsa.yuanzhike.top

[A04] 判断变量类型
来源：http://tiu.hammf.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hkj.iojbl.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vbx.tian-w.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cdj.chenjidiqi.icu

TS:   typeof x; x instanceof Date
来源：http://ual.zhengqikj.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jwk.hnxiangtu.top

Go:   reflect.TypeOf(x).Name()
来源：http://ltm.nanxinkj.top

Ruby: x.class; x.is_a?(Integer)
来源：http://qtv.hywenlv.cn

C#:   x.GetType().Name; x is int
来源：http://nae.0kj1m.cn

[A05] 整数除法与取模
来源：http://nkg.bjfxy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kdl.yangfankeji.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://ugv.gogol.net.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cen.tian-w.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vfv.vqdsnc.cn

Java: 7 / 2; 7 % 2
来源：http://qme.yj20258888.top

Go:   7 / 2; 7 % 2
来源：http://kei.jinqigfzy.top

Ruby: 7 / 2; 7 % 2
来源：http://bdn.guowangkeji.top

C#:   7 / 2; 7 % 2
来源：http://opl.jiagoushi.top

[A06] 字符串转数字
来源：http://xdu.zhijiandao.cn

Py:   int("42"); float("3.14")
来源：http://ugi.sjlbkw.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xdz.hnxiangtu.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://inp.fehbvm.com

TS:   parseInt("42", 10); Number("42")
来源：http://dat.chenjidiqi.icu

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hoz.zycfv.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tnb.tanke756.top

Ruby: "42".to_i; "3.14".to_f
来源：http://nik.xingfuxueyuan.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tmu.zhongyouzk.top

[A07] 数字转字符串
来源：http://ymc.zhaomingkeji.xyz

Py:   str(42)
来源：http://blq.yongpay.top

PHP:  (string) 42; strval(42)
来源：http://okn.havefunace.top

JS:   String(42); (42).toString()
来源：http://zvk.kuanghao11.cn

TS:   String(42)
来源：http://aed.hammf.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nqr.mhx1999.top

Go:   strconv.Itoa(42)
来源：http://kuh.hnqzz.top

Ruby: 42.to_s
来源：http://upv.nanxinkj.top

C#:   42.ToString()
来源：http://jsr.hywenlv.cn

[A08] 取整与四舍五入
来源：http://nrk.yj20258888.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tft.ehwqpu.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zak.gogol.net.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://uel.mhx1999.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bip.cdnleiting.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ale.dashuyun.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://opn.zhongyouzk.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ezh.xingfuxueyuan.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hyy.bbcook.cn

[A09] 绝对值与最大最小值
来源：http://iwo.sxryk.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rbc.sjlbkw.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nkn.zhixingplan.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fhm.wangshuangyany.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pvy.zhaomingkeji.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dsg.zhoulong.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://owh.cucudq.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rwm.cucudq.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pcj.haohaochexian.top

[A10] 生成随机数
来源：http://pxg.gzhubu.top

Py:   import random; random.randint(1, 100)
来源：http://rsj.wangshuangyany.cn

PHP:  random_int(1, 100);
来源：http://pbo.gzhubu.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kvu.haohaochexian.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lfe.ybcxt.top

Java: new Random().nextInt(100) + 1
来源：http://hah.gaohongyu789.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zey.yangfankeji.com

Ruby: rand(1..100)
来源：http://wri.fktsv.cn

C#:   new Random().Next(1, 101)
来源：http://lwf.zhijiandao.cn

[A11] 条件表达式（三元）
来源：http://gdg.tarul.cn

Py:   "yes" if x > 0 else "no"
来源：http://mnw.jinqigufen.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://oxg.gogol.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://apc.zhaomingkeji.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://chz.ywan-chungtsiang.top

Java: x > 0 ? "yes" : "no"
来源：http://pgz.shzxlz.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://tzv.gogol.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gat.0kj1m.cn

C#:   x > 0 ? "yes" : "no"
来源：http://syq.dashuyun.cn

[A12] 字符串插值 / 格式化
来源：http://wxr.yj20258888.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dpz.0kj1m.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wqu.yj20258888.top

JS:   `Hello, ${name}!`
来源：http://rdt.hysaishi.cn

TS:   `Hello, ${name}!`
来源：http://rgq.bjfxy.top

Java: "Hello, %s!".formatted(name)
来源：http://cha.hnqzz.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hez.quarkkingdee.top

Ruby: "Hello, #{name}!"
来源：http://adu.havefunace.top

C#:   $"Hello, {name}!"
来源：http://xtz.gzhubu.top

[A13] 多行字符串（练习 \n 转义）
来源：http://jdz.havefunace.top

Py:   "第一行\n第二行"
来源：http://ato.andypj.xyz

PHP:  "第一行\n第二行"
来源：http://mte.fanxiaobao.xyz

JS:   "第一行\n第二行"
来源：http://poa.c1oappe.top

TS:   "第一行\n第二行"
来源：http://efn.nanxuanxn.top

Java: "第一行\n第二行"
来源：http://kcd.52xcode.cn

Go:   "第一行\n第二行"
来源：http://rqz.chenzaomai.com

Ruby: "第一行\n第二行"
来源：http://azp.yonumen.top

C#:   "第一行\n第二行"
来源：http://ivo.nanxinkj.top

[A14] 注释写法
来源：http://vco.birdmap.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://jgn.nanxinkj.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://gpd.gogol.net.cn

JS:   // 单行；/* 多行 */
来源：http://lkc.svipenyu.cn

TS:   // 单行；/* 多行 */
来源：http://rse.xuetiantiany.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ffx.gzhubu.top

Go:   // 单行；/* 多行 */
来源：http://bjo.redwolf501.top

Ruby: # 单行；=begin 多行 =end
来源：http://huv.xuanzx.com

C#:   // 单行；/* 多行 */
来源：http://bpp.vehdjk.com

[A15] 空值判断与默认值
来源：http://yqf.nanxuanxn.top

Py:   value = data or "默认值"
来源：http://kya.zdqjudy.top

PHP:  $value = $data ?? "默认值";
来源：http://gvo.fzhhl.top

JS:   const value = data ?? "默认值";
来源：http://lac.gaohongyu789.top

TS:   const value = data ?? "默认值";
来源：http://wac.shanyushiyangkeji.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dwc.guannengcc.top

Go:   if data == "" { data = "默认值" }
来源：http://fah.uphjek.com

Ruby: value = data || "默认值"
来源：http://brr.chenzaomai.com

C#:   var value = data ?? "默认值";
来源：http://qdv.9152youxi.cn

[A16] 真假值判断规则
来源：http://paj.cqqwz.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://irp.andypj.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ejm.ydjk.org.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fyt.pycfn.com

TS:   if (!x) {}
来源：http://mlv.shangyingyoupin.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lhv.chenzaomai.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bva.cqqwz.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jdv.ctjpmb.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ebc.guannengcc.top

[A17] 位运算
来源：http://gof.gogol.net.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://awi.shanyushiyangkeji.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xrq.hammf.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dms.cheryme.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ebb.jqgufenzy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://huh.tian-w.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cqu.ydzc1.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ohy.dashuyun.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ked.jlsjyb.cn

[A18] 字符与 ASCII 码互转
来源：http://zrw.ctjpmb.com

Py:   ord("A"); chr(65)
来源：http://dbv.yongpay.top

PHP:  ord("A"); chr(65)
来源：http://dbc.hysaishi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xpn.jiagoushi.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bxp.zhaomingkeji.xyz

Java: (int) 'A'; (char) 65
来源：http://yat.hammf.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hqi.fktsv.cn

Ruby: "A".ord; 65.chr
来源：http://cfi.tarul.cn

C#:   (int)'A'; (char)65
来源：http://cqj.0kj1m.cn

[A19] 交换两个变量
来源：http://qtu.jinghuilouyu.cn

Py:   a, b = b, a
来源：http://mzv.yuxming.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bmo.ivvv.top

JS:   [a, b] = [b, a];
来源：http://fvx.fehbvm.com

TS:   [a, b] = [b, a];
来源：http://ark.ydzc1.top

Java: int t = a; a = b; b = t;
来源：http://azm.daxiang520.top

Go:   a, b = b, a
来源：http://zcp.feifeiyinyue.top

Ruby: a, b = b, a
来源：http://uel.jinqigufen.top

C#:   (a, b) = (b, a);
来源：http://zrm.cdnleiting.top

[A20] 读取标准输入
来源：http://kql.xingfuxueyuan.xyz

Py:   name = input("请输入：")
来源：http://qdz.pengpengdd.cyou

PHP:  $name = trim(fgets(STDIN));
来源：http://hph.hongshengwenyu.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://igf.jinghuilouyu.cn

TS:   // Node.js：readline 模块
来源：http://xcz.zhengqikj.top

Java: new Scanner(System.in).nextLine()
来源：http://vxb.hysaishi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://niu.tarul.cn

Ruby: gets.chomp
来源：http://xqr.cucudq.cn

C#:   Console.ReadLine();
来源：http://xsx.nanxinkj.top

[A21] 保留指定小数位输出
来源：http://unv.iojbl.cn

Py:   f"{3.14159:.2f}"
来源：http://clp.52xcode.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://iip.ydjk.org.cn

JS:   (3.14159).toFixed(2)
来源：http://dic.gotoacloud.top

TS:   (3.14159).toFixed(2)
来源：http://ghw.iojbl.cn

Java: String.format("%.2f", 3.14159)
来源：http://jzm.tarul.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oqn.chenlongwang.top

Ruby: format("%.2f", 3.14159)
来源：http://gmi.havefunace.top

C#:   3.14159.ToString("F2")
来源：http://qve.yfazqb.com

[A22] 获取字符串长度
来源：http://oxh.dianchejie.cn

Py:   len(s)
来源：http://psr.gzhubu.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://may.jianghu66.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tlh.tanke756.top

TS:   s.length
来源：http://tci.daria6918.cn

Java: s.length()
来源：http://dqe.yonumen.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uqy.zhaomingkeji.xyz

Ruby: s.length
来源：http://ekz.yonumen.top

C#:   s.Length
来源：http://fwt.zhixingplan.top

[A23] 大小写转换
来源：http://lsf.ybcxt.top

Py:   s.upper(); s.lower(); s.title()
来源：http://koz.hesvh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://unu.fktsv.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ewj.birdmap.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vbw.shangyingyoupin.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vil.chenlongwang.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://adq.zhiwuduotai.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kzo.shzxlz.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zzy.0kj1m.cn

[A24] 去除首尾空白
来源：http://idg.ehwqpu.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rtm.xingfuxueyuan.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iwc.fktsv.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ymo.hywenlv.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ttc.fzhhl.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kpx.hfpthk.cn

Go:   strings.TrimSpace(s)
来源：http://vlw.sweek.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fvh.bjfxy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qxi.aizwys.cn

[A25] 字符串比较
来源：http://agd.yangfankeji.com

Py:   s1 == s2; s1 != s2
来源：http://rol.yj20258.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zet.mhx1999.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dsl.xylfe.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xuo.jlsjyb.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nez.fanxiaobao.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lob.daxiang520.top

Ruby: s1 == s2; s1 <=> s2
来源：http://qaf.cqqwz.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hcm.chenzaomai.com

[A26] 类型转换总览
来源：http://ejq.ydzc1.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rut.gaohongyu789.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jaw.iojbl.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yox.hcnkem.com

TS:   Number() String() Boolean() x as number
来源：http://rzn.0kj1m.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mjg.fanxiaobao.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jfa.zhaomingkeji.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://ksn.aibaodan.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ipr.bjfxy.top

================================================================================
来源：http://lto.hongshengwenyu.top

B. 流程控制
来源：http://cbj.haohaochexian.top

================================================================================
来源：http://syv.redwolf501.top

[B01] 条件判断 if / else
来源：http://rbc.chenjidiqi.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://pcf.hesvh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xge.tarul.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dbv.hammf.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cil.svipenyu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jmv.chenjidiqi.icu

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sbm.sjlbkw.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fzq.bbcook.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nes.zhengqikj.top

[B02] 多分支 else if / elif
来源：http://fam.jianghu66.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mjm.fanxiaobao.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hkz.nwbrower.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qzz.epnwcf.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://txf.hesvh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hcv.0kj1m.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pyp.zycfv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yil.tanke756.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iqa.epnwcf.com

[B03] switch / match / case
来源：http://wrn.hongshengwenyu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://otw.shanyushiyangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qcn.tian-w.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qcx.snrcjt.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://icw.ctjpmb.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://las.redwolf501.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://waw.fanxiaobao.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qxx.cucudq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rxx.guowangkeji.top

[B04] for 计数循环
来源：http://mja.sysykeji.top

Py:   for i in range(10): print(i)
来源：http://afx.uphjek.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hyl.dianchejie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qlx.hcnkem.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://exs.uphjek.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eeg.zhijiandao.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hen.sysykeji.top

Ruby: 10.times { |i| puts i }
来源：http://dmm.shanyushiyangtech.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bij.havefunace.top

[B05] 遍历数组 / 列表
来源：http://fse.dashuyun.cn

Py:   for item in arr: print(item)
来源：http://nbb.pycfn.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fsm.jqgfzy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hve.yj20258888.top

TS:   for (const item of arr) { console.log(item); }
来源：http://wlz.0kj1m.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hzy.tianlin.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ahi.hcnkem.com

Ruby: arr.each { |item| puts item }
来源：http://qbw.chenzaomai.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kfo.bbcook.cn

[B06] 遍历字典 / 对象
来源：http://yzo.dianchejie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fli.yanxiufei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ewl.zycfv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bvh.daria6918.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ioh.pycfn.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dzc.jinqigufen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tky.shuidangran.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xqn.chenzaomai.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bix.ctjpmb.com

[B07] while 循环
来源：http://zmd.jiagoushi.top

Py:   while i < 10: i += 1
来源：http://yzl.zhongyouzk.top

PHP:  while ($i < 10) { $i++; }
来源：http://uab.feifeiyinyue.top

JS:   while (i < 10) { i++; }
来源：http://uih.cashguo.top

TS:   while (i < 10) { i++; }
来源：http://hiq.bbcook.cn

Java: while (i < 10) { i++; }
来源：http://ade.hnxiangtu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bxs.epnwcf.com

Ruby: while i < 10; i += 1; end
来源：http://krw.hysaishi.cn

C#:   while (i < 10) { i++; }
来源：http://wqu.hysaishi.cn

[B08] do-while（至少执行一次）
来源：http://zjn.cqqwz.cn

Py:   # 无 do-while：用 while True + break
来源：http://vvd.shuidangran.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ctr.sjlbkw.cn

JS:   do { i++; } while (i < 10);
来源：http://ekc.jinqigfzy.top

TS:   do { i++; } while (i < 10);
来源：http://zng.ctjpmb.com

Java: do { i++; } while (i < 10);
来源：http://cvd.nwbrower.top

Go:   for { i++; if i >= 10 { break } }
来源：http://uqs.shzxlz.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rsq.meibo888.top

C#:   do { i++; } while (i < 10);
来源：http://tiq.yongpay.top


<!-- 参考信息 -->