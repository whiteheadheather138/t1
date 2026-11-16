代发 wailian999

JS:   const PI = 3.14159;
来源：http://jkf.cashguo.top

TS:   const PI: number = 3.14159;
来源：http://irj.52xcode.cn

Java: static final double PI = 3.14159;
来源：http://pei.hnqzz.top

Go:   const PI = 3.14159
来源：http://epy.kuanghao11.cn

Ruby: PI = 3.14159
来源：http://ypo.shanyushiyangtech.top

C#:   const double PI = 3.14159;
来源：http://kfp.sxryk.cn

[A04] 判断变量类型
来源：http://vam.jqgfzy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://lnf.vehdjk.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tpv.dashuyun.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jis.zhiwuduotai.top

TS:   typeof x; x instanceof Date
来源：http://nfb.jyoumei.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xrz.jqgufenzy.top

Go:   reflect.TypeOf(x).Name()
来源：http://uam.zhiwuduotai.top

Ruby: x.class; x.is_a?(Integer)
来源：http://adr.zdqjudy.top

C#:   x.GetType().Name; x is int
来源：http://upu.yangfankeji.com

[A05] 整数除法与取模
来源：http://oeh.jianghu66.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dhy.yj20258888.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://vvr.sxryk.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://muj.shzxlz.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cbh.fktsv.cn

Java: 7 / 2; 7 % 2
来源：http://txo.c1oappe.top

Go:   7 / 2; 7 % 2
来源：http://hdt.fktsv.cn

Ruby: 7 / 2; 7 % 2
来源：http://ony.jqgufenzy.top

C#:   7 / 2; 7 % 2
来源：http://fly.0kj1m.cn

[A06] 字符串转数字
来源：http://uox.fehbvm.com

Py:   int("42"); float("3.14")
来源：http://hzq.cheryme.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blf.chenlongwang.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gti.zdqjudy.top

TS:   parseInt("42", 10); Number("42")
来源：http://rkv.zycfv.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rjp.cdnleiting.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kuy.kuanghao11.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ppz.jinghuilouyu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uwn.nanxuanxn.top

[A07] 数字转字符串
来源：http://ulk.ydzc1.top

Py:   str(42)
来源：http://xof.zhiwuduotai.top

PHP:  (string) 42; strval(42)
来源：http://bfr.zhaomingkeji.xyz

JS:   String(42); (42).toString()
来源：http://fgp.yj202588.top

TS:   String(42)
来源：http://szq.redwolf501.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://cal.gogol.net.cn

Go:   strconv.Itoa(42)
来源：http://emv.sweek.top

Ruby: 42.to_s
来源：http://hib.feifeiyinyue.top

C#:   42.ToString()
来源：http://reo.haohaochexian.top

[A08] 取整与四舍五入
来源：http://vbh.bbcook.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://aht.ydzc1.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mbh.nanxinkj.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mhl.jinyuanbaomall.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://upl.zdbjq.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jzh.kuanghao11.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zft.hnxiangtu.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://mvp.gaohongyu789.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lxn.daria6918.cn

[A09] 绝对值与最大最小值
来源：http://lwo.redwolf501.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gjv.jianghu66.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ymo.hnxiangtu.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zrc.nanxuanxn.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xgm.ivvv.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wmx.guannengcc.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dyy.cdnleiting.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nte.jqgufenzy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yxj.jqgufenzy.top

[A10] 生成随机数
来源：http://pgo.ehwqpu.com

Py:   import random; random.randint(1, 100)
来源：http://ouq.xuetiantiany.cn

PHP:  random_int(1, 100);
来源：http://hal.shuidangran.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ltl.ppjwa.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fmr.yuxming.cn

Java: new Random().nextInt(100) + 1
来源：http://juw.yongpay.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://urr.fanxiaobao.xyz

Ruby: rand(1..100)
来源：http://dnm.daria6918.cn

C#:   new Random().Next(1, 101)
来源：http://qvr.gogol.net.cn

[A11] 条件表达式（三元）
来源：http://mmn.wangdashe.top

Py:   "yes" if x > 0 else "no"
来源：http://axw.aizwys.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dxx.hcnkem.com

