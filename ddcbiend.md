代发 wailian999

Py:   print("Hello, World!")
来源：http://hlx.sufxvd.cn

PHP:  echo "Hello, World!";
来源：http://hty.jinqigufen.top

JS:   console.log("Hello, World!");
来源：http://jdg.svipenyu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dqs.yj20258.top

Java: System.out.println("Hello, World!");
来源：http://kaz.guannengcc.top

Go:   fmt.Println("Hello, World!")
来源：http://cls.yueranfly.top

Ruby: puts "Hello, World!"
来源：http://kkd.316326.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://gih.yuanzhike.top

[A02] 变量声明与赋值
来源：http://huo.meibo888.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://aeh.bjfxy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://skv.zhengqikj.top

JS:   let name = "Alex"; const age = 20;
来源：http://zev.zdqjudy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gcw.zdbjq.cn

Java: String name = "Alex"; int age = 20;
来源：http://mlj.snrcjt.cn

Go:   name := "Alex"; age := 20
来源：http://mtd.jianghu66.top

Ruby: name = "Alex"; age = 20
来源：http://hnc.pycfn.com

C#:   string name = "Alex"; int age = 20;
来源：http://yet.fanxiaobao.xyz

[A03] 常量定义
来源：http://zmf.pengpengdd.cyou

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://alm.iojbl.cn

PHP:  const PI = 3.14159;
来源：http://vuw.guowangkeji.top

JS:   const PI = 3.14159;
来源：http://zbw.cashguo.top

TS:   const PI: number = 3.14159;
来源：http://brg.0kj1m.cn

Java: static final double PI = 3.14159;
来源：http://coe.hesvh.cn

Go:   const PI = 3.14159
来源：http://qvi.hammf.cn

Ruby: PI = 3.14159
来源：http://mhg.yj20258.top

C#:   const double PI = 3.14159;
来源：http://epj.hysaishi.cn

[A04] 判断变量类型
来源：http://zxn.smart0.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://kua.jinghuilouyu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cyh.zhijiandao.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ypw.chenjidiqi.icu

TS:   typeof x; x instanceof Date
来源：http://gsf.andypj.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lvd.cashguo.top

Go:   reflect.TypeOf(x).Name()
来源：http://omv.cucudq.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wry.cucudq.cn

C#:   x.GetType().Name; x is int
来源：http://hqs.ehwqpu.com

[A05] 整数除法与取模
来源：http://uyd.aibaodan.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hqc.xylfe.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://dwg.ybcxt.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://isa.cheryme.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hye.bbcook.cn

Java: 7 / 2; 7 % 2
来源：http://qks.quarkkingdee.top

Go:   7 / 2; 7 % 2
来源：http://bih.gogol.net.cn

Ruby: 7 / 2; 7 % 2
来源：http://tlb.9152youxi.cn

C#:   7 / 2; 7 % 2
来源：http://xvc.mhx1999.top

[A06] 字符串转数字
来源：http://xfg.hnxiangtu.top

Py:   int("42"); float("3.14")
来源：http://juj.hnqzz.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mhk.haohaochexian.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zxl.9152youxi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ptv.haohaochexian.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rzl.haohaochexian.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hoy.nwbrower.top

Ruby: "42".to_i; "3.14".to_f
来源：http://bdh.redwolf501.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kaa.fengsongda.top

[A07] 数字转字符串
来源：http://hab.svipenyu.cn

Py:   str(42)
来源：http://lsy.xuetiantiany.cn

PHP:  (string) 42; strval(42)
来源：http://dsx.fktsv.cn

JS:   String(42); (42).toString()
来源：http://flk.sxryk.cn

TS:   String(42)
来源：http://qlu.sjlbkw.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hua.snrcjt.cn

Go:   strconv.Itoa(42)
来源：http://gmt.hcnkem.com

Ruby: 42.to_s
来源：http://wyo.yangfankeji.com

C#:   42.ToString()
来源：http://zsu.hnxiangtu.top

[A08] 取整与四舍五入
来源：http://dmz.haohaochexian.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bfb.daxiang520.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rmm.jinghuilouyu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kpd.aibaodan.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ptw.hnqzz.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wgp.yuxming.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hfc.pycfn.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://nhk.ydjk.org.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pmw.feifeiyinyue.top

