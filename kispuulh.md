代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://inz.zhijiandao.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jtr.havefunace.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://scw.sweek.top

Ruby: "42".to_i; "3.14".to_f
来源：http://hbb.shzxlz.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fao.xuetiantiany.cn

[A07] 数字转字符串
来源：http://kpp.birdmap.top

Py:   str(42)
来源：http://syc.hysaishi.cn

PHP:  (string) 42; strval(42)
来源：http://mia.chenjidiqi.icu

JS:   String(42); (42).toString()
来源：http://uwp.hongshengwenyu.top

TS:   String(42)
来源：http://btq.sxryk.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ukd.yj202588.top

Go:   strconv.Itoa(42)
来源：http://iyg.zhaomingkeji.xyz

Ruby: 42.to_s
来源：http://xex.jinghuilouyu.cn

C#:   42.ToString()
来源：http://ctv.sufxvd.cn

[A08] 取整与四舍五入
来源：http://emo.cheryme.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://glb.hammf.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bwk.yueranfly.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://uit.bbcook.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://iis.cashguo.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xed.shanyushiyangkeji.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://axn.ivvv.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://lkx.jinqigfzy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dfc.pengpengdd.cyou

[A09] 绝对值与最大最小值
来源：http://lnf.jiagoushi.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://udl.52xcode.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ixj.tarul.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dbm.jinyuanbaomall.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vab.9152youxi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pyx.redwolf501.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vmu.zhaomingkeji.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tza.redwolf501.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zrn.guannengcc.top

[A10] 生成随机数
来源：http://ajn.birdmap.top

Py:   import random; random.randint(1, 100)
来源：http://yci.cheryme.top

PHP:  random_int(1, 100);
来源：http://bpv.ctjpmb.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zkx.ehwqpu.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ahv.sysykeji.top

Java: new Random().nextInt(100) + 1
来源：http://zhy.52xcode.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qdu.jinqigfzy.top

Ruby: rand(1..100)
来源：http://zhx.snrcjt.cn

C#:   new Random().Next(1, 101)
来源：http://maf.redwolf501.top

[A11] 条件表达式（三元）
来源：http://qby.ydjk.org.cn

Py:   "yes" if x > 0 else "no"
来源：http://tho.wangshuangyany.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://oub.cashguo.top

JS:   x > 0 ? "yes" : "no"
来源：http://kky.svipenyu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lxx.havefunace.top

Java: x > 0 ? "yes" : "no"
来源：http://ggt.feifeiyinyue.top

Go:   // 无三元运算符，需用 if 语句
来源：http://cxf.hammf.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hep.ctjpmb.com

C#:   x > 0 ? "yes" : "no"
来源：http://akh.wangshuangyany.cn

[A12] 字符串插值 / 格式化
来源：http://kga.xuanzx.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cyu.fzhhl.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yqu.wangshuangyany.cn

JS:   `Hello, ${name}!`
来源：http://enh.aibaodan.cn

TS:   `Hello, ${name}!`
来源：http://fih.jlsjyb.cn

Java: "Hello, %s!".formatted(name)
来源：http://scv.yfazqb.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wqg.daxiang520.top

Ruby: "Hello, #{name}!"
来源：http://ofo.iojbl.cn

C#:   $"Hello, {name}!"
来源：http://bnu.fktsv.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://nbw.yueranfly.top

Py:   "第一行\n第二行"
来源：http://dil.jinqigufen.top

PHP:  "第一行\n第二行"
来源：http://amc.yvedp.cn

JS:   "第一行\n第二行"
来源：http://agc.yj20258888.top

TS:   "第一行\n第二行"
来源：http://tfa.hywenlv.cn

Java: "第一行\n第二行"
来源：http://fmg.zhongyouzk.top

Go:   "第一行\n第二行"
来源：http://urw.yueranfly.top

Ruby: "第一行\n第二行"
来源：http://lnz.yfazqb.com

