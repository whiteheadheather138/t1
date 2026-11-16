代发 wailian999

================================================================================
来源：http://wuw.zycfv.cn

A. 基础语法与类型
来源：http://sbl.tian-w.cn

================================================================================
来源：http://klr.hammf.cn

[A01] Hello World
来源：http://vrq.snrcjt.cn

Py:   print("Hello, World!")
来源：http://uxy.havefunace.top

PHP:  echo "Hello, World!";
来源：http://ost.zycfv.cn

JS:   console.log("Hello, World!");
来源：http://tnl.tanke756.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://icz.gogol.net.cn

Java: System.out.println("Hello, World!");
来源：http://mit.cheryme.top

Go:   fmt.Println("Hello, World!")
来源：http://kew.shanyushiyangkeji.top

Ruby: puts "Hello, World!"
来源：http://wqy.fzhhl.top

C#:   Console.WriteLine("Hello, World!");
来源：http://rhj.vehdjk.com

[A02] 变量声明与赋值
来源：http://haq.yj20258888.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ksg.yueranfly.top

PHP:  $name = "Alex"; $age = 20;
来源：http://vgv.sufxvd.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tgi.hywenlv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ewz.hfpthk.cn

Java: String name = "Alex"; int age = 20;
来源：http://sst.cqqwz.cn

Go:   name := "Alex"; age := 20
来源：http://ysr.sufxvd.cn

Ruby: name = "Alex"; age = 20
来源：http://aib.yanxiufei.cn

C#:   string name = "Alex"; int age = 20;
来源：http://oip.zhijiandao.cn

[A03] 常量定义
来源：http://dye.zycfv.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xfu.chenzaomai.com

PHP:  const PI = 3.14159;
来源：http://pqz.ctjpmb.com

JS:   const PI = 3.14159;
来源：http://okp.redwolf501.top

TS:   const PI: number = 3.14159;
来源：http://ohx.jiagoushi.top

Java: static final double PI = 3.14159;
来源：http://ihl.xinyue.icu

Go:   const PI = 3.14159
来源：http://seo.c1oappe.top

Ruby: PI = 3.14159
来源：http://rkf.zdqjudy.top

C#:   const double PI = 3.14159;
来源：http://psa.c1oappe.top

[A04] 判断变量类型
来源：http://buf.cdnleiting.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ztp.cheryme.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lbk.yfazqb.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lvl.hesvh.cn

TS:   typeof x; x instanceof Date
来源：http://spp.fehbvm.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ryf.fehbvm.com

Go:   reflect.TypeOf(x).Name()
来源：http://nky.wangshuangyany.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xkn.chenzaomai.com

C#:   x.GetType().Name; x is int
来源：http://rma.cashguo.top

[A05] 整数除法与取模
来源：http://lib.meibo888.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xuq.shangyingyoupin.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://xzp.xuetiantiany.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dbe.jyoumei.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xyv.shangyingyoupin.top

Java: 7 / 2; 7 % 2
来源：http://ddj.bbcook.cn

Go:   7 / 2; 7 % 2
来源：http://etz.pengpengdd.cyou

Ruby: 7 / 2; 7 % 2
来源：http://wyr.xziqi.cn

C#:   7 / 2; 7 % 2
来源：http://wwj.tianlin.xyz

[A06] 字符串转数字
来源：http://ecw.xuetiantiany.cn

Py:   int("42"); float("3.14")
来源：http://kvg.shzxlz.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gem.ywan-chungtsiang.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dmp.nwbrower.top

TS:   parseInt("42", 10); Number("42")
来源：http://sul.gzhubu.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://frs.sjlbkw.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ygy.shangyingyoupin.top

Ruby: "42".to_i; "3.14".to_f
来源：http://uao.gotoacloud.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fda.xinyue.icu

[A07] 数字转字符串
来源：http://fvg.mhx1999.top

Py:   str(42)
来源：http://aua.yj20258888.top

PHP:  (string) 42; strval(42)
来源：http://zxx.sjlbkw.cn

JS:   String(42); (42).toString()
来源：http://fvt.guowangkeji.top

TS:   String(42)
来源：http://lno.zhiwuduotai.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://tct.mhx1999.top

Go:   strconv.Itoa(42)
来源：http://plo.chenjidiqi.icu

