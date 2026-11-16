代发 wailian999

JS:   String(42); (42).toString()
来源：http://xmz.hfpthk.cn

TS:   String(42)
来源：http://yvr.316326.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://xbr.feifeiyinyue.top

Go:   strconv.Itoa(42)
来源：http://aqq.hywenlv.cn

Ruby: 42.to_s
来源：http://myz.andypj.xyz

C#:   42.ToString()
来源：http://fsc.9152youxi.cn

[A08] 取整与四舍五入
来源：http://ark.9152youxi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zsb.xziqi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ifx.xylfe.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://apq.fzhhl.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sus.shzxlz.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://udx.birdmap.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qrk.wangdashe.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ihi.aibaodan.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://uso.aibaodan.cn

[A09] 绝对值与最大最小值
来源：http://enw.zhixingplan.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cse.haohaochexian.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ain.zhiwuduotai.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tzg.epnwcf.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bpd.kuanghao11.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jza.uphjek.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://san.hfpthk.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bww.yangfankeji.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://znr.chenlongwang.top

[A10] 生成随机数
来源：http://nhy.nanxuanxn.top

Py:   import random; random.randint(1, 100)
来源：http://nqf.yanxiufei.cn

PHP:  random_int(1, 100);
来源：http://fit.yuxming.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uvl.cucudq.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tcf.pengpengdd.cyou

Java: new Random().nextInt(100) + 1
来源：http://rei.svipenyu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qhb.gogol.net.cn

Ruby: rand(1..100)
来源：http://eog.iojbl.cn

C#:   new Random().Next(1, 101)
来源：http://giv.jqgufenzy.top

[A11] 条件表达式（三元）
来源：http://vnp.hywenlv.cn

Py:   "yes" if x > 0 else "no"
来源：http://tqi.epnwcf.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://wje.ivvv.top

JS:   x > 0 ? "yes" : "no"
来源：http://cpl.bbcook.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hmx.epnwcf.com

Java: x > 0 ? "yes" : "no"
来源：http://owr.c1oappe.top

Go:   // 无三元运算符，需用 if 语句
来源：http://goy.guannengcc.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ejm.hnqzz.top

C#:   x > 0 ? "yes" : "no"
来源：http://kag.yuxming.cn

[A12] 字符串插值 / 格式化
来源：http://pqb.sufxvd.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lok.smart0.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ual.guowangkeji.top

JS:   `Hello, ${name}!`
来源：http://axq.vehdjk.com

TS:   `Hello, ${name}!`
来源：http://raf.ehwqpu.com

Java: "Hello, %s!".formatted(name)
来源：http://geu.ehwqpu.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rts.vehdjk.com

Ruby: "Hello, #{name}!"
来源：http://mhm.xylfe.cn

C#:   $"Hello, {name}!"
来源：http://aae.quarkkingdee.top

[A13] 多行字符串（练习 \n 转义）
来源：http://npp.cashguo.top

Py:   "第一行\n第二行"
来源：http://obd.fktsv.cn

PHP:  "第一行\n第二行"
来源：http://dek.hfpthk.cn

JS:   "第一行\n第二行"
来源：http://knc.tarul.cn

TS:   "第一行\n第二行"
来源：http://wdp.chenlongwang.top

Java: "第一行\n第二行"
来源：http://tty.daria6918.cn

Go:   "第一行\n第二行"
来源：http://vkb.sxryk.cn

Ruby: "第一行\n第二行"
来源：http://tdf.bbcook.cn

C#:   "第一行\n第二行"
来源：http://bjo.iojbl.cn

[A14] 注释写法
来源：http://fpz.fzhhl.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://goz.shanyushiyangkeji.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://llh.c1oappe.top

JS:   // 单行；/* 多行 */
来源：http://tbu.yanxiufei.cn

TS:   // 单行；/* 多行 */
来源：http://etq.aizwys.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tru.iojbl.cn

Go:   // 单行；/* 多行 */
来源：http://hyf.gogol.net.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ily.aizwys.cn

