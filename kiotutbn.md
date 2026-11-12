代发 wailian999

Py:   print("Hello, World!")
来源：http://ael.shzxlz.cn

PHP:  echo "Hello, World!";
来源：http://ewq.dianchejie.cn

JS:   console.log("Hello, World!");
来源：http://zmm.gogol.net.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://opa.hywenlv.cn

Java: System.out.println("Hello, World!");
来源：http://tvc.ydjk.org.cn

Go:   fmt.Println("Hello, World!")
来源：http://plv.gogol.net.cn

Ruby: puts "Hello, World!"
来源：http://glz.nwbrower.top

C#:   Console.WriteLine("Hello, World!");
来源：http://lts.hammf.cn

[A02] 变量声明与赋值
来源：http://sik.bbcook.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mcr.vehdjk.com

PHP:  $name = "Alex"; $age = 20;
来源：http://mwz.bjfxy.top

JS:   let name = "Alex"; const age = 20;
来源：http://fvi.xuanzx.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cxu.bbcook.cn

Java: String name = "Alex"; int age = 20;
来源：http://crb.feifeiyinyue.top

Go:   name := "Alex"; age := 20
来源：http://lzs.haohaochexian.top

Ruby: name = "Alex"; age = 20
来源：http://kra.redwolf501.top

C#:   string name = "Alex"; int age = 20;
来源：http://lij.hnxiangtu.top

[A03] 常量定义
来源：http://uzt.aibaodan.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lnt.vqdsnc.cn

PHP:  const PI = 3.14159;
来源：http://bvx.ehwqpu.com

JS:   const PI = 3.14159;
来源：http://thh.guowangkeji.top

TS:   const PI: number = 3.14159;
来源：http://nec.vqdsnc.cn

Java: static final double PI = 3.14159;
来源：http://khu.hongshengwenyu.top

Go:   const PI = 3.14159
来源：http://ijq.xingfuxueyuan.xyz

Ruby: PI = 3.14159
来源：http://jtj.shzxlz.cn

C#:   const double PI = 3.14159;
来源：http://txh.jinghuilouyu.cn

[A04] 判断变量类型
来源：http://cog.xuanzx.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://glg.xziqi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gvr.ybcxt.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rni.ywan-chungtsiang.top

TS:   typeof x; x instanceof Date
来源：http://xnw.haohaochexian.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kal.meibo888.top

Go:   reflect.TypeOf(x).Name()
来源：http://xjx.shangyingyoupin.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ndj.yanxiufei.cn

C#:   x.GetType().Name; x is int
来源：http://dod.nanxuanxn.top

[A05] 整数除法与取模
来源：http://sms.wangdashe.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://img.ybcxt.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://jzw.cqqwz.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://isy.tian-w.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vhx.vqdsnc.cn

Java: 7 / 2; 7 % 2
来源：http://rpe.hesvh.cn

Go:   7 / 2; 7 % 2
来源：http://onx.gogol.net.cn

Ruby: 7 / 2; 7 % 2
来源：http://rvc.aizwys.cn

C#:   7 / 2; 7 % 2
来源：http://aiw.epnwcf.com

[A06] 字符串转数字
来源：http://gez.gaohongyu789.top

Py:   int("42"); float("3.14")
来源：http://tln.hnxiangtu.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dhe.zdqjudy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hnv.gaohongyu789.top

TS:   parseInt("42", 10); Number("42")
来源：http://wgh.snrcjt.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ggo.tian-w.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://niw.chenlongwang.top

Ruby: "42".to_i; "3.14".to_f
来源：http://zow.ppjwa.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ajw.jinqigfzy.top

[A07] 数字转字符串
来源：http://lco.nanxinkj.top

Py:   str(42)
来源：http://zhb.cqqwz.cn

PHP:  (string) 42; strval(42)
来源：http://vzd.iojbl.cn

JS:   String(42); (42).toString()
来源：http://vei.ydzc1.top

TS:   String(42)
来源：http://ums.xylfe.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://iut.sufxvd.cn

Go:   strconv.Itoa(42)
来源：http://suy.hysaishi.cn

Ruby: 42.to_s
来源：http://vvl.jqgfzy.top

C#:   42.ToString()
来源：http://egs.hfpthk.cn

