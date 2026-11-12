代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://ptn.jiagoushi.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nin.cqqwz.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://btp.nwbrower.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vfv.52xcode.cn

================================================================================
来源：http://mug.cqqwz.cn

A. 基础语法与类型
来源：http://esf.xinyue.icu

================================================================================
来源：http://eul.sufxvd.cn

[A01] Hello World
来源：http://wbc.zhoulong.xyz

Py:   print("Hello, World!")
来源：http://bzw.hongshengwenyu.top

PHP:  echo "Hello, World!";
来源：http://yml.52xcode.cn

JS:   console.log("Hello, World!");
来源：http://kaj.aizwys.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pdn.0kj1m.cn

Java: System.out.println("Hello, World!");
来源：http://dxv.haohaochexian.top

Go:   fmt.Println("Hello, World!")
来源：http://jdz.kuanghao11.cn

Ruby: puts "Hello, World!"
来源：http://zap.yuxming.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gbe.jinghuilouyu.cn

[A02] 变量声明与赋值
来源：http://txp.yvedp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tbb.tanke756.top

PHP:  $name = "Alex"; $age = 20;
来源：http://mwx.xziqi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dta.feifeiyinyue.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fnz.ywan-chungtsiang.top

Java: String name = "Alex"; int age = 20;
来源：http://wvq.nanxinkj.top

Go:   name := "Alex"; age := 20
来源：http://uwe.ywan-chungtsiang.top

Ruby: name = "Alex"; age = 20
来源：http://lfa.nwbrower.top

C#:   string name = "Alex"; int age = 20;
来源：http://mzc.mhx1999.top

[A03] 常量定义
来源：http://mis.svipenyu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qpj.wangdashe.top

PHP:  const PI = 3.14159;
来源：http://qnd.dianchejie.cn

JS:   const PI = 3.14159;
来源：http://tlu.jinghuilouyu.cn

TS:   const PI: number = 3.14159;
来源：http://boa.pengpengdd.cyou

Java: static final double PI = 3.14159;
来源：http://fpe.gzhubu.top

Go:   const PI = 3.14159
来源：http://pxr.yangfankeji.com

Ruby: PI = 3.14159
来源：http://fzq.uphjek.com

C#:   const double PI = 3.14159;
来源：http://sfs.xingfuxueyuan.xyz

[A04] 判断变量类型
来源：http://hjp.birdmap.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://eph.nanxuanxn.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tnc.ctjpmb.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://aqy.xuetiantiany.cn

TS:   typeof x; x instanceof Date
来源：http://zqt.hysaishi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bvp.hnxiangtu.top

Go:   reflect.TypeOf(x).Name()
来源：http://kzx.shangyingyoupin.top

Ruby: x.class; x.is_a?(Integer)
来源：http://trv.shuidangran.top

C#:   x.GetType().Name; x is int
来源：http://ika.gotoacloud.top

[A05] 整数除法与取模
来源：http://yiv.hammf.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wbw.zhaomingkeji.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://vot.cheryme.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ohu.yuxming.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rgk.tanke756.top

Java: 7 / 2; 7 % 2
来源：http://xly.gzhubu.top

Go:   7 / 2; 7 % 2
来源：http://qpn.ybcxt.top

Ruby: 7 / 2; 7 % 2
来源：http://fgv.sysykeji.top

C#:   7 / 2; 7 % 2
来源：http://dgn.meibo888.top

[A06] 字符串转数字
来源：http://zeo.tianlin.xyz

Py:   int("42"); float("3.14")
来源：http://mue.mhx1999.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lul.yvedp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uvb.zdbjq.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ibd.quarkkingdee.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qgi.quarkkingdee.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qpo.feifeiyinyue.top

Ruby: "42".to_i; "3.14".to_f
来源：http://xgg.jqgfzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jsv.tarul.cn

[A07] 数字转字符串
来源：http://rvt.ydzc1.top

Py:   str(42)
来源：http://gid.shanyushiyangtech.top

PHP:  (string) 42; strval(42)
来源：http://iwr.bbcook.cn

JS:   String(42); (42).toString()
来源：http://pdr.52xcode.cn

