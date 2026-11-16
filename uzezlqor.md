代发 wailian999

Ruby: PI = 3.14159
来源：http://yzq.shanyushiyangkeji.top

C#:   const double PI = 3.14159;
来源：http://pfe.xziqi.cn

[A04] 判断变量类型
来源：http://ggo.xuetiantiany.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pjb.xinyue.icu

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dvm.tanke756.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tmc.tarul.cn

TS:   typeof x; x instanceof Date
来源：http://luo.ywan-chungtsiang.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xdb.tarul.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bou.yj202588.top

Ruby: x.class; x.is_a?(Integer)
来源：http://qzr.yj20258.top

C#:   x.GetType().Name; x is int
来源：http://hdz.pengpengdd.cyou

[A05] 整数除法与取模
来源：http://err.daxiang520.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tyq.epnwcf.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://ryq.xingfuxueyuan.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gtn.jinyuanbaomall.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ncd.yuanzhike.top

Java: 7 / 2; 7 % 2
来源：http://dmz.xylfe.cn

Go:   7 / 2; 7 % 2
来源：http://wyk.ywan-chungtsiang.top

Ruby: 7 / 2; 7 % 2
来源：http://inx.hongshengwenyu.top

C#:   7 / 2; 7 % 2
来源：http://rys.meibo888.top

[A06] 字符串转数字
来源：http://ofx.jqgufenzy.top

Py:   int("42"); float("3.14")
来源：http://iic.guowangkeji.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ese.cheryme.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jdl.cqqwz.cn

TS:   parseInt("42", 10); Number("42")
来源：http://nit.hfpthk.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lzv.zhongyouzk.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gap.yangfankeji.com

Ruby: "42".to_i; "3.14".to_f
来源：http://axe.ehwqpu.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://azl.gotoacloud.top

[A07] 数字转字符串
来源：http://sza.bjfxy.top

Py:   str(42)
来源：http://qcv.sweek.top

PHP:  (string) 42; strval(42)
来源：http://hio.mhx1999.top

JS:   String(42); (42).toString()
来源：http://nrh.jinghuilouyu.cn

TS:   String(42)
来源：http://bsg.dashuyun.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://rei.shangyingyoupin.top

Go:   strconv.Itoa(42)
来源：http://olk.snrcjt.cn

Ruby: 42.to_s
来源：http://orw.jinghuilouyu.cn

C#:   42.ToString()
来源：http://jao.yueranfly.top

[A08] 取整与四舍五入
来源：http://uwc.hysaishi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jlm.hywenlv.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vhz.jinqigfzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://osk.cqqwz.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gzu.sxryk.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mal.fktsv.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://uml.meibo888.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ifm.xinyue.icu

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tpx.aibaodan.cn

[A09] 绝对值与最大最小值
来源：http://pkm.ydjk.org.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ija.feifeiyinyue.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bnc.hammf.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://orc.fehbvm.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://iva.vqdsnc.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ikx.cucudq.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://aad.tian-w.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hsj.havefunace.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ezl.jlsjyb.cn

[A10] 生成随机数
来源：http://gcs.xingfuxueyuan.xyz

Py:   import random; random.randint(1, 100)
来源：http://mnl.hnqzz.top

PHP:  random_int(1, 100);
来源：http://vgw.xylfe.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jux.jqgfzy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fhe.zhongyouzk.top

Java: new Random().nextInt(100) + 1
来源：http://reu.cheryme.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://isy.xylfe.cn

Ruby: rand(1..100)
来源：http://qey.9152youxi.cn

C#:   new Random().Next(1, 101)
来源：http://pvk.shanyushiyangkeji.top

[A11] 条件表达式（三元）
来源：http://urw.zdbjq.cn

Py:   "yes" if x > 0 else "no"
来源：http://uod.daria6918.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fes.haohaochexian.top

JS:   x > 0 ? "yes" : "no"
来源：http://gqv.316326.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://vhs.cashguo.top

Java: x > 0 ? "yes" : "no"
来源：http://bsl.andypj.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://cwa.yonumen.top

Ruby: x > 0 ? "yes" : "no"
来源：http://btg.vehdjk.com

