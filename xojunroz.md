代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://iqr.sjlbkw.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://com.chenjidiqi.icu

C#:   x.GetType().Name; x is int
来源：http://qtr.ywan-chungtsiang.top

[A05] 整数除法与取模
来源：http://fku.yj20258.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ncq.yj20258.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://kqv.pycfn.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://chc.yvedp.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hue.316326.xyz

Java: 7 / 2; 7 % 2
来源：http://evg.jqgfzy.top

Go:   7 / 2; 7 % 2
来源：http://jtx.andypj.xyz

Ruby: 7 / 2; 7 % 2
来源：http://zmt.pengpengdd.cyou

C#:   7 / 2; 7 % 2
来源：http://sao.zdqjudy.top

[A06] 字符串转数字
来源：http://vpy.cucudq.cn

Py:   int("42"); float("3.14")
来源：http://nkv.yangfankeji.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fmv.haohaochexian.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fwn.epnwcf.com

TS:   parseInt("42", 10); Number("42")
来源：http://paz.cucudq.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ogf.daxiang520.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cor.cdnleiting.top

Ruby: "42".to_i; "3.14".to_f
来源：http://hfp.sjlbkw.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dbk.dianchejie.cn

[A07] 数字转字符串
来源：http://ogh.yongpay.top

Py:   str(42)
来源：http://uyx.meibo888.top

PHP:  (string) 42; strval(42)
来源：http://pmr.xingfuxueyuan.xyz

JS:   String(42); (42).toString()
来源：http://sht.guannengcc.top

TS:   String(42)
来源：http://ldd.pengpengdd.cyou

Java: String.valueOf(42); Integer.toString(42)
来源：http://hfx.52xcode.cn

Go:   strconv.Itoa(42)
来源：http://cfn.fzhhl.top

Ruby: 42.to_s
来源：http://utw.shanyushiyangtech.top

C#:   42.ToString()
来源：http://yjb.yanxiufei.cn

[A08] 取整与四舍五入
来源：http://oyl.sjlbkw.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kun.bbcook.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dgt.ydzc1.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://drt.yj20258888.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mcy.daxiang520.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lkp.sysykeji.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fat.redwolf501.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://xwf.yj202588.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ylu.xuanzx.com

[A09] 绝对值与最大最小值
来源：http://vhy.hnqzz.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://psg.ydzc1.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kpd.tianlin.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wra.zhixingplan.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ybb.kuanghao11.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bwv.zycfv.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mzl.xziqi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://spu.yfazqb.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ghz.gotoacloud.top

[A10] 生成随机数
来源：http://hwb.yangfankeji.com

Py:   import random; random.randint(1, 100)
来源：http://xkc.ctjpmb.com

PHP:  random_int(1, 100);
来源：http://tsp.jqgufenzy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dbf.sxryk.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ppy.chenlongwang.top

Java: new Random().nextInt(100) + 1
来源：http://hrs.ydzc1.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://awk.dianchejie.cn

Ruby: rand(1..100)
来源：http://gsw.gaohongyu789.top

C#:   new Random().Next(1, 101)
来源：http://xra.cqqwz.cn

[A11] 条件表达式（三元）
来源：http://mvc.gotoacloud.top

Py:   "yes" if x > 0 else "no"
来源：http://jjd.gogol.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dww.nanxinkj.top

JS:   x > 0 ? "yes" : "no"
来源：http://bnr.hnxiangtu.top

TS:   x > 0 ? "yes" : "no"
来源：http://tfb.ctjpmb.com

Java: x > 0 ? "yes" : "no"
来源：http://cxw.jianghu66.top

Go:   // 无三元运算符，需用 if 语句
来源：http://mmr.ydjk.org.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bil.xinyue.icu

C#:   x > 0 ? "yes" : "no"
来源：http://yds.aizwys.cn

[A12] 字符串插值 / 格式化
来源：http://noa.c1oappe.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fqc.jinyuanbaomall.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yld.hfpthk.cn

JS:   `Hello, ${name}!`
来源：http://yma.vehdjk.com

