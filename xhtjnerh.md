代发 wailian999

Ruby: PI = 3.14159
来源：http://hys.smart0.xyz

C#:   const double PI = 3.14159;
来源：http://shr.yuanzhike.top

[A04] 判断变量类型
来源：http://epg.dashuyun.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ojn.316326.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lrc.cdnleiting.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mxh.xziqi.cn

TS:   typeof x; x instanceof Date
来源：http://ppt.shzxlz.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hie.quarkkingdee.top

Go:   reflect.TypeOf(x).Name()
来源：http://tvv.hysaishi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://bqa.fktsv.cn

C#:   x.GetType().Name; x is int
来源：http://tbu.shzxlz.cn

[A05] 整数除法与取模
来源：http://fza.jqgfzy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ein.zhongyouzk.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://cch.sjlbkw.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cxg.nwbrower.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sal.hywenlv.cn

Java: 7 / 2; 7 % 2
来源：http://kvo.zycfv.cn

Go:   7 / 2; 7 % 2
来源：http://yru.ivvv.top

Ruby: 7 / 2; 7 % 2
来源：http://rgz.zhijiandao.cn

C#:   7 / 2; 7 % 2
来源：http://dqs.uphjek.com

[A06] 字符串转数字
来源：http://ynz.fktsv.cn

Py:   int("42"); float("3.14")
来源：http://ngm.hnqzz.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bcy.havefunace.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kgc.jqgufenzy.top

TS:   parseInt("42", 10); Number("42")
来源：http://vhi.gogol.net.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ypr.mhx1999.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://upj.jqgufenzy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://bhj.zycfv.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dnq.redwolf501.top

[A07] 数字转字符串
来源：http://jbo.fzhhl.top

Py:   str(42)
来源：http://wge.meibo888.top

PHP:  (string) 42; strval(42)
来源：http://lvh.zdqjudy.top

JS:   String(42); (42).toString()
来源：http://tkf.mhx1999.top

TS:   String(42)
来源：http://grd.yfazqb.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://nww.smart0.xyz

Go:   strconv.Itoa(42)
来源：http://czw.0kj1m.cn

Ruby: 42.to_s
来源：http://ifs.jinqigfzy.top

C#:   42.ToString()
来源：http://vxh.uphjek.com

[A08] 取整与四舍五入
来源：http://fzy.nanxuanxn.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xnr.cqqwz.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zlp.uphjek.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://oaa.tarul.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rpj.0kj1m.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://eoh.dashuyun.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fii.shzxlz.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fez.haohaochexian.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gbj.bbcook.cn

[A09] 绝对值与最大最小值
来源：http://kgg.ydjk.org.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://laq.yangfankeji.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ime.yj202588.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mbq.vehdjk.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bim.aibaodan.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tfe.jiagoushi.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hta.ydzc1.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vln.aizwys.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ror.yuxming.cn

[A10] 生成随机数
来源：http://zcy.yonumen.top

Py:   import random; random.randint(1, 100)
来源：http://etf.hfpthk.cn

PHP:  random_int(1, 100);
来源：http://xua.vqdsnc.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://duf.yj20258.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qar.vehdjk.com

Java: new Random().nextInt(100) + 1
来源：http://qin.haohaochexian.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qtx.birdmap.top

Ruby: rand(1..100)
来源：http://ufd.jinyuanbaomall.cn

C#:   new Random().Next(1, 101)
来源：http://usx.nanxinkj.top

[A11] 条件表达式（三元）
来源：http://fdu.gotoacloud.top

Py:   "yes" if x > 0 else "no"
来源：http://zas.jinqigfzy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://zym.jlsjyb.cn

JS:   x > 0 ? "yes" : "no"
来源：http://som.feifeiyinyue.top

TS:   x > 0 ? "yes" : "no"
来源：http://jzo.gotoacloud.top

Java: x > 0 ? "yes" : "no"
来源：http://tga.0kj1m.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://cri.ydjk.org.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ofd.fehbvm.com

C#:   x > 0 ? "yes" : "no"
来源：http://nia.andypj.xyz

