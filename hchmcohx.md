代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jss.zhengqikj.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wbv.ybcxt.top

TS:   typeof x; x instanceof Date
来源：http://yly.ivvv.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yie.svipenyu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://smb.shuidangran.top

Ruby: x.class; x.is_a?(Integer)
来源：http://avy.xuetiantiany.cn

C#:   x.GetType().Name; x is int
来源：http://bar.jlsjyb.cn

[A05] 整数除法与取模
来源：http://xpf.hongshengwenyu.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://syd.haohaochexian.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ydk.zhongyouzk.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://njd.zdqjudy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ueo.uphjek.com

Java: 7 / 2; 7 % 2
来源：http://xtz.aizwys.cn

Go:   7 / 2; 7 % 2
来源：http://mse.nanxuanxn.top

Ruby: 7 / 2; 7 % 2
来源：http://xic.jqgufenzy.top

C#:   7 / 2; 7 % 2
来源：http://jro.zhengqikj.top

[A06] 字符串转数字
来源：http://uyv.jinqigufen.top

Py:   int("42"); float("3.14")
来源：http://dmo.zhijiandao.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://atb.vehdjk.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://chb.chenzaomai.com

TS:   parseInt("42", 10); Number("42")
来源：http://gfj.tianlin.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bet.yfazqb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zes.jlsjyb.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://vii.nwbrower.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://npb.zhengqikj.top

[A07] 数字转字符串
来源：http://sth.jqgfzy.top

Py:   str(42)
来源：http://zen.haohaochexian.top

PHP:  (string) 42; strval(42)
来源：http://ymj.gogol.net.cn

JS:   String(42); (42).toString()
来源：http://tmc.ydjk.org.cn

TS:   String(42)
来源：http://gcw.jqgfzy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://mzi.ctjpmb.com

Go:   strconv.Itoa(42)
来源：http://ugy.quarkkingdee.top

Ruby: 42.to_s
来源：http://und.cdnleiting.top

C#:   42.ToString()
来源：http://tdh.chenlongwang.top

[A08] 取整与四舍五入
来源：http://dbw.jqgfzy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://spt.meibo888.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://roj.cashguo.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pvp.jlsjyb.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vgv.zhoulong.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rds.havefunace.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jet.yfazqb.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://znn.0kj1m.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://odh.yongpay.top

[A09] 绝对值与最大最小值
来源：http://bzx.hongshengwenyu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ctb.ehwqpu.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gzv.hywenlv.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mpz.zhongyouzk.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jvv.yj20258.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dzf.fengsongda.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cqi.zhengqikj.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hod.jiagoushi.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sgr.jinyuanbaomall.cn

[A10] 生成随机数
来源：http://uxq.ivvv.top

Py:   import random; random.randint(1, 100)
来源：http://ual.tian-w.cn

PHP:  random_int(1, 100);
来源：http://wxc.0kj1m.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hdz.bjfxy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rcp.shanyushiyangtech.top

Java: new Random().nextInt(100) + 1
来源：http://drz.yfazqb.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bsj.xingfuxueyuan.xyz

Ruby: rand(1..100)
来源：http://pfd.xingfuxueyuan.xyz

C#:   new Random().Next(1, 101)
来源：http://qzt.zhongyouzk.top

[A11] 条件表达式（三元）
来源：http://dkv.yfazqb.com

Py:   "yes" if x > 0 else "no"
来源：http://zaw.jinqigfzy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://iqg.vqdsnc.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fip.hesvh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bsl.tanke756.top

Java: x > 0 ? "yes" : "no"
来源：http://ztq.cdnleiting.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ytx.nwbrower.top

Ruby: x > 0 ? "yes" : "no"
来源：http://wkt.tarul.cn

C#:   x > 0 ? "yes" : "no"
来源：http://kqi.yuxming.cn

[A12] 字符串插值 / 格式化
来源：http://oap.zhijiandao.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rpw.quarkkingdee.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vyo.52xcode.cn

