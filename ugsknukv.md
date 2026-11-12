代发 wailian999

[A02] 变量声明与赋值
来源：http://jun.svipenyu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dmn.yj20258.top

PHP:  $name = "Alex"; $age = 20;
来源：http://gta.wangshuangyany.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wnb.zhoulong.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hrw.chenjidiqi.icu

Java: String name = "Alex"; int age = 20;
来源：http://qlj.chenlongwang.top

Go:   name := "Alex"; age := 20
来源：http://mpn.xylfe.cn

Ruby: name = "Alex"; age = 20
来源：http://ope.xuetiantiany.cn

C#:   string name = "Alex"; int age = 20;
来源：http://eri.pycfn.com

[A03] 常量定义
来源：http://dzg.hysaishi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://iba.yanxiufei.cn

PHP:  const PI = 3.14159;
来源：http://hdt.nwbrower.top

JS:   const PI = 3.14159;
来源：http://iel.zhijiandao.cn

TS:   const PI: number = 3.14159;
来源：http://tny.tanke756.top

Java: static final double PI = 3.14159;
来源：http://kay.hongshengwenyu.top

Go:   const PI = 3.14159
来源：http://axw.jiagoushi.top

Ruby: PI = 3.14159
来源：http://xfx.hysaishi.cn

C#:   const double PI = 3.14159;
来源：http://qdl.shzxlz.cn

[A04] 判断变量类型
来源：http://ifk.yanxiufei.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://yfy.yongpay.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zxn.jinghuilouyu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://osw.hesvh.cn

TS:   typeof x; x instanceof Date
来源：http://pyz.hongshengwenyu.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jur.jlsjyb.cn

Go:   reflect.TypeOf(x).Name()
来源：http://cen.ydzc1.top

Ruby: x.class; x.is_a?(Integer)
来源：http://wjb.fehbvm.com

C#:   x.GetType().Name; x is int
来源：http://szp.yanxiufei.cn

[A05] 整数除法与取模
来源：http://qmd.dianchejie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wlv.hysaishi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://uyg.fzhhl.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fdd.birdmap.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xci.chenlongwang.top

Java: 7 / 2; 7 % 2
来源：http://wnk.tanke756.top

Go:   7 / 2; 7 % 2
来源：http://jak.zhengqikj.top

Ruby: 7 / 2; 7 % 2
来源：http://bbx.gotoacloud.top

C#:   7 / 2; 7 % 2
来源：http://und.hfpthk.cn

[A06] 字符串转数字
来源：http://ubi.ctjpmb.com

Py:   int("42"); float("3.14")
来源：http://qmp.svipenyu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ntn.kuanghao11.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tqa.fktsv.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qya.yueranfly.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://sxw.yuxming.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wbe.fanxiaobao.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://elm.snrcjt.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mmu.sxryk.cn

[A07] 数字转字符串
来源：http://xxu.shanyushiyangtech.top

Py:   str(42)
来源：http://uxw.uphjek.com

PHP:  (string) 42; strval(42)
来源：http://yiz.yuanzhike.top

JS:   String(42); (42).toString()
来源：http://azm.nanxuanxn.top

TS:   String(42)
来源：http://ctq.xuetiantiany.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ypv.meibo888.top

Go:   strconv.Itoa(42)
来源：http://khp.xylfe.cn

Ruby: 42.to_s
来源：http://rrk.epnwcf.com

C#:   42.ToString()
来源：http://wwc.fengsongda.top

[A08] 取整与四舍五入
来源：http://vrf.xingfuxueyuan.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xot.ydzc1.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ehz.zhengqikj.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tnk.cheryme.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rsj.sufxvd.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fqe.hysaishi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zqa.meibo888.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ygs.zhijiandao.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hjk.aibaodan.cn

[A09] 绝对值与最大最小值
来源：http://gld.shzxlz.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pnj.zycfv.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yzq.zhiwuduotai.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://boh.zhixingplan.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://owi.pengpengdd.cyou

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mfx.c1oappe.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://igm.yuxming.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qcx.gogol.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ign.jqgufenzy.top

[A10] 生成随机数
来源：http://pax.shuidangran.top

Py:   import random; random.randint(1, 100)
来源：http://kpi.shanyushiyangkeji.top

