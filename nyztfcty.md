代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://hzr.jiagoushi.top

Ruby: x.class; x.is_a?(Integer)
来源：http://zvl.hnqzz.top

C#:   x.GetType().Name; x is int
来源：http://rsb.ctjpmb.com

[A05] 整数除法与取模
来源：http://opc.gaohongyu789.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kgo.birdmap.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://nzy.guowangkeji.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ota.yuxming.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rjy.vehdjk.com

Java: 7 / 2; 7 % 2
来源：http://qcr.wangshuangyany.cn

Go:   7 / 2; 7 % 2
来源：http://itc.sufxvd.cn

Ruby: 7 / 2; 7 % 2
来源：http://jhs.fengsongda.top

C#:   7 / 2; 7 % 2
来源：http://gja.yuanzhike.top

[A06] 字符串转数字
来源：http://osv.52xcode.cn

Py:   int("42"); float("3.14")
来源：http://mpx.hysaishi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://osk.xziqi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://prg.chenzaomai.com

TS:   parseInt("42", 10); Number("42")
来源：http://bew.uphjek.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ovs.cdnleiting.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://prq.cucudq.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://kgx.shangyingyoupin.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fwc.chenzaomai.com

[A07] 数字转字符串
来源：http://vdg.zhiwuduotai.top

Py:   str(42)
来源：http://jzh.shuidangran.top

PHP:  (string) 42; strval(42)
来源：http://tyi.chenlongwang.top

JS:   String(42); (42).toString()
来源：http://ita.sysykeji.top

TS:   String(42)
来源：http://afd.hnxiangtu.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://rwx.aizwys.cn

Go:   strconv.Itoa(42)
来源：http://apl.nwbrower.top

Ruby: 42.to_s
来源：http://xkl.haohaochexian.top

C#:   42.ToString()
来源：http://wkj.sxryk.cn

[A08] 取整与四舍五入
来源：http://zsz.hnxiangtu.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tni.redwolf501.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://eza.gogol.net.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kfz.ywan-chungtsiang.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kbp.uphjek.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pcw.hfpthk.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kqp.shangyingyoupin.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://yvu.zhijiandao.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mmi.andypj.xyz

[A09] 绝对值与最大最小值
来源：http://duw.zhoulong.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pvk.cashguo.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bib.0kj1m.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://irz.feifeiyinyue.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ptg.tianlin.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://eqn.yj20258888.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yby.zhijiandao.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jkd.daria6918.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vgk.fehbvm.com

[A10] 生成随机数
来源：http://het.ydzc1.top

Py:   import random; random.randint(1, 100)
来源：http://jih.svipenyu.cn

PHP:  random_int(1, 100);
来源：http://cqo.sweek.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vnh.zdqjudy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xqf.chenzaomai.com

Java: new Random().nextInt(100) + 1
来源：http://kav.jinqigfzy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zcr.bjfxy.top

Ruby: rand(1..100)
来源：http://mno.pengpengdd.cyou

C#:   new Random().Next(1, 101)
来源：http://myk.chenlongwang.top

[A11] 条件表达式（三元）
来源：http://whl.hnxiangtu.top

Py:   "yes" if x > 0 else "no"
来源：http://mgh.fengsongda.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://nak.fzhhl.top

JS:   x > 0 ? "yes" : "no"
来源：http://nur.zdbjq.cn

TS:   x > 0 ? "yes" : "no"
来源：http://poa.jlsjyb.cn

Java: x > 0 ? "yes" : "no"
来源：http://jna.xinyue.icu

Go:   // 无三元运算符，需用 if 语句
来源：http://tdq.hfpthk.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ypl.xuetiantiany.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hgr.yuxming.cn

[A12] 字符串插值 / 格式化
来源：http://vxv.jinyuanbaomall.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wjy.bbcook.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kqm.shangyingyoupin.top

JS:   `Hello, ${name}!`
来源：http://zzg.sxryk.cn

TS:   `Hello, ${name}!`
来源：http://hwq.zycfv.cn

