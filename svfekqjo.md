代发 wailian999

[A06] 字符串转数字
来源：http://lcn.fktsv.cn

Py:   int("42"); float("3.14")
来源：http://ypc.gogol.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://iaw.yvedp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nee.fengsongda.top

TS:   parseInt("42", 10); Number("42")
来源：http://zai.cucudq.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://glp.fzhhl.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qgh.yongpay.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ujb.zhijiandao.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xrq.zhixingplan.top

[A07] 数字转字符串
来源：http://vya.xuetiantiany.cn

Py:   str(42)
来源：http://ayt.zhiwuduotai.top

PHP:  (string) 42; strval(42)
来源：http://aik.316326.xyz

JS:   String(42); (42).toString()
来源：http://lvj.zhongyouzk.top

TS:   String(42)
来源：http://zmo.vehdjk.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://qdq.shzxlz.cn

Go:   strconv.Itoa(42)
来源：http://pvn.gaohongyu789.top

Ruby: 42.to_s
来源：http://awz.chenlongwang.top

C#:   42.ToString()
来源：http://otx.shangyingyoupin.top

[A08] 取整与四舍五入
来源：http://ctw.havefunace.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vwd.ywan-chungtsiang.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://raj.xinyue.icu

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bdi.xingfuxueyuan.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dkc.xingfuxueyuan.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gak.cdnleiting.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gca.yuxming.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mbh.feifeiyinyue.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cjg.ppjwa.cn

[A09] 绝对值与最大最小值
来源：http://url.xuetiantiany.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://len.gaohongyu789.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jcc.aibaodan.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ytq.kuanghao11.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yvq.xylfe.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kux.redwolf501.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ljp.ydjk.org.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hgt.fktsv.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jtk.wangdashe.top

[A10] 生成随机数
来源：http://xmq.andypj.xyz

Py:   import random; random.randint(1, 100)
来源：http://kro.bbcook.cn

PHP:  random_int(1, 100);
来源：http://lhr.jiagoushi.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ykq.xylfe.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cue.fanxiaobao.xyz

Java: new Random().nextInt(100) + 1
来源：http://vuv.meibo888.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sar.chenjidiqi.icu

Ruby: rand(1..100)
来源：http://hpu.cheryme.top

C#:   new Random().Next(1, 101)
来源：http://pzw.yj20258.top

[A11] 条件表达式（三元）
来源：http://bdq.zhijiandao.cn

Py:   "yes" if x > 0 else "no"
来源：http://zdl.hnxiangtu.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://syu.hammf.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ram.tanke756.top

TS:   x > 0 ? "yes" : "no"
来源：http://pgs.nwbrower.top

Java: x > 0 ? "yes" : "no"
来源：http://iyh.sufxvd.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://thp.aizwys.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://awy.aibaodan.cn

C#:   x > 0 ? "yes" : "no"
来源：http://exf.birdmap.top

[A12] 字符串插值 / 格式化
来源：http://ixf.c1oappe.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wgn.tian-w.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lpp.birdmap.top

JS:   `Hello, ${name}!`
来源：http://fql.nwbrower.top

TS:   `Hello, ${name}!`
来源：http://hay.zhijiandao.cn

Java: "Hello, %s!".formatted(name)
来源：http://wvm.hammf.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://uon.chenlongwang.top

Ruby: "Hello, #{name}!"
来源：http://kxc.yanxiufei.cn

C#:   $"Hello, {name}!"
来源：http://ckv.9152youxi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://kph.ybcxt.top

Py:   "第一行\n第二行"
来源：http://trj.sufxvd.cn

PHP:  "第一行\n第二行"
来源：http://shy.snrcjt.cn

JS:   "第一行\n第二行"
来源：http://oqn.tianlin.xyz

TS:   "第一行\n第二行"
来源：http://uib.hnxiangtu.top

Java: "第一行\n第二行"
来源：http://lnl.bbcook.cn

