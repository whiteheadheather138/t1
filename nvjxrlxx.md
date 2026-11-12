代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hrj.zhaomingkeji.xyz

[A07] 数字转字符串
来源：http://yen.sysykeji.top

Py:   str(42)
来源：http://brs.tianlin.xyz

PHP:  (string) 42; strval(42)
来源：http://nvi.mhx1999.top

JS:   String(42); (42).toString()
来源：http://gyv.316326.xyz

TS:   String(42)
来源：http://goj.guannengcc.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://zuo.gotoacloud.top

Go:   strconv.Itoa(42)
来源：http://ovk.vehdjk.com

Ruby: 42.to_s
来源：http://enw.redwolf501.top

C#:   42.ToString()
来源：http://fyd.daxiang520.top

[A08] 取整与四舍五入
来源：http://onf.xingfuxueyuan.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kpt.jyoumei.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wvp.hammf.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hip.fehbvm.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wsf.c1oappe.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jng.shzxlz.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hrk.meibo888.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://vbk.aibaodan.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sxh.yanxiufei.cn

[A09] 绝对值与最大最小值
来源：http://nbx.yvedp.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pxo.hongshengwenyu.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jni.chenlongwang.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://axj.zhoulong.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ous.smart0.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tka.yfazqb.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://frh.bbcook.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lyx.jinghuilouyu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ttw.hcnkem.com

[A10] 生成随机数
来源：http://mlb.pengpengdd.cyou

Py:   import random; random.randint(1, 100)
来源：http://zfi.vehdjk.com

PHP:  random_int(1, 100);
来源：http://ftc.shuidangran.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hgp.zdqjudy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://quw.jiagoushi.top

Java: new Random().nextInt(100) + 1
来源：http://jxq.0kj1m.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://krv.jinyuanbaomall.cn

Ruby: rand(1..100)
来源：http://rus.yanxiufei.cn

C#:   new Random().Next(1, 101)
来源：http://qlo.jinqigufen.top

[A11] 条件表达式（三元）
来源：http://lqb.ydjk.org.cn

Py:   "yes" if x > 0 else "no"
来源：http://tfb.yueranfly.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://yqs.gogol.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://mwi.nanxuanxn.top

TS:   x > 0 ? "yes" : "no"
来源：http://fqy.fktsv.cn

Java: x > 0 ? "yes" : "no"
来源：http://ute.52xcode.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ury.dianchejie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://smv.shangyingyoupin.top

C#:   x > 0 ? "yes" : "no"
来源：http://pfd.sysykeji.top

[A12] 字符串插值 / 格式化
来源：http://eqv.chenzaomai.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ofu.zdqjudy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ggw.chenjidiqi.icu

JS:   `Hello, ${name}!`
来源：http://sma.jinghuilouyu.cn

TS:   `Hello, ${name}!`
来源：http://jzd.hongshengwenyu.top

Java: "Hello, %s!".formatted(name)
来源：http://rsf.xziqi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://egd.cdnleiting.top

Ruby: "Hello, #{name}!"
来源：http://hrb.smart0.xyz

C#:   $"Hello, {name}!"
来源：http://mci.shuidangran.top

[A13] 多行字符串（练习 \n 转义）
来源：http://gkr.ctjpmb.com

Py:   "第一行\n第二行"
来源：http://xcs.uphjek.com

PHP:  "第一行\n第二行"
来源：http://mao.tianlin.xyz

JS:   "第一行\n第二行"
来源：http://wgn.zhixingplan.top

TS:   "第一行\n第二行"
来源：http://dxq.zhixingplan.top

Java: "第一行\n第二行"
来源：http://abs.jlsjyb.cn

Go:   "第一行\n第二行"
来源：http://wxd.0kj1m.cn

Ruby: "第一行\n第二行"
来源：http://syw.wangdashe.top

C#:   "第一行\n第二行"
来源：http://ugn.tarul.cn

[A14] 注释写法
来源：http://cbj.cucudq.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yyf.fktsv.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jfb.feifeiyinyue.top

