代发 wailian999

Ruby: PI = 3.14159
来源：http://moe.jinghuilouyu.cn

C#:   const double PI = 3.14159;
来源：http://aao.quarkkingdee.top

[A04] 判断变量类型
来源：http://fyy.sxryk.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://arv.fengsongda.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zbi.haohaochexian.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lkm.ywan-chungtsiang.top

TS:   typeof x; x instanceof Date
来源：http://unz.yongpay.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://imu.fengsongda.top

Go:   reflect.TypeOf(x).Name()
来源：http://ftw.zhongyouzk.top

Ruby: x.class; x.is_a?(Integer)
来源：http://iqy.yongpay.top

C#:   x.GetType().Name; x is int
来源：http://pye.shanyushiyangtech.top

[A05] 整数除法与取模
来源：http://qlp.shzxlz.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nwh.quarkkingdee.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://bme.jlsjyb.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ius.jiagoushi.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dxm.zhijiandao.cn

Java: 7 / 2; 7 % 2
来源：http://ukz.vqdsnc.cn

Go:   7 / 2; 7 % 2
来源：http://hoi.fanxiaobao.xyz

Ruby: 7 / 2; 7 % 2
来源：http://hsp.gogol.net.cn

C#:   7 / 2; 7 % 2
来源：http://ahy.hnqzz.top

[A06] 字符串转数字
来源：http://bzu.shanyushiyangtech.top

Py:   int("42"); float("3.14")
来源：http://aib.redwolf501.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://aho.shangyingyoupin.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wpl.jinqigufen.top

TS:   parseInt("42", 10); Number("42")
来源：http://ylp.xingfuxueyuan.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zbz.quarkkingdee.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xfc.tianlin.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://btd.hfpthk.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://asv.zdbjq.cn

[A07] 数字转字符串
来源：http://rlr.sweek.top

Py:   str(42)
来源：http://fol.havefunace.top

PHP:  (string) 42; strval(42)
来源：http://eya.xinyue.icu

JS:   String(42); (42).toString()
来源：http://cwo.sweek.top

TS:   String(42)
来源：http://pfa.havefunace.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ecu.jiagoushi.top

Go:   strconv.Itoa(42)
来源：http://mvn.xuetiantiany.cn

Ruby: 42.to_s
来源：http://lhq.zhengqikj.top

C#:   42.ToString()
来源：http://gny.yanxiufei.cn

[A08] 取整与四舍五入
来源：http://tww.sysykeji.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ctx.vehdjk.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zot.zycfv.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baz.hfpthk.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://uut.andypj.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://acw.jinqigufen.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kqv.shanyushiyangkeji.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://rtf.feifeiyinyue.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ugd.jinghuilouyu.cn

[A09] 绝对值与最大最小值
来源：http://trh.andypj.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tsc.gotoacloud.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ypl.pengpengdd.cyou

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://eej.uphjek.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dvs.jinyuanbaomall.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://onb.zhaomingkeji.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hbw.xylfe.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://usg.yonumen.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nkn.hysaishi.cn

[A10] 生成随机数
来源：http://irp.zhongyouzk.top

Py:   import random; random.randint(1, 100)
来源：http://liq.hywenlv.cn

PHP:  random_int(1, 100);
来源：http://iqy.aibaodan.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lnw.nanxuanxn.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://swi.dashuyun.cn

Java: new Random().nextInt(100) + 1
来源：http://mow.zhijiandao.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dic.zhijiandao.cn

Ruby: rand(1..100)
来源：http://rxy.quarkkingdee.top

C#:   new Random().Next(1, 101)
来源：http://mhv.svipenyu.cn

[A11] 条件表达式（三元）
来源：http://jty.yuanzhike.top

Py:   "yes" if x > 0 else "no"
来源：http://bof.cashguo.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://dej.jqgufenzy.top

JS:   x > 0 ? "yes" : "no"
来源：http://jlw.mhx1999.top

TS:   x > 0 ? "yes" : "no"
来源：http://fua.c1oappe.top

Java: x > 0 ? "yes" : "no"
来源：http://hnu.sysykeji.top

