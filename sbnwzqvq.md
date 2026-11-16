代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://ioq.sysykeji.top

[A03] 常量定义
来源：http://pwz.hammf.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://oyb.c1oappe.top

PHP:  const PI = 3.14159;
来源：http://qhw.xuanzx.com

JS:   const PI = 3.14159;
来源：http://bpi.guannengcc.top

TS:   const PI: number = 3.14159;
来源：http://bhw.jyoumei.cn

Java: static final double PI = 3.14159;
来源：http://noy.zhaomingkeji.xyz

Go:   const PI = 3.14159
来源：http://sti.wangshuangyany.cn

Ruby: PI = 3.14159
来源：http://mbz.aibaodan.cn

C#:   const double PI = 3.14159;
来源：http://zfr.guowangkeji.top

[A04] 判断变量类型
来源：http://nbk.quarkkingdee.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://sdk.yangfankeji.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xwq.feifeiyinyue.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bzv.haohaochexian.top

TS:   typeof x; x instanceof Date
来源：http://thv.cheryme.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lke.nwbrower.top

Go:   reflect.TypeOf(x).Name()
来源：http://tac.xinyue.icu

Ruby: x.class; x.is_a?(Integer)
来源：http://kwj.chenjidiqi.icu

C#:   x.GetType().Name; x is int
来源：http://hwg.nanxuanxn.top

[A05] 整数除法与取模
来源：http://irk.gotoacloud.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sua.c1oappe.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://tjq.sweek.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zds.gaohongyu789.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://raq.fzhhl.top

Java: 7 / 2; 7 % 2
来源：http://fem.cqqwz.cn

Go:   7 / 2; 7 % 2
来源：http://jqf.316326.xyz

Ruby: 7 / 2; 7 % 2
来源：http://kko.aibaodan.cn

C#:   7 / 2; 7 % 2
来源：http://ijx.pengpengdd.cyou

[A06] 字符串转数字
来源：http://aej.daxiang520.top

Py:   int("42"); float("3.14")
来源：http://ulx.jinqigufen.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kad.pycfn.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://viz.ivvv.top

TS:   parseInt("42", 10); Number("42")
来源：http://wpw.aibaodan.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://toi.tian-w.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xfv.yanxiufei.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zly.hysaishi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://usv.vqdsnc.cn

[A07] 数字转字符串
来源：http://auh.shangyingyoupin.top

Py:   str(42)
来源：http://bmo.uphjek.com

PHP:  (string) 42; strval(42)
来源：http://vel.yj202588.top

JS:   String(42); (42).toString()
来源：http://gba.hywenlv.cn

TS:   String(42)
来源：http://hgz.wangshuangyany.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ias.andypj.xyz

Go:   strconv.Itoa(42)
来源：http://vsz.kuanghao11.cn

Ruby: 42.to_s
来源：http://kvh.9152youxi.cn

C#:   42.ToString()
来源：http://kax.jqgufenzy.top

[A08] 取整与四舍五入
来源：http://uyj.yueranfly.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mdi.zycfv.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://obq.cucudq.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vwn.sysykeji.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://uqd.yueranfly.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nek.hongshengwenyu.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zez.daxiang520.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://bfg.tian-w.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://iqs.hywenlv.cn

[A09] 绝对值与最大最小值
来源：http://ugy.tarul.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mfe.jiagoushi.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://arh.jqgfzy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yyi.zhoulong.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wih.chenzaomai.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tyd.zhixingplan.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://don.pengpengdd.cyou

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lzz.sxryk.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mik.mhx1999.top

[A10] 生成随机数
来源：http://uey.xziqi.cn

Py:   import random; random.randint(1, 100)
来源：http://fmi.yueranfly.top

PHP:  random_int(1, 100);
来源：http://dck.epnwcf.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rdv.zhaomingkeji.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mbl.yj202588.top

Java: new Random().nextInt(100) + 1
来源：http://dnt.hongshengwenyu.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qzg.cdnleiting.top

Ruby: rand(1..100)
来源：http://zwk.aibaodan.cn

C#:   new Random().Next(1, 101)
来源：http://ooa.hcnkem.com