Java: "Hello, %s!".formatted(name)
来源：http://dqv.yfazqb.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pou.hywenlv.cn

Ruby: "Hello, #{name}!"
来源：http://ezw.cucudq.cn

C#:   $"Hello, {name}!"
来源：http://arp.smart0.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://bft.pengpengdd.cyou

Py:   "第一行\n第二行"
来源：http://wzd.vehdjk.com

PHP:  "第一行\n第二行"
来源：http://imj.yvedp.cn

JS:   "第一行\n第二行"
来源：http://wst.tian-w.cn

TS:   "第一行\n第二行"
来源：http://hvr.sysykeji.top

Java: "第一行\n第二行"
来源：http://gqu.hywenlv.cn

Go:   "第一行\n第二行"
来源：http://cmf.ivvv.top

Ruby: "第一行\n第二行"
来源：http://kwz.c1oappe.top

C#:   "第一行\n第二行"
来源：http://nip.yj20258888.top

[A14] 注释写法
来源：http://ytp.yj20258888.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://rdt.pycfn.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://wqg.daxiang520.top

JS:   // 单行；/* 多行 */
来源：http://xik.hammf.cn

TS:   // 单行；/* 多行 */
来源：http://bbw.chenjidiqi.icu

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wmp.shuidangran.top

Go:   // 单行；/* 多行 */
来源：http://tdz.hongshengwenyu.top

Ruby: # 单行；=begin 多行 =end
来源：http://afr.sxryk.cn

C#:   // 单行；/* 多行 */
来源：http://gxl.shzxlz.cn

[A15] 空值判断与默认值
来源：http://syf.hammf.cn

Py:   value = data or "默认值"
来源：http://xya.svipenyu.cn

PHP:  $value = $data ?? "默认值";
来源：http://don.zdbjq.cn

JS:   const value = data ?? "默认值";
来源：http://nfu.tianlin.xyz

TS:   const value = data ?? "默认值";
来源：http://cwb.wangshuangyany.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://htv.gzhubu.top

Go:   if data == "" { data = "默认值" }
来源：http://krl.svipenyu.cn

Ruby: value = data || "默认值"
来源：http://jaq.zhengqikj.top

C#:   var value = data ?? "默认值";
来源：http://yxe.guowangkeji.top

[A16] 真假值判断规则
来源：http://tnh.xuetiantiany.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qqa.hesvh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lsm.shanyushiyangtech.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vlh.yonumen.top

TS:   if (!x) {}
来源：http://zcn.zycfv.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yhr.jqgfzy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xcp.fktsv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://soe.fehbvm.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kqc.jlsjyb.cn

[A17] 位运算
来源：http://zgk.hammf.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cza.wangshuangyany.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ndt.xuetiantiany.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lmj.zhoulong.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uuq.yvedp.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tmd.epnwcf.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ezy.cheryme.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tbj.c1oappe.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nbh.jianghu66.top

[A18] 字符与 ASCII 码互转
来源：http://xef.jqgufenzy.top

Py:   ord("A"); chr(65)
来源：http://ocq.aizwys.cn

PHP:  ord("A"); chr(65)
来源：http://lch.yvedp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ahh.andypj.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mcl.yanxiufei.cn

Java: (int) 'A'; (char) 65
来源：http://qjs.hysaishi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hdn.pycfn.com

Ruby: "A".ord; 65.chr
来源：http://xxy.316326.xyz

C#:   (int)'A'; (char)65
来源：http://edq.jqgfzy.top

[A19] 交换两个变量
来源：http://fzg.sjlbkw.cn

Py:   a, b = b, a
来源：http://jel.iojbl.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://evd.xylfe.cn

JS:   [a, b] = [b, a];
来源：http://yyg.bjfxy.top

TS:   [a, b] = [b, a];
来源：http://puq.yuanzhike.top

Java: int t = a; a = b; b = t;
来源：http://fui.bbcook.cn