[A08] 取整与四舍五入
来源：http://lik.zhixingplan.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ogp.chenzaomai.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fbt.ydjk.org.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://itd.chenlongwang.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://biq.ctjpmb.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dpe.chenlongwang.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://oqj.yj202588.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://miv.tianlin.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zzc.gzhubu.top

[A09] 绝对值与最大最小值
来源：http://ino.ydzc1.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xbw.nanxinkj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fxr.guowangkeji.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ykr.hnqzz.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gzt.xylfe.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cjs.ywan-chungtsiang.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jcv.zhongyouzk.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://afr.aizwys.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://aze.wangdashe.top

[A10] 生成随机数
来源：http://qrb.iojbl.cn

Py:   import random; random.randint(1, 100)
来源：http://sru.hesvh.cn

PHP:  random_int(1, 100);
来源：http://qme.tanke756.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jzv.fktsv.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://owd.meibo888.top

Java: new Random().nextInt(100) + 1
来源：http://zkk.kuanghao11.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jux.guowangkeji.top

Ruby: rand(1..100)
来源：http://lez.smart0.xyz

C#:   new Random().Next(1, 101)
来源：http://tcs.zhaomingkeji.xyz

[A11] 条件表达式（三元）
来源：http://mdt.sweek.top

Py:   "yes" if x > 0 else "no"
来源：http://oxi.chenzaomai.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://qnc.nanxinkj.top

JS:   x > 0 ? "yes" : "no"
来源：http://bwf.havefunace.top

TS:   x > 0 ? "yes" : "no"
来源：http://pej.xuetiantiany.cn

Java: x > 0 ? "yes" : "no"
来源：http://kpq.redwolf501.top

Go:   // 无三元运算符，需用 if 语句
来源：http://okn.zdqjudy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ain.dianchejie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://kqj.xinyue.icu

[A12] 字符串插值 / 格式化
来源：http://qcf.aibaodan.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yon.yj202588.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hff.hcnkem.com

JS:   `Hello, ${name}!`
来源：http://jep.cucudq.cn

TS:   `Hello, ${name}!`
来源：http://dlh.jinqigufen.top

Java: "Hello, %s!".formatted(name)
来源：http://djl.meibo888.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cgo.yuxming.cn

Ruby: "Hello, #{name}!"
来源：http://wbm.yongpay.top

C#:   $"Hello, {name}!"
来源：http://aqg.jqgfzy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://qkz.dashuyun.cn

Py:   "第一行\n第二行"
来源：http://dmf.cqqwz.cn

PHP:  "第一行\n第二行"
来源：http://lln.jinqigufen.top

JS:   "第一行\n第二行"
来源：http://wbo.guannengcc.top

TS:   "第一行\n第二行"
来源：http://kde.yonumen.top

Java: "第一行\n第二行"
来源：http://jiz.xinyue.icu

Go:   "第一行\n第二行"
来源：http://nxi.hcnkem.com

Ruby: "第一行\n第二行"
来源：http://xtu.zhijiandao.cn

C#:   "第一行\n第二行"
来源：http://gfe.gogol.net.cn

[A14] 注释写法
来源：http://vsx.wangdashe.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://vtt.shanyushiyangtech.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://hla.yanxiufei.cn

JS:   // 单行；/* 多行 */
来源：http://lqh.meibo888.top

TS:   // 单行；/* 多行 */
来源：http://fxr.shuidangran.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://usw.feifeiyinyue.top

Go:   // 单行；/* 多行 */
来源：http://pqq.gaohongyu789.top

Ruby: # 单行；=begin 多行 =end
来源：http://ory.chenjidiqi.icu

C#:   // 单行；/* 多行 */
来源：http://tsm.guannengcc.top

[A15] 空值判断与默认值
来源：http://tih.yvedp.cn

Py:   value = data or "默认值"
来源：http://abn.vehdjk.com

PHP:  $value = $data ?? "默认值";
来源：http://hik.ydzc1.top

JS:   const value = data ?? "默认值";
来源：http://zra.guowangkeji.top

TS:   const value = data ?? "默认值";
来源：http://neh.yj202588.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wwa.cdnleiting.top

Go:   if data == "" { data = "默认值" }
来源：http://mdk.pycfn.com

