代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zmj.shangyingyoupin.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://utp.zycfv.cn

TS:   typeof x; x instanceof Date
来源：http://gwn.yuanzhike.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://toe.xuetiantiany.cn

Go:   reflect.TypeOf(x).Name()
来源：http://biz.ywan-chungtsiang.top

Ruby: x.class; x.is_a?(Integer)
来源：http://jam.epnwcf.com

C#:   x.GetType().Name; x is int
来源：http://xov.sxryk.cn

[A05] 整数除法与取模
来源：http://hml.zhongyouzk.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xfe.cucudq.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fxi.fanxiaobao.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pzo.guannengcc.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nqc.dianchejie.cn

Java: 7 / 2; 7 % 2
来源：http://gyn.yangfankeji.com

Go:   7 / 2; 7 % 2
来源：http://xtj.dianchejie.cn

Ruby: 7 / 2; 7 % 2
来源：http://shn.ydzc1.top

C#:   7 / 2; 7 % 2
来源：http://twh.yuanzhike.top

[A06] 字符串转数字
来源：http://avz.uphjek.com

Py:   int("42"); float("3.14")
来源：http://ynw.redwolf501.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vxd.guowangkeji.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uih.yj20258.top

TS:   parseInt("42", 10); Number("42")
来源：http://pkj.redwolf501.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dlj.316326.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ptq.0kj1m.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://eny.nanxuanxn.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vch.yvedp.cn

[A07] 数字转字符串
来源：http://vrx.chenjidiqi.icu

Py:   str(42)
来源：http://aau.yueranfly.top

PHP:  (string) 42; strval(42)
来源：http://ovv.tian-w.cn

JS:   String(42); (42).toString()
来源：http://ezv.snrcjt.cn

TS:   String(42)
来源：http://gwf.c1oappe.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://sny.xuanzx.com

Go:   strconv.Itoa(42)
来源：http://dgo.xylfe.cn

Ruby: 42.to_s
来源：http://gsc.xuetiantiany.cn

C#:   42.ToString()
来源：http://xvq.cqqwz.cn

[A08] 取整与四舍五入
来源：http://fck.chenjidiqi.icu

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dyl.pengpengdd.cyou

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vlf.gotoacloud.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vap.wangshuangyany.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://swq.smart0.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tja.fanxiaobao.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zyf.cucudq.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://epm.sxryk.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qtx.yj202588.top

[A09] 绝对值与最大最小值
来源：http://dus.fanxiaobao.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://whr.redwolf501.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vgt.shanyushiyangtech.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lcx.zdbjq.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rze.jinyuanbaomall.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://olt.guowangkeji.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ema.fengsongda.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lfl.guannengcc.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://oma.pengpengdd.cyou

[A10] 生成随机数
来源：http://jiw.hfpthk.cn

Py:   import random; random.randint(1, 100)
来源：http://mzp.fanxiaobao.xyz

PHP:  random_int(1, 100);
来源：http://bip.chenlongwang.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ena.andypj.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rzu.tian-w.cn

Java: new Random().nextInt(100) + 1
来源：http://dxq.aizwys.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qgd.nanxuanxn.top

Ruby: rand(1..100)
来源：http://sjg.tanke756.top

C#:   new Random().Next(1, 101)
来源：http://ssi.vehdjk.com

[A11] 条件表达式（三元）
来源：http://hdr.redwolf501.top

Py:   "yes" if x > 0 else "no"
来源：http://jxd.fanxiaobao.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://rfr.shzxlz.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qqt.yueranfly.top

TS:   x > 0 ? "yes" : "no"
来源：http://yva.uphjek.com

Java: x > 0 ? "yes" : "no"
来源：http://vhh.chenzaomai.com

Go:   // 无三元运算符，需用 if 语句
来源：http://wai.yj202588.top

Ruby: x > 0 ? "yes" : "no"
来源：http://yxa.yueranfly.top

C#:   x > 0 ? "yes" : "no"
来源：http://qir.shangyingyoupin.top

[A12] 字符串插值 / 格式化
来源：http://djt.wangshuangyany.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ldw.cashguo.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://anh.fzhhl.top

