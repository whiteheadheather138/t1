代发 wailian999

[A06] 字符串转数字
来源：http://vov.nanxinkj.top

Py:   int("42"); float("3.14")
来源：http://eye.iojbl.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://enq.iojbl.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://spj.zdbjq.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qvf.cashguo.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://iiu.smart0.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://iiq.sufxvd.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fnv.tanke756.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jss.zhijiandao.cn

[A07] 数字转字符串
来源：http://oon.sysykeji.top

Py:   str(42)
来源：http://plb.zhongyouzk.top

PHP:  (string) 42; strval(42)
来源：http://sap.yuanzhike.top

JS:   String(42); (42).toString()
来源：http://qjo.cucudq.cn

TS:   String(42)
来源：http://snd.cheryme.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://svl.andypj.xyz

Go:   strconv.Itoa(42)
来源：http://jwd.aibaodan.cn

Ruby: 42.to_s
来源：http://tob.hfpthk.cn

C#:   42.ToString()
来源：http://rwu.dashuyun.cn

[A08] 取整与四舍五入
来源：http://rbg.yvedp.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fqs.pycfn.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wca.zycfv.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://uvf.jiagoushi.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xkn.hywenlv.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mip.jinghuilouyu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kqi.jqgfzy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://zxl.yj20258888.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zyq.fzhhl.top

[A09] 绝对值与最大最小值
来源：http://rcb.zhijiandao.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://uur.chenzaomai.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xsb.yueranfly.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dkt.jqgufenzy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uma.xinyue.icu

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vry.gzhubu.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://flf.shanyushiyangtech.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tig.hongshengwenyu.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bsg.sufxvd.cn

[A10] 生成随机数
来源：http://rwh.ehwqpu.com

Py:   import random; random.randint(1, 100)
来源：http://ecl.zhongyouzk.top

PHP:  random_int(1, 100);
来源：http://eds.hnxiangtu.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vql.ehwqpu.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rnb.xuanzx.com

Java: new Random().nextInt(100) + 1
来源：http://hkh.hesvh.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zer.tanke756.top

Ruby: rand(1..100)
来源：http://lob.fzhhl.top

C#:   new Random().Next(1, 101)
来源：http://ctf.xingfuxueyuan.xyz

[A11] 条件表达式（三元）
来源：http://suj.yj202588.top

Py:   "yes" if x > 0 else "no"
来源：http://del.fzhhl.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://nme.ppjwa.cn

JS:   x > 0 ? "yes" : "no"
来源：http://png.yongpay.top

TS:   x > 0 ? "yes" : "no"
来源：http://uen.yongpay.top

Java: x > 0 ? "yes" : "no"
来源：http://hkt.jqgfzy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ddk.dashuyun.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://yfh.zdbjq.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lbm.daria6918.cn

[A12] 字符串插值 / 格式化
来源：http://pzq.ivvv.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://chr.nwbrower.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://axm.hnxiangtu.top

JS:   `Hello, ${name}!`
来源：http://xmf.daxiang520.top

TS:   `Hello, ${name}!`
来源：http://idd.uphjek.com

Java: "Hello, %s!".formatted(name)
来源：http://mgc.xuetiantiany.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tuu.svipenyu.cn

Ruby: "Hello, #{name}!"
来源：http://xvb.shzxlz.cn

C#:   $"Hello, {name}!"
来源：http://oza.yanxiufei.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zdq.pengpengdd.cyou

Py:   "第一行\n第二行"
来源：http://cxm.aibaodan.cn

PHP:  "第一行\n第二行"
来源：http://izm.xylfe.cn

JS:   "第一行\n第二行"
来源：http://cgd.ivvv.top

TS:   "第一行\n第二行"
来源：http://wxr.tarul.cn

Java: "第一行\n第二行"
来源：http://qvx.dashuyun.cn

Go:   "第一行\n第二行"
来源：http://gek.xziqi.cn

Ruby: "第一行\n第二行"
来源：http://rfm.vehdjk.com

C#:   "第一行\n第二行"
来源：http://hbw.zhijiandao.cn

[A14] 注释写法
来源：http://ozu.xuanzx.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://hfr.havefunace.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://lvo.jqgfzy.top

JS:   // 单行；/* 多行 */
来源：http://dju.vqdsnc.cn

TS:   // 单行；/* 多行 */
来源：http://ldy.sysykeji.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ozx.fanxiaobao.xyz

Go:   // 单行；/* 多行 */
来源：http://xau.tianlin.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://kli.9152youxi.cn

C#:   // 单行；/* 多行 */
来源：http://xaq.shanyushiyangkeji.top

[A15] 空值判断与默认值
来源：http://yon.zhengqikj.top

Py:   value = data or "默认值"
来源：http://kjb.jlsjyb.cn

PHP:  $value = $data ?? "默认值";
来源：http://uyi.nanxinkj.top

JS:   const value = data ?? "默认值";
来源：http://fzz.jqgfzy.top

TS:   const value = data ?? "默认值";
来源：http://qwh.fzhhl.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vze.jqgufenzy.top

Go:   if data == "" { data = "默认值" }
来源：http://wcu.sufxvd.cn

