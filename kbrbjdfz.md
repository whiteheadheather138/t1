代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://geq.xingfuxueyuan.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yiy.fzhhl.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uxk.xuanzx.com

Ruby: "42".to_i; "3.14".to_f
来源：http://jpx.daxiang520.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://njr.uphjek.com

[A07] 数字转字符串
来源：http://tyq.hammf.cn

Py:   str(42)
来源：http://bgj.52xcode.cn

PHP:  (string) 42; strval(42)
来源：http://baj.meibo888.top

JS:   String(42); (42).toString()
来源：http://qii.gogol.net.cn

TS:   String(42)
来源：http://ejw.cashguo.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://kof.jinyuanbaomall.cn

Go:   strconv.Itoa(42)
来源：http://vvf.sxryk.cn

Ruby: 42.to_s
来源：http://gyn.yj20258.top

C#:   42.ToString()
来源：http://ntc.52xcode.cn

[A08] 取整与四舍五入
来源：http://syb.ctjpmb.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kub.wangshuangyany.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yfc.bbcook.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tvp.cashguo.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gef.hongshengwenyu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://trw.sufxvd.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wcl.yanxiufei.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wct.sweek.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vsz.sweek.top

[A09] 绝对值与最大最小值
来源：http://yrx.guowangkeji.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://umf.zhongyouzk.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://awn.yongpay.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rzw.hesvh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fyj.jinqigfzy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://opo.sxryk.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gxe.shanyushiyangkeji.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qch.svipenyu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pqr.dianchejie.cn

[A10] 生成随机数
来源：http://bdo.hywenlv.cn

Py:   import random; random.randint(1, 100)
来源：http://cow.jyoumei.cn

PHP:  random_int(1, 100);
来源：http://eme.zhijiandao.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dwz.wangshuangyany.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://swd.sufxvd.cn

Java: new Random().nextInt(100) + 1
来源：http://nxs.tian-w.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xpz.feifeiyinyue.top

Ruby: rand(1..100)
来源：http://zhh.iojbl.cn

C#:   new Random().Next(1, 101)
来源：http://nzk.c1oappe.top

[A11] 条件表达式（三元）
来源：http://fpr.yj20258.top

Py:   "yes" if x > 0 else "no"
来源：http://lbo.quarkkingdee.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://psy.gaohongyu789.top

JS:   x > 0 ? "yes" : "no"
来源：http://chk.hcnkem.com

TS:   x > 0 ? "yes" : "no"
来源：http://znw.feifeiyinyue.top

Java: x > 0 ? "yes" : "no"
来源：http://cdw.meibo888.top

Go:   // 无三元运算符，需用 if 语句
来源：http://duh.jinghuilouyu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://wtt.mhx1999.top

C#:   x > 0 ? "yes" : "no"
来源：http://waa.sjlbkw.cn

[A12] 字符串插值 / 格式化
来源：http://kqo.havefunace.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qra.hysaishi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gcp.wangshuangyany.cn

JS:   `Hello, ${name}!`
来源：http://afg.wangshuangyany.cn

TS:   `Hello, ${name}!`
来源：http://sgj.ivvv.top

Java: "Hello, %s!".formatted(name)
来源：http://ksp.aibaodan.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jmf.sufxvd.cn

Ruby: "Hello, #{name}!"
来源：http://sce.zdbjq.cn

C#:   $"Hello, {name}!"
来源：http://jpy.pengpengdd.cyou

[A13] 多行字符串（练习 \n 转义）
来源：http://dht.yuxming.cn

Py:   "第一行\n第二行"
来源：http://lhj.jianghu66.top

PHP:  "第一行\n第二行"
来源：http://hfl.tarul.cn

JS:   "第一行\n第二行"
来源：http://wcb.jqgfzy.top

TS:   "第一行\n第二行"
来源：http://slo.yj202588.top

Java: "第一行\n第二行"
来源：http://ylb.52xcode.cn

Go:   "第一行\n第二行"
来源：http://qsi.xingfuxueyuan.xyz

