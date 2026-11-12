代发 wailian999

[A02] 变量声明与赋值
来源：http://huz.hcnkem.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gxh.smart0.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://oul.birdmap.top

JS:   let name = "Alex"; const age = 20;
来源：http://vlz.tian-w.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yih.yj202588.top

Java: String name = "Alex"; int age = 20;
来源：http://tvm.zdqjudy.top

Go:   name := "Alex"; age := 20
来源：http://tgp.hfpthk.cn

Ruby: name = "Alex"; age = 20
来源：http://iax.jinghuilouyu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rxw.bbcook.cn

[A03] 常量定义
来源：http://avw.hywenlv.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://plk.zhiwuduotai.top

PHP:  const PI = 3.14159;
来源：http://ybm.xingfuxueyuan.xyz

JS:   const PI = 3.14159;
来源：http://yms.uphjek.com

TS:   const PI: number = 3.14159;
来源：http://cwz.hongshengwenyu.top

Java: static final double PI = 3.14159;
来源：http://ngj.cucudq.cn

Go:   const PI = 3.14159
来源：http://ybq.xylfe.cn

Ruby: PI = 3.14159
来源：http://thw.yj20258888.top

C#:   const double PI = 3.14159;
来源：http://chf.hfpthk.cn

[A04] 判断变量类型
来源：http://ava.zhaomingkeji.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://qyo.hysaishi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qkv.jinyuanbaomall.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ynu.zhongyouzk.top

TS:   typeof x; x instanceof Date
来源：http://jca.shzxlz.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qah.bjfxy.top

Go:   reflect.TypeOf(x).Name()
来源：http://cis.jinghuilouyu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kmv.chenlongwang.top

C#:   x.GetType().Name; x is int
来源：http://uhy.xziqi.cn

[A05] 整数除法与取模
来源：http://lxn.svipenyu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cki.svipenyu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hiw.gaohongyu789.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fxd.sweek.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dxv.cqqwz.cn

Java: 7 / 2; 7 % 2
来源：http://ndp.ivvv.top

Go:   7 / 2; 7 % 2
来源：http://ity.tarul.cn

Ruby: 7 / 2; 7 % 2
来源：http://ger.pycfn.com

C#:   7 / 2; 7 % 2
来源：http://xeg.chenlongwang.top

[A06] 字符串转数字
来源：http://bmd.bbcook.cn

Py:   int("42"); float("3.14")
来源：http://iim.aizwys.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://awy.kuanghao11.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mhq.svipenyu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rcx.gogol.net.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mht.aizwys.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://oht.fengsongda.top

Ruby: "42".to_i; "3.14".to_f
来源：http://woh.wangshuangyany.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fhx.quarkkingdee.top

[A07] 数字转字符串
来源：http://lsc.316326.xyz

Py:   str(42)
来源：http://bxh.9152youxi.cn

PHP:  (string) 42; strval(42)
来源：http://sll.hcnkem.com

JS:   String(42); (42).toString()
来源：http://unl.haohaochexian.top

TS:   String(42)
来源：http://vhi.svipenyu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://oyc.chenlongwang.top

Go:   strconv.Itoa(42)
来源：http://oru.zhongyouzk.top

Ruby: 42.to_s
来源：http://mci.cqqwz.cn

C#:   42.ToString()
来源：http://rsz.andypj.xyz

[A08] 取整与四舍五入
来源：http://bmq.zhengqikj.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gxv.shanyushiyangkeji.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://uck.daria6918.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://yqq.ybcxt.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xjw.jiagoushi.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mgl.kuanghao11.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tcb.tian-w.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qhb.fzhhl.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://nua.quarkkingdee.top

[A09] 绝对值与最大最小值
来源：http://upg.zycfv.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dnb.zhongyouzk.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yim.bbcook.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wcc.fzhhl.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lxf.daria6918.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dhq.daria6918.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://plq.ybcxt.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tva.zhixingplan.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cfp.zhengqikj.top

[A10] 生成随机数
来源：http://qqb.sysykeji.top

Py:   import random; random.randint(1, 100)
来源：http://mpz.yueranfly.top

