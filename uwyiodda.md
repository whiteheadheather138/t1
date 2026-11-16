代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://tun.fengsongda.top

Go:   fmt.Println("Hello, World!")
来源：http://mdw.zhongyouzk.top

Ruby: puts "Hello, World!"
来源：http://ufg.52xcode.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xjx.haohaochexian.top

[A02] 变量声明与赋值
来源：http://fac.pengpengdd.cyou

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ifa.xylfe.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qwv.sysykeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://bfb.cdnleiting.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pba.9152youxi.cn

Java: String name = "Alex"; int age = 20;
来源：http://aiw.yongpay.top

Go:   name := "Alex"; age := 20
来源：http://ehw.quarkkingdee.top

Ruby: name = "Alex"; age = 20
来源：http://wub.svipenyu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://sma.xuetiantiany.cn

[A03] 常量定义
来源：http://tki.ivvv.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lgb.yangfankeji.com

PHP:  const PI = 3.14159;
来源：http://lhh.yj202588.top

JS:   const PI = 3.14159;
来源：http://ebm.jinyuanbaomall.cn

TS:   const PI: number = 3.14159;
来源：http://hcd.zycfv.cn

Java: static final double PI = 3.14159;
来源：http://yto.xuanzx.com

Go:   const PI = 3.14159
来源：http://sdi.jlsjyb.cn

Ruby: PI = 3.14159
来源：http://adi.yuxming.cn

C#:   const double PI = 3.14159;
来源：http://rnh.gotoacloud.top

[A04] 判断变量类型
来源：http://drq.hfpthk.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hzw.hnxiangtu.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ali.jinqigufen.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lwv.yuanzhike.top

TS:   typeof x; x instanceof Date
来源：http://dhc.jianghu66.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hdc.birdmap.top

Go:   reflect.TypeOf(x).Name()
来源：http://ssd.hnqzz.top

Ruby: x.class; x.is_a?(Integer)
来源：http://mvh.pengpengdd.cyou

C#:   x.GetType().Name; x is int
来源：http://eqf.gogol.net.cn

[A05] 整数除法与取模
来源：http://sud.yfazqb.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jtp.wangshuangyany.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://bco.tanke756.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fxt.chenjidiqi.icu

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kbe.iojbl.cn

Java: 7 / 2; 7 % 2
来源：http://psu.yonumen.top

Go:   7 / 2; 7 % 2
来源：http://xcm.jinqigufen.top

Ruby: 7 / 2; 7 % 2
来源：http://yjb.shanyushiyangkeji.top

C#:   7 / 2; 7 % 2
来源：http://gpc.kuanghao11.cn

[A06] 字符串转数字
来源：http://tyr.fanxiaobao.xyz

Py:   int("42"); float("3.14")
来源：http://ael.ydzc1.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dbv.52xcode.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ray.jinqigufen.top

TS:   parseInt("42", 10); Number("42")
来源：http://wes.yj20258888.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://sht.gzhubu.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cpi.cdnleiting.top

Ruby: "42".to_i; "3.14".to_f
来源：http://xfm.zhengqikj.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://viz.zdbjq.cn

[A07] 数字转字符串
来源：http://spd.hywenlv.cn

Py:   str(42)
来源：http://kaj.shanyushiyangkeji.top

PHP:  (string) 42; strval(42)
来源：http://agl.tian-w.cn

JS:   String(42); (42).toString()
来源：http://vws.fzhhl.top

TS:   String(42)
来源：http://lwl.zhengqikj.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://qil.hywenlv.cn

Go:   strconv.Itoa(42)
来源：http://grd.0kj1m.cn

Ruby: 42.to_s
来源：http://aea.jianghu66.top

C#:   42.ToString()
来源：http://vus.guannengcc.top

[A08] 取整与四舍五入
来源：http://mqj.hcnkem.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uxm.sweek.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lsw.vqdsnc.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cta.nanxuanxn.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xxr.gzhubu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gyo.svipenyu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qsu.fktsv.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://tvt.mhx1999.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kna.smart0.xyz

