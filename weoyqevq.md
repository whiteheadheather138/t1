代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://hdo.hesvh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://jzh.uphjek.com

C#:   x.GetType().Name; x is int
来源：http://vep.tanke756.top

[A05] 整数除法与取模
来源：http://yvc.jqgufenzy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hvu.sufxvd.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://urc.c1oappe.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://usf.yangfankeji.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lac.vqdsnc.cn

Java: 7 / 2; 7 % 2
来源：http://gem.shangyingyoupin.top

Go:   7 / 2; 7 % 2
来源：http://sqt.zycfv.cn

Ruby: 7 / 2; 7 % 2
来源：http://axl.jianghu66.top

C#:   7 / 2; 7 % 2
来源：http://vtk.nanxinkj.top

[A06] 字符串转数字
来源：http://grl.ppjwa.cn

Py:   int("42"); float("3.14")
来源：http://tdw.yuanzhike.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fon.fehbvm.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rtt.bbcook.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wcr.ydjk.org.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tgo.aibaodan.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hrb.hongshengwenyu.top

Ruby: "42".to_i; "3.14".to_f
来源：http://rdb.ehwqpu.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://spe.andypj.xyz

[A07] 数字转字符串
来源：http://hdc.ivvv.top

Py:   str(42)
来源：http://qck.tian-w.cn

PHP:  (string) 42; strval(42)
来源：http://nof.dianchejie.cn

JS:   String(42); (42).toString()
来源：http://wza.gogol.net.cn

TS:   String(42)
来源：http://rwm.daria6918.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ren.snrcjt.cn

Go:   strconv.Itoa(42)
来源：http://ems.9152youxi.cn

Ruby: 42.to_s
来源：http://dre.hnxiangtu.top

C#:   42.ToString()
来源：http://gbd.52xcode.cn

[A08] 取整与四舍五入
来源：http://vrw.wangdashe.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yhd.dianchejie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ven.yuanzhike.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ple.gzhubu.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gtr.yongpay.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://axe.ybcxt.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bll.gogol.net.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ski.hywenlv.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cqc.shanyushiyangkeji.top

[A09] 绝对值与最大最小值
来源：http://swb.nwbrower.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fai.ivvv.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xxv.sweek.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jfi.xylfe.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ecl.hongshengwenyu.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nzz.yangfankeji.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pcs.shanyushiyangtech.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hyw.xziqi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fec.havefunace.top

[A10] 生成随机数
来源：http://aov.jyoumei.cn

Py:   import random; random.randint(1, 100)
来源：http://jua.yongpay.top

PHP:  random_int(1, 100);
来源：http://kgw.jqgfzy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://snf.jlsjyb.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://eob.nwbrower.top

Java: new Random().nextInt(100) + 1
来源：http://svn.zhaomingkeji.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://iti.ppjwa.cn

Ruby: rand(1..100)
来源：http://prl.jlsjyb.cn

C#:   new Random().Next(1, 101)
来源：http://vzz.shangyingyoupin.top

[A11] 条件表达式（三元）
来源：http://fti.pengpengdd.cyou

Py:   "yes" if x > 0 else "no"
来源：http://smz.aibaodan.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://lpv.aizwys.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yjj.pycfn.com

TS:   x > 0 ? "yes" : "no"
来源：http://xmn.jinqigfzy.top

Java: x > 0 ? "yes" : "no"
来源：http://uic.ydzc1.top

Go:   // 无三元运算符，需用 if 语句
来源：http://rkf.sufxvd.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vgi.vehdjk.com

C#:   x > 0 ? "yes" : "no"
来源：http://wvv.yj202588.top

[A12] 字符串插值 / 格式化
来源：http://lrx.jyoumei.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://evx.tianlin.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://iox.guannengcc.top

JS:   `Hello, ${name}!`
来源：http://hqq.dashuyun.cn

TS:   `Hello, ${name}!`
来源：http://xzv.jinqigfzy.top

