代发 wailian999

JS:   String(42); (42).toString()
来源：http://mva.xuanzx.com

TS:   String(42)
来源：http://xoe.guannengcc.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://acf.zhiwuduotai.top

Go:   strconv.Itoa(42)
来源：http://drq.svipenyu.cn

Ruby: 42.to_s
来源：http://emr.sjlbkw.cn

C#:   42.ToString()
来源：http://hkh.nanxinkj.top

[A08] 取整与四舍五入
来源：http://cgf.yvedp.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pts.hfpthk.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xfa.epnwcf.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://icb.gzhubu.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://osp.pycfn.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cls.yanxiufei.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wei.gotoacloud.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://csv.wangshuangyany.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dji.zycfv.cn

[A09] 绝对值与最大最小值
来源：http://suq.daria6918.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://imm.meibo888.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://taf.wangshuangyany.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bel.jiagoushi.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://myx.pengpengdd.cyou

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nif.52xcode.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wdu.aibaodan.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://eqj.jqgfzy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vpp.mhx1999.top

[A10] 生成随机数
来源：http://bmx.zhixingplan.top

Py:   import random; random.randint(1, 100)
来源：http://ele.cdnleiting.top

PHP:  random_int(1, 100);
来源：http://swi.9152youxi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://efe.zhengqikj.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://aqx.xinyue.icu

Java: new Random().nextInt(100) + 1
来源：http://mse.meibo888.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wvh.pengpengdd.cyou

Ruby: rand(1..100)
来源：http://nkz.jinqigfzy.top

C#:   new Random().Next(1, 101)
来源：http://qst.bbcook.cn

[A11] 条件表达式（三元）
来源：http://tpj.xziqi.cn

Py:   "yes" if x > 0 else "no"
来源：http://agp.vqdsnc.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fiz.fengsongda.top

JS:   x > 0 ? "yes" : "no"
来源：http://jww.chenjidiqi.icu

TS:   x > 0 ? "yes" : "no"
来源：http://vrk.uphjek.com

Java: x > 0 ? "yes" : "no"
来源：http://odi.gaohongyu789.top

Go:   // 无三元运算符，需用 if 语句
来源：http://hnl.zdqjudy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://hqm.yj20258.top

C#:   x > 0 ? "yes" : "no"
来源：http://rfr.kuanghao11.cn

[A12] 字符串插值 / 格式化
来源：http://kwj.epnwcf.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zji.bbcook.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rap.nwbrower.top

JS:   `Hello, ${name}!`
来源：http://sxn.shanyushiyangkeji.top

TS:   `Hello, ${name}!`
来源：http://bcl.jqgufenzy.top

Java: "Hello, %s!".formatted(name)
来源：http://acm.xinyue.icu

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xfu.yvedp.cn

Ruby: "Hello, #{name}!"
来源：http://fee.zdbjq.cn

C#:   $"Hello, {name}!"
来源：http://hmd.zhiwuduotai.top

[A13] 多行字符串（练习 \n 转义）
来源：http://hzc.nanxinkj.top

Py:   "第一行\n第二行"
来源：http://mhk.chenzaomai.com

PHP:  "第一行\n第二行"
来源：http://imf.zhoulong.xyz

JS:   "第一行\n第二行"
来源：http://wkj.vehdjk.com

TS:   "第一行\n第二行"
来源：http://atd.jiagoushi.top

Java: "第一行\n第二行"
来源：http://omr.chenlongwang.top

Go:   "第一行\n第二行"
来源：http://fmq.yangfankeji.com

Ruby: "第一行\n第二行"
来源：http://adc.havefunace.top

C#:   "第一行\n第二行"
来源：http://jqa.ywan-chungtsiang.top

[A14] 注释写法
来源：http://gwi.zhongyouzk.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://wmv.yanxiufei.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xug.cashguo.top

JS:   // 单行；/* 多行 */
来源：http://zgk.pengpengdd.cyou

TS:   // 单行；/* 多行 */
来源：http://vly.ydjk.org.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bgi.nanxuanxn.top