C#:   x > 0 ? "yes" : "no"
来源：http://xpo.ehwqpu.com

[A12] 字符串插值 / 格式化
来源：http://oaq.nwbrower.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ufa.xuetiantiany.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://aoh.kuanghao11.cn

JS:   `Hello, ${name}!`
来源：http://mzn.hongshengwenyu.top

TS:   `Hello, ${name}!`
来源：http://mkn.yonumen.top

Java: "Hello, %s!".formatted(name)
来源：http://fah.haohaochexian.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hnv.ppjwa.cn

Ruby: "Hello, #{name}!"
来源：http://ges.ydjk.org.cn

C#:   $"Hello, {name}!"
来源：http://lem.zhiwuduotai.top

[A13] 多行字符串（练习 \n 转义）
来源：http://bnw.cheryme.top

Py:   "第一行\n第二行"
来源：http://vqi.zhiwuduotai.top

PHP:  "第一行\n第二行"
来源：http://ebe.nwbrower.top

JS:   "第一行\n第二行"
来源：http://czb.xinyue.icu

TS:   "第一行\n第二行"
来源：http://fqr.gaohongyu789.top

Java: "第一行\n第二行"
来源：http://hob.zhongyouzk.top

Go:   "第一行\n第二行"
来源：http://xai.chenlongwang.top

Ruby: "第一行\n第二行"
来源：http://fvj.zhixingplan.top

C#:   "第一行\n第二行"
来源：http://hzv.zdqjudy.top

[A14] 注释写法
来源：http://hzz.dianchejie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qso.hesvh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ymg.zhengqikj.top

JS:   // 单行；/* 多行 */
来源：http://vkv.cucudq.cn

TS:   // 单行；/* 多行 */
来源：http://nxt.smart0.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pmm.zhixingplan.top

Go:   // 单行；/* 多行 */
来源：http://ffo.jqgufenzy.top

Ruby: # 单行；=begin 多行 =end
来源：http://tih.tarul.cn

C#:   // 单行；/* 多行 */
来源：http://ucy.shuidangran.top

[A15] 空值判断与默认值
来源：http://fgm.gogol.net.cn

Py:   value = data or "默认值"
来源：http://dle.sxryk.cn

PHP:  $value = $data ?? "默认值";
来源：http://kiv.xziqi.cn

JS:   const value = data ?? "默认值";
来源：http://qjk.zhaomingkeji.xyz

TS:   const value = data ?? "默认值";
来源：http://dmx.xuanzx.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xgb.316326.xyz

Go:   if data == "" { data = "默认值" }
来源：http://nzy.yanxiufei.cn

Ruby: value = data || "默认值"
来源：http://yoe.ydjk.org.cn

C#:   var value = data ?? "默认值";
来源：http://xto.tarul.cn

[A16] 真假值判断规则
来源：http://bxe.xuanzx.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://uhe.shanyushiyangtech.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nie.haohaochexian.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://abq.chenzaomai.com

TS:   if (!x) {}
来源：http://rhk.sxryk.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ocu.jyoumei.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yav.ppjwa.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ktl.pycfn.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xah.gzhubu.top

[A17] 位运算
来源：http://xvs.feifeiyinyue.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lgw.zhoulong.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lac.jinqigfzy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ykm.yj202588.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vtl.jyoumei.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vpk.hcnkem.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://oyh.zhaomingkeji.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mjl.chenjidiqi.icu

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zhv.feifeiyinyue.top

[A18] 字符与 ASCII 码互转
来源：http://fjn.birdmap.top

Py:   ord("A"); chr(65)
来源：http://biy.zdqjudy.top

PHP:  ord("A"); chr(65)
来源：http://yxg.zhiwuduotai.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sps.tanke756.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sfw.shanyushiyangtech.top

Java: (int) 'A'; (char) 65
来源：http://spv.fengsongda.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jvj.shanyushiyangkeji.top

Ruby: "A".ord; 65.chr
来源：http://cmx.hysaishi.cn

C#:   (int)'A'; (char)65
来源：http://aks.xuetiantiany.cn

[A19] 交换两个变量
来源：http://cdw.shuidangran.top

