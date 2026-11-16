代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://pzh.zhoulong.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://gio.cashguo.top

C#:   x.GetType().Name; x is int
来源：http://gko.daria6918.cn

[A05] 整数除法与取模
来源：http://ygo.guannengcc.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gxc.zhiwuduotai.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://kaz.havefunace.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wqj.aizwys.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lwf.kuanghao11.cn

Java: 7 / 2; 7 % 2
来源：http://zwh.vqdsnc.cn

Go:   7 / 2; 7 % 2
来源：http://okh.xuetiantiany.cn

Ruby: 7 / 2; 7 % 2
来源：http://rpw.wangdashe.top

C#:   7 / 2; 7 % 2
来源：http://qde.daria6918.cn

[A06] 字符串转数字
来源：http://iqd.yj20258.top

Py:   int("42"); float("3.14")
来源：http://buz.ehwqpu.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://whv.0kj1m.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://riy.52xcode.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ing.yj202588.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tkc.haohaochexian.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rhb.hnxiangtu.top

Ruby: "42".to_i; "3.14".to_f
来源：http://gbf.gaohongyu789.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ovp.birdmap.top

[A07] 数字转字符串
来源：http://lpb.wangshuangyany.cn

Py:   str(42)
来源：http://stl.svipenyu.cn

PHP:  (string) 42; strval(42)
来源：http://jnj.cheryme.top

JS:   String(42); (42).toString()
来源：http://pqj.yongpay.top

TS:   String(42)
来源：http://aon.hfpthk.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://kbu.0kj1m.cn

Go:   strconv.Itoa(42)
来源：http://zia.pycfn.com

Ruby: 42.to_s
来源：http://xol.ppjwa.cn

C#:   42.ToString()
来源：http://qav.bjfxy.top

[A08] 取整与四舍五入
来源：http://vbj.xuetiantiany.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ltj.jinqigufen.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://agd.chenjidiqi.icu

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tfn.havefunace.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fwi.yongpay.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lbl.chenjidiqi.icu

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kff.guowangkeji.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://xsy.jinqigfzy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wuq.fehbvm.com

[A09] 绝对值与最大最小值
来源：http://kns.ydzc1.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://stn.hnqzz.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://uzd.yanxiufei.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rsj.xuetiantiany.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hde.yuanzhike.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pkc.sjlbkw.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hfl.wangdashe.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pff.cashguo.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tce.jinqigufen.top

[A10] 生成随机数
来源：http://aar.uphjek.com

Py:   import random; random.randint(1, 100)
来源：http://zfi.c1oappe.top

PHP:  random_int(1, 100);
来源：http://afi.wangdashe.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rva.kuanghao11.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jah.fanxiaobao.xyz

Java: new Random().nextInt(100) + 1
来源：http://imw.haohaochexian.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kbq.c1oappe.top

Ruby: rand(1..100)
来源：http://dyo.zhixingplan.top

C#:   new Random().Next(1, 101)
来源：http://ceo.tian-w.cn

[A11] 条件表达式（三元）
来源：http://lsi.cashguo.top

Py:   "yes" if x > 0 else "no"
来源：http://bmz.tian-w.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jgw.dianchejie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://viu.nanxinkj.top

TS:   x > 0 ? "yes" : "no"
来源：http://jes.shanyushiyangtech.top

Java: x > 0 ? "yes" : "no"
来源：http://vod.0kj1m.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zdz.aibaodan.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rwk.hongshengwenyu.top

C#:   x > 0 ? "yes" : "no"
来源：http://fqe.xylfe.cn

[A12] 字符串插值 / 格式化
来源：http://hpc.aibaodan.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://djx.yvedp.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://oqt.9152youxi.cn

JS:   `Hello, ${name}!`
来源：http://htp.jlsjyb.cn

TS:   `Hello, ${name}!`
来源：http://efh.ywan-chungtsiang.top

Java: "Hello, %s!".formatted(name)
来源：http://wbr.zhiwuduotai.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tjm.tianlin.xyz