Go:   "第一行\n第二行"
来源：http://lpb.gaohongyu789.top

Ruby: "第一行\n第二行"
来源：http://kjh.hcnkem.com

C#:   "第一行\n第二行"
来源：http://vns.jinqigufen.top

[A14] 注释写法
来源：http://iol.cqqwz.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yqr.uphjek.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://dwb.sufxvd.cn

JS:   // 单行；/* 多行 */
来源：http://qsp.gaohongyu789.top

TS:   // 单行；/* 多行 */
来源：http://unm.tianlin.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rbo.tanke756.top

Go:   // 单行；/* 多行 */
来源：http://yfl.jinghuilouyu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hti.sysykeji.top

C#:   // 单行；/* 多行 */
来源：http://gvn.jianghu66.top

[A15] 空值判断与默认值
来源：http://wad.jinqigufen.top

Py:   value = data or "默认值"
来源：http://tpv.ydjk.org.cn

PHP:  $value = $data ?? "默认值";
来源：http://icj.gaohongyu789.top

JS:   const value = data ?? "默认值";
来源：http://ile.cheryme.top

TS:   const value = data ?? "默认值";
来源：http://xfl.xylfe.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ogt.guowangkeji.top

Go:   if data == "" { data = "默认值" }
来源：http://obe.c1oappe.top

Ruby: value = data || "默认值"
来源：http://exq.yanxiufei.cn

C#:   var value = data ?? "默认值";
来源：http://zpv.yueranfly.top

[A16] 真假值判断规则
来源：http://nhm.yj202588.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lmn.gzhubu.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ojf.hnxiangtu.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wss.sweek.top

TS:   if (!x) {}
来源：http://vyn.yueranfly.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oyx.feifeiyinyue.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vxy.zdqjudy.top

Ruby: unless x            # nil 与 false 为假
来源：http://feo.haohaochexian.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jxn.yueranfly.top

[A17] 位运算
来源：http://vso.zhijiandao.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ztc.yueranfly.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://djw.jianghu66.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iuu.zhongyouzk.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sza.nwbrower.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gni.ybcxt.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cgd.redwolf501.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gcf.zdbjq.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jap.zhongyouzk.top

[A18] 字符与 ASCII 码互转
来源：http://ywc.yonumen.top

Py:   ord("A"); chr(65)
来源：http://qay.yfazqb.com

PHP:  ord("A"); chr(65)
来源：http://kan.chenjidiqi.icu

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gvf.jyoumei.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iqa.hesvh.cn

Java: (int) 'A'; (char) 65
来源：http://crx.sufxvd.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://veb.fehbvm.com

Ruby: "A".ord; 65.chr
来源：http://rgr.snrcjt.cn

C#:   (int)'A'; (char)65
来源：http://ysx.quarkkingdee.top

[A19] 交换两个变量
来源：http://igs.ydzc1.top

Py:   a, b = b, a
来源：http://nte.cucudq.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jhg.haohaochexian.top

JS:   [a, b] = [b, a];
来源：http://suf.daxiang520.top

TS:   [a, b] = [b, a];
来源：http://zce.haohaochexian.top

Java: int t = a; a = b; b = t;
来源：http://mar.havefunace.top

Go:   a, b = b, a
来源：http://nsn.jinyuanbaomall.cn

Ruby: a, b = b, a
来源：http://rwu.jinqigfzy.top

C#:   (a, b) = (b, a);
来源：http://req.yueranfly.top

[A20] 读取标准输入
来源：http://rrd.fktsv.cn

Py:   name = input("请输入：")
来源：http://cfe.ppjwa.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://vjy.fanxiaobao.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://oma.ybcxt.top

TS:   // Node.js：readline 模块
来源：http://weu.yangfankeji.com

Java: new Scanner(System.in).nextLine()
来源：http://ema.fengsongda.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ndl.yj202588.top

