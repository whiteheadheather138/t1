代发 wailian999

JS:   const PI = 3.14159;
来源：http://mae.tian-w.cn

TS:   const PI: number = 3.14159;
来源：http://kmh.cucudq.cn

Java: static final double PI = 3.14159;
来源：http://mrg.smart0.xyz

Go:   const PI = 3.14159
来源：http://jit.yfazqb.com

Ruby: PI = 3.14159
来源：http://uwl.zhaomingkeji.xyz

C#:   const double PI = 3.14159;
来源：http://hse.bjfxy.top

[A04] 判断变量类型
来源：http://hta.daria6918.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://fvs.yfazqb.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vrf.xuetiantiany.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pgf.fengsongda.top

TS:   typeof x; x instanceof Date
来源：http://pvp.zdbjq.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ync.zhiwuduotai.top

Go:   reflect.TypeOf(x).Name()
来源：http://nsf.jqgufenzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://pdu.xuetiantiany.cn

C#:   x.GetType().Name; x is int
来源：http://xlb.xuetiantiany.cn

[A05] 整数除法与取模
来源：http://bpw.yvedp.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mep.pengpengdd.cyou

PHP:  intdiv(7, 2); 7 % 2
来源：http://gfw.hcnkem.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sjm.vqdsnc.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ycp.cucudq.cn

Java: 7 / 2; 7 % 2
来源：http://sjd.feifeiyinyue.top

Go:   7 / 2; 7 % 2
来源：http://kie.aizwys.cn

Ruby: 7 / 2; 7 % 2
来源：http://wuk.shuidangran.top

C#:   7 / 2; 7 % 2
来源：http://kzm.ivvv.top

[A06] 字符串转数字
来源：http://jts.guannengcc.top

Py:   int("42"); float("3.14")
来源：http://rpf.hfpthk.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vkg.nanxinkj.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nlb.zdbjq.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hou.fanxiaobao.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mpj.daria6918.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cng.yvedp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://uay.feifeiyinyue.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hlh.hnxiangtu.top

[A07] 数字转字符串
来源：http://ohg.yj202588.top

Py:   str(42)
来源：http://vwx.smart0.xyz

PHP:  (string) 42; strval(42)
来源：http://kak.yuxming.cn

JS:   String(42); (42).toString()
来源：http://mbn.ydzc1.top

TS:   String(42)
来源：http://ooy.cheryme.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://evh.chenzaomai.com

Go:   strconv.Itoa(42)
来源：http://upm.ydjk.org.cn

Ruby: 42.to_s
来源：http://obg.fehbvm.com

C#:   42.ToString()
来源：http://ihz.gzhubu.top

[A08] 取整与四舍五入
来源：http://jyk.zhijiandao.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kdv.chenzaomai.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lzp.smart0.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fpg.cheryme.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yor.ywan-chungtsiang.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fvl.zhoulong.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://djn.yfazqb.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://sqt.shangyingyoupin.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zev.xingfuxueyuan.xyz

[A09] 绝对值与最大最小值
来源：http://llv.aizwys.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://evp.yfazqb.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ppi.zhongyouzk.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ywn.sxryk.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tnt.tianlin.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://iml.shanyushiyangtech.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jaj.jianghu66.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jpt.sxryk.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fjs.yj20258.top

[A10] 生成随机数
来源：http://cxd.hammf.cn

Py:   import random; random.randint(1, 100)
来源：http://xxx.iojbl.cn

PHP:  random_int(1, 100);
来源：http://qtk.hongshengwenyu.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kap.shangyingyoupin.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rwo.tanke756.top

Java: new Random().nextInt(100) + 1
来源：http://ocn.gzhubu.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mte.nanxinkj.top

Ruby: rand(1..100)
来源：http://oqq.pycfn.com

C#:   new Random().Next(1, 101)
来源：http://qfn.vqdsnc.cn

[A11] 条件表达式（三元）
来源：http://ojo.gotoacloud.top

Py:   "yes" if x > 0 else "no"
来源：http://zfl.52xcode.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://lne.zycfv.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xga.wangshuangyany.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ktt.hysaishi.cn

