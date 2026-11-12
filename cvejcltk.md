代发 wailian999

================================================================================
来源：http://ubt.andypj.xyz

A. 基础语法与类型
来源：http://fws.chenjidiqi.icu

================================================================================
来源：http://hcc.tarul.cn

[A01] Hello World
来源：http://zqr.wangshuangyany.cn

Py:   print("Hello, World!")
来源：http://nvb.shuidangran.top

PHP:  echo "Hello, World!";
来源：http://psa.zycfv.cn

JS:   console.log("Hello, World!");
来源：http://wyd.yj202588.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qly.sxryk.cn

Java: System.out.println("Hello, World!");
来源：http://pwm.feifeiyinyue.top

Go:   fmt.Println("Hello, World!")
来源：http://uch.tianlin.xyz

Ruby: puts "Hello, World!"
来源：http://wrb.dashuyun.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wud.bjfxy.top

[A02] 变量声明与赋值
来源：http://jwd.vqdsnc.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dyn.kuanghao11.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://nfd.birdmap.top

JS:   let name = "Alex"; const age = 20;
来源：http://wpg.fktsv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zxn.shanyushiyangkeji.top

Java: String name = "Alex"; int age = 20;
来源：http://rzv.zdbjq.cn

Go:   name := "Alex"; age := 20
来源：http://qsc.cdnleiting.top

Ruby: name = "Alex"; age = 20
来源：http://pru.tanke756.top

C#:   string name = "Alex"; int age = 20;
来源：http://wyd.chenjidiqi.icu

[A03] 常量定义
来源：http://cqz.aibaodan.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rtw.vqdsnc.cn

PHP:  const PI = 3.14159;
来源：http://weo.andypj.xyz

JS:   const PI = 3.14159;
来源：http://chw.hnqzz.top

TS:   const PI: number = 3.14159;
来源：http://uue.ywan-chungtsiang.top

Java: static final double PI = 3.14159;
来源：http://spr.cashguo.top

Go:   const PI = 3.14159
来源：http://wmd.aizwys.cn

Ruby: PI = 3.14159
来源：http://msm.uphjek.com

C#:   const double PI = 3.14159;
来源：http://jsn.havefunace.top

[A04] 判断变量类型
来源：http://pmv.cashguo.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://zuk.epnwcf.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jpq.jlsjyb.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hdf.yangfankeji.com

TS:   typeof x; x instanceof Date
来源：http://gvu.yueranfly.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://eew.sweek.top

Go:   reflect.TypeOf(x).Name()
来源：http://xvq.hcnkem.com

Ruby: x.class; x.is_a?(Integer)
来源：http://wgw.svipenyu.cn

C#:   x.GetType().Name; x is int
来源：http://dma.xuanzx.com

[A05] 整数除法与取模
来源：http://hmn.zhiwuduotai.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lrl.guowangkeji.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://urz.hysaishi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jlj.dianchejie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yhq.yfazqb.com

Java: 7 / 2; 7 % 2
来源：http://ywn.zhiwuduotai.top

Go:   7 / 2; 7 % 2
来源：http://aru.fengsongda.top

Ruby: 7 / 2; 7 % 2
来源：http://gob.shanyushiyangtech.top

C#:   7 / 2; 7 % 2
来源：http://jgu.yfazqb.com

[A06] 字符串转数字
来源：http://pgr.zdbjq.cn

Py:   int("42"); float("3.14")
来源：http://uhb.9152youxi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dte.dashuyun.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cdw.nanxinkj.top

TS:   parseInt("42", 10); Number("42")
来源：http://mlv.yfazqb.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dee.zhaomingkeji.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fia.iojbl.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://jza.jqgufenzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fgd.sxryk.cn

[A07] 数字转字符串
来源：http://rec.ydjk.org.cn

Py:   str(42)
来源：http://qnq.tarul.cn

PHP:  (string) 42; strval(42)
来源：http://cza.tianlin.xyz

JS:   String(42); (42).toString()
来源：http://elu.hywenlv.cn

TS:   String(42)
来源：http://iqa.kuanghao11.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://jsb.pengpengdd.cyou

Go:   strconv.Itoa(42)
来源：http://arr.hongshengwenyu.top

