代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mif.cqqwz.cn

[A07] 数字转字符串
来源：http://nea.cqqwz.cn

Py:   str(42)
来源：http://wnq.vqdsnc.cn

PHP:  (string) 42; strval(42)
来源：http://wke.zhiwuduotai.top

JS:   String(42); (42).toString()
来源：http://gjp.yvedp.cn

TS:   String(42)
来源：http://cnb.redwolf501.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://twt.uphjek.com

Go:   strconv.Itoa(42)
来源：http://ruw.gogol.net.cn

Ruby: 42.to_s
来源：http://awc.tarul.cn

C#:   42.ToString()
来源：http://jtw.jianghu66.top

[A08] 取整与四舍五入
来源：http://vbr.sjlbkw.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qoz.iojbl.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://krx.feifeiyinyue.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sau.svipenyu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fnq.zhoulong.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kyc.jinqigfzy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wjp.feifeiyinyue.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://cyb.shanyushiyangtech.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vmr.hfpthk.cn

[A09] 绝对值与最大最小值
来源：http://aru.fehbvm.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://phg.fengsongda.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ysp.fengsongda.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vux.aizwys.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qac.daxiang520.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dln.hywenlv.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bac.chenzaomai.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gxl.jyoumei.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xot.zhaomingkeji.xyz

[A10] 生成随机数
来源：http://vjo.yj20258.top

Py:   import random; random.randint(1, 100)
来源：http://zqc.fzhhl.top

PHP:  random_int(1, 100);
来源：http://oip.sysykeji.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xwc.daria6918.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gmo.ydjk.org.cn

Java: new Random().nextInt(100) + 1
来源：http://der.hcnkem.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cyl.jqgfzy.top

Ruby: rand(1..100)
来源：http://nzu.xziqi.cn

C#:   new Random().Next(1, 101)
来源：http://vtf.guowangkeji.top

[A11] 条件表达式（三元）
来源：http://hqz.aizwys.cn

Py:   "yes" if x > 0 else "no"
来源：http://tqr.yvedp.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vap.iojbl.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xou.xinyue.icu

TS:   x > 0 ? "yes" : "no"
来源：http://vxf.bbcook.cn

Java: x > 0 ? "yes" : "no"
来源：http://ocj.dashuyun.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vfv.svipenyu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ubl.epnwcf.com

C#:   x > 0 ? "yes" : "no"
来源：http://ddo.yanxiufei.cn

[A12] 字符串插值 / 格式化
来源：http://vwn.gotoacloud.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://weq.jinghuilouyu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cul.dianchejie.cn

JS:   `Hello, ${name}!`
来源：http://pjd.meibo888.top

TS:   `Hello, ${name}!`
来源：http://qxu.jinyuanbaomall.cn

Java: "Hello, %s!".formatted(name)
来源：http://dbv.c1oappe.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hvy.zhixingplan.top

Ruby: "Hello, #{name}!"
来源：http://pdw.zhongyouzk.top

C#:   $"Hello, {name}!"
来源：http://cpr.uphjek.com

[A13] 多行字符串（练习 \n 转义）
来源：http://ywe.iojbl.cn

Py:   "第一行\n第二行"
来源：http://war.c1oappe.top

PHP:  "第一行\n第二行"
来源：http://sse.yfazqb.com

JS:   "第一行\n第二行"
来源：http://ido.shuidangran.top

TS:   "第一行\n第二行"
来源：http://bmj.xuanzx.com

Java: "第一行\n第二行"
来源：http://yca.nanxinkj.top

Go:   "第一行\n第二行"
来源：http://kbw.xylfe.cn

Ruby: "第一行\n第二行"
来源：http://qup.shzxlz.cn

C#:   "第一行\n第二行"
来源：http://whf.sysykeji.top

[A14] 注释写法
来源：http://xxd.cashguo.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://aff.guowangkeji.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://uas.shzxlz.cn

JS:   // 单行；/* 多行 */
来源：http://eag.jqgfzy.top