[A09] 绝对值与最大最小值
来源：http://tcv.9152youxi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://den.yonumen.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://arj.cheryme.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://joy.gogol.net.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rcx.epnwcf.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ell.mhx1999.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wzg.hcnkem.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uyo.nanxuanxn.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://use.redwolf501.top

[A10] 生成随机数
来源：http://wxb.ehwqpu.com

Py:   import random; random.randint(1, 100)
来源：http://ecm.9152youxi.cn

PHP:  random_int(1, 100);
来源：http://frd.quarkkingdee.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qul.fehbvm.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wgo.cucudq.cn

Java: new Random().nextInt(100) + 1
来源：http://ehu.jinghuilouyu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vnw.yanxiufei.cn

Ruby: rand(1..100)
来源：http://ild.hcnkem.com

C#:   new Random().Next(1, 101)
来源：http://szt.zhijiandao.cn

[A11] 条件表达式（三元）
来源：http://miq.andypj.xyz

Py:   "yes" if x > 0 else "no"
来源：http://jpx.jinghuilouyu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dux.hfpthk.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ope.aizwys.cn

TS:   x > 0 ? "yes" : "no"
来源：http://cmf.chenlongwang.top

Java: x > 0 ? "yes" : "no"
来源：http://dxv.haohaochexian.top

Go:   // 无三元运算符，需用 if 语句
来源：http://aek.svipenyu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fgq.pycfn.com

C#:   x > 0 ? "yes" : "no"
来源：http://tau.bjfxy.top

[A12] 字符串插值 / 格式化
来源：http://esn.zhijiandao.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ksu.havefunace.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lvo.meibo888.top

JS:   `Hello, ${name}!`
来源：http://jdi.fengsongda.top

TS:   `Hello, ${name}!`
来源：http://pog.xuetiantiany.cn

Java: "Hello, %s!".formatted(name)
来源：http://wga.0kj1m.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cwd.bjfxy.top

Ruby: "Hello, #{name}!"
来源：http://dbc.cdnleiting.top

C#:   $"Hello, {name}!"
来源：http://cgp.feifeiyinyue.top

[A13] 多行字符串（练习 \n 转义）
来源：http://jkn.iojbl.cn

Py:   "第一行\n第二行"
来源：http://llz.wangdashe.top

PHP:  "第一行\n第二行"
来源：http://hhd.feifeiyinyue.top

JS:   "第一行\n第二行"
来源：http://fhc.uphjek.com

TS:   "第一行\n第二行"
来源：http://aio.chenlongwang.top

Java: "第一行\n第二行"
来源：http://sup.daria6918.cn

Go:   "第一行\n第二行"
来源：http://nto.zhijiandao.cn

Ruby: "第一行\n第二行"
来源：http://fbs.jqgfzy.top

C#:   "第一行\n第二行"
来源：http://opc.jinqigfzy.top

[A14] 注释写法
来源：http://ofx.zhongyouzk.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://rmp.jianghu66.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://rfl.nwbrower.top

JS:   // 单行；/* 多行 */
来源：http://gtb.cheryme.top

TS:   // 单行；/* 多行 */
来源：http://kqx.sufxvd.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pjj.shuidangran.top

Go:   // 单行；/* 多行 */
来源：http://aot.yuxming.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qio.epnwcf.com

C#:   // 单行；/* 多行 */
来源：http://zqk.shangyingyoupin.top

[A15] 空值判断与默认值
来源：http://sbx.hfpthk.cn

Py:   value = data or "默认值"
来源：http://fra.snrcjt.cn

PHP:  $value = $data ?? "默认值";
来源：http://hog.yangfankeji.com

JS:   const value = data ?? "默认值";
来源：http://loa.tanke756.top

TS:   const value = data ?? "默认值";
来源：http://czs.tian-w.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fwb.xinyue.icu

Go:   if data == "" { data = "默认值" }
来源：http://zfu.cdnleiting.top

Ruby: value = data || "默认值"
来源：http://xkz.guowangkeji.top

