代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mdw.uphjek.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cpq.yonumen.top

TS:   typeof x; x instanceof Date
来源：http://sii.gaohongyu789.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://aor.yuanzhike.top

Go:   reflect.TypeOf(x).Name()
来源：http://fxa.cqqwz.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://feu.sxryk.cn

C#:   x.GetType().Name; x is int
来源：http://lzr.xuetiantiany.cn

[A05] 整数除法与取模
来源：http://bmh.jinghuilouyu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lpg.yuanzhike.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://uma.hnqzz.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://thz.hesvh.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sdb.fehbvm.com

Java: 7 / 2; 7 % 2
来源：http://dlq.zhaomingkeji.xyz

Go:   7 / 2; 7 % 2
来源：http://qqa.jinyuanbaomall.cn

Ruby: 7 / 2; 7 % 2
来源：http://uxu.guannengcc.top

C#:   7 / 2; 7 % 2
来源：http://rlf.hammf.cn

[A06] 字符串转数字
来源：http://vby.ctjpmb.com

Py:   int("42"); float("3.14")
来源：http://wst.gogol.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cpb.316326.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ivl.fehbvm.com

TS:   parseInt("42", 10); Number("42")
来源：http://rwu.zycfv.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hoj.quarkkingdee.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bpt.ybcxt.top

Ruby: "42".to_i; "3.14".to_f
来源：http://vxp.bjfxy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kzy.yueranfly.top

[A07] 数字转字符串
来源：http://bwy.wangshuangyany.cn

Py:   str(42)
来源：http://rgz.fzhhl.top

PHP:  (string) 42; strval(42)
来源：http://dlc.ywan-chungtsiang.top

JS:   String(42); (42).toString()
来源：http://oep.svipenyu.cn

TS:   String(42)
来源：http://aup.uphjek.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://jql.gogol.net.cn

Go:   strconv.Itoa(42)
来源：http://ohc.zycfv.cn

Ruby: 42.to_s
来源：http://gjp.cashguo.top

C#:   42.ToString()
来源：http://udf.bjfxy.top

[A08] 取整与四舍五入
来源：http://czc.uphjek.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://swh.xuetiantiany.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rtr.wangdashe.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://clz.nwbrower.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ctd.yanxiufei.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ewr.iojbl.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://flz.dianchejie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wns.aibaodan.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://nms.52xcode.cn

[A09] 绝对值与最大最小值
来源：http://kcs.cheryme.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://oxd.shanyushiyangkeji.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vnl.mhx1999.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://paj.hammf.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ure.tian-w.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vlm.jqgfzy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qwj.guowangkeji.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rza.wangshuangyany.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xdz.guowangkeji.top

[A10] 生成随机数
来源：http://scf.kuanghao11.cn

Py:   import random; random.randint(1, 100)
来源：http://lyr.fehbvm.com

PHP:  random_int(1, 100);
来源：http://pko.mhx1999.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hxs.daxiang520.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://drd.52xcode.cn

Java: new Random().nextInt(100) + 1
来源：http://mmq.xziqi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bze.quarkkingdee.top

Ruby: rand(1..100)
来源：http://fzx.iojbl.cn

C#:   new Random().Next(1, 101)
来源：http://lmo.hcnkem.com

[A11] 条件表达式（三元）
来源：http://mcf.ctjpmb.com

Py:   "yes" if x > 0 else "no"
来源：http://wpd.52xcode.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hyv.dianchejie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xdx.yongpay.top

TS:   x > 0 ? "yes" : "no"
来源：http://qra.feifeiyinyue.top

Java: x > 0 ? "yes" : "no"
来源：http://led.hywenlv.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://toc.hongshengwenyu.top

Ruby: x > 0 ? "yes" : "no"
来源：http://slc.nwbrower.top

C#:   x > 0 ? "yes" : "no"
来源：http://wqi.yfazqb.com

[A12] 字符串插值 / 格式化
来源：http://cit.fengsongda.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://udp.yj20258888.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qie.jinqigufen.top

