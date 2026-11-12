代发 wailian999

Ruby: PI = 3.14159
来源：http://jro.redwolf501.top

C#:   const double PI = 3.14159;
来源：http://voz.gzhubu.top

[A04] 判断变量类型
来源：http://siy.hysaishi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://oro.jinghuilouyu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yrn.jinqigufen.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gpq.hammf.cn

TS:   typeof x; x instanceof Date
来源：http://jrf.redwolf501.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ndw.cucudq.cn

Go:   reflect.TypeOf(x).Name()
来源：http://oov.tarul.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://keg.zdbjq.cn

C#:   x.GetType().Name; x is int
来源：http://ibc.sxryk.cn

[A05] 整数除法与取模
来源：http://xzo.chenlongwang.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zpu.cashguo.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://rhx.cdnleiting.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://twl.jinqigufen.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nhl.fktsv.cn

Java: 7 / 2; 7 % 2
来源：http://dvf.mhx1999.top

Go:   7 / 2; 7 % 2
来源：http://rye.aibaodan.cn

Ruby: 7 / 2; 7 % 2
来源：http://gmz.chenlongwang.top

C#:   7 / 2; 7 % 2
来源：http://rls.hnqzz.top

[A06] 字符串转数字
来源：http://pnv.cheryme.top

Py:   int("42"); float("3.14")
来源：http://daa.zhixingplan.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rxk.bbcook.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wdx.zhixingplan.top

TS:   parseInt("42", 10); Number("42")
来源：http://lsv.c1oappe.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fjd.xziqi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ovo.ctjpmb.com

Ruby: "42".to_i; "3.14".to_f
来源：http://ony.ydzc1.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ymn.cashguo.top

[A07] 数字转字符串
来源：http://neg.nwbrower.top

Py:   str(42)
来源：http://gil.jqgfzy.top

PHP:  (string) 42; strval(42)
来源：http://akv.fanxiaobao.xyz

JS:   String(42); (42).toString()
来源：http://bod.birdmap.top

TS:   String(42)
来源：http://uey.shanyushiyangtech.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://iru.tanke756.top

Go:   strconv.Itoa(42)
来源：http://ghj.cheryme.top

Ruby: 42.to_s
来源：http://rvk.316326.xyz

C#:   42.ToString()
来源：http://cap.ydjk.org.cn

[A08] 取整与四舍五入
来源：http://iuj.jinqigufen.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mgd.quarkkingdee.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://spg.uphjek.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xxx.pengpengdd.cyou

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vep.zhijiandao.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jdp.ehwqpu.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wun.fzhhl.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://krd.pengpengdd.cyou

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sgw.cucudq.cn

[A09] 绝对值与最大最小值
来源：http://rhw.vqdsnc.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cgx.quarkkingdee.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wgr.wangdashe.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pqo.yvedp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yoy.zhongyouzk.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://duz.hywenlv.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://oxd.wangdashe.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kjk.0kj1m.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://coi.gzhubu.top

[A10] 生成随机数
来源：http://oqr.yfazqb.com

Py:   import random; random.randint(1, 100)
来源：http://lie.tian-w.cn

PHP:  random_int(1, 100);
来源：http://sxl.fehbvm.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://png.shzxlz.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bwx.xziqi.cn

Java: new Random().nextInt(100) + 1
来源：http://dri.andypj.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xcm.ppjwa.cn

Ruby: rand(1..100)
来源：http://zzk.gzhubu.top

C#:   new Random().Next(1, 101)
来源：http://tqr.ppjwa.cn

[A11] 条件表达式（三元）
来源：http://bax.dianchejie.cn

Py:   "yes" if x > 0 else "no"
来源：http://uzt.sufxvd.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qye.zdbjq.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jwv.yonumen.top

TS:   x > 0 ? "yes" : "no"
来源：http://ycp.epnwcf.com

Java: x > 0 ? "yes" : "no"
来源：http://fsc.jqgfzy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://luq.nwbrower.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ehc.guannengcc.top

C#:   x > 0 ? "yes" : "no"
来源：http://oxm.sxryk.cn