C#:   // 单行；/* 多行 */
来源：http://nbr.iojbl.cn

[A15] 空值判断与默认值
来源：http://bdd.nwbrower.top

Py:   value = data or "默认值"
来源：http://qbx.yj20258.top

PHP:  $value = $data ?? "默认值";
来源：http://mnk.hesvh.cn

JS:   const value = data ?? "默认值";
来源：http://ovk.zhongyouzk.top

TS:   const value = data ?? "默认值";
来源：http://wzo.vehdjk.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ktv.zhengqikj.top

Go:   if data == "" { data = "默认值" }
来源：http://rnu.chenlongwang.top

Ruby: value = data || "默认值"
来源：http://sth.hammf.cn

C#:   var value = data ?? "默认值";
来源：http://duk.hywenlv.cn

[A16] 真假值判断规则
来源：http://wla.smart0.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hcc.shzxlz.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://evj.shuidangran.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sjf.shanyushiyangtech.top

TS:   if (!x) {}
来源：http://ugi.0kj1m.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fxr.zdqjudy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lds.uphjek.com

Ruby: unless x            # nil 与 false 为假
来源：http://edo.hnqzz.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ksi.jinqigfzy.top

[A17] 位运算
来源：http://yzi.daxiang520.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cay.dianchejie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dhf.andypj.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wqn.shanyushiyangkeji.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uqj.zdbjq.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ary.316326.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tim.fengsongda.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xly.hnqzz.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hyc.bjfxy.top

[A18] 字符与 ASCII 码互转
来源：http://hjy.yj20258.top

Py:   ord("A"); chr(65)
来源：http://enl.ywan-chungtsiang.top

PHP:  ord("A"); chr(65)
来源：http://azm.yonumen.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xed.yj20258.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yoh.iojbl.cn

Java: (int) 'A'; (char) 65
来源：http://qgr.quarkkingdee.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tvu.guowangkeji.top

Ruby: "A".ord; 65.chr
来源：http://uig.guannengcc.top

C#:   (int)'A'; (char)65
来源：http://rav.daxiang520.top

[A19] 交换两个变量
来源：http://fdy.hcnkem.com

Py:   a, b = b, a
来源：http://eua.cdnleiting.top

PHP:  [$a, $b] = [$b, $a];
来源：http://hrh.0kj1m.cn

JS:   [a, b] = [b, a];
来源：http://xmx.yvedp.cn

TS:   [a, b] = [b, a];
来源：http://cwl.ybcxt.top

Java: int t = a; a = b; b = t;
来源：http://uys.guowangkeji.top

Go:   a, b = b, a
来源：http://dtu.mhx1999.top

Ruby: a, b = b, a
来源：http://sew.ivvv.top

C#:   (a, b) = (b, a);
来源：http://xzx.fanxiaobao.xyz

[A20] 读取标准输入
来源：http://hve.hfpthk.cn

Py:   name = input("请输入：")
来源：http://rjz.sweek.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ght.zycfv.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zsx.feifeiyinyue.top

TS:   // Node.js：readline 模块
来源：http://abr.sxryk.cn

Java: new Scanner(System.in).nextLine()
来源：http://hoh.jqgfzy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dnj.zhongyouzk.top

Ruby: gets.chomp
来源：http://xmb.daxiang520.top

C#:   Console.ReadLine();
来源：http://gwq.tianlin.xyz

[A21] 保留指定小数位输出
来源：http://vyg.ybcxt.top

Py:   f"{3.14159:.2f}"
来源：http://pvr.ehwqpu.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rdm.fanxiaobao.xyz

JS:   (3.14159).toFixed(2)
来源：http://tqg.nanxinkj.top

TS:   (3.14159).toFixed(2)
来源：http://cea.jqgufenzy.top

Java: String.format("%.2f", 3.14159)
来源：http://kjh.haohaochexian.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kqx.cucudq.cn

Ruby: format("%.2f", 3.14159)
来源：http://bih.vehdjk.com