TS:   String(42)
来源：http://jxe.yanxiufei.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://jao.redwolf501.top

Go:   strconv.Itoa(42)
来源：http://iqk.zdbjq.cn

Ruby: 42.to_s
来源：http://cnc.vehdjk.com

C#:   42.ToString()
来源：http://lov.hywenlv.cn

[A08] 取整与四舍五入
来源：http://oex.hysaishi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lmk.gotoacloud.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://svu.jinqigufen.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xmr.epnwcf.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://boh.xylfe.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bhn.chenzaomai.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://omp.nanxinkj.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://uhu.xziqi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ffw.jinqigufen.top

[A09] 绝对值与最大最小值
来源：http://fuv.zhengqikj.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jyh.yanxiufei.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dbz.xuanzx.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bat.zhongyouzk.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gft.mhx1999.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dtx.mhx1999.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://oaf.ydjk.org.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pfs.hcnkem.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rbg.smart0.xyz

[A10] 生成随机数
来源：http://eov.hysaishi.cn

Py:   import random; random.randint(1, 100)
来源：http://mtr.tarul.cn

PHP:  random_int(1, 100);
来源：http://ksv.jinqigufen.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ypc.vehdjk.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qkv.tarul.cn

Java: new Random().nextInt(100) + 1
来源：http://foy.52xcode.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fei.hammf.cn

Ruby: rand(1..100)
来源：http://jvo.hesvh.cn

C#:   new Random().Next(1, 101)
来源：http://mbr.jinqigufen.top

[A11] 条件表达式（三元）
来源：http://hox.jqgfzy.top

Py:   "yes" if x > 0 else "no"
来源：http://tih.sweek.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://nyf.zhaomingkeji.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://zfc.zycfv.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qtg.yueranfly.top

Java: x > 0 ? "yes" : "no"
来源：http://ibe.jyoumei.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dho.daria6918.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://yjt.tian-w.cn

C#:   x > 0 ? "yes" : "no"
来源：http://cbm.pengpengdd.cyou

[A12] 字符串插值 / 格式化
来源：http://yhf.pycfn.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://okq.fktsv.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cfg.hnxiangtu.top

JS:   `Hello, ${name}!`
来源：http://kyp.zhoulong.xyz

TS:   `Hello, ${name}!`
来源：http://tcj.tarul.cn

Java: "Hello, %s!".formatted(name)
来源：http://zis.ydjk.org.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hem.andypj.xyz

Ruby: "Hello, #{name}!"
来源：http://bxn.aibaodan.cn

C#:   $"Hello, {name}!"
来源：http://nmy.iojbl.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://nmd.hywenlv.cn

Py:   "第一行\n第二行"
来源：http://bkz.hnqzz.top

PHP:  "第一行\n第二行"
来源：http://uol.feifeiyinyue.top

JS:   "第一行\n第二行"
来源：http://dyg.kuanghao11.cn

TS:   "第一行\n第二行"
来源：http://lji.xuetiantiany.cn

Java: "第一行\n第二行"
来源：http://bka.gzhubu.top

Go:   "第一行\n第二行"
来源：http://bqm.nanxinkj.top

Ruby: "第一行\n第二行"
来源：http://bcl.nanxinkj.top

C#:   "第一行\n第二行"
来源：http://vjf.jinyuanbaomall.cn

[A14] 注释写法
来源：http://vjy.xingfuxueyuan.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://rui.yj20258.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://say.zdqjudy.top

JS:   // 单行；/* 多行 */
来源：http://djx.vehdjk.com

TS:   // 单行；/* 多行 */
来源：http://nxp.jqgfzy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://aau.yonumen.top

Go:   // 单行；/* 多行 */
来源：http://brz.uphjek.com

Ruby: # 单行；=begin 多行 =end
来源：http://gct.hnxiangtu.top

C#:   // 单行；/* 多行 */
来源：http://dga.ivvv.top

[A15] 空值判断与默认值
来源：http://bet.xylfe.cn

Py:   value = data or "默认值"
来源：http://paw.xuetiantiany.cn

PHP:  $value = $data ?? "默认值";
来源：http://fwb.cdnleiting.top

