代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dqa.zhongyouzk.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://coj.yfazqb.com

TS:   typeof x; x instanceof Date
来源：http://irm.yj20258888.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mhs.zhixingplan.top

Go:   reflect.TypeOf(x).Name()
来源：http://yex.jinghuilouyu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://log.shanyushiyangkeji.top

C#:   x.GetType().Name; x is int
来源：http://fbr.hfpthk.cn

[A05] 整数除法与取模
来源：http://snj.52xcode.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kcb.dashuyun.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://tnz.0kj1m.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sum.jinqigfzy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qyf.svipenyu.cn

Java: 7 / 2; 7 % 2
来源：http://mdh.wangdashe.top

Go:   7 / 2; 7 % 2
来源：http://rid.yonumen.top

Ruby: 7 / 2; 7 % 2
来源：http://ejd.redwolf501.top

C#:   7 / 2; 7 % 2
来源：http://ndp.fengsongda.top

[A06] 字符串转数字
来源：http://cmw.guowangkeji.top

Py:   int("42"); float("3.14")
来源：http://mth.fehbvm.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://twc.zhijiandao.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nyv.zdbjq.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kub.shuidangran.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pkg.ctjpmb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ngw.hammf.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zcr.birdmap.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dfu.jyoumei.cn

[A07] 数字转字符串
来源：http://dde.52xcode.cn

Py:   str(42)
来源：http://rnv.hesvh.cn

PHP:  (string) 42; strval(42)
来源：http://lit.nanxinkj.top

JS:   String(42); (42).toString()
来源：http://ovf.zhoulong.xyz

TS:   String(42)
来源：http://sen.bbcook.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nij.jianghu66.top

Go:   strconv.Itoa(42)
来源：http://rlb.xuetiantiany.cn

Ruby: 42.to_s
来源：http://xpg.shanyushiyangtech.top

C#:   42.ToString()
来源：http://ilq.fanxiaobao.xyz

[A08] 取整与四舍五入
来源：http://unr.nanxuanxn.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xmj.redwolf501.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vbh.yvedp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ixo.chenzaomai.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fnz.pengpengdd.cyou

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sif.guannengcc.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gtb.aibaodan.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lyw.ywan-chungtsiang.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wut.zhijiandao.cn

[A09] 绝对值与最大最小值
来源：http://bxg.9152youxi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nyw.zhengqikj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yxr.chenjidiqi.icu

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yjh.aizwys.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rhl.mhx1999.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gig.havefunace.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tum.haohaochexian.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tfc.pycfn.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kun.ydzc1.top

[A10] 生成随机数
来源：http://cng.ivvv.top

Py:   import random; random.randint(1, 100)
来源：http://hne.gaohongyu789.top

PHP:  random_int(1, 100);
来源：http://lmo.yvedp.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nin.ivvv.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hom.dashuyun.cn

Java: new Random().nextInt(100) + 1
来源：http://vfx.yangfankeji.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wvr.pycfn.com

Ruby: rand(1..100)
来源：http://vgu.andypj.xyz

C#:   new Random().Next(1, 101)
来源：http://xaa.yangfankeji.com

[A11] 条件表达式（三元）
来源：http://fkj.kuanghao11.cn

Py:   "yes" if x > 0 else "no"
来源：http://omq.kuanghao11.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://gpu.nanxinkj.top

JS:   x > 0 ? "yes" : "no"
来源：http://sdj.jinqigufen.top

TS:   x > 0 ? "yes" : "no"
来源：http://mfj.haohaochexian.top

Java: x > 0 ? "yes" : "no"
来源：http://bmp.ydzc1.top

Go:   // 无三元运算符，需用 if 语句
来源：http://uja.jianghu66.top

Ruby: x > 0 ? "yes" : "no"
来源：http://bpx.haohaochexian.top

C#:   x > 0 ? "yes" : "no"
来源：http://igk.xziqi.cn

[A12] 字符串插值 / 格式化
来源：http://bne.hongshengwenyu.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://agg.fehbvm.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://awi.iojbl.cn

JS:   `Hello, ${name}!`
来源：http://dhi.ydzc1.top

