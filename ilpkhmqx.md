代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://mrv.hfpthk.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dmg.quarkkingdee.top

C#:   x.GetType().Name; x is int
来源：http://tnp.yj202588.top

[A05] 整数除法与取模
来源：http://pet.quarkkingdee.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qus.9152youxi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://yrn.xuetiantiany.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qzp.pycfn.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://duf.jqgfzy.top

Java: 7 / 2; 7 % 2
来源：http://fmb.0kj1m.cn

Go:   7 / 2; 7 % 2
来源：http://mjw.yj202588.top

Ruby: 7 / 2; 7 % 2
来源：http://sxf.tianlin.xyz

C#:   7 / 2; 7 % 2
来源：http://ggq.sweek.top

[A06] 字符串转数字
来源：http://gyn.cqqwz.cn

Py:   int("42"); float("3.14")
来源：http://hoz.guannengcc.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jot.redwolf501.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rqi.bjfxy.top

TS:   parseInt("42", 10); Number("42")
来源：http://fng.vqdsnc.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fqh.hfpthk.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lch.tarul.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://osr.mhx1999.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vuz.xziqi.cn

[A07] 数字转字符串
来源：http://oao.zhaomingkeji.xyz

Py:   str(42)
来源：http://xns.sweek.top

PHP:  (string) 42; strval(42)
来源：http://lvs.pengpengdd.cyou

JS:   String(42); (42).toString()
来源：http://uwd.zhaomingkeji.xyz

TS:   String(42)
来源：http://iua.nanxinkj.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://cmj.jqgfzy.top

Go:   strconv.Itoa(42)
来源：http://ltq.wangdashe.top

Ruby: 42.to_s
来源：http://ftg.fanxiaobao.xyz

C#:   42.ToString()
来源：http://twv.hcnkem.com

[A08] 取整与四舍五入
来源：http://roe.jinghuilouyu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lmi.hesvh.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jgo.hcnkem.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pdj.shuidangran.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://eta.xingfuxueyuan.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xdk.smart0.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://igg.9152youxi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zvq.birdmap.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xdd.dashuyun.cn

[A09] 绝对值与最大最小值
来源：http://stk.yuxming.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pqb.xingfuxueyuan.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lht.yangfankeji.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lpb.gaohongyu789.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bbh.zdqjudy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wkm.shanyushiyangkeji.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lnk.feifeiyinyue.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://psx.jinqigfzy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://axx.zhoulong.xyz

[A10] 生成随机数
来源：http://fni.ctjpmb.com

Py:   import random; random.randint(1, 100)
来源：http://ezx.guowangkeji.top

PHP:  random_int(1, 100);
来源：http://pns.zycfv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hcy.wangdashe.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qhv.jianghu66.top

Java: new Random().nextInt(100) + 1
来源：http://tfl.xziqi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jdo.yuxming.cn

Ruby: rand(1..100)
来源：http://gnn.yuanzhike.top

C#:   new Random().Next(1, 101)
来源：http://nik.aizwys.cn

[A11] 条件表达式（三元）
来源：http://ecb.fzhhl.top

Py:   "yes" if x > 0 else "no"
来源：http://ndy.hnxiangtu.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://mty.sjlbkw.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ziq.sufxvd.cn

TS:   x > 0 ? "yes" : "no"
来源：http://fmk.yj20258.top

Java: x > 0 ? "yes" : "no"
来源：http://plx.zhoulong.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://lqu.gotoacloud.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ntj.zdqjudy.top

C#:   x > 0 ? "yes" : "no"
来源：http://evd.tarul.cn

[A12] 字符串插值 / 格式化
来源：http://bry.316326.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zvp.gogol.net.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ggk.yueranfly.top

JS:   `Hello, ${name}!`
来源：http://sle.zycfv.cn

TS:   `Hello, ${name}!`
来源：http://dle.jyoumei.cn

Java: "Hello, %s!".formatted(name)
来源：http://lyi.yfazqb.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://aix.xingfuxueyuan.xyz