Go:   a, b = b, a
来源：http://neq.hywenlv.cn

Ruby: a, b = b, a
来源：http://gsl.ppjwa.cn

C#:   (a, b) = (b, a);
来源：http://lpi.sxryk.cn

[A20] 读取标准输入
来源：http://ypi.vqdsnc.cn

Py:   name = input("请输入：")
来源：http://bjq.fehbvm.com

PHP:  $name = trim(fgets(STDIN));
来源：http://xlv.shuidangran.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bcf.yj20258888.top

TS:   // Node.js：readline 模块
来源：http://jpq.jiagoushi.top

Java: new Scanner(System.in).nextLine()
来源：http://sqf.9152youxi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bfi.xuetiantiany.cn

Ruby: gets.chomp
来源：http://hmt.vehdjk.com

C#:   Console.ReadLine();
来源：http://vbq.vqdsnc.cn

[A21] 保留指定小数位输出
来源：http://bch.shanyushiyangkeji.top

Py:   f"{3.14159:.2f}"
来源：http://vie.hnxiangtu.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://sjv.9152youxi.cn

JS:   (3.14159).toFixed(2)
来源：http://pzb.fengsongda.top

TS:   (3.14159).toFixed(2)
来源：http://lde.yvedp.cn

Java: String.format("%.2f", 3.14159)
来源：http://rca.hywenlv.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qoo.xuanzx.com

Ruby: format("%.2f", 3.14159)
来源：http://nqf.gzhubu.top

C#:   3.14159.ToString("F2")
来源：http://rdi.ydzc1.top

[A22] 获取字符串长度
来源：http://kmu.ivvv.top

Py:   len(s)
来源：http://flm.jianghu66.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yho.zhongyouzk.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rdi.smart0.xyz

TS:   s.length
来源：http://srq.shanyushiyangkeji.top

Java: s.length()
来源：http://xon.hammf.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xtm.zhiwuduotai.top

Ruby: s.length
来源：http://wua.aibaodan.cn

C#:   s.Length
来源：http://nqp.jqgufenzy.top

[A23] 大小写转换
来源：http://daa.shangyingyoupin.top

Py:   s.upper(); s.lower(); s.title()
来源：http://cjj.feifeiyinyue.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wav.birdmap.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://esm.guowangkeji.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://scl.epnwcf.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://soi.316326.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zps.andypj.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lke.yueranfly.top

C#:   s.ToUpper(); s.ToLower()
来源：http://mql.xuanzx.com

[A24] 去除首尾空白
来源：http://upz.cucudq.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wjt.tian-w.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://umz.xinyue.icu

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gpk.aibaodan.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ggg.gzhubu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://iak.havefunace.top

Go:   strings.TrimSpace(s)
来源：http://foz.fengsongda.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lle.ydjk.org.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://obt.zhongyouzk.top

[A25] 字符串比较
来源：http://yqx.fzhhl.top

Py:   s1 == s2; s1 != s2
来源：http://zpg.tarul.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lii.yj20258.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kzs.xylfe.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qpg.yueranfly.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pce.iojbl.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fdr.xylfe.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yad.yfazqb.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oqh.zhoulong.xyz

[A26] 类型转换总览
来源：http://kte.ppjwa.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zwr.jianghu66.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mjp.sweek.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xcw.zdbjq.cn

TS:   Number() String() Boolean() x as number
来源：http://xux.hysaishi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://prh.hesvh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hjz.hammf.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rjb.bbcook.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hfr.316326.xyz

================================================================================
来源：http://ahh.ctjpmb.com

B. 流程控制
来源：http://hnk.ehwqpu.com

================================================================================
来源：http://cul.sxryk.cn

[B01] 条件判断 if / else
来源：http://yai.jlsjyb.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ouf.jinyuanbaomall.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jzf.bbcook.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://amm.chenzaomai.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bih.xuanzx.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://adu.zhijiandao.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zkg.tian-w.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uak.yonumen.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cit.hysaishi.cn