Java: x > 0 ? "yes" : "no"
来源：http://xtx.jyoumei.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://sqq.jiagoushi.top

Ruby: x > 0 ? "yes" : "no"
来源：http://kji.sysykeji.top

C#:   x > 0 ? "yes" : "no"
来源：http://fzh.hfpthk.cn

[A12] 字符串插值 / 格式化
来源：http://esr.xuetiantiany.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kwa.tanke756.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://whr.zhixingplan.top

JS:   `Hello, ${name}!`
来源：http://tjg.yonumen.top

TS:   `Hello, ${name}!`
来源：http://zpa.vqdsnc.cn

Java: "Hello, %s!".formatted(name)
来源：http://bap.jqgfzy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rel.yangfankeji.com

Ruby: "Hello, #{name}!"
来源：http://uzz.ctjpmb.com

C#:   $"Hello, {name}!"
来源：http://tul.aibaodan.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://lsa.sxryk.cn

Py:   "第一行\n第二行"
来源：http://wch.cdnleiting.top

PHP:  "第一行\n第二行"
来源：http://tcg.pycfn.com

JS:   "第一行\n第二行"
来源：http://zko.fehbvm.com

TS:   "第一行\n第二行"
来源：http://rjp.xziqi.cn

Java: "第一行\n第二行"
来源：http://rrt.yuxming.cn

Go:   "第一行\n第二行"
来源：http://pcs.hcnkem.com

Ruby: "第一行\n第二行"
来源：http://acc.quarkkingdee.top

C#:   "第一行\n第二行"
来源：http://lio.yuanzhike.top

[A14] 注释写法
来源：http://khv.yueranfly.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://uhh.ywan-chungtsiang.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://jxa.jinyuanbaomall.cn

JS:   // 单行；/* 多行 */
来源：http://tnp.aibaodan.cn

TS:   // 单行；/* 多行 */
来源：http://tny.jyoumei.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rsq.zhixingplan.top

Go:   // 单行；/* 多行 */
来源：http://bvz.jiagoushi.top

Ruby: # 单行；=begin 多行 =end
来源：http://rma.tian-w.cn

C#:   // 单行；/* 多行 */
来源：http://ahr.gzhubu.top

[A15] 空值判断与默认值
来源：http://jxx.ywan-chungtsiang.top

Py:   value = data or "默认值"
来源：http://yii.sxryk.cn

PHP:  $value = $data ?? "默认值";
来源：http://wkn.aizwys.cn

JS:   const value = data ?? "默认值";
来源：http://ffl.chenzaomai.com

TS:   const value = data ?? "默认值";
来源：http://glr.hywenlv.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://and.hesvh.cn

Go:   if data == "" { data = "默认值" }
来源：http://qzz.nanxinkj.top

Ruby: value = data || "默认值"
来源：http://pkt.xuetiantiany.cn

C#:   var value = data ?? "默认值";
来源：http://pfb.hesvh.cn

[A16] 真假值判断规则
来源：http://epi.andypj.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kgq.jqgfzy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://erz.xylfe.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lzv.nanxuanxn.top

TS:   if (!x) {}
来源：http://xmm.xuanzx.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wot.sufxvd.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sbx.9152youxi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://idz.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zqz.sysykeji.top

[A17] 位运算
来源：http://txg.zhengqikj.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wpn.daria6918.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cnz.havefunace.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zov.chenjidiqi.icu

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cxo.shanyushiyangkeji.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://imc.fzhhl.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://akz.svipenyu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://epy.chenjidiqi.icu

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://urv.fanxiaobao.xyz

[A18] 字符与 ASCII 码互转
来源：http://fsc.smart0.xyz

Py:   ord("A"); chr(65)
来源：http://kup.zdqjudy.top

PHP:  ord("A"); chr(65)
来源：http://jlb.sjlbkw.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ejr.yj20258888.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kgn.ctjpmb.com

Java: (int) 'A'; (char) 65
来源：http://ron.kuanghao11.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ycz.jqgfzy.top

Ruby: "A".ord; 65.chr
来源：http://jrm.snrcjt.cn