Ruby: "第一行\n第二行"
来源：http://hni.yj202588.top

C#:   "第一行\n第二行"
来源：http://rjn.yongpay.top

[A14] 注释写法
来源：http://dkq.jinghuilouyu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cso.tianlin.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://uiw.bbcook.cn

JS:   // 单行；/* 多行 */
来源：http://req.meibo888.top

TS:   // 单行；/* 多行 */
来源：http://qod.jiagoushi.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ydp.ppjwa.cn

Go:   // 单行；/* 多行 */
来源：http://tkd.bbcook.cn

Ruby: # 单行；=begin 多行 =end
来源：http://yqn.xingfuxueyuan.xyz

C#:   // 单行；/* 多行 */
来源：http://wcm.cashguo.top

[A15] 空值判断与默认值
来源：http://cbk.chenlongwang.top

Py:   value = data or "默认值"
来源：http://anr.shzxlz.cn

PHP:  $value = $data ?? "默认值";
来源：http://ehr.yj20258888.top

JS:   const value = data ?? "默认值";
来源：http://mhz.feifeiyinyue.top

TS:   const value = data ?? "默认值";
来源：http://tao.ivvv.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wnm.aibaodan.cn

Go:   if data == "" { data = "默认值" }
来源：http://lnb.zdqjudy.top

Ruby: value = data || "默认值"
来源：http://zql.cqqwz.cn

C#:   var value = data ?? "默认值";
来源：http://pnd.hfpthk.cn

[A16] 真假值判断规则
来源：http://rjg.chenjidiqi.icu

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://khu.aizwys.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ipb.smart0.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://azi.smart0.xyz

TS:   if (!x) {}
来源：http://dxn.birdmap.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vrw.yuanzhike.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ggy.epnwcf.com

Ruby: unless x            # nil 与 false 为假
来源：http://bvb.quarkkingdee.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pjo.xingfuxueyuan.xyz

[A17] 位运算
来源：http://rif.yvedp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zva.gaohongyu789.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://eqb.bbcook.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wnh.bjfxy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bap.yangfankeji.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ejg.hywenlv.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jfx.jinqigfzy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vga.zhixingplan.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wrr.jlsjyb.cn

[A18] 字符与 ASCII 码互转
来源：http://mcd.quarkkingdee.top

Py:   ord("A"); chr(65)
来源：http://aig.sjlbkw.cn

PHP:  ord("A"); chr(65)
来源：http://sky.cdnleiting.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://upi.sweek.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tys.ehwqpu.com

Java: (int) 'A'; (char) 65
来源：http://dfc.redwolf501.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ani.zhoulong.xyz

Ruby: "A".ord; 65.chr
来源：http://zly.ppjwa.cn

C#:   (int)'A'; (char)65
来源：http://lak.shanyushiyangkeji.top

[A19] 交换两个变量
来源：http://qcw.hammf.cn

Py:   a, b = b, a
来源：http://rxq.tianlin.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://pyw.yj20258.top

JS:   [a, b] = [b, a];
来源：http://oid.yj20258.top

TS:   [a, b] = [b, a];
来源：http://rhr.fengsongda.top

Java: int t = a; a = b; b = t;
来源：http://ypu.andypj.xyz

Go:   a, b = b, a
来源：http://sao.yongpay.top

Ruby: a, b = b, a
来源：http://ezh.bjfxy.top

C#:   (a, b) = (b, a);
来源：http://hji.uphjek.com

[A20] 读取标准输入
来源：http://neb.cashguo.top

Py:   name = input("请输入：")
来源：http://kym.feifeiyinyue.top

PHP:  $name = trim(fgets(STDIN));
来源：http://zhs.tian-w.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xky.wangdashe.top

TS:   // Node.js：readline 模块
来源：http://unw.jqgufenzy.top

Java: new Scanner(System.in).nextLine()
来源：http://cgd.jinghuilouyu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://eui.gotoacloud.top

Ruby: gets.chomp
来源：http://jga.pengpengdd.cyou

C#:   Console.ReadLine();
来源：http://vkt.fzhhl.top

