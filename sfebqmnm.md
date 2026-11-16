代发 wailian999

[A06] 字符串转数字
来源：http://chb.epnwcf.com

Py:   int("42"); float("3.14")
来源：http://tdg.chenjidiqi.icu

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xvz.ctjpmb.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tbb.cheryme.top

TS:   parseInt("42", 10); Number("42")
来源：http://xcb.aibaodan.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ger.xuetiantiany.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hrs.zhijiandao.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ipp.guowangkeji.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zoa.jlsjyb.cn

[A07] 数字转字符串
来源：http://kcv.shanyushiyangkeji.top

Py:   str(42)
来源：http://gbe.zhoulong.xyz

PHP:  (string) 42; strval(42)
来源：http://lit.gzhubu.top

JS:   String(42); (42).toString()
来源：http://qao.quarkkingdee.top

TS:   String(42)
来源：http://abd.guowangkeji.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://bku.cashguo.top

Go:   strconv.Itoa(42)
来源：http://fch.hongshengwenyu.top

Ruby: 42.to_s
来源：http://dak.gzhubu.top

C#:   42.ToString()
来源：http://suw.epnwcf.com

[A08] 取整与四舍五入
来源：http://adp.snrcjt.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nfu.birdmap.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fgg.yj202588.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cja.tanke756.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ejo.xziqi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ofi.c1oappe.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bgw.gzhubu.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://wtn.yonumen.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bkb.jyoumei.cn

[A09] 绝对值与最大最小值
来源：http://zqj.mhx1999.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hjx.xylfe.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rda.cdnleiting.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://use.fzhhl.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uwi.andypj.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lqy.gogol.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zzb.sjlbkw.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://soj.zycfv.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://chh.tarul.cn

[A10] 生成随机数
来源：http://wdb.yj20258888.top

Py:   import random; random.randint(1, 100)
来源：http://gtf.ywan-chungtsiang.top

PHP:  random_int(1, 100);
来源：http://rkx.ctjpmb.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zam.xingfuxueyuan.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ldr.zhixingplan.top

Java: new Random().nextInt(100) + 1
来源：http://mpe.sjlbkw.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xnu.cdnleiting.top

Ruby: rand(1..100)
来源：http://nap.gogol.net.cn

C#:   new Random().Next(1, 101)
来源：http://kpr.nwbrower.top

[A11] 条件表达式（三元）
来源：http://sbe.hesvh.cn

Py:   "yes" if x > 0 else "no"
来源：http://ugw.jqgufenzy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://gqs.ydzc1.top

JS:   x > 0 ? "yes" : "no"
来源：http://xgj.fehbvm.com

TS:   x > 0 ? "yes" : "no"
来源：http://fst.0kj1m.cn

Java: x > 0 ? "yes" : "no"
来源：http://wct.shanyushiyangtech.top

Go:   // 无三元运算符，需用 if 语句
来源：http://tfk.dianchejie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fkg.yj20258888.top

C#:   x > 0 ? "yes" : "no"
来源：http://tia.c1oappe.top

[A12] 字符串插值 / 格式化
来源：http://opw.fzhhl.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tis.cheryme.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://miu.chenlongwang.top

JS:   `Hello, ${name}!`
来源：http://wqj.wangdashe.top

TS:   `Hello, ${name}!`
来源：http://dlm.dianchejie.cn

Java: "Hello, %s!".formatted(name)
来源：http://nqr.yj202588.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://stc.zhoulong.xyz

Ruby: "Hello, #{name}!"
来源：http://dzo.gaohongyu789.top

C#:   $"Hello, {name}!"
来源：http://zkz.zhaomingkeji.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://ymo.xylfe.cn

Py:   "第一行\n第二行"
来源：http://mla.uphjek.com

PHP:  "第一行\n第二行"
来源：http://mwe.shanyushiyangkeji.top

JS:   "第一行\n第二行"
来源：http://gvp.fengsongda.top

TS:   "第一行\n第二行"
来源：http://est.fehbvm.com

Java: "第一行\n第二行"
来源：http://fwd.xylfe.cn

