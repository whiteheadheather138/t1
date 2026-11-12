代发 wailian999

[A06] 字符串转数字
来源：http://hre.jinghuilouyu.cn

Py:   int("42"); float("3.14")
来源：http://gen.gaohongyu789.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fkm.sweek.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ltm.xingfuxueyuan.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://xmo.guowangkeji.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://koi.daria6918.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ccx.hywenlv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://sew.gotoacloud.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://eoy.yanxiufei.cn

[A07] 数字转字符串
来源：http://hmm.hnxiangtu.top

Py:   str(42)
来源：http://awu.chenzaomai.com

PHP:  (string) 42; strval(42)
来源：http://rpl.sysykeji.top

JS:   String(42); (42).toString()
来源：http://zwg.ybcxt.top

TS:   String(42)
来源：http://irx.guannengcc.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ssj.smart0.xyz

Go:   strconv.Itoa(42)
来源：http://wlh.chenjidiqi.icu

Ruby: 42.to_s
来源：http://jmf.vehdjk.com

C#:   42.ToString()
来源：http://mjy.haohaochexian.top

[A08] 取整与四舍五入
来源：http://zti.xinyue.icu

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ozf.nanxinkj.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://huv.ivvv.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xjz.zhaomingkeji.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://roz.yj20258888.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sjo.hfpthk.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pnf.hcnkem.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://pez.gogol.net.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vuj.yj20258.top

[A09] 绝对值与最大最小值
来源：http://hqc.aibaodan.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://atg.yj202588.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gqv.aibaodan.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tai.epnwcf.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xqi.ivvv.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ppc.sjlbkw.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mqe.hcnkem.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pko.bjfxy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bpo.xziqi.cn

[A10] 生成随机数
来源：http://mxn.zhengqikj.top

Py:   import random; random.randint(1, 100)
来源：http://kld.xylfe.cn

PHP:  random_int(1, 100);
来源：http://vtj.zhixingplan.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pzi.chenjidiqi.icu

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ghd.haohaochexian.top

Java: new Random().nextInt(100) + 1
来源：http://lgl.yj20258888.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qzl.shzxlz.cn

Ruby: rand(1..100)
来源：http://ygd.meibo888.top

C#:   new Random().Next(1, 101)
来源：http://xbl.sufxvd.cn

[A11] 条件表达式（三元）
来源：http://bqc.xingfuxueyuan.xyz

Py:   "yes" if x > 0 else "no"
来源：http://yvn.haohaochexian.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://szd.pengpengdd.cyou

JS:   x > 0 ? "yes" : "no"
来源：http://hqj.zdqjudy.top

TS:   x > 0 ? "yes" : "no"
来源：http://vdk.cucudq.cn

Java: x > 0 ? "yes" : "no"
来源：http://xpu.shanyushiyangtech.top

Go:   // 无三元运算符，需用 if 语句
来源：http://hli.yfazqb.com

Ruby: x > 0 ? "yes" : "no"
来源：http://yuc.fzhhl.top

C#:   x > 0 ? "yes" : "no"
来源：http://cce.bbcook.cn

[A12] 字符串插值 / 格式化
来源：http://edh.hammf.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://swx.dianchejie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://opv.shanyushiyangtech.top

JS:   `Hello, ${name}!`
来源：http://rpp.zycfv.cn

TS:   `Hello, ${name}!`
来源：http://yzb.0kj1m.cn

Java: "Hello, %s!".formatted(name)
来源：http://chq.daxiang520.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zka.yueranfly.top

Ruby: "Hello, #{name}!"
来源：http://ood.yueranfly.top

C#:   $"Hello, {name}!"
来源：http://ylb.c1oappe.top

[A13] 多行字符串（练习 \n 转义）
来源：http://vrp.nanxinkj.top

Py:   "第一行\n第二行"
来源：http://jea.jinqigfzy.top

PHP:  "第一行\n第二行"
来源：http://mof.hnqzz.top

JS:   "第一行\n第二行"
来源：http://waj.chenjidiqi.icu