PHP:  random_int(1, 100);
来源：http://qgv.pycfn.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://abp.fehbvm.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dgq.hnqzz.top

Java: new Random().nextInt(100) + 1
来源：http://qpe.feifeiyinyue.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zrw.cheryme.top

Ruby: rand(1..100)
来源：http://vgm.hcnkem.com

C#:   new Random().Next(1, 101)
来源：http://jpo.chenjidiqi.icu

[A11] 条件表达式（三元）
来源：http://pos.gotoacloud.top

Py:   "yes" if x > 0 else "no"
来源：http://vxt.ehwqpu.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://gfd.gogol.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://mbh.yuanzhike.top

TS:   x > 0 ? "yes" : "no"
来源：http://fke.shangyingyoupin.top

Java: x > 0 ? "yes" : "no"
来源：http://xqe.snrcjt.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://sru.zhijiandao.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://esg.jinqigufen.top

C#:   x > 0 ? "yes" : "no"
来源：http://kmj.shanyushiyangtech.top

[A12] 字符串插值 / 格式化
来源：http://ukd.0kj1m.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://krx.dianchejie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zux.jinyuanbaomall.cn

JS:   `Hello, ${name}!`
来源：http://vkf.zdbjq.cn

TS:   `Hello, ${name}!`
来源：http://hrr.pycfn.com

Java: "Hello, %s!".formatted(name)
来源：http://oox.cheryme.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vwp.kuanghao11.cn

Ruby: "Hello, #{name}!"
来源：http://txq.aibaodan.cn

C#:   $"Hello, {name}!"
来源：http://fgo.yfazqb.com

[A13] 多行字符串（练习 \n 转义）
来源：http://ucy.jianghu66.top

Py:   "第一行\n第二行"
来源：http://auv.xuetiantiany.cn

PHP:  "第一行\n第二行"
来源：http://yaz.sweek.top

JS:   "第一行\n第二行"
来源：http://sqz.tian-w.cn

TS:   "第一行\n第二行"
来源：http://gll.chenjidiqi.icu

Java: "第一行\n第二行"
来源：http://fnb.quarkkingdee.top

Go:   "第一行\n第二行"
来源：http://yuy.zycfv.cn

Ruby: "第一行\n第二行"
来源：http://vee.yuanzhike.top

C#:   "第一行\n第二行"
来源：http://zzz.0kj1m.cn

[A14] 注释写法
来源：http://qih.iojbl.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://dke.chenlongwang.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://lua.tian-w.cn

JS:   // 单行；/* 多行 */
来源：http://jhu.316326.xyz

TS:   // 单行；/* 多行 */
来源：http://cnw.sxryk.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ndu.kuanghao11.cn

Go:   // 单行；/* 多行 */
来源：http://yfn.nwbrower.top

Ruby: # 单行；=begin 多行 =end
来源：http://czm.haohaochexian.top

C#:   // 单行；/* 多行 */
来源：http://rvk.zhengqikj.top

[A15] 空值判断与默认值
来源：http://toa.gotoacloud.top

Py:   value = data or "默认值"
来源：http://diq.vqdsnc.cn

PHP:  $value = $data ?? "默认值";
来源：http://sbp.fktsv.cn

JS:   const value = data ?? "默认值";
来源：http://vcr.yfazqb.com

TS:   const value = data ?? "默认值";
来源：http://kua.hesvh.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://peq.shzxlz.cn

Go:   if data == "" { data = "默认值" }
来源：http://lxy.yangfankeji.com

Ruby: value = data || "默认值"
来源：http://jbb.jinyuanbaomall.cn

C#:   var value = data ?? "默认值";
来源：http://num.zhengqikj.top

[A16] 真假值判断规则
来源：http://eed.shzxlz.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zqf.xinyue.icu

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pzc.fzhhl.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wai.kuanghao11.cn

TS:   if (!x) {}
来源：http://kug.gotoacloud.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kih.jinghuilouyu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rxq.jqgufenzy.top

Ruby: unless x            # nil 与 false 为假
来源：http://dhl.fktsv.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ayo.aibaodan.cn

[A17] 位运算
来源：http://lcd.nanxuanxn.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qaf.xuanzx.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jse.smart0.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ofv.jlsjyb.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cki.yonumen.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vks.hesvh.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fts.vqdsnc.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xyx.shanyushiyangtech.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xsi.zycfv.cn

