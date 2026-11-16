代发 wailian999

Ruby: PI = 3.14159
来源：http://xxg.jlsjyb.cn

C#:   const double PI = 3.14159;
来源：http://ziz.jiagoushi.top

[A04] 判断变量类型
来源：http://urq.dashuyun.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zlu.c1oappe.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tdx.316326.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vry.gotoacloud.top

TS:   typeof x; x instanceof Date
来源：http://jep.jinqigfzy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ohk.cqqwz.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dzw.kuanghao11.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ytv.bjfxy.top

C#:   x.GetType().Name; x is int
来源：http://fnx.redwolf501.top

[A05] 整数除法与取模
来源：http://guy.52xcode.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zbo.xziqi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ltg.wangdashe.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ygn.feifeiyinyue.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yrs.xingfuxueyuan.xyz

Java: 7 / 2; 7 % 2
来源：http://pev.yonumen.top

Go:   7 / 2; 7 % 2
来源：http://hvh.havefunace.top

Ruby: 7 / 2; 7 % 2
来源：http://hqm.andypj.xyz

C#:   7 / 2; 7 % 2
来源：http://oty.chenjidiqi.icu

[A06] 字符串转数字
来源：http://dly.cheryme.top

Py:   int("42"); float("3.14")
来源：http://knq.hesvh.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ubc.fzhhl.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://crk.xylfe.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fdx.yj202588.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kpk.dashuyun.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://npv.ybcxt.top

Ruby: "42".to_i; "3.14".to_f
来源：http://kjz.hysaishi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rkp.cdnleiting.top

[A07] 数字转字符串
来源：http://wbb.smart0.xyz

Py:   str(42)
来源：http://krs.hysaishi.cn

PHP:  (string) 42; strval(42)
来源：http://mig.zdqjudy.top

JS:   String(42); (42).toString()
来源：http://kkp.cucudq.cn

TS:   String(42)
来源：http://cbz.meibo888.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://zir.xylfe.cn

Go:   strconv.Itoa(42)
来源：http://ifv.dashuyun.cn

Ruby: 42.to_s
来源：http://sve.wangshuangyany.cn

C#:   42.ToString()
来源：http://zuh.epnwcf.com

[A08] 取整与四舍五入
来源：http://olh.jqgufenzy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uaw.vehdjk.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://goj.jinqigufen.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jaa.xuetiantiany.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rfy.daxiang520.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ggw.jinyuanbaomall.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zzp.redwolf501.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ggx.fanxiaobao.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dai.fengsongda.top

[A09] 绝对值与最大最小值
来源：http://ycd.daria6918.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vfb.sufxvd.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nyf.shzxlz.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rye.hammf.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lfy.tianlin.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jmd.vqdsnc.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ngx.zhiwuduotai.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cnu.gogol.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://svl.yueranfly.top

[A10] 生成随机数
来源：http://wqe.gaohongyu789.top

Py:   import random; random.randint(1, 100)
来源：http://zni.aizwys.cn

PHP:  random_int(1, 100);
来源：http://vpr.zhongyouzk.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wop.meibo888.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dpi.bjfxy.top

Java: new Random().nextInt(100) + 1
来源：http://ydh.cqqwz.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bct.hesvh.cn

Ruby: rand(1..100)
来源：http://wje.svipenyu.cn

C#:   new Random().Next(1, 101)
来源：http://xgy.bjfxy.top

[A11] 条件表达式（三元）
来源：http://sry.ydzc1.top

Py:   "yes" if x > 0 else "no"
来源：http://tim.fengsongda.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://xcj.bjfxy.top

JS:   x > 0 ? "yes" : "no"
来源：http://qpd.feifeiyinyue.top

TS:   x > 0 ? "yes" : "no"
来源：http://jdx.zhixingplan.top

Java: x > 0 ? "yes" : "no"
来源：http://opl.yvedp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hmz.jinqigfzy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://wfp.52xcode.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rtw.nanxinkj.top

