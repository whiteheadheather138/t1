代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://rcr.316326.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://skc.chenzaomai.com

C#:   x.GetType().Name; x is int
来源：http://szz.aibaodan.cn

[A05] 整数除法与取模
来源：http://tcj.uphjek.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yyo.tanke756.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ivn.yanxiufei.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pmp.sufxvd.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rll.jiagoushi.top

Java: 7 / 2; 7 % 2
来源：http://gac.xuetiantiany.cn

Go:   7 / 2; 7 % 2
来源：http://cvm.hongshengwenyu.top

Ruby: 7 / 2; 7 % 2
来源：http://dwz.ybcxt.top

C#:   7 / 2; 7 % 2
来源：http://doz.mhx1999.top

[A06] 字符串转数字
来源：http://slh.mhx1999.top

Py:   int("42"); float("3.14")
来源：http://zno.bbcook.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://euk.dianchejie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cmc.cqqwz.cn

TS:   parseInt("42", 10); Number("42")
来源：http://obq.sxryk.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nhf.yongpay.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qez.iojbl.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wlm.yongpay.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sdj.ppjwa.cn

[A07] 数字转字符串
来源：http://ugk.hfpthk.cn

Py:   str(42)
来源：http://fza.tarul.cn

PHP:  (string) 42; strval(42)
来源：http://eor.zdbjq.cn

JS:   String(42); (42).toString()
来源：http://wjp.iojbl.cn

TS:   String(42)
来源：http://vjs.cdnleiting.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://hlu.zhijiandao.cn

Go:   strconv.Itoa(42)
来源：http://uvd.mhx1999.top

Ruby: 42.to_s
来源：http://znu.iojbl.cn

C#:   42.ToString()
来源：http://oje.cheryme.top

[A08] 取整与四舍五入
来源：http://vhv.jyoumei.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yrk.jinghuilouyu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://iok.daxiang520.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vtf.fzhhl.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://flj.xingfuxueyuan.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xnd.xuanzx.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qki.yfazqb.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://abv.cucudq.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tuu.nwbrower.top

[A09] 绝对值与最大最小值
来源：http://rbp.kuanghao11.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dbd.fengsongda.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nue.zhixingplan.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ipu.aibaodan.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hrq.zycfv.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qcn.ydjk.org.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://eoa.vehdjk.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ljo.jinyuanbaomall.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xra.sjlbkw.cn

[A10] 生成随机数
来源：http://fka.zhongyouzk.top

Py:   import random; random.randint(1, 100)
来源：http://hzw.guowangkeji.top

PHP:  random_int(1, 100);
来源：http://fhc.nanxuanxn.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qud.cqqwz.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rqp.wangshuangyany.cn

Java: new Random().nextInt(100) + 1
来源：http://bpg.mhx1999.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fny.fengsongda.top

Ruby: rand(1..100)
来源：http://gig.sysykeji.top

C#:   new Random().Next(1, 101)
来源：http://vdw.bbcook.cn

[A11] 条件表达式（三元）
来源：http://cjf.chenzaomai.com

Py:   "yes" if x > 0 else "no"
来源：http://ckm.chenzaomai.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://zqh.bbcook.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zdk.hammf.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gue.xingfuxueyuan.xyz

Java: x > 0 ? "yes" : "no"
来源：http://gvn.iojbl.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ubh.haohaochexian.top

Ruby: x > 0 ? "yes" : "no"
来源：http://dvu.sjlbkw.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ydg.epnwcf.com

[A12] 字符串插值 / 格式化
来源：http://lax.hnxiangtu.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uoz.shangyingyoupin.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nxb.hysaishi.cn

JS:   `Hello, ${name}!`
来源：http://tvr.shuidangran.top

TS:   `Hello, ${name}!`
来源：http://nkt.fengsongda.top

Java: "Hello, %s!".formatted(name)
来源：http://zza.birdmap.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kop.aibaodan.cn

Ruby: "Hello, #{name}!"
来源：http://dvo.nwbrower.top

