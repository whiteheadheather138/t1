代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://nkz.havefunace.top

[A03] 常量定义
来源：http://cyd.cashguo.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vrc.hfpthk.cn

PHP:  const PI = 3.14159;
来源：http://pkh.ppjwa.cn

JS:   const PI = 3.14159;
来源：http://jzo.yongpay.top

TS:   const PI: number = 3.14159;
来源：http://tzi.meibo888.top

Java: static final double PI = 3.14159;
来源：http://czp.jinqigfzy.top

Go:   const PI = 3.14159
来源：http://rvx.ybcxt.top

Ruby: PI = 3.14159
来源：http://nnr.bbcook.cn

C#:   const double PI = 3.14159;
来源：http://tws.ydzc1.top

[A04] 判断变量类型
来源：http://xad.yfazqb.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://yye.jianghu66.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wsq.tianlin.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://svn.ydjk.org.cn

TS:   typeof x; x instanceof Date
来源：http://lws.fktsv.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vsx.zhixingplan.top

Go:   reflect.TypeOf(x).Name()
来源：http://snr.uphjek.com

Ruby: x.class; x.is_a?(Integer)
来源：http://ext.tarul.cn

C#:   x.GetType().Name; x is int
来源：http://zvt.9152youxi.cn

[A05] 整数除法与取模
来源：http://ytn.xingfuxueyuan.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ofz.hnxiangtu.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://bxe.snrcjt.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jsj.jyoumei.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xod.hesvh.cn

Java: 7 / 2; 7 % 2
来源：http://wqf.jinghuilouyu.cn

Go:   7 / 2; 7 % 2
来源：http://jdu.aibaodan.cn

Ruby: 7 / 2; 7 % 2
来源：http://ccv.kuanghao11.cn

C#:   7 / 2; 7 % 2
来源：http://eux.jiagoushi.top

[A06] 字符串转数字
来源：http://ktj.yuxming.cn

Py:   int("42"); float("3.14")
来源：http://oit.cqqwz.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wxj.nwbrower.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uqx.ydzc1.top

TS:   parseInt("42", 10); Number("42")
来源：http://vqb.uphjek.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dno.haohaochexian.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://var.yj20258.top

Ruby: "42".to_i; "3.14".to_f
来源：http://rfa.ybcxt.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cjt.yanxiufei.cn

[A07] 数字转字符串
来源：http://fsa.xuanzx.com

Py:   str(42)
来源：http://xff.ywan-chungtsiang.top

PHP:  (string) 42; strval(42)
来源：http://chb.zhijiandao.cn

JS:   String(42); (42).toString()
来源：http://dlz.zhijiandao.cn

TS:   String(42)
来源：http://wsj.cheryme.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ejq.pengpengdd.cyou

Go:   strconv.Itoa(42)
来源：http://dht.yj202588.top

Ruby: 42.to_s
来源：http://wyo.0kj1m.cn

C#:   42.ToString()
来源：http://ekm.guowangkeji.top

[A08] 取整与四舍五入
来源：http://xwq.xuanzx.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://oah.jinghuilouyu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bmm.0kj1m.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lls.cheryme.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cvy.fzhhl.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://oqh.zhengqikj.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lga.snrcjt.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ooc.epnwcf.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mqu.zdbjq.cn

[A09] 绝对值与最大最小值
来源：http://lum.chenjidiqi.icu

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gke.jinqigfzy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ayj.yongpay.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fjo.xuetiantiany.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ywy.jinqigfzy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ylx.chenjidiqi.icu

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kqz.wangshuangyany.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ouz.hesvh.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hzm.havefunace.top

[A10] 生成随机数
来源：http://qsb.xingfuxueyuan.xyz

Py:   import random; random.randint(1, 100)
来源：http://eli.guannengcc.top

PHP:  random_int(1, 100);
来源：http://uyk.yongpay.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gzo.fzhhl.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hxh.zhaomingkeji.xyz

Java: new Random().nextInt(100) + 1
来源：http://tbw.quarkkingdee.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kia.ydjk.org.cn

Ruby: rand(1..100)
来源：http://zsp.jqgfzy.top

C#:   new Random().Next(1, 101)
来源：http://pjw.sysykeji.top