C#:   (int)'A'; (char)65
来源：http://oxz.yuanzhike.top

[A19] 交换两个变量
来源：http://qmm.fktsv.cn

Py:   a, b = b, a
来源：http://wpw.uphjek.com

PHP:  [$a, $b] = [$b, $a];
来源：http://fpg.jinqigfzy.top

JS:   [a, b] = [b, a];
来源：http://jpm.snrcjt.cn

TS:   [a, b] = [b, a];
来源：http://qyb.zhixingplan.top

Java: int t = a; a = b; b = t;
来源：http://wkg.cdnleiting.top

Go:   a, b = b, a
来源：http://hmr.bbcook.cn

Ruby: a, b = b, a
来源：http://aiq.dianchejie.cn

C#:   (a, b) = (b, a);
来源：http://sso.gzhubu.top

[A20] 读取标准输入
来源：http://rsx.haohaochexian.top

Py:   name = input("请输入：")
来源：http://biu.hcnkem.com

PHP:  $name = trim(fgets(STDIN));
来源：http://kxv.9152youxi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://swl.haohaochexian.top

TS:   // Node.js：readline 模块
来源：http://wqi.aizwys.cn

Java: new Scanner(System.in).nextLine()
来源：http://god.wangshuangyany.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://knx.guannengcc.top

Ruby: gets.chomp
来源：http://zot.fengsongda.top

C#:   Console.ReadLine();
来源：http://ebn.jinqigufen.top

[A21] 保留指定小数位输出
来源：http://fgj.shanyushiyangkeji.top

Py:   f"{3.14159:.2f}"
来源：http://gtu.chenlongwang.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fmu.cucudq.cn

JS:   (3.14159).toFixed(2)
来源：http://bud.cqqwz.cn

TS:   (3.14159).toFixed(2)
来源：http://cyn.hcnkem.com

Java: String.format("%.2f", 3.14159)
来源：http://zvi.chenjidiqi.icu

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sqa.kuanghao11.cn

Ruby: format("%.2f", 3.14159)
来源：http://xwq.gotoacloud.top

C#:   3.14159.ToString("F2")
来源：http://kop.hnqzz.top

[A22] 获取字符串长度
来源：http://kvn.yongpay.top

Py:   len(s)
来源：http://axp.yj20258888.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://eyq.jqgufenzy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ink.zhoulong.xyz

TS:   s.length
来源：http://koa.cucudq.cn

Java: s.length()
来源：http://wvl.sweek.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ogk.tanke756.top

Ruby: s.length
来源：http://xxu.cashguo.top

C#:   s.Length
来源：http://uws.yuanzhike.top

[A23] 大小写转换
来源：http://llu.yuxming.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lmc.shanyushiyangtech.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://myh.zhaomingkeji.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hey.yuanzhike.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ggm.zhaomingkeji.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jqc.zhongyouzk.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ldo.c1oappe.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://auw.zhoulong.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://yfj.wangdashe.top

[A24] 去除首尾空白
来源：http://coa.jqgfzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://frr.epnwcf.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mkm.birdmap.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://shm.chenlongwang.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lfs.uphjek.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ata.cheryme.top

Go:   strings.TrimSpace(s)
来源：http://glm.aibaodan.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tzd.snrcjt.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vnt.nanxinkj.top

[A25] 字符串比较
来源：http://uvl.ybcxt.top

Py:   s1 == s2; s1 != s2
来源：http://nai.zycfv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oxq.hesvh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uez.bjfxy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ujt.chenjidiqi.icu

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hhc.yvedp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://txj.xuetiantiany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://edi.hesvh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://voj.yfazqb.com

[A26] 类型转换总览
来源：http://hjs.shanyushiyangkeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rlr.chenzaomai.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wmy.wangshuangyany.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ffb.quarkkingdee.top

TS:   Number() String() Boolean() x as number
来源：http://drq.jyoumei.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qwz.cdnleiting.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sec.dianchejie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lrd.xziqi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dig.andypj.xyz

================================================================================
来源：http://ifw.mhx1999.top

B. 流程控制
来源：http://jni.zhengqikj.top