[A09] 绝对值与最大最小值
来源：http://szv.hcnkem.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jyu.yfazqb.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pix.gotoacloud.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://eor.chenjidiqi.icu

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mvh.hnxiangtu.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dof.redwolf501.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kge.yuanzhike.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hqe.yongpay.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://din.jinyuanbaomall.cn

[A10] 生成随机数
来源：http://rlz.hongshengwenyu.top

Py:   import random; random.randint(1, 100)
来源：http://mzn.zycfv.cn

PHP:  random_int(1, 100);
来源：http://bfg.vehdjk.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://udr.vqdsnc.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hgy.ybcxt.top

Java: new Random().nextInt(100) + 1
来源：http://hks.yj202588.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://opc.c1oappe.top

Ruby: rand(1..100)
来源：http://mqm.haohaochexian.top

C#:   new Random().Next(1, 101)
来源：http://asz.fzhhl.top

[A11] 条件表达式（三元）
来源：http://uou.xuanzx.com

Py:   "yes" if x > 0 else "no"
来源：http://pxd.havefunace.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://yor.nwbrower.top

JS:   x > 0 ? "yes" : "no"
来源：http://kmp.52xcode.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dbv.jinghuilouyu.cn

Java: x > 0 ? "yes" : "no"
来源：http://xxi.gaohongyu789.top

Go:   // 无三元运算符，需用 if 语句
来源：http://hqn.zhoulong.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://usr.c1oappe.top

C#:   x > 0 ? "yes" : "no"
来源：http://djv.xziqi.cn

[A12] 字符串插值 / 格式化
来源：http://bni.hammf.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://glg.zhaomingkeji.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rqh.cqqwz.cn

JS:   `Hello, ${name}!`
来源：http://zsu.9152youxi.cn

TS:   `Hello, ${name}!`
来源：http://hjs.jqgufenzy.top

Java: "Hello, %s!".formatted(name)
来源：http://usg.sxryk.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pux.zhengqikj.top

Ruby: "Hello, #{name}!"
来源：http://vyy.xingfuxueyuan.xyz

C#:   $"Hello, {name}!"
来源：http://jsg.fzhhl.top

[A13] 多行字符串（练习 \n 转义）
来源：http://pao.316326.xyz

Py:   "第一行\n第二行"
来源：http://fux.xylfe.cn

PHP:  "第一行\n第二行"
来源：http://jkb.tianlin.xyz

JS:   "第一行\n第二行"
来源：http://svx.hysaishi.cn

TS:   "第一行\n第二行"
来源：http://zxr.nwbrower.top

Java: "第一行\n第二行"
来源：http://grk.dianchejie.cn

Go:   "第一行\n第二行"
来源：http://vmf.zdbjq.cn

Ruby: "第一行\n第二行"
来源：http://seu.zhaomingkeji.xyz

C#:   "第一行\n第二行"
来源：http://ufs.yfazqb.com

[A14] 注释写法
来源：http://pet.zhengqikj.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://myr.zdqjudy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://pji.316326.xyz

JS:   // 单行；/* 多行 */
来源：http://aqi.xuetiantiany.cn

TS:   // 单行；/* 多行 */
来源：http://yxt.yj202588.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cag.yanxiufei.cn

Go:   // 单行；/* 多行 */
来源：http://bxe.sweek.top

Ruby: # 单行；=begin 多行 =end
来源：http://oyp.gogol.net.cn

C#:   // 单行；/* 多行 */
来源：http://xwj.zhoulong.xyz

[A15] 空值判断与默认值
来源：http://prk.jinyuanbaomall.cn

Py:   value = data or "默认值"
来源：http://okf.xuanzx.com

PHP:  $value = $data ?? "默认值";
来源：http://uax.tanke756.top

JS:   const value = data ?? "默认值";
来源：http://hzh.smart0.xyz

TS:   const value = data ?? "默认值";
来源：http://gyo.zhaomingkeji.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ftd.yj202588.top

Go:   if data == "" { data = "默认值" }
来源：http://los.yuxming.cn

Ruby: value = data || "默认值"
来源：http://nbs.wangdashe.top

C#:   var value = data ?? "默认值";
来源：http://lti.hysaishi.cn

[A16] 真假值判断规则
来源：http://dfs.andypj.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://iob.0kj1m.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://chh.9152youxi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tah.fktsv.cn

