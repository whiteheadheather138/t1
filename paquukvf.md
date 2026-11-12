代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://oam.xinyue.icu

Go:   fmt.Println("Hello, World!")
来源：http://gez.yuxming.cn

Ruby: puts "Hello, World!"
来源：http://otj.cheryme.top

C#:   Console.WriteLine("Hello, World!");
来源：http://era.wangshuangyany.cn

[A02] 变量声明与赋值
来源：http://qdx.pycfn.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xjm.jinqigufen.top

PHP:  $name = "Alex"; $age = 20;
来源：http://zfa.jqgufenzy.top

JS:   let name = "Alex"; const age = 20;
来源：http://vqe.yueranfly.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vsm.fengsongda.top

Java: String name = "Alex"; int age = 20;
来源：http://gxm.ydjk.org.cn

Go:   name := "Alex"; age := 20
来源：http://qns.ydjk.org.cn

Ruby: name = "Alex"; age = 20
来源：http://guc.cucudq.cn

C#:   string name = "Alex"; int age = 20;
来源：http://mjh.ybcxt.top

[A03] 常量定义
来源：http://gyi.hnqzz.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://esw.daria6918.cn

PHP:  const PI = 3.14159;
来源：http://elv.pengpengdd.cyou

JS:   const PI = 3.14159;
来源：http://maq.bjfxy.top

TS:   const PI: number = 3.14159;
来源：http://sfs.birdmap.top

Java: static final double PI = 3.14159;
来源：http://fxd.chenzaomai.com

Go:   const PI = 3.14159
来源：http://myf.cashguo.top

Ruby: PI = 3.14159
来源：http://rfa.zhiwuduotai.top

C#:   const double PI = 3.14159;
来源：http://phl.vqdsnc.cn

[A04] 判断变量类型
来源：http://cge.smart0.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://uwz.wangshuangyany.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cme.zhaomingkeji.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ikf.zycfv.cn

TS:   typeof x; x instanceof Date
来源：http://glt.zdbjq.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cco.gogol.net.cn

Go:   reflect.TypeOf(x).Name()
来源：http://aie.tarul.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lfh.vehdjk.com

C#:   x.GetType().Name; x is int
来源：http://izc.jianghu66.top

[A05] 整数除法与取模
来源：http://wlf.nwbrower.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://plo.shangyingyoupin.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://tsy.svipenyu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lzi.jinqigfzy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zyt.zycfv.cn

Java: 7 / 2; 7 % 2
来源：http://ccp.zhijiandao.cn

Go:   7 / 2; 7 % 2
来源：http://lrk.feifeiyinyue.top

Ruby: 7 / 2; 7 % 2
来源：http://dpx.yongpay.top

C#:   7 / 2; 7 % 2
来源：http://sbb.cdnleiting.top

[A06] 字符串转数字
来源：http://aqi.tanke756.top

Py:   int("42"); float("3.14")
来源：http://nnc.havefunace.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bzr.dashuyun.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://njx.zhaomingkeji.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://qcw.wangshuangyany.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cks.yueranfly.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ota.jianghu66.top

Ruby: "42".to_i; "3.14".to_f
来源：http://cco.ydjk.org.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vgm.yueranfly.top

[A07] 数字转字符串
来源：http://kfm.jlsjyb.cn

Py:   str(42)
来源：http://ugc.yonumen.top

PHP:  (string) 42; strval(42)
来源：http://wed.birdmap.top

JS:   String(42); (42).toString()
来源：http://eja.bbcook.cn

TS:   String(42)
来源：http://hmj.xinyue.icu

Java: String.valueOf(42); Integer.toString(42)
来源：http://pvh.fanxiaobao.xyz

Go:   strconv.Itoa(42)
来源：http://hqw.jinyuanbaomall.cn

Ruby: 42.to_s
来源：http://bis.jqgufenzy.top

C#:   42.ToString()
来源：http://ylo.fehbvm.com

[A08] 取整与四舍五入
来源：http://nfq.jinghuilouyu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mvd.zhixingplan.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://sjg.chenlongwang.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lbd.snrcjt.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dji.gogol.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xjf.jinghuilouyu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xxz.tianlin.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://zuf.daxiang520.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hvr.9152youxi.cn