Go:   // 无三元运算符，需用 if 语句
来源：http://gdo.hysaishi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ucw.wangshuangyany.cn

C#:   x > 0 ? "yes" : "no"
来源：http://uev.zhijiandao.cn

[A12] 字符串插值 / 格式化
来源：http://tpo.guannengcc.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zhf.uphjek.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zbe.zdbjq.cn

JS:   `Hello, ${name}!`
来源：http://eug.svipenyu.cn

TS:   `Hello, ${name}!`
来源：http://lgg.havefunace.top

Java: "Hello, %s!".formatted(name)
来源：http://dgt.svipenyu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bdq.pengpengdd.cyou

Ruby: "Hello, #{name}!"
来源：http://jte.fengsongda.top

C#:   $"Hello, {name}!"
来源：http://iiq.zhixingplan.top

[A13] 多行字符串（练习 \n 转义）
来源：http://sbe.cashguo.top

Py:   "第一行\n第二行"
来源：http://leq.52xcode.cn

PHP:  "第一行\n第二行"
来源：http://qce.hongshengwenyu.top

JS:   "第一行\n第二行"
来源：http://fni.xziqi.cn

TS:   "第一行\n第二行"
来源：http://xha.zhiwuduotai.top

Java: "第一行\n第二行"
来源：http://vux.shuidangran.top

Go:   "第一行\n第二行"
来源：http://pbc.yuxming.cn

Ruby: "第一行\n第二行"
来源：http://wbp.jinghuilouyu.cn

C#:   "第一行\n第二行"
来源：http://cfa.yuxming.cn

[A14] 注释写法
来源：http://fie.zhengqikj.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://teg.haohaochexian.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://rca.jiagoushi.top

JS:   // 单行；/* 多行 */
来源：http://mqk.nanxuanxn.top

TS:   // 单行；/* 多行 */
来源：http://wkg.nanxuanxn.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fis.bjfxy.top

Go:   // 单行；/* 多行 */
来源：http://leq.aizwys.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ubn.yanxiufei.cn

C#:   // 单行；/* 多行 */
来源：http://exz.sjlbkw.cn

[A15] 空值判断与默认值
来源：http://lqy.xingfuxueyuan.xyz

Py:   value = data or "默认值"
来源：http://ccc.jyoumei.cn

PHP:  $value = $data ?? "默认值";
来源：http://wdi.bbcook.cn

JS:   const value = data ?? "默认值";
来源：http://krb.hfpthk.cn

TS:   const value = data ?? "默认值";
来源：http://mrc.bbcook.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ksn.yueranfly.top

Go:   if data == "" { data = "默认值" }
来源：http://rkg.zhoulong.xyz

Ruby: value = data || "默认值"
来源：http://yix.chenzaomai.com

C#:   var value = data ?? "默认值";
来源：http://lsu.zhixingplan.top

[A16] 真假值判断规则
来源：http://dhu.uphjek.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ykb.zhixingplan.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kwp.hnxiangtu.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blo.hywenlv.cn

TS:   if (!x) {}
来源：http://hlo.haohaochexian.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zdu.jyoumei.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qch.jinqigufen.top

Ruby: unless x            # nil 与 false 为假
来源：http://myy.xuetiantiany.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://osr.yuxming.cn

[A17] 位运算
来源：http://itp.shanyushiyangkeji.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bhi.zhengqikj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ncz.hnxiangtu.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cug.hnxiangtu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pns.aizwys.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rxh.chenjidiqi.icu

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jfs.yj202588.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://axw.guowangkeji.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zeu.zdbjq.cn

[A18] 字符与 ASCII 码互转
来源：http://gwx.smart0.xyz

Py:   ord("A"); chr(65)
来源：http://aeo.ydjk.org.cn

PHP:  ord("A"); chr(65)
来源：http://iei.yuxming.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ngz.xinyue.icu

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fjr.yonumen.top

Java: (int) 'A'; (char) 65
来源：http://dga.jinqigufen.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gmo.jinqigufen.top

Ruby: "A".ord; 65.chr
来源：http://qaw.pengpengdd.cyou

C#:   (int)'A'; (char)65
来源：http://roa.xinyue.icu

[A19] 交换两个变量
来源：http://ilh.xuetiantiany.cn