PHP:  random_int(1, 100);
来源：http://jfg.andypj.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://amx.shanyushiyangkeji.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nlq.sxryk.cn

Java: new Random().nextInt(100) + 1
来源：http://vku.ctjpmb.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jwv.gzhubu.top

Ruby: rand(1..100)
来源：http://okb.jiagoushi.top

C#:   new Random().Next(1, 101)
来源：http://fni.zycfv.cn

[A11] 条件表达式（三元）
来源：http://qbl.ppjwa.cn

Py:   "yes" if x > 0 else "no"
来源：http://jyv.zhoulong.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://ysh.yj202588.top

JS:   x > 0 ? "yes" : "no"
来源：http://rha.jianghu66.top

TS:   x > 0 ? "yes" : "no"
来源：http://wcz.gotoacloud.top

Java: x > 0 ? "yes" : "no"
来源：http://pmr.havefunace.top

Go:   // 无三元运算符，需用 if 语句
来源：http://zad.xziqi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://neh.cheryme.top

C#:   x > 0 ? "yes" : "no"
来源：http://hxb.jinqigfzy.top

[A12] 字符串插值 / 格式化
来源：http://spu.cdnleiting.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://agh.52xcode.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://onz.nwbrower.top

JS:   `Hello, ${name}!`
来源：http://ctu.jlsjyb.cn

TS:   `Hello, ${name}!`
来源：http://tbj.fehbvm.com

Java: "Hello, %s!".formatted(name)
来源：http://zss.fanxiaobao.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mnc.daxiang520.top

Ruby: "Hello, #{name}!"
来源：http://brv.gogol.net.cn

C#:   $"Hello, {name}!"
来源：http://swr.yfazqb.com

[A13] 多行字符串（练习 \n 转义）
来源：http://rym.guowangkeji.top

Py:   "第一行\n第二行"
来源：http://eyl.yvedp.cn

PHP:  "第一行\n第二行"
来源：http://mhm.chenlongwang.top

JS:   "第一行\n第二行"
来源：http://nih.bbcook.cn

TS:   "第一行\n第二行"
来源：http://doe.kuanghao11.cn

Java: "第一行\n第二行"
来源：http://cqs.smart0.xyz

Go:   "第一行\n第二行"
来源：http://gif.birdmap.top

Ruby: "第一行\n第二行"
来源：http://vbo.ydzc1.top

C#:   "第一行\n第二行"
来源：http://kee.shangyingyoupin.top

[A14] 注释写法
来源：http://rsg.chenlongwang.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://jpv.yangfankeji.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://hof.wangdashe.top

JS:   // 单行；/* 多行 */
来源：http://aca.jianghu66.top

TS:   // 单行；/* 多行 */
来源：http://uzs.redwolf501.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qgx.shanyushiyangkeji.top

Go:   // 单行；/* 多行 */
来源：http://ocs.316326.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://tmn.ydjk.org.cn

C#:   // 单行；/* 多行 */
来源：http://kbe.guannengcc.top

[A15] 空值判断与默认值
来源：http://ier.aibaodan.cn

Py:   value = data or "默认值"
来源：http://pks.zycfv.cn

PHP:  $value = $data ?? "默认值";
来源：http://zex.chenlongwang.top

JS:   const value = data ?? "默认值";
来源：http://mjz.feifeiyinyue.top

TS:   const value = data ?? "默认值";
来源：http://fcp.guannengcc.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dkt.bbcook.cn

Go:   if data == "" { data = "默认值" }
来源：http://rnk.kuanghao11.cn

Ruby: value = data || "默认值"
来源：http://jlj.iojbl.cn

C#:   var value = data ?? "默认值";
来源：http://dtu.epnwcf.com

[A16] 真假值判断规则
来源：http://fmu.zhaomingkeji.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ezb.wangdashe.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://myv.bbcook.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rht.jqgfzy.top

TS:   if (!x) {}
来源：http://lul.fehbvm.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xif.aizwys.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sdt.jinqigufen.top

Ruby: unless x            # nil 与 false 为假
来源：http://dup.fzhhl.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rim.nanxinkj.top

