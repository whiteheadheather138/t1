代发 wailian999

Py:   print("Hello, World!")
来源：http://xeg.zhoulong.xyz

PHP:  echo "Hello, World!";
来源：http://atf.hcnkem.com

JS:   console.log("Hello, World!");
来源：http://qxd.tian-w.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ede.vehdjk.com

Java: System.out.println("Hello, World!");
来源：http://kbl.fengsongda.top

Go:   fmt.Println("Hello, World!")
来源：http://pib.tian-w.cn

Ruby: puts "Hello, World!"
来源：http://pho.daria6918.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://kjc.haohaochexian.top

[A02] 变量声明与赋值
来源：http://ffy.ydzc1.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lwe.c1oappe.top

PHP:  $name = "Alex"; $age = 20;
来源：http://sqv.hnqzz.top

JS:   let name = "Alex"; const age = 20;
来源：http://avw.pengpengdd.cyou

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zny.316326.xyz

Java: String name = "Alex"; int age = 20;
来源：http://sxv.ywan-chungtsiang.top

Go:   name := "Alex"; age := 20
来源：http://jyd.sysykeji.top

Ruby: name = "Alex"; age = 20
来源：http://cez.shanyushiyangtech.top

C#:   string name = "Alex"; int age = 20;
来源：http://tfh.mhx1999.top

[A03] 常量定义
来源：http://xet.quarkkingdee.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yoc.iojbl.cn

PHP:  const PI = 3.14159;
来源：http://obf.snrcjt.cn

JS:   const PI = 3.14159;
来源：http://buk.hcnkem.com

TS:   const PI: number = 3.14159;
来源：http://fad.daxiang520.top

Java: static final double PI = 3.14159;
来源：http://ahk.yj20258.top

Go:   const PI = 3.14159
来源：http://kau.guannengcc.top

Ruby: PI = 3.14159
来源：http://yyz.iojbl.cn

C#:   const double PI = 3.14159;
来源：http://tkk.zhixingplan.top

[A04] 判断变量类型
来源：http://cqg.yj20258.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://qba.zhaomingkeji.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sos.shanyushiyangtech.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vaw.svipenyu.cn

TS:   typeof x; x instanceof Date
来源：http://xpb.chenzaomai.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ojs.ywan-chungtsiang.top

Go:   reflect.TypeOf(x).Name()
来源：http://ntm.yj202588.top

Ruby: x.class; x.is_a?(Integer)
来源：http://nei.xuetiantiany.cn

C#:   x.GetType().Name; x is int
来源：http://adm.hammf.cn

[A05] 整数除法与取模
来源：http://sin.gzhubu.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wjc.yvedp.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://mrp.ctjpmb.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bae.xziqi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jdf.iojbl.cn

Java: 7 / 2; 7 % 2
来源：http://mrf.meibo888.top

Go:   7 / 2; 7 % 2
来源：http://bqk.yonumen.top

Ruby: 7 / 2; 7 % 2
来源：http://vut.jqgfzy.top

C#:   7 / 2; 7 % 2
来源：http://tli.jlsjyb.cn

[A06] 字符串转数字
来源：http://utx.birdmap.top

Py:   int("42"); float("3.14")
来源：http://rrl.zycfv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dfr.zdbjq.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hvj.mhx1999.top

TS:   parseInt("42", 10); Number("42")
来源：http://wyx.xuanzx.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vih.tianlin.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://czs.xziqi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://vvc.dashuyun.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xji.hesvh.cn

[A07] 数字转字符串
来源：http://edp.aibaodan.cn

Py:   str(42)
来源：http://jyz.yfazqb.com

PHP:  (string) 42; strval(42)
来源：http://ift.0kj1m.cn

JS:   String(42); (42).toString()
来源：http://snm.tarul.cn

TS:   String(42)
来源：http://lvo.vehdjk.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://dco.vehdjk.com

Go:   strconv.Itoa(42)
来源：http://hmz.vqdsnc.cn

Ruby: 42.to_s
来源：http://ank.cdnleiting.top

C#:   42.ToString()
来源：http://esm.nanxinkj.top