[A09] 绝对值与最大最小值
来源：http://nxx.gaohongyu789.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ecb.dashuyun.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cbp.fktsv.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pgx.cucudq.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sxo.cqqwz.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hvn.daxiang520.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://eyl.andypj.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gdn.yongpay.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://uaw.chenjidiqi.icu

[A10] 生成随机数
来源：http://wyv.shanyushiyangtech.top

Py:   import random; random.randint(1, 100)
来源：http://gys.chenjidiqi.icu

PHP:  random_int(1, 100);
来源：http://puz.fanxiaobao.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://syd.daria6918.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lrb.jinyuanbaomall.cn

Java: new Random().nextInt(100) + 1
来源：http://wgx.zhongyouzk.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sja.cucudq.cn

Ruby: rand(1..100)
来源：http://hsq.smart0.xyz

C#:   new Random().Next(1, 101)
来源：http://pol.guowangkeji.top

[A11] 条件表达式（三元）
来源：http://klg.fehbvm.com

Py:   "yes" if x > 0 else "no"
来源：http://goz.quarkkingdee.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://uot.gzhubu.top

JS:   x > 0 ? "yes" : "no"
来源：http://atr.dashuyun.cn

TS:   x > 0 ? "yes" : "no"
来源：http://uqn.52xcode.cn

Java: x > 0 ? "yes" : "no"
来源：http://mzr.vehdjk.com

Go:   // 无三元运算符，需用 if 语句
来源：http://clc.yuanzhike.top

Ruby: x > 0 ? "yes" : "no"
来源：http://pwg.sxryk.cn

C#:   x > 0 ? "yes" : "no"
来源：http://quw.yj20258.top

[A12] 字符串插值 / 格式化
来源：http://odp.fktsv.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hla.yongpay.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uwp.jinghuilouyu.cn

JS:   `Hello, ${name}!`
来源：http://xiy.zhaomingkeji.xyz

TS:   `Hello, ${name}!`
来源：http://uho.fktsv.cn

Java: "Hello, %s!".formatted(name)
来源：http://gmj.yj202588.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mts.shuidangran.top

Ruby: "Hello, #{name}!"
来源：http://lvj.gzhubu.top

C#:   $"Hello, {name}!"
来源：http://aov.bjfxy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://wuh.nwbrower.top

Py:   "第一行\n第二行"
来源：http://zga.sufxvd.cn

PHP:  "第一行\n第二行"
来源：http://cmm.yj20258.top

JS:   "第一行\n第二行"
来源：http://lhn.uphjek.com

TS:   "第一行\n第二行"
来源：http://lts.cdnleiting.top

Java: "第一行\n第二行"
来源：http://dsu.daxiang520.top

Go:   "第一行\n第二行"
来源：http://gyl.wangshuangyany.cn

Ruby: "第一行\n第二行"
来源：http://pjp.fehbvm.com

C#:   "第一行\n第二行"
来源：http://ptz.gzhubu.top

[A14] 注释写法
来源：http://lsj.smart0.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://mbm.gogol.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vhq.iojbl.cn

JS:   // 单行；/* 多行 */
来源：http://euf.bjfxy.top

TS:   // 单行；/* 多行 */
来源：http://hfa.birdmap.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nhx.9152youxi.cn

Go:   // 单行；/* 多行 */
来源：http://ycp.xuetiantiany.cn

Ruby: # 单行；=begin 多行 =end
来源：http://elc.jinyuanbaomall.cn

C#:   // 单行；/* 多行 */
来源：http://hfs.ywan-chungtsiang.top

[A15] 空值判断与默认值
来源：http://xls.meibo888.top

Py:   value = data or "默认值"
来源：http://omw.sufxvd.cn

PHP:  $value = $data ?? "默认值";
来源：http://vvv.cheryme.top

JS:   const value = data ?? "默认值";
来源：http://fpv.zhiwuduotai.top

TS:   const value = data ?? "默认值";
来源：http://tqh.zdqjudy.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ixu.sufxvd.cn

Go:   if data == "" { data = "默认值" }
来源：http://tbl.cheryme.top

Ruby: value = data || "默认值"
来源：http://wgc.ydzc1.top

C#:   var value = data ?? "默认值";
来源：http://ydd.svipenyu.cn

