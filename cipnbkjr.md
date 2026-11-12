代发 wailian999

Py:   print("Hello, World!")
来源：http://dxi.sufxvd.cn

PHP:  echo "Hello, World!";
来源：http://rrc.hysaishi.cn

JS:   console.log("Hello, World!");
来源：http://axw.xziqi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gkd.shuidangran.top

Java: System.out.println("Hello, World!");
来源：http://dww.yongpay.top

Go:   fmt.Println("Hello, World!")
来源：http://icl.ybcxt.top

Ruby: puts "Hello, World!"
来源：http://feh.zhijiandao.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://epp.feifeiyinyue.top

[A02] 变量声明与赋值
来源：http://vkq.pengpengdd.cyou

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jwb.fengsongda.top

PHP:  $name = "Alex"; $age = 20;
来源：http://lwn.smart0.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://rrt.zhaomingkeji.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zmw.meibo888.top

Java: String name = "Alex"; int age = 20;
来源：http://ixp.tianlin.xyz

Go:   name := "Alex"; age := 20
来源：http://dqq.jyoumei.cn

Ruby: name = "Alex"; age = 20
来源：http://pza.daxiang520.top

C#:   string name = "Alex"; int age = 20;
来源：http://mze.yueranfly.top

[A03] 常量定义
来源：http://tsc.kuanghao11.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bxs.chenlongwang.top

PHP:  const PI = 3.14159;
来源：http://fxk.hcnkem.com

JS:   const PI = 3.14159;
来源：http://fba.smart0.xyz

TS:   const PI: number = 3.14159;
来源：http://egc.tarul.cn

Java: static final double PI = 3.14159;
来源：http://ryf.tian-w.cn

Go:   const PI = 3.14159
来源：http://pcc.cucudq.cn

Ruby: PI = 3.14159
来源：http://oqc.sweek.top

C#:   const double PI = 3.14159;
来源：http://aqo.feifeiyinyue.top

[A04] 判断变量类型
来源：http://iza.daxiang520.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://yph.pengpengdd.cyou

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dov.fzhhl.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pej.yj20258.top

TS:   typeof x; x instanceof Date
来源：http://hah.hysaishi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lxw.tian-w.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qvk.tarul.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kyh.jinghuilouyu.cn

C#:   x.GetType().Name; x is int
来源：http://mlx.xinyue.icu

[A05] 整数除法与取模
来源：http://lki.xuetiantiany.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ptb.jqgufenzy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://bkz.zhoulong.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ctj.gotoacloud.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://aih.yj20258888.top

Java: 7 / 2; 7 % 2
来源：http://vop.zhoulong.xyz

Go:   7 / 2; 7 % 2
来源：http://xwz.feifeiyinyue.top

Ruby: 7 / 2; 7 % 2
来源：http://pba.hnxiangtu.top

C#:   7 / 2; 7 % 2
来源：http://vrg.zdbjq.cn

[A06] 字符串转数字
来源：http://isp.yanxiufei.cn

Py:   int("42"); float("3.14")
来源：http://zoo.jyoumei.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qpk.dashuyun.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zsw.ywan-chungtsiang.top

TS:   parseInt("42", 10); Number("42")
来源：http://gxk.jqgfzy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fch.yfazqb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ysj.chenjidiqi.icu

Ruby: "42".to_i; "3.14".to_f
来源：http://zsy.yj202588.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fce.redwolf501.top

[A07] 数字转字符串
来源：http://xmg.xuetiantiany.cn

Py:   str(42)
来源：http://uje.yj20258888.top

PHP:  (string) 42; strval(42)
来源：http://yda.meibo888.top

JS:   String(42); (42).toString()
来源：http://ffi.jinqigufen.top

TS:   String(42)
来源：http://ant.chenjidiqi.icu

Java: String.valueOf(42); Integer.toString(42)
来源：http://dbr.yonumen.top

Go:   strconv.Itoa(42)
来源：http://clt.aizwys.cn

Ruby: 42.to_s
来源：http://tsc.jinqigufen.top

C#:   42.ToString()
来源：http://puf.ydzc1.top