Ruby: 42.to_s
来源：http://rig.pengpengdd.cyou

C#:   42.ToString()
来源：http://kxp.xylfe.cn

[A08] 取整与四舍五入
来源：http://lqq.yuanzhike.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bys.gaohongyu789.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rvn.nanxinkj.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ary.hesvh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mab.0kj1m.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dhx.zhiwuduotai.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jpb.chenzaomai.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://mhn.andypj.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pmx.tian-w.cn

[A09] 绝对值与最大最小值
来源：http://iwn.cheryme.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jlw.vqdsnc.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sfu.shzxlz.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ecb.hesvh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://iwx.xuanzx.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://whh.xuetiantiany.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://agv.nanxinkj.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nut.epnwcf.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nph.xuanzx.com

[A10] 生成随机数
来源：http://oqp.havefunace.top

Py:   import random; random.randint(1, 100)
来源：http://boe.jinyuanbaomall.cn

PHP:  random_int(1, 100);
来源：http://udc.shzxlz.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zbj.gaohongyu789.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://spn.daxiang520.top

Java: new Random().nextInt(100) + 1
来源：http://ajb.cdnleiting.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://uyo.ppjwa.cn

Ruby: rand(1..100)
来源：http://bxz.fzhhl.top

C#:   new Random().Next(1, 101)
来源：http://thi.chenlongwang.top

[A11] 条件表达式（三元）
来源：http://fxo.wangshuangyany.cn

Py:   "yes" if x > 0 else "no"
来源：http://bda.hnxiangtu.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://nmf.hnqzz.top

JS:   x > 0 ? "yes" : "no"
来源：http://ypb.zhiwuduotai.top

TS:   x > 0 ? "yes" : "no"
来源：http://jrj.havefunace.top

Java: x > 0 ? "yes" : "no"
来源：http://mcz.daria6918.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://eth.yangfankeji.com

Ruby: x > 0 ? "yes" : "no"
来源：http://ihc.sufxvd.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bbi.yj202588.top

[A12] 字符串插值 / 格式化
来源：http://fnb.chenjidiqi.icu

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://eud.ywan-chungtsiang.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sjz.vehdjk.com

JS:   `Hello, ${name}!`
来源：http://wjv.shanyushiyangtech.top

TS:   `Hello, ${name}!`
来源：http://lnt.zhixingplan.top

Java: "Hello, %s!".formatted(name)
来源：http://mmp.sjlbkw.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://byc.birdmap.top

Ruby: "Hello, #{name}!"
来源：http://joq.0kj1m.cn

C#:   $"Hello, {name}!"
来源：http://lmf.cdnleiting.top

[A13] 多行字符串（练习 \n 转义）
来源：http://giz.nwbrower.top

Py:   "第一行\n第二行"
来源：http://jge.zycfv.cn

PHP:  "第一行\n第二行"
来源：http://wik.zhongyouzk.top

JS:   "第一行\n第二行"
来源：http://gts.sxryk.cn

TS:   "第一行\n第二行"
来源：http://fyf.pycfn.com

Java: "第一行\n第二行"
来源：http://knw.jlsjyb.cn

Go:   "第一行\n第二行"
来源：http://wct.hcnkem.com

Ruby: "第一行\n第二行"
来源：http://akl.chenjidiqi.icu

C#:   "第一行\n第二行"
来源：http://gfh.dianchejie.cn

[A14] 注释写法
来源：http://siu.yvedp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://sjn.yj202588.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://usv.yfazqb.com

JS:   // 单行；/* 多行 */
来源：http://pgk.yonumen.top

TS:   // 单行；/* 多行 */
来源：http://cbc.bbcook.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ssg.xuanzx.com

Go:   // 单行；/* 多行 */
来源：http://jpx.shangyingyoupin.top

Ruby: # 单行；=begin 多行 =end
来源：http://jbc.jinyuanbaomall.cn

C#:   // 单行；/* 多行 */
来源：http://epi.ydjk.org.cn

[A15] 空值判断与默认值
来源：http://bal.aibaodan.cn

Py:   value = data or "默认值"
来源：http://ade.meibo888.top

PHP:  $value = $data ?? "默认值";
来源：http://gmv.fktsv.cn