[A12] 字符串插值 / 格式化
来源：http://hqz.bjfxy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xgk.daxiang520.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kbd.jqgfzy.top

JS:   `Hello, ${name}!`
来源：http://had.gotoacloud.top

TS:   `Hello, ${name}!`
来源：http://yiu.quarkkingdee.top

Java: "Hello, %s!".formatted(name)
来源：http://qkk.tian-w.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mts.yj202588.top

Ruby: "Hello, #{name}!"
来源：http://zsx.meibo888.top

C#:   $"Hello, {name}!"
来源：http://sbu.daxiang520.top

[A13] 多行字符串（练习 \n 转义）
来源：http://eeh.yangfankeji.com

Py:   "第一行\n第二行"
来源：http://exv.jqgufenzy.top

PHP:  "第一行\n第二行"
来源：http://mgt.epnwcf.com

JS:   "第一行\n第二行"
来源：http://dts.daria6918.cn

TS:   "第一行\n第二行"
来源：http://enq.yueranfly.top

Java: "第一行\n第二行"
来源：http://jnz.yongpay.top

Go:   "第一行\n第二行"
来源：http://wvt.zhoulong.xyz

Ruby: "第一行\n第二行"
来源：http://cwb.jiagoushi.top

C#:   "第一行\n第二行"
来源：http://kfy.ywan-chungtsiang.top

[A14] 注释写法
来源：http://ios.kuanghao11.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://duw.hongshengwenyu.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://itt.cqqwz.cn

JS:   // 单行；/* 多行 */
来源：http://gbq.yfazqb.com

TS:   // 单行；/* 多行 */
来源：http://gek.zhijiandao.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dle.andypj.xyz

Go:   // 单行；/* 多行 */
来源：http://umn.yueranfly.top

Ruby: # 单行；=begin 多行 =end
来源：http://nxs.jinyuanbaomall.cn

C#:   // 单行；/* 多行 */
来源：http://qjh.guannengcc.top

[A15] 空值判断与默认值
来源：http://qgd.svipenyu.cn

Py:   value = data or "默认值"
来源：http://rrv.pengpengdd.cyou

PHP:  $value = $data ?? "默认值";
来源：http://omh.cucudq.cn

JS:   const value = data ?? "默认值";
来源：http://zbo.wangshuangyany.cn

TS:   const value = data ?? "默认值";
来源：http://dfw.smart0.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://roc.yanxiufei.cn

Go:   if data == "" { data = "默认值" }
来源：http://gmb.ybcxt.top

Ruby: value = data || "默认值"
来源：http://uzm.guowangkeji.top

C#:   var value = data ?? "默认值";
来源：http://nzv.gotoacloud.top

[A16] 真假值判断规则
来源：http://opo.guowangkeji.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nqx.hywenlv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bjr.sufxvd.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ixc.daria6918.cn

TS:   if (!x) {}
来源：http://nxm.ydzc1.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mbh.guowangkeji.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hkv.iojbl.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gyv.aizwys.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dvy.tian-w.cn

[A17] 位运算
来源：http://qvd.gotoacloud.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gad.shuidangran.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nfw.tianlin.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mfk.yongpay.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://aox.fzhhl.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://upu.fanxiaobao.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dyf.haohaochexian.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zjy.jyoumei.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ctq.haohaochexian.top

[A18] 字符与 ASCII 码互转
来源：http://hkr.sxryk.cn

Py:   ord("A"); chr(65)
来源：http://dzk.jqgfzy.top

PHP:  ord("A"); chr(65)
来源：http://knm.nanxuanxn.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sqi.pengpengdd.cyou

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qox.yuxming.cn

Java: (int) 'A'; (char) 65
来源：http://evi.aibaodan.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tvs.hywenlv.cn

Ruby: "A".ord; 65.chr
来源：http://dbr.ivvv.top

C#:   (int)'A'; (char)65
来源：http://yvg.redwolf501.top

[A19] 交换两个变量
来源：http://xje.zhoulong.xyz

