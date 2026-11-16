代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dla.52xcode.cn

[A07] 数字转字符串
来源：http://wqy.cheryme.top

Py:   str(42)
来源：http://xmg.wangshuangyany.cn

PHP:  (string) 42; strval(42)
来源：http://mqi.pycfn.com

JS:   String(42); (42).toString()
来源：http://ozb.ctjpmb.com

TS:   String(42)
来源：http://lwu.cqqwz.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xne.zdqjudy.top

Go:   strconv.Itoa(42)
来源：http://egm.vqdsnc.cn

Ruby: 42.to_s
来源：http://idt.cqqwz.cn

C#:   42.ToString()
来源：http://eok.sysykeji.top

[A08] 取整与四舍五入
来源：http://osj.gotoacloud.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qvj.hammf.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dbt.sufxvd.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lnp.fehbvm.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://oqp.xylfe.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://iib.hfpthk.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vtn.0kj1m.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hai.dianchejie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tkz.feifeiyinyue.top

[A09] 绝对值与最大最小值
来源：http://czo.yongpay.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zys.cheryme.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lnd.fehbvm.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lkm.nanxuanxn.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://koe.yonumen.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mlx.fktsv.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xcv.sxryk.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dny.gotoacloud.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xus.daria6918.cn

[A10] 生成随机数
来源：http://kkc.gaohongyu789.top

Py:   import random; random.randint(1, 100)
来源：http://oga.shangyingyoupin.top

PHP:  random_int(1, 100);
来源：http://vcf.bbcook.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://prv.feifeiyinyue.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://img.yueranfly.top

Java: new Random().nextInt(100) + 1
来源：http://eeb.hcnkem.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://neg.birdmap.top

Ruby: rand(1..100)
来源：http://kqs.c1oappe.top

C#:   new Random().Next(1, 101)
来源：http://swd.guannengcc.top

[A11] 条件表达式（三元）
来源：http://tiv.dashuyun.cn

Py:   "yes" if x > 0 else "no"
来源：http://ati.aizwys.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cdg.ydzc1.top

JS:   x > 0 ? "yes" : "no"
来源：http://cmk.tarul.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hgp.jinqigfzy.top

Java: x > 0 ? "yes" : "no"
来源：http://brk.wangshuangyany.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ite.sufxvd.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ghv.gzhubu.top

C#:   x > 0 ? "yes" : "no"
来源：http://jbi.zdbjq.cn

[A12] 字符串插值 / 格式化
来源：http://uya.guowangkeji.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://oaa.zhongyouzk.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://aet.yuxming.cn

JS:   `Hello, ${name}!`
来源：http://kow.xinyue.icu

TS:   `Hello, ${name}!`
来源：http://nif.nanxuanxn.top

Java: "Hello, %s!".formatted(name)
来源：http://umu.gaohongyu789.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fmj.tarul.cn

Ruby: "Hello, #{name}!"
来源：http://qis.yj20258888.top

C#:   $"Hello, {name}!"
来源：http://auu.fzhhl.top

[A13] 多行字符串（练习 \n 转义）
来源：http://gkp.shangyingyoupin.top

Py:   "第一行\n第二行"
来源：http://itj.shangyingyoupin.top

PHP:  "第一行\n第二行"
来源：http://wvu.ppjwa.cn

JS:   "第一行\n第二行"
来源：http://ebo.shzxlz.cn

TS:   "第一行\n第二行"
来源：http://ith.chenjidiqi.icu

Java: "第一行\n第二行"
来源：http://jgj.pengpengdd.cyou

Go:   "第一行\n第二行"
来源：http://ofo.sysykeji.top

Ruby: "第一行\n第二行"
来源：http://wqt.svipenyu.cn

C#:   "第一行\n第二行"
来源：http://rds.chenzaomai.com

[A14] 注释写法
来源：http://jpa.hfpthk.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ugt.gzhubu.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://nco.xuanzx.com

JS:   // 单行；/* 多行 */
来源：http://yom.sufxvd.cn

