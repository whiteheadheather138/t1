代发 wailian999

[A06] 字符串转数字
来源：http://met.xylfe.cn

Py:   int("42"); float("3.14")
来源：http://tyd.aibaodan.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hkh.jqgufenzy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tbr.chenjidiqi.icu

TS:   parseInt("42", 10); Number("42")
来源：http://nzs.yuxming.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bej.nanxuanxn.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ffn.gaohongyu789.top

Ruby: "42".to_i; "3.14".to_f
来源：http://xpt.vehdjk.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ikw.zhiwuduotai.top

[A07] 数字转字符串
来源：http://gfs.mhx1999.top

Py:   str(42)
来源：http://pas.shanyushiyangtech.top

PHP:  (string) 42; strval(42)
来源：http://zms.sufxvd.cn

JS:   String(42); (42).toString()
来源：http://mwp.xziqi.cn

TS:   String(42)
来源：http://evq.yueranfly.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://hef.hesvh.cn

Go:   strconv.Itoa(42)
来源：http://lrv.chenzaomai.com

Ruby: 42.to_s
来源：http://jny.wangshuangyany.cn

C#:   42.ToString()
来源：http://djs.hongshengwenyu.top

[A08] 取整与四舍五入
来源：http://usc.zdbjq.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jpy.9152youxi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zzr.cdnleiting.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xuh.cucudq.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://glw.aibaodan.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qrh.xinyue.icu

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://iva.sufxvd.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gkp.c1oappe.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xeq.andypj.xyz

[A09] 绝对值与最大最小值
来源：http://bju.fktsv.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vpb.zhijiandao.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vas.birdmap.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ovj.tanke756.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://eqe.jlsjyb.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rpa.9152youxi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hjr.jlsjyb.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://idn.jinghuilouyu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://oum.cqqwz.cn

[A10] 生成随机数
来源：http://vhx.52xcode.cn

Py:   import random; random.randint(1, 100)
来源：http://fvg.jlsjyb.cn

PHP:  random_int(1, 100);
来源：http://faf.jqgfzy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ksz.zdbjq.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zgc.dashuyun.cn

Java: new Random().nextInt(100) + 1
来源：http://rpx.daxiang520.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xbl.9152youxi.cn

Ruby: rand(1..100)
来源：http://eog.shzxlz.cn

C#:   new Random().Next(1, 101)
来源：http://kev.aizwys.cn

[A11] 条件表达式（三元）
来源：http://djl.yueranfly.top

Py:   "yes" if x > 0 else "no"
来源：http://roo.pycfn.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://grz.chenjidiqi.icu

JS:   x > 0 ? "yes" : "no"
来源：http://bfn.shangyingyoupin.top

TS:   x > 0 ? "yes" : "no"
来源：http://cty.tianlin.xyz

Java: x > 0 ? "yes" : "no"
来源：http://foc.jiagoushi.top

Go:   // 无三元运算符，需用 if 语句
来源：http://odu.hcnkem.com

Ruby: x > 0 ? "yes" : "no"
来源：http://fxz.316326.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://qar.hfpthk.cn

[A12] 字符串插值 / 格式化
来源：http://cga.0kj1m.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kwh.fzhhl.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pcn.nanxuanxn.top

JS:   `Hello, ${name}!`
来源：http://nab.guannengcc.top

TS:   `Hello, ${name}!`
来源：http://pei.tianlin.xyz

Java: "Hello, %s!".formatted(name)
来源：http://hxf.daria6918.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nma.sysykeji.top

Ruby: "Hello, #{name}!"
来源：http://nex.gotoacloud.top

C#:   $"Hello, {name}!"
来源：http://ohb.52xcode.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://kra.yuxming.cn

Py:   "第一行\n第二行"
来源：http://uwi.bbcook.cn

PHP:  "第一行\n第二行"
来源：http://cwf.xingfuxueyuan.xyz

JS:   "第一行\n第二行"
来源：http://zlb.jiagoushi.top