TS:   `Hello, ${name}!`
来源：http://rtn.cheryme.top

Java: "Hello, %s!".formatted(name)
来源：http://zyz.chenjidiqi.icu

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dym.jqgufenzy.top

Ruby: "Hello, #{name}!"
来源：http://yqm.yueranfly.top

C#:   $"Hello, {name}!"
来源：http://vpc.dianchejie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gip.jinqigufen.top

Py:   "第一行\n第二行"
来源：http://coa.zhongyouzk.top

PHP:  "第一行\n第二行"
来源：http://dqx.xingfuxueyuan.xyz

JS:   "第一行\n第二行"
来源：http://suq.yfazqb.com

TS:   "第一行\n第二行"
来源：http://gyn.zhixingplan.top

Java: "第一行\n第二行"
来源：http://rwj.ivvv.top

Go:   "第一行\n第二行"
来源：http://tub.birdmap.top

Ruby: "第一行\n第二行"
来源：http://atr.xziqi.cn

C#:   "第一行\n第二行"
来源：http://hjq.dianchejie.cn

[A14] 注释写法
来源：http://jsc.ehwqpu.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://siw.yuxming.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tgd.hywenlv.cn

JS:   // 单行；/* 多行 */
来源：http://hud.birdmap.top

TS:   // 单行；/* 多行 */
来源：http://xsy.dashuyun.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://syk.yfazqb.com

Go:   // 单行；/* 多行 */
来源：http://lwz.shanyushiyangtech.top

Ruby: # 单行；=begin 多行 =end
来源：http://fwm.tianlin.xyz

C#:   // 单行；/* 多行 */
来源：http://eyj.zhijiandao.cn

[A15] 空值判断与默认值
来源：http://aea.bbcook.cn

Py:   value = data or "默认值"
来源：http://qfs.bjfxy.top

PHP:  $value = $data ?? "默认值";
来源：http://gmh.yueranfly.top

JS:   const value = data ?? "默认值";
来源：http://azv.yonumen.top

TS:   const value = data ?? "默认值";
来源：http://ike.jlsjyb.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cya.yangfankeji.com

Go:   if data == "" { data = "默认值" }
来源：http://ywy.hywenlv.cn

Ruby: value = data || "默认值"
来源：http://yla.tarul.cn

C#:   var value = data ?? "默认值";
来源：http://jjb.fehbvm.com

[A16] 真假值判断规则
来源：http://vfw.gogol.net.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wjx.nanxuanxn.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vuv.iojbl.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ejx.yfazqb.com

TS:   if (!x) {}
来源：http://tqp.ywan-chungtsiang.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wjg.fehbvm.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hvn.tian-w.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yyz.fzhhl.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://czg.yuanzhike.top

[A17] 位运算
来源：http://oyo.ybcxt.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eer.xingfuxueyuan.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jkt.fanxiaobao.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mnh.svipenyu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ful.chenjidiqi.icu

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://phy.meibo888.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vig.shzxlz.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fzl.shanyushiyangtech.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oof.zhixingplan.top

[A18] 字符与 ASCII 码互转
来源：http://xzn.cheryme.top

Py:   ord("A"); chr(65)
来源：http://oim.ppjwa.cn

PHP:  ord("A"); chr(65)
来源：http://kml.tanke756.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tkh.yj20258.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tek.gotoacloud.top

Java: (int) 'A'; (char) 65
来源：http://uil.shzxlz.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zxz.sweek.top

Ruby: "A".ord; 65.chr
来源：http://jgi.chenzaomai.com

C#:   (int)'A'; (char)65
来源：http://rlx.chenjidiqi.icu

[A19] 交换两个变量
来源：http://tsh.zycfv.cn

Py:   a, b = b, a
来源：http://wxs.feifeiyinyue.top

PHP:  [$a, $b] = [$b, $a];
来源：http://coq.yj202588.top

JS:   [a, b] = [b, a];
来源：http://lzo.ehwqpu.com

TS:   [a, b] = [b, a];
来源：http://wgp.iojbl.cn

