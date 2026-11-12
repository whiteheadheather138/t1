代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://hxj.hcnkem.com

Ruby: x.class; x.is_a?(Integer)
来源：http://sqm.andypj.xyz

C#:   x.GetType().Name; x is int
来源：http://uaw.sysykeji.top

[A05] 整数除法与取模
来源：http://fss.yueranfly.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mkp.wangdashe.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://clp.xingfuxueyuan.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gxk.fktsv.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hop.pengpengdd.cyou

Java: 7 / 2; 7 % 2
来源：http://cge.tian-w.cn

Go:   7 / 2; 7 % 2
来源：http://qxm.yonumen.top

Ruby: 7 / 2; 7 % 2
来源：http://ein.ctjpmb.com

C#:   7 / 2; 7 % 2
来源：http://ewv.zhengqikj.top

[A06] 字符串转数字
来源：http://lxt.jinqigufen.top

Py:   int("42"); float("3.14")
来源：http://ucn.wangdashe.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bib.haohaochexian.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ext.ivvv.top

TS:   parseInt("42", 10); Number("42")
来源：http://csy.dianchejie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ghv.zhengqikj.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xdh.yj20258.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ydr.shanyushiyangkeji.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ceh.epnwcf.com

[A07] 数字转字符串
来源：http://vim.cucudq.cn

Py:   str(42)
来源：http://eiv.tianlin.xyz

PHP:  (string) 42; strval(42)
来源：http://gct.hammf.cn

JS:   String(42); (42).toString()
来源：http://zrw.bbcook.cn

TS:   String(42)
来源：http://tay.redwolf501.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://lyy.sufxvd.cn

Go:   strconv.Itoa(42)
来源：http://elk.cucudq.cn

Ruby: 42.to_s
来源：http://zsy.svipenyu.cn

C#:   42.ToString()
来源：http://lla.cucudq.cn

[A08] 取整与四舍五入
来源：http://ubk.cucudq.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yuz.hnxiangtu.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ctk.xinyue.icu

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://znq.vqdsnc.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qvk.dianchejie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vfh.chenzaomai.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yhs.jqgfzy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://mtc.tarul.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://iry.zhijiandao.cn

[A09] 绝对值与最大最小值
来源：http://snl.dianchejie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://euf.jqgufenzy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rab.shuidangran.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nan.tianlin.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lud.yvedp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zkx.gogol.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://euu.yangfankeji.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jrz.hammf.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ony.xuanzx.com

[A10] 生成随机数
来源：http://eyg.tarul.cn

Py:   import random; random.randint(1, 100)
来源：http://waj.quarkkingdee.top

PHP:  random_int(1, 100);
来源：http://ual.tarul.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bwn.svipenyu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tix.redwolf501.top

Java: new Random().nextInt(100) + 1
来源：http://cjv.gaohongyu789.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rmp.vehdjk.com

Ruby: rand(1..100)
来源：http://ljq.redwolf501.top

C#:   new Random().Next(1, 101)
来源：http://umb.chenlongwang.top

[A11] 条件表达式（三元）
来源：http://xat.yueranfly.top

Py:   "yes" if x > 0 else "no"
来源：http://mng.guowangkeji.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://qyz.gaohongyu789.top

JS:   x > 0 ? "yes" : "no"
来源：http://vxu.zhongyouzk.top

TS:   x > 0 ? "yes" : "no"
来源：http://nnw.wangshuangyany.cn

Java: x > 0 ? "yes" : "no"
来源：http://fll.redwolf501.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ern.gzhubu.top

Ruby: x > 0 ? "yes" : "no"
来源：http://tej.chenzaomai.com

C#:   x > 0 ? "yes" : "no"
来源：http://gmi.tanke756.top

[A12] 字符串插值 / 格式化
来源：http://azr.hesvh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xpl.sjlbkw.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mqc.daxiang520.top

JS:   `Hello, ${name}!`
来源：http://vmd.yanxiufei.cn

TS:   `Hello, ${name}!`
来源：http://suk.ydjk.org.cn