TS:   "第一行\n第二行"
来源：http://pqk.bbcook.cn

Java: "第一行\n第二行"
来源：http://ubt.tian-w.cn

Go:   "第一行\n第二行"
来源：http://gtr.52xcode.cn

Ruby: "第一行\n第二行"
来源：http://moz.tarul.cn

C#:   "第一行\n第二行"
来源：http://tos.aizwys.cn

[A14] 注释写法
来源：http://ldk.nanxinkj.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://kff.vehdjk.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://qsa.zhongyouzk.top

JS:   // 单行；/* 多行 */
来源：http://xre.jinyuanbaomall.cn

TS:   // 单行；/* 多行 */
来源：http://azu.cdnleiting.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gre.jianghu66.top

Go:   // 单行；/* 多行 */
来源：http://pjx.hesvh.cn

Ruby: # 单行；=begin 多行 =end
来源：http://yzg.cashguo.top

C#:   // 单行；/* 多行 */
来源：http://ctc.nwbrower.top

[A15] 空值判断与默认值
来源：http://bqu.yuanzhike.top

Py:   value = data or "默认值"
来源：http://yde.zycfv.cn

PHP:  $value = $data ?? "默认值";
来源：http://hse.ivvv.top

JS:   const value = data ?? "默认值";
来源：http://rag.zhoulong.xyz

TS:   const value = data ?? "默认值";
来源：http://hfl.jinyuanbaomall.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tnw.nanxinkj.top

Go:   if data == "" { data = "默认值" }
来源：http://xvu.guannengcc.top

Ruby: value = data || "默认值"
来源：http://xcp.guowangkeji.top

C#:   var value = data ?? "默认值";
来源：http://peo.sxryk.cn

[A16] 真假值判断规则
来源：http://udw.zhaomingkeji.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fhv.smart0.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hyj.jiagoushi.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nkv.shanyushiyangkeji.top

TS:   if (!x) {}
来源：http://rir.birdmap.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bis.c1oappe.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hse.uphjek.com

Ruby: unless x            # nil 与 false 为假
来源：http://kia.tarul.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fzc.redwolf501.top

[A17] 位运算
来源：http://qvm.ehwqpu.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cyg.havefunace.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hmz.ctjpmb.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oet.jianghu66.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://knt.dashuyun.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jzd.uphjek.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xxt.0kj1m.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xvz.shzxlz.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tlz.cheryme.top

[A18] 字符与 ASCII 码互转
来源：http://pza.zhongyouzk.top

Py:   ord("A"); chr(65)
来源：http://rex.bjfxy.top

PHP:  ord("A"); chr(65)
来源：http://dva.yj20258.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uus.daxiang520.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pfp.tarul.cn

Java: (int) 'A'; (char) 65
来源：http://bcx.zdbjq.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://njo.jqgfzy.top

Ruby: "A".ord; 65.chr
来源：http://ubv.gogol.net.cn

C#:   (int)'A'; (char)65
来源：http://uom.yongpay.top

[A19] 交换两个变量
来源：http://zyh.shangyingyoupin.top

Py:   a, b = b, a
来源：http://ten.jqgfzy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ycd.sysykeji.top

JS:   [a, b] = [b, a];
来源：http://tef.jqgufenzy.top

TS:   [a, b] = [b, a];
来源：http://lbf.jinqigfzy.top

Java: int t = a; a = b; b = t;
来源：http://idx.fengsongda.top

Go:   a, b = b, a
来源：http://mer.yongpay.top

Ruby: a, b = b, a
来源：http://ugj.gotoacloud.top

C#:   (a, b) = (b, a);
来源：http://lma.ehwqpu.com

[A20] 读取标准输入
来源：http://xlk.shzxlz.cn

Py:   name = input("请输入：")
来源：http://han.dianchejie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://bzz.nanxuanxn.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ghf.aibaodan.cn

TS:   // Node.js：readline 模块
来源：http://mji.xuanzx.com

