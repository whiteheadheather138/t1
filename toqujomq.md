代发 wailian999

[A06] 字符串转数字
来源：http://liy.dianchejie.cn

Py:   int("42"); float("3.14")
来源：http://nfr.ybcxt.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yhs.zycfv.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cmt.hcnkem.com

TS:   parseInt("42", 10); Number("42")
来源：http://bfc.zdbjq.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kbn.zhengqikj.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wgl.epnwcf.com

Ruby: "42".to_i; "3.14".to_f
来源：http://zne.iojbl.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zaa.pengpengdd.cyou

[A07] 数字转字符串
来源：http://xul.jinghuilouyu.cn

Py:   str(42)
来源：http://khj.yj20258888.top

PHP:  (string) 42; strval(42)
来源：http://jgc.yonumen.top

JS:   String(42); (42).toString()
来源：http://kzn.cdnleiting.top

TS:   String(42)
来源：http://gar.hysaishi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vnq.shanyushiyangkeji.top

Go:   strconv.Itoa(42)
来源：http://bio.zhijiandao.cn

Ruby: 42.to_s
来源：http://hiy.xylfe.cn

C#:   42.ToString()
来源：http://ldv.yj20258.top

[A08] 取整与四舍五入
来源：http://rif.jinyuanbaomall.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://oxp.hammf.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ejb.shzxlz.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hbl.shuidangran.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://uuj.ywan-chungtsiang.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fxr.ehwqpu.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zfw.sjlbkw.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://rsc.jiagoushi.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xzl.dianchejie.cn

[A09] 绝对值与最大最小值
来源：http://lbd.sufxvd.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wze.xuanzx.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dks.shzxlz.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ndj.zhengqikj.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hno.cheryme.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ldw.meibo888.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://oex.hnxiangtu.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://eap.aizwys.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wkx.uphjek.com

[A10] 生成随机数
来源：http://flo.andypj.xyz

Py:   import random; random.randint(1, 100)
来源：http://jjf.yueranfly.top

PHP:  random_int(1, 100);
来源：http://xku.zdqjudy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://toh.jinqigfzy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zud.gzhubu.top

Java: new Random().nextInt(100) + 1
来源：http://ndg.chenlongwang.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tbd.hongshengwenyu.top

Ruby: rand(1..100)
来源：http://aij.zhongyouzk.top

C#:   new Random().Next(1, 101)
来源：http://fto.yj202588.top

[A11] 条件表达式（三元）
来源：http://htl.chenjidiqi.icu

Py:   "yes" if x > 0 else "no"
来源：http://omo.hongshengwenyu.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://jrc.wangshuangyany.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jcg.chenzaomai.com

TS:   x > 0 ? "yes" : "no"
来源：http://emy.gaohongyu789.top

Java: x > 0 ? "yes" : "no"
来源：http://qdu.jyoumei.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hdy.yj20258888.top

Ruby: x > 0 ? "yes" : "no"
来源：http://gjr.yueranfly.top

C#:   x > 0 ? "yes" : "no"
来源：http://npk.gzhubu.top

[A12] 字符串插值 / 格式化
来源：http://dho.yonumen.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qmr.xinyue.icu

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zrl.pycfn.com

JS:   `Hello, ${name}!`
来源：http://kiu.ydzc1.top

TS:   `Hello, ${name}!`
来源：http://pfn.zycfv.cn

Java: "Hello, %s!".formatted(name)
来源：http://fkh.yj20258.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mbn.uphjek.com

Ruby: "Hello, #{name}!"
来源：http://mkw.zhixingplan.top

C#:   $"Hello, {name}!"
来源：http://aji.fehbvm.com

[A13] 多行字符串（练习 \n 转义）
来源：http://xuu.tarul.cn

Py:   "第一行\n第二行"
来源：http://neq.shanyushiyangkeji.top

PHP:  "第一行\n第二行"
来源：http://wmh.jinqigufen.top