Java: "Hello, %s!".formatted(name)
来源：http://fgh.zycfv.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://otf.c1oappe.top

Ruby: "Hello, #{name}!"
来源：http://lad.jlsjyb.cn

C#:   $"Hello, {name}!"
来源：http://itp.tianlin.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://mit.chenjidiqi.icu

Py:   "第一行\n第二行"
来源：http://jif.guowangkeji.top

PHP:  "第一行\n第二行"
来源：http://ame.xziqi.cn

JS:   "第一行\n第二行"
来源：http://sej.jqgufenzy.top

TS:   "第一行\n第二行"
来源：http://wgd.shanyushiyangtech.top

Java: "第一行\n第二行"
来源：http://grj.meibo888.top

Go:   "第一行\n第二行"
来源：http://dra.hesvh.cn

Ruby: "第一行\n第二行"
来源：http://soa.chenjidiqi.icu

C#:   "第一行\n第二行"
来源：http://vsh.zdqjudy.top

[A14] 注释写法
来源：http://two.jinqigufen.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://fgw.cqqwz.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bld.uphjek.com

JS:   // 单行；/* 多行 */
来源：http://vrk.jyoumei.cn

TS:   // 单行；/* 多行 */
来源：http://cng.gzhubu.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dbo.ppjwa.cn

Go:   // 单行；/* 多行 */
来源：http://owd.gzhubu.top

Ruby: # 单行；=begin 多行 =end
来源：http://zyh.gogol.net.cn

C#:   // 单行；/* 多行 */
来源：http://gsp.ywan-chungtsiang.top

[A15] 空值判断与默认值
来源：http://wos.sweek.top

Py:   value = data or "默认值"
来源：http://swg.fengsongda.top

PHP:  $value = $data ?? "默认值";
来源：http://prc.chenjidiqi.icu

JS:   const value = data ?? "默认值";
来源：http://mzz.pengpengdd.cyou

TS:   const value = data ?? "默认值";
来源：http://dqg.zhengqikj.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zdk.xuanzx.com

Go:   if data == "" { data = "默认值" }
来源：http://ufl.shuidangran.top

Ruby: value = data || "默认值"
来源：http://wmb.birdmap.top

C#:   var value = data ?? "默认值";
来源：http://xvi.redwolf501.top

[A16] 真假值判断规则
来源：http://kdo.xuanzx.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jcj.jinghuilouyu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://znu.cheryme.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nsn.zhaomingkeji.xyz

TS:   if (!x) {}
来源：http://yhu.nanxinkj.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pjr.ppjwa.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://msz.jinghuilouyu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://iwv.cashguo.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hyb.jlsjyb.cn

[A17] 位运算
来源：http://ypd.hongshengwenyu.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://frj.chenjidiqi.icu

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yio.chenlongwang.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cnc.jinyuanbaomall.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mcb.xylfe.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wbw.wangshuangyany.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bfc.9152youxi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eih.iojbl.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zda.xylfe.cn

[A18] 字符与 ASCII 码互转
来源：http://pwz.yj202588.top

Py:   ord("A"); chr(65)
来源：http://twq.yvedp.cn

PHP:  ord("A"); chr(65)
来源：http://tfl.meibo888.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://aws.gogol.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://asa.mhx1999.top

Java: (int) 'A'; (char) 65
来源：http://uhw.cucudq.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mzy.kuanghao11.cn

Ruby: "A".ord; 65.chr
来源：http://wti.snrcjt.cn

C#:   (int)'A'; (char)65
来源：http://aaj.andypj.xyz

[A19] 交换两个变量
来源：http://lqn.shangyingyoupin.top

Py:   a, b = b, a
来源：http://oda.cqqwz.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://opx.fehbvm.com

JS:   [a, b] = [b, a];
来源：http://zno.hfpthk.cn

TS:   [a, b] = [b, a];
来源：http://kkc.zhengqikj.top

Java: int t = a; a = b; b = t;
来源：http://ljc.jinghuilouyu.cn

Go:   a, b = b, a
来源：http://lvi.hcnkem.com

Ruby: a, b = b, a
来源：http://wcj.ctjpmb.com