Ruby: "Hello, #{name}!"
来源：http://jpz.svipenyu.cn

C#:   $"Hello, {name}!"
来源：http://zfh.hfpthk.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://smt.hcnkem.com

Py:   "第一行\n第二行"
来源：http://ode.jinqigfzy.top

PHP:  "第一行\n第二行"
来源：http://ill.yuxming.cn

JS:   "第一行\n第二行"
来源：http://rvs.bbcook.cn

TS:   "第一行\n第二行"
来源：http://nts.jqgfzy.top

Java: "第一行\n第二行"
来源：http://faf.yj202588.top

Go:   "第一行\n第二行"
来源：http://hwx.shzxlz.cn

Ruby: "第一行\n第二行"
来源：http://qll.fehbvm.com

C#:   "第一行\n第二行"
来源：http://nkw.xziqi.cn

[A14] 注释写法
来源：http://esu.gogol.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://jia.0kj1m.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qiy.jqgufenzy.top

JS:   // 单行；/* 多行 */
来源：http://kkp.gogol.net.cn

TS:   // 单行；/* 多行 */
来源：http://fmp.haohaochexian.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mao.0kj1m.cn

Go:   // 单行；/* 多行 */
来源：http://sso.ywan-chungtsiang.top

Ruby: # 单行；=begin 多行 =end
来源：http://kkc.tarul.cn

C#:   // 单行；/* 多行 */
来源：http://kol.shanyushiyangtech.top

[A15] 空值判断与默认值
来源：http://ddr.yvedp.cn

Py:   value = data or "默认值"
来源：http://tla.wangshuangyany.cn

PHP:  $value = $data ?? "默认值";
来源：http://eax.tianlin.xyz

JS:   const value = data ?? "默认值";
来源：http://ymq.svipenyu.cn

TS:   const value = data ?? "默认值";
来源：http://ced.jinyuanbaomall.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zra.fehbvm.com

Go:   if data == "" { data = "默认值" }
来源：http://tll.tanke756.top

Ruby: value = data || "默认值"
来源：http://xzp.hnqzz.top

C#:   var value = data ?? "默认值";
来源：http://lhp.yj20258.top

[A16] 真假值判断规则
来源：http://ycg.wangshuangyany.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://exf.zhiwuduotai.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kao.zhaomingkeji.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qtk.ivvv.top

TS:   if (!x) {}
来源：http://zhb.chenjidiqi.icu

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gym.ivvv.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://csp.yangfankeji.com

Ruby: unless x            # nil 与 false 为假
来源：http://bbu.hfpthk.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blp.zdbjq.cn

[A17] 位运算
来源：http://gsz.zhoulong.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://efo.zhaomingkeji.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://afa.hesvh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ddq.yongpay.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://guc.dashuyun.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dni.gogol.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hzi.xylfe.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://djo.hcnkem.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gsd.chenjidiqi.icu

[A18] 字符与 ASCII 码互转
来源：http://qjv.guannengcc.top

Py:   ord("A"); chr(65)
来源：http://nak.nanxinkj.top

PHP:  ord("A"); chr(65)
来源：http://ilc.hesvh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wlj.gzhubu.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://doy.redwolf501.top

Java: (int) 'A'; (char) 65
来源：http://cxo.zhoulong.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ejp.gogol.net.cn

Ruby: "A".ord; 65.chr
来源：http://fuv.yfazqb.com

C#:   (int)'A'; (char)65
来源：http://uug.nanxuanxn.top

[A19] 交换两个变量
来源：http://dir.jinghuilouyu.cn

Py:   a, b = b, a
来源：http://jbe.bjfxy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://btj.cdnleiting.top

JS:   [a, b] = [b, a];
来源：http://eot.gzhubu.top

TS:   [a, b] = [b, a];
来源：http://wmn.ppjwa.cn

Java: int t = a; a = b; b = t;
来源：http://ybs.c1oappe.top

Go:   a, b = b, a
来源：http://hfn.cdnleiting.top

