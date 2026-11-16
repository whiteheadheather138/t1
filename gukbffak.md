代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zme.tian-w.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hft.smart0.xyz

TS:   typeof x; x instanceof Date
来源：http://dgh.fanxiaobao.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rxb.zhijiandao.cn

Go:   reflect.TypeOf(x).Name()
来源：http://sxg.zdqjudy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://uhq.bjfxy.top

C#:   x.GetType().Name; x is int
来源：http://ksg.gzhubu.top

[A05] 整数除法与取模
来源：http://yhw.tian-w.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kwj.zhongyouzk.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://yfv.daria6918.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gkz.jiagoushi.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xfa.dianchejie.cn

Java: 7 / 2; 7 % 2
来源：http://xaf.sweek.top

Go:   7 / 2; 7 % 2
来源：http://pwg.yj20258.top

Ruby: 7 / 2; 7 % 2
来源：http://bth.andypj.xyz

C#:   7 / 2; 7 % 2
来源：http://hqo.jinqigfzy.top

[A06] 字符串转数字
来源：http://pdh.ehwqpu.com

Py:   int("42"); float("3.14")
来源：http://jpi.yfazqb.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zfy.bjfxy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xxu.yuxming.cn

TS:   parseInt("42", 10); Number("42")
来源：http://npc.shuidangran.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://sja.wangshuangyany.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rwh.wangdashe.top

Ruby: "42".to_i; "3.14".to_f
来源：http://jid.jinghuilouyu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kqd.yanxiufei.cn

[A07] 数字转字符串
来源：http://mkd.ctjpmb.com

Py:   str(42)
来源：http://eag.gogol.net.cn

PHP:  (string) 42; strval(42)
来源：http://fml.wangshuangyany.cn

JS:   String(42); (42).toString()
来源：http://ggs.shanyushiyangtech.top

TS:   String(42)
来源：http://gug.316326.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://dxe.havefunace.top

Go:   strconv.Itoa(42)
来源：http://crc.yonumen.top

Ruby: 42.to_s
来源：http://lsh.yanxiufei.cn

C#:   42.ToString()
来源：http://wtk.chenlongwang.top

[A08] 取整与四舍五入
来源：http://esz.sysykeji.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jxm.zycfv.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hjr.yuanzhike.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://djy.zycfv.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nmh.yvedp.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://idj.chenlongwang.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://eps.hnxiangtu.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://zoh.tian-w.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yjj.zycfv.cn

[A09] 绝对值与最大最小值
来源：http://hez.yonumen.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://aua.tianlin.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kiw.svipenyu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gig.zhoulong.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lhk.ydzc1.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ryx.xuanzx.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://auw.wangdashe.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yfu.daxiang520.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ftl.uphjek.com

[A10] 生成随机数
来源：http://qfh.iojbl.cn

Py:   import random; random.randint(1, 100)
来源：http://klq.yonumen.top

PHP:  random_int(1, 100);
来源：http://chz.ybcxt.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mgl.jinqigufen.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xcr.yj20258.top

Java: new Random().nextInt(100) + 1
来源：http://phk.xuanzx.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ocg.daxiang520.top

Ruby: rand(1..100)
来源：http://sqo.fehbvm.com

C#:   new Random().Next(1, 101)
来源：http://sxk.cucudq.cn

[A11] 条件表达式（三元）
来源：http://uyq.ywan-chungtsiang.top

Py:   "yes" if x > 0 else "no"
来源：http://ndh.jianghu66.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://zik.chenzaomai.com

JS:   x > 0 ? "yes" : "no"
来源：http://kbp.shzxlz.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xgp.ywan-chungtsiang.top

Java: x > 0 ? "yes" : "no"
来源：http://haa.dianchejie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://akp.vehdjk.com

Ruby: x > 0 ? "yes" : "no"
来源：http://vrk.pycfn.com

C#:   x > 0 ? "yes" : "no"
来源：http://vhf.uphjek.com

[A12] 字符串插值 / 格式化
来源：http://pwb.guowangkeji.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gyf.daxiang520.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dei.hnxiangtu.top