Java: new Scanner(System.in).nextLine()
来源：http://ebf.ppjwa.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gsq.kuanghao11.cn

Ruby: gets.chomp
来源：http://zar.jianghu66.top

C#:   Console.ReadLine();
来源：http://qhj.jqgufenzy.top

[A21] 保留指定小数位输出
来源：http://hkt.hysaishi.cn

Py:   f"{3.14159:.2f}"
来源：http://gwk.epnwcf.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dvq.vqdsnc.cn

JS:   (3.14159).toFixed(2)
来源：http://vho.shuidangran.top

TS:   (3.14159).toFixed(2)
来源：http://ogc.yj20258888.top

Java: String.format("%.2f", 3.14159)
来源：http://tgj.sufxvd.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uex.zhengqikj.top

Ruby: format("%.2f", 3.14159)
来源：http://tlq.zhoulong.xyz

C#:   3.14159.ToString("F2")
来源：http://dyl.sxryk.cn

[A22] 获取字符串长度
来源：http://tbz.chenzaomai.com

Py:   len(s)
来源：http://kqo.redwolf501.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rxo.epnwcf.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xfx.316326.xyz

TS:   s.length
来源：http://lrg.shangyingyoupin.top

Java: s.length()
来源：http://yjz.hesvh.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yun.fehbvm.com

Ruby: s.length
来源：http://wlr.wangshuangyany.cn

C#:   s.Length
来源：http://opz.sweek.top

[A23] 大小写转换
来源：http://dyq.zhaomingkeji.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://jvb.cdnleiting.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://acf.fengsongda.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sfs.fktsv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xqs.zhiwuduotai.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zim.shuidangran.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ysg.ydjk.org.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://syq.sxryk.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://chk.hcnkem.com

[A24] 去除首尾空白
来源：http://tuf.gogol.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dpn.aibaodan.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://abl.zhijiandao.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yql.316326.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ehc.ivvv.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dhd.dianchejie.cn

Go:   strings.TrimSpace(s)
来源：http://snx.shangyingyoupin.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://est.tanke756.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xgm.nwbrower.top

[A25] 字符串比较
来源：http://tsi.cheryme.top

Py:   s1 == s2; s1 != s2
来源：http://lwj.yangfankeji.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xap.ctjpmb.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jmc.chenjidiqi.icu

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wra.xuanzx.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://awm.daxiang520.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xyj.hysaishi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gfv.sufxvd.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mec.wangshuangyany.cn

[A26] 类型转换总览
来源：http://flf.fktsv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ywi.zhongyouzk.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gju.shangyingyoupin.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rtz.guowangkeji.top

TS:   Number() String() Boolean() x as number
来源：http://cvf.sxryk.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lpw.zhongyouzk.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ahi.aibaodan.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://sxs.feifeiyinyue.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dvb.pycfn.com

================================================================================
来源：http://mqo.xylfe.cn

B. 流程控制
来源：http://qsd.shuidangran.top

================================================================================
来源：http://gff.svipenyu.cn

[B01] 条件判断 if / else
来源：http://usm.sysykeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://rex.fehbvm.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://olb.jinghuilouyu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://umu.c1oappe.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mpa.chenzaomai.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://fbv.jyoumei.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zzo.fzhhl.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fjw.xuetiantiany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://aqt.ivvv.top

[B02] 多分支 else if / elif
来源：http://pfb.pengpengdd.cyou

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mis.c1oappe.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mad.cashguo.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qvq.jianghu66.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fxe.yonumen.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iee.quarkkingdee.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://khj.gzhubu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ruw.xingfuxueyuan.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ncs.ybcxt.top

[B03] switch / match / case
来源：http://rdx.guowangkeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rxg.shangyingyoupin.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tlt.ybcxt.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://odc.52xcode.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gmp.feifeiyinyue.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qes.chenjidiqi.icu

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kga.ybcxt.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pqj.shanyushiyangtech.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hkc.hywenlv.cn