TS:   "第一行\n第二行"
来源：http://egn.shanyushiyangtech.top

Java: "第一行\n第二行"
来源：http://azq.aizwys.cn

Go:   "第一行\n第二行"
来源：http://syn.jianghu66.top

Ruby: "第一行\n第二行"
来源：http://ias.ybcxt.top

C#:   "第一行\n第二行"
来源：http://gro.yangfankeji.com

[A14] 注释写法
来源：http://deg.cdnleiting.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://aax.xziqi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zir.yonumen.top

JS:   // 单行；/* 多行 */
来源：http://nfz.haohaochexian.top

TS:   // 单行；/* 多行 */
来源：http://uea.gaohongyu789.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mse.tanke756.top

Go:   // 单行；/* 多行 */
来源：http://wlk.daxiang520.top

Ruby: # 单行；=begin 多行 =end
来源：http://hcx.zhongyouzk.top

C#:   // 单行；/* 多行 */
来源：http://hab.meibo888.top

[A15] 空值判断与默认值
来源：http://vsh.cucudq.cn

Py:   value = data or "默认值"
来源：http://ddi.aibaodan.cn

PHP:  $value = $data ?? "默认值";
来源：http://uvu.chenzaomai.com

JS:   const value = data ?? "默认值";
来源：http://vtv.sjlbkw.cn

TS:   const value = data ?? "默认值";
来源：http://qlc.aizwys.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hmu.vehdjk.com

Go:   if data == "" { data = "默认值" }
来源：http://kzt.birdmap.top

Ruby: value = data || "默认值"
来源：http://lyx.gotoacloud.top

C#:   var value = data ?? "默认值";
来源：http://vrt.dianchejie.cn

[A16] 真假值判断规则
来源：http://xrp.ehwqpu.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hzx.jinghuilouyu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lwq.jqgufenzy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://olb.hammf.cn

TS:   if (!x) {}
来源：http://ezs.xinyue.icu

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bvl.xuanzx.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ztk.sufxvd.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hpz.andypj.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zxz.nanxuanxn.top

[A17] 位运算
来源：http://pvw.svipenyu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://krq.kuanghao11.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://icj.hongshengwenyu.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ktg.cucudq.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ide.cheryme.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nab.9152youxi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lpy.yuanzhike.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jgp.aizwys.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ezr.ctjpmb.com

[A18] 字符与 ASCII 码互转
来源：http://onc.sysykeji.top

Py:   ord("A"); chr(65)
来源：http://hqt.nanxinkj.top

PHP:  ord("A"); chr(65)
来源：http://ojs.uphjek.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pds.zhiwuduotai.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xdg.pycfn.com

Java: (int) 'A'; (char) 65
来源：http://inr.xinyue.icu

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mtq.gzhubu.top

Ruby: "A".ord; 65.chr
来源：http://zej.fengsongda.top

C#:   (int)'A'; (char)65
来源：http://qng.0kj1m.cn

[A19] 交换两个变量
来源：http://xwo.yfazqb.com

Py:   a, b = b, a
来源：http://fuv.tanke756.top

PHP:  [$a, $b] = [$b, $a];
来源：http://rxb.cdnleiting.top

JS:   [a, b] = [b, a];
来源：http://rut.gaohongyu789.top

TS:   [a, b] = [b, a];
来源：http://cob.cdnleiting.top

Java: int t = a; a = b; b = t;
来源：http://hqp.shanyushiyangtech.top

Go:   a, b = b, a
来源：http://ftl.havefunace.top

Ruby: a, b = b, a
来源：http://eew.dianchejie.cn

C#:   (a, b) = (b, a);
来源：http://ica.hfpthk.cn

[A20] 读取标准输入
来源：http://vom.shanyushiyangtech.top

Py:   name = input("请输入：")
来源：http://iff.jlsjyb.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hhj.yonumen.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zmy.iojbl.cn

TS:   // Node.js：readline 模块
来源：http://zcm.dashuyun.cn

Java: new Scanner(System.in).nextLine()
来源：http://jsy.fengsongda.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dwu.hesvh.cn