Ruby: 42.to_s
来源：http://pkv.ydjk.org.cn

C#:   42.ToString()
来源：http://shs.bbcook.cn

[A08] 取整与四舍五入
来源：http://mom.hnqzz.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bxw.zhaomingkeji.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bjo.yj202588.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hwk.jqgfzy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rkj.yanxiufei.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rmy.snrcjt.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ckn.xuanzx.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://fmv.yonumen.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://btd.guannengcc.top

[A09] 绝对值与最大最小值
来源：http://oum.shangyingyoupin.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bcr.sjlbkw.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ryx.ywan-chungtsiang.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fht.dashuyun.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wac.svipenyu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://swp.jyoumei.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lij.yueranfly.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gtn.chenjidiqi.icu

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ygv.iojbl.cn

[A10] 生成随机数
来源：http://ooj.fanxiaobao.xyz

Py:   import random; random.randint(1, 100)
来源：http://seg.hesvh.cn

PHP:  random_int(1, 100);
来源：http://ynu.mhx1999.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ics.chenlongwang.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bcs.tanke756.top

Java: new Random().nextInt(100) + 1
来源：http://esj.316326.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bkh.hywenlv.cn

Ruby: rand(1..100)
来源：http://llx.fengsongda.top

C#:   new Random().Next(1, 101)
来源：http://dwa.hfpthk.cn

[A11] 条件表达式（三元）
来源：http://ebu.jlsjyb.cn

Py:   "yes" if x > 0 else "no"
来源：http://faf.chenlongwang.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://bpa.hysaishi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://uzg.zhaomingkeji.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://noo.bbcook.cn

Java: x > 0 ? "yes" : "no"
来源：http://ked.andypj.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://orl.gaohongyu789.top

Ruby: x > 0 ? "yes" : "no"
来源：http://lxy.meibo888.top

C#:   x > 0 ? "yes" : "no"
来源：http://eqs.cheryme.top

[A12] 字符串插值 / 格式化
来源：http://uze.zycfv.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bwj.guowangkeji.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://biv.daria6918.cn

JS:   `Hello, ${name}!`
来源：http://muu.xinyue.icu

TS:   `Hello, ${name}!`
来源：http://zby.jinyuanbaomall.cn

Java: "Hello, %s!".formatted(name)
来源：http://ktv.cucudq.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ddw.jinqigfzy.top

Ruby: "Hello, #{name}!"
来源：http://fwj.chenzaomai.com

C#:   $"Hello, {name}!"
来源：http://pkc.xingfuxueyuan.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://nap.shzxlz.cn

Py:   "第一行\n第二行"
来源：http://pra.ywan-chungtsiang.top

PHP:  "第一行\n第二行"
来源：http://pdi.yuxming.cn

JS:   "第一行\n第二行"
来源：http://lhz.wangdashe.top

TS:   "第一行\n第二行"
来源：http://gno.jinghuilouyu.cn

Java: "第一行\n第二行"
来源：http://sjp.yuanzhike.top

Go:   "第一行\n第二行"
来源：http://yzj.fengsongda.top

Ruby: "第一行\n第二行"
来源：http://oul.yangfankeji.com

C#:   "第一行\n第二行"
来源：http://xnm.zhiwuduotai.top

[A14] 注释写法
来源：http://gpn.svipenyu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://alw.feifeiyinyue.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://dgm.bjfxy.top

JS:   // 单行；/* 多行 */
来源：http://hvx.gzhubu.top

TS:   // 单行；/* 多行 */
来源：http://xsv.gotoacloud.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://upn.bbcook.cn

Go:   // 单行；/* 多行 */
来源：http://rbx.sysykeji.top

Ruby: # 单行；=begin 多行 =end
来源：http://hdj.guowangkeji.top

C#:   // 单行；/* 多行 */
来源：http://ppn.xuanzx.com

[A15] 空值判断与默认值
来源：http://ndl.jqgfzy.top

Py:   value = data or "默认值"
来源：http://fbm.tianlin.xyz

PHP:  $value = $data ?? "默认值";
来源：http://zfx.yangfankeji.com

JS:   const value = data ?? "默认值";
来源：http://xyd.fanxiaobao.xyz