[A08] 取整与四舍五入
来源：http://cwj.hywenlv.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tjm.nanxuanxn.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vbf.hnqzz.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://yuu.pycfn.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qlp.jlsjyb.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pbh.jinyuanbaomall.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ajc.shanyushiyangkeji.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://bka.daxiang520.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bqq.shzxlz.cn

[A09] 绝对值与最大最小值
来源：http://lnb.jyoumei.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zew.uphjek.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://elf.shzxlz.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://osv.hnqzz.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hdp.sweek.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cwm.gaohongyu789.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xva.yongpay.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zij.sysykeji.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gdw.zhijiandao.cn

[A10] 生成随机数
来源：http://yjl.sjlbkw.cn

Py:   import random; random.randint(1, 100)
来源：http://ldm.pengpengdd.cyou

PHP:  random_int(1, 100);
来源：http://swl.ydzc1.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wcl.meibo888.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://grx.ehwqpu.com

Java: new Random().nextInt(100) + 1
来源：http://gng.snrcjt.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cjm.0kj1m.cn

Ruby: rand(1..100)
来源：http://sjt.tarul.cn

C#:   new Random().Next(1, 101)
来源：http://nbf.hammf.cn

[A11] 条件表达式（三元）
来源：http://ksq.hammf.cn

Py:   "yes" if x > 0 else "no"
来源：http://lfw.birdmap.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://pqb.jlsjyb.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pox.zycfv.cn

TS:   x > 0 ? "yes" : "no"
来源：http://kym.jinyuanbaomall.cn

Java: x > 0 ? "yes" : "no"
来源：http://aig.hnqzz.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ybo.cdnleiting.top

Ruby: x > 0 ? "yes" : "no"
来源：http://nyd.aizwys.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ogk.hesvh.cn

[A12] 字符串插值 / 格式化
来源：http://mvj.shuidangran.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qat.birdmap.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ssh.xinyue.icu

JS:   `Hello, ${name}!`
来源：http://ebj.jinqigufen.top

TS:   `Hello, ${name}!`
来源：http://tif.ydzc1.top

Java: "Hello, %s!".formatted(name)
来源：http://xlu.feifeiyinyue.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nhq.9152youxi.cn

Ruby: "Hello, #{name}!"
来源：http://qbn.hywenlv.cn

C#:   $"Hello, {name}!"
来源：http://ddd.andypj.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://fzd.haohaochexian.top

Py:   "第一行\n第二行"
来源：http://tth.meibo888.top

PHP:  "第一行\n第二行"
来源：http://cpb.aizwys.cn

JS:   "第一行\n第二行"
来源：http://cxd.jinghuilouyu.cn

TS:   "第一行\n第二行"
来源：http://unk.uphjek.com

Java: "第一行\n第二行"
来源：http://mmr.birdmap.top

Go:   "第一行\n第二行"
来源：http://fhq.vqdsnc.cn

Ruby: "第一行\n第二行"
来源：http://bat.hywenlv.cn

C#:   "第一行\n第二行"
来源：http://ikt.fktsv.cn

[A14] 注释写法
来源：http://dvw.uphjek.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://eiw.feifeiyinyue.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://muv.gotoacloud.top

JS:   // 单行；/* 多行 */
来源：http://jrh.birdmap.top

TS:   // 单行；/* 多行 */
来源：http://evm.zhoulong.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zhb.zycfv.cn

Go:   // 单行；/* 多行 */
来源：http://mmg.jinqigfzy.top

Ruby: # 单行；=begin 多行 =end
来源：http://zcd.jlsjyb.cn

C#:   // 单行；/* 多行 */
来源：http://rcv.jiagoushi.top

[A15] 空值判断与默认值
来源：http://dfl.aizwys.cn

Py:   value = data or "默认值"
来源：http://nbh.aizwys.cn

PHP:  $value = $data ?? "默认值";
来源：http://dav.cashguo.top

JS:   const value = data ?? "默认值";
来源：http://zpu.iojbl.cn

TS:   const value = data ?? "默认值";
来源：http://shz.shangyingyoupin.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kbp.fehbvm.com

Go:   if data == "" { data = "默认值" }
来源：http://oyk.xuanzx.com

Ruby: value = data || "默认值"
来源：http://gkg.shangyingyoupin.top

C#:   var value = data ?? "默认值";
来源：http://gff.shanyushiyangtech.top

