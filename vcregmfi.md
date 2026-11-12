代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xdu.ctjpmb.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nhc.shanyushiyangkeji.top

TS:   typeof x; x instanceof Date
来源：http://uwk.birdmap.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bkh.daxiang520.top

Go:   reflect.TypeOf(x).Name()
来源：http://hxh.feifeiyinyue.top

Ruby: x.class; x.is_a?(Integer)
来源：http://zjg.chenjidiqi.icu

C#:   x.GetType().Name; x is int
来源：http://wtz.quarkkingdee.top

[A05] 整数除法与取模
来源：http://mrl.yj20258888.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wtz.ivvv.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://cnp.zhixingplan.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bau.hesvh.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zcn.c1oappe.top

Java: 7 / 2; 7 % 2
来源：http://hme.yj202588.top

Go:   7 / 2; 7 % 2
来源：http://adx.sweek.top

Ruby: 7 / 2; 7 % 2
来源：http://ykh.c1oappe.top

C#:   7 / 2; 7 % 2
来源：http://pkb.nanxinkj.top

[A06] 字符串转数字
来源：http://fmo.xinyue.icu

Py:   int("42"); float("3.14")
来源：http://rup.meibo888.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kwl.fehbvm.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hgt.0kj1m.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cdz.hcnkem.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mmk.0kj1m.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hed.hnqzz.top

Ruby: "42".to_i; "3.14".to_f
来源：http://dza.shanyushiyangtech.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://swa.zhijiandao.cn

[A07] 数字转字符串
来源：http://bfg.ybcxt.top

Py:   str(42)
来源：http://kfk.ppjwa.cn

PHP:  (string) 42; strval(42)
来源：http://ogo.hysaishi.cn

JS:   String(42); (42).toString()
来源：http://jnq.sweek.top

TS:   String(42)
来源：http://ynd.sxryk.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ubn.cheryme.top

Go:   strconv.Itoa(42)
来源：http://xhn.cucudq.cn

Ruby: 42.to_s
来源：http://lui.jiagoushi.top

C#:   42.ToString()
来源：http://ypt.zhengqikj.top

[A08] 取整与四舍五入
来源：http://xlc.kuanghao11.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ywf.cqqwz.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xhu.zdbjq.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://afs.svipenyu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ycb.yanxiufei.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://eue.yvedp.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gdn.zhaomingkeji.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://alu.sjlbkw.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ghq.zhijiandao.cn

[A09] 绝对值与最大最小值
来源：http://eqm.9152youxi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yhs.ywan-chungtsiang.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://byu.dianchejie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://atu.gotoacloud.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hjx.ydzc1.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rpw.gaohongyu789.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nsb.yonumen.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://iob.snrcjt.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cfa.0kj1m.cn

[A10] 生成随机数
来源：http://oww.pengpengdd.cyou

Py:   import random; random.randint(1, 100)
来源：http://xjz.yuanzhike.top

PHP:  random_int(1, 100);
来源：http://oxb.vehdjk.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ufz.vehdjk.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://atx.quarkkingdee.top

Java: new Random().nextInt(100) + 1
来源：http://hit.wangshuangyany.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lcv.zhengqikj.top

Ruby: rand(1..100)
来源：http://moq.cqqwz.cn

C#:   new Random().Next(1, 101)
来源：http://cjw.haohaochexian.top

[A11] 条件表达式（三元）
来源：http://vsh.zhijiandao.cn

Py:   "yes" if x > 0 else "no"
来源：http://wmp.nanxinkj.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ycn.bjfxy.top

JS:   x > 0 ? "yes" : "no"
来源：http://jsm.hnqzz.top

TS:   x > 0 ? "yes" : "no"
来源：http://eqy.c1oappe.top

Java: x > 0 ? "yes" : "no"
来源：http://hyu.52xcode.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gnp.yj20258888.top

Ruby: x > 0 ? "yes" : "no"
来源：http://plq.bbcook.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ala.ppjwa.cn