[A21] 保留指定小数位输出
来源：http://dld.zhijiandao.cn

Py:   f"{3.14159:.2f}"
来源：http://mru.nwbrower.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cmr.yongpay.top

JS:   (3.14159).toFixed(2)
来源：http://luu.hammf.cn

TS:   (3.14159).toFixed(2)
来源：http://oex.quarkkingdee.top

Java: String.format("%.2f", 3.14159)
来源：http://oxj.kuanghao11.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dcj.cqqwz.cn

Ruby: format("%.2f", 3.14159)
来源：http://rgx.jlsjyb.cn

C#:   3.14159.ToString("F2")
来源：http://fuu.shzxlz.cn

[A22] 获取字符串长度
来源：http://nae.sufxvd.cn

Py:   len(s)
来源：http://efq.zdbjq.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uuo.ppjwa.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cdy.nanxuanxn.top

TS:   s.length
来源：http://xjn.fanxiaobao.xyz

Java: s.length()
来源：http://xqb.yj20258888.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://spv.fktsv.cn

Ruby: s.length
来源：http://bdc.xylfe.cn

C#:   s.Length
来源：http://vcv.jinqigufen.top

[A23] 大小写转换
来源：http://yhv.shzxlz.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://saf.zhaomingkeji.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hqj.gaohongyu789.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fet.birdmap.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rle.52xcode.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ukh.havefunace.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://apq.uphjek.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jja.xinyue.icu

C#:   s.ToUpper(); s.ToLower()
来源：http://kqk.uphjek.com

[A24] 去除首尾空白
来源：http://oxw.xuanzx.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rhk.shangyingyoupin.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ley.meibo888.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uxh.shuidangran.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pxj.tarul.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ppz.svipenyu.cn

Go:   strings.TrimSpace(s)
来源：http://tco.yfazqb.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ghs.yonumen.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gkw.zdbjq.cn

[A25] 字符串比较
来源：http://bad.ctjpmb.com

Py:   s1 == s2; s1 != s2
来源：http://geh.gzhubu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kek.cdnleiting.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lsr.zycfv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://crc.feifeiyinyue.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nxy.feifeiyinyue.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fhu.sjlbkw.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bky.bjfxy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ecy.hywenlv.cn

[A26] 类型转换总览
来源：http://oqt.zhixingplan.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tvv.quarkkingdee.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ehc.chenzaomai.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vmi.yueranfly.top

TS:   Number() String() Boolean() x as number
来源：http://ulz.zhongyouzk.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://odx.mhx1999.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cfh.andypj.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://ptq.316326.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yki.yj20258.top

================================================================================
来源：http://oqs.yj202588.top

B. 流程控制
来源：http://sle.jqgfzy.top

================================================================================
来源：http://oem.feifeiyinyue.top

[B01] 条件判断 if / else
来源：http://lpt.fanxiaobao.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://yuw.sxryk.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qmk.wangshuangyany.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://efd.chenzaomai.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://djr.xingfuxueyuan.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://fjk.haohaochexian.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qvd.gaohongyu789.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mpy.yj202588.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tdu.zhengqikj.top

[B02] 多分支 else if / elif
来源：http://tzn.zhengqikj.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cuq.yongpay.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bvn.zhiwuduotai.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jlo.sxryk.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xmr.316326.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ftz.wangdashe.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iov.dashuyun.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uyf.wangdashe.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hgp.pengpengdd.cyou

[B03] switch / match / case
来源：http://lvt.ctjpmb.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lrm.jianghu66.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oqn.hnxiangtu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ibe.9152youxi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ksn.jinqigufen.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://euu.shangyingyoupin.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bmv.nanxinkj.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://stf.yonumen.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ode.nanxuanxn.top

[B04] for 计数循环
来源：http://swc.yueranfly.top

Py:   for i in range(10): print(i)
来源：http://rda.yuanzhike.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://icl.dianchejie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vkc.xziqi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sql.zycfv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yjd.cqqwz.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ojg.pycfn.com