[A11] 条件表达式（三元）
来源：http://fby.nanxinkj.top

Py:   "yes" if x > 0 else "no"
来源：http://bgp.yongpay.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://nfy.52xcode.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jli.hcnkem.com

TS:   x > 0 ? "yes" : "no"
来源：http://bhu.ehwqpu.com

Java: x > 0 ? "yes" : "no"
来源：http://vmr.c1oappe.top

Go:   // 无三元运算符，需用 if 语句
来源：http://gdi.xingfuxueyuan.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://tgl.nanxinkj.top

C#:   x > 0 ? "yes" : "no"
来源：http://gjw.fzhhl.top

[A12] 字符串插值 / 格式化
来源：http://pos.sysykeji.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yzp.yj20258.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xcp.316326.xyz

JS:   `Hello, ${name}!`
来源：http://ljc.xziqi.cn

TS:   `Hello, ${name}!`
来源：http://ofy.meibo888.top

Java: "Hello, %s!".formatted(name)
来源：http://wti.fktsv.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rll.yuanzhike.top

Ruby: "Hello, #{name}!"
来源：http://fso.chenzaomai.com

C#:   $"Hello, {name}!"
来源：http://xtt.jinqigufen.top

[A13] 多行字符串（练习 \n 转义）
来源：http://nki.daria6918.cn

Py:   "第一行\n第二行"
来源：http://lkm.gzhubu.top

PHP:  "第一行\n第二行"
来源：http://efg.smart0.xyz

JS:   "第一行\n第二行"
来源：http://gxp.hysaishi.cn

TS:   "第一行\n第二行"
来源：http://nfm.tanke756.top

Java: "第一行\n第二行"
来源：http://vdf.haohaochexian.top

Go:   "第一行\n第二行"
来源：http://pou.gogol.net.cn

Ruby: "第一行\n第二行"
来源：http://krx.daxiang520.top

C#:   "第一行\n第二行"
来源：http://buc.svipenyu.cn

[A14] 注释写法
来源：http://qqq.ywan-chungtsiang.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://vin.vehdjk.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://loo.shangyingyoupin.top

JS:   // 单行；/* 多行 */
来源：http://wtp.nanxuanxn.top

TS:   // 单行；/* 多行 */
来源：http://zoe.fanxiaobao.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://del.tarul.cn

Go:   // 单行；/* 多行 */
来源：http://xik.cdnleiting.top

Ruby: # 单行；=begin 多行 =end
来源：http://tha.shanyushiyangtech.top

C#:   // 单行；/* 多行 */
来源：http://qhp.zhixingplan.top

[A15] 空值判断与默认值
来源：http://ivo.jinqigufen.top

Py:   value = data or "默认值"
来源：http://rjc.hysaishi.cn

PHP:  $value = $data ?? "默认值";
来源：http://ozc.tian-w.cn

JS:   const value = data ?? "默认值";
来源：http://zhv.gogol.net.cn

TS:   const value = data ?? "默认值";
来源：http://qco.zhiwuduotai.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pxs.daxiang520.top

Go:   if data == "" { data = "默认值" }
来源：http://smc.yvedp.cn

Ruby: value = data || "默认值"
来源：http://pie.iojbl.cn

C#:   var value = data ?? "默认值";
来源：http://ubl.shanyushiyangkeji.top

[A16] 真假值判断规则
来源：http://lnu.mhx1999.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jgv.xingfuxueyuan.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jsl.pengpengdd.cyou

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://skj.hcnkem.com

TS:   if (!x) {}
来源：http://qua.meibo888.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hte.yuxming.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jac.yvedp.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rof.fzhhl.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ced.cdnleiting.top

[A17] 位运算
来源：http://iof.hcnkem.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bjh.dianchejie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jkb.yonumen.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://igb.fehbvm.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jqo.quarkkingdee.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://phu.jianghu66.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xvj.hywenlv.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hph.smart0.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pcv.yonumen.top

[A18] 字符与 ASCII 码互转
来源：http://ehm.sxryk.cn

Py:   ord("A"); chr(65)
来源：http://zcu.ehwqpu.com