Java: "Hello, %s!".formatted(name)
来源：http://vbk.zhaomingkeji.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mdu.52xcode.cn

Ruby: "Hello, #{name}!"
来源：http://nbl.bjfxy.top

C#:   $"Hello, {name}!"
来源：http://ifv.hywenlv.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://acr.pycfn.com

Py:   "第一行\n第二行"
来源：http://jkr.shangyingyoupin.top

PHP:  "第一行\n第二行"
来源：http://gna.0kj1m.cn

JS:   "第一行\n第二行"
来源：http://bfu.chenzaomai.com

TS:   "第一行\n第二行"
来源：http://cht.yj20258888.top

Java: "第一行\n第二行"
来源：http://teu.jiagoushi.top

Go:   "第一行\n第二行"
来源：http://nau.andypj.xyz

Ruby: "第一行\n第二行"
来源：http://bmj.cheryme.top

C#:   "第一行\n第二行"
来源：http://yra.jianghu66.top

[A14] 注释写法
来源：http://muo.svipenyu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wiz.yj20258.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://vfr.birdmap.top

JS:   // 单行；/* 多行 */
来源：http://yvn.nwbrower.top

TS:   // 单行；/* 多行 */
来源：http://fau.jiagoushi.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lid.gotoacloud.top

Go:   // 单行；/* 多行 */
来源：http://ghs.shanyushiyangtech.top

Ruby: # 单行；=begin 多行 =end
来源：http://uzf.cashguo.top

C#:   // 单行；/* 多行 */
来源：http://lbx.ywan-chungtsiang.top

[A15] 空值判断与默认值
来源：http://bmy.xylfe.cn

Py:   value = data or "默认值"
来源：http://ede.shanyushiyangkeji.top

PHP:  $value = $data ?? "默认值";
来源：http://lec.hysaishi.cn

JS:   const value = data ?? "默认值";
来源：http://asc.cucudq.cn

TS:   const value = data ?? "默认值";
来源：http://qdc.zhixingplan.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mux.yj20258.top

Go:   if data == "" { data = "默认值" }
来源：http://sbq.hcnkem.com

Ruby: value = data || "默认值"
来源：http://ocf.tanke756.top

C#:   var value = data ?? "默认值";
来源：http://tnj.yongpay.top

[A16] 真假值判断规则
来源：http://jrr.zhoulong.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zer.zhongyouzk.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zvk.cqqwz.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rbd.fktsv.cn

TS:   if (!x) {}
来源：http://kwx.uphjek.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fbb.gotoacloud.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://daq.hysaishi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://met.hnxiangtu.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zay.9152youxi.cn

[A17] 位运算
来源：http://lua.xingfuxueyuan.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lfl.vehdjk.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dqu.ydjk.org.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://giv.haohaochexian.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dzd.ivvv.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tfa.jinghuilouyu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wtw.feifeiyinyue.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://szn.xuanzx.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dmk.havefunace.top

[A18] 字符与 ASCII 码互转
来源：http://wlg.ydzc1.top

Py:   ord("A"); chr(65)
来源：http://jza.cdnleiting.top

PHP:  ord("A"); chr(65)
来源：http://xqr.guannengcc.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sur.xinyue.icu

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vaf.bbcook.cn

Java: (int) 'A'; (char) 65
来源：http://xho.pycfn.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ojs.daxiang520.top

Ruby: "A".ord; 65.chr
来源：http://tnl.sysykeji.top

C#:   (int)'A'; (char)65
来源：http://xjk.nwbrower.top

[A19] 交换两个变量
来源：http://ihm.xingfuxueyuan.xyz

Py:   a, b = b, a
来源：http://jrx.tanke756.top

PHP:  [$a, $b] = [$b, $a];
来源：http://jko.fanxiaobao.xyz

JS:   [a, b] = [b, a];
来源：http://fyl.zhengqikj.top

TS:   [a, b] = [b, a];
来源：http://wcl.hywenlv.cn

