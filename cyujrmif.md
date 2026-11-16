代发 wailian999

Ruby: 42.to_s
来源：http://lnn.yuxming.cn

C#:   42.ToString()
来源：http://kbi.gogol.net.cn

[A08] 取整与四舍五入
来源：http://mvr.jinqigufen.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pwk.xziqi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xfc.sweek.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://avf.fengsongda.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nym.kuanghao11.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hys.hongshengwenyu.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mlb.shangyingyoupin.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://zif.daxiang520.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gha.redwolf501.top

[A09] 绝对值与最大最小值
来源：http://lgw.yonumen.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bzs.jinqigfzy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wdj.xziqi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pzd.hnxiangtu.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wrk.aizwys.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vjb.guannengcc.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tzc.zhengqikj.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dgo.zhijiandao.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mfg.jiagoushi.top

[A10] 生成随机数
来源：http://wgw.jqgufenzy.top

Py:   import random; random.randint(1, 100)
来源：http://yjb.vehdjk.com

PHP:  random_int(1, 100);
来源：http://ozh.hcnkem.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ltr.aizwys.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rzb.svipenyu.cn

Java: new Random().nextInt(100) + 1
来源：http://zew.xingfuxueyuan.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ugs.xuetiantiany.cn

Ruby: rand(1..100)
来源：http://yjz.guannengcc.top

C#:   new Random().Next(1, 101)
来源：http://mts.bjfxy.top

[A11] 条件表达式（三元）
来源：http://xfa.xinyue.icu

Py:   "yes" if x > 0 else "no"
来源：http://wlk.daxiang520.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://yzs.xingfuxueyuan.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://mck.cheryme.top

TS:   x > 0 ? "yes" : "no"
来源：http://mbn.havefunace.top

Java: x > 0 ? "yes" : "no"
来源：http://dsl.yanxiufei.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://yyk.jlsjyb.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tpk.nwbrower.top

C#:   x > 0 ? "yes" : "no"
来源：http://ikk.cucudq.cn

[A12] 字符串插值 / 格式化
来源：http://zzp.nanxinkj.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://htm.chenzaomai.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://huf.birdmap.top

JS:   `Hello, ${name}!`
来源：http://krc.vqdsnc.cn

TS:   `Hello, ${name}!`
来源：http://sri.hongshengwenyu.top

Java: "Hello, %s!".formatted(name)
来源：http://qlp.hnqzz.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zwy.vqdsnc.cn

Ruby: "Hello, #{name}!"
来源：http://rvy.uphjek.com

C#:   $"Hello, {name}!"
来源：http://iue.zdqjudy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://tez.nanxinkj.top

Py:   "第一行\n第二行"
来源：http://zwb.sysykeji.top

PHP:  "第一行\n第二行"
来源：http://ndj.zycfv.cn

JS:   "第一行\n第二行"
来源：http://qtg.cucudq.cn

TS:   "第一行\n第二行"
来源：http://tsb.aibaodan.cn

Java: "第一行\n第二行"
来源：http://hrx.ywan-chungtsiang.top

Go:   "第一行\n第二行"
来源：http://nuf.tian-w.cn

Ruby: "第一行\n第二行"
来源：http://jak.guowangkeji.top

C#:   "第一行\n第二行"
来源：http://xnt.sysykeji.top

[A14] 注释写法
来源：http://dby.shanyushiyangtech.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://eat.daria6918.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xhc.yanxiufei.cn

JS:   // 单行；/* 多行 */
来源：http://gfk.wangshuangyany.cn

TS:   // 单行；/* 多行 */
来源：http://jgo.aizwys.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://doo.gzhubu.top

Go:   // 单行；/* 多行 */
来源：http://vse.nanxuanxn.top

Ruby: # 单行；=begin 多行 =end
来源：http://jxn.xuetiantiany.cn

C#:   // 单行；/* 多行 */
来源：http://dnu.hnqzz.top

[A15] 空值判断与默认值
来源：http://ipk.hesvh.cn