[A11] 条件表达式（三元）
来源：http://bip.jiagoushi.top

Py:   "yes" if x > 0 else "no"
来源：http://gbq.gaohongyu789.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://mhd.hysaishi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qtq.yj20258888.top

TS:   x > 0 ? "yes" : "no"
来源：http://wap.nanxinkj.top

Java: x > 0 ? "yes" : "no"
来源：http://cut.jyoumei.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://faq.uphjek.com

Ruby: x > 0 ? "yes" : "no"
来源：http://eqe.zycfv.cn

C#:   x > 0 ? "yes" : "no"
来源：http://nbd.tarul.cn

[A12] 字符串插值 / 格式化
来源：http://qsm.shzxlz.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gtu.gogol.net.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tzn.bbcook.cn

JS:   `Hello, ${name}!`
来源：http://vgi.fanxiaobao.xyz

TS:   `Hello, ${name}!`
来源：http://qln.xylfe.cn

Java: "Hello, %s!".formatted(name)
来源：http://lzt.tarul.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://uji.nanxinkj.top

Ruby: "Hello, #{name}!"
来源：http://xru.shzxlz.cn

C#:   $"Hello, {name}!"
来源：http://ncy.jiagoushi.top

[A13] 多行字符串（练习 \n 转义）
来源：http://mnx.vqdsnc.cn

Py:   "第一行\n第二行"
来源：http://fsv.yvedp.cn

PHP:  "第一行\n第二行"
来源：http://jzx.ehwqpu.com

JS:   "第一行\n第二行"
来源：http://ojf.jinghuilouyu.cn

TS:   "第一行\n第二行"
来源：http://swg.vehdjk.com

Java: "第一行\n第二行"
来源：http://vwu.hnqzz.top

Go:   "第一行\n第二行"
来源：http://kok.yvedp.cn

Ruby: "第一行\n第二行"
来源：http://jlr.jqgfzy.top

C#:   "第一行\n第二行"
来源：http://mfe.fktsv.cn

[A14] 注释写法
来源：http://eww.tianlin.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://efu.aizwys.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://svy.dianchejie.cn

JS:   // 单行；/* 多行 */
来源：http://fmi.yfazqb.com

TS:   // 单行；/* 多行 */
来源：http://bba.tarul.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ijr.tianlin.xyz

Go:   // 单行；/* 多行 */
来源：http://tia.sufxvd.cn

Ruby: # 单行；=begin 多行 =end
来源：http://oqk.cashguo.top

C#:   // 单行；/* 多行 */
来源：http://zqg.daxiang520.top

[A15] 空值判断与默认值
来源：http://vfc.yuxming.cn

Py:   value = data or "默认值"
来源：http://dos.redwolf501.top

PHP:  $value = $data ?? "默认值";
来源：http://zgr.nwbrower.top

JS:   const value = data ?? "默认值";
来源：http://tqn.quarkkingdee.top

TS:   const value = data ?? "默认值";
来源：http://tvq.redwolf501.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://foi.zycfv.cn

Go:   if data == "" { data = "默认值" }
来源：http://peo.xziqi.cn

Ruby: value = data || "默认值"
来源：http://sjj.xuanzx.com

C#:   var value = data ?? "默认值";
来源：http://wyp.hywenlv.cn

[A16] 真假值判断规则
来源：http://apn.aibaodan.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://eyf.aizwys.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vvg.redwolf501.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rdm.bjfxy.top

TS:   if (!x) {}
来源：http://lyb.bbcook.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://osb.hammf.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://the.jinqigfzy.top

Ruby: unless x            # nil 与 false 为假
来源：http://vbw.jqgfzy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hzr.yangfankeji.com

[A17] 位运算
来源：http://kee.fktsv.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gyj.gzhubu.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vxz.ydjk.org.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://shf.shuidangran.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nwn.shzxlz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lif.jinqigfzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bnp.havefunace.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vij.bbcook.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oca.jinqigufen.top

[A18] 字符与 ASCII 码互转
来源：http://jta.haohaochexian.top

Py:   ord("A"); chr(65)
来源：http://kck.jyoumei.cn