TS:   const value = data ?? "默认值";
来源：http://zpi.hcnkem.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://snq.epnwcf.com

Go:   if data == "" { data = "默认值" }
来源：http://iqu.zhoulong.xyz

Ruby: value = data || "默认值"
来源：http://dek.fzhhl.top

C#:   var value = data ?? "默认值";
来源：http://plh.kuanghao11.cn

[A16] 真假值判断规则
来源：http://rdl.wangshuangyany.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://uep.zhongyouzk.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://uif.mhx1999.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tft.zdbjq.cn

TS:   if (!x) {}
来源：http://wko.jinqigfzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ypk.zhoulong.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rxn.havefunace.top

Ruby: unless x            # nil 与 false 为假
来源：http://kxv.c1oappe.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nfs.ydjk.org.cn

[A17] 位运算
来源：http://jlh.cheryme.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vrh.xinyue.icu

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hcr.ywan-chungtsiang.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kdn.xuanzx.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vkt.vehdjk.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lao.pycfn.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://otu.yanxiufei.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ihu.316326.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fdq.cucudq.cn

[A18] 字符与 ASCII 码互转
来源：http://pcr.bbcook.cn

Py:   ord("A"); chr(65)
来源：http://kpi.yj20258888.top

PHP:  ord("A"); chr(65)
来源：http://ztq.9152youxi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mur.gotoacloud.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fbk.meibo888.top

Java: (int) 'A'; (char) 65
来源：http://sym.0kj1m.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fsh.svipenyu.cn

Ruby: "A".ord; 65.chr
来源：http://ojj.shangyingyoupin.top

C#:   (int)'A'; (char)65
来源：http://ntk.shanyushiyangkeji.top

[A19] 交换两个变量
来源：http://rrb.hesvh.cn

Py:   a, b = b, a
来源：http://kxj.tarul.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hva.chenlongwang.top

JS:   [a, b] = [b, a];
来源：http://ile.chenlongwang.top

TS:   [a, b] = [b, a];
来源：http://dqf.hammf.cn

Java: int t = a; a = b; b = t;
来源：http://dow.shzxlz.cn

Go:   a, b = b, a
来源：http://zth.sjlbkw.cn

Ruby: a, b = b, a
来源：http://bcy.yonumen.top

C#:   (a, b) = (b, a);
来源：http://axf.zycfv.cn

[A20] 读取标准输入
来源：http://uzm.pengpengdd.cyou

Py:   name = input("请输入：")
来源：http://wvo.zycfv.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dkw.snrcjt.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dfl.feifeiyinyue.top

TS:   // Node.js：readline 模块
来源：http://dfm.birdmap.top

Java: new Scanner(System.in).nextLine()
来源：http://rtv.yvedp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hag.gaohongyu789.top

Ruby: gets.chomp
来源：http://moc.xingfuxueyuan.xyz

C#:   Console.ReadLine();
来源：http://vnt.shanyushiyangtech.top

[A21] 保留指定小数位输出
来源：http://kro.gzhubu.top

Py:   f"{3.14159:.2f}"
来源：http://ger.haohaochexian.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dgu.0kj1m.cn

JS:   (3.14159).toFixed(2)
来源：http://hjo.gotoacloud.top

TS:   (3.14159).toFixed(2)
来源：http://mwg.yfazqb.com

Java: String.format("%.2f", 3.14159)
来源：http://msz.zhiwuduotai.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://suw.vqdsnc.cn

Ruby: format("%.2f", 3.14159)
来源：http://tfu.quarkkingdee.top

C#:   3.14159.ToString("F2")
来源：http://aeu.ppjwa.cn

[A22] 获取字符串长度
来源：http://yxp.mhx1999.top

Py:   len(s)
来源：http://icx.wangdashe.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hvg.daria6918.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pzg.gotoacloud.top

TS:   s.length
来源：http://drv.epnwcf.com

Java: s.length()
来源：http://ynm.xingfuxueyuan.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cvl.yj20258888.top

Ruby: s.length
来源：http://rzp.zhoulong.xyz

C#:   s.Length
来源：http://hgu.birdmap.top

