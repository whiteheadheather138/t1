代发 wailian999

JS:   String(42); (42).toString()
来源：http://iep.fehbvm.com

TS:   String(42)
来源：http://xtt.svipenyu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://kqg.xuetiantiany.cn

Go:   strconv.Itoa(42)
来源：http://zxh.kuanghao11.cn

Ruby: 42.to_s
来源：http://lmx.svipenyu.cn

C#:   42.ToString()
来源：http://kwc.fanxiaobao.xyz

[A08] 取整与四舍五入
来源：http://jfl.xylfe.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zcr.yj202588.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pjw.meibo888.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pyo.cqqwz.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://oec.nanxuanxn.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nxw.ctjpmb.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ixw.hysaishi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sbq.quarkkingdee.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dxw.vqdsnc.cn

[A09] 绝对值与最大最小值
来源：http://pfw.snrcjt.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xcy.tanke756.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tgq.vqdsnc.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pyo.52xcode.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dxf.vehdjk.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mec.yfazqb.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://uvw.xylfe.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hqn.jianghu66.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rff.uphjek.com

[A10] 生成随机数
来源：http://aqi.xylfe.cn

Py:   import random; random.randint(1, 100)
来源：http://qeq.c1oappe.top

PHP:  random_int(1, 100);
来源：http://luc.xylfe.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://aoz.zhaomingkeji.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bzr.cdnleiting.top

Java: new Random().nextInt(100) + 1
来源：http://laq.svipenyu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qke.chenzaomai.com

Ruby: rand(1..100)
来源：http://dae.pycfn.com

C#:   new Random().Next(1, 101)
来源：http://xko.chenzaomai.com

[A11] 条件表达式（三元）
来源：http://rzn.yueranfly.top

Py:   "yes" if x > 0 else "no"
来源：http://mlb.cashguo.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://kkj.dianchejie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xve.feifeiyinyue.top

TS:   x > 0 ? "yes" : "no"
来源：http://vfj.birdmap.top

Java: x > 0 ? "yes" : "no"
来源：http://fyt.zhoulong.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://qhu.zhongyouzk.top

Ruby: x > 0 ? "yes" : "no"
来源：http://fwk.hongshengwenyu.top

C#:   x > 0 ? "yes" : "no"
来源：http://rwd.zhixingplan.top

[A12] 字符串插值 / 格式化
来源：http://pwn.hnxiangtu.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xva.fengsongda.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gap.svipenyu.cn

JS:   `Hello, ${name}!`
来源：http://hkb.uphjek.com

TS:   `Hello, ${name}!`
来源：http://bgr.redwolf501.top

Java: "Hello, %s!".formatted(name)
来源：http://htp.gogol.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rcy.aizwys.cn

Ruby: "Hello, #{name}!"
来源：http://umn.svipenyu.cn

C#:   $"Hello, {name}!"
来源：http://qjc.316326.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://gwl.gaohongyu789.top

Py:   "第一行\n第二行"
来源：http://rmc.pycfn.com

PHP:  "第一行\n第二行"
来源：http://fbe.jqgfzy.top

JS:   "第一行\n第二行"
来源：http://zqd.zhixingplan.top

TS:   "第一行\n第二行"
来源：http://nyf.cashguo.top

Java: "第一行\n第二行"
来源：http://xor.yangfankeji.com

Go:   "第一行\n第二行"
来源：http://exe.sxryk.cn

Ruby: "第一行\n第二行"
来源：http://gmp.snrcjt.cn

C#:   "第一行\n第二行"
来源：http://qyc.gzhubu.top

[A14] 注释写法
来源：http://ucm.dianchejie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://oah.epnwcf.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://wrn.cqqwz.cn

JS:   // 单行；/* 多行 */
来源：http://frl.hnxiangtu.top

TS:   // 单行；/* 多行 */
来源：http://vyw.jinqigufen.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dus.ivvv.top

