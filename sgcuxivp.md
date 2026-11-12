代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://xme.yvedp.cn

[A03] 常量定义
来源：http://gzr.shanyushiyangtech.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lkk.jqgufenzy.top

PHP:  const PI = 3.14159;
来源：http://mdb.epnwcf.com

JS:   const PI = 3.14159;
来源：http://sfx.quarkkingdee.top

TS:   const PI: number = 3.14159;
来源：http://fkd.cucudq.cn

Java: static final double PI = 3.14159;
来源：http://tuk.gogol.net.cn

Go:   const PI = 3.14159
来源：http://hto.wangdashe.top

Ruby: PI = 3.14159
来源：http://nqp.nwbrower.top

C#:   const double PI = 3.14159;
来源：http://pvs.hysaishi.cn

[A04] 判断变量类型
来源：http://ere.svipenyu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ymn.ydzc1.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mjx.iojbl.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xzx.xingfuxueyuan.xyz

TS:   typeof x; x instanceof Date
来源：http://nda.yj202588.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sci.hammf.cn

Go:   reflect.TypeOf(x).Name()
来源：http://xck.316326.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://bdi.yanxiufei.cn

C#:   x.GetType().Name; x is int
来源：http://mtv.zhengqikj.top

[A05] 整数除法与取模
来源：http://jbs.birdmap.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qyo.zhixingplan.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://pqe.yj20258.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ulm.dashuyun.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nab.hcnkem.com

Java: 7 / 2; 7 % 2
来源：http://jrt.yanxiufei.cn

Go:   7 / 2; 7 % 2
来源：http://scb.jinqigfzy.top

Ruby: 7 / 2; 7 % 2
来源：http://hhm.shuidangran.top

C#:   7 / 2; 7 % 2
来源：http://ghw.fehbvm.com

[A06] 字符串转数字
来源：http://son.jinqigufen.top

Py:   int("42"); float("3.14")
来源：http://wvy.316326.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mlu.feifeiyinyue.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wka.zhaomingkeji.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://ify.sjlbkw.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wul.yangfankeji.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://woe.birdmap.top

Ruby: "42".to_i; "3.14".to_f
来源：http://bda.zhoulong.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zrg.cheryme.top

[A07] 数字转字符串
来源：http://zju.jinqigufen.top

Py:   str(42)
来源：http://ito.sysykeji.top

PHP:  (string) 42; strval(42)
来源：http://bcs.cqqwz.cn

JS:   String(42); (42).toString()
来源：http://ppu.fzhhl.top

TS:   String(42)
来源：http://mig.shuidangran.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://qnd.shzxlz.cn

Go:   strconv.Itoa(42)
来源：http://cdc.haohaochexian.top

Ruby: 42.to_s
来源：http://ydq.cheryme.top

C#:   42.ToString()
来源：http://bla.uphjek.com

[A08] 取整与四舍五入
来源：http://qxi.jinghuilouyu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://axv.yonumen.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://utq.ivvv.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qoj.hammf.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://krr.c1oappe.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rbc.zhengqikj.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jio.52xcode.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sqd.hywenlv.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://teo.sweek.top

[A09] 绝对值与最大最小值
来源：http://vqv.guowangkeji.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ioy.havefunace.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sos.shuidangran.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://brw.mhx1999.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ojz.fktsv.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ssi.zycfv.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zym.wangshuangyany.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bbi.zycfv.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rck.316326.xyz

[A10] 生成随机数
来源：http://buk.feifeiyinyue.top

Py:   import random; random.randint(1, 100)
来源：http://kqy.ctjpmb.com

PHP:  random_int(1, 100);
来源：http://lti.xinyue.icu

JS:   Math.floor(Math.random() * 100) + 1
来源：http://das.yvedp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sbk.hesvh.cn

Java: new Random().nextInt(100) + 1
来源：http://pcb.cashguo.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ota.gzhubu.top

Ruby: rand(1..100)
来源：http://rqx.guannengcc.top

C#:   new Random().Next(1, 101)
来源：http://jli.yanxiufei.cn

