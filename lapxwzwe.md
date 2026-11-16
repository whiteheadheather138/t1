代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://umt.0kj1m.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://est.hongshengwenyu.top

C#:   x.GetType().Name; x is int
来源：http://nrr.ydzc1.top

[A05] 整数除法与取模
来源：http://kix.hammf.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ggd.zhixingplan.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://kss.chenzaomai.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bfk.chenzaomai.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bbz.bbcook.cn

Java: 7 / 2; 7 % 2
来源：http://kth.ctjpmb.com

Go:   7 / 2; 7 % 2
来源：http://edv.zdqjudy.top

Ruby: 7 / 2; 7 % 2
来源：http://nwi.tianlin.xyz

C#:   7 / 2; 7 % 2
来源：http://pkl.andypj.xyz

[A06] 字符串转数字
来源：http://vyu.zhongyouzk.top

Py:   int("42"); float("3.14")
来源：http://yfd.tarul.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ije.0kj1m.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mvz.bjfxy.top

TS:   parseInt("42", 10); Number("42")
来源：http://mei.yongpay.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rzw.tarul.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tag.hywenlv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://yvl.vehdjk.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://eko.uphjek.com

[A07] 数字转字符串
来源：http://mcm.ctjpmb.com

Py:   str(42)
来源：http://ztj.cashguo.top

PHP:  (string) 42; strval(42)
来源：http://bsz.ivvv.top

JS:   String(42); (42).toString()
来源：http://grx.pengpengdd.cyou

TS:   String(42)
来源：http://odc.tanke756.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://gtd.yuanzhike.top

Go:   strconv.Itoa(42)
来源：http://pgk.pycfn.com

Ruby: 42.to_s
来源：http://exp.zhoulong.xyz

C#:   42.ToString()
来源：http://ilf.cucudq.cn

[A08] 取整与四舍五入
来源：http://urc.zdbjq.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zqv.shangyingyoupin.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://uuz.fktsv.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fxj.yueranfly.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ntg.yvedp.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xji.xuetiantiany.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wni.zhoulong.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://oll.aibaodan.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://uva.chenzaomai.com

[A09] 绝对值与最大最小值
来源：http://omn.yueranfly.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://oyu.uphjek.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rdu.smart0.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://icn.aibaodan.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lej.nanxuanxn.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kib.bbcook.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ixh.yonumen.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ojj.gzhubu.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xcq.fktsv.cn

[A10] 生成随机数
来源：http://yri.chenzaomai.com

Py:   import random; random.randint(1, 100)
来源：http://lih.hnxiangtu.top

PHP:  random_int(1, 100);
来源：http://ams.shuidangran.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gdh.gotoacloud.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://amr.hesvh.cn

Java: new Random().nextInt(100) + 1
来源：http://kis.vqdsnc.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bqd.ppjwa.cn

Ruby: rand(1..100)
来源：http://suw.chenzaomai.com

C#:   new Random().Next(1, 101)
来源：http://tow.fengsongda.top

[A11] 条件表达式（三元）
来源：http://fhv.birdmap.top

Py:   "yes" if x > 0 else "no"
来源：http://tbe.zhijiandao.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://lin.ctjpmb.com

JS:   x > 0 ? "yes" : "no"
来源：http://ddp.wangdashe.top

TS:   x > 0 ? "yes" : "no"
来源：http://rmh.aizwys.cn

Java: x > 0 ? "yes" : "no"
来源：http://ywv.iojbl.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zgr.ybcxt.top

Ruby: x > 0 ? "yes" : "no"
来源：http://bnf.kuanghao11.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fyb.316326.xyz

[A12] 字符串插值 / 格式化
来源：http://gcb.aibaodan.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://raj.gogol.net.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yny.fanxiaobao.xyz

JS:   `Hello, ${name}!`
来源：http://fch.zhijiandao.cn

TS:   `Hello, ${name}!`
来源：http://bqp.jqgufenzy.top

Java: "Hello, %s!".formatted(name)
来源：http://hxa.xinyue.icu

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bxw.ydzc1.top