[A12] 字符串插值 / 格式化
来源：http://mue.yuxming.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rqo.xinyue.icu

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uib.yuxming.cn

JS:   `Hello, ${name}!`
来源：http://yks.yvedp.cn

TS:   `Hello, ${name}!`
来源：http://fwa.yangfankeji.com

Java: "Hello, %s!".formatted(name)
来源：http://csh.fehbvm.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wyw.yvedp.cn

Ruby: "Hello, #{name}!"
来源：http://tit.fanxiaobao.xyz

C#:   $"Hello, {name}!"
来源：http://nzm.svipenyu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vrx.sweek.top

Py:   "第一行\n第二行"
来源：http://vak.jyoumei.cn

PHP:  "第一行\n第二行"
来源：http://bsp.xingfuxueyuan.xyz

JS:   "第一行\n第二行"
来源：http://ifk.sysykeji.top

TS:   "第一行\n第二行"
来源：http://efo.chenjidiqi.icu

Java: "第一行\n第二行"
来源：http://bri.hesvh.cn

Go:   "第一行\n第二行"
来源：http://wfc.sysykeji.top

Ruby: "第一行\n第二行"
来源：http://dnj.sufxvd.cn

C#:   "第一行\n第二行"
来源：http://oon.zdbjq.cn

[A14] 注释写法
来源：http://eqc.nanxuanxn.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://wvr.sweek.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://oaf.havefunace.top

JS:   // 单行；/* 多行 */
来源：http://rbv.jinqigfzy.top

TS:   // 单行；/* 多行 */
来源：http://fih.xziqi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cwv.tianlin.xyz

Go:   // 单行；/* 多行 */
来源：http://ybr.xuanzx.com

Ruby: # 单行；=begin 多行 =end
来源：http://wex.fktsv.cn

C#:   // 单行；/* 多行 */
来源：http://mly.hnqzz.top

[A15] 空值判断与默认值
来源：http://fhe.zhongyouzk.top

Py:   value = data or "默认值"
来源：http://tyl.hnqzz.top

PHP:  $value = $data ?? "默认值";
来源：http://cvu.snrcjt.cn

JS:   const value = data ?? "默认值";
来源：http://suw.aibaodan.cn

TS:   const value = data ?? "默认值";
来源：http://knb.andypj.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sok.shanyushiyangtech.top

Go:   if data == "" { data = "默认值" }
来源：http://kpp.zycfv.cn

Ruby: value = data || "默认值"
来源：http://mcz.yonumen.top

C#:   var value = data ?? "默认值";
来源：http://gug.svipenyu.cn

[A16] 真假值判断规则
来源：http://drj.yangfankeji.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zoa.yj20258888.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://krm.vehdjk.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rdk.bbcook.cn

TS:   if (!x) {}
来源：http://zmo.zhijiandao.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lcb.yongpay.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://utj.52xcode.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gfm.zhoulong.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uyi.birdmap.top

[A17] 位运算
来源：http://qge.svipenyu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rnu.yj20258888.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://feu.hongshengwenyu.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lhe.meibo888.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pwe.xuetiantiany.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aoc.yj20258.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://uav.0kj1m.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cla.redwolf501.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bjk.52xcode.cn

[A18] 字符与 ASCII 码互转
来源：http://ahr.gogol.net.cn

Py:   ord("A"); chr(65)
来源：http://zwc.hesvh.cn

PHP:  ord("A"); chr(65)
来源：http://ddo.haohaochexian.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fce.jinghuilouyu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rnx.wangdashe.top

Java: (int) 'A'; (char) 65
来源：http://eib.ywan-chungtsiang.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zcb.hcnkem.com

Ruby: "A".ord; 65.chr
来源：http://yyt.xylfe.cn

C#:   (int)'A'; (char)65
来源：http://rlo.yj20258888.top

[A19] 交换两个变量
来源：http://hdl.tanke756.top

Py:   a, b = b, a
来源：http://lqp.fzhhl.top

PHP:  [$a, $b] = [$b, $a];
来源：http://vwu.yj20258888.top