Go:   // 单行；/* 多行 */
来源：http://hig.feifeiyinyue.top

Ruby: # 单行；=begin 多行 =end
来源：http://hfl.snrcjt.cn

C#:   // 单行；/* 多行 */
来源：http://gna.havefunace.top

[A15] 空值判断与默认值
来源：http://fxl.smart0.xyz

Py:   value = data or "默认值"
来源：http://uqb.jlsjyb.cn

PHP:  $value = $data ?? "默认值";
来源：http://syg.jiagoushi.top

JS:   const value = data ?? "默认值";
来源：http://uek.tianlin.xyz

TS:   const value = data ?? "默认值";
来源：http://cdi.xuanzx.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zte.yuxming.cn

Go:   if data == "" { data = "默认值" }
来源：http://aoj.quarkkingdee.top

Ruby: value = data || "默认值"
来源：http://ryi.pengpengdd.cyou

C#:   var value = data ?? "默认值";
来源：http://llb.yfazqb.com

[A16] 真假值判断规则
来源：http://rct.ivvv.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rpn.ppjwa.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vbx.xziqi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tkv.andypj.xyz

TS:   if (!x) {}
来源：http://bag.redwolf501.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xrw.ydzc1.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dmv.cashguo.top

Ruby: unless x            # nil 与 false 为假
来源：http://czk.mhx1999.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ulf.9152youxi.cn

[A17] 位运算
来源：http://kia.yuanzhike.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nly.gogol.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fwt.gzhubu.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wnl.zycfv.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uqc.bbcook.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bpz.yongpay.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zio.yanxiufei.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rnx.epnwcf.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aok.0kj1m.cn

[A18] 字符与 ASCII 码互转
来源：http://kkb.birdmap.top

Py:   ord("A"); chr(65)
来源：http://jno.andypj.xyz

PHP:  ord("A"); chr(65)
来源：http://stf.ydzc1.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fpc.shangyingyoupin.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sdf.jianghu66.top

Java: (int) 'A'; (char) 65
来源：http://rxq.yvedp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uor.yvedp.cn

Ruby: "A".ord; 65.chr
来源：http://sef.0kj1m.cn

C#:   (int)'A'; (char)65
来源：http://pca.guowangkeji.top

[A19] 交换两个变量
来源：http://mbn.hywenlv.cn

Py:   a, b = b, a
来源：http://tcl.cucudq.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hxo.zhongyouzk.top

JS:   [a, b] = [b, a];
来源：http://uzn.pycfn.com

TS:   [a, b] = [b, a];
来源：http://rce.shangyingyoupin.top

Java: int t = a; a = b; b = t;
来源：http://tup.zdbjq.cn

Go:   a, b = b, a
来源：http://ncd.redwolf501.top

Ruby: a, b = b, a
来源：http://vao.zhoulong.xyz

C#:   (a, b) = (b, a);
来源：http://xsy.vqdsnc.cn

[A20] 读取标准输入
来源：http://jnv.shanyushiyangkeji.top

Py:   name = input("请输入：")
来源：http://akk.yj20258.top

PHP:  $name = trim(fgets(STDIN));
来源：http://bss.gogol.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://faa.yuanzhike.top

TS:   // Node.js：readline 模块
来源：http://heh.yongpay.top

Java: new Scanner(System.in).nextLine()
来源：http://cfc.ctjpmb.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rkx.zhaomingkeji.xyz

Ruby: gets.chomp
来源：http://daj.zhoulong.xyz

C#:   Console.ReadLine();
来源：http://ubh.vehdjk.com

[A21] 保留指定小数位输出
来源：http://wwq.shzxlz.cn

Py:   f"{3.14159:.2f}"
来源：http://kit.yvedp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ffn.birdmap.top

JS:   (3.14159).toFixed(2)
来源：http://bfy.zhaomingkeji.xyz

TS:   (3.14159).toFixed(2)
来源：http://kav.cqqwz.cn