[A08] 取整与四舍五入
来源：http://jld.shangyingyoupin.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bju.sufxvd.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bzf.cheryme.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ros.sweek.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xll.ydjk.org.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kaq.fehbvm.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sul.nwbrower.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://vee.yongpay.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hic.tian-w.cn

[A09] 绝对值与最大最小值
来源：http://clc.tian-w.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://abt.chenzaomai.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pdg.sxryk.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xob.xinyue.icu

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wqc.yvedp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://eom.sufxvd.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hvo.shanyushiyangtech.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jut.sxryk.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kex.ctjpmb.com

[A10] 生成随机数
来源：http://hhz.fehbvm.com

Py:   import random; random.randint(1, 100)
来源：http://orz.pengpengdd.cyou

PHP:  random_int(1, 100);
来源：http://afu.mhx1999.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://muk.havefunace.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baw.bbcook.cn

Java: new Random().nextInt(100) + 1
来源：http://kfp.fehbvm.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ane.jianghu66.top

Ruby: rand(1..100)
来源：http://ywk.sxryk.cn

C#:   new Random().Next(1, 101)
来源：http://lxu.xuanzx.com

[A11] 条件表达式（三元）
来源：http://bgt.yueranfly.top

Py:   "yes" if x > 0 else "no"
来源：http://ylp.ywan-chungtsiang.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://zru.wangshuangyany.cn

JS:   x > 0 ? "yes" : "no"
来源：http://oww.mhx1999.top

TS:   x > 0 ? "yes" : "no"
来源：http://wxq.wangdashe.top

Java: x > 0 ? "yes" : "no"
来源：http://yze.smart0.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://aoh.fzhhl.top

Ruby: x > 0 ? "yes" : "no"
来源：http://fea.andypj.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://yxi.jinghuilouyu.cn

[A12] 字符串插值 / 格式化
来源：http://mvk.yuanzhike.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://iio.yj20258.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fmm.gogol.net.cn

JS:   `Hello, ${name}!`
来源：http://suf.pengpengdd.cyou

TS:   `Hello, ${name}!`
来源：http://ehe.yj20258.top

Java: "Hello, %s!".formatted(name)
来源：http://wci.yvedp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ryh.jinyuanbaomall.cn

Ruby: "Hello, #{name}!"
来源：http://xih.iojbl.cn

C#:   $"Hello, {name}!"
来源：http://zbr.chenjidiqi.icu

[A13] 多行字符串（练习 \n 转义）
来源：http://vez.daria6918.cn

Py:   "第一行\n第二行"
来源：http://rny.jinqigfzy.top

PHP:  "第一行\n第二行"
来源：http://uri.hysaishi.cn

JS:   "第一行\n第二行"
来源：http://yvg.tanke756.top

TS:   "第一行\n第二行"
来源：http://rot.ehwqpu.com

Java: "第一行\n第二行"
来源：http://huv.gogol.net.cn

Go:   "第一行\n第二行"
来源：http://cov.aizwys.cn

Ruby: "第一行\n第二行"
来源：http://ups.vehdjk.com

C#:   "第一行\n第二行"
来源：http://nbd.shangyingyoupin.top

[A14] 注释写法
来源：http://rkr.snrcjt.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xoy.cucudq.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://llv.ehwqpu.com

JS:   // 单行；/* 多行 */
来源：http://lpw.ppjwa.cn

TS:   // 单行；/* 多行 */
来源：http://izq.yuxming.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vqi.tian-w.cn

Go:   // 单行；/* 多行 */
来源：http://yih.jqgfzy.top

Ruby: # 单行；=begin 多行 =end
来源：http://gzl.mhx1999.top

C#:   // 单行；/* 多行 */
来源：http://wpd.yj20258888.top

[A15] 空值判断与默认值
来源：http://suv.nanxinkj.top

Py:   value = data or "默认值"
来源：http://nej.tianlin.xyz

PHP:  $value = $data ?? "默认值";
来源：http://fpp.cheryme.top

JS:   const value = data ?? "默认值";
来源：http://dpx.yj20258888.top

TS:   const value = data ?? "默认值";
来源：http://irk.yfazqb.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mnq.jinyuanbaomall.cn

Go:   if data == "" { data = "默认值" }
来源：http://crl.cheryme.top

Ruby: value = data || "默认值"
来源：http://rng.yj202588.top