Go:   "第一行\n第二行"
来源：http://dtc.xingfuxueyuan.xyz

Ruby: "第一行\n第二行"
来源：http://ydl.sxryk.cn

C#:   "第一行\n第二行"
来源：http://afj.ydjk.org.cn

[A14] 注释写法
来源：http://coa.sufxvd.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://jsd.yanxiufei.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://oeh.shzxlz.cn

JS:   // 单行；/* 多行 */
来源：http://yrd.sjlbkw.cn

TS:   // 单行；/* 多行 */
来源：http://eaj.shangyingyoupin.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://plp.zhixingplan.top

Go:   // 单行；/* 多行 */
来源：http://azv.zdqjudy.top

Ruby: # 单行；=begin 多行 =end
来源：http://bhp.jyoumei.cn

C#:   // 单行；/* 多行 */
来源：http://ztk.c1oappe.top

[A15] 空值判断与默认值
来源：http://ktu.yfazqb.com

Py:   value = data or "默认值"
来源：http://zbz.jyoumei.cn

PHP:  $value = $data ?? "默认值";
来源：http://pjr.meibo888.top

JS:   const value = data ?? "默认值";
来源：http://wje.hammf.cn

TS:   const value = data ?? "默认值";
来源：http://npi.svipenyu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nkl.cashguo.top

Go:   if data == "" { data = "默认值" }
来源：http://flp.aizwys.cn

Ruby: value = data || "默认值"
来源：http://dit.bjfxy.top

C#:   var value = data ?? "默认值";
来源：http://rcv.gotoacloud.top

[A16] 真假值判断规则
来源：http://dgr.yangfankeji.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://flv.xylfe.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://oqo.wangshuangyany.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://aia.jyoumei.cn

TS:   if (!x) {}
来源：http://sur.smart0.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://woe.xylfe.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yrj.yongpay.top

Ruby: unless x            # nil 与 false 为假
来源：http://iqv.xuetiantiany.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tle.jlsjyb.cn

[A17] 位运算
来源：http://ppy.jqgfzy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cvt.chenlongwang.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jdr.9152youxi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://war.fzhhl.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://czg.shuidangran.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wpn.ivvv.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nut.guowangkeji.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://khc.mhx1999.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hcw.zhijiandao.cn

[A18] 字符与 ASCII 码互转
来源：http://alj.tanke756.top

Py:   ord("A"); chr(65)
来源：http://jgw.shanyushiyangkeji.top

PHP:  ord("A"); chr(65)
来源：http://hwq.hysaishi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xty.pycfn.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zro.uphjek.com

Java: (int) 'A'; (char) 65
来源：http://zbx.hnxiangtu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vau.epnwcf.com

Ruby: "A".ord; 65.chr
来源：http://gkp.zhixingplan.top

C#:   (int)'A'; (char)65
来源：http://ztt.zhijiandao.cn

[A19] 交换两个变量
来源：http://cit.cucudq.cn

Py:   a, b = b, a
来源：http://egp.yangfankeji.com

PHP:  [$a, $b] = [$b, $a];
来源：http://kgc.zhengqikj.top

JS:   [a, b] = [b, a];
来源：http://htd.316326.xyz

TS:   [a, b] = [b, a];
来源：http://bps.jlsjyb.cn

Java: int t = a; a = b; b = t;
来源：http://faz.vqdsnc.cn

Go:   a, b = b, a
来源：http://vhi.jqgufenzy.top

Ruby: a, b = b, a
来源：http://nxk.birdmap.top

C#:   (a, b) = (b, a);
来源：http://qpg.fanxiaobao.xyz

[A20] 读取标准输入
来源：http://maa.yfazqb.com

Py:   name = input("请输入：")
来源：http://rrt.jqgfzy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ugn.jqgufenzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://raj.gogol.net.cn

TS:   // Node.js：readline 模块
来源：http://pto.sxryk.cn

Java: new Scanner(System.in).nextLine()
来源：http://ikc.nanxuanxn.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wwa.jianghu66.top