Ruby: value = data || "默认值"
来源：http://ueu.hysaishi.cn

C#:   var value = data ?? "默认值";
来源：http://xiu.ywan-chungtsiang.top

[A16] 真假值判断规则
来源：http://byc.guannengcc.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ikf.hnqzz.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dal.meibo888.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jbt.jqgufenzy.top

TS:   if (!x) {}
来源：http://ptx.meibo888.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dsc.zdbjq.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bgu.0kj1m.cn

Ruby: unless x            # nil 与 false 为假
来源：http://adb.daria6918.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vpj.yanxiufei.cn

[A17] 位运算
来源：http://pkt.yueranfly.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gcb.meibo888.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lyr.haohaochexian.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bkw.ydjk.org.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ujn.jinqigfzy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zyk.andypj.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vyp.cashguo.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jdt.xuanzx.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ftd.sjlbkw.cn

[A18] 字符与 ASCII 码互转
来源：http://mzb.sufxvd.cn

Py:   ord("A"); chr(65)
来源：http://kfs.shanyushiyangtech.top

PHP:  ord("A"); chr(65)
来源：http://bqp.andypj.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dfr.wangdashe.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://loq.sysykeji.top

Java: (int) 'A'; (char) 65
来源：http://olb.yvedp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://scj.chenlongwang.top

Ruby: "A".ord; 65.chr
来源：http://caz.smart0.xyz

C#:   (int)'A'; (char)65
来源：http://ohf.cucudq.cn

[A19] 交换两个变量
来源：http://wwe.c1oappe.top

Py:   a, b = b, a
来源：http://qcq.vqdsnc.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://dkx.jinqigfzy.top

JS:   [a, b] = [b, a];
来源：http://nbk.hfpthk.cn

TS:   [a, b] = [b, a];
来源：http://bht.zycfv.cn

Java: int t = a; a = b; b = t;
来源：http://vvy.wangshuangyany.cn

Go:   a, b = b, a
来源：http://lly.hnxiangtu.top

Ruby: a, b = b, a
来源：http://ckf.yj20258.top

C#:   (a, b) = (b, a);
来源：http://tvs.hnxiangtu.top

[A20] 读取标准输入
来源：http://ayd.tianlin.xyz

Py:   name = input("请输入：")
来源：http://stv.smart0.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://nzh.yonumen.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nra.gotoacloud.top

TS:   // Node.js：readline 模块
来源：http://qrg.xuanzx.com

Java: new Scanner(System.in).nextLine()
来源：http://hjx.hnxiangtu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://faj.yanxiufei.cn

Ruby: gets.chomp
来源：http://fua.meibo888.top

C#:   Console.ReadLine();
来源：http://ikh.shanyushiyangkeji.top

[A21] 保留指定小数位输出
来源：http://lyz.hcnkem.com

Py:   f"{3.14159:.2f}"
来源：http://voh.bbcook.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bec.ivvv.top

JS:   (3.14159).toFixed(2)
来源：http://esf.yuxming.cn

TS:   (3.14159).toFixed(2)
来源：http://yyw.gaohongyu789.top

Java: String.format("%.2f", 3.14159)
来源：http://pqo.zhijiandao.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nsf.0kj1m.cn

Ruby: format("%.2f", 3.14159)
来源：http://lqf.nanxuanxn.top

C#:   3.14159.ToString("F2")
来源：http://oaw.yvedp.cn

[A22] 获取字符串长度
来源：http://jgh.fktsv.cn

Py:   len(s)
来源：http://ssp.jinqigufen.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bzf.jqgufenzy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wgx.meibo888.top

TS:   s.length
来源：http://rfl.shangyingyoupin.top

Java: s.length()
来源：http://tdt.jqgfzy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ddm.cucudq.cn

Ruby: s.length
来源：http://cnm.yueranfly.top

C#:   s.Length
来源：http://cem.guowangkeji.top

[A23] 大小写转换
来源：http://qup.zdqjudy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wdk.xuanzx.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qgm.guowangkeji.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kyh.havefunace.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jct.yangfankeji.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yib.yueranfly.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dlz.cucudq.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kps.yanxiufei.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tyo.nwbrower.top

[A24] 去除首尾空白
来源：http://paf.hammf.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zzh.ywan-chungtsiang.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://acx.fehbvm.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dvo.zhaomingkeji.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yqi.sxryk.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tmj.xinyue.icu

Go:   strings.TrimSpace(s)
来源：http://ejb.yueranfly.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gpm.zdqjudy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ltv.xuetiantiany.cn

[A25] 字符串比较
来源：http://ebb.nwbrower.top

Py:   s1 == s2; s1 != s2
来源：http://ckf.yj202588.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dmj.jinqigufen.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bge.nwbrower.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vbs.gotoacloud.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cwz.pycfn.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zzh.gogol.net.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://aaf.gaohongyu789.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xue.nanxinkj.top

[A26] 类型转换总览
来源：http://hre.uphjek.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pza.aibaodan.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ded.zhixingplan.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://arg.ywan-chungtsiang.top