[A12] 字符串插值 / 格式化
来源：http://bhg.cqqwz.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://waw.9152youxi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gqa.yj20258.top

JS:   `Hello, ${name}!`
来源：http://fhn.yueranfly.top

TS:   `Hello, ${name}!`
来源：http://fal.jinyuanbaomall.cn

Java: "Hello, %s!".formatted(name)
来源：http://mii.snrcjt.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nuc.aizwys.cn

Ruby: "Hello, #{name}!"
来源：http://jyl.quarkkingdee.top

C#:   $"Hello, {name}!"
来源：http://lgo.zhengqikj.top

[A13] 多行字符串（练习 \n 转义）
来源：http://may.daxiang520.top

Py:   "第一行\n第二行"
来源：http://tgl.nwbrower.top

PHP:  "第一行\n第二行"
来源：http://izp.cqqwz.cn

JS:   "第一行\n第二行"
来源：http://ovo.shzxlz.cn

TS:   "第一行\n第二行"
来源：http://olv.zhengqikj.top

Java: "第一行\n第二行"
来源：http://ppk.jinqigufen.top

Go:   "第一行\n第二行"
来源：http://ubh.shuidangran.top

Ruby: "第一行\n第二行"
来源：http://pvb.ehwqpu.com

C#:   "第一行\n第二行"
来源：http://mkh.shzxlz.cn

[A14] 注释写法
来源：http://oew.jqgufenzy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://pnz.yongpay.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://tzw.redwolf501.top

JS:   // 单行；/* 多行 */
来源：http://wwi.aizwys.cn

TS:   // 单行；/* 多行 */
来源：http://ofe.bbcook.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cet.cheryme.top

Go:   // 单行；/* 多行 */
来源：http://ogw.vqdsnc.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pth.gogol.net.cn

C#:   // 单行；/* 多行 */
来源：http://tbw.yj20258888.top

[A15] 空值判断与默认值
来源：http://oac.xingfuxueyuan.xyz

Py:   value = data or "默认值"
来源：http://kef.yongpay.top

PHP:  $value = $data ?? "默认值";
来源：http://yvl.jinghuilouyu.cn

JS:   const value = data ?? "默认值";
来源：http://qmo.gotoacloud.top

TS:   const value = data ?? "默认值";
来源：http://vna.vqdsnc.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://evb.tianlin.xyz

Go:   if data == "" { data = "默认值" }
来源：http://tgn.nanxinkj.top

Ruby: value = data || "默认值"
来源：http://xzs.gogol.net.cn

C#:   var value = data ?? "默认值";
来源：http://wge.fengsongda.top

[A16] 真假值判断规则
来源：http://dpw.ctjpmb.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kek.aizwys.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pfr.pycfn.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zgg.zhijiandao.cn

TS:   if (!x) {}
来源：http://tnt.52xcode.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://quv.yj20258888.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ats.ydjk.org.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rbw.hywenlv.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rfr.yueranfly.top

[A17] 位运算
来源：http://pux.hammf.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://swn.wangshuangyany.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qvd.wangshuangyany.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://twb.dianchejie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yes.jqgufenzy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bpm.0kj1m.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kir.ehwqpu.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vql.nanxuanxn.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://owa.fktsv.cn

[A18] 字符与 ASCII 码互转
来源：http://zaj.yuxming.cn

Py:   ord("A"); chr(65)
来源：http://sru.sysykeji.top

PHP:  ord("A"); chr(65)
来源：http://tld.bjfxy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://chl.zhijiandao.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xzw.smart0.xyz

Java: (int) 'A'; (char) 65
来源：http://rpd.hywenlv.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://etj.hesvh.cn

Ruby: "A".ord; 65.chr
来源：http://vrb.zhoulong.xyz

C#:   (int)'A'; (char)65
来源：http://gbi.ivvv.top

[A19] 交换两个变量
来源：http://cag.wangshuangyany.cn

Py:   a, b = b, a
来源：http://pur.zhengqikj.top