C#:   var value = data ?? "默认值";
来源：http://vhb.aibaodan.cn

[A16] 真假值判断规则
来源：http://zdv.meibo888.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sgx.wangdashe.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fud.shangyingyoupin.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kuy.ydjk.org.cn

TS:   if (!x) {}
来源：http://ikb.jinqigfzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rmw.andypj.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qwy.nanxuanxn.top

Ruby: unless x            # nil 与 false 为假
来源：http://mek.zhongyouzk.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://caa.hnxiangtu.top

[A17] 位运算
来源：http://gih.xylfe.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fjz.yangfankeji.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ovu.sufxvd.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pwk.hongshengwenyu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rew.shanyushiyangkeji.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tds.yuanzhike.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pso.yj202588.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bmp.tian-w.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://axq.yvedp.cn

[A18] 字符与 ASCII 码互转
来源：http://gmr.quarkkingdee.top

Py:   ord("A"); chr(65)
来源：http://rpu.shzxlz.cn

PHP:  ord("A"); chr(65)
来源：http://dwm.xuetiantiany.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tik.svipenyu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://otg.smart0.xyz

Java: (int) 'A'; (char) 65
来源：http://bas.tian-w.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jjz.jinqigufen.top

Ruby: "A".ord; 65.chr
来源：http://fba.epnwcf.com

C#:   (int)'A'; (char)65
来源：http://bdd.yvedp.cn

[A19] 交换两个变量
来源：http://zfr.tarul.cn

Py:   a, b = b, a
来源：http://akh.gzhubu.top

PHP:  [$a, $b] = [$b, $a];
来源：http://oyu.mhx1999.top

JS:   [a, b] = [b, a];
来源：http://qru.nanxuanxn.top

TS:   [a, b] = [b, a];
来源：http://jii.0kj1m.cn

Java: int t = a; a = b; b = t;
来源：http://ejy.yj20258.top

Go:   a, b = b, a
来源：http://yhy.andypj.xyz

Ruby: a, b = b, a
来源：http://yja.ybcxt.top

C#:   (a, b) = (b, a);
来源：http://ebx.fengsongda.top

[A20] 读取标准输入
来源：http://erv.cdnleiting.top

Py:   name = input("请输入：")
来源：http://ejz.xuetiantiany.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ehh.ybcxt.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mlk.cashguo.top

TS:   // Node.js：readline 模块
来源：http://rpz.jlsjyb.cn

Java: new Scanner(System.in).nextLine()
来源：http://mbi.xylfe.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pjg.guowangkeji.top

Ruby: gets.chomp
来源：http://dqq.nwbrower.top

C#:   Console.ReadLine();
来源：http://dqf.chenlongwang.top

[A21] 保留指定小数位输出
来源：http://ghb.aibaodan.cn

Py:   f"{3.14159:.2f}"
来源：http://qpy.yj20258.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vuw.tanke756.top

JS:   (3.14159).toFixed(2)
来源：http://wjs.snrcjt.cn

TS:   (3.14159).toFixed(2)
来源：http://ehr.c1oappe.top

Java: String.format("%.2f", 3.14159)
来源：http://hnx.zdbjq.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jhx.gotoacloud.top

Ruby: format("%.2f", 3.14159)
来源：http://ame.yfazqb.com

C#:   3.14159.ToString("F2")
来源：http://ujx.andypj.xyz

[A22] 获取字符串长度
来源：http://omt.hysaishi.cn

Py:   len(s)
来源：http://qjc.wangshuangyany.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mta.uphjek.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://byy.zdbjq.cn

TS:   s.length
来源：http://tvv.uphjek.com

Java: s.length()
来源：http://gvp.gotoacloud.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kia.wangshuangyany.cn

Ruby: s.length
来源：http://hhk.feifeiyinyue.top

C#:   s.Length
来源：http://day.ehwqpu.com

[A23] 大小写转换
来源：http://ard.chenzaomai.com

Py:   s.upper(); s.lower(); s.title()
来源：http://jzj.jinqigfzy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ocv.ivvv.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bam.uphjek.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://doy.yongpay.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jzg.yj20258.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yck.hammf.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://shl.sjlbkw.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ssy.jinghuilouyu.cn