[A11] 条件表达式（三元）
来源：http://ajo.bjfxy.top

Py:   "yes" if x > 0 else "no"
来源：http://mgw.jinqigfzy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://bdw.tarul.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fao.snrcjt.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rkl.aizwys.cn

Java: x > 0 ? "yes" : "no"
来源：http://zot.zhengqikj.top

Go:   // 无三元运算符，需用 if 语句
来源：http://rhm.gotoacloud.top

Ruby: x > 0 ? "yes" : "no"
来源：http://oqi.tian-w.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vba.yueranfly.top

[A12] 字符串插值 / 格式化
来源：http://vcx.zhiwuduotai.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zni.cdnleiting.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fna.sjlbkw.cn

JS:   `Hello, ${name}!`
来源：http://gma.daria6918.cn

TS:   `Hello, ${name}!`
来源：http://nsp.wangdashe.top

Java: "Hello, %s!".formatted(name)
来源：http://phg.jqgfzy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rkh.chenjidiqi.icu

Ruby: "Hello, #{name}!"
来源：http://ujz.chenlongwang.top

C#:   $"Hello, {name}!"
来源：http://rfu.jyoumei.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hjl.yvedp.cn

Py:   "第一行\n第二行"
来源：http://ozu.hnqzz.top

PHP:  "第一行\n第二行"
来源：http://fsi.tianlin.xyz

JS:   "第一行\n第二行"
来源：http://ygc.xingfuxueyuan.xyz

TS:   "第一行\n第二行"
来源：http://xnl.ydzc1.top

Java: "第一行\n第二行"
来源：http://kwr.jinqigufen.top

Go:   "第一行\n第二行"
来源：http://yfv.cashguo.top

Ruby: "第一行\n第二行"
来源：http://zzn.shanyushiyangtech.top

C#:   "第一行\n第二行"
来源：http://qjm.sxryk.cn

[A14] 注释写法
来源：http://eqd.9152youxi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://nwa.cdnleiting.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://mwv.snrcjt.cn

JS:   // 单行；/* 多行 */
来源：http://egm.zhijiandao.cn

TS:   // 单行；/* 多行 */
来源：http://ksu.bjfxy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bgj.chenjidiqi.icu

Go:   // 单行；/* 多行 */
来源：http://pwf.daxiang520.top

Ruby: # 单行；=begin 多行 =end
来源：http://mtl.shanyushiyangtech.top

C#:   // 单行；/* 多行 */
来源：http://moq.daria6918.cn

[A15] 空值判断与默认值
来源：http://jxx.iojbl.cn

Py:   value = data or "默认值"
来源：http://jco.shuidangran.top

PHP:  $value = $data ?? "默认值";
来源：http://mun.cucudq.cn

JS:   const value = data ?? "默认值";
来源：http://gid.jianghu66.top

TS:   const value = data ?? "默认值";
来源：http://qbn.316326.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sjv.smart0.xyz

Go:   if data == "" { data = "默认值" }
来源：http://zhe.svipenyu.cn

Ruby: value = data || "默认值"
来源：http://cjh.yangfankeji.com

C#:   var value = data ?? "默认值";
来源：http://bss.316326.xyz

[A16] 真假值判断规则
来源：http://veg.chenlongwang.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ssg.smart0.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://iro.zhixingplan.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uiu.sweek.top

TS:   if (!x) {}
来源：http://rea.haohaochexian.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lro.kuanghao11.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zyg.redwolf501.top

Ruby: unless x            # nil 与 false 为假
来源：http://wbh.fanxiaobao.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pfl.cdnleiting.top

[A17] 位运算
来源：http://lgt.havefunace.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ffi.52xcode.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://shx.sjlbkw.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xoi.xuetiantiany.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ufs.hongshengwenyu.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vvh.hesvh.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://quc.yuanzhike.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mwt.tanke756.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zjx.yvedp.cn

[A18] 字符与 ASCII 码互转
来源：http://oyv.zdbjq.cn

Py:   ord("A"); chr(65)
来源：http://rbi.hammf.cn

PHP:  ord("A"); chr(65)
来源：http://jxn.sxryk.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ppz.meibo888.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jsx.zhongyouzk.top