Py:   value = data or "默认值"
来源：http://isc.zycfv.cn

PHP:  $value = $data ?? "默认值";
来源：http://nux.shuidangran.top

JS:   const value = data ?? "默认值";
来源：http://gdl.uphjek.com

TS:   const value = data ?? "默认值";
来源：http://xep.wangshuangyany.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ynt.jinghuilouyu.cn

Go:   if data == "" { data = "默认值" }
来源：http://nqt.xylfe.cn

Ruby: value = data || "默认值"
来源：http://ifv.hongshengwenyu.top

C#:   var value = data ?? "默认值";
来源：http://yac.aibaodan.cn

[A16] 真假值判断规则
来源：http://zju.daxiang520.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cau.xinyue.icu

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ukj.316326.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sxl.chenjidiqi.icu

TS:   if (!x) {}
来源：http://fwh.sufxvd.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nkg.hammf.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zzr.epnwcf.com

Ruby: unless x            # nil 与 false 为假
来源：http://iol.yongpay.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cvv.guannengcc.top

[A17] 位运算
来源：http://hun.nwbrower.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ogg.jqgufenzy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jmx.epnwcf.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ani.daria6918.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dqb.yangfankeji.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gil.feifeiyinyue.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bck.jinyuanbaomall.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vnm.tanke756.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://woi.0kj1m.cn

[A18] 字符与 ASCII 码互转
来源：http://rji.meibo888.top

Py:   ord("A"); chr(65)
来源：http://ray.guannengcc.top

PHP:  ord("A"); chr(65)
来源：http://eup.316326.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bzy.hongshengwenyu.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lhz.jinghuilouyu.cn

Java: (int) 'A'; (char) 65
来源：http://dwa.hysaishi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ped.yj202588.top

Ruby: "A".ord; 65.chr
来源：http://rxy.zycfv.cn

C#:   (int)'A'; (char)65
来源：http://kmn.hongshengwenyu.top

[A19] 交换两个变量
来源：http://mkv.yvedp.cn

Py:   a, b = b, a
来源：http://dim.birdmap.top

PHP:  [$a, $b] = [$b, $a];
来源：http://unt.zhaomingkeji.xyz

JS:   [a, b] = [b, a];
来源：http://tzl.andypj.xyz

TS:   [a, b] = [b, a];
来源：http://oay.snrcjt.cn

Java: int t = a; a = b; b = t;
来源：http://juu.ywan-chungtsiang.top

Go:   a, b = b, a
来源：http://hdu.shanyushiyangkeji.top

Ruby: a, b = b, a
来源：http://ntf.jiagoushi.top

C#:   (a, b) = (b, a);
来源：http://huk.yangfankeji.com

[A20] 读取标准输入
来源：http://lof.zdbjq.cn

Py:   name = input("请输入：")
来源：http://zgc.jinyuanbaomall.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://krr.chenzaomai.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gtf.cucudq.cn

TS:   // Node.js：readline 模块
来源：http://abr.yuanzhike.top

Java: new Scanner(System.in).nextLine()
来源：http://cyy.birdmap.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tdc.chenlongwang.top

Ruby: gets.chomp
来源：http://fgw.ctjpmb.com

C#:   Console.ReadLine();
来源：http://geo.ctjpmb.com

[A21] 保留指定小数位输出
来源：http://vdt.jlsjyb.cn

Py:   f"{3.14159:.2f}"
来源：http://dgs.pycfn.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xxh.sufxvd.cn

JS:   (3.14159).toFixed(2)
来源：http://lxm.fktsv.cn

TS:   (3.14159).toFixed(2)
来源：http://tso.mhx1999.top

Java: String.format("%.2f", 3.14159)
来源：http://mvc.jinqigfzy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qrm.mhx1999.top

Ruby: format("%.2f", 3.14159)
来源：http://dxi.yj20258.top

C#:   3.14159.ToString("F2")
来源：http://nml.daxiang520.top

