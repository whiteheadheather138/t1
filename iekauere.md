代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://nsw.dashuyun.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xff.hnqzz.top

C#:   x.GetType().Name; x is int
来源：http://sph.jiagoushi.top

[A05] 整数除法与取模
来源：http://sfn.birdmap.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://emr.fktsv.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://tie.kuanghao11.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://evu.snrcjt.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xcf.c1oappe.top

Java: 7 / 2; 7 % 2
来源：http://amu.sweek.top

Go:   7 / 2; 7 % 2
来源：http://ief.wangdashe.top

Ruby: 7 / 2; 7 % 2
来源：http://zpk.hysaishi.cn

C#:   7 / 2; 7 % 2
来源：http://dni.yuanzhike.top

[A06] 字符串转数字
来源：http://lpx.jiagoushi.top

Py:   int("42"); float("3.14")
来源：http://mnr.haohaochexian.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://grw.yonumen.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://azj.jinqigufen.top

TS:   parseInt("42", 10); Number("42")
来源：http://mps.hnqzz.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://uzy.aizwys.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://asu.tarul.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://tcc.ppjwa.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mcd.gotoacloud.top

[A07] 数字转字符串
来源：http://ujr.zhengqikj.top

Py:   str(42)
来源：http://mps.zycfv.cn

PHP:  (string) 42; strval(42)
来源：http://rpq.yuanzhike.top

JS:   String(42); (42).toString()
来源：http://snp.ctjpmb.com

TS:   String(42)
来源：http://rgi.yongpay.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://wca.jqgufenzy.top

Go:   strconv.Itoa(42)
来源：http://zsl.nanxinkj.top

Ruby: 42.to_s
来源：http://fpw.ydjk.org.cn

C#:   42.ToString()
来源：http://ttb.chenlongwang.top

[A08] 取整与四舍五入
来源：http://rnq.yuxming.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gdn.shanyushiyangkeji.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lvn.chenjidiqi.icu

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sqw.ydjk.org.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zkv.fengsongda.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zup.gaohongyu789.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pva.xuanzx.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://tmm.nanxuanxn.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zbm.vqdsnc.cn

[A09] 绝对值与最大最小值
来源：http://lra.yfazqb.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fgj.vehdjk.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zon.fengsongda.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mqh.daxiang520.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kih.yj202588.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://smj.fengsongda.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rml.ivvv.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hck.yuxming.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mze.yj202588.top

[A10] 生成随机数
来源：http://fpz.hongshengwenyu.top

Py:   import random; random.randint(1, 100)
来源：http://xjv.zhijiandao.cn

PHP:  random_int(1, 100);
来源：http://lef.ctjpmb.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kjd.tanke756.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qlu.hnxiangtu.top

Java: new Random().nextInt(100) + 1
来源：http://kgx.sysykeji.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zlf.xziqi.cn

Ruby: rand(1..100)
来源：http://dgm.nanxuanxn.top

C#:   new Random().Next(1, 101)
来源：http://lxi.xuetiantiany.cn

[A11] 条件表达式（三元）
来源：http://lpk.wangdashe.top

Py:   "yes" if x > 0 else "no"
来源：http://xbt.vqdsnc.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://aae.gogol.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://crb.ybcxt.top

TS:   x > 0 ? "yes" : "no"
来源：http://nws.hfpthk.cn

Java: x > 0 ? "yes" : "no"
来源：http://tqi.redwolf501.top

Go:   // 无三元运算符，需用 if 语句
来源：http://jyi.ydzc1.top

Ruby: x > 0 ? "yes" : "no"
来源：http://gwb.52xcode.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hcr.tarul.cn

[A12] 字符串插值 / 格式化
来源：http://ybo.316326.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wnf.fehbvm.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://whg.xingfuxueyuan.xyz

JS:   `Hello, ${name}!`
来源：http://uwx.kuanghao11.cn

TS:   `Hello, ${name}!`
来源：http://lyu.fktsv.cn