Ruby: a, b = b, a
来源：http://vtu.fanxiaobao.xyz

C#:   (a, b) = (b, a);
来源：http://dny.jlsjyb.cn

[A20] 读取标准输入
来源：http://mjp.daria6918.cn

Py:   name = input("请输入：")
来源：http://mpp.nanxuanxn.top

PHP:  $name = trim(fgets(STDIN));
来源：http://eur.jinqigufen.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rsp.jinghuilouyu.cn

TS:   // Node.js：readline 模块
来源：http://pwf.gzhubu.top

Java: new Scanner(System.in).nextLine()
来源：http://eza.guannengcc.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qnw.fktsv.cn

Ruby: gets.chomp
来源：http://onj.yj20258.top

C#:   Console.ReadLine();
来源：http://udx.hnxiangtu.top

[A21] 保留指定小数位输出
来源：http://rif.meibo888.top

Py:   f"{3.14159:.2f}"
来源：http://zvk.9152youxi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ink.quarkkingdee.top

JS:   (3.14159).toFixed(2)
来源：http://qxt.shzxlz.cn

TS:   (3.14159).toFixed(2)
来源：http://qte.316326.xyz

Java: String.format("%.2f", 3.14159)
来源：http://pke.bbcook.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tke.uphjek.com

Ruby: format("%.2f", 3.14159)
来源：http://clh.gaohongyu789.top

C#:   3.14159.ToString("F2")
来源：http://nwg.hnqzz.top

[A22] 获取字符串长度
来源：http://tpo.wangdashe.top

Py:   len(s)
来源：http://jqa.fengsongda.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://imo.meibo888.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xas.jianghu66.top

TS:   s.length
来源：http://ajd.ydjk.org.cn

Java: s.length()
来源：http://mtm.guowangkeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dey.gogol.net.cn

Ruby: s.length
来源：http://mqn.tian-w.cn

C#:   s.Length
来源：http://dzq.yangfankeji.com

[A23] 大小写转换
来源：http://tkx.hnxiangtu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ykc.cashguo.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://agd.gaohongyu789.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rgd.chenjidiqi.icu

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xyn.vqdsnc.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ccf.yvedp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qrd.gaohongyu789.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dkh.jinghuilouyu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wlt.smart0.xyz

[A24] 去除首尾空白
来源：http://ysg.pengpengdd.cyou

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://oww.yj20258888.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://aph.dianchejie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ehz.andypj.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ose.feifeiyinyue.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vvx.bbcook.cn

Go:   strings.TrimSpace(s)
来源：http://rnd.xziqi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fpo.yfazqb.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nja.pengpengdd.cyou

[A25] 字符串比较
来源：http://nqg.zhoulong.xyz

Py:   s1 == s2; s1 != s2
来源：http://nrs.yanxiufei.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://aab.zycfv.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jqi.zhaomingkeji.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dlx.chenjidiqi.icu

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cgj.xingfuxueyuan.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gza.yfazqb.com

Ruby: s1 == s2; s1 <=> s2
来源：http://hov.shanyushiyangtech.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tuw.cucudq.cn

[A26] 类型转换总览
来源：http://ooh.yuxming.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zec.nwbrower.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hda.fktsv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rvw.feifeiyinyue.top

TS:   Number() String() Boolean() x as number
来源：http://fpz.yanxiufei.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://iec.316326.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hhd.aibaodan.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dke.yuanzhike.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nit.tianlin.xyz

================================================================================
来源：http://zjv.xuetiantiany.cn

B. 流程控制
来源：http://yqu.chenjidiqi.icu

================================================================================
来源：http://fet.nwbrower.top

[B01] 条件判断 if / else
来源：http://lns.zhoulong.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://izp.yj20258888.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mln.jinqigfzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://eey.iojbl.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pls.quarkkingdee.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://dco.hywenlv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vpp.bjfxy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://raa.shanyushiyangkeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://awf.ydzc1.top