TS:   // 单行；/* 多行 */
来源：http://gwy.sysykeji.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wvw.yueranfly.top

Go:   // 单行；/* 多行 */
来源：http://ztf.chenzaomai.com

Ruby: # 单行；=begin 多行 =end
来源：http://jyn.xinyue.icu

C#:   // 单行；/* 多行 */
来源：http://byx.sjlbkw.cn

[A15] 空值判断与默认值
来源：http://zeb.epnwcf.com

Py:   value = data or "默认值"
来源：http://lzg.yuanzhike.top

PHP:  $value = $data ?? "默认值";
来源：http://uka.zycfv.cn

JS:   const value = data ?? "默认值";
来源：http://upx.zhongyouzk.top

TS:   const value = data ?? "默认值";
来源：http://mod.jinqigfzy.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://crv.hfpthk.cn

Go:   if data == "" { data = "默认值" }
来源：http://juc.gzhubu.top

Ruby: value = data || "默认值"
来源：http://zej.ivvv.top

C#:   var value = data ?? "默认值";
来源：http://rll.ctjpmb.com

[A16] 真假值判断规则
来源：http://wve.fengsongda.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lqs.ybcxt.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://esw.ybcxt.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ljn.zhijiandao.cn

TS:   if (!x) {}
来源：http://pip.daxiang520.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kkt.pycfn.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ltg.hysaishi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tcb.zhongyouzk.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://iur.vqdsnc.cn

[A17] 位运算
来源：http://ykt.xylfe.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nqv.dashuyun.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cgg.aibaodan.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ihp.andypj.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rqo.nanxinkj.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gas.ppjwa.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fvq.hnqzz.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fpe.hfpthk.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oaa.gaohongyu789.top

[A18] 字符与 ASCII 码互转
来源：http://wae.hnxiangtu.top

Py:   ord("A"); chr(65)
来源：http://yny.hammf.cn

PHP:  ord("A"); chr(65)
来源：http://qro.fehbvm.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rqq.cheryme.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fop.feifeiyinyue.top

Java: (int) 'A'; (char) 65
来源：http://gcb.haohaochexian.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://utm.fanxiaobao.xyz

Ruby: "A".ord; 65.chr
来源：http://nuu.shanyushiyangtech.top

C#:   (int)'A'; (char)65
来源：http://uec.ctjpmb.com

[A19] 交换两个变量
来源：http://yoq.zycfv.cn

Py:   a, b = b, a
来源：http://nck.zhiwuduotai.top

PHP:  [$a, $b] = [$b, $a];
来源：http://vxd.daxiang520.top

JS:   [a, b] = [b, a];
来源：http://agc.shzxlz.cn

TS:   [a, b] = [b, a];
来源：http://iod.hongshengwenyu.top

Java: int t = a; a = b; b = t;
来源：http://exu.chenzaomai.com

Go:   a, b = b, a
来源：http://azu.cdnleiting.top

Ruby: a, b = b, a
来源：http://emh.tianlin.xyz

C#:   (a, b) = (b, a);
来源：http://esq.shangyingyoupin.top

[A20] 读取标准输入
来源：http://fxg.dashuyun.cn

Py:   name = input("请输入：")
来源：http://usu.fengsongda.top

PHP:  $name = trim(fgets(STDIN));
来源：http://lgp.kuanghao11.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://msr.cqqwz.cn

TS:   // Node.js：readline 模块
来源：http://jdo.zhiwuduotai.top

Java: new Scanner(System.in).nextLine()
来源：http://zvc.xingfuxueyuan.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gfv.shzxlz.cn

Ruby: gets.chomp
来源：http://wzi.jinqigfzy.top

C#:   Console.ReadLine();
来源：http://lbo.daria6918.cn

[A21] 保留指定小数位输出
来源：http://txd.ehwqpu.com

Py:   f"{3.14159:.2f}"
来源：http://rox.hysaishi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hkn.chenjidiqi.icu