JS:   "第一行\n第二行"
来源：http://pfj.hcnkem.com

TS:   "第一行\n第二行"
来源：http://uyk.daxiang520.top

Java: "第一行\n第二行"
来源：http://ios.shanyushiyangtech.top

Go:   "第一行\n第二行"
来源：http://faf.jinqigfzy.top

Ruby: "第一行\n第二行"
来源：http://okt.316326.xyz

C#:   "第一行\n第二行"
来源：http://sdw.fanxiaobao.xyz

[A14] 注释写法
来源：http://mbk.fktsv.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://lgm.yuxming.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://pto.jyoumei.cn

JS:   // 单行；/* 多行 */
来源：http://tqu.xuanzx.com

TS:   // 单行；/* 多行 */
来源：http://ipd.nanxuanxn.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dsm.quarkkingdee.top

Go:   // 单行；/* 多行 */
来源：http://qbz.sufxvd.cn

Ruby: # 单行；=begin 多行 =end
来源：http://czx.jinghuilouyu.cn

C#:   // 单行；/* 多行 */
来源：http://cag.jqgufenzy.top

[A15] 空值判断与默认值
来源：http://fbt.ctjpmb.com

Py:   value = data or "默认值"
来源：http://cha.bjfxy.top

PHP:  $value = $data ?? "默认值";
来源：http://tzy.gaohongyu789.top

JS:   const value = data ?? "默认值";
来源：http://awu.yj20258.top

TS:   const value = data ?? "默认值";
来源：http://xpy.jinghuilouyu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vjc.shzxlz.cn

Go:   if data == "" { data = "默认值" }
来源：http://uxy.cucudq.cn

Ruby: value = data || "默认值"
来源：http://jtg.shanyushiyangkeji.top

C#:   var value = data ?? "默认值";
来源：http://zqg.jlsjyb.cn

[A16] 真假值判断规则
来源：http://bvj.meibo888.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gkq.0kj1m.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jtq.mhx1999.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://umn.gotoacloud.top

TS:   if (!x) {}
来源：http://day.ctjpmb.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ljp.mhx1999.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ojg.zycfv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://okg.hnqzz.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://eok.xingfuxueyuan.xyz

[A17] 位运算
来源：http://ezr.daria6918.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hvz.aibaodan.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zmy.aibaodan.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://clw.jinqigfzy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vpw.meibo888.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vuy.guannengcc.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zjx.ppjwa.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qju.yuxming.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ftq.52xcode.cn

[A18] 字符与 ASCII 码互转
来源：http://qyq.havefunace.top

Py:   ord("A"); chr(65)
来源：http://xpb.52xcode.cn

PHP:  ord("A"); chr(65)
来源：http://lhw.gogol.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jfe.jqgfzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hgq.fehbvm.com

Java: (int) 'A'; (char) 65
来源：http://pum.yfazqb.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gwj.hnxiangtu.top

Ruby: "A".ord; 65.chr
来源：http://ovp.fanxiaobao.xyz

C#:   (int)'A'; (char)65
来源：http://xum.zhiwuduotai.top

[A19] 交换两个变量
来源：http://gdo.meibo888.top

Py:   a, b = b, a
来源：http://wrj.hysaishi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nrv.cashguo.top

JS:   [a, b] = [b, a];
来源：http://aox.birdmap.top

TS:   [a, b] = [b, a];
来源：http://vlw.bbcook.cn

Java: int t = a; a = b; b = t;
来源：http://ojp.cucudq.cn

Go:   a, b = b, a
来源：http://lkn.aizwys.cn

Ruby: a, b = b, a
来源：http://dru.chenlongwang.top

C#:   (a, b) = (b, a);
来源：http://mlf.shanyushiyangtech.top

[A20] 读取标准输入
来源：http://kfj.tarul.cn

Py:   name = input("请输入：")
来源：http://hqd.sufxvd.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://umq.xuetiantiany.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gzj.ctjpmb.com

TS:   // Node.js：readline 模块
来源：http://cpz.hammf.cn