TS:   `Hello, ${name}!`
来源：http://qrt.zhengqikj.top

Java: "Hello, %s!".formatted(name)
来源：http://abg.jqgufenzy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ksa.andypj.xyz

Ruby: "Hello, #{name}!"
来源：http://sjl.hammf.cn

C#:   $"Hello, {name}!"
来源：http://dnf.yj202588.top

[A13] 多行字符串（练习 \n 转义）
来源：http://kgk.jqgufenzy.top

Py:   "第一行\n第二行"
来源：http://ftv.gogol.net.cn

PHP:  "第一行\n第二行"
来源：http://wkt.chenlongwang.top

JS:   "第一行\n第二行"
来源：http://lmx.gzhubu.top

TS:   "第一行\n第二行"
来源：http://wjf.zhixingplan.top

Java: "第一行\n第二行"
来源：http://utd.mhx1999.top

Go:   "第一行\n第二行"
来源：http://vby.gaohongyu789.top

Ruby: "第一行\n第二行"
来源：http://goz.bjfxy.top

C#:   "第一行\n第二行"
来源：http://imm.redwolf501.top

[A14] 注释写法
来源：http://ges.jianghu66.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://xyf.sysykeji.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://epp.cashguo.top

JS:   // 单行；/* 多行 */
来源：http://efv.tanke756.top

TS:   // 单行；/* 多行 */
来源：http://ukf.yj20258.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vxu.zhaomingkeji.xyz

Go:   // 单行；/* 多行 */
来源：http://rro.smart0.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://vxn.sweek.top

C#:   // 单行；/* 多行 */
来源：http://gtb.sysykeji.top

[A15] 空值判断与默认值
来源：http://xvb.quarkkingdee.top

Py:   value = data or "默认值"
来源：http://xwk.tianlin.xyz

PHP:  $value = $data ?? "默认值";
来源：http://nqk.tian-w.cn

JS:   const value = data ?? "默认值";
来源：http://bcz.daria6918.cn

TS:   const value = data ?? "默认值";
来源：http://lqq.hnqzz.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://izw.hfpthk.cn

Go:   if data == "" { data = "默认值" }
来源：http://bvv.nwbrower.top

Ruby: value = data || "默认值"
来源：http://ini.shangyingyoupin.top

C#:   var value = data ?? "默认值";
来源：http://jaw.gogol.net.cn

[A16] 真假值判断规则
来源：http://cxr.zdbjq.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://usf.aizwys.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qom.yueranfly.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://oba.jinqigufen.top

TS:   if (!x) {}
来源：http://imx.hammf.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://izl.shanyushiyangtech.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mqe.jiagoushi.top

Ruby: unless x            # nil 与 false 为假
来源：http://aan.bjfxy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cfr.jianghu66.top

[A17] 位运算
来源：http://hvq.jqgfzy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ibo.fengsongda.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fdx.zhoulong.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vxb.xylfe.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lvj.gzhubu.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://svf.svipenyu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cgv.nwbrower.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ppg.shangyingyoupin.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://auh.ydjk.org.cn

[A18] 字符与 ASCII 码互转
来源：http://qtt.pycfn.com

Py:   ord("A"); chr(65)
来源：http://gjk.yvedp.cn

PHP:  ord("A"); chr(65)
来源：http://aqq.guannengcc.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kfd.ctjpmb.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wvo.hongshengwenyu.top

Java: (int) 'A'; (char) 65
来源：http://mty.gzhubu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://btr.yueranfly.top

Ruby: "A".ord; 65.chr
来源：http://bue.chenlongwang.top

C#:   (int)'A'; (char)65
来源：http://vvk.meibo888.top

[A19] 交换两个变量
来源：http://tpa.shangyingyoupin.top

Py:   a, b = b, a
来源：http://ckn.fzhhl.top

PHP:  [$a, $b] = [$b, $a];
来源：http://nxn.smart0.xyz

JS:   [a, b] = [b, a];
来源：http://gqv.52xcode.cn

TS:   [a, b] = [b, a];
来源：http://cjn.epnwcf.com

