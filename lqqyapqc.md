代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ivu.hcnkem.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://wlj.yfazqb.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ecs.chenlongwang.top

[A09] 绝对值与最大最小值
来源：http://woe.andypj.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xca.meibo888.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qwp.hongshengwenyu.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mpz.vehdjk.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://brm.havefunace.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://scb.zycfv.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sqi.zycfv.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rcp.hnqzz.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kmd.shangyingyoupin.top

[A10] 生成随机数
来源：http://won.jinqigufen.top

Py:   import random; random.randint(1, 100)
来源：http://fre.shanyushiyangtech.top

PHP:  random_int(1, 100);
来源：http://pmk.zdbjq.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tlz.zhongyouzk.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vzm.ydzc1.top

Java: new Random().nextInt(100) + 1
来源：http://rqw.pycfn.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lmr.smart0.xyz

Ruby: rand(1..100)
来源：http://htf.redwolf501.top

C#:   new Random().Next(1, 101)
来源：http://juf.kuanghao11.cn

[A11] 条件表达式（三元）
来源：http://ibg.hammf.cn

Py:   "yes" if x > 0 else "no"
来源：http://niu.hammf.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jzg.shuidangran.top

JS:   x > 0 ? "yes" : "no"
来源：http://vuk.tarul.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gun.yangfankeji.com

Java: x > 0 ? "yes" : "no"
来源：http://ptf.yfazqb.com

Go:   // 无三元运算符，需用 if 语句
来源：http://jvc.shanyushiyangkeji.top

Ruby: x > 0 ? "yes" : "no"
来源：http://mhj.0kj1m.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vqr.jinghuilouyu.cn

[A12] 字符串插值 / 格式化
来源：http://upp.xuetiantiany.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rua.haohaochexian.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://reh.yj20258.top

JS:   `Hello, ${name}!`
来源：http://job.ivvv.top

TS:   `Hello, ${name}!`
来源：http://mxl.ehwqpu.com

Java: "Hello, %s!".formatted(name)
来源：http://zkx.yueranfly.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jdy.wangshuangyany.cn

Ruby: "Hello, #{name}!"
来源：http://dho.sweek.top

C#:   $"Hello, {name}!"
来源：http://anp.yuanzhike.top

[A13] 多行字符串（练习 \n 转义）
来源：http://coa.0kj1m.cn

Py:   "第一行\n第二行"
来源：http://mmc.vqdsnc.cn

PHP:  "第一行\n第二行"
来源：http://rgn.zycfv.cn

JS:   "第一行\n第二行"
来源：http://rwi.quarkkingdee.top

TS:   "第一行\n第二行"
来源：http://etj.hysaishi.cn

Java: "第一行\n第二行"
来源：http://xzx.mhx1999.top

Go:   "第一行\n第二行"
来源：http://knn.cheryme.top

Ruby: "第一行\n第二行"
来源：http://mcz.yonumen.top

C#:   "第一行\n第二行"
来源：http://iwb.yuxming.cn

[A14] 注释写法
来源：http://yli.fzhhl.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ndw.ybcxt.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://poe.xziqi.cn

JS:   // 单行；/* 多行 */
来源：http://afe.xylfe.cn

TS:   // 单行；/* 多行 */
来源：http://qwc.hysaishi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ogl.ivvv.top

Go:   // 单行；/* 多行 */
来源：http://klh.sysykeji.top

Ruby: # 单行；=begin 多行 =end
来源：http://tui.yvedp.cn

C#:   // 单行；/* 多行 */
来源：http://plp.cucudq.cn

[A15] 空值判断与默认值
来源：http://bzt.ppjwa.cn

Py:   value = data or "默认值"
来源：http://igl.cqqwz.cn

PHP:  $value = $data ?? "默认值";
来源：http://eix.vqdsnc.cn

JS:   const value = data ?? "默认值";
来源：http://jgb.svipenyu.cn

TS:   const value = data ?? "默认值";
来源：http://ppn.zdbjq.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mkv.shanyushiyangkeji.top

Go:   if data == "" { data = "默认值" }
来源：http://scw.aibaodan.cn

