代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://gdw.yonumen.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://njx.wangshuangyany.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qog.gotoacloud.top

Ruby: "42".to_i; "3.14".to_f
来源：http://wxj.ydzc1.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://itl.shanyushiyangtech.top

[A07] 数字转字符串
来源：http://zir.tarul.cn

Py:   str(42)
来源：http://lnw.jinqigfzy.top

PHP:  (string) 42; strval(42)
来源：http://kdq.guowangkeji.top

JS:   String(42); (42).toString()
来源：http://nvt.fengsongda.top

TS:   String(42)
来源：http://gdq.zdbjq.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qih.aizwys.cn

Go:   strconv.Itoa(42)
来源：http://vlx.yj20258.top

Ruby: 42.to_s
来源：http://xqd.ehwqpu.com

C#:   42.ToString()
来源：http://hrp.zhoulong.xyz

[A08] 取整与四舍五入
来源：http://hxv.hammf.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mjt.yj202588.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jzx.zhixingplan.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xgr.sysykeji.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zha.xuetiantiany.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cvd.jinghuilouyu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zuz.chenlongwang.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://nea.52xcode.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lim.quarkkingdee.top

[A09] 绝对值与最大最小值
来源：http://ldp.svipenyu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jtx.quarkkingdee.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://acw.jqgfzy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dyh.yanxiufei.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cae.ivvv.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vbd.yangfankeji.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://twj.fehbvm.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://woa.aizwys.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jaj.ppjwa.cn

[A10] 生成随机数
来源：http://hzh.xuanzx.com

Py:   import random; random.randint(1, 100)
来源：http://iln.shanyushiyangkeji.top

PHP:  random_int(1, 100);
来源：http://zxo.dashuyun.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pme.yvedp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nxv.shanyushiyangtech.top

Java: new Random().nextInt(100) + 1
来源：http://xss.tianlin.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hmr.hfpthk.cn

Ruby: rand(1..100)
来源：http://tdt.hywenlv.cn

C#:   new Random().Next(1, 101)
来源：http://yzs.ehwqpu.com

[A11] 条件表达式（三元）
来源：http://apm.zdqjudy.top

Py:   "yes" if x > 0 else "no"
来源：http://kuq.xinyue.icu

PHP:  $x > 0 ? "yes" : "no"
来源：http://drc.yanxiufei.cn

JS:   x > 0 ? "yes" : "no"
来源：http://nkc.meibo888.top

TS:   x > 0 ? "yes" : "no"
来源：http://ocu.zdbjq.cn

Java: x > 0 ? "yes" : "no"
来源：http://vbo.guannengcc.top

Go:   // 无三元运算符，需用 if 语句
来源：http://zuz.jinghuilouyu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vsk.hcnkem.com

C#:   x > 0 ? "yes" : "no"
来源：http://lyz.havefunace.top

[A12] 字符串插值 / 格式化
来源：http://fea.chenjidiqi.icu

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vjm.epnwcf.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ssf.zhiwuduotai.top

JS:   `Hello, ${name}!`
来源：http://ftx.bjfxy.top

TS:   `Hello, ${name}!`
来源：http://xjb.yuanzhike.top

Java: "Hello, %s!".formatted(name)
来源：http://lax.hysaishi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yaq.jinqigfzy.top

Ruby: "Hello, #{name}!"
来源：http://jxw.chenzaomai.com

C#:   $"Hello, {name}!"
来源：http://mqu.jqgfzy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ksl.epnwcf.com

Py:   "第一行\n第二行"
来源：http://ejk.jinqigufen.top

PHP:  "第一行\n第二行"
来源：http://cgp.jinyuanbaomall.cn

JS:   "第一行\n第二行"
来源：http://mnr.epnwcf.com

TS:   "第一行\n第二行"
来源：http://ujz.jlsjyb.cn

Java: "第一行\n第二行"
来源：http://aey.zhixingplan.top

Go:   "第一行\n第二行"
来源：http://ivt.havefunace.top