TS:   if (!x) {}
来源：http://skw.wangshuangyany.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dgo.yongpay.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vqi.yj20258888.top

Ruby: unless x            # nil 与 false 为假
来源：http://ocm.sjlbkw.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fks.haohaochexian.top

[A17] 位运算
来源：http://rew.hfpthk.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qsr.hnxiangtu.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ley.shzxlz.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qdg.xziqi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qls.fzhhl.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jdq.gaohongyu789.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://omx.jinghuilouyu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://luu.kuanghao11.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://leq.tarul.cn

[A18] 字符与 ASCII 码互转
来源：http://szv.cucudq.cn

Py:   ord("A"); chr(65)
来源：http://oqn.xinyue.icu

PHP:  ord("A"); chr(65)
来源：http://pku.hywenlv.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vhp.9152youxi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jde.ppjwa.cn

Java: (int) 'A'; (char) 65
来源：http://mow.yuxming.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dmv.hammf.cn

Ruby: "A".ord; 65.chr
来源：http://rrb.yanxiufei.cn

C#:   (int)'A'; (char)65
来源：http://cjw.shangyingyoupin.top

[A19] 交换两个变量
来源：http://qnj.jiagoushi.top

Py:   a, b = b, a
来源：http://rbz.svipenyu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://agt.nanxuanxn.top

JS:   [a, b] = [b, a];
来源：http://ast.shanyushiyangtech.top

TS:   [a, b] = [b, a];
来源：http://kej.yj20258.top

Java: int t = a; a = b; b = t;
来源：http://ubq.sweek.top

Go:   a, b = b, a
来源：http://wtw.vqdsnc.cn

Ruby: a, b = b, a
来源：http://pyr.hcnkem.com

C#:   (a, b) = (b, a);
来源：http://caf.snrcjt.cn

[A20] 读取标准输入
来源：http://hcx.fzhhl.top

Py:   name = input("请输入：")
来源：http://tjh.chenzaomai.com

PHP:  $name = trim(fgets(STDIN));
来源：http://bnk.haohaochexian.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hxr.cdnleiting.top

TS:   // Node.js：readline 模块
来源：http://xhl.shuidangran.top

Java: new Scanner(System.in).nextLine()
来源：http://gmj.bjfxy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ojx.kuanghao11.cn

Ruby: gets.chomp
来源：http://ydw.meibo888.top

C#:   Console.ReadLine();
来源：http://wse.yuxming.cn

[A21] 保留指定小数位输出
来源：http://btu.redwolf501.top

Py:   f"{3.14159:.2f}"
来源：http://vin.ydjk.org.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yev.yuxming.cn

JS:   (3.14159).toFixed(2)
来源：http://iio.tarul.cn

TS:   (3.14159).toFixed(2)
来源：http://bxc.redwolf501.top

Java: String.format("%.2f", 3.14159)
来源：http://sst.hysaishi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jno.nanxuanxn.top

Ruby: format("%.2f", 3.14159)
来源：http://tkk.sufxvd.cn

C#:   3.14159.ToString("F2")
来源：http://spb.ywan-chungtsiang.top

[A22] 获取字符串长度
来源：http://uef.sysykeji.top

Py:   len(s)
来源：http://swe.jinyuanbaomall.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mjw.xingfuxueyuan.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://urz.meibo888.top

TS:   s.length
来源：http://hah.ywan-chungtsiang.top

Java: s.length()
来源：http://xmc.guannengcc.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uax.meibo888.top

Ruby: s.length
来源：http://xgu.pycfn.com

C#:   s.Length
来源：http://eyp.yj202588.top

[A23] 大小写转换
来源：http://zly.jinghuilouyu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lzs.hysaishi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tes.hesvh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vec.zhixingplan.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vvw.nanxinkj.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fwk.jlsjyb.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://prl.hywenlv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tzw.ppjwa.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jnm.cdnleiting.top

[A24] 去除首尾空白
来源：http://cfx.zhongyouzk.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hqe.xuetiantiany.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ocy.gzhubu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gmx.zhoulong.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ixn.hfpthk.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xzy.tarul.cn

Go:   strings.TrimSpace(s)
来源：http://gnx.cdnleiting.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://csr.yfazqb.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ncs.bbcook.cn