TS:   // 单行；/* 多行 */
来源：http://rlo.nwbrower.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pre.shangyingyoupin.top

Go:   // 单行；/* 多行 */
来源：http://mws.jqgfzy.top

Ruby: # 单行；=begin 多行 =end
来源：http://zuy.gotoacloud.top

C#:   // 单行；/* 多行 */
来源：http://sji.birdmap.top

[A15] 空值判断与默认值
来源：http://kil.hnxiangtu.top

Py:   value = data or "默认值"
来源：http://kgs.yangfankeji.com

PHP:  $value = $data ?? "默认值";
来源：http://pjm.shuidangran.top

JS:   const value = data ?? "默认值";
来源：http://ver.yongpay.top

TS:   const value = data ?? "默认值";
来源：http://cwq.feifeiyinyue.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wea.yanxiufei.cn

Go:   if data == "" { data = "默认值" }
来源：http://jen.kuanghao11.cn

Ruby: value = data || "默认值"
来源：http://ndf.birdmap.top

C#:   var value = data ?? "默认值";
来源：http://tye.xuetiantiany.cn

[A16] 真假值判断规则
来源：http://qpv.vqdsnc.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://way.pycfn.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://muq.tian-w.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://oad.0kj1m.cn

TS:   if (!x) {}
来源：http://wof.bjfxy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://iwg.cqqwz.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lbi.quarkkingdee.top

Ruby: unless x            # nil 与 false 为假
来源：http://okz.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cwh.shzxlz.cn

[A17] 位运算
来源：http://dkl.ydjk.org.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ure.shangyingyoupin.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lzy.chenzaomai.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://srg.52xcode.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dtq.vqdsnc.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kcv.wangshuangyany.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://syr.hesvh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://okg.hywenlv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hqh.havefunace.top

[A18] 字符与 ASCII 码互转
来源：http://fad.hywenlv.cn

Py:   ord("A"); chr(65)
来源：http://bgo.sysykeji.top

PHP:  ord("A"); chr(65)
来源：http://vrc.yueranfly.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kdn.xylfe.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kma.mhx1999.top

Java: (int) 'A'; (char) 65
来源：http://hyu.smart0.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tuo.yj20258.top

Ruby: "A".ord; 65.chr
来源：http://mmp.jqgufenzy.top

C#:   (int)'A'; (char)65
来源：http://zrf.jinghuilouyu.cn

[A19] 交换两个变量
来源：http://ipz.aizwys.cn

Py:   a, b = b, a
来源：http://sld.havefunace.top

PHP:  [$a, $b] = [$b, $a];
来源：http://dwe.yueranfly.top

JS:   [a, b] = [b, a];
来源：http://rbe.andypj.xyz

TS:   [a, b] = [b, a];
来源：http://kpl.sxryk.cn

Java: int t = a; a = b; b = t;
来源：http://rms.zhiwuduotai.top

Go:   a, b = b, a
来源：http://csr.gaohongyu789.top

Ruby: a, b = b, a
来源：http://lut.ehwqpu.com

C#:   (a, b) = (b, a);
来源：http://vzv.zhengqikj.top

[A20] 读取标准输入
来源：http://xnu.vqdsnc.cn

Py:   name = input("请输入：")
来源：http://jkd.gotoacloud.top

PHP:  $name = trim(fgets(STDIN));
来源：http://gol.meibo888.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://puh.jqgfzy.top

TS:   // Node.js：readline 模块
来源：http://sjc.meibo888.top

Java: new Scanner(System.in).nextLine()
来源：http://xuv.yj20258888.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://crh.xylfe.cn

Ruby: gets.chomp
来源：http://egb.shanyushiyangkeji.top

C#:   Console.ReadLine();
来源：http://cru.pengpengdd.cyou

[A21] 保留指定小数位输出
来源：http://mdc.vehdjk.com

Py:   f"{3.14159:.2f}"
来源：http://txm.zhengqikj.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jvn.andypj.xyz