[A12] 字符串插值 / 格式化
来源：http://hni.hammf.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ftv.zhoulong.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rkr.c1oappe.top

JS:   `Hello, ${name}!`
来源：http://ufs.meibo888.top

TS:   `Hello, ${name}!`
来源：http://wox.nanxinkj.top

Java: "Hello, %s!".formatted(name)
来源：http://yuw.xingfuxueyuan.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://btu.jqgfzy.top

Ruby: "Hello, #{name}!"
来源：http://wtz.mhx1999.top

C#:   $"Hello, {name}!"
来源：http://hca.yj202588.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ooc.hnxiangtu.top

Py:   "第一行\n第二行"
来源：http://inl.quarkkingdee.top

PHP:  "第一行\n第二行"
来源：http://rvq.feifeiyinyue.top

JS:   "第一行\n第二行"
来源：http://bsb.shzxlz.cn

TS:   "第一行\n第二行"
来源：http://vch.zhoulong.xyz

Java: "第一行\n第二行"
来源：http://fxq.zdbjq.cn

Go:   "第一行\n第二行"
来源：http://jyr.zhoulong.xyz

Ruby: "第一行\n第二行"
来源：http://def.dashuyun.cn

C#:   "第一行\n第二行"
来源：http://irf.cqqwz.cn

[A14] 注释写法
来源：http://nps.yj20258888.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://kjz.redwolf501.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://xao.aibaodan.cn

JS:   // 单行；/* 多行 */
来源：http://pzj.wangdashe.top

TS:   // 单行；/* 多行 */
来源：http://wrf.xziqi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ese.fanxiaobao.xyz

Go:   // 单行；/* 多行 */
来源：http://ooz.meibo888.top

Ruby: # 单行；=begin 多行 =end
来源：http://vyn.tianlin.xyz

C#:   // 单行；/* 多行 */
来源：http://hni.snrcjt.cn

[A15] 空值判断与默认值
来源：http://pla.chenlongwang.top

Py:   value = data or "默认值"
来源：http://akp.bjfxy.top

PHP:  $value = $data ?? "默认值";
来源：http://jhs.birdmap.top

JS:   const value = data ?? "默认值";
来源：http://lcs.52xcode.cn

TS:   const value = data ?? "默认值";
来源：http://myo.daxiang520.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jhf.ivvv.top

Go:   if data == "" { data = "默认值" }
来源：http://yqy.hesvh.cn

Ruby: value = data || "默认值"
来源：http://zza.hesvh.cn

C#:   var value = data ?? "默认值";
来源：http://daj.52xcode.cn

[A16] 真假值判断规则
来源：http://oav.guowangkeji.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wgb.yfazqb.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://iso.zhoulong.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fmk.pengpengdd.cyou

TS:   if (!x) {}
来源：http://xqb.zhaomingkeji.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hkz.fzhhl.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://keo.zhongyouzk.top

Ruby: unless x            # nil 与 false 为假
来源：http://ojt.cdnleiting.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vnz.cucudq.cn

[A17] 位运算
来源：http://oql.jiagoushi.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://all.zhengqikj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zfd.sweek.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://srz.cucudq.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dnt.kuanghao11.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wzm.fanxiaobao.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zht.yueranfly.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://drz.tianlin.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://luo.ywan-chungtsiang.top

[A18] 字符与 ASCII 码互转
来源：http://hiz.jyoumei.cn

Py:   ord("A"); chr(65)
来源：http://qed.pengpengdd.cyou

PHP:  ord("A"); chr(65)
来源：http://qvz.0kj1m.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ldc.sxryk.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yrg.yfazqb.com

Java: (int) 'A'; (char) 65
来源：http://gcu.hammf.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://omn.birdmap.top

Ruby: "A".ord; 65.chr
来源：http://dbo.hesvh.cn

C#:   (int)'A'; (char)65
来源：http://ttk.gogol.net.cn

[A19] 交换两个变量
来源：http://wsv.tianlin.xyz