JS:   `Hello, ${name}!`
来源：http://gqx.shanyushiyangtech.top

TS:   `Hello, ${name}!`
来源：http://sbb.hysaishi.cn

Java: "Hello, %s!".formatted(name)
来源：http://amh.sjlbkw.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sop.yonumen.top

Ruby: "Hello, #{name}!"
来源：http://qbp.dashuyun.cn

C#:   $"Hello, {name}!"
来源：http://ere.fzhhl.top

[A13] 多行字符串（练习 \n 转义）
来源：http://bqb.aibaodan.cn

Py:   "第一行\n第二行"
来源：http://top.zhiwuduotai.top

PHP:  "第一行\n第二行"
来源：http://pnv.sweek.top

JS:   "第一行\n第二行"
来源：http://onw.yfazqb.com

TS:   "第一行\n第二行"
来源：http://oiy.xziqi.cn

Java: "第一行\n第二行"
来源：http://dfz.shangyingyoupin.top

Go:   "第一行\n第二行"
来源：http://abe.zhixingplan.top

Ruby: "第一行\n第二行"
来源：http://kyw.chenzaomai.com

C#:   "第一行\n第二行"
来源：http://fba.vehdjk.com

[A14] 注释写法
来源：http://lew.wangshuangyany.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://hsp.zhiwuduotai.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://qel.shanyushiyangtech.top

JS:   // 单行；/* 多行 */
来源：http://ehj.hcnkem.com

TS:   // 单行；/* 多行 */
来源：http://hid.bbcook.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xij.ivvv.top

Go:   // 单行；/* 多行 */
来源：http://tql.yangfankeji.com

Ruby: # 单行；=begin 多行 =end
来源：http://vso.yueranfly.top

C#:   // 单行；/* 多行 */
来源：http://mrj.yangfankeji.com

[A15] 空值判断与默认值
来源：http://sce.xuanzx.com

Py:   value = data or "默认值"
来源：http://bgn.nanxuanxn.top

PHP:  $value = $data ?? "默认值";
来源：http://tww.yvedp.cn

JS:   const value = data ?? "默认值";
来源：http://jtr.ctjpmb.com

TS:   const value = data ?? "默认值";
来源：http://vxs.zhengqikj.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://upd.havefunace.top

Go:   if data == "" { data = "默认值" }
来源：http://xfd.hywenlv.cn

Ruby: value = data || "默认值"
来源：http://heq.yj202588.top

C#:   var value = data ?? "默认值";
来源：http://rto.jinqigfzy.top

[A16] 真假值判断规则
来源：http://kdh.cucudq.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tzr.zdbjq.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://euj.zycfv.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://oxm.yj202588.top

TS:   if (!x) {}
来源：http://zeq.ydzc1.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://syl.yanxiufei.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qcu.xinyue.icu

Ruby: unless x            # nil 与 false 为假
来源：http://yin.yfazqb.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ept.shuidangran.top

[A17] 位运算
来源：http://nwu.zhaomingkeji.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kkn.wangshuangyany.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zuj.hysaishi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://des.shzxlz.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bjg.shuidangran.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tsb.fktsv.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ibv.wangshuangyany.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oqw.vqdsnc.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cgc.zdbjq.cn

[A18] 字符与 ASCII 码互转
来源：http://xgq.yongpay.top

Py:   ord("A"); chr(65)
来源：http://jcg.hammf.cn

PHP:  ord("A"); chr(65)
来源：http://zzf.xziqi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://scv.sxryk.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://awy.ydjk.org.cn

Java: (int) 'A'; (char) 65
来源：http://nny.shuidangran.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://aqx.fzhhl.top

Ruby: "A".ord; 65.chr
来源：http://eld.yuanzhike.top

C#:   (int)'A'; (char)65
来源：http://lje.jiagoushi.top

[A19] 交换两个变量
来源：http://uzk.gogol.net.cn

Py:   a, b = b, a
来源：http://etn.xziqi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qun.zhixingplan.top