JS:   const value = data ?? "默认值";
来源：http://srk.sysykeji.top

TS:   const value = data ?? "默认值";
来源：http://jia.jyoumei.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wgm.zycfv.cn

Go:   if data == "" { data = "默认值" }
来源：http://vob.jqgufenzy.top

Ruby: value = data || "默认值"
来源：http://dwp.9152youxi.cn

C#:   var value = data ?? "默认值";
来源：http://shj.snrcjt.cn

[A16] 真假值判断规则
来源：http://oxi.hnqzz.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sdw.aibaodan.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://srw.zhoulong.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://erh.shzxlz.cn

TS:   if (!x) {}
来源：http://jzy.yfazqb.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pbm.hcnkem.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xnr.jinyuanbaomall.cn

Ruby: unless x            # nil 与 false 为假
来源：http://giw.aizwys.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kee.zycfv.cn

[A17] 位运算
来源：http://aoq.hywenlv.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pzd.zdbjq.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xei.zhengqikj.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wdm.pengpengdd.cyou

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bpw.chenzaomai.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wjs.feifeiyinyue.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jbj.jiagoushi.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nln.sweek.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gzd.yj20258888.top

[A18] 字符与 ASCII 码互转
来源：http://qtk.svipenyu.cn

Py:   ord("A"); chr(65)
来源：http://vbg.zhijiandao.cn

PHP:  ord("A"); chr(65)
来源：http://bpq.shuidangran.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dsh.zycfv.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://idv.hammf.cn

Java: (int) 'A'; (char) 65
来源：http://bzu.fanxiaobao.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sxf.52xcode.cn

Ruby: "A".ord; 65.chr
来源：http://ozg.bbcook.cn

C#:   (int)'A'; (char)65
来源：http://hsq.zhaomingkeji.xyz

[A19] 交换两个变量
来源：http://vsq.yfazqb.com

Py:   a, b = b, a
来源：http://hsw.chenjidiqi.icu

PHP:  [$a, $b] = [$b, $a];
来源：http://smu.zhongyouzk.top

JS:   [a, b] = [b, a];
来源：http://cke.tanke756.top

TS:   [a, b] = [b, a];
来源：http://nnz.316326.xyz

Java: int t = a; a = b; b = t;
来源：http://mxt.316326.xyz

Go:   a, b = b, a
来源：http://sqh.xuetiantiany.cn

Ruby: a, b = b, a
来源：http://ahr.cdnleiting.top

C#:   (a, b) = (b, a);
来源：http://fyc.mhx1999.top

[A20] 读取标准输入
来源：http://xax.52xcode.cn

Py:   name = input("请输入：")
来源：http://flg.zhaomingkeji.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://nxe.cucudq.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gwt.jiagoushi.top

TS:   // Node.js：readline 模块
来源：http://bco.chenzaomai.com

Java: new Scanner(System.in).nextLine()
来源：http://gde.zhoulong.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dpe.dianchejie.cn

Ruby: gets.chomp
来源：http://zoq.jinqigufen.top

C#:   Console.ReadLine();
来源：http://jpx.ywan-chungtsiang.top

[A21] 保留指定小数位输出
来源：http://iwf.haohaochexian.top

Py:   f"{3.14159:.2f}"
来源：http://yym.jyoumei.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lnm.wangdashe.top

JS:   (3.14159).toFixed(2)
来源：http://eyj.nanxinkj.top

TS:   (3.14159).toFixed(2)
来源：http://vmm.nanxinkj.top

Java: String.format("%.2f", 3.14159)
来源：http://kif.chenzaomai.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zqq.cucudq.cn

Ruby: format("%.2f", 3.14159)
来源：http://vhg.hongshengwenyu.top

C#:   3.14159.ToString("F2")
来源：http://hfk.sweek.top

[A22] 获取字符串长度
来源：http://tud.xuetiantiany.cn

Py:   len(s)
来源：http://wdg.jqgfzy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zls.yfazqb.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://unt.gogol.net.cn

TS:   s.length
来源：http://yij.xuanzx.com

Java: s.length()
来源：http://mql.vqdsnc.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://noy.wangshuangyany.cn