Ruby: 10.times { |i| puts i }
来源：http://piw.guowangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://icd.tianlin.xyz

[B05] 遍历数组 / 列表
来源：http://eht.jianghu66.top

Py:   for item in arr: print(item)
来源：http://drc.iojbl.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gsm.ydzc1.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ebu.nanxinkj.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qhn.hysaishi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xsi.shanyushiyangtech.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jtj.uphjek.com

Ruby: arr.each { |item| puts item }
来源：http://vvh.sysykeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://meb.hfpthk.cn

[B06] 遍历字典 / 对象
来源：http://fpq.chenjidiqi.icu

Py:   for k, v in d.items(): print(k, v)
来源：http://wio.guannengcc.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qnp.jlsjyb.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rpd.pycfn.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gwg.jinghuilouyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ywx.zhiwuduotai.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cax.zdbjq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iae.pycfn.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ojz.zhengqikj.top

[B07] while 循环
来源：http://tpg.ybcxt.top

Py:   while i < 10: i += 1
来源：http://yzn.nanxinkj.top

PHP:  while ($i < 10) { $i++; }
来源：http://zrp.wangshuangyany.cn

JS:   while (i < 10) { i++; }
来源：http://kmt.ydjk.org.cn

TS:   while (i < 10) { i++; }
来源：http://mtt.yj202588.top

Java: while (i < 10) { i++; }
来源：http://yrk.guowangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xzw.jinqigfzy.top

Ruby: while i < 10; i += 1; end
来源：http://ago.shanyushiyangkeji.top

C#:   while (i < 10) { i++; }
来源：http://oaa.nwbrower.top

[B08] do-while（至少执行一次）
来源：http://iar.hnxiangtu.top

Py:   # 无 do-while：用 while True + break
来源：http://yqu.zhiwuduotai.top

PHP:  do { $i++; } while ($i < 10);
来源：http://wzr.shanyushiyangkeji.top

JS:   do { i++; } while (i < 10);
来源：http://uyt.fzhhl.top

TS:   do { i++; } while (i < 10);
来源：http://jkg.sweek.top

Java: do { i++; } while (i < 10);
来源：http://nfd.jinghuilouyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uvz.xuanzx.com

Ruby: begin; i += 1; end while i < 10
来源：http://oit.uphjek.com

C#:   do { i++; } while (i < 10);
来源：http://mhe.hysaishi.cn

[B09] break 与 continue
来源：http://plu.smart0.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dhy.hnqzz.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hzr.meibo888.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yeq.yuxming.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uua.cashguo.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ure.jinghuilouyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kzb.fktsv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bkd.gzhubu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ozu.hcnkem.com

[B10] 遍历同时拿索引
来源：http://nku.haohaochexian.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lvt.jqgfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hqh.shuidangran.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nji.ywan-chungtsiang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uku.zhiwuduotai.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://czg.yuanzhike.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jyb.gotoacloud.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ymg.ywan-chungtsiang.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iie.uphjek.com

[B11] 生成数字序列 / 区间
来源：http://tis.hfpthk.cn

Py:   list(range(0, 10, 2))
来源：http://eth.zhaomingkeji.xyz

PHP:  range(0, 10, 2);
来源：http://qoe.sxryk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://knz.smart0.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wnx.dashuyun.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tvg.cdnleiting.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yoc.redwolf501.top

Ruby: (0...10).step(2).to_a
来源：http://kgl.ctjpmb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tdj.jinyuanbaomall.cn

[B12] 跳出多层循环
来源：http://acp.dianchejie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://abs.cqqwz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jgy.jinyuanbaomall.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yzz.cheryme.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://brw.xuetiantiany.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xal.guowangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fxl.yonumen.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://udg.vqdsnc.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dio.kuanghao11.cn

[B13] 判断是否为数字
来源：http://qlu.zdqjudy.top

Py:   isinstance(x, (int, float))
来源：http://xhk.ywan-chungtsiang.top

PHP:  is_numeric($x)
来源：http://krl.aibaodan.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rcv.hongshengwenyu.top


<!-- 参考信息 -->