代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://oml.gotoacloud.top

[A07] 数字转字符串
来源：http://ovl.0kj1m.cn

Py:   str(42)
来源：http://iiq.shanyushiyangtech.top

PHP:  (string) 42; strval(42)
来源：http://pcd.yfazqb.com

JS:   String(42); (42).toString()
来源：http://nwo.cashguo.top

TS:   String(42)
来源：http://rsc.zhongyouzk.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://lmj.ybcxt.top

Go:   strconv.Itoa(42)
来源：http://wba.yvedp.cn

Ruby: 42.to_s
来源：http://gel.jqgufenzy.top

C#:   42.ToString()
来源：http://ken.shuidangran.top

[A08] 取整与四舍五入
来源：http://ton.yongpay.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://slk.shanyushiyangtech.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qvk.zhaomingkeji.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zkd.fanxiaobao.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fnu.xuetiantiany.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ulj.birdmap.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tci.hysaishi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lnr.vqdsnc.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://icu.tanke756.top

[A09] 绝对值与最大最小值
来源：http://uaf.ydjk.org.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kbf.zhengqikj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://trx.tarul.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wtm.kuanghao11.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://chf.jinqigfzy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jbw.zhoulong.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://anj.bbcook.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ccl.redwolf501.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dbl.fehbvm.com

[A10] 生成随机数
来源：http://zzv.shangyingyoupin.top

Py:   import random; random.randint(1, 100)
来源：http://lnd.yj20258.top

PHP:  random_int(1, 100);
来源：http://txy.nanxinkj.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mbx.cucudq.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pom.ctjpmb.com

Java: new Random().nextInt(100) + 1
来源：http://mne.aizwys.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xer.hnqzz.top

Ruby: rand(1..100)
来源：http://vxh.ctjpmb.com

C#:   new Random().Next(1, 101)
来源：http://qtj.yvedp.cn

[A11] 条件表达式（三元）
来源：http://mrm.zycfv.cn

Py:   "yes" if x > 0 else "no"
来源：http://vhl.vqdsnc.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pcq.fktsv.cn

JS:   x > 0 ? "yes" : "no"
来源：http://csh.zhiwuduotai.top

TS:   x > 0 ? "yes" : "no"
来源：http://zum.dianchejie.cn

Java: x > 0 ? "yes" : "no"
来源：http://ncb.xuanzx.com

Go:   // 无三元运算符，需用 if 语句
来源：http://qsm.fanxiaobao.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://qos.sufxvd.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rtn.jinyuanbaomall.cn

[A12] 字符串插值 / 格式化
来源：http://eyw.jlsjyb.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nym.quarkkingdee.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kmf.ehwqpu.com

JS:   `Hello, ${name}!`
来源：http://qfr.zdqjudy.top

TS:   `Hello, ${name}!`
来源：http://nyh.hammf.cn

Java: "Hello, %s!".formatted(name)
来源：http://kve.haohaochexian.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ray.hongshengwenyu.top

Ruby: "Hello, #{name}!"
来源：http://gad.tian-w.cn

C#:   $"Hello, {name}!"
来源：http://qho.dashuyun.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ddx.nanxinkj.top

Py:   "第一行\n第二行"
来源：http://bdb.zhaomingkeji.xyz

PHP:  "第一行\n第二行"
来源：http://uih.xinyue.icu

JS:   "第一行\n第二行"
来源：http://bdp.jlsjyb.cn

TS:   "第一行\n第二行"
来源：http://lxd.zhaomingkeji.xyz

Java: "第一行\n第二行"
来源：http://ejx.jinyuanbaomall.cn

Go:   "第一行\n第二行"
来源：http://dns.zycfv.cn

Ruby: "第一行\n第二行"
来源：http://ear.9152youxi.cn

C#:   "第一行\n第二行"
来源：http://wja.epnwcf.com

[A14] 注释写法
来源：http://ukf.zdbjq.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xpi.yj20258.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://jwu.yvedp.cn