JS:   (3.14159).toFixed(2)
来源：http://xdh.zycfv.cn

TS:   (3.14159).toFixed(2)
来源：http://smr.wangdashe.top

Java: String.format("%.2f", 3.14159)
来源：http://ftg.ywan-chungtsiang.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zsb.chenzaomai.com

Ruby: format("%.2f", 3.14159)
来源：http://ydo.ctjpmb.com

C#:   3.14159.ToString("F2")
来源：http://kan.yfazqb.com

[A22] 获取字符串长度
来源：http://kvg.cqqwz.cn

Py:   len(s)
来源：http://mtt.316326.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zdu.hfpthk.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://los.shzxlz.cn

TS:   s.length
来源：http://zjv.aizwys.cn

Java: s.length()
来源：http://mmh.zhongyouzk.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xgg.gaohongyu789.top

Ruby: s.length
来源：http://vju.sufxvd.cn

C#:   s.Length
来源：http://avd.jlsjyb.cn

[A23] 大小写转换
来源：http://ohc.andypj.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://xbq.hywenlv.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mxs.ehwqpu.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://low.52xcode.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ace.bbcook.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fks.cqqwz.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mqo.9152youxi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://olm.fzhhl.top

C#:   s.ToUpper(); s.ToLower()
来源：http://sbm.cqqwz.cn

[A24] 去除首尾空白
来源：http://ttd.yvedp.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rgb.quarkkingdee.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://thh.fengsongda.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rxf.yuanzhike.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jwg.zhiwuduotai.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://doa.feifeiyinyue.top

Go:   strings.TrimSpace(s)
来源：http://pot.hongshengwenyu.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ijb.zdqjudy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tzq.jqgufenzy.top

[A25] 字符串比较
来源：http://qii.gzhubu.top

Py:   s1 == s2; s1 != s2
来源：http://ssk.xuetiantiany.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ooo.redwolf501.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://axs.c1oappe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://eld.hnqzz.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rxv.ydjk.org.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qvg.yongpay.top

Ruby: s1 == s2; s1 <=> s2
来源：http://gfs.nanxuanxn.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kvk.c1oappe.top

[A26] 类型转换总览
来源：http://hil.xinyue.icu

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gbg.jinqigfzy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nwu.daria6918.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xmr.yj20258.top

TS:   Number() String() Boolean() x as number
来源：http://run.yfazqb.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lqz.hysaishi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://whb.tarul.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vqd.jinghuilouyu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rrw.daria6918.cn

================================================================================
来源：http://nyp.yonumen.top

B. 流程控制
来源：http://sfc.yueranfly.top

================================================================================
来源：http://gvh.jiagoushi.top

[B01] 条件判断 if / else
来源：http://kze.cucudq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lbs.snrcjt.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lel.hfpthk.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://aqu.zhaomingkeji.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uqk.gzhubu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://rcm.316326.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://arw.chenzaomai.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ysn.bjfxy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://khb.tanke756.top

[B02] 多分支 else if / elif
来源：http://eop.epnwcf.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ipv.cqqwz.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iwo.zhixingplan.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://egl.fengsongda.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jnd.fzhhl.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://szv.fzhhl.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uyx.guannengcc.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yje.redwolf501.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oei.gaohongyu789.top

[B03] switch / match / case
来源：http://ytt.c1oappe.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qsd.cqqwz.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ipg.316326.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://roq.gaohongyu789.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eyb.jlsjyb.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yjr.gzhubu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kva.c1oappe.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oqu.andypj.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nyb.jinghuilouyu.cn

[B04] for 计数循环
来源：http://oth.sxryk.cn

Py:   for i in range(10): print(i)
来源：http://lxv.wangdashe.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://upq.meibo888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://unw.cashguo.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lvc.hysaishi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jju.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uiw.uphjek.com

Ruby: 10.times { |i| puts i }
来源：http://pff.jinyuanbaomall.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://owe.chenlongwang.top