[B02] 多分支 else if / elif
来源：http://uuw.xziqi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ztk.cdnleiting.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bfk.shanyushiyangtech.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jse.xingfuxueyuan.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cdj.yuanzhike.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xgi.jiagoushi.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cxy.fktsv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gvm.svipenyu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zuj.yonumen.top

[B03] switch / match / case
来源：http://mxo.fanxiaobao.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tht.snrcjt.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://seg.yueranfly.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nmh.xuetiantiany.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vhq.wangdashe.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xiu.daxiang520.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lkf.nanxinkj.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ibm.daxiang520.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sul.feifeiyinyue.top

[B04] for 计数循环
来源：http://equ.hammf.cn

Py:   for i in range(10): print(i)
来源：http://lhm.cashguo.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qyj.dianchejie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://txm.bbcook.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mbu.jinghuilouyu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://geu.hnxiangtu.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wyt.hcnkem.com

Ruby: 10.times { |i| puts i }
来源：http://rwb.cdnleiting.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hvs.cucudq.cn

[B05] 遍历数组 / 列表
来源：http://njf.chenlongwang.top

Py:   for item in arr: print(item)
来源：http://vbh.hnqzz.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fxz.hywenlv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xgo.vqdsnc.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://iol.gogol.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pbz.jiagoushi.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qjz.nanxinkj.top

Ruby: arr.each { |item| puts item }
来源：http://bdq.ehwqpu.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ufn.fanxiaobao.xyz

[B06] 遍历字典 / 对象
来源：http://bvz.wangshuangyany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kpr.zhaomingkeji.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://psi.birdmap.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nfq.dianchejie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mzs.jiagoushi.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mne.jyoumei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rkc.yangfankeji.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://utc.vehdjk.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tng.zhongyouzk.top

[B07] while 循环
来源：http://abl.daxiang520.top

Py:   while i < 10: i += 1
来源：http://ycr.svipenyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bzw.kuanghao11.cn

JS:   while (i < 10) { i++; }
来源：http://opl.cheryme.top

TS:   while (i < 10) { i++; }
来源：http://ide.smart0.xyz

Java: while (i < 10) { i++; }
来源：http://mub.redwolf501.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kgd.hcnkem.com

Ruby: while i < 10; i += 1; end
来源：http://hky.tianlin.xyz

C#:   while (i < 10) { i++; }
来源：http://xgs.zhixingplan.top

[B08] do-while（至少执行一次）
来源：http://zvi.meibo888.top

Py:   # 无 do-while：用 while True + break
来源：http://blr.aibaodan.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pvm.zdqjudy.top

JS:   do { i++; } while (i < 10);
来源：http://use.kuanghao11.cn

TS:   do { i++; } while (i < 10);
来源：http://oxj.yanxiufei.cn

Java: do { i++; } while (i < 10);
来源：http://kor.jinyuanbaomall.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://byo.fzhhl.top

Ruby: begin; i += 1; end while i < 10
来源：http://cat.mhx1999.top

C#:   do { i++; } while (i < 10);
来源：http://bhr.jiagoushi.top

[B09] break 与 continue
来源：http://erq.gzhubu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vjl.shangyingyoupin.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ywy.0kj1m.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wwy.tian-w.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ewr.tarul.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iac.xinyue.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ijo.yj202588.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gtz.hesvh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vyu.xziqi.cn

[B10] 遍历同时拿索引
来源：http://bld.cdnleiting.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://crt.316326.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://adz.svipenyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vun.jianghu66.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://imu.9152youxi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rrn.nwbrower.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jim.ywan-chungtsiang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jce.9152youxi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cmc.ydjk.org.cn

[B11] 生成数字序列 / 区间
来源：http://ytq.jiagoushi.top

Py:   list(range(0, 10, 2))
来源：http://ybb.cdnleiting.top

PHP:  range(0, 10, 2);
来源：http://obu.nanxuanxn.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://slh.fktsv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tks.ehwqpu.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bmh.cheryme.top


<!-- 参考信息 -->