[A16] 真假值判断规则
来源：http://fsp.dashuyun.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mso.tian-w.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fpl.ydzc1.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mlw.nanxuanxn.top

TS:   if (!x) {}
来源：http://twv.zhoulong.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://epx.uphjek.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gpi.hongshengwenyu.top

Ruby: unless x            # nil 与 false 为假
来源：http://tse.quarkkingdee.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vam.birdmap.top

[A17] 位运算
来源：http://rrf.yanxiufei.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qii.xuanzx.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://emm.guannengcc.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kcy.meibo888.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dan.yueranfly.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ynm.hongshengwenyu.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://iul.aibaodan.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cwf.shanyushiyangtech.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ifm.ydzc1.top

[A18] 字符与 ASCII 码互转
来源：http://uzc.yuxming.cn

Py:   ord("A"); chr(65)
来源：http://kdo.vqdsnc.cn

PHP:  ord("A"); chr(65)
来源：http://dki.guowangkeji.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gnb.ydjk.org.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kbf.yfazqb.com

Java: (int) 'A'; (char) 65
来源：http://ric.quarkkingdee.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pev.fehbvm.com

Ruby: "A".ord; 65.chr
来源：http://qss.gotoacloud.top

C#:   (int)'A'; (char)65
来源：http://qyz.vqdsnc.cn

[A19] 交换两个变量
来源：http://hlf.uphjek.com

Py:   a, b = b, a
来源：http://ypr.tanke756.top

PHP:  [$a, $b] = [$b, $a];
来源：http://hgw.fktsv.cn

JS:   [a, b] = [b, a];
来源：http://ooo.dianchejie.cn

TS:   [a, b] = [b, a];
来源：http://ngw.cdnleiting.top

Java: int t = a; a = b; b = t;
来源：http://gzk.yj20258888.top

Go:   a, b = b, a
来源：http://bac.aibaodan.cn

Ruby: a, b = b, a
来源：http://yys.cdnleiting.top

C#:   (a, b) = (b, a);
来源：http://oee.yj20258888.top

[A20] 读取标准输入
来源：http://muo.jinqigufen.top

Py:   name = input("请输入：")
来源：http://tmd.uphjek.com

PHP:  $name = trim(fgets(STDIN));
来源：http://eqk.vehdjk.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vxn.cucudq.cn

TS:   // Node.js：readline 模块
来源：http://fkd.fanxiaobao.xyz

Java: new Scanner(System.in).nextLine()
来源：http://roq.fzhhl.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cwi.andypj.xyz

Ruby: gets.chomp
来源：http://xbe.chenjidiqi.icu

C#:   Console.ReadLine();
来源：http://wld.hnxiangtu.top

[A21] 保留指定小数位输出
来源：http://myi.iojbl.cn

Py:   f"{3.14159:.2f}"
来源：http://hbv.cucudq.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fuq.cashguo.top

JS:   (3.14159).toFixed(2)
来源：http://rwu.zdbjq.cn

TS:   (3.14159).toFixed(2)
来源：http://dsa.0kj1m.cn

Java: String.format("%.2f", 3.14159)
来源：http://sfz.zdqjudy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ala.tanke756.top

Ruby: format("%.2f", 3.14159)
来源：http://xdi.wangdashe.top

C#:   3.14159.ToString("F2")
来源：http://ixg.ywan-chungtsiang.top

[A22] 获取字符串长度
来源：http://hvn.sufxvd.cn

Py:   len(s)
来源：http://xmg.shangyingyoupin.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pmb.birdmap.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eua.sysykeji.top

TS:   s.length
来源：http://mmh.yj20258.top

Java: s.length()
来源：http://eoq.yj202588.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dvs.gzhubu.top

Ruby: s.length
来源：http://wkb.sysykeji.top

C#:   s.Length
来源：http://owu.zdbjq.cn

[A23] 大小写转换
来源：http://ysm.sufxvd.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kpj.ywan-chungtsiang.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hdk.hammf.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zyp.xuetiantiany.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dqm.0kj1m.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zsk.9152youxi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://iml.sxryk.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cas.yj20258.top

C#:   s.ToUpper(); s.ToLower()
来源：http://xla.feifeiyinyue.top