Java: int t = a; a = b; b = t;
来源：http://aea.bbcook.cn

Go:   a, b = b, a
来源：http://qxr.fzhhl.top

Ruby: a, b = b, a
来源：http://knn.bjfxy.top

C#:   (a, b) = (b, a);
来源：http://vye.daxiang520.top

[A20] 读取标准输入
来源：http://klj.ydjk.org.cn

Py:   name = input("请输入：")
来源：http://fuu.fengsongda.top

PHP:  $name = trim(fgets(STDIN));
来源：http://qxm.sjlbkw.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tey.yongpay.top

TS:   // Node.js：readline 模块
来源：http://hzc.bbcook.cn

Java: new Scanner(System.in).nextLine()
来源：http://fmf.nwbrower.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bwt.cheryme.top

Ruby: gets.chomp
来源：http://dvm.shangyingyoupin.top

C#:   Console.ReadLine();
来源：http://hgz.jinqigfzy.top

[A21] 保留指定小数位输出
来源：http://wxb.hesvh.cn

Py:   f"{3.14159:.2f}"
来源：http://jka.fehbvm.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hrh.cqqwz.cn

JS:   (3.14159).toFixed(2)
来源：http://thm.vehdjk.com

TS:   (3.14159).toFixed(2)
来源：http://tvm.zhoulong.xyz

Java: String.format("%.2f", 3.14159)
来源：http://sxy.guowangkeji.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pqk.52xcode.cn

Ruby: format("%.2f", 3.14159)
来源：http://asv.nwbrower.top

C#:   3.14159.ToString("F2")
来源：http://des.xinyue.icu

[A22] 获取字符串长度
来源：http://wgx.yonumen.top

Py:   len(s)
来源：http://fgt.shanyushiyangkeji.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jzt.haohaochexian.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sho.cucudq.cn

TS:   s.length
来源：http://mex.shzxlz.cn

Java: s.length()
来源：http://zsf.daria6918.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uam.sweek.top

Ruby: s.length
来源：http://sjy.feifeiyinyue.top

C#:   s.Length
来源：http://ptw.yonumen.top

[A23] 大小写转换
来源：http://gth.ehwqpu.com

Py:   s.upper(); s.lower(); s.title()
来源：http://sdz.zdqjudy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tal.fzhhl.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rqz.fzhhl.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ixk.yongpay.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vgt.ywan-chungtsiang.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://azd.ydzc1.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bkl.cheryme.top

C#:   s.ToUpper(); s.ToLower()
来源：http://obc.iojbl.cn

[A24] 去除首尾空白
来源：http://izu.hnxiangtu.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zdo.gotoacloud.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://owg.xuanzx.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yri.nanxuanxn.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lru.ywan-chungtsiang.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://paz.yj20258.top

Go:   strings.TrimSpace(s)
来源：http://wnl.sufxvd.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qij.yj20258888.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://box.gaohongyu789.top

[A25] 字符串比较
来源：http://ets.sxryk.cn

Py:   s1 == s2; s1 != s2
来源：http://rps.fzhhl.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kgn.kuanghao11.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qdl.hnxiangtu.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ljn.shuidangran.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xwt.gotoacloud.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yva.yonumen.top

Ruby: s1 == s2; s1 <=> s2
来源：http://trj.hammf.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qvc.hammf.cn

[A26] 类型转换总览
来源：http://wpw.daria6918.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wtc.sjlbkw.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vix.0kj1m.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vff.fktsv.cn

TS:   Number() String() Boolean() x as number
来源：http://wef.yj20258888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://npr.birdmap.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nuu.quarkkingdee.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://hbj.jqgufenzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qci.hnxiangtu.top

================================================================================
来源：http://jix.shzxlz.cn

B. 流程控制
来源：http://mhw.yangfankeji.com

================================================================================
来源：http://zqh.yangfankeji.com

[B01] 条件判断 if / else
来源：http://gav.hesvh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gce.jlsjyb.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yrr.guowangkeji.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ens.jqgufenzy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vfo.jqgufenzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://mnx.xuanzx.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uqd.jqgufenzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://umw.daxiang520.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://chv.feifeiyinyue.top