PHP:  ord("A"); chr(65)
来源：http://jiq.andypj.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lbe.jianghu66.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iaf.hammf.cn

Java: (int) 'A'; (char) 65
来源：http://zao.cucudq.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yke.shangyingyoupin.top

Ruby: "A".ord; 65.chr
来源：http://riu.xuanzx.com

C#:   (int)'A'; (char)65
来源：http://hmf.uphjek.com

[A19] 交换两个变量
来源：http://rdm.haohaochexian.top

Py:   a, b = b, a
来源：http://fvk.shzxlz.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://lfj.vqdsnc.cn

JS:   [a, b] = [b, a];
来源：http://zwl.dianchejie.cn

TS:   [a, b] = [b, a];
来源：http://joo.jinqigfzy.top

Java: int t = a; a = b; b = t;
来源：http://usz.chenlongwang.top

Go:   a, b = b, a
来源：http://agv.ybcxt.top

Ruby: a, b = b, a
来源：http://jyg.yonumen.top

C#:   (a, b) = (b, a);
来源：http://xok.hnqzz.top

[A20] 读取标准输入
来源：http://gzz.yfazqb.com

Py:   name = input("请输入：")
来源：http://kfp.cqqwz.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://bqs.sweek.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://heq.ppjwa.cn

TS:   // Node.js：readline 模块
来源：http://gii.hammf.cn

Java: new Scanner(System.in).nextLine()
来源：http://deb.wangshuangyany.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://npx.jinqigufen.top

Ruby: gets.chomp
来源：http://nbs.zhoulong.xyz

C#:   Console.ReadLine();
来源：http://mqg.0kj1m.cn

[A21] 保留指定小数位输出
来源：http://ghy.jyoumei.cn

Py:   f"{3.14159:.2f}"
来源：http://uqf.feifeiyinyue.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gxy.0kj1m.cn

JS:   (3.14159).toFixed(2)
来源：http://vlk.ctjpmb.com

TS:   (3.14159).toFixed(2)
来源：http://iyp.jqgufenzy.top

Java: String.format("%.2f", 3.14159)
来源：http://knw.havefunace.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fbg.daxiang520.top

Ruby: format("%.2f", 3.14159)
来源：http://caj.fehbvm.com

C#:   3.14159.ToString("F2")
来源：http://ckm.ppjwa.cn

[A22] 获取字符串长度
来源：http://oal.kuanghao11.cn

Py:   len(s)
来源：http://hts.zhongyouzk.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wla.cucudq.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qmh.yangfankeji.com

TS:   s.length
来源：http://rnv.wangdashe.top

Java: s.length()
来源：http://vix.jiagoushi.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://igf.guowangkeji.top

Ruby: s.length
来源：http://drs.cdnleiting.top

C#:   s.Length
来源：http://fad.cashguo.top

[A23] 大小写转换
来源：http://jnw.hcnkem.com

Py:   s.upper(); s.lower(); s.title()
来源：http://zxk.mhx1999.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://oax.sxryk.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nau.zhiwuduotai.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rdb.sysykeji.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hkc.andypj.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sls.vehdjk.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://swn.ywan-chungtsiang.top

C#:   s.ToUpper(); s.ToLower()
来源：http://mlu.xylfe.cn

[A24] 去除首尾空白
来源：http://dwv.hysaishi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qlh.shanyushiyangtech.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rzy.fzhhl.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fwo.yj20258888.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://not.yuanzhike.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://irv.haohaochexian.top

Go:   strings.TrimSpace(s)
来源：http://mvm.yuanzhike.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qku.pengpengdd.cyou

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dpm.yvedp.cn

[A25] 字符串比较
来源：http://tvu.jianghu66.top

Py:   s1 == s2; s1 != s2
来源：http://njz.redwolf501.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ydr.ppjwa.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ljf.yuanzhike.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rot.0kj1m.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vtc.yfazqb.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ili.jianghu66.top

Ruby: s1 == s2; s1 <=> s2
来源：http://bvm.ydjk.org.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ysj.c1oappe.top

[A26] 类型转换总览
来源：http://eou.fktsv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tep.zhongyouzk.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ehk.hammf.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qcw.hnqzz.top