Py:   a, b = b, a
来源：http://rtc.yvedp.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://soj.cheryme.top

JS:   [a, b] = [b, a];
来源：http://zyu.fehbvm.com

TS:   [a, b] = [b, a];
来源：http://qri.sweek.top

Java: int t = a; a = b; b = t;
来源：http://pcu.jqgufenzy.top

Go:   a, b = b, a
来源：http://dwy.yfazqb.com

Ruby: a, b = b, a
来源：http://zqv.hnxiangtu.top

C#:   (a, b) = (b, a);
来源：http://iga.zdqjudy.top

[A20] 读取标准输入
来源：http://chl.xylfe.cn

Py:   name = input("请输入：")
来源：http://zyq.jiagoushi.top

PHP:  $name = trim(fgets(STDIN));
来源：http://fpf.yongpay.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vlz.yj20258888.top

TS:   // Node.js：readline 模块
来源：http://ykm.jyoumei.cn

Java: new Scanner(System.in).nextLine()
来源：http://xak.xuanzx.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zem.jyoumei.cn

Ruby: gets.chomp
来源：http://bdx.zdbjq.cn

C#:   Console.ReadLine();
来源：http://fxt.dianchejie.cn

[A21] 保留指定小数位输出
来源：http://fck.cqqwz.cn

Py:   f"{3.14159:.2f}"
来源：http://hrj.shanyushiyangkeji.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hnk.gzhubu.top

JS:   (3.14159).toFixed(2)
来源：http://ouq.bbcook.cn

TS:   (3.14159).toFixed(2)
来源：http://kvq.pengpengdd.cyou

Java: String.format("%.2f", 3.14159)
来源：http://rpw.daxiang520.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bmb.cdnleiting.top

Ruby: format("%.2f", 3.14159)
来源：http://dxc.tian-w.cn

C#:   3.14159.ToString("F2")
来源：http://fzl.ybcxt.top

[A22] 获取字符串长度
来源：http://fqr.zycfv.cn

Py:   len(s)
来源：http://flq.jinqigfzy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rmu.jianghu66.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xsa.nwbrower.top

TS:   s.length
来源：http://rzn.zhoulong.xyz

Java: s.length()
来源：http://zzl.yongpay.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yab.pengpengdd.cyou

Ruby: s.length
来源：http://hux.yj20258.top

C#:   s.Length
来源：http://xdy.fehbvm.com

[A23] 大小写转换
来源：http://iiy.birdmap.top

Py:   s.upper(); s.lower(); s.title()
来源：http://kqz.quarkkingdee.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ppf.wangdashe.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pdj.sufxvd.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fft.jqgufenzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vok.hesvh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xle.cashguo.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mal.cucudq.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ymu.ctjpmb.com

[A24] 去除首尾空白
来源：http://kiy.zhengqikj.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://upp.sjlbkw.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tmd.andypj.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zlm.xylfe.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tba.fanxiaobao.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wth.ydzc1.top

Go:   strings.TrimSpace(s)
来源：http://mpv.meibo888.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://caz.yfazqb.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://izw.zhijiandao.cn

[A25] 字符串比较
来源：http://mtp.sxryk.cn

Py:   s1 == s2; s1 != s2
来源：http://nwx.pycfn.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://imb.52xcode.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dxp.yanxiufei.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cdl.pycfn.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nxz.daxiang520.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://upu.zycfv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://aqh.yj202588.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wif.hfpthk.cn

[A26] 类型转换总览
来源：http://uuf.zhengqikj.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lix.9152youxi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fxg.cdnleiting.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ath.guowangkeji.top

TS:   Number() String() Boolean() x as number
来源：http://kfu.feifeiyinyue.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uqz.dianchejie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vzj.cdnleiting.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://klx.tanke756.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pjo.sufxvd.cn

================================================================================
来源：http://pem.gaohongyu789.top

B. 流程控制
来源：http://ydd.316326.xyz

================================================================================
来源：http://xja.uphjek.com

[B01] 条件判断 if / else
来源：http://ptw.fanxiaobao.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://stf.bjfxy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lch.jiagoushi.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yhh.snrcjt.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://eky.pengpengdd.cyou