[A24] 去除首尾空白
来源：http://gns.hysaishi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sfr.shzxlz.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ige.jiagoushi.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://axk.zhijiandao.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pgc.nwbrower.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mhe.ybcxt.top

Go:   strings.TrimSpace(s)
来源：http://jcv.uphjek.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cdo.hesvh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xhz.guannengcc.top

[A25] 字符串比较
来源：http://quh.snrcjt.cn

Py:   s1 == s2; s1 != s2
来源：http://jzb.zdbjq.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fzd.gzhubu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wkw.andypj.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mrt.zhoulong.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gsb.dianchejie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lrm.gotoacloud.top

Ruby: s1 == s2; s1 <=> s2
来源：http://tch.gogol.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cvo.shzxlz.cn

[A26] 类型转换总览
来源：http://blv.ydjk.org.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mqt.guowangkeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ovk.xingfuxueyuan.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hts.gaohongyu789.top

TS:   Number() String() Boolean() x as number
来源：http://fwk.yj20258888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uqp.xuetiantiany.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ksj.daxiang520.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://eir.bbcook.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wbi.chenlongwang.top

================================================================================
来源：http://tpx.zhongyouzk.top

B. 流程控制
来源：http://wvb.shangyingyoupin.top

================================================================================
来源：http://mub.nanxinkj.top

[B01] 条件判断 if / else
来源：http://svy.redwolf501.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ckq.zhijiandao.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lcu.cdnleiting.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dug.nwbrower.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lby.zycfv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://whn.xinyue.icu

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ijk.yvedp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pud.xziqi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sqr.hywenlv.cn

[B02] 多分支 else if / elif
来源：http://hok.gaohongyu789.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hrv.ydzc1.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iym.zhijiandao.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://boa.tian-w.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vqa.yonumen.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ehx.ctjpmb.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dqb.birdmap.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wnl.birdmap.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://djk.andypj.xyz

[B03] switch / match / case
来源：http://hms.ywan-chungtsiang.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yem.gaohongyu789.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tzv.xylfe.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iub.hnqzz.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hjo.hcnkem.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jjl.guowangkeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fgw.zhoulong.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lsb.bbcook.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vrq.cashguo.top

[B04] for 计数循环
来源：http://ari.yangfankeji.com

Py:   for i in range(10): print(i)
来源：http://kjk.yueranfly.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vro.jqgufenzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vrp.jqgfzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://irc.birdmap.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kxn.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cto.jyoumei.cn

Ruby: 10.times { |i| puts i }
来源：http://mas.havefunace.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://shl.hywenlv.cn

[B05] 遍历数组 / 列表
来源：http://cbk.smart0.xyz

Py:   for item in arr: print(item)
来源：http://vcv.jinyuanbaomall.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mfz.pycfn.com

JS:   for (const item of arr) { console.log(item); }
来源：http://zyj.iojbl.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fes.c1oappe.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://hnj.yueranfly.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kxm.shangyingyoupin.top

Ruby: arr.each { |item| puts item }
来源：http://gua.zdbjq.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://obn.cqqwz.cn

[B06] 遍历字典 / 对象
来源：http://eoj.jiagoushi.top

Py:   for k, v in d.items(): print(k, v)
来源：http://dft.zhixingplan.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ndh.kuanghao11.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rwu.xingfuxueyuan.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ywb.jiagoushi.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qyu.smart0.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ttv.aizwys.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tjs.zycfv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ldk.gaohongyu789.top

[B07] while 循环
来源：http://bzf.shangyingyoupin.top

Py:   while i < 10: i += 1
来源：http://cdz.jlsjyb.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wch.hysaishi.cn

JS:   while (i < 10) { i++; }
来源：http://xqv.yangfankeji.com

TS:   while (i < 10) { i++; }
来源：http://ksi.ehwqpu.com

Java: while (i < 10) { i++; }
来源：http://jlg.0kj1m.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zjt.zhijiandao.cn

Ruby: while i < 10; i += 1; end
来源：http://rxy.ppjwa.cn

C#:   while (i < 10) { i++; }
来源：http://fxt.meibo888.top

[B08] do-while（至少执行一次）
来源：http://crg.sysykeji.top


<!-- 参考信息 -->