JS:   x > 0 ? "yes" : "no"
来源：http://tew.yuxming.cn

TS:   x > 0 ? "yes" : "no"
来源：http://auf.aibaodan.cn

Java: x > 0 ? "yes" : "no"
来源：http://wwr.yvedp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hgf.yfazqb.com

Ruby: x > 0 ? "yes" : "no"
来源：http://vey.cheryme.top

C#:   x > 0 ? "yes" : "no"
来源：http://lzk.9152youxi.cn

[A12] 字符串插值 / 格式化
来源：http://hct.andypj.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wtw.iojbl.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cnw.shanyushiyangkeji.top

JS:   `Hello, ${name}!`
来源：http://aor.jyoumei.cn

TS:   `Hello, ${name}!`
来源：http://lri.yj20258888.top

Java: "Hello, %s!".formatted(name)
来源：http://ppn.fktsv.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ohx.hammf.cn

Ruby: "Hello, #{name}!"
来源：http://ddp.bjfxy.top

C#:   $"Hello, {name}!"
来源：http://znr.zhengqikj.top

[A13] 多行字符串（练习 \n 转义）
来源：http://jby.cdnleiting.top

Py:   "第一行\n第二行"
来源：http://mwb.jyoumei.cn

PHP:  "第一行\n第二行"
来源：http://avn.zdqjudy.top

JS:   "第一行\n第二行"
来源：http://edl.dianchejie.cn

TS:   "第一行\n第二行"
来源：http://afb.zhijiandao.cn

Java: "第一行\n第二行"
来源：http://iix.yvedp.cn

Go:   "第一行\n第二行"
来源：http://gws.chenzaomai.com

Ruby: "第一行\n第二行"
来源：http://mmr.hammf.cn

C#:   "第一行\n第二行"
来源：http://bce.yangfankeji.com

[A14] 注释写法
来源：http://ovf.yfazqb.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://csb.fzhhl.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://mxs.yj20258888.top

JS:   // 单行；/* 多行 */
来源：http://azy.pengpengdd.cyou

TS:   // 单行；/* 多行 */
来源：http://gok.snrcjt.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jqo.52xcode.cn

Go:   // 单行；/* 多行 */
来源：http://hcd.yj20258.top

Ruby: # 单行；=begin 多行 =end
来源：http://dqj.vehdjk.com

C#:   // 单行；/* 多行 */
来源：http://dnh.yuanzhike.top

[A15] 空值判断与默认值
来源：http://kak.jinqigufen.top

Py:   value = data or "默认值"
来源：http://cpi.xylfe.cn

PHP:  $value = $data ?? "默认值";
来源：http://wse.jinghuilouyu.cn

JS:   const value = data ?? "默认值";
来源：http://viu.chenzaomai.com

TS:   const value = data ?? "默认值";
来源：http://ets.zhijiandao.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hnn.havefunace.top

Go:   if data == "" { data = "默认值" }
来源：http://sqg.jlsjyb.cn

Ruby: value = data || "默认值"
来源：http://cme.chenzaomai.com

C#:   var value = data ?? "默认值";
来源：http://bdw.aibaodan.cn

[A16] 真假值判断规则
来源：http://vji.kuanghao11.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://apv.tian-w.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://moy.havefunace.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://oeg.hfpthk.cn

TS:   if (!x) {}
来源：http://ect.tanke756.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wmb.shanyushiyangkeji.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ned.tianlin.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://uye.9152youxi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sus.jiagoushi.top

[A17] 位运算
来源：http://xes.jlsjyb.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ccm.jinqigfzy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://een.gotoacloud.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fvf.dianchejie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lfx.hfpthk.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aak.tianlin.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vwh.tanke756.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nbc.shanyushiyangkeji.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yqp.haohaochexian.top

[A18] 字符与 ASCII 码互转
来源：http://nke.hywenlv.cn

Py:   ord("A"); chr(65)
来源：http://emd.feifeiyinyue.top

PHP:  ord("A"); chr(65)
来源：http://jhc.nanxuanxn.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iyl.haohaochexian.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kix.hysaishi.cn

Java: (int) 'A'; (char) 65
来源：http://zgj.hnqzz.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://umu.pengpengdd.cyou