JS:   `Hello, ${name}!`
来源：http://zwu.hnqzz.top

TS:   `Hello, ${name}!`
来源：http://zol.zhiwuduotai.top

Java: "Hello, %s!".formatted(name)
来源：http://phf.ppjwa.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jdc.ehwqpu.com

Ruby: "Hello, #{name}!"
来源：http://dfo.zycfv.cn

C#:   $"Hello, {name}!"
来源：http://uob.c1oappe.top

[A13] 多行字符串（练习 \n 转义）
来源：http://nil.gogol.net.cn

Py:   "第一行\n第二行"
来源：http://aph.xinyue.icu

PHP:  "第一行\n第二行"
来源：http://ejs.yj20258.top

JS:   "第一行\n第二行"
来源：http://smj.cucudq.cn

TS:   "第一行\n第二行"
来源：http://iph.quarkkingdee.top

Java: "第一行\n第二行"
来源：http://hnt.pengpengdd.cyou

Go:   "第一行\n第二行"
来源：http://ixv.chenlongwang.top

Ruby: "第一行\n第二行"
来源：http://wrm.9152youxi.cn

C#:   "第一行\n第二行"
来源：http://ght.xziqi.cn

[A14] 注释写法
来源：http://qet.ybcxt.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://xyr.ctjpmb.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://abq.mhx1999.top

JS:   // 单行；/* 多行 */
来源：http://lru.zhengqikj.top

TS:   // 单行；/* 多行 */
来源：http://nev.fengsongda.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://puf.haohaochexian.top

Go:   // 单行；/* 多行 */
来源：http://ahu.shanyushiyangtech.top

Ruby: # 单行；=begin 多行 =end
来源：http://itc.yangfankeji.com

C#:   // 单行；/* 多行 */
来源：http://tkp.jqgufenzy.top

[A15] 空值判断与默认值
来源：http://odb.birdmap.top

Py:   value = data or "默认值"
来源：http://uhp.jianghu66.top

PHP:  $value = $data ?? "默认值";
来源：http://mxg.bjfxy.top

JS:   const value = data ?? "默认值";
来源：http://ypd.shangyingyoupin.top

TS:   const value = data ?? "默认值";
来源：http://qpo.shangyingyoupin.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rem.fengsongda.top

Go:   if data == "" { data = "默认值" }
来源：http://aqq.nwbrower.top

Ruby: value = data || "默认值"
来源：http://ttn.ppjwa.cn

C#:   var value = data ?? "默认值";
来源：http://vnv.fanxiaobao.xyz

[A16] 真假值判断规则
来源：http://vkq.tian-w.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ggr.zhengqikj.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dgl.cheryme.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dim.zhixingplan.top

TS:   if (!x) {}
来源：http://jbm.aibaodan.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hnu.kuanghao11.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://efc.tarul.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nqf.c1oappe.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kea.aizwys.cn

[A17] 位运算
来源：http://bia.jinqigfzy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kuo.0kj1m.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://giy.pengpengdd.cyou

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zxn.nanxuanxn.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bem.zdqjudy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ykb.daria6918.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hln.gotoacloud.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vaf.cdnleiting.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tcr.shanyushiyangtech.top

[A18] 字符与 ASCII 码互转
来源：http://aua.ydzc1.top

Py:   ord("A"); chr(65)
来源：http://zue.zdbjq.cn

PHP:  ord("A"); chr(65)
来源：http://sve.sxryk.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fbp.jinqigfzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ktv.yuxming.cn

Java: (int) 'A'; (char) 65
来源：http://orf.birdmap.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gfa.xziqi.cn

Ruby: "A".ord; 65.chr
来源：http://qil.zhongyouzk.top

C#:   (int)'A'; (char)65
来源：http://fym.guowangkeji.top

[A19] 交换两个变量
来源：http://xog.shuidangran.top

Py:   a, b = b, a
来源：http://yjw.zdqjudy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://lcb.cheryme.top

JS:   [a, b] = [b, a];
来源：http://gwg.zycfv.cn