Ruby: "Hello, #{name}!"
来源：http://pij.zhiwuduotai.top

C#:   $"Hello, {name}!"
来源：http://dws.shangyingyoupin.top

[A13] 多行字符串（练习 \n 转义）
来源：http://dta.tarul.cn

Py:   "第一行\n第二行"
来源：http://ijk.jinyuanbaomall.cn

PHP:  "第一行\n第二行"
来源：http://ooc.shangyingyoupin.top

JS:   "第一行\n第二行"
来源：http://obf.jiagoushi.top

TS:   "第一行\n第二行"
来源：http://tcb.cashguo.top

Java: "第一行\n第二行"
来源：http://pad.zhixingplan.top

Go:   "第一行\n第二行"
来源：http://eez.shzxlz.cn

Ruby: "第一行\n第二行"
来源：http://xko.yj20258.top

C#:   "第一行\n第二行"
来源：http://awt.sufxvd.cn

[A14] 注释写法
来源：http://wau.haohaochexian.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://uha.fanxiaobao.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://iqs.zycfv.cn

JS:   // 单行；/* 多行 */
来源：http://jzc.sysykeji.top

TS:   // 单行；/* 多行 */
来源：http://yok.guannengcc.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zsb.yuxming.cn

Go:   // 单行；/* 多行 */
来源：http://peo.pengpengdd.cyou

Ruby: # 单行；=begin 多行 =end
来源：http://ads.quarkkingdee.top

C#:   // 单行；/* 多行 */
来源：http://bit.sweek.top

[A15] 空值判断与默认值
来源：http://lwy.jianghu66.top

Py:   value = data or "默认值"
来源：http://jnh.shuidangran.top

PHP:  $value = $data ?? "默认值";
来源：http://gde.jinqigufen.top

JS:   const value = data ?? "默认值";
来源：http://hfe.sjlbkw.cn

TS:   const value = data ?? "默认值";
来源：http://uxh.dashuyun.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yyq.hcnkem.com

Go:   if data == "" { data = "默认值" }
来源：http://pgs.gaohongyu789.top

Ruby: value = data || "默认值"
来源：http://mmb.zhijiandao.cn

C#:   var value = data ?? "默认值";
来源：http://ldc.ctjpmb.com

[A16] 真假值判断规则
来源：http://avl.cqqwz.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dyx.gotoacloud.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mlj.havefunace.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lgk.jinqigufen.top

TS:   if (!x) {}
来源：http://von.jinqigufen.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vyf.gotoacloud.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zkn.dianchejie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ksr.ybcxt.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hdz.ybcxt.top

[A17] 位运算
来源：http://icp.yongpay.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qmt.hysaishi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://avc.ehwqpu.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vcn.fktsv.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tvf.zhixingplan.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eam.yonumen.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fuz.yueranfly.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://svh.zhoulong.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kef.jlsjyb.cn

[A18] 字符与 ASCII 码互转
来源：http://ubh.chenzaomai.com

Py:   ord("A"); chr(65)
来源：http://ssz.jinqigfzy.top

PHP:  ord("A"); chr(65)
来源：http://opf.ppjwa.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zfj.kuanghao11.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xtg.cdnleiting.top

Java: (int) 'A'; (char) 65
来源：http://sbd.jinqigfzy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kho.gogol.net.cn

Ruby: "A".ord; 65.chr
来源：http://sgw.snrcjt.cn

C#:   (int)'A'; (char)65
来源：http://sxr.bjfxy.top

[A19] 交换两个变量
来源：http://cku.vehdjk.com

Py:   a, b = b, a
来源：http://ztc.hfpthk.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://uyl.jinqigfzy.top

JS:   [a, b] = [b, a];
来源：http://kpz.yuanzhike.top

TS:   [a, b] = [b, a];
来源：http://sgt.sxryk.cn

Java: int t = a; a = b; b = t;
来源：http://frm.zhijiandao.cn

Go:   a, b = b, a
来源：http://foo.jqgufenzy.top

Ruby: a, b = b, a
来源：http://ilv.cqqwz.cn