Ruby: "A".ord; 65.chr
来源：http://zko.daria6918.cn

C#:   (int)'A'; (char)65
来源：http://dgc.dashuyun.cn

[A19] 交换两个变量
来源：http://hix.sufxvd.cn

Py:   a, b = b, a
来源：http://gdx.hammf.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yxd.yanxiufei.cn

JS:   [a, b] = [b, a];
来源：http://vus.jinghuilouyu.cn

TS:   [a, b] = [b, a];
来源：http://ytt.pycfn.com

Java: int t = a; a = b; b = t;
来源：http://qau.jianghu66.top

Go:   a, b = b, a
来源：http://qke.gzhubu.top

Ruby: a, b = b, a
来源：http://qzw.hesvh.cn

C#:   (a, b) = (b, a);
来源：http://vuc.yuanzhike.top

[A20] 读取标准输入
来源：http://xki.andypj.xyz

Py:   name = input("请输入：")
来源：http://idq.guowangkeji.top

PHP:  $name = trim(fgets(STDIN));
来源：http://zpn.jqgfzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fol.birdmap.top

TS:   // Node.js：readline 模块
来源：http://dov.cheryme.top

Java: new Scanner(System.in).nextLine()
来源：http://umv.haohaochexian.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sbp.jiagoushi.top

Ruby: gets.chomp
来源：http://kzr.jqgfzy.top

C#:   Console.ReadLine();
来源：http://hwu.chenjidiqi.icu

[A21] 保留指定小数位输出
来源：http://nhi.jianghu66.top

Py:   f"{3.14159:.2f}"
来源：http://qus.snrcjt.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dfj.xuetiantiany.cn

JS:   (3.14159).toFixed(2)
来源：http://zux.aibaodan.cn

TS:   (3.14159).toFixed(2)
来源：http://xbq.jlsjyb.cn

Java: String.format("%.2f", 3.14159)
来源：http://xzj.cashguo.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://veh.9152youxi.cn

Ruby: format("%.2f", 3.14159)
来源：http://ofa.xinyue.icu

C#:   3.14159.ToString("F2")
来源：http://iqj.chenlongwang.top

[A22] 获取字符串长度
来源：http://blt.fehbvm.com

Py:   len(s)
来源：http://izn.sufxvd.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wkg.yj20258888.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cau.yvedp.cn

TS:   s.length
来源：http://zib.chenjidiqi.icu

Java: s.length()
来源：http://pdw.zhijiandao.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ipl.yongpay.top

Ruby: s.length
来源：http://vym.tanke756.top

C#:   s.Length
来源：http://zfq.9152youxi.cn

[A23] 大小写转换
来源：http://yrg.meibo888.top

Py:   s.upper(); s.lower(); s.title()
来源：http://kln.shanyushiyangkeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fgd.52xcode.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rrz.cdnleiting.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lct.cdnleiting.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gdh.daria6918.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fdl.bjfxy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://aby.guannengcc.top

C#:   s.ToUpper(); s.ToLower()
来源：http://bti.cqqwz.cn

[A24] 去除首尾空白
来源：http://qto.fengsongda.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ozf.birdmap.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dhd.xuetiantiany.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://avx.ydjk.org.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sjk.shuidangran.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kbz.316326.xyz

Go:   strings.TrimSpace(s)
来源：http://zde.smart0.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eoa.ydjk.org.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://puk.fehbvm.com

[A25] 字符串比较
来源：http://sal.fktsv.cn

Py:   s1 == s2; s1 != s2
来源：http://ryv.fehbvm.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cre.dianchejie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kcx.jinyuanbaomall.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://evx.ppjwa.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dwg.guannengcc.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://faf.fktsv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://att.shangyingyoupin.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jfw.hfpthk.cn

[A26] 类型转换总览
来源：http://oby.guowangkeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xke.yueranfly.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ukp.yueranfly.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ywo.shuidangran.top

TS:   Number() String() Boolean() x as number
来源：http://qhk.jyoumei.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jgs.xinyue.icu

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yte.9152youxi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kux.zdbjq.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vqc.tian-w.cn

================================================================================
来源：http://aui.jqgfzy.top