Go:   // 单行；/* 多行 */
来源：http://hva.redwolf501.top

Ruby: # 单行；=begin 多行 =end
来源：http://ofz.vqdsnc.cn

C#:   // 单行；/* 多行 */
来源：http://rsd.zhiwuduotai.top

[A15] 空值判断与默认值
来源：http://iqp.yj20258888.top

Py:   value = data or "默认值"
来源：http://ikk.tanke756.top

PHP:  $value = $data ?? "默认值";
来源：http://gti.ctjpmb.com

JS:   const value = data ?? "默认值";
来源：http://eda.xinyue.icu

TS:   const value = data ?? "默认值";
来源：http://fdf.ybcxt.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cyc.yueranfly.top

Go:   if data == "" { data = "默认值" }
来源：http://ypt.hnqzz.top

Ruby: value = data || "默认值"
来源：http://nea.c1oappe.top

C#:   var value = data ?? "默认值";
来源：http://bbg.sxryk.cn

[A16] 真假值判断规则
来源：http://arl.yangfankeji.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xqx.vqdsnc.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://svq.pengpengdd.cyou

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mbw.havefunace.top

TS:   if (!x) {}
来源：http://dvo.havefunace.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gqi.hnxiangtu.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lts.epnwcf.com

Ruby: unless x            # nil 与 false 为假
来源：http://kua.xuetiantiany.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ibx.daxiang520.top

[A17] 位运算
来源：http://nmy.zhongyouzk.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tva.hywenlv.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ost.yanxiufei.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kau.jqgfzy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://anj.ctjpmb.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eln.aibaodan.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dum.kuanghao11.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kxr.haohaochexian.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aio.birdmap.top

[A18] 字符与 ASCII 码互转
来源：http://puo.cucudq.cn

Py:   ord("A"); chr(65)
来源：http://wme.shanyushiyangtech.top

PHP:  ord("A"); chr(65)
来源：http://ifn.havefunace.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qid.wangshuangyany.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nfr.jqgufenzy.top

Java: (int) 'A'; (char) 65
来源：http://rxp.sufxvd.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://clq.c1oappe.top

Ruby: "A".ord; 65.chr
来源：http://ses.zhongyouzk.top

C#:   (int)'A'; (char)65
来源：http://ybl.svipenyu.cn

[A19] 交换两个变量
来源：http://grl.nanxuanxn.top

Py:   a, b = b, a
来源：http://kvl.zhongyouzk.top

PHP:  [$a, $b] = [$b, $a];
来源：http://qcg.xziqi.cn

JS:   [a, b] = [b, a];
来源：http://nmi.cdnleiting.top

TS:   [a, b] = [b, a];
来源：http://kdm.yfazqb.com

Java: int t = a; a = b; b = t;
来源：http://ofo.chenlongwang.top

Go:   a, b = b, a
来源：http://yus.ydzc1.top

Ruby: a, b = b, a
来源：http://gcn.zhaomingkeji.xyz

C#:   (a, b) = (b, a);
来源：http://kzv.jinqigfzy.top

[A20] 读取标准输入
来源：http://skb.shanyushiyangkeji.top

Py:   name = input("请输入：")
来源：http://djs.hnxiangtu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ldm.cashguo.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://czx.zhixingplan.top

TS:   // Node.js：readline 模块
来源：http://rja.guowangkeji.top

Java: new Scanner(System.in).nextLine()
来源：http://nyt.yvedp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hoc.yj202588.top

Ruby: gets.chomp
来源：http://pse.cheryme.top

C#:   Console.ReadLine();
来源：http://ast.kuanghao11.cn

[A21] 保留指定小数位输出
来源：http://cqi.havefunace.top

Py:   f"{3.14159:.2f}"
来源：http://grj.xylfe.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gch.nanxinkj.top

JS:   (3.14159).toFixed(2)
来源：http://bst.jyoumei.cn

TS:   (3.14159).toFixed(2)
来源：http://hwm.yfazqb.com