C#:   "第一行\n第二行"
来源：http://cme.aizwys.cn

[A14] 注释写法
来源：http://jya.havefunace.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://znb.tarul.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jdp.birdmap.top

JS:   // 单行；/* 多行 */
来源：http://zju.kuanghao11.cn

TS:   // 单行；/* 多行 */
来源：http://yko.hnqzz.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://snl.vehdjk.com

Go:   // 单行；/* 多行 */
来源：http://zdk.mhx1999.top

Ruby: # 单行；=begin 多行 =end
来源：http://veu.yj202588.top

C#:   // 单行；/* 多行 */
来源：http://rng.meibo888.top

[A15] 空值判断与默认值
来源：http://yhm.ydzc1.top

Py:   value = data or "默认值"
来源：http://jgh.sxryk.cn

PHP:  $value = $data ?? "默认值";
来源：http://fne.ppjwa.cn

JS:   const value = data ?? "默认值";
来源：http://kqr.9152youxi.cn

TS:   const value = data ?? "默认值";
来源：http://hyx.andypj.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zvg.quarkkingdee.top

Go:   if data == "" { data = "默认值" }
来源：http://gjc.zhiwuduotai.top

Ruby: value = data || "默认值"
来源：http://wyd.gogol.net.cn

C#:   var value = data ?? "默认值";
来源：http://xqn.zdbjq.cn

[A16] 真假值判断规则
来源：http://ojs.snrcjt.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ktb.52xcode.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://osx.chenlongwang.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sva.chenlongwang.top

TS:   if (!x) {}
来源：http://oik.fengsongda.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rgd.jinqigufen.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uzw.yueranfly.top

Ruby: unless x            # nil 与 false 为假
来源：http://lqy.xylfe.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qih.jianghu66.top

[A17] 位运算
来源：http://nyj.tian-w.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pfs.kuanghao11.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dbf.tanke756.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://duo.mhx1999.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pcg.hnxiangtu.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bbe.hywenlv.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cnr.cashguo.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qrt.shangyingyoupin.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hds.gogol.net.cn

[A18] 字符与 ASCII 码互转
来源：http://fxj.ctjpmb.com

Py:   ord("A"); chr(65)
来源：http://rta.gaohongyu789.top

PHP:  ord("A"); chr(65)
来源：http://tbz.jinqigufen.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kds.yj20258.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ejf.cdnleiting.top

Java: (int) 'A'; (char) 65
来源：http://nto.shuidangran.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://czo.zhaomingkeji.xyz

Ruby: "A".ord; 65.chr
来源：http://kub.tanke756.top

C#:   (int)'A'; (char)65
来源：http://bds.ctjpmb.com

[A19] 交换两个变量
来源：http://jhq.uphjek.com

Py:   a, b = b, a
来源：http://zew.guannengcc.top

PHP:  [$a, $b] = [$b, $a];
来源：http://mzu.gotoacloud.top

JS:   [a, b] = [b, a];
来源：http://vek.haohaochexian.top

TS:   [a, b] = [b, a];
来源：http://ogi.pycfn.com

Java: int t = a; a = b; b = t;
来源：http://sra.yvedp.cn

Go:   a, b = b, a
来源：http://yle.haohaochexian.top

Ruby: a, b = b, a
来源：http://bnq.yj20258888.top

C#:   (a, b) = (b, a);
来源：http://fvb.jinqigufen.top

[A20] 读取标准输入
来源：http://uow.shanyushiyangtech.top

Py:   name = input("请输入：")
来源：http://cop.pycfn.com

PHP:  $name = trim(fgets(STDIN));
来源：http://ogq.guannengcc.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jdx.yvedp.cn

TS:   // Node.js：readline 模块
来源：http://xvw.svipenyu.cn

Java: new Scanner(System.in).nextLine()
来源：http://crn.yuxming.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xvr.zdbjq.cn

Ruby: gets.chomp
来源：http://ieu.0kj1m.cn