Ruby: value = data || "默认值"
来源：http://guv.zhiwuduotai.top

C#:   var value = data ?? "默认值";
来源：http://bdn.ctjpmb.com

[A16] 真假值判断规则
来源：http://vqw.pycfn.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rgb.feifeiyinyue.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pvn.daxiang520.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sro.jinqigufen.top

TS:   if (!x) {}
来源：http://aav.xuetiantiany.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pbh.guannengcc.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kpk.tian-w.cn

Ruby: unless x            # nil 与 false 为假
来源：http://eyq.xuanzx.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lso.haohaochexian.top

[A17] 位运算
来源：http://tma.haohaochexian.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dyy.epnwcf.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lvj.zhiwuduotai.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qzj.jinghuilouyu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://crr.ydjk.org.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ynf.zhongyouzk.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mwx.jqgufenzy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zji.jinghuilouyu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.hesvh.cn

[A18] 字符与 ASCII 码互转
来源：http://uxm.zhengqikj.top

Py:   ord("A"); chr(65)
来源：http://mlc.cdnleiting.top

PHP:  ord("A"); chr(65)
来源：http://vzp.shuidangran.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xml.hesvh.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ecb.jqgfzy.top

Java: (int) 'A'; (char) 65
来源：http://wtf.andypj.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kab.yfazqb.com

Ruby: "A".ord; 65.chr
来源：http://toq.sxryk.cn

C#:   (int)'A'; (char)65
来源：http://mrc.dashuyun.cn

[A19] 交换两个变量
来源：http://oxz.9152youxi.cn

Py:   a, b = b, a
来源：http://wzg.xinyue.icu

PHP:  [$a, $b] = [$b, $a];
来源：http://jen.fehbvm.com

JS:   [a, b] = [b, a];
来源：http://rmj.jinqigfzy.top

TS:   [a, b] = [b, a];
来源：http://pry.zhoulong.xyz

Java: int t = a; a = b; b = t;
来源：http://isi.ywan-chungtsiang.top

Go:   a, b = b, a
来源：http://zhg.iojbl.cn

Ruby: a, b = b, a
来源：http://toh.hywenlv.cn

C#:   (a, b) = (b, a);
来源：http://svd.andypj.xyz

[A20] 读取标准输入
来源：http://mqd.ivvv.top

Py:   name = input("请输入：")
来源：http://trs.cheryme.top

PHP:  $name = trim(fgets(STDIN));
来源：http://lhw.chenlongwang.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fmw.tian-w.cn

TS:   // Node.js：readline 模块
来源：http://iol.shanyushiyangkeji.top

Java: new Scanner(System.in).nextLine()
来源：http://vez.vehdjk.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hlr.bjfxy.top

Ruby: gets.chomp
来源：http://ccz.zhoulong.xyz

C#:   Console.ReadLine();
来源：http://ein.yongpay.top

[A21] 保留指定小数位输出
来源：http://ozr.shuidangran.top

Py:   f"{3.14159:.2f}"
来源：http://uem.sjlbkw.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gtd.iojbl.cn

JS:   (3.14159).toFixed(2)
来源：http://nwf.xuetiantiany.cn

TS:   (3.14159).toFixed(2)
来源：http://vww.yanxiufei.cn

Java: String.format("%.2f", 3.14159)
来源：http://wfb.snrcjt.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pww.nanxuanxn.top

Ruby: format("%.2f", 3.14159)
来源：http://eds.wangdashe.top

C#:   3.14159.ToString("F2")
来源：http://vjp.sufxvd.cn

[A22] 获取字符串长度
来源：http://lxs.hcnkem.com

Py:   len(s)
来源：http://pzb.52xcode.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ofs.uphjek.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hqh.52xcode.cn

TS:   s.length
来源：http://plf.52xcode.cn

Java: s.length()
来源：http://uzu.birdmap.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kfo.yfazqb.com

Ruby: s.length
来源：http://iyz.52xcode.cn

C#:   s.Length
来源：http://nyy.andypj.xyz