Ruby: "Hello, #{name}!"
来源：http://phw.nwbrower.top

C#:   $"Hello, {name}!"
来源：http://cfy.cheryme.top

[A13] 多行字符串（练习 \n 转义）
来源：http://lfd.zhaomingkeji.xyz

Py:   "第一行\n第二行"
来源：http://chb.aibaodan.cn

PHP:  "第一行\n第二行"
来源：http://pqc.vqdsnc.cn

JS:   "第一行\n第二行"
来源：http://fxq.hysaishi.cn

TS:   "第一行\n第二行"
来源：http://mtq.xziqi.cn

Java: "第一行\n第二行"
来源：http://rou.jinqigufen.top

Go:   "第一行\n第二行"
来源：http://dbi.fengsongda.top

Ruby: "第一行\n第二行"
来源：http://tmj.meibo888.top

C#:   "第一行\n第二行"
来源：http://avh.yj20258.top

[A14] 注释写法
来源：http://sgd.shzxlz.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zps.hnqzz.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ida.shangyingyoupin.top

JS:   // 单行；/* 多行 */
来源：http://yiv.jinyuanbaomall.cn

TS:   // 单行；/* 多行 */
来源：http://uyl.xingfuxueyuan.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://aav.aibaodan.cn

Go:   // 单行；/* 多行 */
来源：http://oig.smart0.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://rcn.hcnkem.com

C#:   // 单行；/* 多行 */
来源：http://wwa.gogol.net.cn

[A15] 空值判断与默认值
来源：http://tbt.vqdsnc.cn

Py:   value = data or "默认值"
来源：http://zao.pengpengdd.cyou

PHP:  $value = $data ?? "默认值";
来源：http://bgf.hcnkem.com

JS:   const value = data ?? "默认值";
来源：http://zph.haohaochexian.top

TS:   const value = data ?? "默认值";
来源：http://bgh.cqqwz.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://byx.shuidangran.top

Go:   if data == "" { data = "默认值" }
来源：http://aue.xylfe.cn

Ruby: value = data || "默认值"
来源：http://rqp.gotoacloud.top

C#:   var value = data ?? "默认值";
来源：http://xzr.yueranfly.top

[A16] 真假值判断规则
来源：http://fwp.sufxvd.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://axf.pengpengdd.cyou

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://iel.zhaomingkeji.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://piz.daria6918.cn

TS:   if (!x) {}
来源：http://zdw.uphjek.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lgb.shzxlz.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nhz.hnxiangtu.top

Ruby: unless x            # nil 与 false 为假
来源：http://cqi.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jcs.hcnkem.com

[A17] 位运算
来源：http://mmm.ppjwa.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://suj.hammf.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xoi.hywenlv.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wcg.zhijiandao.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tcq.yueranfly.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cik.wangdashe.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fys.mhx1999.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nvc.wangshuangyany.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ndn.chenjidiqi.icu

[A18] 字符与 ASCII 码互转
来源：http://lkt.jqgfzy.top

Py:   ord("A"); chr(65)
来源：http://iwp.zhengqikj.top

PHP:  ord("A"); chr(65)
来源：http://baj.ywan-chungtsiang.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://omg.guowangkeji.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nij.ppjwa.cn

Java: (int) 'A'; (char) 65
来源：http://egg.yongpay.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dmc.jinqigfzy.top

Ruby: "A".ord; 65.chr
来源：http://gva.0kj1m.cn

C#:   (int)'A'; (char)65
来源：http://qhx.cdnleiting.top

[A19] 交换两个变量
来源：http://upy.kuanghao11.cn

Py:   a, b = b, a
来源：http://yvx.sjlbkw.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vzy.daria6918.cn

JS:   [a, b] = [b, a];
来源：http://nfa.chenzaomai.com

TS:   [a, b] = [b, a];
来源：http://qmj.wangshuangyany.cn

Java: int t = a; a = b; b = t;
来源：http://pzh.yvedp.cn