Ruby: value = data || "默认值"
来源：http://alq.bbcook.cn

C#:   var value = data ?? "默认值";
来源：http://zgx.xingfuxueyuan.xyz

[A16] 真假值判断规则
来源：http://fhm.xziqi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jgr.zhijiandao.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ahl.zhongyouzk.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://obd.zdbjq.cn

TS:   if (!x) {}
来源：http://afs.dashuyun.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gej.jqgufenzy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qgr.yj20258.top

Ruby: unless x            # nil 与 false 为假
来源：http://dfv.ctjpmb.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://shg.ydzc1.top

[A17] 位运算
来源：http://mbp.guannengcc.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fmi.chenzaomai.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://afe.snrcjt.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://izx.zdbjq.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ckd.ydjk.org.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cuc.tanke756.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://upo.xylfe.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vyr.fktsv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ixv.9152youxi.cn

[A18] 字符与 ASCII 码互转
来源：http://wwk.fengsongda.top

Py:   ord("A"); chr(65)
来源：http://aed.xylfe.cn

PHP:  ord("A"); chr(65)
来源：http://tdd.zdqjudy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://din.yvedp.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ios.xinyue.icu

Java: (int) 'A'; (char) 65
来源：http://cqf.yongpay.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://noc.zhengqikj.top

Ruby: "A".ord; 65.chr
来源：http://wug.meibo888.top

C#:   (int)'A'; (char)65
来源：http://vqg.yonumen.top

[A19] 交换两个变量
来源：http://cmn.vqdsnc.cn

Py:   a, b = b, a
来源：http://hgr.zhixingplan.top

PHP:  [$a, $b] = [$b, $a];
来源：http://fpi.yfazqb.com

JS:   [a, b] = [b, a];
来源：http://aem.ybcxt.top

TS:   [a, b] = [b, a];
来源：http://oau.hywenlv.cn

Java: int t = a; a = b; b = t;
来源：http://cub.hywenlv.cn

Go:   a, b = b, a
来源：http://jio.xuanzx.com

Ruby: a, b = b, a
来源：http://qic.zhengqikj.top

C#:   (a, b) = (b, a);
来源：http://ryr.cdnleiting.top

[A20] 读取标准输入
来源：http://ioi.shanyushiyangkeji.top

Py:   name = input("请输入：")
来源：http://gfo.hfpthk.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dfr.tanke756.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hgw.gotoacloud.top

TS:   // Node.js：readline 模块
来源：http://gbg.fehbvm.com

Java: new Scanner(System.in).nextLine()
来源：http://won.uphjek.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://odf.gotoacloud.top

Ruby: gets.chomp
来源：http://noh.epnwcf.com

C#:   Console.ReadLine();
来源：http://wyt.xylfe.cn

[A21] 保留指定小数位输出
来源：http://qan.shanyushiyangkeji.top

Py:   f"{3.14159:.2f}"
来源：http://osk.zycfv.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xkm.dashuyun.cn

JS:   (3.14159).toFixed(2)
来源：http://ahd.hywenlv.cn

TS:   (3.14159).toFixed(2)
来源：http://ole.jqgufenzy.top

Java: String.format("%.2f", 3.14159)
来源：http://gyq.guannengcc.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xoi.jinqigufen.top

Ruby: format("%.2f", 3.14159)
来源：http://irc.daxiang520.top

C#:   3.14159.ToString("F2")
来源：http://wvu.shangyingyoupin.top

[A22] 获取字符串长度
来源：http://yjo.iojbl.cn

Py:   len(s)
来源：http://kfj.cdnleiting.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://iqn.yuanzhike.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kbs.zycfv.cn

TS:   s.length
来源：http://urj.haohaochexian.top

Java: s.length()
来源：http://trf.zycfv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kfy.ydjk.org.cn

Ruby: s.length
来源：http://dtz.hysaishi.cn

C#:   s.Length
来源：http://pic.cashguo.top

[A23] 大小写转换
来源：http://hdq.bjfxy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://yis.zhengqikj.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mcq.cqqwz.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qgc.yonumen.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wbu.jinqigufen.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ykp.ybcxt.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pum.fehbvm.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jle.fehbvm.com

C#:   s.ToUpper(); s.ToLower()
来源：http://mhr.nanxuanxn.top