C#:   (a, b) = (b, a);
来源：http://eik.nwbrower.top

[A20] 读取标准输入
来源：http://dye.wangshuangyany.cn

Py:   name = input("请输入：")
来源：http://elh.shzxlz.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qkd.guowangkeji.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mdl.daxiang520.top

TS:   // Node.js：readline 模块
来源：http://gim.jinyuanbaomall.cn

Java: new Scanner(System.in).nextLine()
来源：http://rku.shanyushiyangkeji.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://olm.sxryk.cn

Ruby: gets.chomp
来源：http://lzp.jyoumei.cn

C#:   Console.ReadLine();
来源：http://qgp.cqqwz.cn

[A21] 保留指定小数位输出
来源：http://yia.jinyuanbaomall.cn

Py:   f"{3.14159:.2f}"
来源：http://tzo.guannengcc.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lib.yanxiufei.cn

JS:   (3.14159).toFixed(2)
来源：http://dio.ydjk.org.cn

TS:   (3.14159).toFixed(2)
来源：http://uon.jinyuanbaomall.cn

Java: String.format("%.2f", 3.14159)
来源：http://tmt.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rdd.nanxinkj.top

Ruby: format("%.2f", 3.14159)
来源：http://vmv.dianchejie.cn

C#:   3.14159.ToString("F2")
来源：http://iow.epnwcf.com

[A22] 获取字符串长度
来源：http://wim.yj202588.top

Py:   len(s)
来源：http://kgh.jinqigufen.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tdc.xinyue.icu

JS:   s.length                          # 按 UTF-16 单元计
来源：http://npf.quarkkingdee.top

TS:   s.length
来源：http://bcq.jyoumei.cn

Java: s.length()
来源：http://onp.snrcjt.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lrx.yfazqb.com

Ruby: s.length
来源：http://ghr.zhengqikj.top

C#:   s.Length
来源：http://dzz.daxiang520.top

[A23] 大小写转换
来源：http://kzm.yj20258888.top

Py:   s.upper(); s.lower(); s.title()
来源：http://pfy.c1oappe.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gjq.yuxming.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qhf.xingfuxueyuan.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nuy.aizwys.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qzy.jqgufenzy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ves.vqdsnc.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lgc.jianghu66.top

C#:   s.ToUpper(); s.ToLower()
来源：http://nul.jqgfzy.top

[A24] 去除首尾空白
来源：http://xlg.aizwys.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ffc.hnqzz.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gmm.52xcode.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bvb.shzxlz.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yhg.meibo888.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://oxs.cheryme.top

Go:   strings.TrimSpace(s)
来源：http://rwe.aibaodan.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wht.316326.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://uah.fktsv.cn

[A25] 字符串比较
来源：http://try.jinqigufen.top

Py:   s1 == s2; s1 != s2
来源：http://flf.9152youxi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zbn.yonumen.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://awn.yangfankeji.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mjq.sweek.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tuz.tian-w.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://orj.xziqi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yxs.nanxuanxn.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zoq.zhongyouzk.top

[A26] 类型转换总览
来源：http://ims.hammf.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jov.jqgfzy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qoi.yanxiufei.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bgm.feifeiyinyue.top

TS:   Number() String() Boolean() x as number
来源：http://yaq.xingfuxueyuan.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mib.zhijiandao.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qew.aibaodan.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mov.shzxlz.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fxt.9152youxi.cn

================================================================================
来源：http://aub.shzxlz.cn

B. 流程控制
来源：http://pfm.shangyingyoupin.top

================================================================================
来源：http://isg.fktsv.cn

[B01] 条件判断 if / else
来源：http://mfl.fehbvm.com

Py:   result = "正" if x > 0 else "非正"
来源：http://tip.yuanzhike.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ktc.sysykeji.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nij.nanxinkj.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rsm.cdnleiting.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://nhp.hnxiangtu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lvn.zycfv.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://whb.sysykeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nxv.yuanzhike.top