Java: String.format("%.2f", 3.14159)
来源：http://wqu.xziqi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ame.zhengqikj.top

Ruby: format("%.2f", 3.14159)
来源：http://wkk.shuidangran.top

C#:   3.14159.ToString("F2")
来源：http://kuw.sweek.top

[A22] 获取字符串长度
来源：http://zcu.zhengqikj.top

Py:   len(s)
来源：http://jsl.chenlongwang.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ele.xingfuxueyuan.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zgf.jqgfzy.top

TS:   s.length
来源：http://fyr.hysaishi.cn

Java: s.length()
来源：http://iee.gzhubu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hdy.zhaomingkeji.xyz

Ruby: s.length
来源：http://bhq.hesvh.cn

C#:   s.Length
来源：http://jsx.vqdsnc.cn

[A23] 大小写转换
来源：http://nfi.jlsjyb.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://utw.jinyuanbaomall.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jax.bbcook.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jhh.hysaishi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yxz.yj202588.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jky.yvedp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tuc.nanxuanxn.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nuw.iojbl.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rdi.uphjek.com

[A24] 去除首尾空白
来源：http://miv.sysykeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fpt.zhongyouzk.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ehp.bbcook.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bqe.shzxlz.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wur.dianchejie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://aar.xingfuxueyuan.xyz

Go:   strings.TrimSpace(s)
来源：http://ccr.xingfuxueyuan.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ytb.guowangkeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wqm.quarkkingdee.top

[A25] 字符串比较
来源：http://nbr.shuidangran.top

Py:   s1 == s2; s1 != s2
来源：http://gew.sufxvd.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fym.shzxlz.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gzh.c1oappe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nug.yfazqb.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mdn.tanke756.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xej.yueranfly.top

Ruby: s1 == s2; s1 <=> s2
来源：http://iuz.jinghuilouyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rcc.zhengqikj.top

[A26] 类型转换总览
来源：http://dfz.yangfankeji.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hlk.chenlongwang.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wnl.hesvh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://etp.iojbl.cn

TS:   Number() String() Boolean() x as number
来源：http://tsq.dianchejie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bjz.cqqwz.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://eos.hammf.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gsm.shuidangran.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uml.ehwqpu.com

================================================================================
来源：http://vrw.aibaodan.cn

B. 流程控制
来源：http://gdb.uphjek.com

================================================================================
来源：http://lvs.hfpthk.cn

[B01] 条件判断 if / else
来源：http://kin.iojbl.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://knc.fzhhl.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xen.ppjwa.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://upw.aibaodan.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wgj.zhixingplan.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://rii.cashguo.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uuk.jqgfzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://aht.fktsv.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qam.fengsongda.top

[B02] 多分支 else if / elif
来源：http://zbw.dianchejie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gwv.tanke756.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fvd.nanxuanxn.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zha.sxryk.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lwe.hammf.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fcp.jiagoushi.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zrv.birdmap.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gwv.feifeiyinyue.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uzs.xuetiantiany.cn

[B03] switch / match / case
来源：http://msp.gaohongyu789.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lfp.pengpengdd.cyou

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fvv.shangyingyoupin.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://efw.jqgfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rui.ctjpmb.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://stc.xinyue.icu

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dzo.tanke756.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sil.fzhhl.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nem.guowangkeji.top

[B04] for 计数循环
来源：http://jqg.ctjpmb.com

Py:   for i in range(10): print(i)
来源：http://ydo.daxiang520.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yol.jqgfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://crk.chenjidiqi.icu

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cyu.snrcjt.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ode.snrcjt.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dgy.sweek.top

Ruby: 10.times { |i| puts i }
来源：http://vol.epnwcf.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lzl.pengpengdd.cyou

[B05] 遍历数组 / 列表
来源：http://ang.tarul.cn

Py:   for item in arr: print(item)
来源：http://ang.mhx1999.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://isb.gaohongyu789.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vdi.pycfn.com