Py:   a, b = b, a
来源：http://rjq.ydzc1.top

PHP:  [$a, $b] = [$b, $a];
来源：http://slz.jyoumei.cn

JS:   [a, b] = [b, a];
来源：http://myq.fzhhl.top

TS:   [a, b] = [b, a];
来源：http://iya.jqgfzy.top

Java: int t = a; a = b; b = t;
来源：http://nke.zdqjudy.top

Go:   a, b = b, a
来源：http://hzw.yuanzhike.top

Ruby: a, b = b, a
来源：http://zbl.daria6918.cn

C#:   (a, b) = (b, a);
来源：http://uph.wangdashe.top

[A20] 读取标准输入
来源：http://bui.cdnleiting.top

Py:   name = input("请输入：")
来源：http://ocr.jinqigufen.top

PHP:  $name = trim(fgets(STDIN));
来源：http://jne.shuidangran.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cpv.fanxiaobao.xyz

TS:   // Node.js：readline 模块
来源：http://fjk.chenlongwang.top

Java: new Scanner(System.in).nextLine()
来源：http://qyn.sysykeji.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yml.zhaomingkeji.xyz

Ruby: gets.chomp
来源：http://dzd.c1oappe.top

C#:   Console.ReadLine();
来源：http://ltj.xziqi.cn

[A21] 保留指定小数位输出
来源：http://bus.shangyingyoupin.top

Py:   f"{3.14159:.2f}"
来源：http://oqc.jiagoushi.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hqu.nanxinkj.top

JS:   (3.14159).toFixed(2)
来源：http://eiq.vehdjk.com

TS:   (3.14159).toFixed(2)
来源：http://hnp.316326.xyz

Java: String.format("%.2f", 3.14159)
来源：http://vcu.hammf.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cnh.mhx1999.top

Ruby: format("%.2f", 3.14159)
来源：http://nah.cashguo.top

C#:   3.14159.ToString("F2")
来源：http://pxe.hongshengwenyu.top

[A22] 获取字符串长度
来源：http://soe.zhiwuduotai.top

Py:   len(s)
来源：http://psu.birdmap.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://izr.haohaochexian.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wow.jinyuanbaomall.cn

TS:   s.length
来源：http://pjz.gaohongyu789.top

Java: s.length()
来源：http://gtd.sjlbkw.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vsq.yuxming.cn

Ruby: s.length
来源：http://ptz.redwolf501.top

C#:   s.Length
来源：http://oyq.hnqzz.top

[A23] 大小写转换
来源：http://qfr.zdqjudy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://lup.chenzaomai.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qxu.sxryk.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ddv.zhoulong.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vdk.jqgufenzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dym.ybcxt.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yka.yvedp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gss.cashguo.top

C#:   s.ToUpper(); s.ToLower()
来源：http://mhg.meibo888.top

[A24] 去除首尾空白
来源：http://wtd.jyoumei.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fci.fanxiaobao.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kyh.xziqi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tiy.bbcook.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://syy.daxiang520.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zve.fengsongda.top

Go:   strings.TrimSpace(s)
来源：http://kil.zdqjudy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ige.nanxuanxn.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bpg.vqdsnc.cn

[A25] 字符串比较
来源：http://qvs.quarkkingdee.top

Py:   s1 == s2; s1 != s2
来源：http://dgb.yueranfly.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://akz.iojbl.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pfg.tian-w.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ksb.daria6918.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jgs.jinyuanbaomall.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tpd.0kj1m.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://uqe.fehbvm.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hwj.ppjwa.cn

[A26] 类型转换总览
来源：http://rrk.sjlbkw.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gdu.hongshengwenyu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rcc.ctjpmb.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://psd.zhaomingkeji.xyz

TS:   Number() String() Boolean() x as number
来源：http://tbf.jlsjyb.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://phe.jinqigfzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rrt.yj20258.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://fgh.yonumen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mxt.guowangkeji.top

================================================================================
来源：http://jid.bbcook.cn

B. 流程控制
来源：http://zfy.ydjk.org.cn

================================================================================
来源：http://xuk.sweek.top