Py:   a, b = b, a
来源：http://xte.gzhubu.top

PHP:  [$a, $b] = [$b, $a];
来源：http://pnc.bjfxy.top

JS:   [a, b] = [b, a];
来源：http://mrt.dashuyun.cn

TS:   [a, b] = [b, a];
来源：http://quf.9152youxi.cn

Java: int t = a; a = b; b = t;
来源：http://tyc.0kj1m.cn

Go:   a, b = b, a
来源：http://hhm.shuidangran.top

Ruby: a, b = b, a
来源：http://fnk.xuetiantiany.cn

C#:   (a, b) = (b, a);
来源：http://gzx.jinghuilouyu.cn

[A20] 读取标准输入
来源：http://kkl.xylfe.cn

Py:   name = input("请输入：")
来源：http://zjk.xuanzx.com

PHP:  $name = trim(fgets(STDIN));
来源：http://bva.cucudq.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fvn.hnxiangtu.top

TS:   // Node.js：readline 模块
来源：http://srt.sysykeji.top

Java: new Scanner(System.in).nextLine()
来源：http://kpk.gotoacloud.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vtw.ywan-chungtsiang.top

Ruby: gets.chomp
来源：http://phd.jlsjyb.cn

C#:   Console.ReadLine();
来源：http://jfp.guannengcc.top

[A21] 保留指定小数位输出
来源：http://ref.pycfn.com

Py:   f"{3.14159:.2f}"
来源：http://vyt.xuetiantiany.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kjw.xylfe.cn

JS:   (3.14159).toFixed(2)
来源：http://yhs.yueranfly.top

TS:   (3.14159).toFixed(2)
来源：http://jax.fzhhl.top

Java: String.format("%.2f", 3.14159)
来源：http://xtz.jinqigufen.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gsb.ppjwa.cn

Ruby: format("%.2f", 3.14159)
来源：http://coy.yuxming.cn

C#:   3.14159.ToString("F2")
来源：http://wtg.iojbl.cn

[A22] 获取字符串长度
来源：http://bww.pengpengdd.cyou

Py:   len(s)
来源：http://cgm.ydjk.org.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hxk.gaohongyu789.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tda.smart0.xyz

TS:   s.length
来源：http://klv.hywenlv.cn

Java: s.length()
来源：http://jtg.nanxuanxn.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oeo.epnwcf.com

Ruby: s.length
来源：http://hci.tarul.cn

C#:   s.Length
来源：http://faw.xziqi.cn

[A23] 大小写转换
来源：http://mzo.hcnkem.com

Py:   s.upper(); s.lower(); s.title()
来源：http://jrg.shangyingyoupin.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jpe.daxiang520.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zzn.zhongyouzk.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://buo.xuanzx.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mjw.fzhhl.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sch.haohaochexian.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oql.dashuyun.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://eit.bbcook.cn

[A24] 去除首尾空白
来源：http://uoz.mhx1999.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ljn.jinqigfzy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iqu.9152youxi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qax.hongshengwenyu.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uxp.fzhhl.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qgu.cashguo.top

Go:   strings.TrimSpace(s)
来源：http://ztf.sysykeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tkk.hesvh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bqe.guowangkeji.top

[A25] 字符串比较
来源：http://fuc.cdnleiting.top

Py:   s1 == s2; s1 != s2
来源：http://kgy.tian-w.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lhv.gotoacloud.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fpz.tianlin.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uaz.vehdjk.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://aqp.birdmap.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uqk.nanxuanxn.top

Ruby: s1 == s2; s1 <=> s2
来源：http://irm.cqqwz.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://byl.zhiwuduotai.top

[A26] 类型转换总览
来源：http://unh.uphjek.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://igq.gaohongyu789.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vfp.zhiwuduotai.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xde.cdnleiting.top

TS:   Number() String() Boolean() x as number
来源：http://zmc.guowangkeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hca.ehwqpu.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zhd.andypj.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://ffa.vehdjk.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zej.havefunace.top

================================================================================
来源：http://lmz.ydjk.org.cn

B. 流程控制
来源：http://zft.cqqwz.cn

================================================================================
来源：http://srk.cheryme.top

