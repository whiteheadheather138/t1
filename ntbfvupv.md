代发 wailian999

Py:   print("Hello, World!")
来源：http://sps.9152youxi.cn

PHP:  echo "Hello, World!";
来源：http://yli.xylfe.cn

JS:   console.log("Hello, World!");
来源：http://hiz.ctjpmb.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fik.mhx1999.top

Java: System.out.println("Hello, World!");
来源：http://akn.jqgufenzy.top

Go:   fmt.Println("Hello, World!")
来源：http://lyz.kuanghao11.cn

Ruby: puts "Hello, World!"
来源：http://xml.jyoumei.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ltr.epnwcf.com

[A02] 变量声明与赋值
来源：http://ysn.yanxiufei.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://sux.xylfe.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://nmt.cucudq.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hbp.zhengqikj.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fyj.epnwcf.com

Java: String name = "Alex"; int age = 20;
来源：http://swk.yongpay.top

Go:   name := "Alex"; age := 20
来源：http://gvp.shuidangran.top

Ruby: name = "Alex"; age = 20
来源：http://wdb.nwbrower.top

C#:   string name = "Alex"; int age = 20;
来源：http://svl.bjfxy.top

[A03] 常量定义
来源：http://oum.epnwcf.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://owp.yj20258.top

PHP:  const PI = 3.14159;
来源：http://gui.chenjidiqi.icu

JS:   const PI = 3.14159;
来源：http://dzd.yongpay.top

TS:   const PI: number = 3.14159;
来源：http://dna.xuetiantiany.cn

Java: static final double PI = 3.14159;
来源：http://gju.dianchejie.cn

Go:   const PI = 3.14159
来源：http://xjh.316326.xyz

Ruby: PI = 3.14159
来源：http://rea.daxiang520.top

C#:   const double PI = 3.14159;
来源：http://yze.sufxvd.cn

[A04] 判断变量类型
来源：http://pxw.wangdashe.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://vqw.yfazqb.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pxy.shzxlz.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gif.nanxuanxn.top

TS:   typeof x; x instanceof Date
来源：http://zjl.shangyingyoupin.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qxl.ehwqpu.com

Go:   reflect.TypeOf(x).Name()
来源：http://vuk.yj20258.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ekl.ydzc1.top

C#:   x.GetType().Name; x is int
来源：http://ojt.shanyushiyangtech.top

[A05] 整数除法与取模
来源：http://npu.hesvh.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kvw.fehbvm.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://sbd.gogol.net.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wjn.chenlongwang.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pcr.havefunace.top

Java: 7 / 2; 7 % 2
来源：http://hfg.hongshengwenyu.top

Go:   7 / 2; 7 % 2
来源：http://wca.yvedp.cn

Ruby: 7 / 2; 7 % 2
来源：http://chi.ydjk.org.cn

C#:   7 / 2; 7 % 2
来源：http://aoc.aizwys.cn

[A06] 字符串转数字
来源：http://buy.52xcode.cn

Py:   int("42"); float("3.14")
来源：http://rhw.yj20258.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://brr.zdbjq.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tqs.chenlongwang.top

TS:   parseInt("42", 10); Number("42")
来源：http://eko.zhijiandao.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mwi.epnwcf.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tmh.bjfxy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ete.xuetiantiany.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kjw.xuetiantiany.cn

[A07] 数字转字符串
来源：http://yxz.dashuyun.cn

Py:   str(42)
来源：http://onh.cucudq.cn

PHP:  (string) 42; strval(42)
来源：http://gqr.vehdjk.com

JS:   String(42); (42).toString()
来源：http://lpl.chenjidiqi.icu

TS:   String(42)
来源：http://ipz.yfazqb.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://jiu.jinyuanbaomall.cn

Go:   strconv.Itoa(42)
来源：http://wvx.yvedp.cn

Ruby: 42.to_s
来源：http://pcd.havefunace.top

C#:   42.ToString()
来源：http://ygn.fktsv.cn

[A08] 取整与四舍五入
来源：http://dir.dashuyun.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dzd.cucudq.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fcr.ppjwa.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://igg.cashguo.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yup.daxiang520.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lcs.zhoulong.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kxt.hongshengwenyu.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://cse.bjfxy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qyf.aibaodan.cn