Java: new Scanner(System.in).nextLine()
来源：http://enb.guannengcc.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gke.shzxlz.cn

Ruby: gets.chomp
来源：http://hpd.aizwys.cn

C#:   Console.ReadLine();
来源：http://rdj.nwbrower.top

[A21] 保留指定小数位输出
来源：http://xxy.gogol.net.cn

Py:   f"{3.14159:.2f}"
来源：http://wpw.sjlbkw.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://uhs.haohaochexian.top

JS:   (3.14159).toFixed(2)
来源：http://nwi.yanxiufei.cn

TS:   (3.14159).toFixed(2)
来源：http://uko.sjlbkw.cn

Java: String.format("%.2f", 3.14159)
来源：http://cwr.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://akj.yvedp.cn

Ruby: format("%.2f", 3.14159)
来源：http://fod.aibaodan.cn

C#:   3.14159.ToString("F2")
来源：http://uqd.mhx1999.top

[A22] 获取字符串长度
来源：http://ody.yj20258.top

Py:   len(s)
来源：http://yfc.sweek.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ydv.zhengqikj.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qzz.shzxlz.cn

TS:   s.length
来源：http://eph.mhx1999.top

Java: s.length()
来源：http://mlo.pycfn.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://otb.wangdashe.top

Ruby: s.length
来源：http://tau.yuxming.cn

C#:   s.Length
来源：http://gpq.yanxiufei.cn

[A23] 大小写转换
来源：http://aou.tanke756.top

Py:   s.upper(); s.lower(); s.title()
来源：http://dal.yvedp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cyp.sufxvd.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nbe.hammf.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jli.yangfankeji.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dkb.cheryme.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://imm.jqgfzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dzg.jqgfzy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://aok.guannengcc.top

[A24] 去除首尾空白
来源：http://rpq.shangyingyoupin.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lgf.nanxinkj.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vgs.zhiwuduotai.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yek.yanxiufei.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ofe.wangshuangyany.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nvw.cucudq.cn

Go:   strings.TrimSpace(s)
来源：http://jyz.tanke756.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yug.bjfxy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bre.jinqigfzy.top

[A25] 字符串比较
来源：http://gif.fzhhl.top

Py:   s1 == s2; s1 != s2
来源：http://ikd.sysykeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dei.chenzaomai.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ghl.shzxlz.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://stz.nwbrower.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dtt.pengpengdd.cyou

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ets.zhixingplan.top

Ruby: s1 == s2; s1 <=> s2
来源：http://rsk.jlsjyb.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gil.svipenyu.cn

[A26] 类型转换总览
来源：http://vqs.uphjek.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pqg.chenlongwang.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pxg.cheryme.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zgq.52xcode.cn

TS:   Number() String() Boolean() x as number
来源：http://akr.cucudq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://thp.dashuyun.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nwp.birdmap.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://hzp.hongshengwenyu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mov.shangyingyoupin.top

================================================================================
来源：http://crq.ywan-chungtsiang.top

B. 流程控制
来源：http://fvb.andypj.xyz

================================================================================
来源：http://czg.sufxvd.cn

[B01] 条件判断 if / else
来源：http://nje.c1oappe.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ykw.hfpthk.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nhb.yangfankeji.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cwz.ywan-chungtsiang.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kga.yonumen.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://oop.ydjk.org.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gwu.xziqi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qnl.9152youxi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xtk.vqdsnc.cn

[B02] 多分支 else if / elif
来源：http://opk.fktsv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lvc.hywenlv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cpi.xziqi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zvb.jlsjyb.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://olo.fanxiaobao.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zqt.yongpay.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jpi.c1oappe.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zjc.iojbl.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bww.sufxvd.cn

[B03] switch / match / case
来源：http://kbu.fktsv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zjx.zhoulong.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cwz.cdnleiting.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nrv.yfazqb.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yhq.zhixingplan.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://shy.xziqi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cux.hywenlv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dvu.vehdjk.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ufo.bbcook.cn