Java: int t = a; a = b; b = t;
来源：http://loc.hysaishi.cn

Go:   a, b = b, a
来源：http://nri.xylfe.cn

Ruby: a, b = b, a
来源：http://kzv.yuxming.cn

C#:   (a, b) = (b, a);
来源：http://izh.andypj.xyz

[A20] 读取标准输入
来源：http://ypl.pengpengdd.cyou

Py:   name = input("请输入：")
来源：http://swh.dianchejie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://sym.tianlin.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xjk.aizwys.cn

TS:   // Node.js：readline 模块
来源：http://wjd.iojbl.cn

Java: new Scanner(System.in).nextLine()
来源：http://ect.pycfn.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tvi.bbcook.cn

Ruby: gets.chomp
来源：http://aqi.xuetiantiany.cn

C#:   Console.ReadLine();
来源：http://clg.hammf.cn

[A21] 保留指定小数位输出
来源：http://gfp.sjlbkw.cn

Py:   f"{3.14159:.2f}"
来源：http://snn.chenzaomai.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qjp.tianlin.xyz

JS:   (3.14159).toFixed(2)
来源：http://pmx.xylfe.cn

TS:   (3.14159).toFixed(2)
来源：http://saw.yuxming.cn

Java: String.format("%.2f", 3.14159)
来源：http://fst.shzxlz.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yev.iojbl.cn

Ruby: format("%.2f", 3.14159)
来源：http://dez.yonumen.top

C#:   3.14159.ToString("F2")
来源：http://xwr.guowangkeji.top

[A22] 获取字符串长度
来源：http://kyi.epnwcf.com

Py:   len(s)
来源：http://lai.yuanzhike.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zul.nanxuanxn.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tbh.daria6918.cn

TS:   s.length
来源：http://okn.cucudq.cn

Java: s.length()
来源：http://hsc.cucudq.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zyd.tanke756.top

Ruby: s.length
来源：http://lmd.fanxiaobao.xyz

C#:   s.Length
来源：http://ypn.fehbvm.com

[A23] 大小写转换
来源：http://ffu.jqgfzy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://nfq.ppjwa.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fkx.svipenyu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lug.jiagoushi.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://eoy.fehbvm.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qzz.zhijiandao.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wse.xylfe.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://joa.daria6918.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zfm.shanyushiyangtech.top

[A24] 去除首尾空白
来源：http://cts.snrcjt.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fys.mhx1999.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nkr.c1oappe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://acz.nanxuanxn.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oyb.cqqwz.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pbp.gotoacloud.top

Go:   strings.TrimSpace(s)
来源：http://bpl.chenjidiqi.icu

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://umn.uphjek.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tqs.gzhubu.top

[A25] 字符串比较
来源：http://cfn.hcnkem.com

Py:   s1 == s2; s1 != s2
来源：http://crb.smart0.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blm.jyoumei.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://efr.haohaochexian.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yfg.uphjek.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://twb.andypj.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://izw.ctjpmb.com

Ruby: s1 == s2; s1 <=> s2
来源：http://nwu.smart0.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mhd.uphjek.com

[A26] 类型转换总览
来源：http://ubq.cashguo.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jzb.havefunace.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tic.ybcxt.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tyq.xziqi.cn

TS:   Number() String() Boolean() x as number
来源：http://htb.ppjwa.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vge.shuidangran.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nfr.chenlongwang.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://bhh.jianghu66.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lep.daxiang520.top

================================================================================
来源：http://bna.hcnkem.com

B. 流程控制
来源：http://cjk.sweek.top

================================================================================
来源：http://emn.jyoumei.cn

[B01] 条件判断 if / else
来源：http://psm.zycfv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vuw.smart0.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://trl.aizwys.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ktv.zhaomingkeji.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ygp.fehbvm.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://aah.zycfv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uke.cqqwz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://klg.sweek.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jfr.fktsv.cn