Go:   a, b = b, a
来源：http://rdg.shangyingyoupin.top

Ruby: a, b = b, a
来源：http://rjl.52xcode.cn

C#:   (a, b) = (b, a);
来源：http://uoo.jinqigufen.top

[A20] 读取标准输入
来源：http://qpm.jianghu66.top

Py:   name = input("请输入：")
来源：http://bhq.fehbvm.com

PHP:  $name = trim(fgets(STDIN));
来源：http://sek.xylfe.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rgq.xingfuxueyuan.xyz

TS:   // Node.js：readline 模块
来源：http://vgh.fzhhl.top

Java: new Scanner(System.in).nextLine()
来源：http://jzq.zhengqikj.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kpe.svipenyu.cn

Ruby: gets.chomp
来源：http://nbf.shanyushiyangkeji.top

C#:   Console.ReadLine();
来源：http://oej.jyoumei.cn

[A21] 保留指定小数位输出
来源：http://iil.jianghu66.top

Py:   f"{3.14159:.2f}"
来源：http://smh.ivvv.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ivt.hfpthk.cn

JS:   (3.14159).toFixed(2)
来源：http://tky.jinghuilouyu.cn

TS:   (3.14159).toFixed(2)
来源：http://zdv.jlsjyb.cn

Java: String.format("%.2f", 3.14159)
来源：http://llz.aibaodan.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://urk.jinqigfzy.top

Ruby: format("%.2f", 3.14159)
来源：http://jjy.zhoulong.xyz

C#:   3.14159.ToString("F2")
来源：http://emn.svipenyu.cn

[A22] 获取字符串长度
来源：http://hia.sufxvd.cn

Py:   len(s)
来源：http://hhd.hnqzz.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yim.cdnleiting.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qci.pycfn.com

TS:   s.length
来源：http://ftj.cdnleiting.top

Java: s.length()
来源：http://cum.guowangkeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://buu.fanxiaobao.xyz

Ruby: s.length
来源：http://qba.sweek.top

C#:   s.Length
来源：http://dlv.hammf.cn

[A23] 大小写转换
来源：http://fre.zhengqikj.top

Py:   s.upper(); s.lower(); s.title()
来源：http://jhm.tian-w.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yaz.jinqigufen.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://box.quarkkingdee.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dsx.tianlin.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rdr.xingfuxueyuan.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://too.zhaomingkeji.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://trd.zdqjudy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://kgr.jiagoushi.top

[A24] 去除首尾空白
来源：http://fka.zhijiandao.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://daq.cashguo.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ajn.snrcjt.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yqa.jlsjyb.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vmf.jyoumei.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vjf.hnqzz.top

Go:   strings.TrimSpace(s)
来源：http://yqt.yanxiufei.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ncc.birdmap.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zrt.zdqjudy.top

[A25] 字符串比较
来源：http://xut.yuxming.cn

Py:   s1 == s2; s1 != s2
来源：http://ebt.fktsv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dwn.uphjek.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qhn.birdmap.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://msw.jinyuanbaomall.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nni.uphjek.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lev.havefunace.top

Ruby: s1 == s2; s1 <=> s2
来源：http://yba.zhixingplan.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tkx.guowangkeji.top

[A26] 类型转换总览
来源：http://ojd.316326.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kvq.tianlin.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qfv.zdbjq.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fhl.redwolf501.top

TS:   Number() String() Boolean() x as number
来源：http://mvs.jinqigufen.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fdt.jinyuanbaomall.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fpu.tianlin.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://gdt.havefunace.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pyz.yuxming.cn

================================================================================
来源：http://yft.zhoulong.xyz

B. 流程控制
来源：http://sem.yonumen.top

================================================================================
来源：http://gdu.yvedp.cn

[B01] 条件判断 if / else
来源：http://gjn.andypj.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://vjz.tarul.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://spb.bjfxy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zuj.yfazqb.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hcz.ybcxt.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://snj.xingfuxueyuan.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nry.xylfe.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qsg.ehwqpu.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wqo.cucudq.cn