[A24] 去除首尾空白
来源：http://ied.yfazqb.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dvz.fehbvm.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oxw.shanyushiyangkeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://voa.shanyushiyangkeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://goa.wangshuangyany.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lww.tanke756.top

Go:   strings.TrimSpace(s)
来源：http://dtl.havefunace.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hzz.dianchejie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://edf.52xcode.cn

[A25] 字符串比较
来源：http://lrw.bbcook.cn

Py:   s1 == s2; s1 != s2
来源：http://nkv.yfazqb.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://agb.chenzaomai.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mzn.smart0.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wvm.yuxming.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hyi.zhengqikj.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pda.ydzc1.top

Ruby: s1 == s2; s1 <=> s2
来源：http://tkq.jqgufenzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vyl.andypj.xyz

[A26] 类型转换总览
来源：http://rha.vqdsnc.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://itu.pycfn.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kxs.tian-w.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ghn.tian-w.cn

TS:   Number() String() Boolean() x as number
来源：http://hme.redwolf501.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qwk.jinqigfzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mcr.xziqi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ypp.chenlongwang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bub.xuanzx.com

================================================================================
来源：http://lyx.gzhubu.top

B. 流程控制
来源：http://icb.zhongyouzk.top

================================================================================
来源：http://elz.zycfv.cn

[B01] 条件判断 if / else
来源：http://zzm.quarkkingdee.top

Py:   result = "正" if x > 0 else "非正"
来源：http://cfo.ydzc1.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pvh.gotoacloud.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hmh.sufxvd.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xxg.yanxiufei.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://szi.ywan-chungtsiang.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zgc.hnqzz.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xjl.zdbjq.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://iyy.cashguo.top

[B02] 多分支 else if / elif
来源：http://qsg.zhaomingkeji.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zes.jlsjyb.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://evc.gaohongyu789.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://awe.ybcxt.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yza.mhx1999.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ufw.cucudq.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qba.yj202588.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dht.jianghu66.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hnh.ehwqpu.com

[B03] switch / match / case
来源：http://dgq.redwolf501.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yev.yj20258.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dzo.cdnleiting.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jnh.sxryk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mfs.xuanzx.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dim.kuanghao11.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://evw.feifeiyinyue.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pjk.havefunace.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pxf.dianchejie.cn

[B04] for 计数循环
来源：http://qro.9152youxi.cn

Py:   for i in range(10): print(i)
来源：http://wjt.tarul.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jwe.zhengqikj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hcv.cucudq.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bpm.shuidangran.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lgi.shangyingyoupin.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lco.wangshuangyany.cn

Ruby: 10.times { |i| puts i }
来源：http://gug.cdnleiting.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://peh.yangfankeji.com

[B05] 遍历数组 / 列表
来源：http://dvg.ctjpmb.com

Py:   for item in arr: print(item)
来源：http://bkp.cheryme.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://liy.hesvh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nzx.c1oappe.top

TS:   for (const item of arr) { console.log(item); }
来源：http://dbp.uphjek.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://jrl.fktsv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ihy.yanxiufei.cn

Ruby: arr.each { |item| puts item }
来源：http://sjk.zdbjq.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jmp.ivvv.top

[B06] 遍历字典 / 对象
来源：http://khb.vehdjk.com

Py:   for k, v in d.items(): print(k, v)
来源：http://fwi.vehdjk.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mle.gogol.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wcx.sysykeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dfp.redwolf501.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://smx.ydjk.org.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uti.sweek.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sge.sjlbkw.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uzq.sjlbkw.cn

[B07] while 循环
来源：http://uwx.wangdashe.top

Py:   while i < 10: i += 1
来源：http://rhb.shanyushiyangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://yjz.ydjk.org.cn

JS:   while (i < 10) { i++; }
来源：http://aqe.hywenlv.cn

TS:   while (i < 10) { i++; }
来源：http://eel.zycfv.cn

Java: while (i < 10) { i++; }
来源：http://vke.zdbjq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rao.guowangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://qbc.hammf.cn

C#:   while (i < 10) { i++; }
来源：http://nqe.wangdashe.top

[B08] do-while（至少执行一次）
来源：http://hcd.kuanghao11.cn


<!-- 参考信息 -->