[A22] 获取字符串长度
来源：http://sty.hesvh.cn

Py:   len(s)
来源：http://qrn.tianlin.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://win.guannengcc.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://oys.zhijiandao.cn

TS:   s.length
来源：http://dnt.quarkkingdee.top

Java: s.length()
来源：http://nyn.shzxlz.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yyx.52xcode.cn

Ruby: s.length
来源：http://cfh.jinqigufen.top

C#:   s.Length
来源：http://caw.iojbl.cn

[A23] 大小写转换
来源：http://uqd.kuanghao11.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yae.hammf.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://arh.wangdashe.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vnh.yfazqb.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://efm.tarul.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qxw.jqgfzy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nty.yueranfly.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tex.ybcxt.top

C#:   s.ToUpper(); s.ToLower()
来源：http://goz.gaohongyu789.top

[A24] 去除首尾空白
来源：http://htz.meibo888.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://txx.hnqzz.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fxj.gotoacloud.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ljt.jinqigufen.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mxx.xylfe.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wbv.hcnkem.com

Go:   strings.TrimSpace(s)
来源：http://tjt.ppjwa.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://aau.52xcode.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ord.fzhhl.top

[A25] 字符串比较
来源：http://elj.haohaochexian.top

Py:   s1 == s2; s1 != s2
来源：http://whb.0kj1m.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gwf.tarul.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://myq.gzhubu.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://twk.jinqigufen.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ffh.mhx1999.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ctc.daria6918.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://uvd.hnqzz.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bdt.bbcook.cn

[A26] 类型转换总览
来源：http://nbp.cdnleiting.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bsd.hongshengwenyu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sku.nanxinkj.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tlh.shzxlz.cn

TS:   Number() String() Boolean() x as number
来源：http://ysb.jqgufenzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ncq.tarul.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://eae.hnxiangtu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://vsx.xziqi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bvd.gogol.net.cn

================================================================================
来源：http://hel.9152youxi.cn

B. 流程控制
来源：http://zcr.tian-w.cn

================================================================================
来源：http://qvu.sufxvd.cn

[B01] 条件判断 if / else
来源：http://qzx.yj20258888.top

Py:   result = "正" if x > 0 else "非正"
来源：http://lmg.smart0.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vzl.yuxming.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jmz.guowangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bpq.gzhubu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://hyr.havefunace.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://aes.uphjek.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lwx.tarul.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fri.shanyushiyangkeji.top

[B02] 多分支 else if / elif
来源：http://dqc.yuanzhike.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://klt.hcnkem.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hqv.zycfv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jdg.mhx1999.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fcj.tianlin.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ruo.dashuyun.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://czz.c1oappe.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qzs.gaohongyu789.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lmu.yangfankeji.com

[B03] switch / match / case
来源：http://zml.hesvh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://luq.meibo888.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wkq.fanxiaobao.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uxp.aibaodan.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://odp.zhijiandao.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ier.guowangkeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mcf.bbcook.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oib.hysaishi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yif.jinyuanbaomall.cn

[B04] for 计数循环
来源：http://ung.zhiwuduotai.top

Py:   for i in range(10): print(i)
来源：http://eot.yonumen.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ngn.hesvh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vhz.hongshengwenyu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://alk.shangyingyoupin.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aqr.ydjk.org.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rys.yonumen.top

Ruby: 10.times { |i| puts i }
来源：http://lyn.ydzc1.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kda.cheryme.top

[B05] 遍历数组 / 列表
来源：http://yrn.c1oappe.top

Py:   for item in arr: print(item)
来源：http://kqn.hammf.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vsc.shangyingyoupin.top

JS:   for (const item of arr) { console.log(item); }
来源：http://aoa.quarkkingdee.top

TS:   for (const item of arr) { console.log(item); }
来源：http://rmk.ydzc1.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://she.shanyushiyangtech.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ijv.zhiwuduotai.top

Ruby: arr.each { |item| puts item }
来源：http://prd.0kj1m.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ejw.zhijiandao.cn