Ruby: gets.chomp
来源：http://cqy.zhiwuduotai.top

C#:   Console.ReadLine();
来源：http://zgx.jinqigufen.top

[A21] 保留指定小数位输出
来源：http://qlw.zycfv.cn

Py:   f"{3.14159:.2f}"
来源：http://tmw.iojbl.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qdz.ctjpmb.com

JS:   (3.14159).toFixed(2)
来源：http://toh.chenzaomai.com

TS:   (3.14159).toFixed(2)
来源：http://cyl.ydjk.org.cn

Java: String.format("%.2f", 3.14159)
来源：http://utx.ivvv.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pov.tanke756.top

Ruby: format("%.2f", 3.14159)
来源：http://yyp.tarul.cn

C#:   3.14159.ToString("F2")
来源：http://vqo.iojbl.cn

[A22] 获取字符串长度
来源：http://plt.aibaodan.cn

Py:   len(s)
来源：http://sxx.sweek.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://egf.shanyushiyangtech.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ijm.guowangkeji.top

TS:   s.length
来源：http://pys.xziqi.cn

Java: s.length()
来源：http://mtj.chenzaomai.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zsg.yueranfly.top

Ruby: s.length
来源：http://qdh.shzxlz.cn

C#:   s.Length
来源：http://lox.shzxlz.cn

[A23] 大小写转换
来源：http://gbz.pycfn.com

Py:   s.upper(); s.lower(); s.title()
来源：http://tbh.cheryme.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bjd.316326.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xwd.chenzaomai.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://suw.mhx1999.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bfx.yj20258888.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cgd.meibo888.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ffg.ppjwa.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://abg.yongpay.top

[A24] 去除首尾空白
来源：http://nir.cqqwz.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ugs.ctjpmb.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ylc.epnwcf.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://quj.zhijiandao.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://syx.yj20258.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ksr.sysykeji.top

Go:   strings.TrimSpace(s)
来源：http://jca.shuidangran.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cyb.52xcode.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cvk.cdnleiting.top

[A25] 字符串比较
来源：http://aln.yj20258888.top

Py:   s1 == s2; s1 != s2
来源：http://sgk.ybcxt.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pmf.guannengcc.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fpn.xingfuxueyuan.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lnv.zhengqikj.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cgd.xziqi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nao.andypj.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://kro.jqgfzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vfe.aibaodan.cn

[A26] 类型转换总览
来源：http://ptd.xinyue.icu

Py:   int() float() str() bool() list() dict() tuple()
来源：http://eqk.yj20258888.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qgw.quarkkingdee.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yzu.tarul.cn

TS:   Number() String() Boolean() x as number
来源：http://sca.yj20258888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dvl.yj20258888.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qkr.chenlongwang.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://syi.hongshengwenyu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://iit.gotoacloud.top

================================================================================
来源：http://kfv.guannengcc.top

B. 流程控制
来源：http://nlh.zdbjq.cn

================================================================================
来源：http://psy.yvedp.cn

[B01] 条件判断 if / else
来源：http://sfv.yfazqb.com

Py:   result = "正" if x > 0 else "非正"
来源：http://rsy.ppjwa.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cll.sweek.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jet.hesvh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ykl.nanxuanxn.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://lzl.jyoumei.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://exp.quarkkingdee.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pit.fengsongda.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ohz.zhengqikj.top

[B02] 多分支 else if / elif
来源：http://kow.fktsv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hbb.snrcjt.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://loz.hnxiangtu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bzr.aibaodan.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zic.zhiwuduotai.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lqc.nwbrower.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jqu.iojbl.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bcb.quarkkingdee.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lea.hnxiangtu.top

[B03] switch / match / case
来源：http://pzh.aibaodan.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jtj.ydzc1.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://psb.fzhhl.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://flu.chenlongwang.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wni.hfpthk.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ian.vehdjk.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yqb.daria6918.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ave.sjlbkw.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bhn.xylfe.cn

[B04] for 计数循环
来源：http://moa.havefunace.top