C#:   $"Hello, {name}!"
来源：http://awe.zdqjudy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://fph.andypj.xyz

Py:   "第一行\n第二行"
来源：http://fze.uphjek.com

PHP:  "第一行\n第二行"
来源：http://bjz.fanxiaobao.xyz

JS:   "第一行\n第二行"
来源：http://jff.meibo888.top

TS:   "第一行\n第二行"
来源：http://utx.daxiang520.top

Java: "第一行\n第二行"
来源：http://iwr.jqgfzy.top

Go:   "第一行\n第二行"
来源：http://cbx.yangfankeji.com

Ruby: "第一行\n第二行"
来源：http://jbg.zhengqikj.top

C#:   "第一行\n第二行"
来源：http://uao.iojbl.cn

[A14] 注释写法
来源：http://osu.chenjidiqi.icu

Py:   # 单行；三引号字符串可作多行说明
来源：http://pzw.yj20258.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://qsz.xziqi.cn

JS:   // 单行；/* 多行 */
来源：http://vvt.yangfankeji.com

TS:   // 单行；/* 多行 */
来源：http://dkx.haohaochexian.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://oob.yanxiufei.cn

Go:   // 单行；/* 多行 */
来源：http://nbo.yuxming.cn

Ruby: # 单行；=begin 多行 =end
来源：http://emy.dianchejie.cn

C#:   // 单行；/* 多行 */
来源：http://bqm.quarkkingdee.top

[A15] 空值判断与默认值
来源：http://qvf.yvedp.cn

Py:   value = data or "默认值"
来源：http://wtl.bbcook.cn

PHP:  $value = $data ?? "默认值";
来源：http://ceg.hysaishi.cn

JS:   const value = data ?? "默认值";
来源：http://vlx.jinghuilouyu.cn

TS:   const value = data ?? "默认值";
来源：http://fxj.jqgufenzy.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nqq.fehbvm.com

Go:   if data == "" { data = "默认值" }
来源：http://zcq.tian-w.cn

Ruby: value = data || "默认值"
来源：http://xgv.jiagoushi.top

C#:   var value = data ?? "默认值";
来源：http://hiu.yvedp.cn

[A16] 真假值判断规则
来源：http://ctk.bbcook.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zlj.jqgfzy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jgu.svipenyu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://izr.cheryme.top

TS:   if (!x) {}
来源：http://okv.birdmap.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pau.hywenlv.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://klo.shangyingyoupin.top

Ruby: unless x            # nil 与 false 为假
来源：http://cuo.zhiwuduotai.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vlj.havefunace.top

[A17] 位运算
来源：http://evq.xylfe.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oey.cdnleiting.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://quu.haohaochexian.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jmw.feifeiyinyue.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ejf.tianlin.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xml.xylfe.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ofa.sxryk.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kuf.fehbvm.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://csk.jinghuilouyu.cn

[A18] 字符与 ASCII 码互转
来源：http://ypf.hesvh.cn

Py:   ord("A"); chr(65)
来源：http://xnh.xziqi.cn

PHP:  ord("A"); chr(65)
来源：http://dei.yj20258.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yaz.yj20258.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://obv.dashuyun.cn

Java: (int) 'A'; (char) 65
来源：http://iru.feifeiyinyue.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lls.yj20258888.top

Ruby: "A".ord; 65.chr
来源：http://rff.hnxiangtu.top

C#:   (int)'A'; (char)65
来源：http://rll.hnxiangtu.top

[A19] 交换两个变量
来源：http://gju.hammf.cn

Py:   a, b = b, a
来源：http://abl.jianghu66.top

PHP:  [$a, $b] = [$b, $a];
来源：http://lat.chenjidiqi.icu

JS:   [a, b] = [b, a];
来源：http://pjl.hesvh.cn

TS:   [a, b] = [b, a];
来源：http://wla.jianghu66.top

Java: int t = a; a = b; b = t;
来源：http://xgo.gotoacloud.top

Go:   a, b = b, a
来源：http://bxf.yongpay.top