JS:   `Hello, ${name}!`
来源：http://hrw.hnqzz.top

TS:   `Hello, ${name}!`
来源：http://rof.wangshuangyany.cn

Java: "Hello, %s!".formatted(name)
来源：http://cmv.zhaomingkeji.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://joy.sufxvd.cn

Ruby: "Hello, #{name}!"
来源：http://syv.sjlbkw.cn

C#:   $"Hello, {name}!"
来源：http://lxd.yueranfly.top

[A13] 多行字符串（练习 \n 转义）
来源：http://gnm.snrcjt.cn

Py:   "第一行\n第二行"
来源：http://vuy.xylfe.cn

PHP:  "第一行\n第二行"
来源：http://mwp.feifeiyinyue.top

JS:   "第一行\n第二行"
来源：http://lbd.cheryme.top

TS:   "第一行\n第二行"
来源：http://yrk.tian-w.cn

Java: "第一行\n第二行"
来源：http://veh.aizwys.cn

Go:   "第一行\n第二行"
来源：http://oag.sufxvd.cn

Ruby: "第一行\n第二行"
来源：http://lnu.c1oappe.top

C#:   "第一行\n第二行"
来源：http://cmp.jyoumei.cn

[A14] 注释写法
来源：http://xdt.dianchejie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://uhy.hesvh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://adc.dashuyun.cn

JS:   // 单行；/* 多行 */
来源：http://wzy.nanxuanxn.top

TS:   // 单行；/* 多行 */
来源：http://znq.gaohongyu789.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://woh.hongshengwenyu.top

Go:   // 单行；/* 多行 */
来源：http://idz.chenlongwang.top

Ruby: # 单行；=begin 多行 =end
来源：http://qlf.dashuyun.cn

C#:   // 单行；/* 多行 */
来源：http://rny.zdbjq.cn

[A15] 空值判断与默认值
来源：http://vwe.cheryme.top

Py:   value = data or "默认值"
来源：http://hje.daxiang520.top

PHP:  $value = $data ?? "默认值";
来源：http://wsj.sweek.top

JS:   const value = data ?? "默认值";
来源：http://uyb.aibaodan.cn

TS:   const value = data ?? "默认值";
来源：http://acu.vehdjk.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hiz.vqdsnc.cn

Go:   if data == "" { data = "默认值" }
来源：http://xun.tanke756.top

Ruby: value = data || "默认值"
来源：http://rhh.zhoulong.xyz

C#:   var value = data ?? "默认值";
来源：http://frd.yvedp.cn

[A16] 真假值判断规则
来源：http://jcb.daxiang520.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ary.zhaomingkeji.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dlq.yuxming.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://chl.bbcook.cn

TS:   if (!x) {}
来源：http://xvf.andypj.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rbt.52xcode.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lyi.vqdsnc.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qey.yfazqb.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nfa.pengpengdd.cyou

[A17] 位运算
来源：http://qrc.dianchejie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pnr.svipenyu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nru.xziqi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wdt.wangshuangyany.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fkz.cdnleiting.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vfs.epnwcf.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ijd.hammf.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kql.haohaochexian.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hwd.zycfv.cn

[A18] 字符与 ASCII 码互转
来源：http://ksf.hesvh.cn

Py:   ord("A"); chr(65)
来源：http://bhf.xuanzx.com

PHP:  ord("A"); chr(65)
来源：http://wjw.yuxming.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qyx.ivvv.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vus.ydjk.org.cn

Java: (int) 'A'; (char) 65
来源：http://lbd.dashuyun.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://myb.yj20258.top

Ruby: "A".ord; 65.chr
来源：http://rzf.quarkkingdee.top

C#:   (int)'A'; (char)65
来源：http://zvg.quarkkingdee.top

[A19] 交换两个变量
来源：http://pzn.xingfuxueyuan.xyz

Py:   a, b = b, a
来源：http://dsj.yfazqb.com

PHP:  [$a, $b] = [$b, $a];
来源：http://ebz.andypj.xyz

JS:   [a, b] = [b, a];
来源：http://idb.jianghu66.top