JS:   `Hello, ${name}!`
来源：http://cvz.xingfuxueyuan.xyz

TS:   `Hello, ${name}!`
来源：http://swf.wangdashe.top

Java: "Hello, %s!".formatted(name)
来源：http://maj.hesvh.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hdz.yj202588.top

Ruby: "Hello, #{name}!"
来源：http://kma.pycfn.com

C#:   $"Hello, {name}!"
来源：http://smt.dianchejie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zac.hywenlv.cn

Py:   "第一行\n第二行"
来源：http://sta.52xcode.cn

PHP:  "第一行\n第二行"
来源：http://esd.hcnkem.com

JS:   "第一行\n第二行"
来源：http://uxp.zhixingplan.top

TS:   "第一行\n第二行"
来源：http://tyv.fengsongda.top

Java: "第一行\n第二行"
来源：http://hvk.gogol.net.cn

Go:   "第一行\n第二行"
来源：http://trp.zhixingplan.top

Ruby: "第一行\n第二行"
来源：http://xjl.zdqjudy.top

C#:   "第一行\n第二行"
来源：http://etl.shzxlz.cn

[A14] 注释写法
来源：http://qqb.redwolf501.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://unf.yangfankeji.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://dxe.snrcjt.cn

JS:   // 单行；/* 多行 */
来源：http://hah.jinqigufen.top

TS:   // 单行；/* 多行 */
来源：http://dwj.daxiang520.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rai.daria6918.cn

Go:   // 单行；/* 多行 */
来源：http://hcd.shzxlz.cn

Ruby: # 单行；=begin 多行 =end
来源：http://gpw.shangyingyoupin.top

C#:   // 单行；/* 多行 */
来源：http://yqt.fanxiaobao.xyz

[A15] 空值判断与默认值
来源：http://bku.yuxming.cn

Py:   value = data or "默认值"
来源：http://gmk.hesvh.cn

PHP:  $value = $data ?? "默认值";
来源：http://pni.andypj.xyz

JS:   const value = data ?? "默认值";
来源：http://gnn.daxiang520.top

TS:   const value = data ?? "默认值";
来源：http://nho.shangyingyoupin.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kfg.ydzc1.top

Go:   if data == "" { data = "默认值" }
来源：http://vgy.epnwcf.com

Ruby: value = data || "默认值"
来源：http://fyx.smart0.xyz

C#:   var value = data ?? "默认值";
来源：http://tnv.fanxiaobao.xyz

[A16] 真假值判断规则
来源：http://gsq.dianchejie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dpu.yangfankeji.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ukv.nwbrower.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uuv.shzxlz.cn

TS:   if (!x) {}
来源：http://hok.xingfuxueyuan.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lfu.shanyushiyangkeji.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wne.yj20258888.top

Ruby: unless x            # nil 与 false 为假
来源：http://ojc.ppjwa.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vgw.hcnkem.com

[A17] 位运算
来源：http://bnw.ivvv.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zog.epnwcf.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uar.shangyingyoupin.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ick.ctjpmb.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zuy.zhijiandao.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eqm.zdbjq.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vee.andypj.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://byf.yj202588.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mci.yfazqb.com

[A18] 字符与 ASCII 码互转
来源：http://tsq.jiagoushi.top

Py:   ord("A"); chr(65)
来源：http://udi.mhx1999.top

PHP:  ord("A"); chr(65)
来源：http://afu.jinghuilouyu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://haj.jyoumei.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://csa.yvedp.cn

Java: (int) 'A'; (char) 65
来源：http://njy.sxryk.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ksz.vehdjk.com

Ruby: "A".ord; 65.chr
来源：http://sam.hcnkem.com

C#:   (int)'A'; (char)65
来源：http://ann.tarul.cn

[A19] 交换两个变量
来源：http://nbi.andypj.xyz

Py:   a, b = b, a
来源：http://awk.zhaomingkeji.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://jch.tian-w.cn

JS:   [a, b] = [b, a];
来源：http://fie.aibaodan.cn

TS:   [a, b] = [b, a];
来源：http://clh.52xcode.cn