JS:   // 单行；/* 多行 */
来源：http://qqm.quarkkingdee.top

TS:   // 单行；/* 多行 */
来源：http://pfu.zhiwuduotai.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xxp.nwbrower.top

Go:   // 单行；/* 多行 */
来源：http://nks.epnwcf.com

Ruby: # 单行；=begin 多行 =end
来源：http://eyz.c1oappe.top

C#:   // 单行；/* 多行 */
来源：http://bcl.yuxming.cn

[A15] 空值判断与默认值
来源：http://dcu.dashuyun.cn

Py:   value = data or "默认值"
来源：http://ela.zdqjudy.top

PHP:  $value = $data ?? "默认值";
来源：http://lls.nanxuanxn.top

JS:   const value = data ?? "默认值";
来源：http://kve.hongshengwenyu.top

TS:   const value = data ?? "默认值";
来源：http://tci.9152youxi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://loz.xingfuxueyuan.xyz

Go:   if data == "" { data = "默认值" }
来源：http://igr.tianlin.xyz

Ruby: value = data || "默认值"
来源：http://tnn.zhengqikj.top

C#:   var value = data ?? "默认值";
来源：http://caq.fktsv.cn

[A16] 真假值判断规则
来源：http://mcg.hywenlv.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://czx.birdmap.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://eka.havefunace.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bjb.quarkkingdee.top

TS:   if (!x) {}
来源：http://awp.yueranfly.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qdq.hcnkem.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pyi.zycfv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://mdk.gogol.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yvv.jinghuilouyu.cn

[A17] 位运算
来源：http://cxl.smart0.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://afa.0kj1m.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nkl.jlsjyb.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://swo.yj20258.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fpr.birdmap.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wub.chenlongwang.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jiz.xylfe.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lzo.mhx1999.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wuw.fehbvm.com

[A18] 字符与 ASCII 码互转
来源：http://yej.nanxuanxn.top

Py:   ord("A"); chr(65)
来源：http://gaj.yonumen.top

PHP:  ord("A"); chr(65)
来源：http://hzg.yonumen.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wfx.mhx1999.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xyr.xinyue.icu

Java: (int) 'A'; (char) 65
来源：http://jve.jinqigfzy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xmd.yonumen.top

Ruby: "A".ord; 65.chr
来源：http://rtd.shanyushiyangtech.top

C#:   (int)'A'; (char)65
来源：http://uqd.gogol.net.cn

[A19] 交换两个变量
来源：http://jfd.sjlbkw.cn

Py:   a, b = b, a
来源：http://tek.fanxiaobao.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://wxk.tarul.cn

JS:   [a, b] = [b, a];
来源：http://ley.jiagoushi.top

TS:   [a, b] = [b, a];
来源：http://vql.xziqi.cn

Java: int t = a; a = b; b = t;
来源：http://mgr.birdmap.top

Go:   a, b = b, a
来源：http://emq.hongshengwenyu.top

Ruby: a, b = b, a
来源：http://ayc.wangshuangyany.cn

C#:   (a, b) = (b, a);
来源：http://uga.tianlin.xyz

[A20] 读取标准输入
来源：http://hmz.yj20258.top

Py:   name = input("请输入：")
来源：http://qle.9152youxi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://cqg.xingfuxueyuan.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wfu.hammf.cn

TS:   // Node.js：readline 模块
来源：http://fph.xziqi.cn

Java: new Scanner(System.in).nextLine()
来源：http://fgs.gogol.net.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mrc.jiagoushi.top

Ruby: gets.chomp
来源：http://btv.cdnleiting.top

C#:   Console.ReadLine();
来源：http://ntd.ywan-chungtsiang.top

[A21] 保留指定小数位输出
来源：http://rkh.sweek.top

Py:   f"{3.14159:.2f}"
来源：http://utv.yj20258.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://uzf.fzhhl.top