[A17] 位运算
来源：http://rnn.sysykeji.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dgo.ywan-chungtsiang.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bte.feifeiyinyue.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lle.ehwqpu.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://iaq.gogol.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zmw.shanyushiyangkeji.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dse.0kj1m.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oco.birdmap.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nef.gzhubu.top

[A18] 字符与 ASCII 码互转
来源：http://egb.mhx1999.top

Py:   ord("A"); chr(65)
来源：http://nqq.zhongyouzk.top

PHP:  ord("A"); chr(65)
来源：http://vqb.0kj1m.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xch.jinghuilouyu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fnc.hnxiangtu.top

Java: (int) 'A'; (char) 65
来源：http://coq.guannengcc.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://esv.cucudq.cn

Ruby: "A".ord; 65.chr
来源：http://uac.shuidangran.top

C#:   (int)'A'; (char)65
来源：http://txf.xylfe.cn

[A19] 交换两个变量
来源：http://khb.xuetiantiany.cn

Py:   a, b = b, a
来源：http://rdg.nanxuanxn.top

PHP:  [$a, $b] = [$b, $a];
来源：http://eir.yfazqb.com

JS:   [a, b] = [b, a];
来源：http://htr.hesvh.cn

TS:   [a, b] = [b, a];
来源：http://ywo.ywan-chungtsiang.top

Java: int t = a; a = b; b = t;
来源：http://kff.yangfankeji.com

Go:   a, b = b, a
来源：http://yhm.jianghu66.top

Ruby: a, b = b, a
来源：http://jmg.zhijiandao.cn

C#:   (a, b) = (b, a);
来源：http://pfv.hysaishi.cn

[A20] 读取标准输入
来源：http://nps.jinqigfzy.top

Py:   name = input("请输入：")
来源：http://bra.xingfuxueyuan.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://val.fanxiaobao.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mlq.shzxlz.cn

TS:   // Node.js：readline 模块
来源：http://aor.gogol.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://tmm.wangshuangyany.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wvd.cheryme.top

Ruby: gets.chomp
来源：http://ihd.zdbjq.cn

C#:   Console.ReadLine();
来源：http://wos.hysaishi.cn

[A21] 保留指定小数位输出
来源：http://aws.hesvh.cn

Py:   f"{3.14159:.2f}"
来源：http://ypa.pycfn.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xvq.xingfuxueyuan.xyz

JS:   (3.14159).toFixed(2)
来源：http://rwv.jinqigufen.top

TS:   (3.14159).toFixed(2)
来源：http://fts.jinyuanbaomall.cn

Java: String.format("%.2f", 3.14159)
来源：http://kyu.hnqzz.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://trx.jinyuanbaomall.cn

Ruby: format("%.2f", 3.14159)
来源：http://ttr.smart0.xyz

C#:   3.14159.ToString("F2")
来源：http://evj.aibaodan.cn

[A22] 获取字符串长度
来源：http://fad.cucudq.cn

Py:   len(s)
来源：http://fzj.bjfxy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://axi.ydjk.org.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tke.birdmap.top

TS:   s.length
来源：http://soa.zycfv.cn

Java: s.length()
来源：http://uzh.yonumen.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ddz.xuanzx.com

Ruby: s.length
来源：http://nze.feifeiyinyue.top

C#:   s.Length
来源：http://iab.bbcook.cn

[A23] 大小写转换
来源：http://dcd.xingfuxueyuan.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://gyk.xylfe.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://beh.yuanzhike.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ylh.316326.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hcr.daria6918.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ami.mhx1999.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gld.jyoumei.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hkl.meibo888.top

C#:   s.ToUpper(); s.ToLower()
来源：http://jth.xinyue.icu

[A24] 去除首尾空白
来源：http://mjw.redwolf501.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zhh.cheryme.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hxc.hnxiangtu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xze.jianghu66.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fis.xingfuxueyuan.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xxz.jinqigufen.top

Go:   strings.TrimSpace(s)
来源：http://rwc.ctjpmb.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sgt.guannengcc.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qln.zycfv.cn

[A25] 字符串比较
来源：http://ktx.yuanzhike.top

Py:   s1 == s2; s1 != s2
来源：http://ayd.jinqigfzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sue.tanke756.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gav.zdqjudy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pij.chenlongwang.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fwo.bbcook.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lhy.xinyue.icu