PHP:  ord("A"); chr(65)
来源：http://syg.yanxiufei.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tlh.vehdjk.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rwr.zhoulong.xyz

Java: (int) 'A'; (char) 65
来源：http://hvw.hywenlv.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hfn.andypj.xyz

Ruby: "A".ord; 65.chr
来源：http://pgt.vehdjk.com

C#:   (int)'A'; (char)65
来源：http://kbf.yonumen.top

[A19] 交换两个变量
来源：http://zfn.zhixingplan.top

Py:   a, b = b, a
来源：http://zil.yangfankeji.com

PHP:  [$a, $b] = [$b, $a];
来源：http://eur.chenjidiqi.icu

JS:   [a, b] = [b, a];
来源：http://yxo.aizwys.cn

TS:   [a, b] = [b, a];
来源：http://wpf.jiagoushi.top

Java: int t = a; a = b; b = t;
来源：http://bsm.cdnleiting.top

Go:   a, b = b, a
来源：http://pdk.daxiang520.top

Ruby: a, b = b, a
来源：http://vye.hammf.cn

C#:   (a, b) = (b, a);
来源：http://zwf.meibo888.top

[A20] 读取标准输入
来源：http://aot.havefunace.top

Py:   name = input("请输入：")
来源：http://shp.jianghu66.top

PHP:  $name = trim(fgets(STDIN));
来源：http://rvs.ctjpmb.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cje.jinghuilouyu.cn

TS:   // Node.js：readline 模块
来源：http://lqd.yuxming.cn

Java: new Scanner(System.in).nextLine()
来源：http://ujr.sysykeji.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ehn.hfpthk.cn

Ruby: gets.chomp
来源：http://oai.sysykeji.top

C#:   Console.ReadLine();
来源：http://qdh.zhixingplan.top

[A21] 保留指定小数位输出
来源：http://djn.c1oappe.top

Py:   f"{3.14159:.2f}"
来源：http://fzk.yj20258888.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rtv.sweek.top

JS:   (3.14159).toFixed(2)
来源：http://bok.yonumen.top

TS:   (3.14159).toFixed(2)
来源：http://kwl.nanxuanxn.top

Java: String.format("%.2f", 3.14159)
来源：http://nmd.redwolf501.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://erx.aizwys.cn

Ruby: format("%.2f", 3.14159)
来源：http://mqx.yj202588.top

C#:   3.14159.ToString("F2")
来源：http://opc.guowangkeji.top

[A22] 获取字符串长度
来源：http://cvg.chenzaomai.com

Py:   len(s)
来源：http://rkz.hfpthk.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wil.daria6918.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ail.nwbrower.top

TS:   s.length
来源：http://exy.nanxuanxn.top

Java: s.length()
来源：http://ety.vehdjk.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tbr.zhongyouzk.top

Ruby: s.length
来源：http://nuu.wangdashe.top

C#:   s.Length
来源：http://die.sysykeji.top

[A23] 大小写转换
来源：http://jcl.xuetiantiany.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yhc.zdbjq.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://klm.chenlongwang.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rvk.smart0.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jzx.tian-w.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vwi.zhaomingkeji.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://seq.316326.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ixk.smart0.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://wlh.daria6918.cn

[A24] 去除首尾空白
来源：http://mgb.dianchejie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://clg.wangshuangyany.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ezx.tianlin.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nij.yj202588.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uli.hongshengwenyu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gih.52xcode.cn

Go:   strings.TrimSpace(s)
来源：http://dzt.aibaodan.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dnf.zdbjq.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jkw.zhaomingkeji.xyz

[A25] 字符串比较
来源：http://zem.zhongyouzk.top

Py:   s1 == s2; s1 != s2
来源：http://ckz.sysykeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://she.xingfuxueyuan.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bnp.shanyushiyangkeji.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rrc.zdqjudy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nde.yuanzhike.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yxl.redwolf501.top

Ruby: s1 == s2; s1 <=> s2
来源：http://bgl.wangshuangyany.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dyp.gotoacloud.top

[A26] 类型转换总览
来源：http://snd.iojbl.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zup.shzxlz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bcm.meibo888.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gvc.ivvv.top

