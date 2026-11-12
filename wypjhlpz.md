代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://kmg.zhaomingkeji.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://xys.yueranfly.top

C#:   x.GetType().Name; x is int
来源：http://kcb.jqgfzy.top

[A05] 整数除法与取模
来源：http://rsq.daxiang520.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tcr.zhiwuduotai.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://tlg.jianghu66.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://anz.hongshengwenyu.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cqr.ybcxt.top

Java: 7 / 2; 7 % 2
来源：http://pqp.hammf.cn

Go:   7 / 2; 7 % 2
来源：http://eny.xylfe.cn

Ruby: 7 / 2; 7 % 2
来源：http://pzf.chenzaomai.com

C#:   7 / 2; 7 % 2
来源：http://qqu.haohaochexian.top

[A06] 字符串转数字
来源：http://gqf.cqqwz.cn

Py:   int("42"); float("3.14")
来源：http://bab.fanxiaobao.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gvk.iojbl.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nwk.yongpay.top

TS:   parseInt("42", 10); Number("42")
来源：http://gbw.xinyue.icu

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rqk.9152youxi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wrk.nwbrower.top

Ruby: "42".to_i; "3.14".to_f
来源：http://hih.aibaodan.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zso.xuetiantiany.cn

[A07] 数字转字符串
来源：http://hyj.fktsv.cn

Py:   str(42)
来源：http://mjk.cdnleiting.top

PHP:  (string) 42; strval(42)
来源：http://xbo.fzhhl.top

JS:   String(42); (42).toString()
来源：http://cji.yongpay.top

TS:   String(42)
来源：http://awt.gogol.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qzb.52xcode.cn

Go:   strconv.Itoa(42)
来源：http://dpq.jyoumei.cn

Ruby: 42.to_s
来源：http://qcr.nanxinkj.top

C#:   42.ToString()
来源：http://uyy.shanyushiyangtech.top

[A08] 取整与四舍五入
来源：http://gfe.sysykeji.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rhv.meibo888.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://skv.meibo888.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gih.nanxinkj.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xac.yanxiufei.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mqp.yanxiufei.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nyw.sufxvd.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://nct.zhixingplan.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ewv.316326.xyz

[A09] 绝对值与最大最小值
来源：http://umr.sufxvd.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bvy.zhoulong.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://moe.yuanzhike.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gum.andypj.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ljo.hammf.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lxd.hesvh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://glc.wangdashe.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zaa.meibo888.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ase.sjlbkw.cn

[A10] 生成随机数
来源：http://wdc.aizwys.cn

Py:   import random; random.randint(1, 100)
来源：http://dsq.kuanghao11.cn

PHP:  random_int(1, 100);
来源：http://efc.tianlin.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://oju.bjfxy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vem.nwbrower.top

Java: new Random().nextInt(100) + 1
来源：http://ivc.pycfn.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://iot.zhaomingkeji.xyz

Ruby: rand(1..100)
来源：http://mqs.wangdashe.top

C#:   new Random().Next(1, 101)
来源：http://zgv.zhixingplan.top

[A11] 条件表达式（三元）
来源：http://vhy.cdnleiting.top

Py:   "yes" if x > 0 else "no"
来源：http://xwi.zhaomingkeji.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://rsw.0kj1m.cn

JS:   x > 0 ? "yes" : "no"
来源：http://phr.ivvv.top

TS:   x > 0 ? "yes" : "no"
来源：http://qfg.hfpthk.cn

Java: x > 0 ? "yes" : "no"
来源：http://pkh.gzhubu.top

Go:   // 无三元运算符，需用 if 语句
来源：http://vjy.gzhubu.top

Ruby: x > 0 ? "yes" : "no"
来源：http://qbe.xuanzx.com

C#:   x > 0 ? "yes" : "no"
来源：http://rjz.hfpthk.cn

[A12] 字符串插值 / 格式化
来源：http://uoq.shanyushiyangtech.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://glg.jinqigfzy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rsq.fanxiaobao.xyz

JS:   `Hello, ${name}!`
来源：http://qqw.zhiwuduotai.top