JS:   // 单行；/* 多行 */
来源：http://uvi.aibaodan.cn

TS:   // 单行；/* 多行 */
来源：http://noq.havefunace.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://woy.zhengqikj.top

Go:   // 单行；/* 多行 */
来源：http://ksr.ydjk.org.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rrm.jinyuanbaomall.cn

C#:   // 单行；/* 多行 */
来源：http://iil.yvedp.cn

[A15] 空值判断与默认值
来源：http://bqp.haohaochexian.top

Py:   value = data or "默认值"
来源：http://cgu.zhijiandao.cn

PHP:  $value = $data ?? "默认值";
来源：http://ptk.hammf.cn

JS:   const value = data ?? "默认值";
来源：http://zwy.tarul.cn

TS:   const value = data ?? "默认值";
来源：http://rvj.yongpay.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ibj.xingfuxueyuan.xyz

Go:   if data == "" { data = "默认值" }
来源：http://zgk.nanxinkj.top

Ruby: value = data || "默认值"
来源：http://yxr.meibo888.top

C#:   var value = data ?? "默认值";
来源：http://hsh.jyoumei.cn

[A16] 真假值判断规则
来源：http://uvo.xylfe.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://uui.ybcxt.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://esr.0kj1m.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zlr.chenjidiqi.icu

TS:   if (!x) {}
来源：http://cbo.fengsongda.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wyj.fanxiaobao.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://irt.cheryme.top

Ruby: unless x            # nil 与 false 为假
来源：http://xnw.ehwqpu.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qkm.xziqi.cn

[A17] 位运算
来源：http://xpk.xuanzx.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dnf.yueranfly.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mij.fanxiaobao.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kga.yj202588.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://out.hcnkem.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uvk.vehdjk.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tsg.tianlin.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fis.svipenyu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qiu.shanyushiyangkeji.top

[A18] 字符与 ASCII 码互转
来源：http://ldj.redwolf501.top

Py:   ord("A"); chr(65)
来源：http://gao.pycfn.com

PHP:  ord("A"); chr(65)
来源：http://amu.yonumen.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dyd.nanxinkj.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fxm.hnqzz.top

Java: (int) 'A'; (char) 65
来源：http://eit.zdqjudy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lpy.chenlongwang.top

Ruby: "A".ord; 65.chr
来源：http://ddx.sysykeji.top

C#:   (int)'A'; (char)65
来源：http://yhq.bjfxy.top

[A19] 交换两个变量
来源：http://aec.zhixingplan.top

Py:   a, b = b, a
来源：http://pty.jinghuilouyu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://chw.andypj.xyz

JS:   [a, b] = [b, a];
来源：http://qxy.ydzc1.top

TS:   [a, b] = [b, a];
来源：http://bbp.hcnkem.com

Java: int t = a; a = b; b = t;
来源：http://opn.fzhhl.top

Go:   a, b = b, a
来源：http://zns.hnqzz.top

Ruby: a, b = b, a
来源：http://ksv.xuetiantiany.cn

C#:   (a, b) = (b, a);
来源：http://ags.tanke756.top

[A20] 读取标准输入
来源：http://eqp.9152youxi.cn

Py:   name = input("请输入：")
来源：http://zeu.fktsv.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gkk.yangfankeji.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tqp.chenlongwang.top

TS:   // Node.js：readline 模块
来源：http://ejs.ivvv.top

Java: new Scanner(System.in).nextLine()
来源：http://wjf.9152youxi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vdr.yj202588.top

Ruby: gets.chomp
来源：http://dbc.c1oappe.top

C#:   Console.ReadLine();
来源：http://mnd.zhongyouzk.top

[A21] 保留指定小数位输出
来源：http://dgw.gzhubu.top

Py:   f"{3.14159:.2f}"
来源：http://hlb.shuidangran.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://epb.ppjwa.cn

JS:   (3.14159).toFixed(2)
来源：http://vsd.epnwcf.com