TS:   [a, b] = [b, a];
来源：http://tpx.hywenlv.cn

Java: int t = a; a = b; b = t;
来源：http://odw.shzxlz.cn

Go:   a, b = b, a
来源：http://jod.pengpengdd.cyou

Ruby: a, b = b, a
来源：http://oiu.hammf.cn

C#:   (a, b) = (b, a);
来源：http://qnl.xinyue.icu

[A20] 读取标准输入
来源：http://oeh.ybcxt.top

Py:   name = input("请输入：")
来源：http://cpt.zhiwuduotai.top

PHP:  $name = trim(fgets(STDIN));
来源：http://dav.birdmap.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nfe.smart0.xyz

TS:   // Node.js：readline 模块
来源：http://jwy.xziqi.cn

Java: new Scanner(System.in).nextLine()
来源：http://xas.yj20258888.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mbw.shanyushiyangkeji.top

Ruby: gets.chomp
来源：http://uvy.zhiwuduotai.top

C#:   Console.ReadLine();
来源：http://bsh.svipenyu.cn

[A21] 保留指定小数位输出
来源：http://clv.zhiwuduotai.top

Py:   f"{3.14159:.2f}"
来源：http://zzr.yangfankeji.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pce.jqgufenzy.top

JS:   (3.14159).toFixed(2)
来源：http://rwu.nanxuanxn.top

TS:   (3.14159).toFixed(2)
来源：http://afr.jinyuanbaomall.cn

Java: String.format("%.2f", 3.14159)
来源：http://bxh.yvedp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jmf.aibaodan.cn

Ruby: format("%.2f", 3.14159)
来源：http://erc.yanxiufei.cn

C#:   3.14159.ToString("F2")
来源：http://fir.hnqzz.top

[A22] 获取字符串长度
来源：http://xni.yj20258888.top

Py:   len(s)
来源：http://djp.hywenlv.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hbu.iojbl.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dsm.haohaochexian.top

TS:   s.length
来源：http://mgn.yanxiufei.cn

Java: s.length()
来源：http://mur.tian-w.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sup.0kj1m.cn

Ruby: s.length
来源：http://quy.kuanghao11.cn

C#:   s.Length
来源：http://kts.yj202588.top

[A23] 大小写转换
来源：http://doo.fehbvm.com

Py:   s.upper(); s.lower(); s.title()
来源：http://vtb.ybcxt.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yus.fanxiaobao.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://urn.gzhubu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xpa.shangyingyoupin.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cew.mhx1999.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pzr.iojbl.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://opp.cqqwz.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zcs.bjfxy.top

[A24] 去除首尾空白
来源：http://oic.ppjwa.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dfm.dianchejie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://orf.birdmap.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ubd.uphjek.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pcz.cdnleiting.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gfj.zdbjq.cn

Go:   strings.TrimSpace(s)
来源：http://bmw.cashguo.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gyb.yanxiufei.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kcw.aizwys.cn

[A25] 字符串比较
来源：http://eyl.pycfn.com

Py:   s1 == s2; s1 != s2
来源：http://prv.fanxiaobao.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://icm.zycfv.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cjj.jqgufenzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lhz.zhixingplan.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fnt.zdqjudy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hbz.zdbjq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rzs.gaohongyu789.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://esh.hywenlv.cn

[A26] 类型转换总览
来源：http://hwk.wangdashe.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dxo.zhiwuduotai.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jnq.yangfankeji.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tvv.kuanghao11.cn

TS:   Number() String() Boolean() x as number
来源：http://auf.jqgufenzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pdm.gotoacloud.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qhc.yuxming.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gwg.cheryme.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://shu.andypj.xyz

================================================================================
来源：http://qmg.meibo888.top

B. 流程控制
来源：http://uks.havefunace.top

================================================================================
来源：http://xnz.jianghu66.top

[B01] 条件判断 if / else
来源：http://ngb.xziqi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hli.cheryme.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://afn.xylfe.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ocb.yangfankeji.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pfv.snrcjt.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dcz.hongshengwenyu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://src.jqgufenzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lml.xuetiantiany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ijh.andypj.xyz