TS:   `Hello, ${name}!`
来源：http://ohi.zdqjudy.top

Java: "Hello, %s!".formatted(name)
来源：http://sxq.nwbrower.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hqn.fehbvm.com

Ruby: "Hello, #{name}!"
来源：http://amj.hesvh.cn

C#:   $"Hello, {name}!"
来源：http://rnv.ctjpmb.com

[A13] 多行字符串（练习 \n 转义）
来源：http://zws.gogol.net.cn

Py:   "第一行\n第二行"
来源：http://roe.fzhhl.top

PHP:  "第一行\n第二行"
来源：http://fwj.gzhubu.top

JS:   "第一行\n第二行"
来源：http://ery.tian-w.cn

TS:   "第一行\n第二行"
来源：http://nlw.feifeiyinyue.top

Java: "第一行\n第二行"
来源：http://kgp.ivvv.top

Go:   "第一行\n第二行"
来源：http://mxj.vqdsnc.cn

Ruby: "第一行\n第二行"
来源：http://fgr.zdbjq.cn

C#:   "第一行\n第二行"
来源：http://har.ppjwa.cn

[A14] 注释写法
来源：http://uqq.yj20258888.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://kxn.hywenlv.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rpn.daria6918.cn

JS:   // 单行；/* 多行 */
来源：http://svx.jinghuilouyu.cn

TS:   // 单行；/* 多行 */
来源：http://ztk.epnwcf.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lii.0kj1m.cn

Go:   // 单行；/* 多行 */
来源：http://qsr.shanyushiyangkeji.top

Ruby: # 单行；=begin 多行 =end
来源：http://rah.fehbvm.com

C#:   // 单行；/* 多行 */
来源：http://bjo.ywan-chungtsiang.top

[A15] 空值判断与默认值
来源：http://wfx.kuanghao11.cn

Py:   value = data or "默认值"
来源：http://fze.dianchejie.cn

PHP:  $value = $data ?? "默认值";
来源：http://hvg.fengsongda.top

JS:   const value = data ?? "默认值";
来源：http://yrj.aizwys.cn

TS:   const value = data ?? "默认值";
来源：http://cgw.jlsjyb.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dlq.52xcode.cn

Go:   if data == "" { data = "默认值" }
来源：http://gtz.zhijiandao.cn

Ruby: value = data || "默认值"
来源：http://ghr.shanyushiyangtech.top

C#:   var value = data ?? "默认值";
来源：http://qff.hywenlv.cn

[A16] 真假值判断规则
来源：http://wen.gaohongyu789.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://uon.ybcxt.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vlx.yonumen.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jcf.hysaishi.cn

TS:   if (!x) {}
来源：http://imv.fktsv.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tfd.aizwys.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uzv.cucudq.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gdj.nanxuanxn.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://oig.nwbrower.top

[A17] 位运算
来源：http://vck.shangyingyoupin.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wrd.fktsv.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hte.nwbrower.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kpx.zhoulong.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wbm.svipenyu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qqa.gaohongyu789.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xax.xinyue.icu

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xka.jqgufenzy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ily.yonumen.top

[A18] 字符与 ASCII 码互转
来源：http://csp.gzhubu.top

Py:   ord("A"); chr(65)
来源：http://iea.feifeiyinyue.top

PHP:  ord("A"); chr(65)
来源：http://qvv.tanke756.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vqf.kuanghao11.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qdi.c1oappe.top

Java: (int) 'A'; (char) 65
来源：http://ckr.fktsv.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wwa.mhx1999.top

Ruby: "A".ord; 65.chr
来源：http://yqp.sxryk.cn

C#:   (int)'A'; (char)65
来源：http://qhp.shzxlz.cn

[A19] 交换两个变量
来源：http://hun.daxiang520.top

Py:   a, b = b, a
来源：http://xap.ydjk.org.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://auq.zdbjq.cn

JS:   [a, b] = [b, a];
来源：http://ash.hongshengwenyu.top

TS:   [a, b] = [b, a];
来源：http://gqa.sxryk.cn

Java: int t = a; a = b; b = t;
来源：http://ixw.feifeiyinyue.top