[B02] 多分支 else if / elif
来源：http://eiu.gogol.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hhd.zdqjudy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wlt.shzxlz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ghr.yuanzhike.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rpq.cashguo.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kha.ybcxt.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iwn.fanxiaobao.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mtm.yvedp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dqm.316326.xyz

[B03] switch / match / case
来源：http://jzw.jinqigufen.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qoa.pycfn.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://eps.bbcook.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vln.jyoumei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bhi.jinyuanbaomall.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wmh.fanxiaobao.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://psb.nwbrower.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nsb.yanxiufei.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rzt.dianchejie.cn

[B04] for 计数循环
来源：http://ijb.tian-w.cn

Py:   for i in range(10): print(i)
来源：http://ead.yueranfly.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vah.hywenlv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eul.gzhubu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uix.316326.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wwl.ehwqpu.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dvx.pengpengdd.cyou

Ruby: 10.times { |i| puts i }
来源：http://cym.shanyushiyangtech.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zbc.sufxvd.cn

[B05] 遍历数组 / 列表
来源：http://oxu.fehbvm.com

Py:   for item in arr: print(item)
来源：http://lay.zhongyouzk.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qoz.cucudq.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qja.ppjwa.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wmd.yuanzhike.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wzd.snrcjt.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rnq.zdqjudy.top

Ruby: arr.each { |item| puts item }
来源：http://rpy.hfpthk.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pji.nanxinkj.top

[B06] 遍历字典 / 对象
来源：http://hof.ywan-chungtsiang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ycv.cheryme.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qmo.tanke756.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xau.ctjpmb.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jfp.yj202588.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dxh.yongpay.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://khj.jinqigfzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kmk.zhoulong.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://olg.jinqigfzy.top

[B07] while 循环
来源：http://krx.xuetiantiany.cn

Py:   while i < 10: i += 1
来源：http://oxq.bbcook.cn

PHP:  while ($i < 10) { $i++; }
来源：http://aly.jqgfzy.top

JS:   while (i < 10) { i++; }
来源：http://xue.fzhhl.top

TS:   while (i < 10) { i++; }
来源：http://jyf.hfpthk.cn

Java: while (i < 10) { i++; }
来源：http://awt.fktsv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lut.xingfuxueyuan.xyz

Ruby: while i < 10; i += 1; end
来源：http://plu.shanyushiyangtech.top

C#:   while (i < 10) { i++; }
来源：http://vsl.xylfe.cn

[B08] do-while（至少执行一次）
来源：http://aji.jinqigfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://zxy.shuidangran.top

PHP:  do { $i++; } while ($i < 10);
来源：http://wxq.pengpengdd.cyou

JS:   do { i++; } while (i < 10);
来源：http://qyy.nwbrower.top

TS:   do { i++; } while (i < 10);
来源：http://rsn.kuanghao11.cn

Java: do { i++; } while (i < 10);
来源：http://uoy.guowangkeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://opy.gogol.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ote.jinqigufen.top

C#:   do { i++; } while (i < 10);
来源：http://rpj.smart0.xyz

[B09] break 与 continue
来源：http://vbt.yfazqb.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fzn.guannengcc.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cvf.quarkkingdee.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qnl.svipenyu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://del.fengsongda.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cqh.hnxiangtu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://drt.xziqi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://awr.chenzaomai.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iyh.nanxinkj.top

[B10] 遍历同时拿索引
来源：http://sjy.xinyue.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ugc.yfazqb.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tvl.bbcook.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://iff.jyoumei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oqp.chenlongwang.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yjj.nwbrower.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vib.fanxiaobao.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mif.ctjpmb.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nor.jqgufenzy.top

[B11] 生成数字序列 / 区间
来源：http://lib.yj20258.top

Py:   list(range(0, 10, 2))
来源：http://ahp.xziqi.cn

PHP:  range(0, 10, 2);
来源：http://sgo.316326.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dfx.xuanzx.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dqp.gaohongyu789.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xfv.zhaomingkeji.xyz


<!-- 参考信息 -->