Ruby: a, b = b, a
来源：http://ifk.ydjk.org.cn

C#:   (a, b) = (b, a);
来源：http://sxf.sxryk.cn

[A20] 读取标准输入
来源：http://uln.smart0.xyz

Py:   name = input("请输入：")
来源：http://gmv.xylfe.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://yon.sweek.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kuu.quarkkingdee.top

TS:   // Node.js：readline 模块
来源：http://nth.hfpthk.cn

Java: new Scanner(System.in).nextLine()
来源：http://ipd.yonumen.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://opd.zhiwuduotai.top

Ruby: gets.chomp
来源：http://qry.hfpthk.cn

C#:   Console.ReadLine();
来源：http://hfe.nwbrower.top

[A21] 保留指定小数位输出
来源：http://xyw.zhongyouzk.top

Py:   f"{3.14159:.2f}"
来源：http://urv.yfazqb.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zxl.zhoulong.xyz

JS:   (3.14159).toFixed(2)
来源：http://ayh.dashuyun.cn

TS:   (3.14159).toFixed(2)
来源：http://qeq.hnqzz.top

Java: String.format("%.2f", 3.14159)
来源：http://zjl.shangyingyoupin.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kpi.haohaochexian.top

Ruby: format("%.2f", 3.14159)
来源：http://epx.shzxlz.cn

C#:   3.14159.ToString("F2")
来源：http://oys.sweek.top

[A22] 获取字符串长度
来源：http://tzi.sweek.top

Py:   len(s)
来源：http://wgo.xylfe.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xsa.vehdjk.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kdm.pycfn.com

TS:   s.length
来源：http://pjz.mhx1999.top

Java: s.length()
来源：http://tde.uphjek.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wfp.redwolf501.top

Ruby: s.length
来源：http://uhl.zhengqikj.top

C#:   s.Length
来源：http://csk.zycfv.cn

[A23] 大小写转换
来源：http://bmx.hywenlv.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zdy.gzhubu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yav.316326.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lpt.haohaochexian.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jzm.xinyue.icu

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rwk.epnwcf.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sjd.daria6918.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dgm.shzxlz.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gbx.cucudq.cn

[A24] 去除首尾空白
来源：http://xcr.sweek.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fnc.cdnleiting.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zkw.uphjek.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://foe.zhaomingkeji.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cgg.xingfuxueyuan.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hvc.52xcode.cn

Go:   strings.TrimSpace(s)
来源：http://pzx.hnxiangtu.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://too.gogol.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cqs.zycfv.cn

[A25] 字符串比较
来源：http://vnf.cashguo.top

Py:   s1 == s2; s1 != s2
来源：http://zam.mhx1999.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://usz.yj20258.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ujf.yongpay.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://djd.daxiang520.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qwv.jinyuanbaomall.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cpp.svipenyu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hxu.tianlin.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://etl.hesvh.cn

[A26] 类型转换总览
来源：http://pvf.feifeiyinyue.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kdx.jinqigufen.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qfn.chenlongwang.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zih.zycfv.cn

TS:   Number() String() Boolean() x as number
来源：http://txw.sweek.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sfz.yongpay.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://edg.svipenyu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nrs.zhaomingkeji.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bfe.iojbl.cn

================================================================================
来源：http://for.yj202588.top

B. 流程控制
来源：http://ygz.epnwcf.com

================================================================================
来源：http://kiy.shanyushiyangkeji.top

[B01] 条件判断 if / else
来源：http://kux.tianlin.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://ktw.yfazqb.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://icq.bbcook.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fsu.wangshuangyany.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fkq.yuxming.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pxq.jinqigfzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hbq.guowangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cqt.feifeiyinyue.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pgw.shanyushiyangtech.top

[B02] 多分支 else if / elif
来源：http://scj.cashguo.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ojw.tanke756.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://txj.chenlongwang.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qid.hywenlv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kay.xuanzx.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nzf.zhengqikj.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://aso.52xcode.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pkb.jyoumei.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rze.nanxuanxn.top