JS:   [a, b] = [b, a];
来源：http://ybk.wangshuangyany.cn

TS:   [a, b] = [b, a];
来源：http://dmq.cqqwz.cn

Java: int t = a; a = b; b = t;
来源：http://dbe.kuanghao11.cn

Go:   a, b = b, a
来源：http://ara.svipenyu.cn

Ruby: a, b = b, a
来源：http://gox.ybcxt.top

C#:   (a, b) = (b, a);
来源：http://ftr.fanxiaobao.xyz

[A20] 读取标准输入
来源：http://rsu.shanyushiyangtech.top

Py:   name = input("请输入：")
来源：http://loj.fzhhl.top

PHP:  $name = trim(fgets(STDIN));
来源：http://oxe.ppjwa.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ueu.haohaochexian.top

TS:   // Node.js：readline 模块
来源：http://nmu.vqdsnc.cn

Java: new Scanner(System.in).nextLine()
来源：http://szj.hesvh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://luh.gotoacloud.top

Ruby: gets.chomp
来源：http://dbh.quarkkingdee.top

C#:   Console.ReadLine();
来源：http://nkt.xingfuxueyuan.xyz

[A21] 保留指定小数位输出
来源：http://qxo.hammf.cn

Py:   f"{3.14159:.2f}"
来源：http://yzu.yanxiufei.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wgj.guannengcc.top

JS:   (3.14159).toFixed(2)
来源：http://qpk.havefunace.top

TS:   (3.14159).toFixed(2)
来源：http://yev.yj202588.top

Java: String.format("%.2f", 3.14159)
来源：http://xcp.hcnkem.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://exn.tarul.cn

Ruby: format("%.2f", 3.14159)
来源：http://rvo.daxiang520.top

C#:   3.14159.ToString("F2")
来源：http://uys.jqgfzy.top

[A22] 获取字符串长度
来源：http://ugh.ydjk.org.cn

Py:   len(s)
来源：http://tyt.daxiang520.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zan.gogol.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://log.hongshengwenyu.top

TS:   s.length
来源：http://une.xuanzx.com

Java: s.length()
来源：http://hup.yonumen.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cfj.yanxiufei.cn

Ruby: s.length
来源：http://drt.cqqwz.cn

C#:   s.Length
来源：http://hhc.vqdsnc.cn

[A23] 大小写转换
来源：http://rbv.aizwys.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ffm.meibo888.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qmz.zhiwuduotai.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dko.cqqwz.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://aqm.sxryk.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ojg.shanyushiyangtech.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dzf.tianlin.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gna.shanyushiyangtech.top

C#:   s.ToUpper(); s.ToLower()
来源：http://unb.ehwqpu.com

[A24] 去除首尾空白
来源：http://kns.jinqigufen.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xpk.ehwqpu.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://knf.ppjwa.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vdw.birdmap.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zyz.pengpengdd.cyou

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://eee.havefunace.top

Go:   strings.TrimSpace(s)
来源：http://ajk.guowangkeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zrm.gzhubu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wni.tian-w.cn

[A25] 字符串比较
来源：http://sbf.ydzc1.top

Py:   s1 == s2; s1 != s2
来源：http://utt.yj20258888.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://akn.cashguo.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zzy.yanxiufei.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sem.nwbrower.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://isd.ctjpmb.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lga.jinghuilouyu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mlv.dashuyun.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dng.cdnleiting.top

[A26] 类型转换总览
来源：http://nqz.jqgufenzy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vow.jqgufenzy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://coo.meibo888.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hxv.ydzc1.top

TS:   Number() String() Boolean() x as number
来源：http://voc.yj20258888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hqr.andypj.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gra.chenzaomai.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://pke.9152youxi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ggq.yonumen.top

================================================================================
来源：http://jkf.cucudq.cn

B. 流程控制
来源：http://deh.hywenlv.cn

================================================================================
来源：http://olm.xuetiantiany.cn