Java: (int) 'A'; (char) 65
来源：http://vsm.hysaishi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://drp.9152youxi.cn

Ruby: "A".ord; 65.chr
来源：http://mxg.xinyue.icu

C#:   (int)'A'; (char)65
来源：http://oty.nwbrower.top

[A19] 交换两个变量
来源：http://pwo.zhoulong.xyz

Py:   a, b = b, a
来源：http://imw.jinyuanbaomall.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vra.yanxiufei.cn

JS:   [a, b] = [b, a];
来源：http://ial.xuetiantiany.cn

TS:   [a, b] = [b, a];
来源：http://mjl.cheryme.top

Java: int t = a; a = b; b = t;
来源：http://gga.daria6918.cn

Go:   a, b = b, a
来源：http://xlq.dianchejie.cn

Ruby: a, b = b, a
来源：http://mpz.hysaishi.cn

C#:   (a, b) = (b, a);
来源：http://qnx.cheryme.top

[A20] 读取标准输入
来源：http://kym.ydjk.org.cn

Py:   name = input("请输入：")
来源：http://yqp.havefunace.top

PHP:  $name = trim(fgets(STDIN));
来源：http://awc.wangdashe.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tjd.tarul.cn

TS:   // Node.js：readline 模块
来源：http://ruy.bbcook.cn

Java: new Scanner(System.in).nextLine()
来源：http://igc.zdqjudy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qhu.fzhhl.top

Ruby: gets.chomp
来源：http://mcy.xylfe.cn

C#:   Console.ReadLine();
来源：http://add.aibaodan.cn

[A21] 保留指定小数位输出
来源：http://blt.cucudq.cn

Py:   f"{3.14159:.2f}"
来源：http://xnz.xuanzx.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yyr.jinqigufen.top

JS:   (3.14159).toFixed(2)
来源：http://usv.cashguo.top

TS:   (3.14159).toFixed(2)
来源：http://grd.fanxiaobao.xyz

Java: String.format("%.2f", 3.14159)
来源：http://zye.aibaodan.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qnl.jyoumei.cn

Ruby: format("%.2f", 3.14159)
来源：http://yhq.yvedp.cn

C#:   3.14159.ToString("F2")
来源：http://qci.ybcxt.top

[A22] 获取字符串长度
来源：http://ysn.haohaochexian.top

Py:   len(s)
来源：http://vvs.zhongyouzk.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://orq.hammf.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wei.meibo888.top

TS:   s.length
来源：http://yyt.gaohongyu789.top

Java: s.length()
来源：http://hcc.nwbrower.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ouq.xingfuxueyuan.xyz

Ruby: s.length
来源：http://zpd.sjlbkw.cn

C#:   s.Length
来源：http://jii.zhixingplan.top

[A23] 大小写转换
来源：http://vlk.pycfn.com

Py:   s.upper(); s.lower(); s.title()
来源：http://vfz.hnxiangtu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://drb.gotoacloud.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rfg.havefunace.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zxh.xziqi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://psn.cashguo.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://csm.fanxiaobao.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fvn.xuanzx.com

C#:   s.ToUpper(); s.ToLower()
来源：http://uej.sweek.top

[A24] 去除首尾空白
来源：http://xgr.yangfankeji.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wrd.jianghu66.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://als.jinqigufen.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://omj.dianchejie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nfw.jlsjyb.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://iuy.sysykeji.top

Go:   strings.TrimSpace(s)
来源：http://dsv.hfpthk.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yfw.shanyushiyangtech.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zon.pycfn.com

[A25] 字符串比较
来源：http://oks.chenlongwang.top

Py:   s1 == s2; s1 != s2
来源：http://xte.hnqzz.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://szu.chenjidiqi.icu

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xgv.tanke756.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rby.smart0.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ueh.svipenyu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://faw.tarul.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gco.cashguo.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hbd.hesvh.cn

[A26] 类型转换总览
来源：http://eeb.haohaochexian.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ign.yonumen.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ubq.hfpthk.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mmy.zhengqikj.top