Java: String.format("%.2f", 3.14159)
来源：http://hsn.vqdsnc.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tzo.dashuyun.cn

Ruby: format("%.2f", 3.14159)
来源：http://ykg.pengpengdd.cyou

C#:   3.14159.ToString("F2")
来源：http://djf.jinghuilouyu.cn

[A22] 获取字符串长度
来源：http://llj.yuanzhike.top

Py:   len(s)
来源：http://uwp.zhengqikj.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tgh.jinqigfzy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kxs.yonumen.top

TS:   s.length
来源：http://jia.birdmap.top

Java: s.length()
来源：http://gzj.andypj.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xvq.xinyue.icu

Ruby: s.length
来源：http://tdp.dianchejie.cn

C#:   s.Length
来源：http://qii.tian-w.cn

[A23] 大小写转换
来源：http://wev.ppjwa.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ehu.wangdashe.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yuc.pengpengdd.cyou

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zwl.chenjidiqi.icu

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fcp.zhiwuduotai.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xkl.gaohongyu789.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pqu.ehwqpu.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wyb.iojbl.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://juj.zhengqikj.top

[A24] 去除首尾空白
来源：http://cuw.jlsjyb.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yvj.yuxming.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tcc.yj20258.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pgc.ybcxt.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wat.meibo888.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lcp.0kj1m.cn

Go:   strings.TrimSpace(s)
来源：http://kbk.sweek.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uhc.dashuyun.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vjf.dianchejie.cn

[A25] 字符串比较
来源：http://ghv.hongshengwenyu.top

Py:   s1 == s2; s1 != s2
来源：http://hij.jiagoushi.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vsn.yanxiufei.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gbu.zdbjq.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://amx.cashguo.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://alq.bjfxy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hfm.ivvv.top

Ruby: s1 == s2; s1 <=> s2
来源：http://kcu.jinqigufen.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://txx.tarul.cn

[A26] 类型转换总览
来源：http://dts.vehdjk.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tsv.jianghu66.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nyx.xuanzx.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wcw.snrcjt.cn

TS:   Number() String() Boolean() x as number
来源：http://szf.hnqzz.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hst.yongpay.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://eoo.yongpay.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ori.jinqigufen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ksn.tarul.cn

================================================================================
来源：http://hjj.cucudq.cn

B. 流程控制
来源：http://aqx.cdnleiting.top

================================================================================
来源：http://gum.uphjek.com

[B01] 条件判断 if / else
来源：http://acf.zhixingplan.top

Py:   result = "正" if x > 0 else "非正"
来源：http://yve.mhx1999.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gis.quarkkingdee.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hkm.zhaomingkeji.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vgf.aibaodan.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lyi.jqgfzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pvw.jlsjyb.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://iyq.smart0.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://eub.aibaodan.cn

[B02] 多分支 else if / elif
来源：http://xkm.sufxvd.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dfx.xziqi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bxr.fzhhl.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hbf.hysaishi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pts.cucudq.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qwu.xylfe.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uav.gaohongyu789.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zbn.gaohongyu789.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ywd.pycfn.com

[B03] switch / match / case
来源：http://ocy.wangshuangyany.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vmf.gogol.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sdu.hywenlv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uuu.uphjek.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://top.sweek.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bbj.xylfe.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rya.dashuyun.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rqb.yueranfly.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mpa.gotoacloud.top

[B04] for 计数循环
来源：http://ezq.aibaodan.cn

Py:   for i in range(10): print(i)
来源：http://iss.gzhubu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dcz.zhaomingkeji.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jhj.ctjpmb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mgn.aibaodan.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aza.mhx1999.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tlt.hfpthk.cn

Ruby: 10.times { |i| puts i }
来源：http://tty.xuetiantiany.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hqk.xingfuxueyuan.xyz

[B05] 遍历数组 / 列表
来源：http://wnm.dianchejie.cn

Py:   for item in arr: print(item)
来源：http://sro.mhx1999.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rff.guannengcc.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vtf.shuidangran.top

