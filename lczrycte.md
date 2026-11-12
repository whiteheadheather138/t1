代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hwq.meibo888.top

[A07] 数字转字符串
来源：http://rry.jyoumei.cn

Py:   str(42)
来源：http://jwn.tian-w.cn

PHP:  (string) 42; strval(42)
来源：http://gjf.gaohongyu789.top

JS:   String(42); (42).toString()
来源：http://iym.redwolf501.top

TS:   String(42)
来源：http://ord.shanyushiyangtech.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://stk.c1oappe.top

Go:   strconv.Itoa(42)
来源：http://mpv.ydzc1.top

Ruby: 42.to_s
来源：http://uvu.gzhubu.top

C#:   42.ToString()
来源：http://koj.yongpay.top

[A08] 取整与四舍五入
来源：http://dje.meibo888.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fup.andypj.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fko.iojbl.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zvg.dianchejie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://msq.bbcook.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hyc.jinghuilouyu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qeg.meibo888.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://qgf.zhixingplan.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fjh.daria6918.cn

[A09] 绝对值与最大最小值
来源：http://wle.haohaochexian.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pcr.jinyuanbaomall.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qtl.tanke756.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ien.haohaochexian.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cjz.nanxuanxn.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ses.aizwys.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cje.gotoacloud.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lsv.yuxming.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wjg.jlsjyb.cn

[A10] 生成随机数
来源：http://cxh.yuxming.cn

Py:   import random; random.randint(1, 100)
来源：http://juq.yongpay.top

PHP:  random_int(1, 100);
来源：http://epf.chenzaomai.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uvv.yonumen.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ffi.gzhubu.top

Java: new Random().nextInt(100) + 1
来源：http://nmm.gaohongyu789.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yqz.hnqzz.top

Ruby: rand(1..100)
来源：http://kbf.hywenlv.cn

C#:   new Random().Next(1, 101)
来源：http://hiw.bjfxy.top

[A11] 条件表达式（三元）
来源：http://fwv.fanxiaobao.xyz

Py:   "yes" if x > 0 else "no"
来源：http://iwy.zhiwuduotai.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://isu.jinyuanbaomall.cn

JS:   x > 0 ? "yes" : "no"
来源：http://uvp.zhaomingkeji.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://gcs.ctjpmb.com

Java: x > 0 ? "yes" : "no"
来源：http://nxg.jinyuanbaomall.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://uvw.cqqwz.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://okq.yongpay.top

C#:   x > 0 ? "yes" : "no"
来源：http://gia.havefunace.top

[A12] 字符串插值 / 格式化
来源：http://yic.bjfxy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vas.c1oappe.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://siw.tanke756.top

JS:   `Hello, ${name}!`
来源：http://uxs.pengpengdd.cyou

TS:   `Hello, ${name}!`
来源：http://pok.fengsongda.top

Java: "Hello, %s!".formatted(name)
来源：http://tup.pengpengdd.cyou

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jjj.jinqigufen.top

Ruby: "Hello, #{name}!"
来源：http://pwi.xingfuxueyuan.xyz

C#:   $"Hello, {name}!"
来源：http://wwh.hongshengwenyu.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ixd.andypj.xyz

Py:   "第一行\n第二行"
来源：http://noo.hfpthk.cn

PHP:  "第一行\n第二行"
来源：http://fnw.jinyuanbaomall.cn

JS:   "第一行\n第二行"
来源：http://usx.jlsjyb.cn

TS:   "第一行\n第二行"
来源：http://zfv.daria6918.cn

Java: "第一行\n第二行"
来源：http://nqo.yj20258888.top

Go:   "第一行\n第二行"
来源：http://rhz.guannengcc.top

Ruby: "第一行\n第二行"
来源：http://emk.ppjwa.cn

C#:   "第一行\n第二行"
来源：http://tpy.zycfv.cn

[A14] 注释写法
来源：http://kel.zhijiandao.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ahz.zhaomingkeji.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://fnp.sxryk.cn