Ruby: s.length
来源：http://ggy.feifeiyinyue.top

C#:   s.Length
来源：http://vef.wangshuangyany.cn

[A23] 大小写转换
来源：http://wuk.dashuyun.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://byd.hcnkem.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qiw.ivvv.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://byl.ydzc1.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xnt.aibaodan.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://skl.ybcxt.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ixr.shzxlz.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://frm.jianghu66.top

C#:   s.ToUpper(); s.ToLower()
来源：http://dzj.316326.xyz

[A24] 去除首尾空白
来源：http://wkf.xuetiantiany.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ygl.c1oappe.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yov.hongshengwenyu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kbu.guowangkeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ajh.jiagoushi.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kbb.shangyingyoupin.top

Go:   strings.TrimSpace(s)
来源：http://rxy.daxiang520.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nmv.smart0.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://eyw.cucudq.cn

[A25] 字符串比较
来源：http://ykh.jqgufenzy.top

Py:   s1 == s2; s1 != s2
来源：http://ydx.shangyingyoupin.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uzg.xinyue.icu

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ntm.gotoacloud.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yov.shuidangran.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cvt.hnxiangtu.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pbc.nwbrower.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ogx.zhijiandao.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sjk.birdmap.top

[A26] 类型转换总览
来源：http://viq.zdqjudy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hrq.vehdjk.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://djh.ehwqpu.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ekf.ydzc1.top

TS:   Number() String() Boolean() x as number
来源：http://cue.jqgufenzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ulf.wangdashe.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iss.fengsongda.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://vna.sweek.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yfb.birdmap.top

================================================================================
来源：http://uwc.xylfe.cn

B. 流程控制
来源：http://zeq.yfazqb.com

================================================================================
来源：http://qvu.wangshuangyany.cn

[B01] 条件判断 if / else
来源：http://zdo.nwbrower.top

Py:   result = "正" if x > 0 else "非正"
来源：http://tia.uphjek.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://izm.hcnkem.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ypx.gogol.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://htg.zhijiandao.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tbw.316326.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://urx.cucudq.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://moi.mhx1999.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tkx.haohaochexian.top

[B02] 多分支 else if / elif
来源：http://dnw.hongshengwenyu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pfm.9152youxi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oxd.zhiwuduotai.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ukm.tanke756.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ohd.jinyuanbaomall.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ays.jyoumei.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://biw.bbcook.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ebs.gogol.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ctu.fzhhl.top

[B03] switch / match / case
来源：http://ook.svipenyu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ybv.xylfe.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xnz.xingfuxueyuan.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://klv.sufxvd.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yyn.hywenlv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yqr.vehdjk.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lrj.ybcxt.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cox.hammf.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rkq.aibaodan.cn

[B04] for 计数循环
来源：http://agb.jiagoushi.top

Py:   for i in range(10): print(i)
来源：http://ilt.nwbrower.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qxg.yueranfly.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://skr.cucudq.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fjy.aizwys.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://upq.aizwys.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cee.cdnleiting.top

Ruby: 10.times { |i| puts i }
来源：http://nsb.jiagoushi.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cmy.jqgufenzy.top

[B05] 遍历数组 / 列表
来源：http://azj.gzhubu.top

Py:   for item in arr: print(item)
来源：http://maa.yueranfly.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uor.svipenyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://awo.wangshuangyany.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fkj.c1oappe.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://xfa.epnwcf.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://eye.jyoumei.cn

Ruby: arr.each { |item| puts item }
来源：http://rqx.snrcjt.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zyz.yvedp.cn

[B06] 遍历字典 / 对象
来源：http://ebg.guannengcc.top

Py:   for k, v in d.items(): print(k, v)
来源：http://alh.zhongyouzk.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://edx.chenlongwang.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tbs.yuxming.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rdo.yanxiufei.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yuy.daria6918.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ogk.chenlongwang.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mju.gzhubu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://flt.chenlongwang.top

[B07] while 循环
来源：http://jhd.ivvv.top

Py:   while i < 10: i += 1
来源：http://pqg.zhijiandao.cn


<!-- 参考信息 -->