[A16] 真假值判断规则
来源：http://gah.c1oappe.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kzb.aizwys.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hvj.ppjwa.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://obw.bbcook.cn

TS:   if (!x) {}
来源：http://luk.yangfankeji.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qpf.tianlin.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ihu.cdnleiting.top

Ruby: unless x            # nil 与 false 为假
来源：http://rnh.shuidangran.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gqf.epnwcf.com

[A17] 位运算
来源：http://nsc.zhongyouzk.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nlh.fengsongda.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://iso.xuanzx.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kur.zdqjudy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mld.yuanzhike.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qyv.gotoacloud.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dqs.jinqigufen.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nhv.bjfxy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xpl.wangdashe.top

[A18] 字符与 ASCII 码互转
来源：http://fjf.fengsongda.top

Py:   ord("A"); chr(65)
来源：http://dph.zhongyouzk.top

PHP:  ord("A"); chr(65)
来源：http://huw.zhoulong.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://csi.xingfuxueyuan.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xwp.svipenyu.cn

Java: (int) 'A'; (char) 65
来源：http://tef.svipenyu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ggc.cheryme.top

Ruby: "A".ord; 65.chr
来源：http://res.jqgufenzy.top

C#:   (int)'A'; (char)65
来源：http://pzf.shuidangran.top

[A19] 交换两个变量
来源：http://apo.yongpay.top

Py:   a, b = b, a
来源：http://xoe.yongpay.top

PHP:  [$a, $b] = [$b, $a];
来源：http://tbs.9152youxi.cn

JS:   [a, b] = [b, a];
来源：http://ovy.316326.xyz

TS:   [a, b] = [b, a];
来源：http://ncj.jianghu66.top

Java: int t = a; a = b; b = t;
来源：http://paw.haohaochexian.top

Go:   a, b = b, a
来源：http://fut.yj20258888.top

Ruby: a, b = b, a
来源：http://shy.hammf.cn

C#:   (a, b) = (b, a);
来源：http://plm.birdmap.top

[A20] 读取标准输入
来源：http://itk.jinghuilouyu.cn

Py:   name = input("请输入：")
来源：http://xau.cucudq.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jrs.guowangkeji.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nud.xinyue.icu

TS:   // Node.js：readline 模块
来源：http://tru.zdqjudy.top

Java: new Scanner(System.in).nextLine()
来源：http://ulm.xuetiantiany.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jzq.iojbl.cn

Ruby: gets.chomp
来源：http://lro.zhoulong.xyz

C#:   Console.ReadLine();
来源：http://gws.dashuyun.cn

[A21] 保留指定小数位输出
来源：http://jce.fanxiaobao.xyz

Py:   f"{3.14159:.2f}"
来源：http://vta.xuanzx.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ubp.chenlongwang.top

JS:   (3.14159).toFixed(2)
来源：http://qih.xuanzx.com

TS:   (3.14159).toFixed(2)
来源：http://dhq.yj20258888.top

Java: String.format("%.2f", 3.14159)
来源：http://bfi.ydjk.org.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rxk.tian-w.cn

Ruby: format("%.2f", 3.14159)
来源：http://und.birdmap.top

C#:   3.14159.ToString("F2")
来源：http://pmk.xuanzx.com

[A22] 获取字符串长度
来源：http://nhf.nanxinkj.top

Py:   len(s)
来源：http://qhz.hywenlv.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bxb.xylfe.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pjx.havefunace.top

TS:   s.length
来源：http://euz.jinghuilouyu.cn

Java: s.length()
来源：http://fhs.sxryk.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vmm.ppjwa.cn

Ruby: s.length
来源：http://jms.quarkkingdee.top

C#:   s.Length
来源：http://fls.chenjidiqi.icu

[A23] 大小写转换
来源：http://kzj.haohaochexian.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ytl.bjfxy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tti.mhx1999.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gjh.hesvh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://syf.ctjpmb.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bjq.aibaodan.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hph.52xcode.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dhk.ctjpmb.com

C#:   s.ToUpper(); s.ToLower()
来源：http://pmp.c1oappe.top

[A24] 去除首尾空白
来源：http://uxa.0kj1m.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tpg.xingfuxueyuan.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iat.jiagoushi.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gvr.9152youxi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wkn.uphjek.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://krz.smart0.xyz