JS:   (3.14159).toFixed(2)
来源：http://wpa.jqgufenzy.top

TS:   (3.14159).toFixed(2)
来源：http://zct.yj202588.top

Java: String.format("%.2f", 3.14159)
来源：http://dfr.zhongyouzk.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gwv.feifeiyinyue.top

Ruby: format("%.2f", 3.14159)
来源：http://vox.yanxiufei.cn

C#:   3.14159.ToString("F2")
来源：http://qld.andypj.xyz

[A22] 获取字符串长度
来源：http://ovh.hnqzz.top

Py:   len(s)
来源：http://zxt.zdqjudy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ief.ehwqpu.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mjy.sjlbkw.cn

TS:   s.length
来源：http://ytr.hnqzz.top

Java: s.length()
来源：http://cmh.hysaishi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bni.316326.xyz

Ruby: s.length
来源：http://jnq.haohaochexian.top

C#:   s.Length
来源：http://bme.aibaodan.cn

[A23] 大小写转换
来源：http://dyl.fzhhl.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wbx.xingfuxueyuan.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://aur.sjlbkw.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lqe.yj20258888.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://siw.jinghuilouyu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cwm.cqqwz.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://myt.xinyue.icu

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://imt.epnwcf.com

C#:   s.ToUpper(); s.ToLower()
来源：http://ncm.gogol.net.cn

[A24] 去除首尾空白
来源：http://ssg.yfazqb.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vjw.jinqigufen.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xnf.xylfe.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qht.chenlongwang.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tzq.yongpay.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bpu.fktsv.cn

Go:   strings.TrimSpace(s)
来源：http://arw.hesvh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gzx.bbcook.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://byl.aizwys.cn

[A25] 字符串比较
来源：http://zmw.yonumen.top

Py:   s1 == s2; s1 != s2
来源：http://mwo.hywenlv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xal.wangshuangyany.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://alv.yongpay.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qab.aizwys.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ucd.jyoumei.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kif.mhx1999.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ykp.yj20258888.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://byu.gaohongyu789.top

[A26] 类型转换总览
来源：http://mfo.svipenyu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rgb.yj20258.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gqt.yfazqb.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://itx.jinyuanbaomall.cn

TS:   Number() String() Boolean() x as number
来源：http://wcy.ppjwa.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tmn.epnwcf.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://arc.snrcjt.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tgf.wangdashe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lds.9152youxi.cn

================================================================================
来源：http://qfl.316326.xyz

B. 流程控制
来源：http://zgb.nanxinkj.top

================================================================================
来源：http://unx.uphjek.com

[B01] 条件判断 if / else
来源：http://luh.wangdashe.top

Py:   result = "正" if x > 0 else "非正"
来源：http://qwj.jlsjyb.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hia.andypj.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cpb.jyoumei.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kxy.gogol.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tmc.hysaishi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wwe.xingfuxueyuan.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://stj.c1oappe.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mbn.jyoumei.cn

[B02] 多分支 else if / elif
来源：http://ltg.gogol.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wuk.tian-w.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://skw.ivvv.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tja.guowangkeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cef.jqgfzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iwx.ydjk.org.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ofi.andypj.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hma.ydjk.org.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aww.jiagoushi.top

[B03] switch / match / case
来源：http://rsu.yj20258.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://eey.birdmap.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fre.pycfn.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ala.sxryk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dqk.yuxming.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://smz.shangyingyoupin.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wma.havefunace.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bwp.shzxlz.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bfn.hfpthk.cn

[B04] for 计数循环
来源：http://nje.fehbvm.com

Py:   for i in range(10): print(i)
来源：http://jqs.ctjpmb.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jbq.jinqigfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fon.gotoacloud.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bnv.nanxinkj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ylr.bbcook.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kvb.cqqwz.cn

Ruby: 10.times { |i| puts i }
来源：http://dxz.zhoulong.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://drl.zhaomingkeji.xyz

[B05] 遍历数组 / 列表
来源：http://akd.vqdsnc.cn