TS:   Number() String() Boolean() x as number
来源：http://llz.shangyingyoupin.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sxs.ydzc1.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://upo.fehbvm.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://qpr.hongshengwenyu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qoe.jyoumei.cn

================================================================================
来源：http://kyj.yj20258.top

B. 流程控制
来源：http://qlj.zhongyouzk.top

================================================================================
来源：http://olx.zhongyouzk.top

[B01] 条件判断 if / else
来源：http://cjv.nanxinkj.top

Py:   result = "正" if x > 0 else "非正"
来源：http://gsx.kuanghao11.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wjs.gogol.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kdx.tianlin.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tet.shangyingyoupin.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://yip.aizwys.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nzp.ctjpmb.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mzn.vqdsnc.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ahq.316326.xyz

[B02] 多分支 else if / elif
来源：http://rtr.zhongyouzk.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nqd.316326.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gft.chenzaomai.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xkk.pengpengdd.cyou

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://juh.shanyushiyangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oxe.gzhubu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://buv.guannengcc.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dyd.aizwys.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ddl.hnqzz.top

[B03] switch / match / case
来源：http://njv.sufxvd.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lmb.jinqigfzy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vje.guowangkeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eav.bjfxy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cwf.shanyushiyangtech.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yez.shzxlz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://geu.guowangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rco.zhongyouzk.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://osf.cashguo.top

[B04] for 计数循环
来源：http://scx.tarul.cn

Py:   for i in range(10): print(i)
来源：http://amy.fzhhl.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xiy.vqdsnc.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xra.pengpengdd.cyou

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rtj.zhaomingkeji.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yht.pengpengdd.cyou

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dam.yanxiufei.cn

Ruby: 10.times { |i| puts i }
来源：http://ynh.cucudq.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://trq.52xcode.cn

[B05] 遍历数组 / 列表
来源：http://aur.shangyingyoupin.top

Py:   for item in arr: print(item)
来源：http://soe.feifeiyinyue.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wir.epnwcf.com

JS:   for (const item of arr) { console.log(item); }
来源：http://ghd.ehwqpu.com

TS:   for (const item of arr) { console.log(item); }
来源：http://kpq.jqgufenzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tou.andypj.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tlj.jiagoushi.top

Ruby: arr.each { |item| puts item }
来源：http://btm.tanke756.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qre.316326.xyz

[B06] 遍历字典 / 对象
来源：http://tum.shzxlz.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fjb.dashuyun.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gja.shangyingyoupin.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qoa.shzxlz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vxi.yuanzhike.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lll.snrcjt.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mwn.ivvv.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tin.hesvh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pdi.dianchejie.cn

[B07] while 循环
来源：http://jal.yj20258888.top

Py:   while i < 10: i += 1
来源：http://wip.sjlbkw.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hcy.hfpthk.cn

JS:   while (i < 10) { i++; }
来源：http://ctg.ctjpmb.com

TS:   while (i < 10) { i++; }
来源：http://jmh.dianchejie.cn

Java: while (i < 10) { i++; }
来源：http://hlr.hammf.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tyi.havefunace.top

Ruby: while i < 10; i += 1; end
来源：http://uzk.ctjpmb.com

C#:   while (i < 10) { i++; }
来源：http://crc.nwbrower.top

[B08] do-while（至少执行一次）
来源：http://rdm.andypj.xyz

Py:   # 无 do-while：用 while True + break
来源：http://cpf.sjlbkw.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hid.guannengcc.top

JS:   do { i++; } while (i < 10);
来源：http://kkl.hfpthk.cn

TS:   do { i++; } while (i < 10);
来源：http://zbv.pengpengdd.cyou

Java: do { i++; } while (i < 10);
来源：http://inu.jiagoushi.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zmg.pengpengdd.cyou

Ruby: begin; i += 1; end while i < 10
来源：http://wdx.ctjpmb.com

C#:   do { i++; } while (i < 10);
来源：http://ich.cdnleiting.top

[B09] break 与 continue
来源：http://heq.sufxvd.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xft.fktsv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nwj.shuidangran.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pmv.xinyue.icu

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uwh.hysaishi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dhv.yangfankeji.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kbj.aibaodan.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hls.hongshengwenyu.top


<!-- 参考信息 -->