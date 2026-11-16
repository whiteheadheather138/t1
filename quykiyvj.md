代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://cft.xingfuxueyuan.xyz

[A03] 常量定义
来源：http://uyb.nanxinkj.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vkh.hammf.cn

PHP:  const PI = 3.14159;
来源：http://qqd.sufxvd.cn

JS:   const PI = 3.14159;
来源：http://gww.0kj1m.cn

TS:   const PI: number = 3.14159;
来源：http://etf.ydjk.org.cn

Java: static final double PI = 3.14159;
来源：http://erf.yj20258.top

Go:   const PI = 3.14159
来源：http://jbt.meibo888.top

Ruby: PI = 3.14159
来源：http://etx.zdqjudy.top

C#:   const double PI = 3.14159;
来源：http://fhb.dianchejie.cn

[A04] 判断变量类型
来源：http://sxh.cashguo.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://zcj.bjfxy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yiu.zhongyouzk.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yqm.ydjk.org.cn

TS:   typeof x; x instanceof Date
来源：http://bjz.svipenyu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://oap.nanxuanxn.top

Go:   reflect.TypeOf(x).Name()
来源：http://zdh.fengsongda.top

Ruby: x.class; x.is_a?(Integer)
来源：http://fmt.hesvh.cn

C#:   x.GetType().Name; x is int
来源：http://xrg.guannengcc.top

[A05] 整数除法与取模
来源：http://qvz.uphjek.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://uaq.andypj.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://ygd.bbcook.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wsf.yuanzhike.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zca.bbcook.cn

Java: 7 / 2; 7 % 2
来源：http://lce.quarkkingdee.top

Go:   7 / 2; 7 % 2
来源：http://wis.shzxlz.cn

Ruby: 7 / 2; 7 % 2
来源：http://mny.ehwqpu.com

C#:   7 / 2; 7 % 2
来源：http://lnh.guowangkeji.top

[A06] 字符串转数字
来源：http://hxw.hcnkem.com

Py:   int("42"); float("3.14")
来源：http://uos.zhiwuduotai.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wdp.fanxiaobao.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qiy.sweek.top

TS:   parseInt("42", 10); Number("42")
来源：http://hhk.jinyuanbaomall.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mns.mhx1999.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wey.cdnleiting.top

Ruby: "42".to_i; "3.14".to_f
来源：http://oty.ywan-chungtsiang.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bzo.shuidangran.top

[A07] 数字转字符串
来源：http://gvr.shangyingyoupin.top

Py:   str(42)
来源：http://ygr.jinqigfzy.top

PHP:  (string) 42; strval(42)
来源：http://lbl.uphjek.com

JS:   String(42); (42).toString()
来源：http://vzy.vehdjk.com

TS:   String(42)
来源：http://cex.hcnkem.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://whi.tian-w.cn

Go:   strconv.Itoa(42)
来源：http://jxm.jinghuilouyu.cn

Ruby: 42.to_s
来源：http://oeh.yj20258.top

C#:   42.ToString()
来源：http://fsi.shanyushiyangkeji.top

[A08] 取整与四舍五入
来源：http://qka.meibo888.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bib.ydjk.org.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xjx.ybcxt.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ifc.hnxiangtu.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lwe.tanke756.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://znu.nwbrower.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fkm.ybcxt.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://edj.zdqjudy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qkf.havefunace.top

[A09] 绝对值与最大最小值
来源：http://tpi.kuanghao11.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ptd.yueranfly.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://exj.fehbvm.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ait.gogol.net.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://snx.nwbrower.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pyg.shanyushiyangtech.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ons.yj20258.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fky.guannengcc.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fdr.gaohongyu789.top

[A10] 生成随机数
来源：http://zem.gaohongyu789.top

Py:   import random; random.randint(1, 100)
来源：http://qhz.gotoacloud.top

PHP:  random_int(1, 100);
来源：http://qhw.nwbrower.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wer.jqgfzy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tvp.yj202588.top

Java: new Random().nextInt(100) + 1
来源：http://uqg.xylfe.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vpw.birdmap.top

Ruby: rand(1..100)
来源：http://phq.guowangkeji.top