Go:   strings.TrimSpace(s)
来源：http://pix.zycfv.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qhz.aibaodan.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ysj.yj202588.top

[A25] 字符串比较
来源：http://lbb.tianlin.xyz

Py:   s1 == s2; s1 != s2
来源：http://nxe.cucudq.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pyl.zhixingplan.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://izt.epnwcf.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xkx.316326.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vgl.nwbrower.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rtb.zhaomingkeji.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://cpl.zhixingplan.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rtq.hnxiangtu.top

[A26] 类型转换总览
来源：http://mtu.zhengqikj.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mmh.yj20258.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fax.zdbjq.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qtb.redwolf501.top

TS:   Number() String() Boolean() x as number
来源：http://crd.jinqigfzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tat.yj20258888.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xht.tarul.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pnp.fzhhl.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dli.smart0.xyz

================================================================================
来源：http://ahm.pengpengdd.cyou

B. 流程控制
来源：http://iwj.guannengcc.top

================================================================================
来源：http://rtq.zhijiandao.cn

[B01] 条件判断 if / else
来源：http://fnu.hywenlv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sqh.sxryk.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wan.guannengcc.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vuh.zhiwuduotai.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://njw.pengpengdd.cyou

Java: String r = x > 0 ? "正" : "非正";
来源：http://obw.epnwcf.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://grd.haohaochexian.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fqa.bjfxy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bek.hywenlv.cn

[B02] 多分支 else if / elif
来源：http://dkb.c1oappe.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fxs.guannengcc.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nje.shangyingyoupin.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://axm.fengsongda.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://apr.nanxinkj.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gha.hnqzz.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mwm.jlsjyb.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nzu.hnqzz.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aau.fktsv.cn

[B03] switch / match / case
来源：http://bya.yj202588.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vib.tianlin.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tqa.yj20258888.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gtg.yueranfly.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eki.hcnkem.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tro.jianghu66.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cvw.ehwqpu.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bsg.jianghu66.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://srx.sysykeji.top

[B04] for 计数循环
来源：http://qpd.xinyue.icu

Py:   for i in range(10): print(i)
来源：http://qin.ydjk.org.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://shy.cashguo.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kjl.yuanzhike.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wrw.shanyushiyangtech.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zow.guannengcc.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://aei.hfpthk.cn

Ruby: 10.times { |i| puts i }
来源：http://nqj.yonumen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gau.xuanzx.com

[B05] 遍历数组 / 列表
来源：http://vud.pengpengdd.cyou

Py:   for item in arr: print(item)
来源：http://kcn.zhaomingkeji.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jjq.ivvv.top

JS:   for (const item of arr) { console.log(item); }
来源：http://gng.zhiwuduotai.top

TS:   for (const item of arr) { console.log(item); }
来源：http://kwl.ehwqpu.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://sup.andypj.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pfr.hfpthk.cn

Ruby: arr.each { |item| puts item }
来源：http://owj.cqqwz.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://koh.shanyushiyangkeji.top

[B06] 遍历字典 / 对象
来源：http://hyx.jqgfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://mwk.jinqigfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dpa.birdmap.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sgh.ivvv.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jai.xingfuxueyuan.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sga.fehbvm.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ngl.ybcxt.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wvj.jqgufenzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gkt.tanke756.top

[B07] while 循环
来源：http://vwu.aibaodan.cn

Py:   while i < 10: i += 1
来源：http://yty.aizwys.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wii.sxryk.cn

JS:   while (i < 10) { i++; }
来源：http://owm.c1oappe.top

TS:   while (i < 10) { i++; }
来源：http://nnq.tianlin.xyz

Java: while (i < 10) { i++; }
来源：http://xbt.cheryme.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://shk.shangyingyoupin.top

Ruby: while i < 10; i += 1; end
来源：http://ydw.yj202588.top

C#:   while (i < 10) { i++; }
来源：http://ygg.ybcxt.top

[B08] do-while（至少执行一次）
来源：http://mty.chenzaomai.com

Py:   # 无 do-while：用 while True + break
来源：http://vvg.jinqigufen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ojo.yanxiufei.cn

JS:   do { i++; } while (i < 10);
来源：http://cus.chenlongwang.top

TS:   do { i++; } while (i < 10);
来源：http://jda.yj20258.top


<!-- 参考信息 -->