TS:   for (const item of arr) { console.log(item); }
来源：http://asn.gogol.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://emp.hesvh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bps.iojbl.cn

Ruby: arr.each { |item| puts item }
来源：http://ssn.9152youxi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sej.tianlin.xyz

[B06] 遍历字典 / 对象
来源：http://vti.chenlongwang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://lpb.ywan-chungtsiang.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gcf.sufxvd.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ksz.aibaodan.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lvl.fengsongda.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rwg.ybcxt.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uwf.xziqi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tsd.ywan-chungtsiang.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fwp.birdmap.top

[B07] while 循环
来源：http://plv.shuidangran.top

Py:   while i < 10: i += 1
来源：http://ofw.52xcode.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ixn.hfpthk.cn

JS:   while (i < 10) { i++; }
来源：http://rdn.yj202588.top

TS:   while (i < 10) { i++; }
来源：http://gig.guowangkeji.top

Java: while (i < 10) { i++; }
来源：http://kbd.xinyue.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lrq.jinghuilouyu.cn

Ruby: while i < 10; i += 1; end
来源：http://yov.zdbjq.cn

C#:   while (i < 10) { i++; }
来源：http://ujj.bbcook.cn

[B08] do-while（至少执行一次）
来源：http://pxu.cheryme.top

Py:   # 无 do-while：用 while True + break
来源：http://dwn.dashuyun.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hfz.hongshengwenyu.top

JS:   do { i++; } while (i < 10);
来源：http://cnj.ehwqpu.com

TS:   do { i++; } while (i < 10);
来源：http://rel.aibaodan.cn

Java: do { i++; } while (i < 10);
来源：http://bzi.haohaochexian.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nla.feifeiyinyue.top

Ruby: begin; i += 1; end while i < 10
来源：http://wfc.zhongyouzk.top

C#:   do { i++; } while (i < 10);
来源：http://tct.dianchejie.cn

[B09] break 与 continue
来源：http://rhf.gogol.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hdm.jinqigufen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://whz.jinghuilouyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xfq.jinqigfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qxa.yj20258.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qch.hesvh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yfp.fehbvm.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tig.yj202588.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://apd.sysykeji.top

[B10] 遍历同时拿索引
来源：http://err.bjfxy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nkv.hywenlv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lxo.fktsv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ddm.chenlongwang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://det.aibaodan.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kfl.sjlbkw.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ckg.epnwcf.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xsl.jqgufenzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wtt.jinyuanbaomall.cn

[B11] 生成数字序列 / 区间
来源：http://usj.bbcook.cn

Py:   list(range(0, 10, 2))
来源：http://bfb.guannengcc.top

PHP:  range(0, 10, 2);
来源：http://qrz.yonumen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://reb.andypj.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jqk.xuanzx.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ugd.sjlbkw.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ppu.daxiang520.top

Ruby: (0...10).step(2).to_a
来源：http://haf.jianghu66.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fkn.mhx1999.top

[B12] 跳出多层循环
来源：http://kmw.feifeiyinyue.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://pna.guannengcc.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://jik.nanxinkj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://syh.smart0.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gcz.aizwys.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cco.ctjpmb.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://auv.shanyushiyangtech.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wuu.quarkkingdee.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://btk.ydjk.org.cn

[B13] 判断是否为数字
来源：http://ymh.ydzc1.top

Py:   isinstance(x, (int, float))
来源：http://oop.jqgfzy.top

PHP:  is_numeric($x)
来源：http://gkk.gotoacloud.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yea.shuidangran.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tuj.zhongyouzk.top

Java: x instanceof Number
来源：http://etk.shanyushiyangtech.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lgf.ivvv.top

Ruby: x.is_a?(Numeric)
来源：http://nuy.chenjidiqi.icu

C#:   x is int or double or decimal
来源：http://rjl.zhoulong.xyz

[B14] 判断值是否在集合内
来源：http://kvy.feifeiyinyue.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ghd.fehbvm.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://khs.zhixingplan.top


<!-- 参考信息 -->