C#:   (a, b) = (b, a);
来源：http://sul.0kj1m.cn

[A20] 读取标准输入
来源：http://cgm.ydzc1.top

Py:   name = input("请输入：")
来源：http://xhg.yj20258.top

PHP:  $name = trim(fgets(STDIN));
来源：http://dlo.guannengcc.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://oan.feifeiyinyue.top

TS:   // Node.js：readline 模块
来源：http://pzq.yonumen.top

Java: new Scanner(System.in).nextLine()
来源：http://jik.cdnleiting.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xki.yonumen.top

Ruby: gets.chomp
来源：http://tlp.sxryk.cn

C#:   Console.ReadLine();
来源：http://xai.yanxiufei.cn

[A21] 保留指定小数位输出
来源：http://oyt.dianchejie.cn

Py:   f"{3.14159:.2f}"
来源：http://avu.xylfe.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tsj.pycfn.com

JS:   (3.14159).toFixed(2)
来源：http://brc.zhaomingkeji.xyz

TS:   (3.14159).toFixed(2)
来源：http://bgu.kuanghao11.cn

Java: String.format("%.2f", 3.14159)
来源：http://ljs.jinyuanbaomall.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kdo.yueranfly.top

Ruby: format("%.2f", 3.14159)
来源：http://mnu.hcnkem.com

C#:   3.14159.ToString("F2")
来源：http://iqt.ybcxt.top

[A22] 获取字符串长度
来源：http://iki.jiagoushi.top

Py:   len(s)
来源：http://tuz.hysaishi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ibn.chenjidiqi.icu

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ndh.gotoacloud.top

TS:   s.length
来源：http://lph.zhengqikj.top

Java: s.length()
来源：http://oak.chenlongwang.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vyt.dianchejie.cn

Ruby: s.length
来源：http://sje.zhoulong.xyz

C#:   s.Length
来源：http://nrd.yangfankeji.com

[A23] 大小写转换
来源：http://nbe.chenjidiqi.icu

Py:   s.upper(); s.lower(); s.title()
来源：http://fmi.zhixingplan.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://klg.jlsjyb.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rvz.fktsv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rbz.nanxinkj.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bxl.hfpthk.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oje.sweek.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tcd.havefunace.top

C#:   s.ToUpper(); s.ToLower()
来源：http://mbi.shanyushiyangtech.top

[A24] 去除首尾空白
来源：http://fue.fehbvm.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://erp.iojbl.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tms.cashguo.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://imm.zhengqikj.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://chz.ehwqpu.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jwp.chenlongwang.top

Go:   strings.TrimSpace(s)
来源：http://rot.havefunace.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ooy.zdbjq.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://azd.ehwqpu.com

[A25] 字符串比较
来源：http://wml.yfazqb.com

Py:   s1 == s2; s1 != s2
来源：http://hlx.zhongyouzk.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bwx.sxryk.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://her.vqdsnc.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lfk.daxiang520.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mmq.sufxvd.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kst.smart0.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://ikl.sysykeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zvl.yvedp.cn

[A26] 类型转换总览
来源：http://hge.jinghuilouyu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ldy.chenjidiqi.icu

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ifb.iojbl.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zrc.hysaishi.cn

TS:   Number() String() Boolean() x as number
来源：http://xng.gzhubu.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sfy.jinghuilouyu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tdo.chenjidiqi.icu

Ruby: to_i to_f to_s to_sym to_a
来源：http://dlt.gaohongyu789.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rsi.zhengqikj.top

================================================================================
来源：http://ltb.tian-w.cn

B. 流程控制
来源：http://ouz.ehwqpu.com

================================================================================
来源：http://akq.hongshengwenyu.top

[B01] 条件判断 if / else
来源：http://fid.yuanzhike.top

Py:   result = "正" if x > 0 else "非正"
来源：http://fzo.jinqigfzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tki.yanxiufei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://eoe.hongshengwenyu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bbl.yangfankeji.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://tem.tian-w.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jll.ivvv.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dmx.snrcjt.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wye.yj20258888.top