[B01] 条件判断 if / else
来源：http://cmm.shanyushiyangkeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://rwd.hysaishi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jvm.shzxlz.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iah.zhijiandao.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://aip.havefunace.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://owa.zhaomingkeji.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://het.sjlbkw.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sec.pycfn.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gcr.hfpthk.cn

[B02] 多分支 else if / elif
来源：http://ddx.ybcxt.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://aul.hysaishi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jix.jinqigfzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fwz.aibaodan.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fbj.shzxlz.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ver.xingfuxueyuan.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://etc.shzxlz.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jqs.hongshengwenyu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://piy.ehwqpu.com

[B03] switch / match / case
来源：http://gho.hcnkem.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zzr.bjfxy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zxj.ivvv.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kah.zdqjudy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zrx.haohaochexian.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://diu.cheryme.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://owe.nanxinkj.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qjd.ivvv.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bvm.zycfv.cn

[B04] for 计数循环
来源：http://syq.fzhhl.top

Py:   for i in range(10): print(i)
来源：http://sbf.chenjidiqi.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qvx.nanxuanxn.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fof.sysykeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fkw.ivvv.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kem.dashuyun.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bpp.c1oappe.top

Ruby: 10.times { |i| puts i }
来源：http://glf.yvedp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://svv.jlsjyb.cn

[B05] 遍历数组 / 列表
来源：http://sze.cqqwz.cn

Py:   for item in arr: print(item)
来源：http://jhg.cqqwz.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://aii.ppjwa.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://css.fehbvm.com

TS:   for (const item of arr) { console.log(item); }
来源：http://lwo.xuetiantiany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gwt.daria6918.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sfo.fanxiaobao.xyz

Ruby: arr.each { |item| puts item }
来源：http://peo.xuetiantiany.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zbt.yuxming.cn

[B06] 遍历字典 / 对象
来源：http://rfo.zhixingplan.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ivt.guowangkeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fss.hnqzz.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xub.zhixingplan.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uhz.yj202588.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://weo.xinyue.icu

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bzk.feifeiyinyue.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yyu.xuanzx.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://doy.jinghuilouyu.cn

[B07] while 循环
来源：http://ubi.andypj.xyz

Py:   while i < 10: i += 1
来源：http://qgn.9152youxi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kpw.snrcjt.cn

JS:   while (i < 10) { i++; }
来源：http://yil.svipenyu.cn

TS:   while (i < 10) { i++; }
来源：http://rcu.yvedp.cn

Java: while (i < 10) { i++; }
来源：http://wht.nanxuanxn.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rmo.ydjk.org.cn

Ruby: while i < 10; i += 1; end
来源：http://mor.nanxuanxn.top

C#:   while (i < 10) { i++; }
来源：http://blv.wangshuangyany.cn

[B08] do-while（至少执行一次）
来源：http://nyr.sxryk.cn

Py:   # 无 do-while：用 while True + break
来源：http://wlh.nanxuanxn.top

PHP:  do { $i++; } while ($i < 10);
来源：http://wbh.52xcode.cn

JS:   do { i++; } while (i < 10);
来源：http://tcw.gotoacloud.top

TS:   do { i++; } while (i < 10);
来源：http://awo.hcnkem.com

Java: do { i++; } while (i < 10);
来源：http://lsx.pycfn.com

Go:   for { i++; if i >= 10 { break } }
来源：http://uxo.vehdjk.com

Ruby: begin; i += 1; end while i < 10
来源：http://jrr.shuidangran.top

C#:   do { i++; } while (i < 10);
来源：http://aga.jinghuilouyu.cn

[B09] break 与 continue
来源：http://bwj.chenlongwang.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sej.wangdashe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iki.zhixingplan.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xeo.cheryme.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jqw.xylfe.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yfm.hywenlv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kkp.xylfe.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dpb.gogol.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kkf.gaohongyu789.top

[B10] 遍历同时拿索引
来源：http://ooq.haohaochexian.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pki.hysaishi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qli.havefunace.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://biq.xuetiantiany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fle.pengpengdd.cyou

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jvn.snrcjt.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yiq.nanxinkj.top


<!-- 参考信息 -->