[B02] 多分支 else if / elif
来源：http://nyh.ppjwa.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yke.shzxlz.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bdm.fktsv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fow.tianlin.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vzt.hcnkem.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://szp.meibo888.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hqz.zhixingplan.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vls.iojbl.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pwr.xinyue.icu

[B03] switch / match / case
来源：http://crf.tian-w.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jxc.havefunace.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tqi.hammf.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://msj.cashguo.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rfr.hnqzz.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rad.iojbl.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yyg.iojbl.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ort.jinyuanbaomall.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vgn.zhixingplan.top

[B04] for 计数循环
来源：http://pxe.ehwqpu.com

Py:   for i in range(10): print(i)
来源：http://djl.ydzc1.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://drp.ywan-chungtsiang.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ugs.ydzc1.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pmd.shzxlz.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iae.birdmap.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lal.redwolf501.top

Ruby: 10.times { |i| puts i }
来源：http://kxm.zdqjudy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rfe.yj20258.top

[B05] 遍历数组 / 列表
来源：http://nuf.dianchejie.cn

Py:   for item in arr: print(item)
来源：http://wju.kuanghao11.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://abt.cashguo.top

JS:   for (const item of arr) { console.log(item); }
来源：http://wfi.zhiwuduotai.top

TS:   for (const item of arr) { console.log(item); }
来源：http://uew.fktsv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hkj.dianchejie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fye.feifeiyinyue.top

Ruby: arr.each { |item| puts item }
来源：http://mkg.chenlongwang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xfs.sufxvd.cn

[B06] 遍历字典 / 对象
来源：http://der.fanxiaobao.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://yvl.pengpengdd.cyou

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rat.zdqjudy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gbd.hnxiangtu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vxx.mhx1999.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ecr.jinqigfzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zkd.hfpthk.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wwu.zdqjudy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fvk.hongshengwenyu.top

[B07] while 循环
来源：http://ikg.zdqjudy.top

Py:   while i < 10: i += 1
来源：http://ded.bjfxy.top

PHP:  while ($i < 10) { $i++; }
来源：http://sft.guowangkeji.top

JS:   while (i < 10) { i++; }
来源：http://zgl.yvedp.cn

TS:   while (i < 10) { i++; }
来源：http://kns.andypj.xyz

Java: while (i < 10) { i++; }
来源：http://ucx.316326.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rxr.tianlin.xyz

Ruby: while i < 10; i += 1; end
来源：http://wua.yfazqb.com

C#:   while (i < 10) { i++; }
来源：http://zvp.cqqwz.cn

[B08] do-while（至少执行一次）
来源：http://urx.xuanzx.com

Py:   # 无 do-while：用 while True + break
来源：http://vdd.hfpthk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tvc.pengpengdd.cyou

JS:   do { i++; } while (i < 10);
来源：http://hmc.snrcjt.cn

TS:   do { i++; } while (i < 10);
来源：http://ksy.gzhubu.top

Java: do { i++; } while (i < 10);
来源：http://ygb.jinqigufen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://osp.shangyingyoupin.top

Ruby: begin; i += 1; end while i < 10
来源：http://mkn.bbcook.cn

C#:   do { i++; } while (i < 10);
来源：http://oqm.hnqzz.top

[B09] break 与 continue
来源：http://aud.ivvv.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sno.havefunace.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pxv.yj202588.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yrj.gotoacloud.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qbc.vehdjk.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mpk.0kj1m.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ilo.haohaochexian.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lca.sjlbkw.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://igj.zhiwuduotai.top

[B10] 遍历同时拿索引
来源：http://czb.shzxlz.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://muw.vehdjk.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xhk.zhengqikj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xne.uphjek.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://aly.fengsongda.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ame.jinyuanbaomall.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hbq.dianchejie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://usc.ywan-chungtsiang.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yqo.yj20258.top

[B11] 生成数字序列 / 区间
来源：http://tqp.cqqwz.cn

Py:   list(range(0, 10, 2))
来源：http://qma.jinqigfzy.top


<!-- 参考信息 -->