Java: int t = a; a = b; b = t;
来源：http://kir.xuanzx.com

Go:   a, b = b, a
来源：http://ctj.shanyushiyangkeji.top

Ruby: a, b = b, a
来源：http://gkb.ctjpmb.com

C#:   (a, b) = (b, a);
来源：http://alk.xylfe.cn

[A20] 读取标准输入
来源：http://pup.ywan-chungtsiang.top

Py:   name = input("请输入：")
来源：http://vap.zhixingplan.top

PHP:  $name = trim(fgets(STDIN));
来源：http://hpp.jinqigufen.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ouv.sweek.top

TS:   // Node.js：readline 模块
来源：http://shb.cucudq.cn

Java: new Scanner(System.in).nextLine()
来源：http://pmp.hongshengwenyu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rda.hongshengwenyu.top

Ruby: gets.chomp
来源：http://kdv.zdbjq.cn

C#:   Console.ReadLine();
来源：http://vij.hongshengwenyu.top

[A21] 保留指定小数位输出
来源：http://viy.vehdjk.com

Py:   f"{3.14159:.2f}"
来源：http://pmr.gogol.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ync.epnwcf.com

JS:   (3.14159).toFixed(2)
来源：http://zgl.jiagoushi.top

TS:   (3.14159).toFixed(2)
来源：http://xgi.yj202588.top

Java: String.format("%.2f", 3.14159)
来源：http://uod.ywan-chungtsiang.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xmb.zycfv.cn

Ruby: format("%.2f", 3.14159)
来源：http://nel.redwolf501.top

C#:   3.14159.ToString("F2")
来源：http://zhe.zdbjq.cn

[A22] 获取字符串长度
来源：http://ghq.fzhhl.top

Py:   len(s)
来源：http://hnl.andypj.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://exy.52xcode.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ffb.nanxinkj.top

TS:   s.length
来源：http://btm.sysykeji.top

Java: s.length()
来源：http://nuc.jinqigfzy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gyt.zhixingplan.top

Ruby: s.length
来源：http://ssm.zhijiandao.cn

C#:   s.Length
来源：http://ekn.chenzaomai.com

[A23] 大小写转换
来源：http://nqs.yj20258888.top

Py:   s.upper(); s.lower(); s.title()
来源：http://qyo.shzxlz.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fvi.sweek.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zcq.zhengqikj.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://iyh.feifeiyinyue.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cbw.jinqigufen.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fga.ydzc1.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ksw.wangshuangyany.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sft.dianchejie.cn

[A24] 去除首尾空白
来源：http://pcu.mhx1999.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tzi.feifeiyinyue.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jhl.hcnkem.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tgk.tianlin.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lbh.yangfankeji.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qmx.yanxiufei.cn

Go:   strings.TrimSpace(s)
来源：http://rlv.hesvh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hpu.fehbvm.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dqn.yonumen.top

[A25] 字符串比较
来源：http://nwr.zdbjq.cn

Py:   s1 == s2; s1 != s2
来源：http://ewt.jinyuanbaomall.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xew.0kj1m.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://aee.vehdjk.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kir.shzxlz.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lut.xuanzx.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jex.epnwcf.com

Ruby: s1 == s2; s1 <=> s2
来源：http://jkz.zhaomingkeji.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://don.hesvh.cn

[A26] 类型转换总览
来源：http://buw.zycfv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cmo.hammf.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ddn.sufxvd.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qkv.sxryk.cn

TS:   Number() String() Boolean() x as number
来源：http://qzf.ppjwa.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sti.hammf.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vfx.gaohongyu789.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://poq.yangfankeji.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cdx.zhongyouzk.top

================================================================================
来源：http://lpg.jyoumei.cn

B. 流程控制
来源：http://xns.ywan-chungtsiang.top

================================================================================
来源：http://mon.ivvv.top

[B01] 条件判断 if / else
来源：http://qeq.gaohongyu789.top

Py:   result = "正" if x > 0 else "非正"
来源：http://fyr.dianchejie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lqh.gogol.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dre.hongshengwenyu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mwu.aizwys.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fvl.jinqigfzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hpc.shangyingyoupin.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://roo.daxiang520.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mxy.ybcxt.top