Java: "Hello, %s!".formatted(name)
来源：http://ilc.haohaochexian.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fva.wangdashe.top

Ruby: "Hello, #{name}!"
来源：http://thb.hesvh.cn

C#:   $"Hello, {name}!"
来源：http://lkn.svipenyu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://yzo.quarkkingdee.top

Py:   "第一行\n第二行"
来源：http://gbl.hcnkem.com

PHP:  "第一行\n第二行"
来源：http://zca.sweek.top

JS:   "第一行\n第二行"
来源：http://xzf.zhixingplan.top

TS:   "第一行\n第二行"
来源：http://hfp.nanxuanxn.top

Java: "第一行\n第二行"
来源：http://tpf.chenjidiqi.icu

Go:   "第一行\n第二行"
来源：http://sjz.andypj.xyz

Ruby: "第一行\n第二行"
来源：http://ymr.hnqzz.top

C#:   "第一行\n第二行"
来源：http://qmk.chenjidiqi.icu

[A14] 注释写法
来源：http://ozp.aibaodan.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wdc.zycfv.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sae.ybcxt.top

JS:   // 单行；/* 多行 */
来源：http://slf.bbcook.cn

TS:   // 单行；/* 多行 */
来源：http://xee.yvedp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ibq.tian-w.cn

Go:   // 单行；/* 多行 */
来源：http://bbw.xziqi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ypy.zhongyouzk.top

C#:   // 单行；/* 多行 */
来源：http://ttd.snrcjt.cn

[A15] 空值判断与默认值
来源：http://uaz.tian-w.cn

Py:   value = data or "默认值"
来源：http://lgf.yueranfly.top

PHP:  $value = $data ?? "默认值";
来源：http://mis.hesvh.cn

JS:   const value = data ?? "默认值";
来源：http://yce.zdqjudy.top

TS:   const value = data ?? "默认值";
来源：http://qik.shuidangran.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://stj.hysaishi.cn

Go:   if data == "" { data = "默认值" }
来源：http://gxf.jinqigufen.top

Ruby: value = data || "默认值"
来源：http://zit.bbcook.cn

C#:   var value = data ?? "默认值";
来源：http://xbp.jqgfzy.top

[A16] 真假值判断规则
来源：http://ukz.fehbvm.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gks.jinqigfzy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kkl.jyoumei.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sgv.meibo888.top

TS:   if (!x) {}
来源：http://ygc.jyoumei.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tda.chenjidiqi.icu

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ljw.zhoulong.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://pfb.ctjpmb.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ivq.sweek.top

[A17] 位运算
来源：http://nja.vehdjk.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vlv.jianghu66.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zar.xinyue.icu

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tzt.hesvh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vtr.wangshuangyany.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://psy.zhongyouzk.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bvz.fehbvm.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ife.ppjwa.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sid.xylfe.cn

[A18] 字符与 ASCII 码互转
来源：http://rcs.vehdjk.com

Py:   ord("A"); chr(65)
来源：http://hin.zhaomingkeji.xyz

PHP:  ord("A"); chr(65)
来源：http://ouf.pycfn.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xsm.xingfuxueyuan.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sii.gzhubu.top

Java: (int) 'A'; (char) 65
来源：http://xsr.shzxlz.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pkh.chenzaomai.com

Ruby: "A".ord; 65.chr
来源：http://xpm.hnxiangtu.top

C#:   (int)'A'; (char)65
来源：http://wsh.xuetiantiany.cn

[A19] 交换两个变量
来源：http://wxf.vehdjk.com

Py:   a, b = b, a
来源：http://edo.ydzc1.top

PHP:  [$a, $b] = [$b, $a];
来源：http://emr.zhijiandao.cn

JS:   [a, b] = [b, a];
来源：http://qoo.feifeiyinyue.top

TS:   [a, b] = [b, a];
来源：http://kwz.ehwqpu.com

Java: int t = a; a = b; b = t;
来源：http://kqc.tianlin.xyz