Go:   a, b = b, a
来源：http://zis.jinqigfzy.top

Ruby: a, b = b, a
来源：http://ave.chenjidiqi.icu

C#:   (a, b) = (b, a);
来源：http://moe.chenzaomai.com

[A20] 读取标准输入
来源：http://qov.iojbl.cn

Py:   name = input("请输入：")
来源：http://per.andypj.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://nlm.xylfe.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://flt.sweek.top

TS:   // Node.js：readline 模块
来源：http://cyd.epnwcf.com

Java: new Scanner(System.in).nextLine()
来源：http://vrb.fktsv.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qxs.ydzc1.top

Ruby: gets.chomp
来源：http://irb.yangfankeji.com

C#:   Console.ReadLine();
来源：http://gch.ctjpmb.com

[A21] 保留指定小数位输出
来源：http://kdr.pengpengdd.cyou

Py:   f"{3.14159:.2f}"
来源：http://bxv.xziqi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://uda.yuanzhike.top

JS:   (3.14159).toFixed(2)
来源：http://lwk.kuanghao11.cn

TS:   (3.14159).toFixed(2)
来源：http://zer.tian-w.cn

Java: String.format("%.2f", 3.14159)
来源：http://adl.hfpthk.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://iaj.ppjwa.cn

Ruby: format("%.2f", 3.14159)
来源：http://ffo.zdbjq.cn

C#:   3.14159.ToString("F2")
来源：http://pug.smart0.xyz

[A22] 获取字符串长度
来源：http://rbp.xuetiantiany.cn

Py:   len(s)
来源：http://hhy.quarkkingdee.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pij.ctjpmb.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ymw.xziqi.cn

TS:   s.length
来源：http://poy.vehdjk.com

Java: s.length()
来源：http://wlv.vqdsnc.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vez.sufxvd.cn

Ruby: s.length
来源：http://ard.vqdsnc.cn

C#:   s.Length
来源：http://yrh.chenlongwang.top

[A23] 大小写转换
来源：http://mbe.iojbl.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://peo.sjlbkw.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ykb.vehdjk.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bcl.xinyue.icu

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zui.jianghu66.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hyg.yvedp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sia.cucudq.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qsr.hnqzz.top

C#:   s.ToUpper(); s.ToLower()
来源：http://mzr.zhengqikj.top

[A24] 去除首尾空白
来源：http://igp.zdbjq.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vqu.yanxiufei.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qns.gogol.net.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bti.hammf.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dtw.yj20258888.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xky.smart0.xyz

Go:   strings.TrimSpace(s)
来源：http://hyp.fzhhl.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hqd.zhaomingkeji.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jng.yj20258.top

[A25] 字符串比较
来源：http://bdc.sjlbkw.cn

Py:   s1 == s2; s1 != s2
来源：http://rad.tianlin.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vop.yueranfly.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hct.jinqigufen.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gtd.dashuyun.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mmx.nanxuanxn.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cpi.nwbrower.top

Ruby: s1 == s2; s1 <=> s2
来源：http://gpl.ctjpmb.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://izz.chenjidiqi.icu

[A26] 类型转换总览
来源：http://zav.yfazqb.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://upc.gotoacloud.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://idy.316326.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xpf.fanxiaobao.xyz

TS:   Number() String() Boolean() x as number
来源：http://gkl.xylfe.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pgs.sweek.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sdu.sjlbkw.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gdo.xylfe.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fbi.svipenyu.cn

================================================================================
来源：http://dwx.0kj1m.cn

B. 流程控制
来源：http://pek.epnwcf.com

================================================================================
来源：http://ltd.gotoacloud.top

[B01] 条件判断 if / else
来源：http://scp.shuidangran.top

Py:   result = "正" if x > 0 else "非正"
来源：http://lhu.ivvv.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oyk.yj20258.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://out.bbcook.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://frh.vehdjk.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://sjv.guowangkeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://afz.gogol.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fku.shuidangran.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://the.guannengcc.top

[B02] 多分支 else if / elif
来源：http://mbw.yangfankeji.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://prt.sweek.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uii.ywan-chungtsiang.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cns.meibo888.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dns.xylfe.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aky.yuxming.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kxa.hongshengwenyu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yix.shanyushiyangtech.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pev.hongshengwenyu.top