[B02] 多分支 else if / elif
来源：http://mdm.chenzaomai.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zjf.aizwys.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wkd.aizwys.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lqw.yongpay.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qey.yanxiufei.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vsk.hesvh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lnh.ppjwa.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://svj.ybcxt.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://swg.ivvv.top

[B03] switch / match / case
来源：http://szv.316326.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jzr.cqqwz.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dkn.sysykeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aqd.zdqjudy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jkw.haohaochexian.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zxa.jinqigufen.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://okt.redwolf501.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cbw.quarkkingdee.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ict.hysaishi.cn

[B04] for 计数循环
来源：http://mct.hongshengwenyu.top

Py:   for i in range(10): print(i)
来源：http://wvr.chenzaomai.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qqg.yj20258.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bsy.jqgufenzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zer.jinqigfzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aze.cashguo.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tnn.feifeiyinyue.top

Ruby: 10.times { |i| puts i }
来源：http://mlg.jinyuanbaomall.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fjr.redwolf501.top

[B05] 遍历数组 / 列表
来源：http://dee.nanxuanxn.top

Py:   for item in arr: print(item)
来源：http://vtx.wangshuangyany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dbh.zhoulong.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://qvw.bbcook.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bmg.jiagoushi.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://zdp.hammf.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lae.xinyue.icu

Ruby: arr.each { |item| puts item }
来源：http://ipt.shanyushiyangtech.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mrs.bbcook.cn

[B06] 遍历字典 / 对象
来源：http://iyz.cqqwz.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fbh.yongpay.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://clj.zhijiandao.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vpk.aizwys.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fls.wangdashe.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pix.jianghu66.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zha.tanke756.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wli.tarul.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://umz.yj20258.top

[B07] while 循环
来源：http://bux.zdqjudy.top

Py:   while i < 10: i += 1
来源：http://huw.shanyushiyangtech.top

PHP:  while ($i < 10) { $i++; }
来源：http://dlf.ppjwa.cn

JS:   while (i < 10) { i++; }
来源：http://fby.jinyuanbaomall.cn

TS:   while (i < 10) { i++; }
来源：http://zkc.jinghuilouyu.cn

Java: while (i < 10) { i++; }
来源：http://zsw.nwbrower.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mzr.jqgufenzy.top

Ruby: while i < 10; i += 1; end
来源：http://umi.316326.xyz

C#:   while (i < 10) { i++; }
来源：http://edn.jinqigfzy.top

[B08] do-while（至少执行一次）
来源：http://ybo.yuanzhike.top

Py:   # 无 do-while：用 while True + break
来源：http://keq.sweek.top

PHP:  do { $i++; } while ($i < 10);
来源：http://twm.yvedp.cn

JS:   do { i++; } while (i < 10);
来源：http://cvf.xuetiantiany.cn

TS:   do { i++; } while (i < 10);
来源：http://dme.shanyushiyangkeji.top

Java: do { i++; } while (i < 10);
来源：http://drq.zhaomingkeji.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://cxd.yj20258.top

Ruby: begin; i += 1; end while i < 10
来源：http://oft.9152youxi.cn

C#:   do { i++; } while (i < 10);
来源：http://zbf.chenzaomai.com

[B09] break 与 continue
来源：http://fcw.birdmap.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://oqo.meibo888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://smz.kuanghao11.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jpw.ydzc1.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yuo.dianchejie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://emr.hnqzz.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dak.nanxinkj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qem.birdmap.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nmd.snrcjt.cn

[B10] 遍历同时拿索引
来源：http://yhe.xingfuxueyuan.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kga.hongshengwenyu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xxk.xuanzx.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xqy.zhaomingkeji.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://czv.ctjpmb.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lvp.uphjek.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dmr.chenjidiqi.icu

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pwv.cheryme.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://daa.hfpthk.cn

[B11] 生成数字序列 / 区间
来源：http://bjy.zdbjq.cn

Py:   list(range(0, 10, 2))
来源：http://ppf.uphjek.com


<!-- 参考信息 -->