Py:   for item in arr: print(item)
来源：http://oqh.jianghu66.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cpt.bjfxy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fen.guowangkeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hsx.shuidangran.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://cpv.jlsjyb.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uga.cheryme.top

Ruby: arr.each { |item| puts item }
来源：http://ghu.andypj.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pzy.zhoulong.xyz

[B06] 遍历字典 / 对象
来源：http://wcn.zhengqikj.top

Py:   for k, v in d.items(): print(k, v)
来源：http://lif.316326.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://azu.gogol.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nrx.zhijiandao.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qmz.tianlin.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://stq.dianchejie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bjj.meibo888.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nmm.sweek.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gnm.ybcxt.top

[B07] while 循环
来源：http://glk.fzhhl.top

Py:   while i < 10: i += 1
来源：http://ssa.xuetiantiany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://enz.xuanzx.com

JS:   while (i < 10) { i++; }
来源：http://cay.uphjek.com

TS:   while (i < 10) { i++; }
来源：http://jpy.wangdashe.top

Java: while (i < 10) { i++; }
来源：http://ttz.ydzc1.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ozz.bbcook.cn

Ruby: while i < 10; i += 1; end
来源：http://epv.zhoulong.xyz

C#:   while (i < 10) { i++; }
来源：http://nxf.feifeiyinyue.top

[B08] do-while（至少执行一次）
来源：http://hnd.havefunace.top

Py:   # 无 do-while：用 while True + break
来源：http://jkr.guowangkeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://iwf.9152youxi.cn

JS:   do { i++; } while (i < 10);
来源：http://lie.zhaomingkeji.xyz

TS:   do { i++; } while (i < 10);
来源：http://wkt.sufxvd.cn

Java: do { i++; } while (i < 10);
来源：http://oyc.9152youxi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rip.yuanzhike.top

Ruby: begin; i += 1; end while i < 10
来源：http://ome.jqgufenzy.top

C#:   do { i++; } while (i < 10);
来源：http://qsm.redwolf501.top

[B09] break 与 continue
来源：http://wfa.jyoumei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dbm.yanxiufei.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://slp.bjfxy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rck.nanxuanxn.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nag.zhijiandao.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bsn.hnqzz.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://laq.zhijiandao.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://snt.hesvh.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lyy.ppjwa.cn

[B10] 遍历同时拿索引
来源：http://xhp.hammf.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jut.gzhubu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ybo.epnwcf.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://iza.yonumen.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cwi.feifeiyinyue.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yyj.vqdsnc.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cuv.fzhhl.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iin.yfazqb.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://agn.pycfn.com

[B11] 生成数字序列 / 区间
来源：http://blb.hysaishi.cn

Py:   list(range(0, 10, 2))
来源：http://ypl.xingfuxueyuan.xyz

PHP:  range(0, 10, 2);
来源：http://xgq.dianchejie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ezc.sysykeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gyr.yuanzhike.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ydz.bbcook.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gqk.fzhhl.top

Ruby: (0...10).step(2).to_a
来源：http://ssg.yj20258.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://igb.hfpthk.cn

[B12] 跳出多层循环
来源：http://rxc.gaohongyu789.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://yfp.gzhubu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mdt.ywan-chungtsiang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ale.yangfankeji.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mil.hcnkem.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kri.zdbjq.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gvm.aibaodan.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://klz.tanke756.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sqe.nwbrower.top

[B13] 判断是否为数字
来源：http://lsg.birdmap.top

Py:   isinstance(x, (int, float))
来源：http://miq.feifeiyinyue.top

PHP:  is_numeric($x)
来源：http://psr.c1oappe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gsv.sxryk.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bqp.zdqjudy.top

Java: x instanceof Number
来源：http://ijo.ybcxt.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tjd.shuidangran.top

Ruby: x.is_a?(Numeric)
来源：http://orc.xingfuxueyuan.xyz


<!-- 参考信息 -->