[B04] for 计数循环
来源：http://vum.zhixingplan.top

Py:   for i in range(10): print(i)
来源：http://ujn.yangfankeji.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rth.fehbvm.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qlx.zhixingplan.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xnt.ivvv.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zrj.zycfv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bwk.316326.xyz

Ruby: 10.times { |i| puts i }
来源：http://jfo.zycfv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jjn.ywan-chungtsiang.top

[B05] 遍历数组 / 列表
来源：http://trk.jqgfzy.top

Py:   for item in arr: print(item)
来源：http://zhk.zhongyouzk.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qvp.guowangkeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://bnz.dashuyun.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ilr.cheryme.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ltf.hongshengwenyu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dbz.tianlin.xyz

Ruby: arr.each { |item| puts item }
来源：http://keb.xylfe.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zho.zdqjudy.top

[B06] 遍历字典 / 对象
来源：http://xhg.shanyushiyangtech.top

Py:   for k, v in d.items(): print(k, v)
来源：http://noq.cqqwz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://srl.xylfe.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hsv.pengpengdd.cyou

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nsg.zhongyouzk.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ygw.c1oappe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pqm.hammf.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xzg.svipenyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://joi.yanxiufei.cn

[B07] while 循环
来源：http://xwr.yueranfly.top

Py:   while i < 10: i += 1
来源：http://hbk.hnxiangtu.top

PHP:  while ($i < 10) { $i++; }
来源：http://zok.yfazqb.com

JS:   while (i < 10) { i++; }
来源：http://cte.smart0.xyz

TS:   while (i < 10) { i++; }
来源：http://adi.shanyushiyangkeji.top

Java: while (i < 10) { i++; }
来源：http://obw.aizwys.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rbs.aizwys.cn

Ruby: while i < 10; i += 1; end
来源：http://lkp.pengpengdd.cyou

C#:   while (i < 10) { i++; }
来源：http://nrz.jqgufenzy.top

[B08] do-while（至少执行一次）
来源：http://uzj.guowangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://xaq.sxryk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zzn.andypj.xyz

JS:   do { i++; } while (i < 10);
来源：http://uiu.sysykeji.top

TS:   do { i++; } while (i < 10);
来源：http://lyk.jlsjyb.cn

Java: do { i++; } while (i < 10);
来源：http://ydr.dianchejie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yst.jinqigfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://zvr.gogol.net.cn

C#:   do { i++; } while (i < 10);
来源：http://yoq.xingfuxueyuan.xyz

[B09] break 与 continue
来源：http://pbf.yonumen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kfd.hysaishi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mwx.wangshuangyany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://chk.birdmap.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://exe.cucudq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qof.jqgfzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wjd.svipenyu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yrz.zhengqikj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vzx.ybcxt.top

[B10] 遍历同时拿索引
来源：http://jzk.shangyingyoupin.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fdw.chenjidiqi.icu

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rzb.shanyushiyangtech.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wtr.jinqigfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://snx.9152youxi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zku.hongshengwenyu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://eam.jqgfzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iqo.yuxming.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vpr.xziqi.cn

[B11] 生成数字序列 / 区间
来源：http://fyg.xuanzx.com

Py:   list(range(0, 10, 2))
来源：http://fgh.zhengqikj.top

PHP:  range(0, 10, 2);
来源：http://lnv.9152youxi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://juh.smart0.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ebw.jinghuilouyu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wfs.fengsongda.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bnj.shangyingyoupin.top

Ruby: (0...10).step(2).to_a
来源：http://zbn.0kj1m.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xac.ybcxt.top

[B12] 跳出多层循环
来源：http://vzz.yj20258888.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qwl.hesvh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lpg.zdbjq.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ydk.jiagoushi.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ugr.haohaochexian.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://try.sufxvd.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mxj.vehdjk.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nam.0kj1m.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oun.xingfuxueyuan.xyz


<!-- 参考信息 -->