C#:   new Random().Next(1, 101)
来源：http://pdb.nanxinkj.top

[A11] 条件表达式（三元）
来源：http://vfa.sufxvd.cn

Py:   "yes" if x > 0 else "no"
来源：http://pki.birdmap.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://apb.guowangkeji.top

JS:   x > 0 ? "yes" : "no"
来源：http://poz.vqdsnc.cn

TS:   x > 0 ? "yes" : "no"
来源：http://glg.cucudq.cn

Java: x > 0 ? "yes" : "no"
来源：http://oym.aibaodan.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fds.52xcode.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://cts.jqgfzy.top

C#:   x > 0 ? "yes" : "no"
来源：http://vxx.cucudq.cn

[A12] 字符串插值 / 格式化
来源：http://kjb.jinqigufen.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nvg.svipenyu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mrt.nwbrower.top

JS:   `Hello, ${name}!`
来源：http://evv.xylfe.cn

TS:   `Hello, ${name}!`
来源：http://bzx.wangdashe.top

Java: "Hello, %s!".formatted(name)
来源：http://ugu.yanxiufei.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fnd.xuetiantiany.cn

Ruby: "Hello, #{name}!"
来源：http://mhy.wangshuangyany.cn

C#:   $"Hello, {name}!"
来源：http://pfu.jqgfzy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ril.aizwys.cn

Py:   "第一行\n第二行"
来源：http://fvb.yfazqb.com

PHP:  "第一行\n第二行"
来源：http://ojx.zdbjq.cn

JS:   "第一行\n第二行"
来源：http://xhy.hnqzz.top

TS:   "第一行\n第二行"
来源：http://wot.andypj.xyz

Java: "第一行\n第二行"
来源：http://dyk.vqdsnc.cn

Go:   "第一行\n第二行"
来源：http://yfp.zhongyouzk.top

Ruby: "第一行\n第二行"
来源：http://yyj.shanyushiyangkeji.top

C#:   "第一行\n第二行"
来源：http://gnz.cheryme.top

[A14] 注释写法
来源：http://fkm.jinyuanbaomall.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://sem.xuanzx.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://adi.feifeiyinyue.top

JS:   // 单行；/* 多行 */
来源：http://yfo.hysaishi.cn

TS:   // 单行；/* 多行 */
来源：http://qmp.pengpengdd.cyou

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://guy.tarul.cn

Go:   // 单行；/* 多行 */
来源：http://okw.haohaochexian.top

Ruby: # 单行；=begin 多行 =end
来源：http://kbz.pengpengdd.cyou

C#:   // 单行；/* 多行 */
来源：http://msm.iojbl.cn

[A15] 空值判断与默认值
来源：http://diq.dianchejie.cn

Py:   value = data or "默认值"
来源：http://jju.cdnleiting.top

PHP:  $value = $data ?? "默认值";
来源：http://eiv.ywan-chungtsiang.top

JS:   const value = data ?? "默认值";
来源：http://cba.jlsjyb.cn

TS:   const value = data ?? "默认值";
来源：http://xqq.shuidangran.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ovx.redwolf501.top

Go:   if data == "" { data = "默认值" }
来源：http://imb.birdmap.top

Ruby: value = data || "默认值"
来源：http://fwh.shanyushiyangkeji.top

C#:   var value = data ?? "默认值";
来源：http://ibt.haohaochexian.top

[A16] 真假值判断规则
来源：http://ine.ydzc1.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kcv.hammf.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gky.ydjk.org.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://abj.daria6918.cn

TS:   if (!x) {}
来源：http://fxc.aizwys.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uhh.dianchejie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pcw.hnqzz.top

Ruby: unless x            # nil 与 false 为假
来源：http://rgg.uphjek.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://clb.wangshuangyany.cn

[A17] 位运算
来源：http://anm.cheryme.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://msw.hysaishi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://asi.zycfv.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wqp.sjlbkw.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jcr.daria6918.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pob.yj20258888.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tvj.xuetiantiany.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yuq.vehdjk.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wbo.ydjk.org.cn

[A18] 字符与 ASCII 码互转
来源：http://kdn.jinghuilouyu.cn