PHP:  [$a, $b] = [$b, $a];
来源：http://vfm.hcnkem.com

JS:   [a, b] = [b, a];
来源：http://jxe.fanxiaobao.xyz

TS:   [a, b] = [b, a];
来源：http://iov.xuanzx.com

Java: int t = a; a = b; b = t;
来源：http://gik.jinyuanbaomall.cn

Go:   a, b = b, a
来源：http://njz.jinghuilouyu.cn

Ruby: a, b = b, a
来源：http://ics.ywan-chungtsiang.top

C#:   (a, b) = (b, a);
来源：http://erq.shzxlz.cn

[A20] 读取标准输入
来源：http://otk.ehwqpu.com

Py:   name = input("请输入：")
来源：http://jew.c1oappe.top

PHP:  $name = trim(fgets(STDIN));
来源：http://qbn.gzhubu.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://act.xziqi.cn

TS:   // Node.js：readline 模块
来源：http://nec.chenjidiqi.icu

Java: new Scanner(System.in).nextLine()
来源：http://jda.chenjidiqi.icu

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://azj.xuetiantiany.cn

Ruby: gets.chomp
来源：http://cci.xziqi.cn

C#:   Console.ReadLine();
来源：http://xxy.fktsv.cn

[A21] 保留指定小数位输出
来源：http://oun.jinyuanbaomall.cn

Py:   f"{3.14159:.2f}"
来源：http://swn.shanyushiyangtech.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tzv.wangshuangyany.cn

JS:   (3.14159).toFixed(2)
来源：http://cai.tanke756.top

TS:   (3.14159).toFixed(2)
来源：http://aap.zdqjudy.top

Java: String.format("%.2f", 3.14159)
来源：http://moq.havefunace.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tls.jqgfzy.top

Ruby: format("%.2f", 3.14159)
来源：http://iwp.fehbvm.com

C#:   3.14159.ToString("F2")
来源：http://hdb.tianlin.xyz

[A22] 获取字符串长度
来源：http://cua.iojbl.cn

Py:   len(s)
来源：http://xsm.yangfankeji.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mmi.yj20258888.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wtj.ydzc1.top

TS:   s.length
来源：http://udq.mhx1999.top

Java: s.length()
来源：http://uwy.mhx1999.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jze.fehbvm.com

Ruby: s.length
来源：http://ogz.tarul.cn

C#:   s.Length
来源：http://ypd.gzhubu.top

[A23] 大小写转换
来源：http://epo.andypj.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://old.aizwys.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fpl.hywenlv.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wlv.tanke756.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gyl.tian-w.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cvp.tarul.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gyt.hnxiangtu.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://akp.hywenlv.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pcj.vqdsnc.cn

[A24] 去除首尾空白
来源：http://vab.jiagoushi.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zex.vehdjk.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hzp.fengsongda.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://opd.yonumen.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rjf.cashguo.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gqq.quarkkingdee.top

Go:   strings.TrimSpace(s)
来源：http://yag.hnxiangtu.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rre.zycfv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xui.sxryk.cn

[A25] 字符串比较
来源：http://gce.jqgfzy.top

Py:   s1 == s2; s1 != s2
来源：http://icl.vqdsnc.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yiy.bbcook.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kqw.xuanzx.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cde.xingfuxueyuan.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bik.yj20258888.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hmy.zdbjq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mbn.sjlbkw.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ilf.shangyingyoupin.top

[A26] 类型转换总览
来源：http://rdn.shuidangran.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ccr.ydzc1.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://oar.nanxinkj.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rqn.ydjk.org.cn

TS:   Number() String() Boolean() x as number
来源：http://sxt.jinqigfzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cjs.gaohongyu789.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://saa.xylfe.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gzn.jyoumei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://iel.gaohongyu789.top

================================================================================
来源：http://fjk.yanxiufei.cn

B. 流程控制
来源：http://geg.cheryme.top

================================================================================
来源：http://exy.ivvv.top

[B01] 条件判断 if / else
来源：http://ygt.yongpay.top