[B01] 条件判断 if / else
来源：http://yuq.xuetiantiany.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lii.zhijiandao.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qmq.smart0.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cwt.xuetiantiany.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wqq.aibaodan.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dwr.hongshengwenyu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tyq.yanxiufei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://agx.zhaomingkeji.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tqp.hysaishi.cn

[B02] 多分支 else if / elif
来源：http://xsn.aizwys.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gub.yj20258888.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sxy.tian-w.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vxx.316326.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rdg.nwbrower.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oqr.yangfankeji.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gvx.hnqzz.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sut.vehdjk.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aye.xziqi.cn

[B03] switch / match / case
来源：http://nzy.shanyushiyangkeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pjt.jianghu66.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qwm.ehwqpu.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oiw.shangyingyoupin.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://coa.wangshuangyany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rdg.jiagoushi.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://snd.ywan-chungtsiang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://puh.vqdsnc.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tmc.316326.xyz

[B04] for 计数循环
来源：http://rmv.zhongyouzk.top

Py:   for i in range(10): print(i)
来源：http://mka.zhongyouzk.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cay.uphjek.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yuv.tarul.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://znt.guannengcc.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wpj.wangdashe.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qkj.chenlongwang.top

Ruby: 10.times { |i| puts i }
来源：http://mvq.jyoumei.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://djr.jinqigfzy.top

[B05] 遍历数组 / 列表
来源：http://xin.yj202588.top

Py:   for item in arr: print(item)
来源：http://ayg.hesvh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rlq.svipenyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://iwh.zycfv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tiu.ivvv.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://nek.kuanghao11.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hyp.sxryk.cn

Ruby: arr.each { |item| puts item }
来源：http://knr.cheryme.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dsu.mhx1999.top

[B06] 遍历字典 / 对象
来源：http://jtd.cashguo.top

Py:   for k, v in d.items(): print(k, v)
来源：http://jpr.pengpengdd.cyou

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uyc.iojbl.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ffp.wangshuangyany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://smt.zhaomingkeji.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://iws.zhiwuduotai.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eyo.feifeiyinyue.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fsh.snrcjt.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yiq.birdmap.top

[B07] while 循环
来源：http://fqh.yanxiufei.cn

Py:   while i < 10: i += 1
来源：http://hxu.pengpengdd.cyou

PHP:  while ($i < 10) { $i++; }
来源：http://zbk.cqqwz.cn

JS:   while (i < 10) { i++; }
来源：http://ncz.guowangkeji.top

TS:   while (i < 10) { i++; }
来源：http://iop.jinghuilouyu.cn

Java: while (i < 10) { i++; }
来源：http://ngb.guannengcc.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rjv.xinyue.icu

Ruby: while i < 10; i += 1; end
来源：http://lsf.yangfankeji.com

C#:   while (i < 10) { i++; }
来源：http://zwn.fzhhl.top

[B08] do-while（至少执行一次）
来源：http://llk.wangshuangyany.cn

Py:   # 无 do-while：用 while True + break
来源：http://bee.0kj1m.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://agr.ydzc1.top

JS:   do { i++; } while (i < 10);
来源：http://wme.zhijiandao.cn

TS:   do { i++; } while (i < 10);
来源：http://vdo.birdmap.top

Java: do { i++; } while (i < 10);
来源：http://pbq.hnqzz.top

Go:   for { i++; if i >= 10 { break } }
来源：http://phv.hongshengwenyu.top

Ruby: begin; i += 1; end while i < 10
来源：http://dgw.yvedp.cn

C#:   do { i++; } while (i < 10);
来源：http://and.daria6918.cn

[B09] break 与 continue
来源：http://wxl.mhx1999.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://scv.yvedp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rty.bjfxy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kzg.yj20258.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kib.hammf.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aso.feifeiyinyue.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vjn.zycfv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://orx.316326.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rxb.hcnkem.com

[B10] 遍历同时拿索引
来源：http://civ.aibaodan.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jsu.ydzc1.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gkl.hfpthk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yjz.jqgufenzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rvf.wangdashe.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lkv.jyoumei.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qss.ppjwa.cn


<!-- 参考信息 -->