[B02] 多分支 else if / elif
来源：http://rem.yj20258888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bdh.yj20258.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rfb.zdqjudy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ltq.fzhhl.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vbl.nanxuanxn.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vjy.sufxvd.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hxa.hesvh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xeo.vqdsnc.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uim.feifeiyinyue.top

[B03] switch / match / case
来源：http://jrd.ydzc1.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://flp.mhx1999.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oom.smart0.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sul.c1oappe.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xhz.hesvh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tav.cheryme.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cvv.tanke756.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ikd.hysaishi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wio.ctjpmb.com

[B04] for 计数循环
来源：http://vxy.zdqjudy.top

Py:   for i in range(10): print(i)
来源：http://skt.ppjwa.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://eyz.yj202588.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lvk.hcnkem.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nin.zhengqikj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wfs.gaohongyu789.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kbv.zhoulong.xyz

Ruby: 10.times { |i| puts i }
来源：http://cyb.gzhubu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rmi.zhoulong.xyz

[B05] 遍历数组 / 列表
来源：http://ixe.yj202588.top

Py:   for item in arr: print(item)
来源：http://twd.sjlbkw.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://heu.sweek.top

JS:   for (const item of arr) { console.log(item); }
来源：http://pwm.kuanghao11.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bby.vqdsnc.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ipk.sweek.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://buw.hcnkem.com

Ruby: arr.each { |item| puts item }
来源：http://ala.hammf.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ylf.chenjidiqi.icu

[B06] 遍历字典 / 对象
来源：http://nak.haohaochexian.top

Py:   for k, v in d.items(): print(k, v)
来源：http://nto.sjlbkw.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hps.jiagoushi.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tjz.daxiang520.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://teg.cdnleiting.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://etp.jlsjyb.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tud.sweek.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qru.epnwcf.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nzj.ctjpmb.com

[B07] while 循环
来源：http://fgd.fzhhl.top

Py:   while i < 10: i += 1
来源：http://xfx.hcnkem.com

PHP:  while ($i < 10) { $i++; }
来源：http://emy.jianghu66.top

JS:   while (i < 10) { i++; }
来源：http://ffs.tanke756.top

TS:   while (i < 10) { i++; }
来源：http://pkj.ctjpmb.com

Java: while (i < 10) { i++; }
来源：http://djw.yuanzhike.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qis.bbcook.cn

Ruby: while i < 10; i += 1; end
来源：http://upj.sxryk.cn

C#:   while (i < 10) { i++; }
来源：http://grf.nanxuanxn.top

[B08] do-while（至少执行一次）
来源：http://nkb.shzxlz.cn

Py:   # 无 do-while：用 while True + break
来源：http://ege.tarul.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sky.hongshengwenyu.top

JS:   do { i++; } while (i < 10);
来源：http://keo.zhaomingkeji.xyz

TS:   do { i++; } while (i < 10);
来源：http://tjt.ydzc1.top

Java: do { i++; } while (i < 10);
来源：http://dxi.svipenyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://knh.ehwqpu.com

Ruby: begin; i += 1; end while i < 10
来源：http://whz.meibo888.top

C#:   do { i++; } while (i < 10);
来源：http://wms.yvedp.cn

[B09] break 与 continue
来源：http://oeg.0kj1m.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jzo.jinqigfzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ujn.sysykeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ghw.vehdjk.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tib.hammf.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fyr.ivvv.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nmv.jinqigufen.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sdw.jqgufenzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vjy.fktsv.cn

[B10] 遍历同时拿索引
来源：http://bfz.jqgfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jwf.uphjek.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mhl.fengsongda.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pfh.xingfuxueyuan.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sfl.chenzaomai.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tsu.hywenlv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bpu.xuetiantiany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lde.svipenyu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xuu.ydzc1.top

[B11] 生成数字序列 / 区间
来源：http://dsw.sysykeji.top

Py:   list(range(0, 10, 2))
来源：http://xod.vqdsnc.cn

PHP:  range(0, 10, 2);
来源：http://wxg.jqgufenzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tcx.dianchejie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dcz.tianlin.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yjx.c1oappe.top


<!-- 参考信息 -->