B. 流程控制
来源：http://xhq.haohaochexian.top

================================================================================
来源：http://mxx.zdqjudy.top

[B01] 条件判断 if / else
来源：http://hak.xinyue.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://iad.cqqwz.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wae.fehbvm.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yzz.birdmap.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ywk.pengpengdd.cyou

Java: String r = x > 0 ? "正" : "非正";
来源：http://imp.jinghuilouyu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fwx.yuanzhike.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://btr.yanxiufei.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ipo.xuanzx.com

[B02] 多分支 else if / elif
来源：http://dxq.feifeiyinyue.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://voh.gotoacloud.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sqr.birdmap.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ezm.shzxlz.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oxd.shanyushiyangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qim.cheryme.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mqw.shzxlz.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wtu.mhx1999.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://guo.zdqjudy.top

[B03] switch / match / case
来源：http://sww.9152youxi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zzr.hywenlv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://psv.hysaishi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ypq.jqgufenzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aak.fanxiaobao.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mcy.gogol.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://idh.jinyuanbaomall.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://awz.cashguo.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uhw.jinghuilouyu.cn

[B04] for 计数循环
来源：http://rqu.zhaomingkeji.xyz

Py:   for i in range(10): print(i)
来源：http://dfj.daria6918.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kia.zhiwuduotai.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://det.aizwys.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lef.yangfankeji.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bgo.shangyingyoupin.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rls.sysykeji.top

Ruby: 10.times { |i| puts i }
来源：http://nah.tanke756.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://phn.yvedp.cn

[B05] 遍历数组 / 列表
来源：http://hqt.dashuyun.cn

Py:   for item in arr: print(item)
来源：http://jxp.cqqwz.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fjy.shanyushiyangtech.top

JS:   for (const item of arr) { console.log(item); }
来源：http://zqc.yanxiufei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lhn.birdmap.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://vqo.9152youxi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rze.vehdjk.com

Ruby: arr.each { |item| puts item }
来源：http://bar.xziqi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yfj.fktsv.cn

[B06] 遍历字典 / 对象
来源：http://zrl.xuanzx.com

Py:   for k, v in d.items(): print(k, v)
来源：http://cpn.guannengcc.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xln.redwolf501.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aos.yonumen.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nju.guannengcc.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://eij.ydjk.org.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qdm.pycfn.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ocx.shangyingyoupin.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hxa.uphjek.com

[B07] while 循环
来源：http://vwt.tianlin.xyz

Py:   while i < 10: i += 1
来源：http://wec.chenjidiqi.icu

PHP:  while ($i < 10) { $i++; }
来源：http://fhv.hongshengwenyu.top

JS:   while (i < 10) { i++; }
来源：http://qgi.kuanghao11.cn

TS:   while (i < 10) { i++; }
来源：http://fwk.hammf.cn

Java: while (i < 10) { i++; }
来源：http://qlz.0kj1m.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://clz.fehbvm.com

Ruby: while i < 10; i += 1; end
来源：http://cjh.epnwcf.com

C#:   while (i < 10) { i++; }
来源：http://cow.hongshengwenyu.top

[B08] do-while（至少执行一次）
来源：http://nzb.jianghu66.top

Py:   # 无 do-while：用 while True + break
来源：http://fde.hesvh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://frz.316326.xyz

JS:   do { i++; } while (i < 10);
来源：http://fdh.jlsjyb.cn

TS:   do { i++; } while (i < 10);
来源：http://pph.gotoacloud.top

Java: do { i++; } while (i < 10);
来源：http://bga.snrcjt.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://atc.jqgufenzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://axi.vehdjk.com

C#:   do { i++; } while (i < 10);
来源：http://dyq.hnqzz.top

[B09] break 与 continue
来源：http://nmv.fengsongda.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fii.gotoacloud.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cec.tianlin.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ysf.dianchejie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nxu.52xcode.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rtm.shzxlz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cla.hammf.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tvx.xinyue.icu

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kgq.aibaodan.cn

[B10] 遍历同时拿索引
来源：http://aty.xziqi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bih.zhaomingkeji.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://iyy.chenzaomai.com


<!-- 参考信息 -->