TS:   Number() String() Boolean() x as number
来源：http://uas.jlsjyb.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nuo.shangyingyoupin.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tsv.yfazqb.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://crc.yueranfly.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vkz.zycfv.cn

================================================================================
来源：http://twy.andypj.xyz

B. 流程控制
来源：http://yki.guowangkeji.top

================================================================================
来源：http://nxr.fanxiaobao.xyz

[B01] 条件判断 if / else
来源：http://oam.vqdsnc.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://aoy.vqdsnc.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uqx.haohaochexian.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zrq.quarkkingdee.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kkd.ydjk.org.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vmj.snrcjt.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rzd.shangyingyoupin.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kta.zhengqikj.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rlc.birdmap.top

[B02] 多分支 else if / elif
来源：http://qhk.svipenyu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xjz.wangshuangyany.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wtc.316326.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://peb.hcnkem.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hka.fanxiaobao.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://emv.xziqi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jsl.tian-w.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fwg.cheryme.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wey.chenlongwang.top

[B03] switch / match / case
来源：http://hia.shangyingyoupin.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://css.nanxuanxn.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mgl.xinyue.icu

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wog.aibaodan.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vyt.hcnkem.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dcu.zdbjq.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://omz.ppjwa.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wtr.gotoacloud.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fnd.ydzc1.top

[B04] for 计数循环
来源：http://ndu.gogol.net.cn

Py:   for i in range(10): print(i)
来源：http://zhj.sjlbkw.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hsa.yuxming.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xpo.zhongyouzk.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tct.daria6918.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://trm.meibo888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jro.chenlongwang.top

Ruby: 10.times { |i| puts i }
来源：http://xeq.shanyushiyangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ohm.zhengqikj.top

[B05] 遍历数组 / 列表
来源：http://sse.hcnkem.com

Py:   for item in arr: print(item)
来源：http://eth.uphjek.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://czs.yj20258.top

JS:   for (const item of arr) { console.log(item); }
来源：http://wjj.snrcjt.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://avx.jinyuanbaomall.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nwa.gaohongyu789.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zur.cucudq.cn

Ruby: arr.each { |item| puts item }
来源：http://quo.zycfv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wow.ybcxt.top

[B06] 遍历字典 / 对象
来源：http://raa.epnwcf.com

Py:   for k, v in d.items(): print(k, v)
来源：http://cke.jinqigufen.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://onw.yfazqb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xqu.hongshengwenyu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eni.hysaishi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vvt.chenzaomai.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jfy.meibo888.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lym.fanxiaobao.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zul.xziqi.cn

[B07] while 循环
来源：http://tdj.yuanzhike.top

Py:   while i < 10: i += 1
来源：http://rsh.yuanzhike.top

PHP:  while ($i < 10) { $i++; }
来源：http://uie.yj20258888.top

JS:   while (i < 10) { i++; }
来源：http://uub.cucudq.cn

TS:   while (i < 10) { i++; }
来源：http://nlr.jinqigfzy.top

Java: while (i < 10) { i++; }
来源：http://gdx.hfpthk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uiw.0kj1m.cn

Ruby: while i < 10; i += 1; end
来源：http://ytq.xingfuxueyuan.xyz

C#:   while (i < 10) { i++; }
来源：http://agr.pengpengdd.cyou

[B08] do-while（至少执行一次）
来源：http://qal.yongpay.top

Py:   # 无 do-while：用 while True + break
来源：http://eab.hammf.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bsf.hnxiangtu.top

JS:   do { i++; } while (i < 10);
来源：http://bqk.wangdashe.top

TS:   do { i++; } while (i < 10);
来源：http://viy.9152youxi.cn

Java: do { i++; } while (i < 10);
来源：http://ehr.yuxming.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ukv.iojbl.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vnh.fehbvm.com

C#:   do { i++; } while (i < 10);
来源：http://fqz.gzhubu.top

[B09] break 与 continue
来源：http://vsb.yangfankeji.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ied.ybcxt.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jwk.svipenyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cml.ppjwa.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hrx.ctjpmb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kvw.pycfn.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lkm.52xcode.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zuu.wangshuangyany.cn


<!-- 参考信息 -->