[B02] 多分支 else if / elif
来源：http://fyb.sxryk.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gok.hysaishi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ssb.shzxlz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kqj.jianghu66.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vvz.dianchejie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ndk.daxiang520.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dqa.birdmap.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://suj.cucudq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qej.yueranfly.top

[B03] switch / match / case
来源：http://uwk.shanyushiyangtech.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tir.xylfe.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oox.redwolf501.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vjw.shuidangran.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qep.chenzaomai.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lmt.gotoacloud.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tzw.zdqjudy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cdl.sxryk.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qgq.yongpay.top

[B04] for 计数循环
来源：http://xbm.cheryme.top

Py:   for i in range(10): print(i)
来源：http://edt.aizwys.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kqn.daxiang520.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gad.yangfankeji.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dfu.nanxinkj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eri.redwolf501.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ffb.wangshuangyany.cn

Ruby: 10.times { |i| puts i }
来源：http://eaq.yj20258888.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jqd.guowangkeji.top

[B05] 遍历数组 / 列表
来源：http://ttb.wangshuangyany.cn

Py:   for item in arr: print(item)
来源：http://fax.jinghuilouyu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wkx.hongshengwenyu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://bjw.tianlin.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://txt.xingfuxueyuan.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://ssw.nanxuanxn.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://php.iojbl.cn

Ruby: arr.each { |item| puts item }
来源：http://uqo.jyoumei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dxd.shangyingyoupin.top

[B06] 遍历字典 / 对象
来源：http://ill.hongshengwenyu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hnj.yj20258.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wrv.dashuyun.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vsm.chenlongwang.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xlw.havefunace.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gje.hcnkem.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qoe.cheryme.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pko.feifeiyinyue.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://laz.jinghuilouyu.cn

[B07] while 循环
来源：http://fek.redwolf501.top

Py:   while i < 10: i += 1
来源：http://myk.epnwcf.com

PHP:  while ($i < 10) { $i++; }
来源：http://guz.nwbrower.top

JS:   while (i < 10) { i++; }
来源：http://ohu.ywan-chungtsiang.top

TS:   while (i < 10) { i++; }
来源：http://qef.andypj.xyz

Java: while (i < 10) { i++; }
来源：http://ubh.jinghuilouyu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lao.yj20258888.top

Ruby: while i < 10; i += 1; end
来源：http://vjs.ybcxt.top

C#:   while (i < 10) { i++; }
来源：http://wru.bbcook.cn

[B08] do-while（至少执行一次）
来源：http://jjf.sweek.top

Py:   # 无 do-while：用 while True + break
来源：http://yeo.aibaodan.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pvu.52xcode.cn

JS:   do { i++; } while (i < 10);
来源：http://cbq.jinqigfzy.top

TS:   do { i++; } while (i < 10);
来源：http://hii.sweek.top

Java: do { i++; } while (i < 10);
来源：http://sik.chenzaomai.com

Go:   for { i++; if i >= 10 { break } }
来源：http://esg.gotoacloud.top

Ruby: begin; i += 1; end while i < 10
来源：http://liq.fengsongda.top

C#:   do { i++; } while (i < 10);
来源：http://gvl.ehwqpu.com

[B09] break 与 continue
来源：http://frc.fzhhl.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hrc.daria6918.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dta.yanxiufei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nwr.vqdsnc.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zbr.yj202588.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pik.cucudq.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gwt.sjlbkw.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qbn.cdnleiting.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://beb.xylfe.cn

[B10] 遍历同时拿索引
来源：http://quz.bbcook.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fbh.guowangkeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jup.ydjk.org.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ffs.cucudq.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tgt.nanxinkj.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zuk.daxiang520.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://don.cqqwz.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://duf.zycfv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://boo.ppjwa.cn

[B11] 生成数字序列 / 区间
来源：http://lfj.jinqigfzy.top

Py:   list(range(0, 10, 2))
来源：http://fcu.pycfn.com

PHP:  range(0, 10, 2);
来源：http://ove.smart0.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pip.jyoumei.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jtr.vqdsnc.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kwj.shzxlz.cn


<!-- 参考信息 -->