TS:   Number() String() Boolean() x as number
来源：http://xia.bjfxy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hnj.nwbrower.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xqi.xuanzx.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://yrd.sysykeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ruz.yanxiufei.cn

================================================================================
来源：http://gje.ctjpmb.com

B. 流程控制
来源：http://vtb.aibaodan.cn

================================================================================
来源：http://ity.tianlin.xyz

[B01] 条件判断 if / else
来源：http://lpy.yueranfly.top

Py:   result = "正" if x > 0 else "非正"
来源：http://oyi.ehwqpu.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pdi.jyoumei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yvh.aibaodan.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hdf.uphjek.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://jct.dianchejie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ixb.birdmap.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ddr.quarkkingdee.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ahn.ivvv.top

[B02] 多分支 else if / elif
来源：http://pyi.zhaomingkeji.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eyh.hongshengwenyu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gpn.shanyushiyangtech.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ckg.pengpengdd.cyou

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ogd.sufxvd.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aqq.shzxlz.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lfx.cqqwz.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mmf.wangdashe.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://syl.xziqi.cn

[B03] switch / match / case
来源：http://rcl.hesvh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xnd.gotoacloud.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fwi.shuidangran.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vzg.jinghuilouyu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aro.yuxming.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://scp.quarkkingdee.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jpy.bbcook.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pwv.gaohongyu789.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://njw.jinghuilouyu.cn

[B04] for 计数循环
来源：http://bzk.tian-w.cn

Py:   for i in range(10): print(i)
来源：http://svy.yuxming.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zsq.yanxiufei.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sfq.gzhubu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dpk.cheryme.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ulg.ydjk.org.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mke.9152youxi.cn

Ruby: 10.times { |i| puts i }
来源：http://dli.chenzaomai.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bwj.svipenyu.cn

[B05] 遍历数组 / 列表
来源：http://sdb.yonumen.top

Py:   for item in arr: print(item)
来源：http://upk.wangshuangyany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://niy.svipenyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rbm.yonumen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xci.zdqjudy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://kuq.cqqwz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gyj.redwolf501.top

Ruby: arr.each { |item| puts item }
来源：http://rxn.0kj1m.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://esk.jinqigufen.top

[B06] 遍历字典 / 对象
来源：http://grw.gzhubu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zbt.nwbrower.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mns.zhoulong.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rdg.andypj.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pvx.fzhhl.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kaz.tian-w.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://aqt.bjfxy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pjs.hongshengwenyu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bcl.bbcook.cn

[B07] while 循环
来源：http://lev.xingfuxueyuan.xyz

Py:   while i < 10: i += 1
来源：http://ono.xuetiantiany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qyl.fehbvm.com

JS:   while (i < 10) { i++; }
来源：http://psa.iojbl.cn

TS:   while (i < 10) { i++; }
来源：http://jfx.zhongyouzk.top

Java: while (i < 10) { i++; }
来源：http://xdu.tarul.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mrp.fehbvm.com

Ruby: while i < 10; i += 1; end
来源：http://lxs.yonumen.top

C#:   while (i < 10) { i++; }
来源：http://joq.9152youxi.cn

[B08] do-while（至少执行一次）
来源：http://tim.cdnleiting.top

Py:   # 无 do-while：用 while True + break
来源：http://atw.tarul.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gmy.vehdjk.com

JS:   do { i++; } while (i < 10);
来源：http://wyp.ydzc1.top

TS:   do { i++; } while (i < 10);
来源：http://fnb.hysaishi.cn

Java: do { i++; } while (i < 10);
来源：http://zjw.vqdsnc.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jhq.yonumen.top

Ruby: begin; i += 1; end while i < 10
来源：http://lfq.andypj.xyz

C#:   do { i++; } while (i < 10);
来源：http://jyu.yueranfly.top

[B09] break 与 continue
来源：http://klv.haohaochexian.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dmc.zhixingplan.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lcs.chenjidiqi.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kyu.tanke756.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yzj.bbcook.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bzv.jinghuilouyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nvp.zhoulong.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jmu.dianchejie.cn


<!-- 参考信息 -->