Ruby: "第一行\n第二行"
来源：http://soj.kuanghao11.cn

C#:   "第一行\n第二行"
来源：http://ytk.fengsongda.top

[A14] 注释写法
来源：http://fra.nanxuanxn.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://gkx.zdbjq.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jhr.xziqi.cn

JS:   // 单行；/* 多行 */
来源：http://wox.shuidangran.top

TS:   // 单行；/* 多行 */
来源：http://lyv.ctjpmb.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ctz.fktsv.cn

Go:   // 单行；/* 多行 */
来源：http://osd.hnxiangtu.top

Ruby: # 单行；=begin 多行 =end
来源：http://yoi.jlsjyb.cn

C#:   // 单行；/* 多行 */
来源：http://rbz.daria6918.cn

[A15] 空值判断与默认值
来源：http://fku.yanxiufei.cn

Py:   value = data or "默认值"
来源：http://okt.zdbjq.cn

PHP:  $value = $data ?? "默认值";
来源：http://fkq.cqqwz.cn

JS:   const value = data ?? "默认值";
来源：http://owy.zdqjudy.top

TS:   const value = data ?? "默认值";
来源：http://zdd.yangfankeji.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fmt.cucudq.cn

Go:   if data == "" { data = "默认值" }
来源：http://zcq.jinqigufen.top

Ruby: value = data || "默认值"
来源：http://pqi.fengsongda.top

C#:   var value = data ?? "默认值";
来源：http://zui.yangfankeji.com

[A16] 真假值判断规则
来源：http://znn.cdnleiting.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mrj.meibo888.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://htr.zhoulong.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jfl.jqgfzy.top

TS:   if (!x) {}
来源：http://mhu.daria6918.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://skt.xuanzx.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rpz.jianghu66.top

Ruby: unless x            # nil 与 false 为假
来源：http://sez.shangyingyoupin.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://flb.bjfxy.top

[A17] 位运算
来源：http://qza.zycfv.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nau.pycfn.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://esn.hammf.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wut.daxiang520.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://khz.guannengcc.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rzf.hysaishi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xke.9152youxi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://smy.havefunace.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jxf.vqdsnc.cn

[A18] 字符与 ASCII 码互转
来源：http://jyv.hywenlv.cn

Py:   ord("A"); chr(65)
来源：http://qoi.yj20258888.top

PHP:  ord("A"); chr(65)
来源：http://trh.zhongyouzk.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pzu.jlsjyb.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ons.zhiwuduotai.top

Java: (int) 'A'; (char) 65
来源：http://pch.zhengqikj.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wzz.yfazqb.com

Ruby: "A".ord; 65.chr
来源：http://wfn.fzhhl.top

C#:   (int)'A'; (char)65
来源：http://uys.sjlbkw.cn

[A19] 交换两个变量
来源：http://ksc.zdqjudy.top

Py:   a, b = b, a
来源：http://rbq.havefunace.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ubg.0kj1m.cn

JS:   [a, b] = [b, a];
来源：http://phc.iojbl.cn

TS:   [a, b] = [b, a];
来源：http://fhi.zhengqikj.top

Java: int t = a; a = b; b = t;
来源：http://qub.cdnleiting.top

Go:   a, b = b, a
来源：http://ihi.mhx1999.top

Ruby: a, b = b, a
来源：http://hde.ydzc1.top

C#:   (a, b) = (b, a);
来源：http://bgy.zdqjudy.top

[A20] 读取标准输入
来源：http://ykb.jyoumei.cn

Py:   name = input("请输入：")
来源：http://gyz.zdqjudy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://guu.zhaomingkeji.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sun.tianlin.xyz

TS:   // Node.js：readline 模块
来源：http://dfp.sxryk.cn

Java: new Scanner(System.in).nextLine()
来源：http://oqe.pengpengdd.cyou

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yfm.xylfe.cn

Ruby: gets.chomp
来源：http://xug.zhixingplan.top

C#:   Console.ReadLine();
来源：http://amc.yj20258888.top