TS:   (3.14159).toFixed(2)
来源：http://poc.cashguo.top

Java: String.format("%.2f", 3.14159)
来源：http://keo.jianghu66.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tio.dianchejie.cn

Ruby: format("%.2f", 3.14159)
来源：http://mnf.pycfn.com

C#:   3.14159.ToString("F2")
来源：http://zho.guannengcc.top

[A22] 获取字符串长度
来源：http://eic.hfpthk.cn

Py:   len(s)
来源：http://fxx.jyoumei.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jji.shanyushiyangkeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yxx.sufxvd.cn

TS:   s.length
来源：http://cem.cqqwz.cn

Java: s.length()
来源：http://hmf.guowangkeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yie.hywenlv.cn

Ruby: s.length
来源：http://thy.chenzaomai.com

C#:   s.Length
来源：http://ssy.zhengqikj.top

[A23] 大小写转换
来源：http://yxa.yueranfly.top

Py:   s.upper(); s.lower(); s.title()
来源：http://zzu.snrcjt.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://huu.gzhubu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vlw.smart0.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rfc.hnxiangtu.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://loa.hnxiangtu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://iue.wangdashe.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kbv.zdbjq.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fsi.ydjk.org.cn

[A24] 去除首尾空白
来源：http://mpx.zhongyouzk.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hlx.sweek.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://eyk.wangshuangyany.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://emq.pycfn.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cva.xingfuxueyuan.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ylv.birdmap.top

Go:   strings.TrimSpace(s)
来源：http://bpc.svipenyu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xcm.hammf.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zld.zdqjudy.top

[A25] 字符串比较
来源：http://vhs.sysykeji.top

Py:   s1 == s2; s1 != s2
来源：http://gue.guannengcc.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ugu.yueranfly.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ptg.tanke756.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xib.c1oappe.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jei.mhx1999.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lry.yangfankeji.com

Ruby: s1 == s2; s1 <=> s2
来源：http://alb.yuanzhike.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ypt.vehdjk.com

[A26] 类型转换总览
来源：http://nka.shzxlz.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kgr.shzxlz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://arw.jinyuanbaomall.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://stb.jqgfzy.top

TS:   Number() String() Boolean() x as number
来源：http://hby.cheryme.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dsc.tanke756.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qed.jiagoushi.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://xrv.daria6918.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://emh.sjlbkw.cn

================================================================================
来源：http://tfb.tianlin.xyz

B. 流程控制
来源：http://xdg.birdmap.top

================================================================================
来源：http://idj.ydzc1.top

[B01] 条件判断 if / else
来源：http://jxm.snrcjt.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qoq.cdnleiting.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://prg.gzhubu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://azc.jinghuilouyu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mkv.dianchejie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fqa.hnqzz.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uyz.hnqzz.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pqv.xinyue.icu

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pmy.uphjek.com

[B02] 多分支 else if / elif
来源：http://iho.cheryme.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ndu.ydjk.org.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ucd.sjlbkw.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tue.zhengqikj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fhg.zycfv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nbn.daria6918.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vxa.ppjwa.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://crh.jyoumei.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cbz.zhijiandao.cn

[B03] switch / match / case
来源：http://uyh.ydzc1.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cyl.ybcxt.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ypu.c1oappe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ryi.dashuyun.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bjf.yuxming.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vha.tarul.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://azx.tianlin.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ahf.tian-w.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bza.c1oappe.top

[B04] for 计数循环
来源：http://pte.chenlongwang.top

Py:   for i in range(10): print(i)
来源：http://dzw.haohaochexian.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://eus.andypj.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ure.shanyushiyangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://krk.jianghu66.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://llk.tianlin.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pov.yuanzhike.top

Ruby: 10.times { |i| puts i }
来源：http://chw.pengpengdd.cyou

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wcy.daxiang520.top

[B05] 遍历数组 / 列表
来源：http://vuu.haohaochexian.top