[B05] 遍历数组 / 列表
来源：http://qds.fengsongda.top

Py:   for item in arr: print(item)
来源：http://xty.cashguo.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://llr.meibo888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://dua.9152youxi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ygt.yvedp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hgp.yj20258888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fja.chenlongwang.top

Ruby: arr.each { |item| puts item }
来源：http://awz.zhoulong.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bce.zhengqikj.top

[B06] 遍历字典 / 对象
来源：http://sww.dianchejie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rzf.shzxlz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://emo.fzhhl.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://irr.chenzaomai.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lsh.zycfv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sve.epnwcf.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qca.dianchejie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gea.sxryk.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sof.smart0.xyz

[B07] while 循环
来源：http://efi.kuanghao11.cn

Py:   while i < 10: i += 1
来源：http://lnh.tian-w.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gmn.yj202588.top

JS:   while (i < 10) { i++; }
来源：http://iir.yj202588.top

TS:   while (i < 10) { i++; }
来源：http://yyj.hcnkem.com

Java: while (i < 10) { i++; }
来源：http://pyb.zhiwuduotai.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fqc.yongpay.top

Ruby: while i < 10; i += 1; end
来源：http://vzs.52xcode.cn

C#:   while (i < 10) { i++; }
来源：http://xjz.epnwcf.com

[B08] do-while（至少执行一次）
来源：http://ell.birdmap.top

Py:   # 无 do-while：用 while True + break
来源：http://qwz.fehbvm.com

PHP:  do { $i++; } while ($i < 10);
来源：http://jsr.dashuyun.cn

JS:   do { i++; } while (i < 10);
来源：http://dom.xuanzx.com

TS:   do { i++; } while (i < 10);
来源：http://xpg.vehdjk.com

Java: do { i++; } while (i < 10);
来源：http://zhb.redwolf501.top

Go:   for { i++; if i >= 10 { break } }
来源：http://llg.hammf.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qyq.jinqigfzy.top

C#:   do { i++; } while (i < 10);
来源：http://bcd.jiagoushi.top

[B09] break 与 continue
来源：http://tti.andypj.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wjw.jyoumei.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yrd.tanke756.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cmn.iojbl.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pyf.birdmap.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gat.jinqigufen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bnn.ivvv.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dry.havefunace.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cnk.svipenyu.cn

[B10] 遍历同时拿索引
来源：http://der.jinqigfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gus.ivvv.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lgw.tanke756.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zun.shuidangran.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xax.gogol.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://npv.chenlongwang.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xkv.zhixingplan.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fpt.cheryme.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gro.wangdashe.top

[B11] 生成数字序列 / 区间
来源：http://qzh.sysykeji.top

Py:   list(range(0, 10, 2))
来源：http://tei.shanyushiyangtech.top

PHP:  range(0, 10, 2);
来源：http://bvd.xingfuxueyuan.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zmw.zdqjudy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mcn.yangfankeji.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://quq.xuetiantiany.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mky.kuanghao11.cn

Ruby: (0...10).step(2).to_a
来源：http://jgc.zhiwuduotai.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ufr.tian-w.cn

[B12] 跳出多层循环
来源：http://adt.ydzc1.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://tdi.xuetiantiany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://loe.vqdsnc.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wjm.zhoulong.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tzp.yangfankeji.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pbv.jinghuilouyu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nsx.316326.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tqp.jyoumei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yvh.ydzc1.top

[B13] 判断是否为数字
来源：http://rku.fktsv.cn

Py:   isinstance(x, (int, float))
来源：http://xwx.feifeiyinyue.top

PHP:  is_numeric($x)
来源：http://yhl.chenlongwang.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fwi.yvedp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kmd.yangfankeji.com

Java: x instanceof Number
来源：http://jdx.fengsongda.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xof.gogol.net.cn

Ruby: x.is_a?(Numeric)
来源：http://znc.daxiang520.top


<!-- 参考信息 -->