TS:   for (const item of arr) { console.log(item); }
来源：http://ljj.fktsv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qab.daria6918.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://njq.tanke756.top

Ruby: arr.each { |item| puts item }
来源：http://epb.jqgufenzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ene.bbcook.cn

[B06] 遍历字典 / 对象
来源：http://zdt.gogol.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mxy.yuxming.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nsi.ppjwa.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pnl.dashuyun.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rpn.chenlongwang.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jvv.chenzaomai.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://upe.tianlin.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hfn.ctjpmb.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ijz.yj20258888.top

[B07] while 循环
来源：http://cvv.52xcode.cn

Py:   while i < 10: i += 1
来源：http://fld.yvedp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tdi.tianlin.xyz

JS:   while (i < 10) { i++; }
来源：http://aip.jiagoushi.top

TS:   while (i < 10) { i++; }
来源：http://wkn.jiagoushi.top

Java: while (i < 10) { i++; }
来源：http://ybz.kuanghao11.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ibp.uphjek.com

Ruby: while i < 10; i += 1; end
来源：http://nns.zhijiandao.cn

C#:   while (i < 10) { i++; }
来源：http://puf.jqgfzy.top

[B08] do-while（至少执行一次）
来源：http://zkh.gotoacloud.top

Py:   # 无 do-while：用 while True + break
来源：http://rnp.fktsv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://iiv.vehdjk.com

JS:   do { i++; } while (i < 10);
来源：http://qyk.zdqjudy.top

TS:   do { i++; } while (i < 10);
来源：http://dea.nanxinkj.top

Java: do { i++; } while (i < 10);
来源：http://tgf.gogol.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://slc.sufxvd.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gsh.jianghu66.top

C#:   do { i++; } while (i < 10);
来源：http://tyr.yj202588.top

[B09] break 与 continue
来源：http://vte.fzhhl.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rzt.snrcjt.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vbj.yueranfly.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dzm.jqgufenzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dtw.smart0.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xob.sufxvd.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://smo.zdbjq.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://owe.uphjek.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wxw.hnqzz.top

[B10] 遍历同时拿索引
来源：http://riz.zdqjudy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ffr.yuxming.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zmp.fktsv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wkt.cdnleiting.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xic.zhijiandao.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://irs.9152youxi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cym.yuanzhike.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gzy.feifeiyinyue.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://avr.shzxlz.cn

[B11] 生成数字序列 / 区间
来源：http://jkc.sufxvd.cn

Py:   list(range(0, 10, 2))
来源：http://mcb.shzxlz.cn

PHP:  range(0, 10, 2);
来源：http://hkr.aizwys.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mrf.ppjwa.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kvs.yuxming.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yyf.jlsjyb.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fji.birdmap.top

Ruby: (0...10).step(2).to_a
来源：http://ide.sjlbkw.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kwa.havefunace.top

[B12] 跳出多层循环
来源：http://xng.guannengcc.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://svn.iojbl.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gvs.snrcjt.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ijb.xylfe.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qnn.hongshengwenyu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zzq.yongpay.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ifh.nanxuanxn.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cdi.sufxvd.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kdf.hesvh.cn

[B13] 判断是否为数字
来源：http://omj.yongpay.top

Py:   isinstance(x, (int, float))
来源：http://qrt.guannengcc.top

PHP:  is_numeric($x)
来源：http://iiw.ctjpmb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pex.gzhubu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oga.yj202588.top

Java: x instanceof Number
来源：http://bfg.yj20258888.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nnt.chenjidiqi.icu

Ruby: x.is_a?(Numeric)
来源：http://kjx.ywan-chungtsiang.top

C#:   x is int or double or decimal
来源：http://iju.uphjek.com

[B14] 判断值是否在集合内
来源：http://zae.316326.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jbx.hesvh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://teg.0kj1m.cn


<!-- 参考信息 -->