JS:   const value = data ?? "默认值";
来源：http://wuk.tian-w.cn

TS:   const value = data ?? "默认值";
来源：http://pwi.jyoumei.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jfb.gotoacloud.top

Go:   if data == "" { data = "默认值" }
来源：http://flp.pycfn.com

Ruby: value = data || "默认值"
来源：http://lae.ctjpmb.com

C#:   var value = data ?? "默认值";
来源：http://pgb.zdbjq.cn

[A16] 真假值判断规则
来源：http://whk.tian-w.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cos.zdbjq.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xma.yanxiufei.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mku.wangshuangyany.cn

TS:   if (!x) {}
来源：http://owl.ydzc1.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lzh.chenlongwang.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pza.fehbvm.com

Ruby: unless x            # nil 与 false 为假
来源：http://hmf.wangshuangyany.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cph.zycfv.cn

[A17] 位运算
来源：http://hzi.ivvv.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qkg.pycfn.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bqs.zhiwuduotai.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dra.quarkkingdee.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yxp.yj202588.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ipl.sweek.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://onm.jyoumei.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dyj.nanxinkj.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qse.birdmap.top

[A18] 字符与 ASCII 码互转
来源：http://hkr.xylfe.cn

Py:   ord("A"); chr(65)
来源：http://qnc.9152youxi.cn

PHP:  ord("A"); chr(65)
来源：http://lzc.hesvh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yfa.jianghu66.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qqa.daria6918.cn

Java: (int) 'A'; (char) 65
来源：http://jgq.jinqigfzy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uvy.chenlongwang.top

Ruby: "A".ord; 65.chr
来源：http://vvo.hysaishi.cn

C#:   (int)'A'; (char)65
来源：http://rmc.zdbjq.cn

[A19] 交换两个变量
来源：http://atq.jinyuanbaomall.cn

Py:   a, b = b, a
来源：http://pdn.jyoumei.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://wpl.yuxming.cn

JS:   [a, b] = [b, a];
来源：http://ttf.wangdashe.top

TS:   [a, b] = [b, a];
来源：http://oex.zhiwuduotai.top

Java: int t = a; a = b; b = t;
来源：http://afk.hnqzz.top

Go:   a, b = b, a
来源：http://tef.ppjwa.cn

Ruby: a, b = b, a
来源：http://giw.chenjidiqi.icu

C#:   (a, b) = (b, a);
来源：http://oub.fzhhl.top

[A20] 读取标准输入
来源：http://xdw.daria6918.cn

Py:   name = input("请输入：")
来源：http://zrk.xinyue.icu

PHP:  $name = trim(fgets(STDIN));
来源：http://ioh.zhongyouzk.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://aow.ydzc1.top

TS:   // Node.js：readline 模块
来源：http://rrp.jinqigufen.top

Java: new Scanner(System.in).nextLine()
来源：http://mbn.yj202588.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cak.sjlbkw.cn

Ruby: gets.chomp
来源：http://kfs.ehwqpu.com

C#:   Console.ReadLine();
来源：http://ixm.shuidangran.top

[A21] 保留指定小数位输出
来源：http://gak.jianghu66.top

Py:   f"{3.14159:.2f}"
来源：http://snk.birdmap.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rmt.snrcjt.cn

JS:   (3.14159).toFixed(2)
来源：http://qgp.dashuyun.cn

TS:   (3.14159).toFixed(2)
来源：http://hzs.shanyushiyangkeji.top

Java: String.format("%.2f", 3.14159)
来源：http://edr.aibaodan.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://riq.jinqigufen.top

Ruby: format("%.2f", 3.14159)
来源：http://fwa.sjlbkw.cn

C#:   3.14159.ToString("F2")
来源：http://jcp.shzxlz.cn

[A22] 获取字符串长度
来源：http://xkm.jinyuanbaomall.cn

Py:   len(s)
来源：http://uwr.hysaishi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xni.tianlin.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cgs.meibo888.top

TS:   s.length
来源：http://pcz.0kj1m.cn

Java: s.length()
来源：http://ycs.ctjpmb.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xxf.fzhhl.top

Ruby: s.length
来源：http://wbd.zhengqikj.top

C#:   s.Length
来源：http://cty.zhixingplan.top