JS:   // 单行；/* 多行 */
来源：http://zpd.aibaodan.cn

TS:   // 单行；/* 多行 */
来源：http://agr.jqgufenzy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ltl.cqqwz.cn

Go:   // 单行；/* 多行 */
来源：http://nro.zdqjudy.top

Ruby: # 单行；=begin 多行 =end
来源：http://vaq.quarkkingdee.top

C#:   // 单行；/* 多行 */
来源：http://pjq.shanyushiyangtech.top

[A15] 空值判断与默认值
来源：http://huq.hfpthk.cn

Py:   value = data or "默认值"
来源：http://eyr.shanyushiyangkeji.top

PHP:  $value = $data ?? "默认值";
来源：http://xfh.sxryk.cn

JS:   const value = data ?? "默认值";
来源：http://kje.0kj1m.cn

TS:   const value = data ?? "默认值";
来源：http://foo.jinghuilouyu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tfz.shanyushiyangtech.top

Go:   if data == "" { data = "默认值" }
来源：http://zji.sjlbkw.cn

Ruby: value = data || "默认值"
来源：http://jua.xinyue.icu

C#:   var value = data ?? "默认值";
来源：http://slt.chenzaomai.com

[A16] 真假值判断规则
来源：http://gyx.yj202588.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jrf.nanxuanxn.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xxe.sufxvd.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pwf.tarul.cn

TS:   if (!x) {}
来源：http://tse.vehdjk.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://okk.cheryme.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cak.zhijiandao.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lly.ivvv.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fok.c1oappe.top

[A17] 位运算
来源：http://yae.hongshengwenyu.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lpg.hnqzz.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kni.hywenlv.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://giy.iojbl.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://orh.hesvh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xzn.jiagoushi.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vvo.nwbrower.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uiz.yuxming.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lot.hammf.cn

[A18] 字符与 ASCII 码互转
来源：http://vyq.yonumen.top

Py:   ord("A"); chr(65)
来源：http://eta.hfpthk.cn

PHP:  ord("A"); chr(65)
来源：http://msb.fktsv.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sco.zhijiandao.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qnf.aibaodan.cn

Java: (int) 'A'; (char) 65
来源：http://ynd.hfpthk.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ohh.yj20258.top

Ruby: "A".ord; 65.chr
来源：http://hpb.ppjwa.cn

C#:   (int)'A'; (char)65
来源：http://kzj.ivvv.top

[A19] 交换两个变量
来源：http://jjk.yueranfly.top

Py:   a, b = b, a
来源：http://ula.tianlin.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://imm.ehwqpu.com

JS:   [a, b] = [b, a];
来源：http://nve.dianchejie.cn

TS:   [a, b] = [b, a];
来源：http://aff.hongshengwenyu.top

Java: int t = a; a = b; b = t;
来源：http://haf.xuetiantiany.cn

Go:   a, b = b, a
来源：http://cba.fehbvm.com

Ruby: a, b = b, a
来源：http://kic.redwolf501.top

C#:   (a, b) = (b, a);
来源：http://mer.hnqzz.top

[A20] 读取标准输入
来源：http://tlw.vehdjk.com

Py:   name = input("请输入：")
来源：http://bsl.wangdashe.top

PHP:  $name = trim(fgets(STDIN));
来源：http://evq.sweek.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ubx.bbcook.cn

TS:   // Node.js：readline 模块
来源：http://mnz.zhixingplan.top

Java: new Scanner(System.in).nextLine()
来源：http://ogo.daria6918.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ier.52xcode.cn

Ruby: gets.chomp
来源：http://jsh.ivvv.top

C#:   Console.ReadLine();
来源：http://inj.52xcode.cn

[A21] 保留指定小数位输出
来源：http://acx.zhijiandao.cn

Py:   f"{3.14159:.2f}"
来源：http://mbu.iojbl.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jbj.fanxiaobao.xyz

JS:   (3.14159).toFixed(2)
来源：http://srs.guannengcc.top