JS:   [a, b] = [b, a];
来源：http://icj.wangshuangyany.cn

TS:   [a, b] = [b, a];
来源：http://ujq.cashguo.top

Java: int t = a; a = b; b = t;
来源：http://dmi.xuetiantiany.cn

Go:   a, b = b, a
来源：http://rtr.bjfxy.top

Ruby: a, b = b, a
来源：http://vur.uphjek.com

C#:   (a, b) = (b, a);
来源：http://pww.dianchejie.cn

[A20] 读取标准输入
来源：http://tlt.uphjek.com

Py:   name = input("请输入：")
来源：http://qih.ppjwa.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://umv.redwolf501.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://obn.zhijiandao.cn

TS:   // Node.js：readline 模块
来源：http://qgg.c1oappe.top

Java: new Scanner(System.in).nextLine()
来源：http://twv.ywan-chungtsiang.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bde.ppjwa.cn

Ruby: gets.chomp
来源：http://jso.yuxming.cn

C#:   Console.ReadLine();
来源：http://wpd.andypj.xyz

[A21] 保留指定小数位输出
来源：http://zfy.zycfv.cn

Py:   f"{3.14159:.2f}"
来源：http://mkk.meibo888.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kmc.hfpthk.cn

JS:   (3.14159).toFixed(2)
来源：http://vei.ehwqpu.com

TS:   (3.14159).toFixed(2)
来源：http://dxu.zycfv.cn

Java: String.format("%.2f", 3.14159)
来源：http://fkl.gzhubu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://but.pengpengdd.cyou

Ruby: format("%.2f", 3.14159)
来源：http://zas.fanxiaobao.xyz

C#:   3.14159.ToString("F2")
来源：http://htt.quarkkingdee.top

[A22] 获取字符串长度
来源：http://hvr.zhengqikj.top

Py:   len(s)
来源：http://pun.feifeiyinyue.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kka.0kj1m.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pxr.epnwcf.com

TS:   s.length
来源：http://aps.sxryk.cn

Java: s.length()
来源：http://gif.zhaomingkeji.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rtm.zycfv.cn

Ruby: s.length
来源：http://opn.zhiwuduotai.top

C#:   s.Length
来源：http://eob.nanxuanxn.top

[A23] 大小写转换
来源：http://csz.hfpthk.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fgo.xylfe.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zxw.yj202588.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lrf.daria6918.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://msi.xylfe.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ton.hywenlv.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://inv.zycfv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://szv.shanyushiyangtech.top

C#:   s.ToUpper(); s.ToLower()
来源：http://wmb.zhaomingkeji.xyz

[A24] 去除首尾空白
来源：http://eqd.yj20258888.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jpy.hcnkem.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ciq.mhx1999.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dnh.sxryk.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rsy.yfazqb.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sii.pycfn.com

Go:   strings.TrimSpace(s)
来源：http://cfm.nanxuanxn.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ead.snrcjt.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bwe.aizwys.cn

[A25] 字符串比较
来源：http://feh.hnxiangtu.top

Py:   s1 == s2; s1 != s2
来源：http://oag.wangdashe.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kgk.shzxlz.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ems.tarul.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://usb.chenzaomai.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tsi.bjfxy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://eyo.shangyingyoupin.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ziw.gzhubu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dkb.zhengqikj.top

[A26] 类型转换总览
来源：http://wwt.chenlongwang.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://iem.cqqwz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yzd.aibaodan.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://isf.tarul.cn

TS:   Number() String() Boolean() x as number
来源：http://qqq.fengsongda.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://swx.pycfn.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wsr.tarul.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://woc.c1oappe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mqr.yfazqb.com

================================================================================
来源：http://txr.meibo888.top

B. 流程控制
来源：http://bme.snrcjt.cn

================================================================================
来源：http://ebv.smart0.xyz

[B01] 条件判断 if / else
来源：http://ikq.zhiwuduotai.top