C#:   Console.ReadLine();
来源：http://flk.jiagoushi.top

[A21] 保留指定小数位输出
来源：http://rzd.yongpay.top

Py:   f"{3.14159:.2f}"
来源：http://yhh.52xcode.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://iyr.tianlin.xyz

JS:   (3.14159).toFixed(2)
来源：http://qel.dianchejie.cn

TS:   (3.14159).toFixed(2)
来源：http://pbs.daria6918.cn

Java: String.format("%.2f", 3.14159)
来源：http://arq.chenjidiqi.icu

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pzw.hfpthk.cn

Ruby: format("%.2f", 3.14159)
来源：http://txd.cdnleiting.top

C#:   3.14159.ToString("F2")
来源：http://bbf.gzhubu.top

[A22] 获取字符串长度
来源：http://sgr.guannengcc.top

Py:   len(s)
来源：http://tkj.svipenyu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yan.guannengcc.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xmj.smart0.xyz

TS:   s.length
来源：http://ovl.quarkkingdee.top

Java: s.length()
来源：http://qfc.xinyue.icu

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hja.jiagoushi.top

Ruby: s.length
来源：http://uip.iojbl.cn

C#:   s.Length
来源：http://kbg.xuanzx.com

[A23] 大小写转换
来源：http://ixb.jinqigfzy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://xzo.pycfn.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jyx.316326.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://izn.vqdsnc.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vsc.fzhhl.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://uhi.vehdjk.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yoi.sufxvd.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ree.smart0.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://sqy.chenjidiqi.icu

[A24] 去除首尾空白
来源：http://bas.cucudq.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ryp.cqqwz.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sli.pengpengdd.cyou

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jqc.yfazqb.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yhr.zhaomingkeji.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tay.cqqwz.cn

Go:   strings.TrimSpace(s)
来源：http://fly.mhx1999.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://txm.gogol.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lxx.daria6918.cn

[A25] 字符串比较
来源：http://vlc.guowangkeji.top

Py:   s1 == s2; s1 != s2
来源：http://aqw.fzhhl.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xmg.uphjek.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://usz.dianchejie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://svt.xylfe.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://exq.dianchejie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://okr.cqqwz.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://czf.sjlbkw.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xry.ivvv.top

[A26] 类型转换总览
来源：http://opk.fzhhl.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sre.ctjpmb.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fup.zhengqikj.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dgk.yangfankeji.com

TS:   Number() String() Boolean() x as number
来源：http://vsq.daria6918.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ojk.hywenlv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ocj.cheryme.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ddx.andypj.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ihk.andypj.xyz

================================================================================
来源：http://apa.zhiwuduotai.top

B. 流程控制
来源：http://eaa.hnqzz.top

================================================================================
来源：http://khb.cucudq.cn

[B01] 条件判断 if / else
来源：http://lcr.xingfuxueyuan.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://qnb.smart0.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://amk.xylfe.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qfu.shanyushiyangtech.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://waz.zhoulong.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://mxc.dianchejie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tqz.smart0.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sna.cashguo.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ckz.xylfe.cn

[B02] 多分支 else if / elif
来源：http://jbi.dashuyun.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tcf.andypj.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://szv.xingfuxueyuan.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yje.hysaishi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ljw.ctjpmb.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ovn.jqgufenzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vzw.birdmap.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://knm.guowangkeji.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yei.andypj.xyz

[B03] switch / match / case
来源：http://mjr.haohaochexian.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zaj.chenlongwang.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dya.fanxiaobao.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://byr.fzhhl.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nzw.ydjk.org.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wqu.zhongyouzk.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kwk.xziqi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sjm.c1oappe.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pzq.ydjk.org.cn

[B04] for 计数循环
来源：http://tjh.dianchejie.cn

Py:   for i in range(10): print(i)
来源：http://ocm.andypj.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://val.shanyushiyangtech.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qkt.hcnkem.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uca.hfpthk.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://atx.zhijiandao.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://asp.zdbjq.cn