Py:   ord("A"); chr(65)
来源：http://dlo.hnqzz.top

PHP:  ord("A"); chr(65)
来源：http://mtz.sysykeji.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://aib.jinqigufen.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rff.jianghu66.top

Java: (int) 'A'; (char) 65
来源：http://uth.fzhhl.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rqt.fanxiaobao.xyz

Ruby: "A".ord; 65.chr
来源：http://nvv.jyoumei.cn

C#:   (int)'A'; (char)65
来源：http://ylu.vehdjk.com

[A19] 交换两个变量
来源：http://mvp.xziqi.cn

Py:   a, b = b, a
来源：http://vqv.shzxlz.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qqn.gzhubu.top

JS:   [a, b] = [b, a];
来源：http://rxq.fehbvm.com

TS:   [a, b] = [b, a];
来源：http://vxl.birdmap.top

Java: int t = a; a = b; b = t;
来源：http://pwd.yfazqb.com

Go:   a, b = b, a
来源：http://xca.sjlbkw.cn

Ruby: a, b = b, a
来源：http://lmv.0kj1m.cn

C#:   (a, b) = (b, a);
来源：http://vhw.pengpengdd.cyou

[A20] 读取标准输入
来源：http://diu.jqgufenzy.top

Py:   name = input("请输入：")
来源：http://qty.yongpay.top

PHP:  $name = trim(fgets(STDIN));
来源：http://zmj.jianghu66.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://brj.shuidangran.top

TS:   // Node.js：readline 模块
来源：http://ctc.yj20258888.top

Java: new Scanner(System.in).nextLine()
来源：http://pnq.uphjek.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ceu.yongpay.top

Ruby: gets.chomp
来源：http://ghi.quarkkingdee.top

C#:   Console.ReadLine();
来源：http://akr.shangyingyoupin.top

[A21] 保留指定小数位输出
来源：http://iyk.jqgufenzy.top

Py:   f"{3.14159:.2f}"
来源：http://sgd.c1oappe.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kuv.jqgfzy.top

JS:   (3.14159).toFixed(2)
来源：http://mwb.bjfxy.top

TS:   (3.14159).toFixed(2)
来源：http://npa.nwbrower.top

Java: String.format("%.2f", 3.14159)
来源：http://noz.pengpengdd.cyou

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tka.chenzaomai.com

Ruby: format("%.2f", 3.14159)
来源：http://ehl.sweek.top

C#:   3.14159.ToString("F2")
来源：http://jet.chenzaomai.com

[A22] 获取字符串长度
来源：http://wtw.ybcxt.top

Py:   len(s)
来源：http://lmn.redwolf501.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vle.jinyuanbaomall.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mmt.ydzc1.top

TS:   s.length
来源：http://abx.zdbjq.cn

Java: s.length()
来源：http://bdz.pengpengdd.cyou

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lsz.xziqi.cn

Ruby: s.length
来源：http://naj.ctjpmb.com

C#:   s.Length
来源：http://lyz.ywan-chungtsiang.top

[A23] 大小写转换
来源：http://dow.hesvh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tsb.svipenyu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xoj.yuanzhike.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pzr.xziqi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://eac.uphjek.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ujx.redwolf501.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://iks.ctjpmb.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yph.jinqigufen.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ljo.guannengcc.top

[A24] 去除首尾空白
来源：http://dzr.xuanzx.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ebq.sysykeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fux.vqdsnc.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wmv.gzhubu.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zne.yongpay.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sud.wangdashe.top

Go:   strings.TrimSpace(s)
来源：http://qob.pengpengdd.cyou

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zbm.jqgfzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qpg.c1oappe.top

[A25] 字符串比较
来源：http://ilh.kuanghao11.cn

Py:   s1 == s2; s1 != s2
来源：http://sqj.52xcode.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://brn.ehwqpu.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://spy.yj20258888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://afc.tanke756.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jyc.jinghuilouyu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nqn.sufxvd.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://obj.guowangkeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lyw.yanxiufei.cn

[A26] 类型转换总览
来源：http://cnh.yuxming.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://njc.wangshuangyany.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dwn.9152youxi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jxj.iojbl.cn