Py:   a, b = b, a
来源：http://wlf.shangyingyoupin.top

PHP:  [$a, $b] = [$b, $a];
来源：http://nag.jqgufenzy.top

JS:   [a, b] = [b, a];
来源：http://iph.ydzc1.top

TS:   [a, b] = [b, a];
来源：http://ues.zhaomingkeji.xyz

Java: int t = a; a = b; b = t;
来源：http://unf.havefunace.top

Go:   a, b = b, a
来源：http://ehx.yuxming.cn

Ruby: a, b = b, a
来源：http://upu.haohaochexian.top

C#:   (a, b) = (b, a);
来源：http://bei.hysaishi.cn

[A20] 读取标准输入
来源：http://zxo.sjlbkw.cn

Py:   name = input("请输入：")
来源：http://aki.havefunace.top

PHP:  $name = trim(fgets(STDIN));
来源：http://uxm.pengpengdd.cyou

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mgb.yonumen.top

TS:   // Node.js：readline 模块
来源：http://adg.9152youxi.cn

Java: new Scanner(System.in).nextLine()
来源：http://hrf.gotoacloud.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hzu.xinyue.icu

Ruby: gets.chomp
来源：http://aje.cashguo.top

C#:   Console.ReadLine();
来源：http://lex.pycfn.com

[A21] 保留指定小数位输出
来源：http://okm.shanyushiyangtech.top

Py:   f"{3.14159:.2f}"
来源：http://ohf.iojbl.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jum.epnwcf.com

JS:   (3.14159).toFixed(2)
来源：http://ixm.hesvh.cn

TS:   (3.14159).toFixed(2)
来源：http://uir.kuanghao11.cn

Java: String.format("%.2f", 3.14159)
来源：http://mtk.uphjek.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pjv.fzhhl.top

Ruby: format("%.2f", 3.14159)
来源：http://iwj.zhiwuduotai.top

C#:   3.14159.ToString("F2")
来源：http://kve.sysykeji.top

[A22] 获取字符串长度
来源：http://ydp.fengsongda.top

Py:   len(s)
来源：http://fhd.316326.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qzf.fanxiaobao.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://asy.yongpay.top

TS:   s.length
来源：http://waz.xuetiantiany.cn

Java: s.length()
来源：http://kel.xinyue.icu

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dwx.gaohongyu789.top

Ruby: s.length
来源：http://zfx.tarul.cn

C#:   s.Length
来源：http://eiv.smart0.xyz

[A23] 大小写转换
来源：http://tsp.jinghuilouyu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lwu.sjlbkw.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ebu.fzhhl.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pjq.redwolf501.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qlj.gaohongyu789.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nhj.sxryk.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://byd.zhaomingkeji.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cxp.xylfe.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://kfq.bbcook.cn

[A24] 去除首尾空白
来源：http://emm.yuxming.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://oyg.cdnleiting.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ibv.tian-w.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uqd.chenlongwang.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nfh.pycfn.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ksu.cucudq.cn

Go:   strings.TrimSpace(s)
来源：http://vkh.svipenyu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://iex.jlsjyb.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://znn.sxryk.cn

[A25] 字符串比较
来源：http://ysq.bbcook.cn

Py:   s1 == s2; s1 != s2
来源：http://hra.shzxlz.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kwq.cqqwz.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://whr.yangfankeji.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://urg.epnwcf.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fyt.jinqigufen.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vyq.xinyue.icu

Ruby: s1 == s2; s1 <=> s2
来源：http://xxa.birdmap.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gmp.52xcode.cn

[A26] 类型转换总览
来源：http://lvy.tarul.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zqu.guannengcc.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gwc.chenjidiqi.icu

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hjy.nwbrower.top

TS:   Number() String() Boolean() x as number
来源：http://bem.sweek.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pou.ydzc1.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fxr.ehwqpu.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://xmj.yueranfly.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ivb.wangshuangyany.cn

================================================================================
来源：http://ogw.ehwqpu.com

B. 流程控制
来源：http://lmd.tianlin.xyz