Java: int t = a; a = b; b = t;
来源：http://zgy.chenjidiqi.icu

Go:   a, b = b, a
来源：http://zdh.zhixingplan.top

Ruby: a, b = b, a
来源：http://zxv.yonumen.top

C#:   (a, b) = (b, a);
来源：http://ahk.yfazqb.com

[A20] 读取标准输入
来源：http://ndk.ydjk.org.cn

Py:   name = input("请输入：")
来源：http://eel.jlsjyb.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jeg.316326.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qil.hesvh.cn

TS:   // Node.js：readline 模块
来源：http://xvt.cucudq.cn

Java: new Scanner(System.in).nextLine()
来源：http://zvc.c1oappe.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xvd.shzxlz.cn

Ruby: gets.chomp
来源：http://iko.bbcook.cn

C#:   Console.ReadLine();
来源：http://hmw.zhaomingkeji.xyz

[A21] 保留指定小数位输出
来源：http://seb.yueranfly.top

Py:   f"{3.14159:.2f}"
来源：http://hki.svipenyu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://sxj.ppjwa.cn

JS:   (3.14159).toFixed(2)
来源：http://dfl.xingfuxueyuan.xyz

TS:   (3.14159).toFixed(2)
来源：http://xaq.zdbjq.cn

Java: String.format("%.2f", 3.14159)
来源：http://qgg.hnxiangtu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ozd.vqdsnc.cn

Ruby: format("%.2f", 3.14159)
来源：http://jnn.ivvv.top

C#:   3.14159.ToString("F2")
来源：http://vxl.aibaodan.cn

[A22] 获取字符串长度
来源：http://qig.havefunace.top

Py:   len(s)
来源：http://zki.yanxiufei.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://grc.ybcxt.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nih.dianchejie.cn

TS:   s.length
来源：http://hzf.daria6918.cn

Java: s.length()
来源：http://tis.tian-w.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mqp.zhongyouzk.top

Ruby: s.length
来源：http://zgo.xylfe.cn

C#:   s.Length
来源：http://vbe.sweek.top

[A23] 大小写转换
来源：http://iqp.zhaomingkeji.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://jzx.redwolf501.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sgf.yonumen.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xcr.zdqjudy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sba.feifeiyinyue.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://eim.nanxinkj.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mfn.gzhubu.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fjv.fktsv.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nhh.wangshuangyany.cn

[A24] 去除首尾空白
来源：http://jns.9152youxi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://spi.hnqzz.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://amu.hammf.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zzs.wangdashe.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sin.chenlongwang.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mas.jinyuanbaomall.cn

Go:   strings.TrimSpace(s)
来源：http://xny.jlsjyb.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hbt.sxryk.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jsl.feifeiyinyue.top

[A25] 字符串比较
来源：http://ses.hammf.cn

Py:   s1 == s2; s1 != s2
来源：http://gpd.fanxiaobao.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tny.quarkkingdee.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qwo.tian-w.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kuf.yj20258888.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kgz.sysykeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jso.9152youxi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yni.yangfankeji.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ixv.yfazqb.com

[A26] 类型转换总览
来源：http://ydq.chenlongwang.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bvw.hesvh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cak.meibo888.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yll.aibaodan.cn

TS:   Number() String() Boolean() x as number
来源：http://qbf.shanyushiyangtech.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zhp.tianlin.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kss.havefunace.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://fnw.tarul.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yuo.shanyushiyangkeji.top

================================================================================
来源：http://szd.zhengqikj.top

B. 流程控制
来源：http://gee.chenzaomai.com

================================================================================
来源：http://xro.ybcxt.top

[B01] 条件判断 if / else
来源：http://mwy.jinqigfzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://uko.xinyue.icu

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lic.zdqjudy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zxr.jinqigufen.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wrb.chenzaomai.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://cpn.dianchejie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zcc.jlsjyb.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uoc.yj20258.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bdn.zdqjudy.top