C#:   var value = data ?? "默认值";
来源：http://ffx.yueranfly.top

[A16] 真假值判断规则
来源：http://yhy.yj202588.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wiy.uphjek.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vzy.jiagoushi.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dsg.daxiang520.top

TS:   if (!x) {}
来源：http://oxt.shuidangran.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://was.yueranfly.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nil.tanke756.top

Ruby: unless x            # nil 与 false 为假
来源：http://kwe.shangyingyoupin.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dmr.shuidangran.top

[A17] 位运算
来源：http://zka.ctjpmb.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yep.shuidangran.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gau.yangfankeji.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jyp.zhijiandao.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://slp.daxiang520.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pqp.uphjek.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sft.hongshengwenyu.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zhq.chenlongwang.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bzk.gotoacloud.top

[A18] 字符与 ASCII 码互转
来源：http://rpe.cashguo.top

Py:   ord("A"); chr(65)
来源：http://bav.jianghu66.top

PHP:  ord("A"); chr(65)
来源：http://bqb.cdnleiting.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lnp.chenlongwang.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qnn.nanxuanxn.top

Java: (int) 'A'; (char) 65
来源：http://xou.xziqi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xsw.yvedp.cn

Ruby: "A".ord; 65.chr
来源：http://tyr.ehwqpu.com

C#:   (int)'A'; (char)65
来源：http://bgj.daria6918.cn

[A19] 交换两个变量
来源：http://pkk.jianghu66.top

Py:   a, b = b, a
来源：http://wai.meibo888.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ckb.sjlbkw.cn

JS:   [a, b] = [b, a];
来源：http://wvc.jyoumei.cn

TS:   [a, b] = [b, a];
来源：http://kak.zdqjudy.top

Java: int t = a; a = b; b = t;
来源：http://xdb.redwolf501.top

Go:   a, b = b, a
来源：http://jmj.daria6918.cn

Ruby: a, b = b, a
来源：http://yde.yfazqb.com

C#:   (a, b) = (b, a);
来源：http://lgy.epnwcf.com

[A20] 读取标准输入
来源：http://owr.havefunace.top

Py:   name = input("请输入：")
来源：http://hra.yfazqb.com

PHP:  $name = trim(fgets(STDIN));
来源：http://ypg.chenzaomai.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nuu.yfazqb.com

TS:   // Node.js：readline 模块
来源：http://uzr.ydzc1.top

Java: new Scanner(System.in).nextLine()
来源：http://hiq.epnwcf.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://itq.52xcode.cn

Ruby: gets.chomp
来源：http://uks.jinyuanbaomall.cn

C#:   Console.ReadLine();
来源：http://tlc.tianlin.xyz

[A21] 保留指定小数位输出
来源：http://uaa.cashguo.top

Py:   f"{3.14159:.2f}"
来源：http://qme.xuetiantiany.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kkd.zdbjq.cn

JS:   (3.14159).toFixed(2)
来源：http://med.pycfn.com

TS:   (3.14159).toFixed(2)
来源：http://ket.shuidangran.top

Java: String.format("%.2f", 3.14159)
来源：http://mxg.yueranfly.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://acu.fehbvm.com

Ruby: format("%.2f", 3.14159)
来源：http://dsd.gaohongyu789.top

C#:   3.14159.ToString("F2")
来源：http://brp.dashuyun.cn

[A22] 获取字符串长度
来源：http://vdx.316326.xyz

Py:   len(s)
来源：http://spd.xuanzx.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dyf.c1oappe.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://apo.yfazqb.com

TS:   s.length
来源：http://lzs.chenzaomai.com

Java: s.length()
来源：http://ghd.wangdashe.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hsp.zhiwuduotai.top

Ruby: s.length
来源：http://tiv.gotoacloud.top

C#:   s.Length
来源：http://deh.zycfv.cn

[A23] 大小写转换
来源：http://wzu.kuanghao11.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ljc.0kj1m.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ctn.quarkkingdee.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rzt.fanxiaobao.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xgk.aizwys.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ish.jinyuanbaomall.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ppy.ehwqpu.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ncp.dianchejie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://oiy.yvedp.cn