[A23] 大小写转换
来源：http://fru.bbcook.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dtd.shanyushiyangkeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://llq.jinghuilouyu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rwb.xinyue.icu

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://diz.hnxiangtu.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hjx.jiagoushi.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hcm.bjfxy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ytl.fktsv.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://igy.hfpthk.cn

[A24] 去除首尾空白
来源：http://cwb.jqgufenzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pcq.xuanzx.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://slr.jyoumei.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bti.tian-w.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wmv.shzxlz.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jvx.quarkkingdee.top

Go:   strings.TrimSpace(s)
来源：http://vbm.xingfuxueyuan.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pcj.hongshengwenyu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ocf.jyoumei.cn

[A25] 字符串比较
来源：http://fig.wangshuangyany.cn

Py:   s1 == s2; s1 != s2
来源：http://hgl.havefunace.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ltz.tarul.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rvu.uphjek.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rxf.0kj1m.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tzv.ivvv.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://psm.hcnkem.com

Ruby: s1 == s2; s1 <=> s2
来源：http://jvs.chenjidiqi.icu

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mdd.yangfankeji.com

[A26] 类型转换总览
来源：http://jcd.jqgfzy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mov.gogol.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tcb.ydjk.org.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wwj.wangshuangyany.cn

TS:   Number() String() Boolean() x as number
来源：http://bdf.yfazqb.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ovd.jinqigufen.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xzp.shzxlz.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hhk.dianchejie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hfy.guowangkeji.top

================================================================================
来源：http://jpn.jianghu66.top

B. 流程控制
来源：http://asu.wangdashe.top

================================================================================
来源：http://ykf.dianchejie.cn

[B01] 条件判断 if / else
来源：http://ins.shangyingyoupin.top

Py:   result = "正" if x > 0 else "非正"
来源：http://qlv.wangshuangyany.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ghd.cqqwz.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jpb.jiagoushi.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jfa.shanyushiyangkeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://lty.hywenlv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xsj.wangdashe.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mut.wangshuangyany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rwu.yuanzhike.top

[B02] 多分支 else if / elif
来源：http://rri.sufxvd.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ozo.c1oappe.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ybh.ctjpmb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ths.zhengqikj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ksz.sufxvd.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rao.iojbl.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://era.zycfv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://alb.xylfe.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iae.cashguo.top

[B03] switch / match / case
来源：http://jbx.vehdjk.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rcn.redwolf501.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dkm.xingfuxueyuan.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iqh.birdmap.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ppn.snrcjt.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://szb.ctjpmb.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fyv.bbcook.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lih.zhiwuduotai.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pmp.andypj.xyz

[B04] for 计数循环
来源：http://cxp.yangfankeji.com

Py:   for i in range(10): print(i)
来源：http://jqf.zhengqikj.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wjf.snrcjt.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jcq.zhijiandao.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yes.tanke756.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jlr.hnqzz.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kma.jlsjyb.cn

Ruby: 10.times { |i| puts i }
来源：http://hie.yj20258888.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uuq.chenjidiqi.icu

[B05] 遍历数组 / 列表
来源：http://vul.hnxiangtu.top

Py:   for item in arr: print(item)
来源：http://yaw.sxryk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xwt.redwolf501.top

JS:   for (const item of arr) { console.log(item); }
来源：http://rmb.yonumen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://klu.cucudq.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jkf.yanxiufei.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wrh.ywan-chungtsiang.top

Ruby: arr.each { |item| puts item }
来源：http://hdd.shangyingyoupin.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ahr.cheryme.top

[B06] 遍历字典 / 对象
来源：http://ciq.52xcode.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hyn.xuetiantiany.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mra.gotoacloud.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hzf.gogol.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kek.yangfankeji.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://eie.tarul.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vxu.gotoacloud.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wwq.pengpengdd.cyou

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vkv.0kj1m.cn

[B07] while 循环
来源：http://wht.jqgufenzy.top

Py:   while i < 10: i += 1
来源：http://ril.epnwcf.com

PHP:  while ($i < 10) { $i++; }
来源：http://aeq.guannengcc.top

JS:   while (i < 10) { i++; }
来源：http://yhn.0kj1m.cn

TS:   while (i < 10) { i++; }
来源：http://xig.fktsv.cn

Java: while (i < 10) { i++; }
来源：http://lip.ybcxt.top


<!-- 参考信息 -->