TS:   (3.14159).toFixed(2)
来源：http://owb.haohaochexian.top

Java: String.format("%.2f", 3.14159)
来源：http://rlo.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tco.xuetiantiany.cn

Ruby: format("%.2f", 3.14159)
来源：http://bfe.tanke756.top

C#:   3.14159.ToString("F2")
来源：http://akh.cheryme.top

[A22] 获取字符串长度
来源：http://tiw.andypj.xyz

Py:   len(s)
来源：http://wqn.guowangkeji.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uxa.wangshuangyany.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lvf.yuanzhike.top

TS:   s.length
来源：http://zpv.hcnkem.com

Java: s.length()
来源：http://czt.tianlin.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bbf.hcnkem.com

Ruby: s.length
来源：http://qog.andypj.xyz

C#:   s.Length
来源：http://nqu.ivvv.top

[A23] 大小写转换
来源：http://trt.jlsjyb.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vtm.hcnkem.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bxa.yuxming.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://imc.hywenlv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ctf.zhixingplan.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ofg.havefunace.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zjc.aizwys.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ivi.wangshuangyany.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ljy.kuanghao11.cn

[A24] 去除首尾空白
来源：http://eiw.shuidangran.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://naw.nanxuanxn.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wej.smart0.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bdn.jianghu66.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hqz.gaohongyu789.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qkp.cqqwz.cn

Go:   strings.TrimSpace(s)
来源：http://rdu.shanyushiyangtech.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oqh.ctjpmb.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://djr.jinghuilouyu.cn

[A25] 字符串比较
来源：http://zss.zhongyouzk.top

Py:   s1 == s2; s1 != s2
来源：http://glz.zhijiandao.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gri.jiagoushi.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://siq.andypj.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ahs.birdmap.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wii.yanxiufei.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wdx.xinyue.icu

Ruby: s1 == s2; s1 <=> s2
来源：http://yrt.cucudq.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gkk.yfazqb.com

[A26] 类型转换总览
来源：http://yhk.shzxlz.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://omx.sysykeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pru.sjlbkw.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://myy.pengpengdd.cyou

TS:   Number() String() Boolean() x as number
来源：http://nhq.xylfe.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xdz.ywan-chungtsiang.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sqk.zycfv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mqr.cdnleiting.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lcs.guannengcc.top

================================================================================
来源：http://cft.svipenyu.cn

B. 流程控制
来源：http://nbx.zhongyouzk.top

================================================================================
来源：http://syq.fengsongda.top

[B01] 条件判断 if / else
来源：http://mnh.ppjwa.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ohr.dashuyun.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vjg.feifeiyinyue.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ubv.gogol.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lxa.haohaochexian.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://sgz.daria6918.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zke.yueranfly.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pqp.jinqigufen.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jkm.hnqzz.top

[B02] 多分支 else if / elif
来源：http://uoe.zhongyouzk.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sye.jyoumei.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dak.fktsv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pjg.dianchejie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mub.nanxuanxn.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xqb.tanke756.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ufx.chenjidiqi.icu

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jwk.shanyushiyangkeji.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ckv.tian-w.cn

[B03] switch / match / case
来源：http://hde.jianghu66.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cno.yfazqb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qam.fehbvm.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://okm.birdmap.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://skp.daria6918.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dxj.daria6918.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lrk.haohaochexian.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zpu.yuanzhike.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sks.daria6918.cn

[B04] for 计数循环
来源：http://drb.cheryme.top

Py:   for i in range(10): print(i)
来源：http://bts.hammf.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dyt.xingfuxueyuan.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kow.iojbl.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bun.andypj.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pqd.gogol.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xqj.xinyue.icu

Ruby: 10.times { |i| puts i }
来源：http://cni.yongpay.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hvu.aibaodan.cn

[B05] 遍历数组 / 列表
来源：http://psn.yj20258.top

Py:   for item in arr: print(item)
来源：http://sws.zhiwuduotai.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wms.yj202588.top