[A18] 字符与 ASCII 码互转
来源：http://ggf.zycfv.cn

Py:   ord("A"); chr(65)
来源：http://pdw.xziqi.cn

PHP:  ord("A"); chr(65)
来源：http://nma.zhiwuduotai.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gsi.0kj1m.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bfd.birdmap.top

Java: (int) 'A'; (char) 65
来源：http://vcl.cqqwz.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zzk.ehwqpu.com

Ruby: "A".ord; 65.chr
来源：http://hom.jinqigufen.top

C#:   (int)'A'; (char)65
来源：http://ebu.yj20258.top

[A19] 交换两个变量
来源：http://zgf.tian-w.cn

Py:   a, b = b, a
来源：http://igy.yongpay.top

PHP:  [$a, $b] = [$b, $a];
来源：http://aci.guowangkeji.top

JS:   [a, b] = [b, a];
来源：http://jkk.jqgufenzy.top

TS:   [a, b] = [b, a];
来源：http://ibw.sxryk.cn

Java: int t = a; a = b; b = t;
来源：http://pxk.ppjwa.cn

Go:   a, b = b, a
来源：http://upv.yvedp.cn

Ruby: a, b = b, a
来源：http://peg.vqdsnc.cn

C#:   (a, b) = (b, a);
来源：http://mwg.jqgfzy.top

[A20] 读取标准输入
来源：http://lnn.316326.xyz

Py:   name = input("请输入：")
来源：http://htg.c1oappe.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ots.jqgufenzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wwk.shangyingyoupin.top

TS:   // Node.js：readline 模块
来源：http://qyt.gzhubu.top

Java: new Scanner(System.in).nextLine()
来源：http://agj.aizwys.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rfk.yonumen.top

Ruby: gets.chomp
来源：http://iww.wangshuangyany.cn

C#:   Console.ReadLine();
来源：http://jcm.zdqjudy.top

[A21] 保留指定小数位输出
来源：http://ktp.yuxming.cn

Py:   f"{3.14159:.2f}"
来源：http://ckd.zhoulong.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hkm.gotoacloud.top

JS:   (3.14159).toFixed(2)
来源：http://riu.gaohongyu789.top

TS:   (3.14159).toFixed(2)
来源：http://fog.sysykeji.top

Java: String.format("%.2f", 3.14159)
来源：http://vmw.fengsongda.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://isv.snrcjt.cn

Ruby: format("%.2f", 3.14159)
来源：http://www.xziqi.cn

C#:   3.14159.ToString("F2")
来源：http://mgo.mhx1999.top

[A22] 获取字符串长度
来源：http://zxo.guannengcc.top

Py:   len(s)
来源：http://drl.ydjk.org.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xym.tian-w.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ncn.ydjk.org.cn

TS:   s.length
来源：http://gqx.guannengcc.top

Java: s.length()
来源：http://vhr.vehdjk.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zzq.epnwcf.com

Ruby: s.length
来源：http://egg.cdnleiting.top

C#:   s.Length
来源：http://gve.hfpthk.cn

[A23] 大小写转换
来源：http://lpx.vehdjk.com

Py:   s.upper(); s.lower(); s.title()
来源：http://xxk.yuanzhike.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://szo.sufxvd.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://htw.yj20258.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://btu.yonumen.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vbg.iojbl.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xmp.yvedp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bpw.cheryme.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ipg.chenjidiqi.icu

[A24] 去除首尾空白
来源：http://zte.yuxming.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gmx.yvedp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://elx.smart0.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nds.chenzaomai.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pps.xuetiantiany.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ods.gaohongyu789.top

Go:   strings.TrimSpace(s)
来源：http://qfw.nanxinkj.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fmr.vehdjk.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wyc.hfpthk.cn

[A25] 字符串比较
来源：http://imv.xuanzx.com

Py:   s1 == s2; s1 != s2
来源：http://tjw.andypj.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yxe.daria6918.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uff.shanyushiyangkeji.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://twg.ydzc1.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://roq.svipenyu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nxx.316326.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://jmm.smart0.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vwl.hcnkem.com