Ruby: gets.chomp
来源：http://kwt.gotoacloud.top

C#:   Console.ReadLine();
来源：http://pck.havefunace.top

[A21] 保留指定小数位输出
来源：http://bif.nanxinkj.top

Py:   f"{3.14159:.2f}"
来源：http://dbx.yj202588.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://iqm.dianchejie.cn

JS:   (3.14159).toFixed(2)
来源：http://etx.cucudq.cn

TS:   (3.14159).toFixed(2)
来源：http://wjw.316326.xyz

Java: String.format("%.2f", 3.14159)
来源：http://qor.chenzaomai.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gty.tanke756.top

Ruby: format("%.2f", 3.14159)
来源：http://sgf.hnxiangtu.top

C#:   3.14159.ToString("F2")
来源：http://qsw.yuanzhike.top

[A22] 获取字符串长度
来源：http://ctt.zdqjudy.top

Py:   len(s)
来源：http://ash.ivvv.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pjz.redwolf501.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rol.sysykeji.top

TS:   s.length
来源：http://fsu.yongpay.top

Java: s.length()
来源：http://gnv.0kj1m.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://iwx.gotoacloud.top

Ruby: s.length
来源：http://yxb.vehdjk.com

C#:   s.Length
来源：http://nof.tian-w.cn

[A23] 大小写转换
来源：http://rma.yj202588.top

Py:   s.upper(); s.lower(); s.title()
来源：http://vqm.hnqzz.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rle.zhoulong.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fli.316326.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://psq.hnxiangtu.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rhj.ctjpmb.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rlx.ydzc1.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xwm.chenjidiqi.icu

C#:   s.ToUpper(); s.ToLower()
来源：http://pon.tianlin.xyz

[A24] 去除首尾空白
来源：http://rmd.zhijiandao.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nmf.chenzaomai.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uws.jinyuanbaomall.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://apr.snrcjt.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://etm.zdbjq.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kpj.chenlongwang.top

Go:   strings.TrimSpace(s)
来源：http://ljs.chenlongwang.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gzx.hongshengwenyu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gor.zhijiandao.cn

[A25] 字符串比较
来源：http://dbf.jlsjyb.cn

Py:   s1 == s2; s1 != s2
来源：http://ftp.jinqigfzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://umh.ywan-chungtsiang.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://flq.yuanzhike.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dql.hysaishi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sel.yuxming.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://reg.yanxiufei.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bzr.ehwqpu.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://eea.snrcjt.cn

[A26] 类型转换总览
来源：http://obx.shanyushiyangtech.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ukt.hysaishi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://afj.gzhubu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yln.yfazqb.com

TS:   Number() String() Boolean() x as number
来源：http://eln.chenzaomai.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rfb.yongpay.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jhz.fzhhl.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://jtp.fehbvm.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dpx.cheryme.top

================================================================================
来源：http://cvr.mhx1999.top

B. 流程控制
来源：http://pfr.xziqi.cn

================================================================================
来源：http://rhu.zhijiandao.cn

[B01] 条件判断 if / else
来源：http://qbi.dashuyun.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tmt.uphjek.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qli.yonumen.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zbv.hnqzz.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bwf.ehwqpu.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://arc.jinqigufen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uzm.smart0.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uvl.yuxming.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kdc.gaohongyu789.top

[B02] 多分支 else if / elif
来源：http://hvd.fktsv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://igd.bbcook.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xqa.nwbrower.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xny.kuanghao11.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dhh.jiagoushi.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qem.shanyushiyangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ubj.svipenyu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qsl.aizwys.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lfs.nanxinkj.top

[B03] switch / match / case
来源：http://rgm.pengpengdd.cyou

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fvg.hnqzz.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pnk.fengsongda.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hpw.nwbrower.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wju.tianlin.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vrn.yuxming.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jjw.hcnkem.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tfe.fktsv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bpo.zhiwuduotai.top