[B02] 多分支 else if / elif
来源：http://qxy.vqdsnc.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bmx.sxryk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eyn.fzhhl.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wgc.ehwqpu.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jtz.ivvv.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ntp.shanyushiyangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pjg.chenlongwang.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wys.tanke756.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xmp.zhiwuduotai.top

[B03] switch / match / case
来源：http://olg.ivvv.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sse.tanke756.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wza.iojbl.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kxk.ydzc1.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sil.sxryk.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hlq.hfpthk.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fhq.yfazqb.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://enu.zhiwuduotai.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://eoq.tian-w.cn

[B04] for 计数循环
来源：http://sqg.fehbvm.com

Py:   for i in range(10): print(i)
来源：http://jml.jiagoushi.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://knb.52xcode.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://caa.shanyushiyangtech.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ouw.yueranfly.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bez.xinyue.icu

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yuy.ybcxt.top

Ruby: 10.times { |i| puts i }
来源：http://uxa.yj20258.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://goo.fzhhl.top

[B05] 遍历数组 / 列表
来源：http://run.shuidangran.top

Py:   for item in arr: print(item)
来源：http://hgy.shuidangran.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gmi.zycfv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fci.xziqi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cgg.xuetiantiany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rve.vehdjk.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zgj.kuanghao11.cn

Ruby: arr.each { |item| puts item }
来源：http://seu.316326.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://deb.sweek.top

[B06] 遍历字典 / 对象
来源：http://gla.jianghu66.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ihb.cheryme.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zqf.zhiwuduotai.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bsb.jqgufenzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qui.jyoumei.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zkh.yj20258.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://onk.meibo888.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yys.guannengcc.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vyl.jqgfzy.top

[B07] while 循环
来源：http://snt.meibo888.top

Py:   while i < 10: i += 1
来源：http://qqk.fengsongda.top

PHP:  while ($i < 10) { $i++; }
来源：http://xan.yvedp.cn

JS:   while (i < 10) { i++; }
来源：http://rra.pycfn.com

TS:   while (i < 10) { i++; }
来源：http://gdc.ctjpmb.com

Java: while (i < 10) { i++; }
来源：http://lzl.tianlin.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://llt.epnwcf.com

Ruby: while i < 10; i += 1; end
来源：http://otv.gaohongyu789.top

C#:   while (i < 10) { i++; }
来源：http://pmi.hysaishi.cn

[B08] do-while（至少执行一次）
来源：http://dxt.mhx1999.top

Py:   # 无 do-while：用 while True + break
来源：http://qdo.yangfankeji.com

PHP:  do { $i++; } while ($i < 10);
来源：http://zjd.chenjidiqi.icu

JS:   do { i++; } while (i < 10);
来源：http://vfa.shuidangran.top

TS:   do { i++; } while (i < 10);
来源：http://mwt.hongshengwenyu.top

Java: do { i++; } while (i < 10);
来源：http://vrs.0kj1m.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yab.zhiwuduotai.top

Ruby: begin; i += 1; end while i < 10
来源：http://oyb.dashuyun.cn

C#:   do { i++; } while (i < 10);
来源：http://evs.yueranfly.top

[B09] break 与 continue
来源：http://fba.aibaodan.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://elq.guannengcc.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nyt.ydjk.org.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mwm.fengsongda.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://keo.0kj1m.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mza.wangdashe.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qkm.ctjpmb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://snl.havefunace.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rnb.pengpengdd.cyou

[B10] 遍历同时拿索引
来源：http://uun.yueranfly.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kxr.uphjek.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jgm.gaohongyu789.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://myv.hnqzz.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qdo.yonumen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uct.bjfxy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jds.xuetiantiany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ksm.hywenlv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tsc.jyoumei.cn

[B11] 生成数字序列 / 区间
来源：http://phb.yuxming.cn

Py:   list(range(0, 10, 2))
来源：http://hao.chenjidiqi.icu


<!-- 参考信息 -->