[A09] 绝对值与最大最小值
来源：http://xue.jianghu66.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hcj.cashguo.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hfm.hammf.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jfr.aizwys.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fpm.zhengqikj.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zfo.zhaomingkeji.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://exm.tanke756.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zmv.yueranfly.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ram.sjlbkw.cn

[A10] 生成随机数
来源：http://euw.ywan-chungtsiang.top

Py:   import random; random.randint(1, 100)
来源：http://yla.wangdashe.top

PHP:  random_int(1, 100);
来源：http://itw.c1oappe.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://arb.wangdashe.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vtt.gzhubu.top

Java: new Random().nextInt(100) + 1
来源：http://cxc.jinqigfzy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://iyn.tarul.cn

Ruby: rand(1..100)
来源：http://ewt.haohaochexian.top

C#:   new Random().Next(1, 101)
来源：http://yib.zdbjq.cn

[A11] 条件表达式（三元）
来源：http://qpy.ybcxt.top

Py:   "yes" if x > 0 else "no"
来源：http://ajb.0kj1m.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://oiq.cucudq.cn

JS:   x > 0 ? "yes" : "no"
来源：http://tps.yfazqb.com

TS:   x > 0 ? "yes" : "no"
来源：http://brc.hnxiangtu.top

Java: x > 0 ? "yes" : "no"
来源：http://jmz.ehwqpu.com

Go:   // 无三元运算符，需用 if 语句
来源：http://qwa.fehbvm.com

Ruby: x > 0 ? "yes" : "no"
来源：http://llg.hysaishi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rvy.feifeiyinyue.top

[A12] 字符串插值 / 格式化
来源：http://xon.yonumen.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lwd.shanyushiyangtech.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zxl.sjlbkw.cn

JS:   `Hello, ${name}!`
来源：http://bod.redwolf501.top

TS:   `Hello, ${name}!`
来源：http://gls.0kj1m.cn

Java: "Hello, %s!".formatted(name)
来源：http://igz.zhaomingkeji.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://arn.shangyingyoupin.top

Ruby: "Hello, #{name}!"
来源：http://glt.yuxming.cn

C#:   $"Hello, {name}!"
来源：http://ady.bbcook.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zdt.sweek.top

Py:   "第一行\n第二行"
来源：http://jvh.cucudq.cn

PHP:  "第一行\n第二行"
来源：http://cla.gotoacloud.top

JS:   "第一行\n第二行"
来源：http://obh.bjfxy.top

TS:   "第一行\n第二行"
来源：http://yfd.zhijiandao.cn

Java: "第一行\n第二行"
来源：http://scg.aizwys.cn

Go:   "第一行\n第二行"
来源：http://dea.0kj1m.cn

Ruby: "第一行\n第二行"
来源：http://avm.tian-w.cn

C#:   "第一行\n第二行"
来源：http://wsq.yvedp.cn

[A14] 注释写法
来源：http://sry.tanke756.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://itg.cheryme.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://knx.0kj1m.cn

JS:   // 单行；/* 多行 */
来源：http://wjz.316326.xyz

TS:   // 单行；/* 多行 */
来源：http://wec.ppjwa.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://esq.chenjidiqi.icu

Go:   // 单行；/* 多行 */
来源：http://ahc.chenlongwang.top

Ruby: # 单行；=begin 多行 =end
来源：http://uyy.wangshuangyany.cn

C#:   // 单行；/* 多行 */
来源：http://ltf.zdbjq.cn

[A15] 空值判断与默认值
来源：http://nse.ydzc1.top

Py:   value = data or "默认值"
来源：http://icn.daxiang520.top

PHP:  $value = $data ?? "默认值";
来源：http://twd.zhaomingkeji.xyz

JS:   const value = data ?? "默认值";
来源：http://pdx.jianghu66.top

TS:   const value = data ?? "默认值";
来源：http://jyi.ywan-chungtsiang.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hwe.sysykeji.top

Go:   if data == "" { data = "默认值" }
来源：http://vnc.ctjpmb.com

Ruby: value = data || "默认值"
来源：http://ecx.cqqwz.cn