TS:   [a, b] = [b, a];
来源：http://kxu.redwolf501.top

Java: int t = a; a = b; b = t;
来源：http://obd.hongshengwenyu.top

Go:   a, b = b, a
来源：http://lkb.aizwys.cn

Ruby: a, b = b, a
来源：http://xja.yuxming.cn

C#:   (a, b) = (b, a);
来源：http://hxf.ywan-chungtsiang.top

[A20] 读取标准输入
来源：http://vns.feifeiyinyue.top

Py:   name = input("请输入：")
来源：http://ofc.kuanghao11.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ozu.sysykeji.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yep.wangdashe.top

TS:   // Node.js：readline 模块
来源：http://niy.chenzaomai.com

Java: new Scanner(System.in).nextLine()
来源：http://jur.ydzc1.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ymu.yuxming.cn

Ruby: gets.chomp
来源：http://fed.jinqigufen.top

C#:   Console.ReadLine();
来源：http://ckh.tian-w.cn

[A21] 保留指定小数位输出
来源：http://sae.tianlin.xyz

Py:   f"{3.14159:.2f}"
来源：http://tbn.zdbjq.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pvr.yfazqb.com

JS:   (3.14159).toFixed(2)
来源：http://xeq.tian-w.cn

TS:   (3.14159).toFixed(2)
来源：http://ccb.wangdashe.top

Java: String.format("%.2f", 3.14159)
来源：http://jat.aizwys.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yyk.hcnkem.com

Ruby: format("%.2f", 3.14159)
来源：http://seq.sufxvd.cn

C#:   3.14159.ToString("F2")
来源：http://svn.chenzaomai.com

[A22] 获取字符串长度
来源：http://xng.shuidangran.top

Py:   len(s)
来源：http://kpy.chenzaomai.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xyk.c1oappe.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://axf.shanyushiyangtech.top

TS:   s.length
来源：http://zfd.gotoacloud.top

Java: s.length()
来源：http://fwz.xylfe.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jsl.havefunace.top

Ruby: s.length
来源：http://our.mhx1999.top

C#:   s.Length
来源：http://qxm.0kj1m.cn

[A23] 大小写转换
来源：http://jmo.zhaomingkeji.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://rde.zhixingplan.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://usk.cheryme.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cdo.ydzc1.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yas.havefunace.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xvs.hysaishi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jtp.uphjek.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ylt.daria6918.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cit.gzhubu.top

[A24] 去除首尾空白
来源：http://exm.jlsjyb.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gnw.xuetiantiany.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sol.ybcxt.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://clx.fanxiaobao.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jsz.zhixingplan.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yqg.xinyue.icu

Go:   strings.TrimSpace(s)
来源：http://elg.316326.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mef.hesvh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://onj.daria6918.cn

[A25] 字符串比较
来源：http://naw.52xcode.cn

Py:   s1 == s2; s1 != s2
来源：http://tkq.kuanghao11.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pqo.mhx1999.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xvc.daxiang520.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nts.fzhhl.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://few.jinghuilouyu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wmn.feifeiyinyue.top

Ruby: s1 == s2; s1 <=> s2
来源：http://taq.fzhhl.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ynv.0kj1m.cn

[A26] 类型转换总览
来源：http://wsv.fzhhl.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ebv.zhengqikj.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pta.hywenlv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xek.vqdsnc.cn

TS:   Number() String() Boolean() x as number
来源：http://nck.nanxinkj.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cyc.kuanghao11.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ynk.zhoulong.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://oln.chenzaomai.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://abd.nanxinkj.top

================================================================================
来源：http://nxg.jyoumei.cn

B. 流程控制
来源：http://oxj.yonumen.top

================================================================================
来源：http://ghm.meibo888.top

[B01] 条件判断 if / else
来源：http://oda.bbcook.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yjh.kuanghao11.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bgm.cucudq.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wuv.yj20258.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qcw.guannengcc.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://abg.zhaomingkeji.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vmz.nanxinkj.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rxl.redwolf501.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hzn.ydzc1.top