Py:   for i in range(10): print(i)
来源：http://pgs.hnxiangtu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qgw.tianlin.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xcm.jinyuanbaomall.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bjm.vehdjk.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://evm.yfazqb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mxx.shangyingyoupin.top

Ruby: 10.times { |i| puts i }
来源：http://nsl.sjlbkw.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://oxn.jqgfzy.top

[B05] 遍历数组 / 列表
来源：http://xbg.ydjk.org.cn

Py:   for item in arr: print(item)
来源：http://dfy.daxiang520.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baz.yangfankeji.com

JS:   for (const item of arr) { console.log(item); }
来源：http://jgx.gzhubu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tds.kuanghao11.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://oex.iojbl.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://msr.shzxlz.cn

Ruby: arr.each { |item| puts item }
来源：http://afl.yangfankeji.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tts.daria6918.cn

[B06] 遍历字典 / 对象
来源：http://ide.nanxinkj.top

Py:   for k, v in d.items(): print(k, v)
来源：http://mda.zdbjq.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://puj.yvedp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ocr.jinqigfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vpw.pycfn.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://auq.jlsjyb.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pnl.sxryk.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tmw.ybcxt.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vbt.chenlongwang.top

[B07] while 循环
来源：http://ssg.xuanzx.com

Py:   while i < 10: i += 1
来源：http://kqu.andypj.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://yeu.hfpthk.cn

JS:   while (i < 10) { i++; }
来源：http://gpy.0kj1m.cn

TS:   while (i < 10) { i++; }
来源：http://qku.xylfe.cn

Java: while (i < 10) { i++; }
来源：http://tjp.smart0.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kxm.iojbl.cn

Ruby: while i < 10; i += 1; end
来源：http://qqo.redwolf501.top

C#:   while (i < 10) { i++; }
来源：http://ljt.birdmap.top

[B08] do-while（至少执行一次）
来源：http://cgr.hnxiangtu.top

Py:   # 无 do-while：用 while True + break
来源：http://jyd.quarkkingdee.top

PHP:  do { $i++; } while ($i < 10);
来源：http://nuw.zhoulong.xyz

JS:   do { i++; } while (i < 10);
来源：http://rnq.chenzaomai.com

TS:   do { i++; } while (i < 10);
来源：http://mda.yj20258.top

Java: do { i++; } while (i < 10);
来源：http://xvw.yj20258888.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ror.mhx1999.top

Ruby: begin; i += 1; end while i < 10
来源：http://itl.shanyushiyangtech.top

C#:   do { i++; } while (i < 10);
来源：http://ldj.hysaishi.cn

[B09] break 与 continue
来源：http://rbf.gzhubu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bxa.cucudq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://meb.gaohongyu789.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xue.fzhhl.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://coh.hnxiangtu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ito.gogol.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xwe.xingfuxueyuan.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://now.bbcook.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xgd.hongshengwenyu.top

[B10] 遍历同时拿索引
来源：http://szf.gzhubu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yxh.ehwqpu.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oxy.bjfxy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fmz.jianghu66.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yxg.vqdsnc.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ngc.uphjek.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bjz.feifeiyinyue.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://okc.meibo888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cqk.xziqi.cn

[B11] 生成数字序列 / 区间
来源：http://xqu.jianghu66.top

Py:   list(range(0, 10, 2))
来源：http://boa.yangfankeji.com

PHP:  range(0, 10, 2);
来源：http://sjh.hywenlv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ins.zhengqikj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xuk.pengpengdd.cyou

Java: IntStream.range(0, 10).boxed().toList()
来源：http://btm.uphjek.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bex.yuxming.cn

Ruby: (0...10).step(2).to_a
来源：http://ufs.ydzc1.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cct.ydzc1.top

[B12] 跳出多层循环
来源：http://qvb.feifeiyinyue.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vrr.yfazqb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://utb.chenjidiqi.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ldn.xingfuxueyuan.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bbg.9152youxi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xvd.ydjk.org.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jeh.hysaishi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ggu.yueranfly.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ceh.ybcxt.top


<!-- 参考信息 -->