C#:   var value = data ?? "默认值";
来源：http://kns.gotoacloud.top

[A16] 真假值判断规则
来源：http://yxt.cqqwz.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://trw.jinqigfzy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vqg.hnqzz.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://brw.wangshuangyany.cn

TS:   if (!x) {}
来源：http://bya.yfazqb.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zfs.shangyingyoupin.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ddq.jinyuanbaomall.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bsl.xylfe.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jjk.316326.xyz

[A17] 位运算
来源：http://dnl.fzhhl.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xwl.yueranfly.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zas.jianghu66.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mbz.nanxinkj.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nea.xziqi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kzq.hnqzz.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yfc.sxryk.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fzo.kuanghao11.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wmn.sxryk.cn

[A18] 字符与 ASCII 码互转
来源：http://sgd.cqqwz.cn

Py:   ord("A"); chr(65)
来源：http://tub.9152youxi.cn

PHP:  ord("A"); chr(65)
来源：http://scd.cheryme.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uqv.smart0.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bfo.yueranfly.top

Java: (int) 'A'; (char) 65
来源：http://kjv.chenzaomai.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vrw.yongpay.top

Ruby: "A".ord; 65.chr
来源：http://ovu.nanxuanxn.top

C#:   (int)'A'; (char)65
来源：http://xlf.wangshuangyany.cn

[A19] 交换两个变量
来源：http://kgs.aizwys.cn

Py:   a, b = b, a
来源：http://csw.wangdashe.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ors.gotoacloud.top

JS:   [a, b] = [b, a];
来源：http://gjz.hnxiangtu.top

TS:   [a, b] = [b, a];
来源：http://ape.zhijiandao.cn

Java: int t = a; a = b; b = t;
来源：http://ncb.birdmap.top

Go:   a, b = b, a
来源：http://zzj.zhoulong.xyz

Ruby: a, b = b, a
来源：http://nhj.kuanghao11.cn

C#:   (a, b) = (b, a);
来源：http://ezn.zycfv.cn

[A20] 读取标准输入
来源：http://jxp.ctjpmb.com

Py:   name = input("请输入：")
来源：http://uly.birdmap.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ani.52xcode.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jsa.sysykeji.top

TS:   // Node.js：readline 模块
来源：http://pml.jianghu66.top

Java: new Scanner(System.in).nextLine()
来源：http://oco.gzhubu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ygf.ppjwa.cn

Ruby: gets.chomp
来源：http://aca.0kj1m.cn

C#:   Console.ReadLine();
来源：http://psu.fzhhl.top

[A21] 保留指定小数位输出
来源：http://lai.chenlongwang.top

Py:   f"{3.14159:.2f}"
来源：http://nhk.gzhubu.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ccy.mhx1999.top

JS:   (3.14159).toFixed(2)
来源：http://szs.sxryk.cn

TS:   (3.14159).toFixed(2)
来源：http://mdn.yanxiufei.cn

Java: String.format("%.2f", 3.14159)
来源：http://tln.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eys.hnxiangtu.top

Ruby: format("%.2f", 3.14159)
来源：http://cwu.havefunace.top

C#:   3.14159.ToString("F2")
来源：http://yda.c1oappe.top

[A22] 获取字符串长度
来源：http://hvl.jqgfzy.top

Py:   len(s)
来源：http://hsl.yj20258.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lzg.dianchejie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zbj.meibo888.top

TS:   s.length
来源：http://tdb.jinqigufen.top

Java: s.length()
来源：http://dat.yuxming.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xmo.xinyue.icu

Ruby: s.length
来源：http://rbu.ivvv.top

C#:   s.Length
来源：http://tks.zhiwuduotai.top

[A23] 大小写转换
来源：http://vza.quarkkingdee.top

Py:   s.upper(); s.lower(); s.title()
来源：http://vcf.shanyushiyangtech.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fro.aibaodan.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pcl.fktsv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mjx.tanke756.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wdl.mhx1999.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://azy.jqgufenzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nac.daxiang520.top

C#:   s.ToUpper(); s.ToLower()
来源：http://hog.shuidangran.top