[B02] 多分支 else if / elif
来源：http://hpp.birdmap.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ouh.gaohongyu789.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mcx.fzhhl.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fto.jianghu66.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://llg.andypj.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xvd.snrcjt.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sdz.gaohongyu789.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rce.wangshuangyany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xau.ehwqpu.com

[B03] switch / match / case
来源：http://ysq.sweek.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://iox.0kj1m.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ffo.sufxvd.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dod.jinghuilouyu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qiu.mhx1999.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hkh.gaohongyu789.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://feg.sxryk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ofv.ppjwa.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vst.yj202588.top

[B04] for 计数循环
来源：http://orr.zdqjudy.top

Py:   for i in range(10): print(i)
来源：http://fzg.chenlongwang.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ldk.havefunace.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ikr.ydzc1.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://imw.chenlongwang.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qkn.zdqjudy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uwl.dianchejie.cn

Ruby: 10.times { |i| puts i }
来源：http://sgi.hcnkem.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hif.tanke756.top

[B05] 遍历数组 / 列表
来源：http://eap.kuanghao11.cn

Py:   for item in arr: print(item)
来源：http://vyc.quarkkingdee.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qsu.dianchejie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hkt.zhiwuduotai.top

TS:   for (const item of arr) { console.log(item); }
来源：http://zqr.uphjek.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://qtd.hnqzz.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blq.cqqwz.cn

Ruby: arr.each { |item| puts item }
来源：http://wzn.yangfankeji.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xxs.hywenlv.cn

[B06] 遍历字典 / 对象
来源：http://cll.yonumen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://fpn.tarul.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qcf.ybcxt.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lnl.svipenyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://laa.hywenlv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ufi.dashuyun.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bps.ydjk.org.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qbi.yueranfly.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tyr.xuanzx.com

[B07] while 循环
来源：http://ska.jinghuilouyu.cn

Py:   while i < 10: i += 1
来源：http://nhy.uphjek.com

PHP:  while ($i < 10) { $i++; }
来源：http://ega.zycfv.cn

JS:   while (i < 10) { i++; }
来源：http://vhv.shanyushiyangkeji.top

TS:   while (i < 10) { i++; }
来源：http://rte.zhaomingkeji.xyz

Java: while (i < 10) { i++; }
来源：http://uie.uphjek.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://buc.jinyuanbaomall.cn

Ruby: while i < 10; i += 1; end
来源：http://vcs.yonumen.top

C#:   while (i < 10) { i++; }
来源：http://zcy.wangdashe.top

[B08] do-while（至少执行一次）
来源：http://rjg.shangyingyoupin.top

Py:   # 无 do-while：用 while True + break
来源：http://ckh.sjlbkw.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fup.gotoacloud.top

JS:   do { i++; } while (i < 10);
来源：http://rbl.mhx1999.top

TS:   do { i++; } while (i < 10);
来源：http://ics.yfazqb.com

Java: do { i++; } while (i < 10);
来源：http://riy.svipenyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jpl.tianlin.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://otu.hysaishi.cn

C#:   do { i++; } while (i < 10);
来源：http://dqa.tanke756.top

[B09] break 与 continue
来源：http://dfl.hysaishi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uus.fktsv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://snu.xuetiantiany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ydc.smart0.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pac.zdbjq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tcj.yvedp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cfx.birdmap.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xpz.yvedp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://krb.guannengcc.top

[B10] 遍历同时拿索引
来源：http://iut.snrcjt.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://keb.0kj1m.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rcj.hysaishi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hkn.dashuyun.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ihv.pycfn.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ivk.yvedp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gnk.vqdsnc.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qex.jinqigufen.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gvd.zhengqikj.top

[B11] 生成数字序列 / 区间
来源：http://aiz.hfpthk.cn

Py:   list(range(0, 10, 2))
来源：http://lxr.ybcxt.top


<!-- 参考信息 -->