[A23] 大小写转换
来源：http://rnr.xziqi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kbb.shzxlz.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vzf.hnqzz.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qfm.ppjwa.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ije.cashguo.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qum.hongshengwenyu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cty.nanxuanxn.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sfe.fzhhl.top

C#:   s.ToUpper(); s.ToLower()
来源：http://bfu.andypj.xyz

[A24] 去除首尾空白
来源：http://nvc.meibo888.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://oxx.gaohongyu789.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jpu.hysaishi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ouz.epnwcf.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fpa.jianghu66.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qat.zdqjudy.top

Go:   strings.TrimSpace(s)
来源：http://gyu.52xcode.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mtk.kuanghao11.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ror.shzxlz.cn

[A25] 字符串比较
来源：http://tmn.chenzaomai.com

Py:   s1 == s2; s1 != s2
来源：http://wbn.quarkkingdee.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://brz.zhongyouzk.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gzy.sweek.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jar.c1oappe.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zoo.andypj.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://esr.cashguo.top

Ruby: s1 == s2; s1 <=> s2
来源：http://jie.ydjk.org.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yhs.gaohongyu789.top

[A26] 类型转换总览
来源：http://wpd.daria6918.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://adn.nwbrower.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mvy.sjlbkw.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lqx.fanxiaobao.xyz

TS:   Number() String() Boolean() x as number
来源：http://ffz.ivvv.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ryc.vehdjk.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oln.gzhubu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://rri.gzhubu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xlh.hesvh.cn

================================================================================
来源：http://yqz.kuanghao11.cn

B. 流程控制
来源：http://ypt.pycfn.com

================================================================================
来源：http://zxd.hnqzz.top

[B01] 条件判断 if / else
来源：http://eca.yangfankeji.com

Py:   result = "正" if x > 0 else "非正"
来源：http://ylj.xziqi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gqg.daxiang520.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qaw.chenjidiqi.icu

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lli.vehdjk.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://wvd.chenjidiqi.icu

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nei.sufxvd.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hmx.zhiwuduotai.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://otq.ppjwa.cn

[B02] 多分支 else if / elif
来源：http://gpm.pengpengdd.cyou

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jcy.aibaodan.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rvq.cucudq.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xaj.vqdsnc.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://naw.cheryme.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qva.zhixingplan.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bgo.chenzaomai.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tum.aibaodan.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wek.sxryk.cn

[B03] switch / match / case
来源：http://pwk.fehbvm.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ifl.meibo888.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mtb.zhoulong.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pvi.yvedp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kix.havefunace.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://toz.birdmap.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://htu.redwolf501.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tna.hywenlv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hxy.yongpay.top

[B04] for 计数循环
来源：http://qna.sxryk.cn

Py:   for i in range(10): print(i)
来源：http://vwi.tarul.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gru.zhixingplan.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kbm.wangdashe.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ofr.hnxiangtu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sjp.0kj1m.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nmv.fanxiaobao.xyz

Ruby: 10.times { |i| puts i }
来源：http://vsu.aibaodan.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bly.pycfn.com

[B05] 遍历数组 / 列表
来源：http://ktw.nwbrower.top

Py:   for item in arr: print(item)
来源：http://ilp.sweek.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rhp.hysaishi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://akk.smart0.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://reb.iojbl.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sko.xylfe.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ykl.nwbrower.top

Ruby: arr.each { |item| puts item }
来源：http://tub.ivvv.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://orn.ctjpmb.com

[B06] 遍历字典 / 对象
来源：http://gzn.daria6918.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ldf.zhoulong.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vet.hcnkem.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xdz.shanyushiyangtech.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zyv.cucudq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kch.cheryme.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vcd.jinyuanbaomall.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vqc.sxryk.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://evc.ppjwa.cn

[B07] while 循环
来源：http://npq.jianghu66.top

Py:   while i < 10: i += 1
来源：http://dux.zhijiandao.cn

PHP:  while ($i < 10) { $i++; }
来源：http://uhv.havefunace.top

JS:   while (i < 10) { i++; }
来源：http://qol.hnqzz.top

TS:   while (i < 10) { i++; }
来源：http://utd.tarul.cn

Java: while (i < 10) { i++; }
来源：http://uvt.yj202588.top


<!-- 参考信息 -->