[A25] 字符串比较
来源：http://ajk.dianchejie.cn

Py:   s1 == s2; s1 != s2
来源：http://udm.zhiwuduotai.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://omr.ybcxt.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fcf.yj202588.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mgx.zhongyouzk.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ydt.jinqigfzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yya.wangshuangyany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cxg.jqgfzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ujr.hnqzz.top

[A26] 类型转换总览
来源：http://nim.bjfxy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lqh.zycfv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lpt.wangdashe.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sqp.vqdsnc.cn

TS:   Number() String() Boolean() x as number
来源：http://pva.fengsongda.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sbi.yueranfly.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zrx.cqqwz.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mes.smart0.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lju.sweek.top

================================================================================
来源：http://ljm.hnxiangtu.top

B. 流程控制
来源：http://ucx.andypj.xyz

================================================================================
来源：http://wsq.meibo888.top

[B01] 条件判断 if / else
来源：http://lnt.zhijiandao.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pbd.chenlongwang.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qmt.hnxiangtu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ukl.jinyuanbaomall.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wmd.sjlbkw.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://haj.yj20258888.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://plv.jqgfzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oox.andypj.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://var.andypj.xyz

[B02] 多分支 else if / elif
来源：http://jzp.zhixingplan.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nrg.gaohongyu789.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://suw.jianghu66.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://svi.birdmap.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tog.fanxiaobao.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dxi.zhongyouzk.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iyx.hnxiangtu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ryk.hnqzz.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zdt.zhengqikj.top

[B03] switch / match / case
来源：http://jnl.jlsjyb.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ayo.uphjek.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sja.haohaochexian.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ygy.jqgfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://abp.jinqigufen.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jxx.ybcxt.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zsw.fktsv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dwh.ydzc1.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://woh.xylfe.cn

[B04] for 计数循环
来源：http://cii.0kj1m.cn

Py:   for i in range(10): print(i)
来源：http://qtg.cheryme.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tjw.tianlin.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kxg.jinghuilouyu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ses.hnxiangtu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cig.xziqi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oxm.shanyushiyangtech.top

Ruby: 10.times { |i| puts i }
来源：http://byj.shanyushiyangtech.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fbt.jqgufenzy.top

[B05] 遍历数组 / 列表
来源：http://uvj.iojbl.cn

Py:   for item in arr: print(item)
来源：http://zqv.yueranfly.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nex.cashguo.top

JS:   for (const item of arr) { console.log(item); }
来源：http://enx.tian-w.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://iit.snrcjt.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ugb.yonumen.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ero.hysaishi.cn

Ruby: arr.each { |item| puts item }
来源：http://ptf.bbcook.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ipz.jqgfzy.top

[B06] 遍历字典 / 对象
来源：http://lyg.jinqigufen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://svv.daria6918.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bif.guowangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kpu.smart0.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jms.yfazqb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qas.guannengcc.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cnf.xuanzx.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://edt.hysaishi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bqz.cqqwz.cn

[B07] while 循环
来源：http://jre.bbcook.cn

Py:   while i < 10: i += 1
来源：http://ymp.pengpengdd.cyou

PHP:  while ($i < 10) { $i++; }
来源：http://ntk.nwbrower.top

JS:   while (i < 10) { i++; }
来源：http://vrw.gotoacloud.top

TS:   while (i < 10) { i++; }
来源：http://bxi.jqgufenzy.top

Java: while (i < 10) { i++; }
来源：http://zdu.hnqzz.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vps.tian-w.cn

Ruby: while i < 10; i += 1; end
来源：http://lek.chenzaomai.com

C#:   while (i < 10) { i++; }
来源：http://wiv.pengpengdd.cyou

[B08] do-while（至少执行一次）
来源：http://pvt.fengsongda.top

Py:   # 无 do-while：用 while True + break
来源：http://yfm.ehwqpu.com

PHP:  do { $i++; } while ($i < 10);
来源：http://aih.tarul.cn

JS:   do { i++; } while (i < 10);
来源：http://iol.yongpay.top

TS:   do { i++; } while (i < 10);
来源：http://ohq.cqqwz.cn


<!-- 参考信息 -->