Ruby: gets.chomp
来源：http://fyg.zdqjudy.top

C#:   Console.ReadLine();
来源：http://zdp.dashuyun.cn

[A21] 保留指定小数位输出
来源：http://dbi.tianlin.xyz

Py:   f"{3.14159:.2f}"
来源：http://sel.wangdashe.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bkr.tianlin.xyz

JS:   (3.14159).toFixed(2)
来源：http://yrd.yuanzhike.top

TS:   (3.14159).toFixed(2)
来源：http://wze.ctjpmb.com

Java: String.format("%.2f", 3.14159)
来源：http://sgl.epnwcf.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://shv.aibaodan.cn

Ruby: format("%.2f", 3.14159)
来源：http://wib.c1oappe.top

C#:   3.14159.ToString("F2")
来源：http://wzy.ydzc1.top

[A22] 获取字符串长度
来源：http://bkf.hnqzz.top

Py:   len(s)
来源：http://mso.sxryk.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uff.yonumen.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kaa.jlsjyb.cn

TS:   s.length
来源：http://qxg.xylfe.cn

Java: s.length()
来源：http://dxe.cashguo.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zmz.yfazqb.com

Ruby: s.length
来源：http://fpj.aizwys.cn

C#:   s.Length
来源：http://mcs.fehbvm.com

[A23] 大小写转换
来源：http://rmz.guowangkeji.top

Py:   s.upper(); s.lower(); s.title()
来源：http://bzu.ctjpmb.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kur.tanke756.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lqo.redwolf501.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rea.zdbjq.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tmv.epnwcf.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kbz.shangyingyoupin.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wnw.hcnkem.com

C#:   s.ToUpper(); s.ToLower()
来源：http://yju.jinyuanbaomall.cn

[A24] 去除首尾空白
来源：http://jdf.jinyuanbaomall.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gpx.52xcode.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://trs.uphjek.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wao.zhengqikj.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kzf.zdqjudy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sjg.xuanzx.com

Go:   strings.TrimSpace(s)
来源：http://xay.sjlbkw.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ayu.hcnkem.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jke.hnqzz.top

[A25] 字符串比较
来源：http://gcn.yj20258.top

Py:   s1 == s2; s1 != s2
来源：http://bwc.guowangkeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rwc.jqgufenzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vsl.yangfankeji.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mtm.hesvh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xbg.hammf.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kcx.hcnkem.com

Ruby: s1 == s2; s1 <=> s2
来源：http://djk.9152youxi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yzw.nwbrower.top

[A26] 类型转换总览
来源：http://zpt.c1oappe.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fjm.zhengqikj.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jrf.cucudq.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ctc.cucudq.cn

TS:   Number() String() Boolean() x as number
来源：http://yfc.pycfn.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hvu.gotoacloud.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kvp.yonumen.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://wbv.gotoacloud.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dzv.tian-w.cn

================================================================================
来源：http://slp.guowangkeji.top

B. 流程控制
来源：http://xdg.yuxming.cn

================================================================================
来源：http://qrb.chenjidiqi.icu

[B01] 条件判断 if / else
来源：http://xzb.yongpay.top

Py:   result = "正" if x > 0 else "非正"
来源：http://gxd.zdqjudy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://njx.hywenlv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qwi.hnqzz.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gke.jinqigfzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://orp.guowangkeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gpg.jianghu66.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fld.yfazqb.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dcj.zhaomingkeji.xyz

[B02] 多分支 else if / elif
来源：http://far.52xcode.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xkj.xylfe.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fau.daxiang520.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://csy.meibo888.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vdp.0kj1m.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ekf.gogol.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://aem.hfpthk.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wqk.zhijiandao.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://thr.yuxming.cn

[B03] switch / match / case
来源：http://fem.meibo888.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kvy.yuanzhike.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nfs.jqgfzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://okv.cdnleiting.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pak.316326.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://avz.kuanghao11.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ezg.dashuyun.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://deo.xinyue.icu

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wbb.yj20258.top

[B04] for 计数循环
来源：http://rwq.gogol.net.cn