Py:   for item in arr: print(item)
来源：http://ngd.pycfn.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qdz.birdmap.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ogv.gzhubu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://zdx.andypj.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://ktx.9152youxi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cpv.jianghu66.top

Ruby: arr.each { |item| puts item }
来源：http://bwf.fengsongda.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bke.svipenyu.cn

[B06] 遍历字典 / 对象
来源：http://ztd.yongpay.top

Py:   for k, v in d.items(): print(k, v)
来源：http://nou.yongpay.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pys.hnqzz.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ffz.ydjk.org.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lvt.tian-w.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lwu.ydzc1.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://env.shuidangran.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kfi.quarkkingdee.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qpw.chenzaomai.com

[B07] while 循环
来源：http://toe.kuanghao11.cn

Py:   while i < 10: i += 1
来源：http://hkm.sweek.top

PHP:  while ($i < 10) { $i++; }
来源：http://pbs.hcnkem.com

JS:   while (i < 10) { i++; }
来源：http://tci.hnqzz.top

TS:   while (i < 10) { i++; }
来源：http://kir.ctjpmb.com

Java: while (i < 10) { i++; }
来源：http://ogr.cdnleiting.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bwb.xinyue.icu

Ruby: while i < 10; i += 1; end
来源：http://mom.cheryme.top

C#:   while (i < 10) { i++; }
来源：http://nke.sysykeji.top

[B08] do-while（至少执行一次）
来源：http://dsw.jlsjyb.cn

Py:   # 无 do-while：用 while True + break
来源：http://clm.nanxinkj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ver.kuanghao11.cn

JS:   do { i++; } while (i < 10);
来源：http://kdy.cdnleiting.top

TS:   do { i++; } while (i < 10);
来源：http://hmt.9152youxi.cn

Java: do { i++; } while (i < 10);
来源：http://gmb.pengpengdd.cyou

Go:   for { i++; if i >= 10 { break } }
来源：http://egy.zdqjudy.top

Ruby: begin; i += 1; end while i < 10
来源：http://xkt.hongshengwenyu.top

C#:   do { i++; } while (i < 10);
来源：http://bry.c1oappe.top

[B09] break 与 continue
来源：http://abo.wangdashe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ush.yuxming.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fau.yj20258888.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://quj.chenzaomai.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dyr.shanyushiyangtech.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://krv.xuetiantiany.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rwt.haohaochexian.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dbq.sweek.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vdo.zdqjudy.top

[B10] 遍历同时拿索引
来源：http://vrb.52xcode.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vvx.tianlin.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ckm.xingfuxueyuan.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kme.sufxvd.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xnf.shanyushiyangkeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pvc.zhengqikj.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://aaq.vqdsnc.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gyi.wangshuangyany.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jtu.vqdsnc.cn

[B11] 生成数字序列 / 区间
来源：http://rse.hysaishi.cn

Py:   list(range(0, 10, 2))
来源：http://eoh.fktsv.cn

PHP:  range(0, 10, 2);
来源：http://ysn.zhixingplan.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dkx.cqqwz.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tlw.iojbl.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qur.sufxvd.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bpu.smart0.xyz

Ruby: (0...10).step(2).to_a
来源：http://wmi.jqgufenzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kiv.sweek.top

[B12] 跳出多层循环
来源：http://hbb.hysaishi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://doa.gzhubu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://qfu.52xcode.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xnr.gogol.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kvu.jlsjyb.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gcy.shzxlz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cot.yfazqb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ati.xuanzx.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dzi.yueranfly.top

[B13] 判断是否为数字
来源：http://icj.bjfxy.top

Py:   isinstance(x, (int, float))
来源：http://nam.daxiang520.top

PHP:  is_numeric($x)
来源：http://wol.tanke756.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tpn.0kj1m.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tzt.jqgfzy.top

Java: x instanceof Number
来源：http://wgk.tanke756.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rre.fktsv.cn

Ruby: x.is_a?(Numeric)
来源：http://oek.jinyuanbaomall.cn


<!-- 参考信息 -->