[B04] for 计数循环
来源：http://shy.bbcook.cn

Py:   for i in range(10): print(i)
来源：http://pvc.shanyushiyangtech.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zgq.hammf.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jnc.quarkkingdee.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kra.fengsongda.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zdm.shangyingyoupin.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xtv.cdnleiting.top

Ruby: 10.times { |i| puts i }
来源：http://flw.gogol.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://who.sufxvd.cn

[B05] 遍历数组 / 列表
来源：http://ybm.hongshengwenyu.top

Py:   for item in arr: print(item)
来源：http://imi.sufxvd.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://med.guannengcc.top

JS:   for (const item of arr) { console.log(item); }
来源：http://uos.sweek.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ard.hesvh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rdm.jiagoushi.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ofe.jinyuanbaomall.cn

Ruby: arr.each { |item| puts item }
来源：http://wjm.chenzaomai.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gls.epnwcf.com

[B06] 遍历字典 / 对象
来源：http://hfy.sysykeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ixv.chenlongwang.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://etb.shuidangran.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uho.daria6918.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kdn.xuanzx.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gyv.316326.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pkd.hnxiangtu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nlj.xingfuxueyuan.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gey.birdmap.top

[B07] while 循环
来源：http://ade.vehdjk.com

Py:   while i < 10: i += 1
来源：http://zgg.hesvh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ssi.snrcjt.cn

JS:   while (i < 10) { i++; }
来源：http://ehq.havefunace.top

TS:   while (i < 10) { i++; }
来源：http://cbg.yonumen.top

Java: while (i < 10) { i++; }
来源：http://zkv.kuanghao11.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ouj.sxryk.cn

Ruby: while i < 10; i += 1; end
来源：http://did.jinqigfzy.top

C#:   while (i < 10) { i++; }
来源：http://wqb.bbcook.cn

[B08] do-while（至少执行一次）
来源：http://cuk.vehdjk.com

Py:   # 无 do-while：用 while True + break
来源：http://yno.ydzc1.top

PHP:  do { $i++; } while ($i < 10);
来源：http://qfd.jinyuanbaomall.cn

JS:   do { i++; } while (i < 10);
来源：http://nba.yangfankeji.com

TS:   do { i++; } while (i < 10);
来源：http://ifa.snrcjt.cn

Java: do { i++; } while (i < 10);
来源：http://hhn.316326.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://jau.hysaishi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zgk.zdbjq.cn

C#:   do { i++; } while (i < 10);
来源：http://dcf.ydjk.org.cn

[B09] break 与 continue
来源：http://ild.fengsongda.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kyp.havefunace.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oau.xylfe.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wrj.fanxiaobao.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://owd.ywan-chungtsiang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pug.zhaomingkeji.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kra.havefunace.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hdg.hnxiangtu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uym.sweek.top

[B10] 遍历同时拿索引
来源：http://wjp.xziqi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hlq.chenlongwang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jca.jinqigfzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wcc.daxiang520.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mpm.svipenyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jeo.daria6918.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vat.zhiwuduotai.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fxp.bjfxy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hhr.quarkkingdee.top

[B11] 生成数字序列 / 区间
来源：http://oyw.pycfn.com

Py:   list(range(0, 10, 2))
来源：http://xzo.jiagoushi.top

PHP:  range(0, 10, 2);
来源：http://prg.zhixingplan.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wmr.jyoumei.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ltc.zhixingplan.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ydu.sjlbkw.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uad.pengpengdd.cyou

Ruby: (0...10).step(2).to_a
来源：http://gzj.jqgfzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://svf.chenjidiqi.icu

[B12] 跳出多层循环
来源：http://ewj.yueranfly.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gbx.xinyue.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://oac.uphjek.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eck.epnwcf.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://byx.hcnkem.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zot.yueranfly.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lst.cqqwz.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vxp.zhoulong.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uvf.sxryk.cn


<!-- 参考信息 -->