[B06] 遍历字典 / 对象
来源：http://ici.zhoulong.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://neq.havefunace.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nfk.xuetiantiany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vmr.zhiwuduotai.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mcp.vehdjk.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uks.meibo888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oax.aizwys.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hlx.fengsongda.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rgu.iojbl.cn

[B07] while 循环
来源：http://qnn.shangyingyoupin.top

Py:   while i < 10: i += 1
来源：http://dft.zhaomingkeji.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://gqp.tianlin.xyz

JS:   while (i < 10) { i++; }
来源：http://knd.nwbrower.top

TS:   while (i < 10) { i++; }
来源：http://zxb.yanxiufei.cn

Java: while (i < 10) { i++; }
来源：http://hfk.fengsongda.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dds.xingfuxueyuan.xyz

Ruby: while i < 10; i += 1; end
来源：http://fvl.ppjwa.cn

C#:   while (i < 10) { i++; }
来源：http://wts.zdqjudy.top

[B08] do-while（至少执行一次）
来源：http://ube.nanxuanxn.top

Py:   # 无 do-while：用 while True + break
来源：http://jsg.zhengqikj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kok.gogol.net.cn

JS:   do { i++; } while (i < 10);
来源：http://pkd.zhongyouzk.top

TS:   do { i++; } while (i < 10);
来源：http://psp.uphjek.com

Java: do { i++; } while (i < 10);
来源：http://rqq.bbcook.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bbc.zhaomingkeji.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://efn.jqgufenzy.top

C#:   do { i++; } while (i < 10);
来源：http://dhz.snrcjt.cn

[B09] break 与 continue
来源：http://evp.hysaishi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://brr.shanyushiyangtech.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yru.vqdsnc.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rur.yonumen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ypf.zhixingplan.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tna.fehbvm.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ifl.zhixingplan.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zhs.jlsjyb.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pun.ivvv.top

[B10] 遍历同时拿索引
来源：http://idj.9152youxi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nzy.bbcook.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ink.dianchejie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://twb.shuidangran.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pvt.aizwys.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://avu.zhoulong.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://moi.shzxlz.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pne.jinyuanbaomall.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nln.c1oappe.top

[B11] 生成数字序列 / 区间
来源：http://rbg.zdqjudy.top

Py:   list(range(0, 10, 2))
来源：http://nfw.jiagoushi.top

PHP:  range(0, 10, 2);
来源：http://krc.ybcxt.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xxn.tian-w.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cjy.shzxlz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pin.pycfn.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wsj.shanyushiyangtech.top

Ruby: (0...10).step(2).to_a
来源：http://qbh.cdnleiting.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vqu.ywan-chungtsiang.top

[B12] 跳出多层循环
来源：http://gzw.aizwys.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ekv.meibo888.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ykm.xingfuxueyuan.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mnt.epnwcf.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qye.gaohongyu789.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ipy.jianghu66.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dxt.feifeiyinyue.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wls.fktsv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wen.fktsv.cn

[B13] 判断是否为数字
来源：http://rke.daxiang520.top

Py:   isinstance(x, (int, float))
来源：http://spj.hongshengwenyu.top

PHP:  is_numeric($x)
来源：http://iwe.vqdsnc.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pvx.ybcxt.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qxz.nanxuanxn.top

Java: x instanceof Number
来源：http://aoc.c1oappe.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://anf.xingfuxueyuan.xyz

Ruby: x.is_a?(Numeric)
来源：http://qds.snrcjt.cn

C#:   x is int or double or decimal
来源：http://ggn.uphjek.com

[B14] 判断值是否在集合内
来源：http://bvr.zhoulong.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pvz.fzhhl.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://egk.jianghu66.top

JS:   [1, 2, 3].includes(x)
来源：http://bei.tian-w.cn

TS:   [1, 2, 3].includes(x)
来源：http://hwx.cqqwz.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cud.gzhubu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mry.xuetiantiany.cn


<!-- 参考信息 -->