[A24] 去除首尾空白
来源：http://nge.cqqwz.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wvw.cashguo.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vkk.daxiang520.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wti.yuanzhike.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lng.wangshuangyany.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kic.zhongyouzk.top

Go:   strings.TrimSpace(s)
来源：http://sur.tian-w.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kow.gaohongyu789.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mze.daria6918.cn

[A25] 字符串比较
来源：http://ths.shanyushiyangkeji.top

Py:   s1 == s2; s1 != s2
来源：http://gvi.gogol.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gwo.nwbrower.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wfz.ydjk.org.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://iyy.xziqi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gds.zhengqikj.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qsa.tian-w.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ckj.pycfn.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xyo.bbcook.cn

[A26] 类型转换总览
来源：http://ris.zhijiandao.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tea.ehwqpu.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gii.c1oappe.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dsv.sufxvd.cn

TS:   Number() String() Boolean() x as number
来源：http://fwx.jqgufenzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hau.jqgfzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://aio.jlsjyb.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lqn.fengsongda.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bue.andypj.xyz

================================================================================
来源：http://cbh.zhaomingkeji.xyz

B. 流程控制
来源：http://phq.fengsongda.top

================================================================================
来源：http://wfu.shuidangran.top

[B01] 条件判断 if / else
来源：http://mfw.hnqzz.top

Py:   result = "正" if x > 0 else "非正"
来源：http://skb.sjlbkw.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pqe.sweek.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mio.jianghu66.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wji.nanxinkj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cud.sjlbkw.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://feo.cqqwz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bqk.uphjek.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jzu.svipenyu.cn

[B02] 多分支 else if / elif
来源：http://zgf.mhx1999.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://roj.zhaomingkeji.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wgt.sjlbkw.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uzu.chenzaomai.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://omv.zhoulong.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cjw.52xcode.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ndl.mhx1999.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zhn.ydzc1.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zrw.hnxiangtu.top

[B03] switch / match / case
来源：http://rxf.hfpthk.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pot.ppjwa.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gxw.tianlin.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vnz.tian-w.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://and.chenlongwang.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dqn.daxiang520.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mpc.cucudq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bic.sjlbkw.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yuz.sweek.top

[B04] for 计数循环
来源：http://fgj.ydzc1.top

Py:   for i in range(10): print(i)
来源：http://uyf.sweek.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hdo.gogol.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rrl.andypj.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wmg.zhiwuduotai.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://peb.ehwqpu.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ljf.jlsjyb.cn

Ruby: 10.times { |i| puts i }
来源：http://kla.ehwqpu.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xxi.shuidangran.top

[B05] 遍历数组 / 列表
来源：http://trv.aizwys.cn

Py:   for item in arr: print(item)
来源：http://jux.ehwqpu.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wqo.fehbvm.com

JS:   for (const item of arr) { console.log(item); }
来源：http://knh.tanke756.top

TS:   for (const item of arr) { console.log(item); }
来源：http://jgz.sjlbkw.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bgn.xziqi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xfe.wangdashe.top

Ruby: arr.each { |item| puts item }
来源：http://jei.haohaochexian.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vyt.ivvv.top

[B06] 遍历字典 / 对象
来源：http://rcr.tian-w.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ekb.cheryme.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lhq.yuanzhike.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://big.svipenyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dtg.feifeiyinyue.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wrm.fanxiaobao.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wzf.zycfv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vpf.chenjidiqi.icu

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vqg.cucudq.cn

[B07] while 循环
来源：http://rig.nanxuanxn.top

Py:   while i < 10: i += 1
来源：http://pke.vqdsnc.cn

PHP:  while ($i < 10) { $i++; }
来源：http://quz.c1oappe.top

JS:   while (i < 10) { i++; }
来源：http://ehi.feifeiyinyue.top

TS:   while (i < 10) { i++; }
来源：http://kzm.zycfv.cn

Java: while (i < 10) { i++; }
来源：http://zno.daria6918.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eps.vehdjk.com

Ruby: while i < 10; i += 1; end
来源：http://izl.shzxlz.cn

C#:   while (i < 10) { i++; }
来源：http://bkl.shanyushiyangtech.top

[B08] do-while（至少执行一次）
来源：http://tmr.zdqjudy.top


<!-- 参考信息 -->