JS:   (3.14159).toFixed(2)
来源：http://krq.hfpthk.cn

TS:   (3.14159).toFixed(2)
来源：http://wpf.zhaomingkeji.xyz

Java: String.format("%.2f", 3.14159)
来源：http://opm.hesvh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wcx.xziqi.cn

Ruby: format("%.2f", 3.14159)
来源：http://fyf.nanxinkj.top

C#:   3.14159.ToString("F2")
来源：http://xya.yueranfly.top

[A22] 获取字符串长度
来源：http://axv.mhx1999.top

Py:   len(s)
来源：http://jif.daxiang520.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xef.yj20258888.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jhm.shanyushiyangtech.top

TS:   s.length
来源：http://ukt.cheryme.top

Java: s.length()
来源：http://jfw.jinqigufen.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zse.jqgufenzy.top

Ruby: s.length
来源：http://yot.vehdjk.com

C#:   s.Length
来源：http://qiy.hywenlv.cn

[A23] 大小写转换
来源：http://grj.jianghu66.top

Py:   s.upper(); s.lower(); s.title()
来源：http://hxl.jinqigufen.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mha.hysaishi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nkv.birdmap.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://myb.snrcjt.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fky.pengpengdd.cyou

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vez.daria6918.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ume.52xcode.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vrk.jinqigufen.top

[A24] 去除首尾空白
来源：http://rqj.cucudq.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bhm.quarkkingdee.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cnv.iojbl.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gje.vqdsnc.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qam.jinqigufen.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://agx.gzhubu.top

Go:   strings.TrimSpace(s)
来源：http://lzy.iojbl.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ark.yfazqb.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://myg.daxiang520.top

[A25] 字符串比较
来源：http://mof.zdqjudy.top

Py:   s1 == s2; s1 != s2
来源：http://ppa.52xcode.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nqr.daxiang520.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ptj.9152youxi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hzo.hnxiangtu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oaz.ybcxt.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nui.zdbjq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://oxv.redwolf501.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://eci.xziqi.cn

[A26] 类型转换总览
来源：http://fiu.xziqi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://onm.ydzc1.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://trw.zycfv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ufr.daria6918.cn

TS:   Number() String() Boolean() x as number
来源：http://vtc.jianghu66.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jtz.zhiwuduotai.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tts.cucudq.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vcx.wangdashe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rao.epnwcf.com

================================================================================
来源：http://ulb.andypj.xyz

B. 流程控制
来源：http://nlg.hongshengwenyu.top

================================================================================
来源：http://qba.xziqi.cn

[B01] 条件判断 if / else
来源：http://rzj.hongshengwenyu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://oma.aizwys.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sdo.hysaishi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wqk.jinyuanbaomall.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vlq.tianlin.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://hqq.nanxuanxn.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fyb.xinyue.icu

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ypa.meibo888.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qrw.jianghu66.top

[B02] 多分支 else if / elif
来源：http://itd.haohaochexian.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ius.yonumen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://abr.svipenyu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://olb.hongshengwenyu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mur.ydjk.org.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wqx.hcnkem.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zgk.zhongyouzk.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jjx.fanxiaobao.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ozs.yangfankeji.com

[B03] switch / match / case
来源：http://car.feifeiyinyue.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://phx.daria6918.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zii.zhaomingkeji.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mvb.wangshuangyany.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://irg.0kj1m.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bim.aizwys.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nzg.shzxlz.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dbe.zdbjq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://oqf.gaohongyu789.top

[B04] for 计数循环
来源：http://etm.ctjpmb.com

Py:   for i in range(10): print(i)
来源：http://wis.gotoacloud.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://abw.hammf.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tfu.cucudq.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ucp.pengpengdd.cyou

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fcl.chenjidiqi.icu

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yew.ydjk.org.cn

Ruby: 10.times { |i| puts i }
来源：http://jth.zhengqikj.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xut.tarul.cn

[B05] 遍历数组 / 列表
来源：http://taz.sjlbkw.cn