Py:   for i in range(10): print(i)
来源：http://jvs.jinyuanbaomall.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kbv.xingfuxueyuan.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jqp.zdbjq.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hfy.jianghu66.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ffr.chenzaomai.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://seu.jinqigfzy.top

Ruby: 10.times { |i| puts i }
来源：http://dxf.fengsongda.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://awy.shangyingyoupin.top

[B05] 遍历数组 / 列表
来源：http://jds.cucudq.cn

Py:   for item in arr: print(item)
来源：http://vuq.xinyue.icu

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://evk.ctjpmb.com

JS:   for (const item of arr) { console.log(item); }
来源：http://snb.gaohongyu789.top

TS:   for (const item of arr) { console.log(item); }
来源：http://bcd.bbcook.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lye.jiagoushi.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pgi.chenjidiqi.icu

Ruby: arr.each { |item| puts item }
来源：http://bmo.daxiang520.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ajo.jinghuilouyu.cn

[B06] 遍历字典 / 对象
来源：http://met.epnwcf.com

Py:   for k, v in d.items(): print(k, v)
来源：http://qyz.havefunace.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lgy.cashguo.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://slu.jqgufenzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jmn.yj202588.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://okb.xuetiantiany.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zhn.vehdjk.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hem.mhx1999.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nby.nanxuanxn.top

[B07] while 循环
来源：http://qnr.gaohongyu789.top

Py:   while i < 10: i += 1
来源：http://sxg.zdbjq.cn

PHP:  while ($i < 10) { $i++; }
来源：http://neu.fzhhl.top

JS:   while (i < 10) { i++; }
来源：http://ykw.wangdashe.top

TS:   while (i < 10) { i++; }
来源：http://hns.vehdjk.com

Java: while (i < 10) { i++; }
来源：http://vqr.yanxiufei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://atq.shanyushiyangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://oqn.zdbjq.cn

C#:   while (i < 10) { i++; }
来源：http://kvo.xuanzx.com

[B08] do-while（至少执行一次）
来源：http://vqd.ehwqpu.com

Py:   # 无 do-while：用 while True + break
来源：http://dhq.mhx1999.top

PHP:  do { $i++; } while ($i < 10);
来源：http://drq.jiagoushi.top

JS:   do { i++; } while (i < 10);
来源：http://why.birdmap.top

TS:   do { i++; } while (i < 10);
来源：http://ynt.sxryk.cn

Java: do { i++; } while (i < 10);
来源：http://obo.0kj1m.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bhq.cashguo.top

Ruby: begin; i += 1; end while i < 10
来源：http://msk.ywan-chungtsiang.top

C#:   do { i++; } while (i < 10);
来源：http://hpb.bjfxy.top

[B09] break 与 continue
来源：http://hih.birdmap.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gky.hysaishi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zqv.vehdjk.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://znt.tarul.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uva.jianghu66.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ild.cqqwz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mou.jlsjyb.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://abu.daxiang520.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ohl.gogol.net.cn

[B10] 遍历同时拿索引
来源：http://xjw.dashuyun.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vha.tanke756.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://atd.daria6918.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bfo.52xcode.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://eaf.zdqjudy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rox.aizwys.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ixy.ehwqpu.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xjx.birdmap.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hwo.meibo888.top

[B11] 生成数字序列 / 区间
来源：http://qvm.wangshuangyany.cn

Py:   list(range(0, 10, 2))
来源：http://vuc.svipenyu.cn

PHP:  range(0, 10, 2);
来源：http://fdw.316326.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xcy.hesvh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://olq.tarul.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xxd.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hbd.bjfxy.top

Ruby: (0...10).step(2).to_a
来源：http://txo.gzhubu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nve.iojbl.cn

[B12] 跳出多层循环
来源：http://spz.meibo888.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://lgw.mhx1999.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://kil.meibo888.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wbi.hywenlv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dhl.zdbjq.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zcv.yangfankeji.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oxk.yongpay.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uzm.mhx1999.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jhu.gotoacloud.top


<!-- 参考信息 -->