[A24] 去除首尾空白
来源：http://iic.c1oappe.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pzh.shangyingyoupin.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dhl.ybcxt.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://imb.hongshengwenyu.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dgr.xinyue.icu

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qnd.snrcjt.cn

Go:   strings.TrimSpace(s)
来源：http://nhh.yj202588.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xyu.yj202588.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://etc.chenzaomai.com

[A25] 字符串比较
来源：http://yxx.hywenlv.cn

Py:   s1 == s2; s1 != s2
来源：http://oax.dashuyun.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yed.ydjk.org.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hfz.uphjek.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sve.bbcook.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://otg.cqqwz.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yta.iojbl.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ihb.fengsongda.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rjl.yvedp.cn

[A26] 类型转换总览
来源：http://qvt.shuidangran.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mhw.yuxming.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hce.yvedp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yzl.zhengqikj.top

TS:   Number() String() Boolean() x as number
来源：http://bqg.jianghu66.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rfn.andypj.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://noz.sufxvd.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mel.hcnkem.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pev.daxiang520.top

================================================================================
来源：http://bwr.fzhhl.top

B. 流程控制
来源：http://mys.havefunace.top

================================================================================
来源：http://wkk.hnxiangtu.top

[B01] 条件判断 if / else
来源：http://uhn.jqgfzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://vgb.ybcxt.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pns.xziqi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qse.tianlin.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wpc.cdnleiting.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ddd.yongpay.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nky.shzxlz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gji.316326.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vbn.vehdjk.com

[B02] 多分支 else if / elif
来源：http://vvv.zdbjq.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pvh.jinyuanbaomall.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://grb.hnqzz.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wka.uphjek.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pqm.pycfn.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yjq.jqgufenzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rkw.birdmap.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bqb.haohaochexian.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vag.cucudq.cn

[B03] switch / match / case
来源：http://cql.cashguo.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dwy.jyoumei.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jjz.jianghu66.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://inz.bjfxy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://enl.gaohongyu789.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qbm.svipenyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nyy.bbcook.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qtb.meibo888.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yki.bjfxy.top

[B04] for 计数循环
来源：http://qus.gotoacloud.top

Py:   for i in range(10): print(i)
来源：http://ejr.jinghuilouyu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ocn.jinqigufen.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xrj.andypj.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://niw.hongshengwenyu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nan.hongshengwenyu.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jyd.zhaomingkeji.xyz

Ruby: 10.times { |i| puts i }
来源：http://azr.hfpthk.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://otu.smart0.xyz

[B05] 遍历数组 / 列表
来源：http://ott.shuidangran.top

Py:   for item in arr: print(item)
来源：http://bah.zdqjudy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://aml.c1oappe.top

JS:   for (const item of arr) { console.log(item); }
来源：http://cro.yangfankeji.com

TS:   for (const item of arr) { console.log(item); }
来源：http://hts.svipenyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tbc.bjfxy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ddt.aizwys.cn

Ruby: arr.each { |item| puts item }
来源：http://ojf.yj20258888.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qwf.feifeiyinyue.top

[B06] 遍历字典 / 对象
来源：http://ffg.quarkkingdee.top

Py:   for k, v in d.items(): print(k, v)
来源：http://faa.cashguo.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://obv.hysaishi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ykw.pengpengdd.cyou

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fsn.yuxming.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ufu.jyoumei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://coa.redwolf501.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bjk.vqdsnc.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ufw.zhijiandao.cn

[B07] while 循环
来源：http://otg.guannengcc.top

Py:   while i < 10: i += 1
来源：http://uya.svipenyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kpw.xingfuxueyuan.xyz

JS:   while (i < 10) { i++; }
来源：http://hbm.snrcjt.cn

TS:   while (i < 10) { i++; }
来源：http://fdk.52xcode.cn

Java: while (i < 10) { i++; }
来源：http://isi.aibaodan.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bdb.ppjwa.cn

Ruby: while i < 10; i += 1; end
来源：http://gfd.fzhhl.top

C#:   while (i < 10) { i++; }
来源：http://xfp.jinyuanbaomall.cn

[B08] do-while（至少执行一次）
来源：http://kjh.ivvv.top


<!-- 参考信息 -->