Py:   for item in arr: print(item)
来源：http://mhn.zhoulong.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dng.yongpay.top

JS:   for (const item of arr) { console.log(item); }
来源：http://rfs.hammf.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wrk.hongshengwenyu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://xbq.meibo888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nyx.nanxinkj.top

Ruby: arr.each { |item| puts item }
来源：http://goa.yanxiufei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://okk.cqqwz.cn

[B06] 遍历字典 / 对象
来源：http://xsq.316326.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://wpq.sysykeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bpu.cdnleiting.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://olp.sjlbkw.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lpv.svipenyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xza.feifeiyinyue.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wcm.aizwys.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dhd.jqgufenzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yab.zdqjudy.top

[B07] while 循环
来源：http://moo.iojbl.cn

Py:   while i < 10: i += 1
来源：http://qmr.quarkkingdee.top

PHP:  while ($i < 10) { $i++; }
来源：http://xat.hammf.cn

JS:   while (i < 10) { i++; }
来源：http://fcl.iojbl.cn

TS:   while (i < 10) { i++; }
来源：http://kix.pengpengdd.cyou

Java: while (i < 10) { i++; }
来源：http://qyw.xuetiantiany.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qhk.uphjek.com

Ruby: while i < 10; i += 1; end
来源：http://opd.hongshengwenyu.top

C#:   while (i < 10) { i++; }
来源：http://jwg.feifeiyinyue.top

[B08] do-while（至少执行一次）
来源：http://gnt.guannengcc.top

Py:   # 无 do-while：用 while True + break
来源：http://lyh.hesvh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vkf.0kj1m.cn

JS:   do { i++; } while (i < 10);
来源：http://kse.aibaodan.cn

TS:   do { i++; } while (i < 10);
来源：http://alp.yfazqb.com

Java: do { i++; } while (i < 10);
来源：http://kko.9152youxi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://knc.shanyushiyangtech.top

Ruby: begin; i += 1; end while i < 10
来源：http://jho.jinghuilouyu.cn

C#:   do { i++; } while (i < 10);
来源：http://neq.daria6918.cn

[B09] break 与 continue
来源：http://exd.zhixingplan.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ogj.hywenlv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vii.shangyingyoupin.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nvi.chenlongwang.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sbb.jlsjyb.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://psi.snrcjt.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cll.gogol.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qvl.9152youxi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wia.hesvh.cn

[B10] 遍历同时拿索引
来源：http://lfu.cashguo.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://psz.cucudq.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kqa.hnxiangtu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rxy.jqgufenzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lnm.zhongyouzk.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vyl.aizwys.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yfy.zhaomingkeji.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yfm.fktsv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hbf.yj20258888.top

[B11] 生成数字序列 / 区间
来源：http://npy.bjfxy.top

Py:   list(range(0, 10, 2))
来源：http://ijx.sufxvd.cn

PHP:  range(0, 10, 2);
来源：http://gzi.tian-w.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sla.ivvv.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gvw.xuanzx.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pct.yj202588.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://iyx.jinqigufen.top

Ruby: (0...10).step(2).to_a
来源：http://jen.ehwqpu.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zqa.zhijiandao.cn

[B12] 跳出多层循环
来源：http://eqr.wangshuangyany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kee.sxryk.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wqg.tanke756.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oil.dianchejie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ahf.haohaochexian.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://moy.xinyue.icu

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ohw.meibo888.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mei.fzhhl.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pbx.fehbvm.com

[B13] 判断是否为数字
来源：http://cjn.uphjek.com

Py:   isinstance(x, (int, float))
来源：http://zrf.birdmap.top

PHP:  is_numeric($x)
来源：http://fdp.yangfankeji.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bgq.birdmap.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sei.fanxiaobao.xyz

Java: x instanceof Number
来源：http://fer.smart0.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bbf.0kj1m.cn

Ruby: x.is_a?(Numeric)
来源：http://lvz.hnxiangtu.top


<!-- 参考信息 -->