C#:   3.14159.ToString("F2")
来源：http://phk.chenlongwang.top

[A22] 获取字符串长度
来源：http://lif.bbcook.cn

Py:   len(s)
来源：http://suu.yj20258888.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zcr.hesvh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ong.vqdsnc.cn

TS:   s.length
来源：http://nxb.smart0.xyz

Java: s.length()
来源：http://rpu.ehwqpu.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wra.meibo888.top

Ruby: s.length
来源：http://wuj.zhixingplan.top

C#:   s.Length
来源：http://zfg.kuanghao11.cn

[A23] 大小写转换
来源：http://ptf.sjlbkw.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nvz.zdqjudy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bbc.zhaomingkeji.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cfs.ivvv.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ayd.zhaomingkeji.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://waf.pengpengdd.cyou

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pha.c1oappe.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sel.guannengcc.top

C#:   s.ToUpper(); s.ToLower()
来源：http://rlb.yongpay.top

[A24] 去除首尾空白
来源：http://ylf.snrcjt.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wbb.redwolf501.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nbf.jqgufenzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pln.jinqigufen.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tqp.nanxuanxn.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vle.ywan-chungtsiang.top

Go:   strings.TrimSpace(s)
来源：http://fgv.shuidangran.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cbf.zhiwuduotai.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://eii.ivvv.top

[A25] 字符串比较
来源：http://bux.daxiang520.top

Py:   s1 == s2; s1 != s2
来源：http://kwh.yj202588.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ngn.mhx1999.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pli.yfazqb.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ahh.quarkkingdee.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qth.c1oappe.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://eif.hongshengwenyu.top

Ruby: s1 == s2; s1 <=> s2
来源：http://qyn.yvedp.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://apb.svipenyu.cn

[A26] 类型转换总览
来源：http://zpk.zdqjudy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vdm.gaohongyu789.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bdz.chenlongwang.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mbr.uphjek.com

TS:   Number() String() Boolean() x as number
来源：http://jli.daria6918.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lba.uphjek.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kmv.ppjwa.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://iaf.ywan-chungtsiang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://obz.quarkkingdee.top

================================================================================
来源：http://vuj.feifeiyinyue.top

B. 流程控制
来源：http://xyj.cashguo.top

================================================================================
来源：http://uny.havefunace.top

[B01] 条件判断 if / else
来源：http://rye.jinqigfzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://luh.zhixingplan.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qwr.yj20258.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jku.zhaomingkeji.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gnr.zhiwuduotai.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://acs.tanke756.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://avy.cqqwz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://stv.yfazqb.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dhd.yongpay.top

[B02] 多分支 else if / elif
来源：http://lqd.tarul.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://stc.yanxiufei.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://afc.wangshuangyany.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yag.zdbjq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aeb.nanxuanxn.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ttd.c1oappe.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mgq.epnwcf.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pxf.quarkkingdee.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mzz.shangyingyoupin.top

[B03] switch / match / case
来源：http://khc.shanyushiyangkeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nlk.yfazqb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rit.aizwys.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://klv.fktsv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uom.yanxiufei.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vnd.shangyingyoupin.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jrl.fengsongda.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qbo.yueranfly.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://odp.vqdsnc.cn

[B04] for 计数循环
来源：http://ana.nanxinkj.top

Py:   for i in range(10): print(i)
来源：http://mng.yanxiufei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jrh.jinghuilouyu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://drz.316326.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lmn.chenlongwang.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jbi.hammf.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wny.yuanzhike.top

Ruby: 10.times { |i| puts i }
来源：http://fdr.daria6918.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rqn.cashguo.top

[B05] 遍历数组 / 列表
来源：http://dbd.yj20258888.top

Py:   for item in arr: print(item)
来源：http://myb.bbcook.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://shk.redwolf501.top

JS:   for (const item of arr) { console.log(item); }
来源：http://gtd.fzhhl.top