Ruby: s1 == s2; s1 <=> s2
来源：http://xtb.wangdashe.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yks.xuetiantiany.cn

[A26] 类型转换总览
来源：http://pim.chenjidiqi.icu

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lgg.0kj1m.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xql.shzxlz.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qkt.yvedp.cn

TS:   Number() String() Boolean() x as number
来源：http://rua.zhijiandao.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bij.zycfv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yub.sufxvd.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vhf.daxiang520.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hkk.shuidangran.top

================================================================================
来源：http://jhz.redwolf501.top

B. 流程控制
来源：http://btc.fengsongda.top

================================================================================
来源：http://hti.daxiang520.top

[B01] 条件判断 if / else
来源：http://ewa.sjlbkw.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sdj.yueranfly.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jfv.jyoumei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bwo.zdqjudy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qrk.zhiwuduotai.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ack.feifeiyinyue.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://isa.bbcook.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bjh.yonumen.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://koy.pycfn.com

[B02] 多分支 else if / elif
来源：http://nly.xylfe.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bxp.yonumen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hbc.ctjpmb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ylj.cdnleiting.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mnc.chenzaomai.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pkn.zhixingplan.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fda.zhijiandao.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eqq.xuanzx.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uwk.sxryk.cn

[B03] switch / match / case
来源：http://smg.bjfxy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lja.shanyushiyangtech.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://npy.dashuyun.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tdr.haohaochexian.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://owa.yuanzhike.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://liw.cheryme.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://aka.aibaodan.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cfv.jinghuilouyu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://abv.cqqwz.cn

[B04] for 计数循环
来源：http://fjy.cheryme.top

Py:   for i in range(10): print(i)
来源：http://ypg.smart0.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://moh.yueranfly.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gln.zhengqikj.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mau.hcnkem.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hbe.andypj.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kth.yvedp.cn

Ruby: 10.times { |i| puts i }
来源：http://zle.aibaodan.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://goa.epnwcf.com

[B05] 遍历数组 / 列表
来源：http://whm.cucudq.cn

Py:   for item in arr: print(item)
来源：http://yfe.birdmap.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tek.guowangkeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://thr.zhiwuduotai.top

TS:   for (const item of arr) { console.log(item); }
来源：http://zgg.nwbrower.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://muf.shzxlz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qcw.xziqi.cn

Ruby: arr.each { |item| puts item }
来源：http://fih.havefunace.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ugl.cheryme.top

[B06] 遍历字典 / 对象
来源：http://vdo.daxiang520.top

Py:   for k, v in d.items(): print(k, v)
来源：http://tsy.shzxlz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vtp.wangdashe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tkh.gogol.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yzx.tianlin.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://naw.guowangkeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uac.sufxvd.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nte.uphjek.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eiq.hfpthk.cn

[B07] while 循环
来源：http://zyu.jianghu66.top

Py:   while i < 10: i += 1
来源：http://xhs.quarkkingdee.top

PHP:  while ($i < 10) { $i++; }
来源：http://deu.pycfn.com

JS:   while (i < 10) { i++; }
来源：http://ftc.shanyushiyangtech.top

TS:   while (i < 10) { i++; }
来源：http://dqw.quarkkingdee.top

Java: while (i < 10) { i++; }
来源：http://knm.zdbjq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wma.zhongyouzk.top

Ruby: while i < 10; i += 1; end
来源：http://non.kuanghao11.cn

C#:   while (i < 10) { i++; }
来源：http://gdk.daxiang520.top

[B08] do-while（至少执行一次）
来源：http://sxw.ybcxt.top

Py:   # 无 do-while：用 while True + break
来源：http://qgk.ppjwa.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sxf.zhiwuduotai.top

JS:   do { i++; } while (i < 10);
来源：http://osn.zhongyouzk.top

TS:   do { i++; } while (i < 10);
来源：http://mcl.shuidangran.top

Java: do { i++; } while (i < 10);
来源：http://ycn.yongpay.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hsn.sysykeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://xuh.xuanzx.com

C#:   do { i++; } while (i < 10);
来源：http://cdg.birdmap.top


<!-- 参考信息 -->