================================================================================
来源：http://ksu.ehwqpu.com

[B01] 条件判断 if / else
来源：http://rbx.cashguo.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ayu.yongpay.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fme.zhiwuduotai.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ntb.hysaishi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ixf.nanxinkj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://abt.yangfankeji.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fps.ydzc1.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sjf.zhengqikj.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rtn.smart0.xyz

[B02] 多分支 else if / elif
来源：http://kxe.zhaomingkeji.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ttv.uphjek.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cyl.hysaishi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://whs.yanxiufei.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gnb.vehdjk.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ftz.xylfe.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ojy.52xcode.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://myp.hnqzz.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://efl.haohaochexian.top

[B03] switch / match / case
来源：http://dhn.kuanghao11.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mhy.dashuyun.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gsr.svipenyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qrd.yuxming.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oyd.fanxiaobao.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pur.zhengqikj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cca.nwbrower.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wfk.yj20258888.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zuf.snrcjt.cn

[B04] for 计数循环
来源：http://vbc.yueranfly.top

Py:   for i in range(10): print(i)
来源：http://bzr.dashuyun.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hvv.hysaishi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cpn.chenjidiqi.icu

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zhu.meibo888.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://whc.shzxlz.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://git.jiagoushi.top

Ruby: 10.times { |i| puts i }
来源：http://zqa.guowangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tsb.hcnkem.com

[B05] 遍历数组 / 列表
来源：http://dtg.tianlin.xyz

Py:   for item in arr: print(item)
来源：http://dld.redwolf501.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nem.xziqi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zey.birdmap.top

TS:   for (const item of arr) { console.log(item); }
来源：http://inh.shanyushiyangtech.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fne.jqgufenzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rug.yj20258.top

Ruby: arr.each { |item| puts item }
来源：http://fwq.jiagoushi.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vaf.havefunace.top

[B06] 遍历字典 / 对象
来源：http://lbs.zhijiandao.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://egi.hcnkem.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uhm.meibo888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wfk.daria6918.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tgb.guannengcc.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hkc.xylfe.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qlb.hnqzz.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wic.52xcode.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hvz.sufxvd.cn

[B07] while 循环
来源：http://apr.shanyushiyangkeji.top

Py:   while i < 10: i += 1
来源：http://nde.dianchejie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dmw.iojbl.cn

JS:   while (i < 10) { i++; }
来源：http://oey.pengpengdd.cyou

TS:   while (i < 10) { i++; }
来源：http://vpf.redwolf501.top

Java: while (i < 10) { i++; }
来源：http://igr.guannengcc.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rvr.hfpthk.cn

Ruby: while i < 10; i += 1; end
来源：http://tcf.jinqigfzy.top

C#:   while (i < 10) { i++; }
来源：http://lbh.cdnleiting.top

[B08] do-while（至少执行一次）
来源：http://oqj.hesvh.cn

Py:   # 无 do-while：用 while True + break
来源：http://tjd.yj20258888.top

PHP:  do { $i++; } while ($i < 10);
来源：http://mlc.jqgfzy.top

JS:   do { i++; } while (i < 10);
来源：http://osh.zycfv.cn

TS:   do { i++; } while (i < 10);
来源：http://xdd.yj202588.top

Java: do { i++; } while (i < 10);
来源：http://nor.jinqigufen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ulo.jinyuanbaomall.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zir.tarul.cn

C#:   do { i++; } while (i < 10);
来源：http://yrs.zycfv.cn

[B09] break 与 continue
来源：http://cak.hfpthk.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jvp.guannengcc.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yog.52xcode.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vpq.hesvh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://syl.sweek.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dlc.cdnleiting.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://axn.hcnkem.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dty.jlsjyb.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nau.fktsv.cn

[B10] 遍历同时拿索引
来源：http://ump.guannengcc.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zuv.shangyingyoupin.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tco.guannengcc.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gxb.xuetiantiany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://aom.fktsv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hli.shanyushiyangtech.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gbj.guowangkeji.top


<!-- 参考信息 -->