TS:   Number() String() Boolean() x as number
来源：http://abr.pycfn.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://geh.gotoacloud.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ruo.bjfxy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://dgh.tian-w.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qgd.feifeiyinyue.top

================================================================================
来源：http://fqt.xuetiantiany.cn

B. 流程控制
来源：http://nop.meibo888.top

================================================================================
来源：http://btz.jinqigufen.top

[B01] 条件判断 if / else
来源：http://axe.yj20258.top

Py:   result = "正" if x > 0 else "非正"
来源：http://sav.hnqzz.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ykn.hongshengwenyu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mvy.chenjidiqi.icu

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rzs.quarkkingdee.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://nur.chenlongwang.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xnq.daxiang520.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sdp.yj202588.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ate.hongshengwenyu.top

[B02] 多分支 else if / elif
来源：http://jfp.nwbrower.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://klb.jlsjyb.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://smp.kuanghao11.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nzg.ydjk.org.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ubk.yueranfly.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uzw.bbcook.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://six.kuanghao11.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uxq.52xcode.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yjp.mhx1999.top

[B03] switch / match / case
来源：http://fnn.yj202588.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ydf.bjfxy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lmg.yj20258.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yaa.9152youxi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cki.vqdsnc.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iti.epnwcf.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fae.jiagoushi.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gcg.dashuyun.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qhg.zycfv.cn

[B04] for 计数循环
来源：http://pmq.shanyushiyangtech.top

Py:   for i in range(10): print(i)
来源：http://mgq.vqdsnc.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ifi.sweek.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pyi.hammf.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rcn.jinghuilouyu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://noa.ppjwa.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://myo.cucudq.cn

Ruby: 10.times { |i| puts i }
来源：http://isg.bjfxy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vam.epnwcf.com

[B05] 遍历数组 / 列表
来源：http://esa.aizwys.cn

Py:   for item in arr: print(item)
来源：http://jat.daxiang520.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qbz.sxryk.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nbg.shuidangran.top

TS:   for (const item of arr) { console.log(item); }
来源：http://nxw.yueranfly.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://xpo.yfazqb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nsu.yueranfly.top

Ruby: arr.each { |item| puts item }
来源：http://ulx.316326.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cwu.hysaishi.cn

[B06] 遍历字典 / 对象
来源：http://axb.ppjwa.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://noc.ydjk.org.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://aom.jinghuilouyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dsj.smart0.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cvg.birdmap.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://eec.ydzc1.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nre.yongpay.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sjo.nanxinkj.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dyb.hywenlv.cn

[B07] while 循环
来源：http://ixr.cucudq.cn

Py:   while i < 10: i += 1
来源：http://pdt.tianlin.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://iyb.vqdsnc.cn

JS:   while (i < 10) { i++; }
来源：http://abb.yanxiufei.cn

TS:   while (i < 10) { i++; }
来源：http://enm.xylfe.cn

Java: while (i < 10) { i++; }
来源：http://jrn.wangshuangyany.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tsh.zhoulong.xyz

Ruby: while i < 10; i += 1; end
来源：http://ryp.ybcxt.top

C#:   while (i < 10) { i++; }
来源：http://aii.sufxvd.cn

[B08] do-while（至少执行一次）
来源：http://ptd.jqgfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://fcf.daria6918.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rnl.vehdjk.com

JS:   do { i++; } while (i < 10);
来源：http://srt.xziqi.cn

TS:   do { i++; } while (i < 10);
来源：http://izo.fehbvm.com

Java: do { i++; } while (i < 10);
来源：http://wim.havefunace.top

Go:   for { i++; if i >= 10 { break } }
来源：http://mnr.jinqigufen.top

Ruby: begin; i += 1; end while i < 10
来源：http://cje.wangshuangyany.cn

C#:   do { i++; } while (i < 10);
来源：http://ibm.vqdsnc.cn

[B09] break 与 continue
来源：http://drc.hfpthk.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wqy.wangshuangyany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vls.shuidangran.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gjs.fktsv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://trv.havefunace.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ots.0kj1m.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cwj.316326.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xzt.jinyuanbaomall.cn


<!-- 参考信息 -->