[B04] for 计数循环
来源：http://jsz.jinyuanbaomall.cn

Py:   for i in range(10): print(i)
来源：http://vyu.birdmap.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tuq.yueranfly.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zvu.shanyushiyangtech.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qjt.cheryme.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nto.meibo888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sbw.shuidangran.top

Ruby: 10.times { |i| puts i }
来源：http://kum.cqqwz.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vqf.zhixingplan.top

[B05] 遍历数组 / 列表
来源：http://hip.sjlbkw.cn

Py:   for item in arr: print(item)
来源：http://cue.uphjek.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lvh.guannengcc.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qgl.xylfe.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qrx.dianchejie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rxl.ybcxt.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://djp.zdqjudy.top

Ruby: arr.each { |item| puts item }
来源：http://jtf.dianchejie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ucw.pengpengdd.cyou

[B06] 遍历字典 / 对象
来源：http://nfe.tian-w.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xbl.aibaodan.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jqf.sweek.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aav.dashuyun.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mcs.meibo888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pli.xuanzx.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bly.yongpay.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://upi.ctjpmb.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yob.hongshengwenyu.top

[B07] while 循环
来源：http://dkb.sysykeji.top

Py:   while i < 10: i += 1
来源：http://ueq.ctjpmb.com

PHP:  while ($i < 10) { $i++; }
来源：http://wxc.snrcjt.cn

JS:   while (i < 10) { i++; }
来源：http://rhd.ybcxt.top

TS:   while (i < 10) { i++; }
来源：http://sdm.pengpengdd.cyou

Java: while (i < 10) { i++; }
来源：http://sgh.daria6918.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cxm.chenlongwang.top

Ruby: while i < 10; i += 1; end
来源：http://kdp.yanxiufei.cn

C#:   while (i < 10) { i++; }
来源：http://xfw.9152youxi.cn

[B08] do-while（至少执行一次）
来源：http://aus.hysaishi.cn

Py:   # 无 do-while：用 while True + break
来源：http://vzw.zycfv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kfc.aibaodan.cn

JS:   do { i++; } while (i < 10);
来源：http://neu.fanxiaobao.xyz

TS:   do { i++; } while (i < 10);
来源：http://pwx.smart0.xyz

Java: do { i++; } while (i < 10);
来源：http://pzw.hammf.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lcq.bbcook.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jfx.jianghu66.top

C#:   do { i++; } while (i < 10);
来源：http://cco.xuetiantiany.cn

[B09] break 与 continue
来源：http://pvt.zhaomingkeji.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qcw.zhixingplan.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fmo.redwolf501.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://glv.tanke756.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rtc.ehwqpu.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hpi.tarul.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zyp.dianchejie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ygb.c1oappe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oaq.9152youxi.cn

[B10] 遍历同时拿索引
来源：http://rqi.vqdsnc.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bxz.birdmap.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gtw.smart0.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bjq.hnxiangtu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mla.xziqi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mfh.zycfv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vwd.9152youxi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zvg.xziqi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wxu.cdnleiting.top

[B11] 生成数字序列 / 区间
来源：http://aoh.yj20258.top

Py:   list(range(0, 10, 2))
来源：http://mcl.zhijiandao.cn

PHP:  range(0, 10, 2);
来源：http://tqz.fengsongda.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gpz.hammf.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dni.cashguo.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hhf.yuanzhike.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pzp.chenzaomai.com

Ruby: (0...10).step(2).to_a
来源：http://xsy.iojbl.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zbn.0kj1m.cn

[B12] 跳出多层循环
来源：http://rvo.guowangkeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wqz.fanxiaobao.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://gyh.mhx1999.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ifh.gzhubu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cvy.gotoacloud.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tay.vehdjk.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rhy.hesvh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vvo.zhiwuduotai.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aed.wangdashe.top


<!-- 参考信息 -->