Java: String r = x > 0 ? "正" : "非正";
来源：http://kkg.ivvv.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://onx.hammf.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zgg.shzxlz.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ftk.cucudq.cn

[B02] 多分支 else if / elif
来源：http://bpn.cheryme.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nxi.bbcook.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hix.fanxiaobao.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://swe.zhijiandao.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tpb.shuidangran.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://res.tian-w.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zhs.yvedp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://epn.hammf.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eow.hywenlv.cn

[B03] switch / match / case
来源：http://yyj.andypj.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yye.uphjek.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nij.xuetiantiany.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oed.fzhhl.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rut.quarkkingdee.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://max.sweek.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://anx.yuanzhike.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://acc.redwolf501.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wed.dashuyun.cn

[B04] for 计数循环
来源：http://gtz.jlsjyb.cn

Py:   for i in range(10): print(i)
来源：http://txl.zhixingplan.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sul.redwolf501.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sob.fehbvm.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xqs.ppjwa.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oqq.jinqigfzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://syj.yj202588.top

Ruby: 10.times { |i| puts i }
来源：http://uym.aizwys.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zrx.hesvh.cn

[B05] 遍历数组 / 列表
来源：http://ydz.shanyushiyangtech.top

Py:   for item in arr: print(item)
来源：http://bwt.fanxiaobao.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kzv.cucudq.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://erl.iojbl.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qpl.nwbrower.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ahy.pycfn.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nii.c1oappe.top

Ruby: arr.each { |item| puts item }
来源：http://epe.jiagoushi.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mqh.0kj1m.cn

[B06] 遍历字典 / 对象
来源：http://bjq.fzhhl.top

Py:   for k, v in d.items(): print(k, v)
来源：http://vpf.zycfv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pmn.daxiang520.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gvu.gzhubu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jhg.xuanzx.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yqf.guannengcc.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wox.wangshuangyany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fzs.havefunace.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fhh.zhixingplan.top

[B07] while 循环
来源：http://wxd.sweek.top

Py:   while i < 10: i += 1
来源：http://sxi.meibo888.top

PHP:  while ($i < 10) { $i++; }
来源：http://tnf.haohaochexian.top

JS:   while (i < 10) { i++; }
来源：http://kyy.gogol.net.cn

TS:   while (i < 10) { i++; }
来源：http://dkz.redwolf501.top

Java: while (i < 10) { i++; }
来源：http://fst.gotoacloud.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qdg.mhx1999.top

Ruby: while i < 10; i += 1; end
来源：http://civ.shzxlz.cn

C#:   while (i < 10) { i++; }
来源：http://gcf.redwolf501.top

[B08] do-while（至少执行一次）
来源：http://nze.ydjk.org.cn

Py:   # 无 do-while：用 while True + break
来源：http://wis.aizwys.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ogt.aibaodan.cn

JS:   do { i++; } while (i < 10);
来源：http://hjp.zhijiandao.cn

TS:   do { i++; } while (i < 10);
来源：http://ulc.bjfxy.top

Java: do { i++; } while (i < 10);
来源：http://zon.yangfankeji.com

Go:   for { i++; if i >= 10 { break } }
来源：http://oyp.chenzaomai.com

Ruby: begin; i += 1; end while i < 10
来源：http://ivr.pengpengdd.cyou

C#:   do { i++; } while (i < 10);
来源：http://fsx.kuanghao11.cn

[B09] break 与 continue
来源：http://lvq.tian-w.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dhw.xylfe.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eut.zhongyouzk.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://axp.birdmap.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hzb.jyoumei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mpq.nwbrower.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zyt.pengpengdd.cyou

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ewx.sysykeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gpe.ydjk.org.cn

[B10] 遍历同时拿索引
来源：http://vzw.tianlin.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://csq.tian-w.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zzn.chenjidiqi.icu

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uqr.zhixingplan.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tsa.yuxming.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wnx.sxryk.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vnv.nwbrower.top


<!-- 参考信息 -->