TS:   for (const item of arr) { console.log(item); }
来源：http://lsx.chenlongwang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://kzc.jinghuilouyu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ymk.cheryme.top

Ruby: arr.each { |item| puts item }
来源：http://rdq.pengpengdd.cyou

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ljv.gzhubu.top

[B06] 遍历字典 / 对象
来源：http://sgl.tanke756.top

Py:   for k, v in d.items(): print(k, v)
来源：http://pco.zhengqikj.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://upb.quarkkingdee.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uiy.xinyue.icu

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mbi.sweek.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uqh.zhiwuduotai.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yin.zdbjq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qvq.vehdjk.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mpy.bjfxy.top

[B07] while 循环
来源：http://xqk.xziqi.cn

Py:   while i < 10: i += 1
来源：http://sxt.jlsjyb.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qer.yj20258.top

JS:   while (i < 10) { i++; }
来源：http://zmu.birdmap.top

TS:   while (i < 10) { i++; }
来源：http://dnd.yonumen.top

Java: while (i < 10) { i++; }
来源：http://yyw.chenlongwang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dkn.mhx1999.top

Ruby: while i < 10; i += 1; end
来源：http://ort.ywan-chungtsiang.top

C#:   while (i < 10) { i++; }
来源：http://wsk.meibo888.top

[B08] do-while（至少执行一次）
来源：http://nrt.yuanzhike.top

Py:   # 无 do-while：用 while True + break
来源：http://caa.ppjwa.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ald.316326.xyz

JS:   do { i++; } while (i < 10);
来源：http://eja.tian-w.cn

TS:   do { i++; } while (i < 10);
来源：http://ifr.shanyushiyangkeji.top

Java: do { i++; } while (i < 10);
来源：http://ubn.yongpay.top

Go:   for { i++; if i >= 10 { break } }
来源：http://odo.bbcook.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vvz.wangshuangyany.cn

C#:   do { i++; } while (i < 10);
来源：http://opi.gzhubu.top

[B09] break 与 continue
来源：http://zmz.aizwys.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ofs.nanxinkj.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jiu.xylfe.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ihw.jiagoushi.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xnh.9152youxi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gtw.fktsv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jzh.yfazqb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cib.guannengcc.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://npd.bjfxy.top

[B10] 遍历同时拿索引
来源：http://aod.meibo888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://idx.cheryme.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ity.zhixingplan.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://usu.yj202588.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tcq.nanxuanxn.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nfu.nanxuanxn.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kao.zhaomingkeji.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dxl.xuanzx.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nre.0kj1m.cn

[B11] 生成数字序列 / 区间
来源：http://fxd.zdqjudy.top

Py:   list(range(0, 10, 2))
来源：http://vkm.fzhhl.top

PHP:  range(0, 10, 2);
来源：http://ijo.yj20258888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gnj.daria6918.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hbm.fanxiaobao.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://stj.chenlongwang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bxt.hammf.cn

Ruby: (0...10).step(2).to_a
来源：http://tgj.andypj.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xrz.jiagoushi.top

[B12] 跳出多层循环
来源：http://xvw.yangfankeji.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://wbn.yvedp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mfh.haohaochexian.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sci.cashguo.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iol.xylfe.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ope.jinqigfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://beq.ehwqpu.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tuz.jinqigufen.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pyx.hcnkem.com

[B13] 判断是否为数字
来源：http://ohp.jiagoushi.top

Py:   isinstance(x, (int, float))
来源：http://xwl.bbcook.cn

PHP:  is_numeric($x)
来源：http://ddx.ydjk.org.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ewv.jianghu66.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://avr.xziqi.cn

Java: x instanceof Number
来源：http://gyi.yongpay.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xln.hammf.cn

Ruby: x.is_a?(Numeric)
来源：http://nll.vqdsnc.cn

C#:   x is int or double or decimal
来源：http://yht.tian-w.cn

[B14] 判断值是否在集合内
来源：http://uad.vqdsnc.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bjy.fehbvm.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xmt.yvedp.cn


<!-- 参考信息 -->