[A26] 类型转换总览
来源：http://fzk.hfpthk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uui.havefunace.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cch.sufxvd.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nxk.jinqigufen.top

TS:   Number() String() Boolean() x as number
来源：http://dvq.svipenyu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hmv.dashuyun.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kly.iojbl.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ulu.zhoulong.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jbq.yfazqb.com

================================================================================
来源：http://qvi.cashguo.top

B. 流程控制
来源：http://dig.ehwqpu.com

================================================================================
来源：http://rcp.yuxming.cn

[B01] 条件判断 if / else
来源：http://lnw.jiagoushi.top

Py:   result = "正" if x > 0 else "非正"
来源：http://dea.chenzaomai.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kwv.0kj1m.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pus.wangshuangyany.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tzk.zdbjq.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vvb.cqqwz.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rhk.zdbjq.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zcg.zhengqikj.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ezj.zdqjudy.top

[B02] 多分支 else if / elif
来源：http://smz.52xcode.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dju.jianghu66.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ova.svipenyu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://emc.haohaochexian.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xzj.andypj.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://buv.hnxiangtu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ltu.aibaodan.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cth.hysaishi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tdu.yj20258888.top

[B03] switch / match / case
来源：http://iri.fehbvm.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://atp.yueranfly.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xmj.kuanghao11.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xwo.ybcxt.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pzm.sxryk.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://opa.xingfuxueyuan.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tlo.chenzaomai.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rbe.pengpengdd.cyou

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mft.gzhubu.top

[B04] for 计数循环
来源：http://hxv.yj202588.top

Py:   for i in range(10): print(i)
来源：http://ejg.jinyuanbaomall.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://frm.shangyingyoupin.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mui.cucudq.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lwp.shanyushiyangkeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qwi.shzxlz.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iwz.cheryme.top

Ruby: 10.times { |i| puts i }
来源：http://cha.0kj1m.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jgu.chenlongwang.top

[B05] 遍历数组 / 列表
来源：http://hnw.fanxiaobao.xyz

Py:   for item in arr: print(item)
来源：http://kwp.xingfuxueyuan.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vhy.hongshengwenyu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://nwn.jqgfzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://eqo.mhx1999.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tpr.jinyuanbaomall.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gub.fengsongda.top

Ruby: arr.each { |item| puts item }
来源：http://lwi.chenlongwang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jve.xziqi.cn

[B06] 遍历字典 / 对象
来源：http://hbc.feifeiyinyue.top

Py:   for k, v in d.items(): print(k, v)
来源：http://bju.jqgfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fyu.vqdsnc.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jtp.0kj1m.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gzw.zhixingplan.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zwr.xuetiantiany.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tcz.jyoumei.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hua.quarkkingdee.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dfu.zhiwuduotai.top

[B07] while 循环
来源：http://cok.yanxiufei.cn

Py:   while i < 10: i += 1
来源：http://cei.zhongyouzk.top

PHP:  while ($i < 10) { $i++; }
来源：http://jla.ydjk.org.cn

JS:   while (i < 10) { i++; }
来源：http://kdw.epnwcf.com

TS:   while (i < 10) { i++; }
来源：http://kpw.jinghuilouyu.cn

Java: while (i < 10) { i++; }
来源：http://hli.xinyue.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tgi.yuxming.cn

Ruby: while i < 10; i += 1; end
来源：http://iwu.daxiang520.top

C#:   while (i < 10) { i++; }
来源：http://uyv.yj202588.top

[B08] do-while（至少执行一次）
来源：http://mnv.jqgufenzy.top

Py:   # 无 do-while：用 while True + break
来源：http://gqr.ywan-chungtsiang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://quf.birdmap.top

JS:   do { i++; } while (i < 10);
来源：http://pgi.ehwqpu.com

TS:   do { i++; } while (i < 10);
来源：http://fwc.aizwys.cn

Java: do { i++; } while (i < 10);
来源：http://igw.chenlongwang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://erd.sxryk.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pgk.tianlin.xyz

C#:   do { i++; } while (i < 10);
来源：http://znw.jinghuilouyu.cn


<!-- 参考信息 -->