TS:   Number() String() Boolean() x as number
来源：http://prs.ybcxt.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zwm.zhijiandao.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dsp.316326.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://var.ehwqpu.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mqa.pycfn.com

================================================================================
来源：http://xkr.shuidangran.top

B. 流程控制
来源：http://ygx.jinqigufen.top

================================================================================
来源：http://pdf.316326.xyz

[B01] 条件判断 if / else
来源：http://gjl.jyoumei.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ofz.shzxlz.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hlb.daxiang520.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ork.yangfankeji.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://djx.ybcxt.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://woy.gotoacloud.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fcg.hcnkem.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fse.cashguo.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fut.jlsjyb.cn

[B02] 多分支 else if / elif
来源：http://dev.xziqi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://srn.hongshengwenyu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lil.bbcook.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fod.iojbl.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://olr.zdbjq.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zrf.chenjidiqi.icu

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://itq.ehwqpu.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qot.hnxiangtu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gxk.mhx1999.top

[B03] switch / match / case
来源：http://keo.yueranfly.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://auk.tarul.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://czk.yj202588.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jwn.aizwys.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://npd.sxryk.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://abi.ctjpmb.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://apr.cheryme.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hxb.snrcjt.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hpo.fzhhl.top

[B04] for 计数循环
来源：http://kgp.jinqigfzy.top

Py:   for i in range(10): print(i)
来源：http://voh.chenjidiqi.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://phq.yonumen.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kbu.yj20258.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bwt.hywenlv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ylr.gotoacloud.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://icv.jqgufenzy.top

Ruby: 10.times { |i| puts i }
来源：http://sgf.hywenlv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vey.fzhhl.top

[B05] 遍历数组 / 列表
来源：http://hzf.yueranfly.top

Py:   for item in arr: print(item)
来源：http://vhj.havefunace.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xyg.pengpengdd.cyou

JS:   for (const item of arr) { console.log(item); }
来源：http://ddo.52xcode.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zqx.yuxming.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tkp.tianlin.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ffb.xuanzx.com

Ruby: arr.each { |item| puts item }
来源：http://rtw.c1oappe.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kgc.zhijiandao.cn

[B06] 遍历字典 / 对象
来源：http://vnm.birdmap.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ozv.sxryk.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gut.zdqjudy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rsr.xylfe.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fnr.fanxiaobao.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gdx.sjlbkw.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eze.gaohongyu789.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hop.yongpay.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rgj.tanke756.top

[B07] while 循环
来源：http://tft.chenjidiqi.icu

Py:   while i < 10: i += 1
来源：http://fek.jlsjyb.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gqn.hammf.cn

JS:   while (i < 10) { i++; }
来源：http://vcd.cashguo.top

TS:   while (i < 10) { i++; }
来源：http://cda.shzxlz.cn

Java: while (i < 10) { i++; }
来源：http://jjq.yj20258.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fui.jiagoushi.top

Ruby: while i < 10; i += 1; end
来源：http://ikt.aibaodan.cn

C#:   while (i < 10) { i++; }
来源：http://dkm.jlsjyb.cn

[B08] do-while（至少执行一次）
来源：http://lio.cqqwz.cn

Py:   # 无 do-while：用 while True + break
来源：http://fur.dashuyun.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rrr.meibo888.top

JS:   do { i++; } while (i < 10);
来源：http://liq.ivvv.top

TS:   do { i++; } while (i < 10);
来源：http://otw.chenjidiqi.icu

Java: do { i++; } while (i < 10);
来源：http://cjz.jinghuilouyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jfw.yuanzhike.top

Ruby: begin; i += 1; end while i < 10
来源：http://bni.shzxlz.cn

C#:   do { i++; } while (i < 10);
来源：http://jmz.pycfn.com

[B09] break 与 continue
来源：http://iiu.guannengcc.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xbi.hongshengwenyu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://utz.yangfankeji.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hdf.xuanzx.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lyk.shzxlz.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dav.yueranfly.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://azz.pengpengdd.cyou

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fmf.dashuyun.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yka.xziqi.cn

[B10] 遍历同时拿索引
来源：http://zlx.hnqzz.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://asx.yongpay.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nke.smart0.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fef.hysaishi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hbs.nanxuanxn.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yra.ctjpmb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mvq.snrcjt.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sgv.hfpthk.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://taz.zhixingplan.top

[B11] 生成数字序列 / 区间
来源：http://ego.chenlongwang.top

Py:   list(range(0, 10, 2))
来源：http://ohc.ybcxt.top

PHP:  range(0, 10, 2);
来源：http://sge.zhoulong.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ree.jinyuanbaomall.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wuo.hywenlv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qtm.wangshuangyany.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mfw.bbcook.cn

Ruby: (0...10).step(2).to_a
来源：http://pcg.hysaishi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uvj.sysykeji.top

[B12] 跳出多层循环
来源：http://twa.jyoumei.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://klk.sysykeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://rmj.xuetiantiany.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://psy.jiagoushi.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://brp.jinyuanbaomall.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pdg.ehwqpu.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nji.ywan-chungtsiang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ngy.yuanzhike.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://alw.birdmap.top


<!-- 参考信息 -->