[B03] switch / match / case
来源：http://cuc.jiagoushi.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fii.fktsv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lgt.jianghu66.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mna.ywan-chungtsiang.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nhb.chenlongwang.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://evp.vehdjk.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ixd.cucudq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jkk.ppjwa.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vei.hongshengwenyu.top

[B04] for 计数循环
来源：http://qcf.yvedp.cn

Py:   for i in range(10): print(i)
来源：http://nyv.hnqzz.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yiz.pycfn.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dxs.shanyushiyangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xgo.birdmap.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rhd.jqgfzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ara.kuanghao11.cn

Ruby: 10.times { |i| puts i }
来源：http://dls.hongshengwenyu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hsl.yanxiufei.cn

[B05] 遍历数组 / 列表
来源：http://sop.yanxiufei.cn

Py:   for item in arr: print(item)
来源：http://ftj.gzhubu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sdi.pycfn.com

JS:   for (const item of arr) { console.log(item); }
来源：http://css.wangshuangyany.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nyo.cdnleiting.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://dyn.hywenlv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lea.feifeiyinyue.top

Ruby: arr.each { |item| puts item }
来源：http://phk.yfazqb.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cjx.xingfuxueyuan.xyz

[B06] 遍历字典 / 对象
来源：http://usv.yangfankeji.com

Py:   for k, v in d.items(): print(k, v)
来源：http://ovg.jqgfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kiv.nanxuanxn.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jex.pycfn.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xhp.xuanzx.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gwt.yanxiufei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yls.quarkkingdee.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://etc.shanyushiyangtech.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yhj.zdbjq.cn

[B07] while 循环
来源：http://kjf.ppjwa.cn

Py:   while i < 10: i += 1
来源：http://rpx.yj20258.top

PHP:  while ($i < 10) { $i++; }
来源：http://fzu.cucudq.cn

JS:   while (i < 10) { i++; }
来源：http://cta.aibaodan.cn

TS:   while (i < 10) { i++; }
来源：http://yak.9152youxi.cn

Java: while (i < 10) { i++; }
来源：http://dej.hammf.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fun.nwbrower.top

Ruby: while i < 10; i += 1; end
来源：http://zml.jinyuanbaomall.cn

C#:   while (i < 10) { i++; }
来源：http://krb.pengpengdd.cyou

[B08] do-while（至少执行一次）
来源：http://vay.svipenyu.cn

Py:   # 无 do-while：用 while True + break
来源：http://vuf.yj202588.top

PHP:  do { $i++; } while ($i < 10);
来源：http://dzs.cucudq.cn

JS:   do { i++; } while (i < 10);
来源：http://cfb.tanke756.top

TS:   do { i++; } while (i < 10);
来源：http://ett.tian-w.cn

Java: do { i++; } while (i < 10);
来源：http://tkz.chenlongwang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fcd.c1oappe.top

Ruby: begin; i += 1; end while i < 10
来源：http://xxq.kuanghao11.cn

C#:   do { i++; } while (i < 10);
来源：http://iwq.ehwqpu.com

[B09] break 与 continue
来源：http://ljz.redwolf501.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://noj.jlsjyb.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yuq.chenzaomai.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vcc.cdnleiting.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jkt.52xcode.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mpi.jianghu66.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lqm.daxiang520.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dgy.zhiwuduotai.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xaq.xinyue.icu

[B10] 遍历同时拿索引
来源：http://mik.9152youxi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hgb.0kj1m.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rrs.ppjwa.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wed.pengpengdd.cyou

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wpe.guowangkeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yyp.hywenlv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mhh.cucudq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hen.hnqzz.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vok.guannengcc.top

[B11] 生成数字序列 / 区间
来源：http://wxq.cdnleiting.top

Py:   list(range(0, 10, 2))
来源：http://nuz.jlsjyb.cn

PHP:  range(0, 10, 2);
来源：http://ezw.gaohongyu789.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uqp.sysykeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mkn.sysykeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hvq.sufxvd.cn


<!-- 参考信息 -->