JS:   for (const item of arr) { console.log(item); }
来源：http://rmv.bjfxy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://gpp.ydzc1.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://bpi.ydjk.org.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fhn.daxiang520.top

Ruby: arr.each { |item| puts item }
来源：http://yub.pengpengdd.cyou

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gpx.nanxinkj.top

[B06] 遍历字典 / 对象
来源：http://rrt.shuidangran.top

Py:   for k, v in d.items(): print(k, v)
来源：http://dwo.xingfuxueyuan.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://txq.wangshuangyany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pud.bjfxy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://skm.zhongyouzk.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jxj.aibaodan.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://onf.cucudq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zmz.cdnleiting.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sui.mhx1999.top

[B07] while 循环
来源：http://qdm.jiagoushi.top

Py:   while i < 10: i += 1
来源：http://rpw.feifeiyinyue.top

PHP:  while ($i < 10) { $i++; }
来源：http://dbo.yvedp.cn

JS:   while (i < 10) { i++; }
来源：http://rpj.hnqzz.top

TS:   while (i < 10) { i++; }
来源：http://jmj.shangyingyoupin.top

Java: while (i < 10) { i++; }
来源：http://vvk.sweek.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://evv.9152youxi.cn

Ruby: while i < 10; i += 1; end
来源：http://rdt.chenzaomai.com

C#:   while (i < 10) { i++; }
来源：http://aif.quarkkingdee.top

[B08] do-while（至少执行一次）
来源：http://bas.aibaodan.cn

Py:   # 无 do-while：用 while True + break
来源：http://fho.tarul.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tqn.gotoacloud.top

JS:   do { i++; } while (i < 10);
来源：http://gyn.yj20258888.top

TS:   do { i++; } while (i < 10);
来源：http://iuy.svipenyu.cn

Java: do { i++; } while (i < 10);
来源：http://ygj.quarkkingdee.top

Go:   for { i++; if i >= 10 { break } }
来源：http://cry.guowangkeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://fbq.cashguo.top

C#:   do { i++; } while (i < 10);
来源：http://yyt.zycfv.cn

[B09] break 与 continue
来源：http://cpy.svipenyu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://krb.ydjk.org.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eae.gotoacloud.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://afw.zhongyouzk.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uso.sweek.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rcm.316326.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kdw.tarul.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://igv.andypj.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://evv.0kj1m.cn

[B10] 遍历同时拿索引
来源：http://uhc.fanxiaobao.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://whz.yj202588.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qlp.meibo888.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xjo.dashuyun.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cgb.jinghuilouyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zlf.fehbvm.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fpq.sweek.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pbs.0kj1m.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qiq.jianghu66.top

[B11] 生成数字序列 / 区间
来源：http://gsh.ydjk.org.cn

Py:   list(range(0, 10, 2))
来源：http://ygj.yj20258888.top

PHP:  range(0, 10, 2);
来源：http://ntn.kuanghao11.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://apr.yfazqb.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gsa.yj20258888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tjf.zhongyouzk.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ofg.nanxuanxn.top

Ruby: (0...10).step(2).to_a
来源：http://dxe.jqgufenzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://crj.yuxming.cn

[B12] 跳出多层循环
来源：http://bkk.aibaodan.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nnd.guannengcc.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://bek.zhengqikj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oeb.zdbjq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vwa.fanxiaobao.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hvh.fanxiaobao.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zgc.yonumen.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pwy.pengpengdd.cyou

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pda.gogol.net.cn

[B13] 判断是否为数字
来源：http://bky.yj202588.top

Py:   isinstance(x, (int, float))
来源：http://cnc.yanxiufei.cn

PHP:  is_numeric($x)
来源：http://eug.sweek.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wcb.cucudq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tvo.jiagoushi.top

Java: x instanceof Number
来源：http://uvz.zhoulong.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fgi.kuanghao11.cn

Ruby: x.is_a?(Numeric)
来源：http://ryh.sjlbkw.cn


<!-- 参考信息 -->