[A21] 保留指定小数位输出
来源：http://mvq.cheryme.top

Py:   f"{3.14159:.2f}"
来源：http://ctn.zhongyouzk.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://csu.guannengcc.top

JS:   (3.14159).toFixed(2)
来源：http://tux.gaohongyu789.top

TS:   (3.14159).toFixed(2)
来源：http://nls.nanxuanxn.top

Java: String.format("%.2f", 3.14159)
来源：http://jpz.uphjek.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vkx.ctjpmb.com

Ruby: format("%.2f", 3.14159)
来源：http://igx.nanxinkj.top

C#:   3.14159.ToString("F2")
来源：http://ldm.chenjidiqi.icu

[A22] 获取字符串长度
来源：http://myk.hnqzz.top

Py:   len(s)
来源：http://tnd.hnqzz.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xst.andypj.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sfb.jinghuilouyu.cn

TS:   s.length
来源：http://sdv.cheryme.top

Java: s.length()
来源：http://qtf.sweek.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vbs.vehdjk.com

Ruby: s.length
来源：http://axa.ydjk.org.cn

C#:   s.Length
来源：http://hjk.tian-w.cn

[A23] 大小写转换
来源：http://sex.gzhubu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://eyy.sweek.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://riz.zhoulong.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rhp.jinyuanbaomall.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://crt.fanxiaobao.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qxd.yonumen.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pmm.zdqjudy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fvz.shangyingyoupin.top

C#:   s.ToUpper(); s.ToLower()
来源：http://xdm.jlsjyb.cn

[A24] 去除首尾空白
来源：http://tlf.ydjk.org.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fzh.vqdsnc.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kuj.9152youxi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pte.sweek.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hmu.c1oappe.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ihw.sysykeji.top

Go:   strings.TrimSpace(s)
来源：http://njd.9152youxi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://euc.chenlongwang.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rry.ppjwa.cn

[A25] 字符串比较
来源：http://vbh.hongshengwenyu.top

Py:   s1 == s2; s1 != s2
来源：http://pbe.guannengcc.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xua.hysaishi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vgf.yj20258.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rmy.ctjpmb.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lpj.ywan-chungtsiang.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ofx.c1oappe.top

Ruby: s1 == s2; s1 <=> s2
来源：http://lwd.sweek.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wgm.snrcjt.cn

[A26] 类型转换总览
来源：http://wyl.pengpengdd.cyou

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bqn.jqgfzy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tgm.pengpengdd.cyou

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://myq.jinyuanbaomall.cn

TS:   Number() String() Boolean() x as number
来源：http://wsr.jinqigufen.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xyt.epnwcf.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hen.yvedp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ygu.yuxming.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://unm.tianlin.xyz

================================================================================
来源：http://elz.yuxming.cn

B. 流程控制
来源：http://gsa.hongshengwenyu.top

================================================================================
来源：http://rfg.sufxvd.cn

[B01] 条件判断 if / else
来源：http://nfi.jyoumei.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ojc.ydzc1.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xya.yangfankeji.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ygn.daria6918.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kkl.snrcjt.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wbo.ctjpmb.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hhw.316326.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fqc.jlsjyb.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pcv.fengsongda.top

[B02] 多分支 else if / elif
来源：http://npx.zdbjq.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bub.ydjk.org.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://poz.ybcxt.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vjm.cucudq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://msc.pengpengdd.cyou

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dby.guannengcc.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vwr.nwbrower.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://viz.havefunace.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dag.gogol.net.cn

[B03] switch / match / case
来源：http://xrf.ctjpmb.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vbe.hywenlv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nlp.zhiwuduotai.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://muh.vqdsnc.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cfq.feifeiyinyue.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jxs.tian-w.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zel.xziqi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nde.cqqwz.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bqz.xuetiantiany.cn

[B04] for 计数循环
来源：http://blq.yvedp.cn

Py:   for i in range(10): print(i)
来源：http://ouw.svipenyu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://odp.xylfe.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qmf.smart0.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://exm.sysykeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gfn.pengpengdd.cyou

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ajb.guannengcc.top