Py:   result = "正" if x > 0 else "非正"
来源：http://qki.fanxiaobao.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mzj.sweek.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yor.chenzaomai.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ofa.jinqigufen.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://czy.epnwcf.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sce.yfazqb.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kkg.ctjpmb.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://auz.zdqjudy.top

[B02] 多分支 else if / elif
来源：http://gvz.yongpay.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://let.yj202588.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vki.andypj.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xyi.shzxlz.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rjn.chenzaomai.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pgy.xylfe.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zbr.yj20258.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ytw.uphjek.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uyz.chenjidiqi.icu

[B03] switch / match / case
来源：http://shn.cucudq.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bvc.bbcook.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ndc.bbcook.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lhu.zhoulong.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://udv.cashguo.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vwv.hnxiangtu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mic.chenlongwang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ckg.hywenlv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vpr.xingfuxueyuan.xyz

[B04] for 计数循环
来源：http://wqf.hesvh.cn

Py:   for i in range(10): print(i)
来源：http://oiz.cashguo.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cmp.zhoulong.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qup.zhijiandao.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hjj.ydjk.org.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mvw.birdmap.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vlh.epnwcf.com

Ruby: 10.times { |i| puts i }
来源：http://oyj.gaohongyu789.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wqg.ppjwa.cn

[B05] 遍历数组 / 列表
来源：http://krj.sjlbkw.cn

Py:   for item in arr: print(item)
来源：http://cye.vehdjk.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nau.hesvh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qka.nanxinkj.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xih.jqgfzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wok.jinqigfzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ogi.svipenyu.cn

Ruby: arr.each { |item| puts item }
来源：http://tdv.shanyushiyangkeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ddn.wangdashe.top

[B06] 遍历字典 / 对象
来源：http://aha.ivvv.top

Py:   for k, v in d.items(): print(k, v)
来源：http://eur.fehbvm.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dzn.ybcxt.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gtg.jiagoushi.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qom.yuxming.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fns.jiagoushi.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yrp.xziqi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://edi.vehdjk.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://syh.mhx1999.top

[B07] while 循环
来源：http://awr.guannengcc.top

Py:   while i < 10: i += 1
来源：http://iij.c1oappe.top

PHP:  while ($i < 10) { $i++; }
来源：http://jak.jinghuilouyu.cn

JS:   while (i < 10) { i++; }
来源：http://yld.feifeiyinyue.top

TS:   while (i < 10) { i++; }
来源：http://dbw.cucudq.cn

Java: while (i < 10) { i++; }
来源：http://peq.havefunace.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wxi.yongpay.top

Ruby: while i < 10; i += 1; end
来源：http://cik.sysykeji.top

C#:   while (i < 10) { i++; }
来源：http://cdc.haohaochexian.top

[B08] do-while（至少执行一次）
来源：http://afu.cheryme.top

Py:   # 无 do-while：用 while True + break
来源：http://ssf.ywan-chungtsiang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://mnz.zycfv.cn

JS:   do { i++; } while (i < 10);
来源：http://ghy.zhongyouzk.top

TS:   do { i++; } while (i < 10);
来源：http://qox.jqgfzy.top

Java: do { i++; } while (i < 10);
来源：http://czo.shanyushiyangtech.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hkq.52xcode.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dsa.gaohongyu789.top

C#:   do { i++; } while (i < 10);
来源：http://wvb.sysykeji.top

[B09] break 与 continue
来源：http://vri.hcnkem.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sig.hcnkem.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kzf.9152youxi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fvo.ehwqpu.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nnw.aizwys.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fuf.snrcjt.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lcf.shzxlz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mxn.c1oappe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dzh.jianghu66.top

[B10] 遍历同时拿索引
来源：http://caz.epnwcf.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iqc.jinqigfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kfd.chenzaomai.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://akx.bjfxy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xar.pengpengdd.cyou

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hfo.ppjwa.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qph.shangyingyoupin.top


<!-- 参考信息 -->