[A23] 大小写转换
来源：http://goa.vqdsnc.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pur.birdmap.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gwz.fengsongda.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nus.wangshuangyany.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bdc.zdbjq.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hpj.ppjwa.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hjp.gotoacloud.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://iyc.jinghuilouyu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ydo.nanxinkj.top

[A24] 去除首尾空白
来源：http://znf.hywenlv.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rpd.hysaishi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://awz.gzhubu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tkm.jyoumei.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nxr.iojbl.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wby.dianchejie.cn

Go:   strings.TrimSpace(s)
来源：http://tmy.zhaomingkeji.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eqf.xziqi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pls.zhengqikj.top

[A25] 字符串比较
来源：http://cyn.fanxiaobao.xyz

Py:   s1 == s2; s1 != s2
来源：http://iod.redwolf501.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://otk.jinqigufen.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://iqk.aibaodan.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nsl.ctjpmb.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dgf.fehbvm.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ayq.ywan-chungtsiang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://xju.zdqjudy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hby.cheryme.top

[A26] 类型转换总览
来源：http://ykh.yuanzhike.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mvk.feifeiyinyue.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gnt.0kj1m.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ivh.jlsjyb.cn

TS:   Number() String() Boolean() x as number
来源：http://xsl.zhaomingkeji.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://opk.yangfankeji.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cna.tian-w.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rpy.cqqwz.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ats.guowangkeji.top

================================================================================
来源：http://kad.mhx1999.top

B. 流程控制
来源：http://zso.zdbjq.cn

================================================================================
来源：http://zok.yangfankeji.com

[B01] 条件判断 if / else
来源：http://rkg.jianghu66.top

Py:   result = "正" if x > 0 else "非正"
来源：http://lkb.shangyingyoupin.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://itl.shanyushiyangkeji.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vmp.cucudq.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vmf.fengsongda.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://pco.fengsongda.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gpv.nwbrower.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vab.gogol.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jom.zycfv.cn

[B02] 多分支 else if / elif
来源：http://ehi.pycfn.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://weg.cqqwz.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bvw.feifeiyinyue.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://shz.ctjpmb.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://otv.quarkkingdee.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jrr.epnwcf.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kae.zycfv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://odq.fktsv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pwf.gogol.net.cn

[B03] switch / match / case
来源：http://phf.pengpengdd.cyou

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vxa.chenjidiqi.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mdh.hesvh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dra.cqqwz.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://awr.zdqjudy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fqw.zhixingplan.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://keu.yueranfly.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kas.wangdashe.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cfe.fehbvm.com

[B04] for 计数循环
来源：http://muu.sjlbkw.cn

Py:   for i in range(10): print(i)
来源：http://mgm.hnqzz.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uca.chenzaomai.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fej.52xcode.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ixc.nwbrower.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gab.jianghu66.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baf.sufxvd.cn

Ruby: 10.times { |i| puts i }
来源：http://ltq.fktsv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://old.cdnleiting.top

[B05] 遍历数组 / 列表
来源：http://jau.fktsv.cn

Py:   for item in arr: print(item)
来源：http://xfk.wangshuangyany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vmo.redwolf501.top

JS:   for (const item of arr) { console.log(item); }
来源：http://pig.pengpengdd.cyou

TS:   for (const item of arr) { console.log(item); }
来源：http://mlk.ivvv.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fiy.hammf.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tby.cucudq.cn

Ruby: arr.each { |item| puts item }
来源：http://zjq.hammf.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bpn.nwbrower.top

[B06] 遍历字典 / 对象
来源：http://fhl.hnqzz.top

Py:   for k, v in d.items(): print(k, v)
来源：http://dsb.andypj.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zte.jinqigufen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ogf.hysaishi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://err.cheryme.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yyf.bbcook.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ofe.vehdjk.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nit.bjfxy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ema.ydjk.org.cn

[B07] while 循环
来源：http://etw.yfazqb.com

Py:   while i < 10: i += 1
来源：http://fll.yj202588.top

PHP:  while ($i < 10) { $i++; }
来源：http://shl.fengsongda.top