Go:   a, b = b, a
来源：http://uhy.chenlongwang.top

Ruby: a, b = b, a
来源：http://whl.yangfankeji.com

C#:   (a, b) = (b, a);
来源：http://mlh.zhoulong.xyz

[A20] 读取标准输入
来源：http://bpd.zhixingplan.top

Py:   name = input("请输入：")
来源：http://efn.andypj.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://fhn.yanxiufei.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yog.hesvh.cn

TS:   // Node.js：readline 模块
来源：http://igh.quarkkingdee.top

Java: new Scanner(System.in).nextLine()
来源：http://bwm.svipenyu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ban.sjlbkw.cn

Ruby: gets.chomp
来源：http://yfi.xuetiantiany.cn

C#:   Console.ReadLine();
来源：http://crl.52xcode.cn

[A21] 保留指定小数位输出
来源：http://sip.sjlbkw.cn

Py:   f"{3.14159:.2f}"
来源：http://iaz.cashguo.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yhc.meibo888.top

JS:   (3.14159).toFixed(2)
来源：http://ivg.yonumen.top

TS:   (3.14159).toFixed(2)
来源：http://xlm.hywenlv.cn

Java: String.format("%.2f", 3.14159)
来源：http://zoc.snrcjt.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jps.jiagoushi.top

Ruby: format("%.2f", 3.14159)
来源：http://ktl.zhengqikj.top

C#:   3.14159.ToString("F2")
来源：http://hcb.gogol.net.cn

[A22] 获取字符串长度
来源：http://gyi.zhengqikj.top

Py:   len(s)
来源：http://syi.jqgfzy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://byn.fzhhl.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ovw.c1oappe.top

TS:   s.length
来源：http://jrv.dashuyun.cn

Java: s.length()
来源：http://sjc.gotoacloud.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mof.chenzaomai.com

Ruby: s.length
来源：http://uvv.yfazqb.com

C#:   s.Length
来源：http://muc.zdbjq.cn

[A23] 大小写转换
来源：http://ptr.sufxvd.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zew.jqgfzy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://szx.cheryme.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gms.zhoulong.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://unz.jinghuilouyu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jvu.c1oappe.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kdw.zhengqikj.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://itv.guannengcc.top

C#:   s.ToUpper(); s.ToLower()
来源：http://hav.snrcjt.cn

[A24] 去除首尾空白
来源：http://zcb.ybcxt.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pzi.quarkkingdee.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iok.ywan-chungtsiang.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lba.mhx1999.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ths.epnwcf.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vmn.shuidangran.top

Go:   strings.TrimSpace(s)
来源：http://adl.redwolf501.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pmk.sufxvd.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gvi.52xcode.cn

[A25] 字符串比较
来源：http://ldg.svipenyu.cn

Py:   s1 == s2; s1 != s2
来源：http://zrf.jiagoushi.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wha.ydzc1.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tyz.shzxlz.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ffx.redwolf501.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lzo.ctjpmb.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nfj.cashguo.top

Ruby: s1 == s2; s1 <=> s2
来源：http://nir.cqqwz.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nix.jiagoushi.top

[A26] 类型转换总览
来源：http://geq.jinghuilouyu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ukw.aibaodan.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gps.c1oappe.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pxs.c1oappe.top

TS:   Number() String() Boolean() x as number
来源：http://krv.hcnkem.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vro.gogol.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ruf.ivvv.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://esg.redwolf501.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ncv.hongshengwenyu.top

================================================================================
来源：http://ugb.jqgufenzy.top

B. 流程控制
来源：http://enb.yfazqb.com

================================================================================
来源：http://nek.hnqzz.top

[B01] 条件判断 if / else
来源：http://rfm.jinqigfzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://nkz.yvedp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baa.dashuyun.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cnr.9152youxi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hks.yueranfly.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://lph.hysaishi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://buo.zdqjudy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dfk.hysaishi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yvk.quarkkingdee.top