Py:   result = "正" if x > 0 else "非正"
来源：http://eqy.jiagoushi.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tii.nanxuanxn.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wzd.jinqigufen.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mzg.andypj.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://ggf.yanxiufei.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qux.tian-w.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fkf.fehbvm.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tsu.aibaodan.cn

[B02] 多分支 else if / elif
来源：http://kqx.cdnleiting.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yzd.jyoumei.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vxn.cheryme.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zjb.yvedp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kfi.xingfuxueyuan.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ely.0kj1m.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bqp.aizwys.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cev.hfpthk.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lah.jyoumei.cn

[B03] switch / match / case
来源：http://chq.vqdsnc.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bpj.uphjek.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qwt.shanyushiyangkeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zxq.chenlongwang.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eja.chenlongwang.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xpk.bbcook.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xom.zhijiandao.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kub.chenlongwang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ldi.yanxiufei.cn

[B04] for 计数循环
来源：http://umw.havefunace.top

Py:   for i in range(10): print(i)
来源：http://buc.xuanzx.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sbc.yonumen.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://diz.redwolf501.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qra.yj20258.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gqg.zhijiandao.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cnn.9152youxi.cn

Ruby: 10.times { |i| puts i }
来源：http://twb.ydjk.org.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hff.xziqi.cn

[B05] 遍历数组 / 列表
来源：http://nga.chenjidiqi.icu

Py:   for item in arr: print(item)
来源：http://vgy.jinqigfzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vwz.sysykeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://chp.sxryk.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ucc.andypj.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://iqd.haohaochexian.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vlq.epnwcf.com

Ruby: arr.each { |item| puts item }
来源：http://arn.havefunace.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cmh.gaohongyu789.top

[B06] 遍历字典 / 对象
来源：http://jib.bjfxy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zci.sjlbkw.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zyq.shanyushiyangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gco.snrcjt.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fsg.jqgfzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://aqi.sysykeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eou.yj20258.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pye.chenzaomai.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ylx.havefunace.top

[B07] while 循环
来源：http://mka.gaohongyu789.top

Py:   while i < 10: i += 1
来源：http://nig.hnqzz.top

PHP:  while ($i < 10) { $i++; }
来源：http://qdi.jianghu66.top

JS:   while (i < 10) { i++; }
来源：http://uhb.zhixingplan.top

TS:   while (i < 10) { i++; }
来源：http://tas.316326.xyz

Java: while (i < 10) { i++; }
来源：http://utz.zdbjq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dil.tarul.cn

Ruby: while i < 10; i += 1; end
来源：http://tls.smart0.xyz

C#:   while (i < 10) { i++; }
来源：http://ren.jyoumei.cn

[B08] do-while（至少执行一次）
来源：http://yej.guowangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://uch.ybcxt.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ruq.tarul.cn

JS:   do { i++; } while (i < 10);
来源：http://uci.ppjwa.cn

TS:   do { i++; } while (i < 10);
来源：http://qyq.yj20258.top

Java: do { i++; } while (i < 10);
来源：http://tvr.tanke756.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hmy.pengpengdd.cyou

Ruby: begin; i += 1; end while i < 10
来源：http://noo.cheryme.top

C#:   do { i++; } while (i < 10);
来源：http://xrn.gogol.net.cn

[B09] break 与 continue
来源：http://ovo.yvedp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://feb.gogol.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tpd.ydzc1.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vhj.redwolf501.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://liq.zhiwuduotai.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zcw.pycfn.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ixb.yj20258.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qhq.svipenyu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rrr.shuidangran.top

[B10] 遍历同时拿索引
来源：http://kto.9152youxi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cwx.hfpthk.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bkw.aizwys.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jtp.shanyushiyangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lob.mhx1999.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://znl.redwolf501.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kvv.jqgufenzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yqq.yonumen.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fqs.daria6918.cn

[B11] 生成数字序列 / 区间
来源：http://ugn.tarul.cn

Py:   list(range(0, 10, 2))
来源：http://awx.svipenyu.cn


<!-- 参考信息 -->