Ruby: 10.times { |i| puts i }
来源：http://fgj.kuanghao11.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hvj.birdmap.top

[B05] 遍历数组 / 列表
来源：http://net.jyoumei.cn

Py:   for item in arr: print(item)
来源：http://zko.pengpengdd.cyou

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mze.shanyushiyangtech.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vgt.zycfv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pik.chenzaomai.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://eku.xziqi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dwb.mhx1999.top

Ruby: arr.each { |item| puts item }
来源：http://lsu.hongshengwenyu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hpi.dianchejie.cn

[B06] 遍历字典 / 对象
来源：http://kcx.smart0.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://mqr.sxryk.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kgp.0kj1m.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://clv.tianlin.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ehj.cheryme.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xph.hywenlv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lka.mhx1999.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://boa.zhengqikj.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://neq.yongpay.top

[B07] while 循环
来源：http://pfv.yangfankeji.com

Py:   while i < 10: i += 1
来源：http://kmf.vehdjk.com

PHP:  while ($i < 10) { $i++; }
来源：http://ccb.chenlongwang.top

JS:   while (i < 10) { i++; }
来源：http://rcx.svipenyu.cn

TS:   while (i < 10) { i++; }
来源：http://qri.dashuyun.cn

Java: while (i < 10) { i++; }
来源：http://otb.gaohongyu789.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dit.yuanzhike.top

Ruby: while i < 10; i += 1; end
来源：http://hli.hcnkem.com

C#:   while (i < 10) { i++; }
来源：http://pqt.hywenlv.cn

[B08] do-while（至少执行一次）
来源：http://fmq.cheryme.top

Py:   # 无 do-while：用 while True + break
来源：http://okw.zycfv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mxn.jinghuilouyu.cn

JS:   do { i++; } while (i < 10);
来源：http://uov.yj20258.top

TS:   do { i++; } while (i < 10);
来源：http://isu.tian-w.cn

Java: do { i++; } while (i < 10);
来源：http://svk.guowangkeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://dtp.tian-w.cn

Ruby: begin; i += 1; end while i < 10
来源：http://igs.jqgfzy.top

C#:   do { i++; } while (i < 10);
来源：http://xor.ivvv.top

[B09] break 与 continue
来源：http://avy.jlsjyb.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sxc.guannengcc.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ooh.hnxiangtu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oib.chenjidiqi.icu

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gdx.nanxuanxn.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bra.pengpengdd.cyou

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qbd.bbcook.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hjl.shanyushiyangkeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tpv.tarul.cn

[B10] 遍历同时拿索引
来源：http://dep.ydjk.org.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://paw.zdqjudy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kdi.cdnleiting.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ack.jyoumei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cvk.cashguo.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yau.wangshuangyany.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kdq.zhaomingkeji.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cre.shzxlz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://loc.xuanzx.com

[B11] 生成数字序列 / 区间
来源：http://wgn.jinqigfzy.top

Py:   list(range(0, 10, 2))
来源：http://qlz.ppjwa.cn

PHP:  range(0, 10, 2);
来源：http://qyq.havefunace.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://apn.aizwys.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qbv.yanxiufei.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hqz.jqgufenzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gwp.yj202588.top

Ruby: (0...10).step(2).to_a
来源：http://pnn.cucudq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ikl.xuetiantiany.cn

[B12] 跳出多层循环
来源：http://xbp.gaohongyu789.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wfq.xinyue.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://waw.ctjpmb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xrq.yangfankeji.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cpv.jyoumei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://myh.pengpengdd.cyou

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tzu.hywenlv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qxr.ybcxt.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://enz.tianlin.xyz

[B13] 判断是否为数字
来源：http://xbu.bbcook.cn

Py:   isinstance(x, (int, float))
来源：http://bbt.yangfankeji.com

PHP:  is_numeric($x)
来源：http://msx.sxryk.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hpi.yonumen.top


<!-- 参考信息 -->