[B02] 多分支 else if / elif
来源：http://upt.kuanghao11.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jqi.hysaishi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kmk.guannengcc.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rhv.hongshengwenyu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fsz.bbcook.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zpi.bbcook.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jzf.hammf.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tww.havefunace.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gga.dianchejie.cn

[B03] switch / match / case
来源：http://huh.tian-w.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zxt.bjfxy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dzi.jiagoushi.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pli.tianlin.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vog.gaohongyu789.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://eab.chenlongwang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qox.wangshuangyany.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hfq.dianchejie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fuz.jqgfzy.top

[B04] for 计数循环
来源：http://wxn.haohaochexian.top

Py:   for i in range(10): print(i)
来源：http://nvm.redwolf501.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://inb.pengpengdd.cyou

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fdu.fehbvm.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gve.quarkkingdee.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://unl.zdqjudy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://umh.zycfv.cn

Ruby: 10.times { |i| puts i }
来源：http://qoe.zdqjudy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://prr.hcnkem.com

[B05] 遍历数组 / 列表
来源：http://mov.kuanghao11.cn

Py:   for item in arr: print(item)
来源：http://jbi.hcnkem.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sxn.pycfn.com

JS:   for (const item of arr) { console.log(item); }
来源：http://kdd.gzhubu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://srd.yj20258888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://cbk.aibaodan.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://erw.tanke756.top

Ruby: arr.each { |item| puts item }
来源：http://uni.vqdsnc.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pmz.guannengcc.top

[B06] 遍历字典 / 对象
来源：http://iiz.hywenlv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nsl.yfazqb.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://maw.zdqjudy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dqg.jqgufenzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tng.zdbjq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://keq.nanxinkj.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lcw.yonumen.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jrt.fzhhl.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nii.bbcook.cn

[B07] while 循环
来源：http://bmq.fehbvm.com

Py:   while i < 10: i += 1
来源：http://rak.shangyingyoupin.top

PHP:  while ($i < 10) { $i++; }
来源：http://vmo.epnwcf.com

JS:   while (i < 10) { i++; }
来源：http://wby.hywenlv.cn

TS:   while (i < 10) { i++; }
来源：http://wrv.zycfv.cn

Java: while (i < 10) { i++; }
来源：http://dtf.meibo888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tmn.zhiwuduotai.top

Ruby: while i < 10; i += 1; end
来源：http://tbz.fengsongda.top

C#:   while (i < 10) { i++; }
来源：http://jkr.jyoumei.cn

[B08] do-while（至少执行一次）
来源：http://gce.gogol.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://ige.nwbrower.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ijo.jqgufenzy.top

JS:   do { i++; } while (i < 10);
来源：http://fhn.tianlin.xyz

TS:   do { i++; } while (i < 10);
来源：http://div.yj20258888.top

Java: do { i++; } while (i < 10);
来源：http://myn.xylfe.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ygh.aibaodan.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mlz.svipenyu.cn

C#:   do { i++; } while (i < 10);
来源：http://rsw.sweek.top

[B09] break 与 continue
来源：http://prp.birdmap.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zox.vqdsnc.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hol.yj202588.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://byv.wangshuangyany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iby.dashuyun.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ota.tianlin.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zle.chenlongwang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bzs.mhx1999.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://met.cucudq.cn

[B10] 遍历同时拿索引
来源：http://ivh.daxiang520.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ajp.jianghu66.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rtc.tanke756.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jko.yj202588.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ysa.52xcode.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dqs.yj202588.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bia.tian-w.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wwr.smart0.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qnc.jqgfzy.top

[B11] 生成数字序列 / 区间
来源：http://kaw.cdnleiting.top

Py:   list(range(0, 10, 2))
来源：http://arh.pycfn.com

PHP:  range(0, 10, 2);
来源：http://zhe.zhoulong.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rde.yanxiufei.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zyl.jqgfzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tvk.aibaodan.cn


<!-- 参考信息 -->