[B01] 条件判断 if / else
来源：http://uqw.aibaodan.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://njd.aibaodan.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://egw.fzhhl.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nnu.xylfe.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://unu.svipenyu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://muy.cheryme.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lzo.fengsongda.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fxz.hnqzz.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hra.yongpay.top

[B02] 多分支 else if / elif
来源：http://giv.bbcook.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://chw.bbcook.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ets.cheryme.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cyi.tanke756.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qaz.gaohongyu789.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oki.yueranfly.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tpi.hywenlv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xwb.hfpthk.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bzh.316326.xyz

[B03] switch / match / case
来源：http://mdk.zhoulong.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bik.gaohongyu789.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uzm.zycfv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aeu.jinqigfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://leh.sysykeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gef.sweek.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nzd.daria6918.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://act.xylfe.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dty.fktsv.cn

[B04] for 计数循环
来源：http://pch.wangdashe.top

Py:   for i in range(10): print(i)
来源：http://owx.sufxvd.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://owe.ybcxt.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jps.gotoacloud.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yxf.yuxming.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://agt.hcnkem.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fzb.ybcxt.top

Ruby: 10.times { |i| puts i }
来源：http://grb.pycfn.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ccd.hammf.cn

[B05] 遍历数组 / 列表
来源：http://kto.yuanzhike.top

Py:   for item in arr: print(item)
来源：http://smb.ctjpmb.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wra.hysaishi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://irk.yfazqb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://shy.tanke756.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ypg.zycfv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ssn.shanyushiyangtech.top

Ruby: arr.each { |item| puts item }
来源：http://rpt.aibaodan.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jbc.snrcjt.cn

[B06] 遍历字典 / 对象
来源：http://mxo.zhijiandao.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uqf.andypj.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://arm.andypj.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tev.epnwcf.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wtv.yonumen.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ivr.yj20258888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zad.haohaochexian.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qxz.jinyuanbaomall.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qdb.xuetiantiany.cn

[B07] while 循环
来源：http://ftl.jyoumei.cn

Py:   while i < 10: i += 1
来源：http://gmd.cashguo.top

PHP:  while ($i < 10) { $i++; }
来源：http://ggd.andypj.xyz

JS:   while (i < 10) { i++; }
来源：http://oma.andypj.xyz

TS:   while (i < 10) { i++; }
来源：http://jsv.gaohongyu789.top

Java: while (i < 10) { i++; }
来源：http://jyb.wangshuangyany.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iak.guowangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://psc.jinqigfzy.top

C#:   while (i < 10) { i++; }
来源：http://uwx.shangyingyoupin.top

[B08] do-while（至少执行一次）
来源：http://qry.vqdsnc.cn

Py:   # 无 do-while：用 while True + break
来源：http://rgy.yangfankeji.com

PHP:  do { $i++; } while ($i < 10);
来源：http://gru.hesvh.cn

JS:   do { i++; } while (i < 10);
来源：http://vvk.jinyuanbaomall.cn

TS:   do { i++; } while (i < 10);
来源：http://hhv.hywenlv.cn

Java: do { i++; } while (i < 10);
来源：http://uot.yj202588.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bal.c1oappe.top

Ruby: begin; i += 1; end while i < 10
来源：http://vlg.52xcode.cn

C#:   do { i++; } while (i < 10);
来源：http://zhj.xylfe.cn

[B09] break 与 continue
来源：http://amj.yj20258888.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://msc.52xcode.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kar.zhixingplan.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qja.shangyingyoupin.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://txx.cheryme.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dah.daria6918.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vgu.daxiang520.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rld.shanyushiyangtech.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bit.zhijiandao.cn

[B10] 遍历同时拿索引
来源：http://oqb.chenjidiqi.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ljz.jinqigufen.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hry.gaohongyu789.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vbe.xylfe.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rty.gzhubu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://shb.haohaochexian.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fdx.yfazqb.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nih.tian-w.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yhv.feifeiyinyue.top

[B11] 生成数字序列 / 区间
来源：http://yft.bbcook.cn

Py:   list(range(0, 10, 2))
来源：http://ltx.0kj1m.cn


<!-- 参考信息 -->