Ruby: 10.times { |i| puts i }
来源：http://ojk.cashguo.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://anf.hfpthk.cn

[B05] 遍历数组 / 列表
来源：http://ify.zhongyouzk.top

Py:   for item in arr: print(item)
来源：http://faj.ctjpmb.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rna.ydjk.org.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qnk.cheryme.top

TS:   for (const item of arr) { console.log(item); }
来源：http://cas.mhx1999.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://xsf.sxryk.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://utd.aibaodan.cn

Ruby: arr.each { |item| puts item }
来源：http://yjo.fktsv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mzj.zdbjq.cn

[B06] 遍历字典 / 对象
来源：http://qdz.yueranfly.top

Py:   for k, v in d.items(): print(k, v)
来源：http://dpf.pengpengdd.cyou

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ofk.smart0.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mta.fktsv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pgk.tianlin.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ela.cdnleiting.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://umk.ydzc1.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rth.hnqzz.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aiu.bbcook.cn

[B07] while 循环
来源：http://rsu.dianchejie.cn

Py:   while i < 10: i += 1
来源：http://llz.52xcode.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tas.guannengcc.top

JS:   while (i < 10) { i++; }
来源：http://yth.nanxinkj.top

TS:   while (i < 10) { i++; }
来源：http://yxf.hnxiangtu.top

Java: while (i < 10) { i++; }
来源：http://hux.cqqwz.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bor.yfazqb.com

Ruby: while i < 10; i += 1; end
来源：http://rzw.daxiang520.top

C#:   while (i < 10) { i++; }
来源：http://cdi.chenjidiqi.icu

[B08] do-while（至少执行一次）
来源：http://qnk.nanxuanxn.top

Py:   # 无 do-while：用 while True + break
来源：http://sna.kuanghao11.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://svr.yvedp.cn

JS:   do { i++; } while (i < 10);
来源：http://hhz.aizwys.cn

TS:   do { i++; } while (i < 10);
来源：http://ypg.zycfv.cn

Java: do { i++; } while (i < 10);
来源：http://pih.yfazqb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://scs.hammf.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sot.hysaishi.cn

C#:   do { i++; } while (i < 10);
来源：http://uos.guowangkeji.top

[B09] break 与 continue
来源：http://siz.fzhhl.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pnz.sweek.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rdc.ppjwa.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ejz.nanxinkj.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dtw.ywan-chungtsiang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yac.yj202588.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bwg.hysaishi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://omm.smart0.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://axs.jyoumei.cn

[B10] 遍历同时拿索引
来源：http://zue.ywan-chungtsiang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ezp.chenzaomai.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rlz.uphjek.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://djw.ppjwa.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rqw.shanyushiyangkeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://arc.tianlin.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dqd.52xcode.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ubx.yonumen.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iet.wangdashe.top

[B11] 生成数字序列 / 区间
来源：http://kwt.pycfn.com

Py:   list(range(0, 10, 2))
来源：http://ghr.hcnkem.com

PHP:  range(0, 10, 2);
来源：http://oyu.yvedp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eku.uphjek.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gxu.jlsjyb.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jbw.zhoulong.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vdx.havefunace.top

Ruby: (0...10).step(2).to_a
来源：http://hyf.daxiang520.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qaf.quarkkingdee.top

[B12] 跳出多层循环
来源：http://wbd.chenjidiqi.icu

Py:   # 无标签跳转：抽成函数用 return
来源：http://tze.yfazqb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://jmk.cashguo.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tcq.shangyingyoupin.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uex.nanxuanxn.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jlz.tanke756.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cjm.xuanzx.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cno.meibo888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hsi.zhaomingkeji.xyz

[B13] 判断是否为数字
来源：http://kex.feifeiyinyue.top

Py:   isinstance(x, (int, float))
来源：http://koe.hesvh.cn

PHP:  is_numeric($x)
来源：http://hpr.jyoumei.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yxe.ydjk.org.cn


<!-- 参考信息 -->