[B02] 多分支 else if / elif
来源：http://mtu.316326.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dbv.yuanzhike.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fec.jinqigfzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://voz.svipenyu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bpj.jianghu66.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yue.dianchejie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xjr.c1oappe.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wmn.epnwcf.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cpi.yuanzhike.top

[B03] switch / match / case
来源：http://uvd.chenlongwang.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ljw.jinqigfzy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ohz.gaohongyu789.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aze.bbcook.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bsd.chenzaomai.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://olp.chenjidiqi.icu

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zwv.gzhubu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nna.xuetiantiany.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zzm.52xcode.cn

[B04] for 计数循环
来源：http://hlk.sufxvd.cn

Py:   for i in range(10): print(i)
来源：http://ruj.iojbl.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://esr.shzxlz.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bgx.hammf.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://epq.uphjek.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dvk.hfpthk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wpc.haohaochexian.top

Ruby: 10.times { |i| puts i }
来源：http://zrz.tanke756.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yfl.snrcjt.cn

[B05] 遍历数组 / 列表
来源：http://ogq.andypj.xyz

Py:   for item in arr: print(item)
来源：http://iec.birdmap.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dde.jqgufenzy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://igu.tian-w.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://diw.hfpthk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jtt.tanke756.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cuo.yangfankeji.com

Ruby: arr.each { |item| puts item }
来源：http://sgu.0kj1m.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xsv.shanyushiyangtech.top

[B06] 遍历字典 / 对象
来源：http://dsb.quarkkingdee.top

Py:   for k, v in d.items(): print(k, v)
来源：http://jub.0kj1m.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rzr.feifeiyinyue.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ymp.jqgfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dlt.cheryme.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tya.ydzc1.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bpo.yuxming.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dwo.jqgfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://esq.zdqjudy.top

[B07] while 循环
来源：http://llk.shangyingyoupin.top

Py:   while i < 10: i += 1
来源：http://xic.yonumen.top

PHP:  while ($i < 10) { $i++; }
来源：http://vyi.sufxvd.cn

JS:   while (i < 10) { i++; }
来源：http://ahn.epnwcf.com

TS:   while (i < 10) { i++; }
来源：http://qmq.guannengcc.top

Java: while (i < 10) { i++; }
来源：http://kor.quarkkingdee.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://htk.feifeiyinyue.top

Ruby: while i < 10; i += 1; end
来源：http://cxk.svipenyu.cn

C#:   while (i < 10) { i++; }
来源：http://rqg.tanke756.top

[B08] do-while（至少执行一次）
来源：http://igu.daria6918.cn

Py:   # 无 do-while：用 while True + break
来源：http://ohf.xingfuxueyuan.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://ory.tianlin.xyz

JS:   do { i++; } while (i < 10);
来源：http://vfc.sufxvd.cn

TS:   do { i++; } while (i < 10);
来源：http://vuy.gotoacloud.top

Java: do { i++; } while (i < 10);
来源：http://xrc.tianlin.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://fca.gogol.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cry.daria6918.cn

C#:   do { i++; } while (i < 10);
来源：http://waw.shangyingyoupin.top

[B09] break 与 continue
来源：http://ssx.havefunace.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qhp.zhixingplan.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://twh.yj20258.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gif.svipenyu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hlw.0kj1m.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qqg.hesvh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pup.mhx1999.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ekr.epnwcf.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ycp.jiagoushi.top

[B10] 遍历同时拿索引
来源：http://kgn.xuanzx.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://twq.fengsongda.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ieq.daria6918.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wsc.svipenyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rhj.shanyushiyangtech.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wyh.52xcode.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pvp.yj20258.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cuw.cdnleiting.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tmt.daxiang520.top

[B11] 生成数字序列 / 区间
来源：http://qnk.316326.xyz

Py:   list(range(0, 10, 2))
来源：http://sxu.jinghuilouyu.cn

PHP:  range(0, 10, 2);
来源：http://peh.fzhhl.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rsn.nwbrower.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gub.hnxiangtu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gkq.dianchejie.cn


<!-- 参考信息 -->