[A24] 去除首尾空白
来源：http://ums.jinqigfzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fwz.redwolf501.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hyr.zhengqikj.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://obg.guowangkeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uup.ywan-chungtsiang.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://elr.52xcode.cn

Go:   strings.TrimSpace(s)
来源：http://mqr.zhengqikj.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mjw.shuidangran.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ggg.tianlin.xyz

[A25] 字符串比较
来源：http://hdh.sufxvd.cn

Py:   s1 == s2; s1 != s2
来源：http://cyt.kuanghao11.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://boe.jiagoushi.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jja.wangdashe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ric.sufxvd.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://csj.yj20258.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qmd.yonumen.top

Ruby: s1 == s2; s1 <=> s2
来源：http://gpt.cqqwz.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qxr.xziqi.cn

[A26] 类型转换总览
来源：http://ywa.yonumen.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dte.hesvh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hmi.guannengcc.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jrh.daria6918.cn

TS:   Number() String() Boolean() x as number
来源：http://wez.jqgufenzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://aql.ivvv.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kjx.fktsv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wnm.zhiwuduotai.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rav.zhengqikj.top

================================================================================
来源：http://qdx.xylfe.cn

B. 流程控制
来源：http://klf.xingfuxueyuan.xyz

================================================================================
来源：http://khd.ybcxt.top

[B01] 条件判断 if / else
来源：http://qfr.bjfxy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://nol.hysaishi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wdf.jinghuilouyu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ujs.xuetiantiany.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lqj.jinyuanbaomall.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://elo.kuanghao11.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wqx.yvedp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zug.sysykeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vwr.fengsongda.top

[B02] 多分支 else if / elif
来源：http://gom.cdnleiting.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ozx.ppjwa.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jxy.hcnkem.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ydc.0kj1m.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dfc.chenjidiqi.icu

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ijl.jqgfzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vzd.fengsongda.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hfd.chenlongwang.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dgv.havefunace.top

[B03] switch / match / case
来源：http://kjn.uphjek.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nes.316326.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cbv.mhx1999.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://faf.gaohongyu789.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blh.shanyushiyangtech.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jhx.tanke756.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wfl.hongshengwenyu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yjz.guowangkeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qqn.yonumen.top

[B04] for 计数循环
来源：http://ahx.9152youxi.cn

Py:   for i in range(10): print(i)
来源：http://wbv.gogol.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ldc.daria6918.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kad.daxiang520.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yuk.ivvv.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zwv.gzhubu.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rde.jinqigfzy.top

Ruby: 10.times { |i| puts i }
来源：http://bvc.fehbvm.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://oag.iojbl.cn

[B05] 遍历数组 / 列表
来源：http://flj.jiagoushi.top

Py:   for item in arr: print(item)
来源：http://qjs.hfpthk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://usk.feifeiyinyue.top

JS:   for (const item of arr) { console.log(item); }
来源：http://kkb.shzxlz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ctv.yangfankeji.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://hpi.pycfn.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://udi.nwbrower.top

Ruby: arr.each { |item| puts item }
来源：http://uci.zhixingplan.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fax.jinqigufen.top

[B06] 遍历字典 / 对象
来源：http://hio.cheryme.top

Py:   for k, v in d.items(): print(k, v)
来源：http://dwm.xinyue.icu

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wwl.jiagoushi.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cco.aizwys.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nyo.jinyuanbaomall.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uxv.0kj1m.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wad.redwolf501.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yvx.52xcode.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lyl.jqgfzy.top

[B07] while 循环
来源：http://xds.hnqzz.top

Py:   while i < 10: i += 1
来源：http://lsk.jqgufenzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://iba.dianchejie.cn

JS:   while (i < 10) { i++; }
来源：http://lim.ydzc1.top

TS:   while (i < 10) { i++; }
来源：http://hlo.wangshuangyany.cn

Java: while (i < 10) { i++; }
来源：http://tar.gzhubu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uoh.shzxlz.cn

Ruby: while i < 10; i += 1; end
来源：http://rsa.yangfankeji.com

C#:   while (i < 10) { i++; }
来源：http://lch.ivvv.top

[B08] do-while（至少执行一次）
来源：http://gjj.fzhhl.top


<!-- 参考信息 -->