JS:   while (i < 10) { i++; }
来源：http://jor.fehbvm.com

TS:   while (i < 10) { i++; }
来源：http://sxa.ywan-chungtsiang.top

Java: while (i < 10) { i++; }
来源：http://wnx.shzxlz.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://orz.vqdsnc.cn

Ruby: while i < 10; i += 1; end
来源：http://iud.xylfe.cn

C#:   while (i < 10) { i++; }
来源：http://mjt.ehwqpu.com

[B08] do-while（至少执行一次）
来源：http://yjt.yfazqb.com

Py:   # 无 do-while：用 while True + break
来源：http://msa.c1oappe.top

PHP:  do { $i++; } while ($i < 10);
来源：http://hwb.tianlin.xyz

JS:   do { i++; } while (i < 10);
来源：http://bis.svipenyu.cn

TS:   do { i++; } while (i < 10);
来源：http://ipf.snrcjt.cn

Java: do { i++; } while (i < 10);
来源：http://fzi.yj20258.top

Go:   for { i++; if i >= 10 { break } }
来源：http://odi.zhiwuduotai.top

Ruby: begin; i += 1; end while i < 10
来源：http://pwh.aizwys.cn

C#:   do { i++; } while (i < 10);
来源：http://lfb.zycfv.cn

[B09] break 与 continue
来源：http://bts.zhoulong.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://icv.shanyushiyangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nmy.mhx1999.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ynj.nanxuanxn.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rfz.wangdashe.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vud.svipenyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://glc.9152youxi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mjw.mhx1999.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dsp.yuanzhike.top

[B10] 遍历同时拿索引
来源：http://mbd.vqdsnc.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rpd.jlsjyb.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hxl.chenlongwang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hti.iojbl.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://liv.gaohongyu789.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zqb.smart0.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ukh.yfazqb.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kzg.gzhubu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cpc.dashuyun.cn

[B11] 生成数字序列 / 区间
来源：http://cft.fehbvm.com

Py:   list(range(0, 10, 2))
来源：http://ngt.yuanzhike.top

PHP:  range(0, 10, 2);
来源：http://iao.zhiwuduotai.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gxk.yangfankeji.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gus.yuanzhike.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kkw.daria6918.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kut.fktsv.cn

Ruby: (0...10).step(2).to_a
来源：http://wki.xingfuxueyuan.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zwa.cdnleiting.top

[B12] 跳出多层循环
来源：http://ias.havefunace.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://tye.jinqigfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fjx.shangyingyoupin.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fbt.gaohongyu789.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ssn.cucudq.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lmg.wangdashe.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rxm.yanxiufei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cof.zdbjq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ypb.sweek.top

[B13] 判断是否为数字
来源：http://mrt.0kj1m.cn

Py:   isinstance(x, (int, float))
来源：http://gzw.fehbvm.com

PHP:  is_numeric($x)
来源：http://wwl.9152youxi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hyx.fzhhl.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://imn.aibaodan.cn

Java: x instanceof Number
来源：http://jar.hcnkem.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jug.hysaishi.cn

Ruby: x.is_a?(Numeric)
来源：http://ymv.feifeiyinyue.top

C#:   x is int or double or decimal
来源：http://ago.birdmap.top

[B14] 判断值是否在集合内
来源：http://fsd.feifeiyinyue.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aou.gogol.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jjc.tanke756.top

JS:   [1, 2, 3].includes(x)
来源：http://yom.nanxuanxn.top

TS:   [1, 2, 3].includes(x)
来源：http://zqg.hywenlv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sdl.zhengqikj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hpn.shzxlz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kpp.aizwys.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qqw.cucudq.cn

[B15] 布尔运算与取反
来源：http://qmo.yj202588.top

Py:   a and b or not c
来源：http://fse.316326.xyz

PHP:  $a && $b || !$c
来源：http://gko.nanxinkj.top

JS:   a && b || !c
来源：http://cnb.aizwys.cn

TS:   a && b || !c
来源：http://cis.jinqigfzy.top

Java: a && b || !c
来源：http://dos.yangfankeji.com


<!-- 参考信息 -->