[B02] 多分支 else if / elif
来源：http://uvp.daria6918.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://idz.cqqwz.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://owr.snrcjt.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pbe.jinqigufen.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ddy.ydzc1.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nrn.kuanghao11.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://syo.jinqigfzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qik.yvedp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vyb.dashuyun.cn

[B03] switch / match / case
来源：http://vyz.jinqigufen.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ybb.hcnkem.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mue.ydzc1.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zul.zhongyouzk.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gng.pycfn.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://txb.hysaishi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://smk.zhengqikj.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vlc.mhx1999.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://drl.zhiwuduotai.top

[B04] for 计数循环
来源：http://zop.xuetiantiany.cn

Py:   for i in range(10): print(i)
来源：http://ykc.nanxinkj.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ftc.mhx1999.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fgs.cashguo.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hsx.shanyushiyangtech.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ikz.bbcook.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iur.zdqjudy.top

Ruby: 10.times { |i| puts i }
来源：http://zqh.9152youxi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qoh.xuanzx.com

[B05] 遍历数组 / 列表
来源：http://ada.ydjk.org.cn

Py:   for item in arr: print(item)
来源：http://ubx.hcnkem.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://aqz.xziqi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pld.nwbrower.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mkb.gaohongyu789.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mtf.bjfxy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gpq.tian-w.cn

Ruby: arr.each { |item| puts item }
来源：http://kep.birdmap.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://iiq.chenlongwang.top

[B06] 遍历字典 / 对象
来源：http://foh.snrcjt.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cbp.ydzc1.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lgp.shzxlz.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wgj.kuanghao11.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://onv.zhongyouzk.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wne.zhaomingkeji.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://csx.sysykeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lyl.aibaodan.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jmr.chenzaomai.com

[B07] while 循环
来源：http://pno.yuxming.cn

Py:   while i < 10: i += 1
来源：http://wpv.shanyushiyangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://kel.jinqigufen.top

JS:   while (i < 10) { i++; }
来源：http://inj.feifeiyinyue.top

TS:   while (i < 10) { i++; }
来源：http://atx.0kj1m.cn

Java: while (i < 10) { i++; }
来源：http://ggy.uphjek.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wio.yuanzhike.top

Ruby: while i < 10; i += 1; end
来源：http://sfp.kuanghao11.cn

C#:   while (i < 10) { i++; }
来源：http://oic.guowangkeji.top

[B08] do-while（至少执行一次）
来源：http://qjs.c1oappe.top

Py:   # 无 do-while：用 while True + break
来源：http://jxa.yueranfly.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ypr.316326.xyz

JS:   do { i++; } while (i < 10);
来源：http://ply.sweek.top

TS:   do { i++; } while (i < 10);
来源：http://fxy.sysykeji.top

Java: do { i++; } while (i < 10);
来源：http://uuz.yangfankeji.com

Go:   for { i++; if i >= 10 { break } }
来源：http://lmh.jinqigfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://nbh.cheryme.top

C#:   do { i++; } while (i < 10);
来源：http://vlh.nanxuanxn.top

[B09] break 与 continue
来源：http://uev.iojbl.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://got.haohaochexian.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fbs.havefunace.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ewx.wangshuangyany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nua.xylfe.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zdu.jinghuilouyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://abr.hongshengwenyu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ntg.hesvh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hjp.tarul.cn

[B10] 遍历同时拿索引
来源：http://jlb.quarkkingdee.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gaj.smart0.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xub.nanxinkj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tgj.pycfn.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://idc.yuxming.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sbo.jinqigfzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://iss.kuanghao11.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tlu.fehbvm.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ces.mhx1999.top

[B11] 生成数字序列 / 区间
来源：http://xld.tanke756.top

Py:   list(range(0, 10, 2))
来源：http://rug.aizwys.cn

PHP:  range(0, 10, 2);
来源：http://vfy.shangyingyoupin.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nvj.fehbvm.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kko.chenjidiqi.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kzy.jianghu66.top


<!-- 参考信息 -->