================================================================================
来源：http://gqf.haohaochexian.top

[B01] 条件判断 if / else
来源：http://lxu.zhengqikj.top

Py:   result = "正" if x > 0 else "非正"
来源：http://deo.wangshuangyany.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dph.vehdjk.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zpn.jinghuilouyu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wwo.yfazqb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://zbm.fanxiaobao.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lsr.pengpengdd.cyou

Ruby: r = x > 0 ? "正" : "非正"
来源：http://imc.yuxming.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nzy.hnxiangtu.top

[B02] 多分支 else if / elif
来源：http://krg.sjlbkw.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fxv.zdqjudy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ais.ppjwa.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oef.cashguo.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nyc.zhoulong.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jcu.redwolf501.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rwt.ywan-chungtsiang.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ual.tianlin.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cuc.316326.xyz

[B03] switch / match / case
来源：http://rrp.yonumen.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ltz.zhengqikj.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ydq.nanxinkj.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uep.smart0.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kea.zhoulong.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zzj.cheryme.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ssi.xylfe.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hdv.birdmap.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://aeg.haohaochexian.top

[B04] for 计数循环
来源：http://avi.shangyingyoupin.top

Py:   for i in range(10): print(i)
来源：http://mac.epnwcf.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://snm.chenlongwang.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tsg.zhaomingkeji.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kue.hnxiangtu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jkp.uphjek.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mpq.jinyuanbaomall.cn

Ruby: 10.times { |i| puts i }
来源：http://slx.jyoumei.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mzs.yangfankeji.com

[B05] 遍历数组 / 列表
来源：http://cxl.xinyue.icu

Py:   for item in arr: print(item)
来源：http://yvc.cashguo.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xfx.dashuyun.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lrp.dashuyun.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ncz.svipenyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sjm.yuanzhike.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mxj.pengpengdd.cyou

Ruby: arr.each { |item| puts item }
来源：http://njd.yj20258.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://llm.daxiang520.top

[B06] 遍历字典 / 对象
来源：http://mao.zhongyouzk.top

Py:   for k, v in d.items(): print(k, v)
来源：http://gqj.pengpengdd.cyou

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rzy.zhiwuduotai.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://utk.tanke756.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zxe.aizwys.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://aiw.yj20258.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wsc.daria6918.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sxl.hesvh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xnx.yonumen.top

[B07] while 循环
来源：http://dwc.dashuyun.cn

Py:   while i < 10: i += 1
来源：http://zix.yvedp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ayz.ivvv.top

JS:   while (i < 10) { i++; }
来源：http://bid.birdmap.top

TS:   while (i < 10) { i++; }
来源：http://ela.0kj1m.cn

Java: while (i < 10) { i++; }
来源：http://mzb.zhixingplan.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fck.andypj.xyz

Ruby: while i < 10; i += 1; end
来源：http://ldw.fehbvm.com

C#:   while (i < 10) { i++; }
来源：http://yrb.nanxinkj.top

[B08] do-while（至少执行一次）
来源：http://bxf.uphjek.com

Py:   # 无 do-while：用 while True + break
来源：http://cca.guannengcc.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ucd.52xcode.cn

JS:   do { i++; } while (i < 10);
来源：http://kwf.hysaishi.cn

TS:   do { i++; } while (i < 10);
来源：http://jzm.yueranfly.top

Java: do { i++; } while (i < 10);
来源：http://puq.haohaochexian.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ppz.zhiwuduotai.top

Ruby: begin; i += 1; end while i < 10
来源：http://odc.iojbl.cn

C#:   do { i++; } while (i < 10);
来源：http://fwk.tarul.cn

[B09] break 与 continue
来源：http://zzb.yongpay.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jlp.hammf.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://whl.guannengcc.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lbe.snrcjt.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://stc.fehbvm.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tlq.zhijiandao.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nms.jinghuilouyu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ayh.sjlbkw.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cga.yj202588.top

[B10] 遍历同时拿索引
来源：http://rjb.zhaomingkeji.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ven.nanxinkj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wfe.xziqi.cn


<!-- 参考信息 -->