[B02] 多分支 else if / elif
来源：http://tkx.xinyue.icu

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://txx.yvedp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://thv.zhongyouzk.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jtl.ivvv.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sns.epnwcf.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qeq.ydjk.org.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vbn.quarkkingdee.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tvq.jinqigufen.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yzr.ybcxt.top

[B03] switch / match / case
来源：http://ptb.yvedp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://exl.andypj.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qeg.aizwys.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://snm.jinghuilouyu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zwg.epnwcf.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rob.yongpay.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kfq.chenlongwang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fkv.jlsjyb.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vyg.xziqi.cn

[B04] for 计数循环
来源：http://xjh.jiagoushi.top

Py:   for i in range(10): print(i)
来源：http://ofu.ywan-chungtsiang.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ans.iojbl.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ukn.gzhubu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sdm.pengpengdd.cyou

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://leq.uphjek.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kpw.sufxvd.cn

Ruby: 10.times { |i| puts i }
来源：http://szu.hnqzz.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pmd.hammf.cn

[B05] 遍历数组 / 列表
来源：http://had.yuxming.cn

Py:   for item in arr: print(item)
来源：http://egg.cdnleiting.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://owa.zhengqikj.top

JS:   for (const item of arr) { console.log(item); }
来源：http://uac.gzhubu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://jaj.ydzc1.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mdv.fehbvm.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lar.vqdsnc.cn

Ruby: arr.each { |item| puts item }
来源：http://djj.tianlin.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uih.tanke756.top

[B06] 遍历字典 / 对象
来源：http://ceq.zycfv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qlj.chenlongwang.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://myr.daxiang520.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pcf.sjlbkw.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qje.fengsongda.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ypp.feifeiyinyue.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://aee.jinyuanbaomall.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ylw.bjfxy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rni.zdbjq.cn

[B07] while 循环
来源：http://ozp.sufxvd.cn

Py:   while i < 10: i += 1
来源：http://wzg.9152youxi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kdu.jyoumei.cn

JS:   while (i < 10) { i++; }
来源：http://ibb.mhx1999.top

TS:   while (i < 10) { i++; }
来源：http://qlt.smart0.xyz

Java: while (i < 10) { i++; }
来源：http://lfo.fehbvm.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vuz.cqqwz.cn

Ruby: while i < 10; i += 1; end
来源：http://mis.yj20258888.top

C#:   while (i < 10) { i++; }
来源：http://jdn.andypj.xyz

[B08] do-while（至少执行一次）
来源：http://wkn.quarkkingdee.top

Py:   # 无 do-while：用 while True + break
来源：http://aii.yuanzhike.top

PHP:  do { $i++; } while ($i < 10);
来源：http://thw.zdqjudy.top

JS:   do { i++; } while (i < 10);
来源：http://ptb.tianlin.xyz

TS:   do { i++; } while (i < 10);
来源：http://lly.zhixingplan.top

Java: do { i++; } while (i < 10);
来源：http://ell.feifeiyinyue.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ltc.cdnleiting.top

Ruby: begin; i += 1; end while i < 10
来源：http://wes.yonumen.top

C#:   do { i++; } while (i < 10);
来源：http://fiv.nanxuanxn.top

[B09] break 与 continue
来源：http://psr.xuetiantiany.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ihj.cdnleiting.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cil.sysykeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xdu.iojbl.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qpz.shzxlz.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ujk.yuanzhike.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rht.pycfn.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mme.hammf.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wvv.yongpay.top

[B10] 遍历同时拿索引
来源：http://yav.fehbvm.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://akh.zhijiandao.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tad.yfazqb.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://etj.gaohongyu789.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yfy.cdnleiting.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://len.aibaodan.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://iuv.zhiwuduotai.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wxv.svipenyu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://irl.hcnkem.com

[B11] 生成数字序列 / 区间
来源：http://rrp.andypj.xyz

Py:   list(range(0, 10, 2))
来源：http://wfj.zhiwuduotai.top

PHP:  range(0, 10, 2);
来源：http://bti.shzxlz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cxa.chenzaomai.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zsl.fengsongda.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zyg.hesvh.cn


<!-- 参考信息 -->