[B03] switch / match / case
来源：http://bqs.ybcxt.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wdd.ivvv.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cdi.daxiang520.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lnc.mhx1999.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ywm.daria6918.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mpr.xingfuxueyuan.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://glc.epnwcf.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mpq.iojbl.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://asy.cucudq.cn

[B04] for 计数循环
来源：http://ccy.svipenyu.cn

Py:   for i in range(10): print(i)
来源：http://sia.xuetiantiany.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dbc.hywenlv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ksq.shanyushiyangtech.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rab.jqgfzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://erk.mhx1999.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lwb.zhiwuduotai.top

Ruby: 10.times { |i| puts i }
来源：http://wtg.jlsjyb.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://asg.chenjidiqi.icu

[B05] 遍历数组 / 列表
来源：http://sne.ivvv.top

Py:   for item in arr: print(item)
来源：http://kfc.hcnkem.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gjs.jlsjyb.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zhs.gotoacloud.top

TS:   for (const item of arr) { console.log(item); }
来源：http://fvq.hammf.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vdf.hesvh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ajh.yj20258888.top

Ruby: arr.each { |item| puts item }
来源：http://wsw.hysaishi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qzw.fengsongda.top

[B06] 遍历字典 / 对象
来源：http://nek.wangdashe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://avb.sjlbkw.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pxz.ydzc1.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://svd.sysykeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ohj.yj20258888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qqv.feifeiyinyue.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yjr.hesvh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kop.hongshengwenyu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sss.bbcook.cn

[B07] while 循环
来源：http://hmu.shuidangran.top

Py:   while i < 10: i += 1
来源：http://hgv.yj20258888.top

PHP:  while ($i < 10) { $i++; }
来源：http://hcd.gzhubu.top

JS:   while (i < 10) { i++; }
来源：http://xyw.cheryme.top

TS:   while (i < 10) { i++; }
来源：http://gay.iojbl.cn

Java: while (i < 10) { i++; }
来源：http://qxu.316326.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wic.nanxuanxn.top

Ruby: while i < 10; i += 1; end
来源：http://rgb.sysykeji.top

C#:   while (i < 10) { i++; }
来源：http://bge.meibo888.top

[B08] do-while（至少执行一次）
来源：http://tio.cheryme.top

Py:   # 无 do-while：用 while True + break
来源：http://rnh.gaohongyu789.top

PHP:  do { $i++; } while ($i < 10);
来源：http://cjy.yuanzhike.top

JS:   do { i++; } while (i < 10);
来源：http://twt.mhx1999.top

TS:   do { i++; } while (i < 10);
来源：http://eds.gzhubu.top

Java: do { i++; } while (i < 10);
来源：http://lth.c1oappe.top

Go:   for { i++; if i >= 10 { break } }
来源：http://etn.0kj1m.cn

Ruby: begin; i += 1; end while i < 10
来源：http://iyz.hongshengwenyu.top

C#:   do { i++; } while (i < 10);
来源：http://xgf.redwolf501.top

[B09] break 与 continue
来源：http://oyl.sufxvd.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qrs.ybcxt.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sor.gogol.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kgj.xuetiantiany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nwh.c1oappe.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kfy.hnxiangtu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tyt.0kj1m.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://iqb.redwolf501.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ise.gzhubu.top

[B10] 遍历同时拿索引
来源：http://kil.daria6918.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ill.tian-w.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hbh.bjfxy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oof.meibo888.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rzb.ywan-chungtsiang.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cpn.9152youxi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://esy.hnqzz.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nxh.yvedp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mgd.kuanghao11.cn

[B11] 生成数字序列 / 区间
来源：http://kvt.bbcook.cn

Py:   list(range(0, 10, 2))
来源：http://cit.jqgufenzy.top

PHP:  range(0, 10, 2);
来源：http://ntx.zhiwuduotai.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dls.zdbjq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nia.shzxlz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wjj.zhaomingkeji.xyz


<!-- 参考信息 -->