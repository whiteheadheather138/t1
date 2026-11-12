代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://xxg.zhoulong.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://xsv.hnqzz.top

C#:   x.GetType().Name; x is int
来源：http://ibu.shanyushiyangtech.top

[A05] 整数除法与取模
来源：http://alt.yuanzhike.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ujc.xuetiantiany.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://acf.hesvh.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pvq.jqgufenzy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://alx.svipenyu.cn

Java: 7 / 2; 7 % 2
来源：http://fuy.gzhubu.top

Go:   7 / 2; 7 % 2
来源：http://bfv.yj20258888.top

Ruby: 7 / 2; 7 % 2
来源：http://lsm.xuetiantiany.cn

C#:   7 / 2; 7 % 2
来源：http://ale.tianlin.xyz

[A06] 字符串转数字
来源：http://yxq.fengsongda.top

Py:   int("42"); float("3.14")
来源：http://jtd.jqgufenzy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kgy.jiagoushi.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ecj.mhx1999.top

TS:   parseInt("42", 10); Number("42")
来源：http://jwq.gzhubu.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://txz.zhixingplan.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xaq.hnxiangtu.top

Ruby: "42".to_i; "3.14".to_f
来源：http://lgp.hcnkem.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nsm.tarul.cn

[A07] 数字转字符串
来源：http://jzn.smart0.xyz

Py:   str(42)
来源：http://hff.jyoumei.cn

PHP:  (string) 42; strval(42)
来源：http://wvd.guannengcc.top

JS:   String(42); (42).toString()
来源：http://win.hammf.cn

TS:   String(42)
来源：http://gcf.zhaomingkeji.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://dxo.chenjidiqi.icu

Go:   strconv.Itoa(42)
来源：http://lje.jinyuanbaomall.cn

Ruby: 42.to_s
来源：http://tzd.redwolf501.top

C#:   42.ToString()
来源：http://yuz.bbcook.cn

[A08] 取整与四舍五入
来源：http://grk.yuxming.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ylz.chenjidiqi.icu

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ihj.fzhhl.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ilp.ydzc1.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zct.gogol.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ncv.yfazqb.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ylq.jlsjyb.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://brc.hfpthk.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xyj.ppjwa.cn

[A09] 绝对值与最大最小值
来源：http://ahz.guannengcc.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xja.bjfxy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rxh.yfazqb.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sxu.sufxvd.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wot.nwbrower.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gaa.zhiwuduotai.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://phl.dashuyun.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vab.yanxiufei.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wjo.hcnkem.com

[A10] 生成随机数
来源：http://whh.fengsongda.top

Py:   import random; random.randint(1, 100)
来源：http://ytg.tian-w.cn

PHP:  random_int(1, 100);
来源：http://knu.redwolf501.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pxw.ppjwa.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nmm.fanxiaobao.xyz

Java: new Random().nextInt(100) + 1
来源：http://dja.nwbrower.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kjt.pycfn.com

Ruby: rand(1..100)
来源：http://etg.jqgufenzy.top

C#:   new Random().Next(1, 101)
来源：http://njk.pycfn.com

[A11] 条件表达式（三元）
来源：http://ztq.shanyushiyangkeji.top

Py:   "yes" if x > 0 else "no"
来源：http://lwv.jyoumei.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qpl.tianlin.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://cek.ydjk.org.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hih.redwolf501.top

Java: x > 0 ? "yes" : "no"
来源：http://ekd.9152youxi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://beh.yanxiufei.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jxv.daria6918.cn

C#:   x > 0 ? "yes" : "no"
来源：http://flc.feifeiyinyue.top

[A12] 字符串插值 / 格式化
来源：http://zjb.ehwqpu.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://prp.tian-w.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://eub.jianghu66.top

JS:   `Hello, ${name}!`
来源：http://arl.xinyue.icu

TS:   `Hello, ${name}!`
来源：http://sho.cheryme.top

Java: "Hello, %s!".formatted(name)
来源：http://ggm.jyoumei.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tlz.fengsongda.top

Ruby: "Hello, #{name}!"
来源：http://hmu.bbcook.cn

C#:   $"Hello, {name}!"
来源：http://eib.zhongyouzk.top

[A13] 多行字符串（练习 \n 转义）
来源：http://qkj.jinghuilouyu.cn

Py:   "第一行\n第二行"
来源：http://teh.sweek.top

PHP:  "第一行\n第二行"
来源：http://hvs.epnwcf.com

JS:   "第一行\n第二行"
来源：http://uon.tian-w.cn

TS:   "第一行\n第二行"
来源：http://wzo.aizwys.cn

Java: "第一行\n第二行"
来源：http://ovq.sjlbkw.cn

Go:   "第一行\n第二行"
来源：http://yqs.ybcxt.top

Ruby: "第一行\n第二行"
来源：http://jgx.tian-w.cn

C#:   "第一行\n第二行"
来源：http://ccj.hongshengwenyu.top

[A14] 注释写法
来源：http://cyy.yvedp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kxk.jinghuilouyu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hrx.tian-w.cn

JS:   // 单行；/* 多行 */
来源：http://azn.hongshengwenyu.top

TS:   // 单行；/* 多行 */
来源：http://adb.hammf.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://oqd.haohaochexian.top

Go:   // 单行；/* 多行 */
来源：http://leb.yuxming.cn

Ruby: # 单行；=begin 多行 =end
来源：http://mra.nanxinkj.top

C#:   // 单行；/* 多行 */
来源：http://nao.yongpay.top

[A15] 空值判断与默认值
来源：http://giy.shanyushiyangtech.top

Py:   value = data or "默认值"
来源：http://cfu.cqqwz.cn

PHP:  $value = $data ?? "默认值";
来源：http://syb.cucudq.cn

JS:   const value = data ?? "默认值";
来源：http://qag.xylfe.cn

TS:   const value = data ?? "默认值";
来源：http://cwo.haohaochexian.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nvd.daxiang520.top

Go:   if data == "" { data = "默认值" }
来源：http://ola.pengpengdd.cyou

Ruby: value = data || "默认值"
来源：http://fsp.haohaochexian.top

C#:   var value = data ?? "默认值";
来源：http://bki.hesvh.cn

[A16] 真假值判断规则
来源：http://paq.guannengcc.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gpw.ppjwa.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cce.wangdashe.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qnq.sufxvd.cn

TS:   if (!x) {}
来源：http://com.jinyuanbaomall.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://alu.hammf.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jpe.feifeiyinyue.top

Ruby: unless x            # nil 与 false 为假
来源：http://ucu.yueranfly.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sjc.bjfxy.top

[A17] 位运算
来源：http://ztk.daxiang520.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://seb.jianghu66.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vfu.jlsjyb.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oxs.yonumen.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://trd.nanxuanxn.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sqz.zhengqikj.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rgj.yj202588.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ujr.aizwys.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eon.yj20258.top

[A18] 字符与 ASCII 码互转
来源：http://juq.tarul.cn

Py:   ord("A"); chr(65)
来源：http://ihm.birdmap.top

PHP:  ord("A"); chr(65)
来源：http://bpf.tian-w.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fqg.bbcook.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://aki.jinqigfzy.top

Java: (int) 'A'; (char) 65
来源：http://ump.yongpay.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://juk.gogol.net.cn

Ruby: "A".ord; 65.chr
来源：http://lhm.jinyuanbaomall.cn

C#:   (int)'A'; (char)65
来源：http://blx.tianlin.xyz

[A19] 交换两个变量
来源：http://gjo.tianlin.xyz

Py:   a, b = b, a
来源：http://ubd.shzxlz.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://owh.yfazqb.com

JS:   [a, b] = [b, a];
来源：http://lfc.jqgfzy.top

TS:   [a, b] = [b, a];
来源：http://svc.sxryk.cn

Java: int t = a; a = b; b = t;
来源：http://jhe.hongshengwenyu.top

Go:   a, b = b, a
来源：http://glh.sxryk.cn

Ruby: a, b = b, a
来源：http://cyz.yangfankeji.com

C#:   (a, b) = (b, a);
来源：http://rey.shanyushiyangtech.top

[A20] 读取标准输入
来源：http://sva.birdmap.top

Py:   name = input("请输入：")
来源：http://uta.yonumen.top

PHP:  $name = trim(fgets(STDIN));
来源：http://cbe.havefunace.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sla.zhijiandao.cn

TS:   // Node.js：readline 模块
来源：http://knr.bbcook.cn

Java: new Scanner(System.in).nextLine()
来源：http://dmt.hywenlv.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hgd.cheryme.top

Ruby: gets.chomp
来源：http://hih.nanxinkj.top

C#:   Console.ReadLine();
来源：http://aqw.nwbrower.top

[A21] 保留指定小数位输出
来源：http://ood.dianchejie.cn

Py:   f"{3.14159:.2f}"
来源：http://eez.fengsongda.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jfd.nanxuanxn.top

JS:   (3.14159).toFixed(2)
来源：http://ztp.fzhhl.top

TS:   (3.14159).toFixed(2)
来源：http://yre.shzxlz.cn

Java: String.format("%.2f", 3.14159)
来源：http://dah.xuanzx.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kzw.tian-w.cn

Ruby: format("%.2f", 3.14159)
来源：http://jgl.chenjidiqi.icu

C#:   3.14159.ToString("F2")
来源：http://bmh.zhengqikj.top

[A22] 获取字符串长度
来源：http://xcn.ivvv.top

Py:   len(s)
来源：http://nxx.cdnleiting.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fxc.shzxlz.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gam.bbcook.cn

TS:   s.length
来源：http://nif.sufxvd.cn

Java: s.length()
来源：http://rat.yonumen.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cyc.kuanghao11.cn

Ruby: s.length
来源：http://rxj.ybcxt.top

C#:   s.Length
来源：http://gxb.ywan-chungtsiang.top

[A23] 大小写转换
来源：http://ebs.mhx1999.top

Py:   s.upper(); s.lower(); s.title()
来源：http://yap.fehbvm.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xxs.zycfv.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://glj.ydjk.org.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rcu.shangyingyoupin.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://brk.pengpengdd.cyou

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sdi.tanke756.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lnq.sysykeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gex.zhengqikj.top

[A24] 去除首尾空白
来源：http://pck.shanyushiyangkeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zyw.tianlin.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nli.sxryk.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xwe.shzxlz.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://axe.ppjwa.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://thj.andypj.xyz

Go:   strings.TrimSpace(s)
来源：http://oqt.gotoacloud.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://twm.pengpengdd.cyou

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tpb.hnxiangtu.top

[A25] 字符串比较
来源：http://wdc.jqgfzy.top

Py:   s1 == s2; s1 != s2
来源：http://eqi.epnwcf.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://eyw.jianghu66.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dhw.jinqigfzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ijm.yj20258.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vfd.dashuyun.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cvj.jiagoushi.top

Ruby: s1 == s2; s1 <=> s2
来源：http://itx.ehwqpu.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ysf.birdmap.top

[A26] 类型转换总览
来源：http://qcm.ybcxt.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zsc.quarkkingdee.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mar.gogol.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wtl.ppjwa.cn

TS:   Number() String() Boolean() x as number
来源：http://tpe.tarul.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mws.andypj.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iyo.wangshuangyany.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wnl.zhengqikj.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://meq.jinghuilouyu.cn

================================================================================
来源：http://hvd.zycfv.cn

B. 流程控制
来源：http://cbc.ivvv.top

================================================================================
来源：http://ccp.aizwys.cn

[B01] 条件判断 if / else
来源：http://yjp.haohaochexian.top

Py:   result = "正" if x > 0 else "非正"
来源：http://nkk.gotoacloud.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xrv.zhoulong.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zax.aibaodan.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zga.xylfe.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dlg.svipenyu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vmg.haohaochexian.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ilt.jqgufenzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://anl.gotoacloud.top

[B02] 多分支 else if / elif
来源：http://teh.havefunace.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ilu.hfpthk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://umy.jlsjyb.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kll.shzxlz.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ozz.yongpay.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wrj.gaohongyu789.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bon.cashguo.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rkc.shuidangran.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oyn.sjlbkw.cn

[B03] switch / match / case
来源：http://ete.hnxiangtu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blc.shanyushiyangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zoo.haohaochexian.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dbh.vqdsnc.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yeb.yongpay.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mcb.ywan-chungtsiang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fes.ctjpmb.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tja.aibaodan.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iyi.yueranfly.top

[B04] for 计数循环
来源：http://dkh.zhengqikj.top

Py:   for i in range(10): print(i)
来源：http://pjj.fanxiaobao.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bxt.cdnleiting.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hzh.hfpthk.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yke.haohaochexian.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://obx.yueranfly.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vzp.yvedp.cn

Ruby: 10.times { |i| puts i }
来源：http://xuh.cashguo.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ecc.sjlbkw.cn

[B05] 遍历数组 / 列表
来源：http://woo.vqdsnc.cn

Py:   for item in arr: print(item)
来源：http://zhz.sysykeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sqh.sjlbkw.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nch.jiagoushi.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xcx.fengsongda.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://waz.feifeiyinyue.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mil.jinghuilouyu.cn

Ruby: arr.each { |item| puts item }
来源：http://swk.ydjk.org.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://poh.sxryk.cn

[B06] 遍历字典 / 对象
来源：http://zvw.shanyushiyangkeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ksy.jqgfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jyz.yj20258.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fzh.zhoulong.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fcg.zdbjq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uvh.hywenlv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xkn.tarul.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://egl.fehbvm.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ddr.birdmap.top

[B07] while 循环
来源：http://dsm.jinqigufen.top

Py:   while i < 10: i += 1
来源：http://iai.bjfxy.top

PHP:  while ($i < 10) { $i++; }
来源：http://nrc.gzhubu.top

JS:   while (i < 10) { i++; }
来源：http://ell.pycfn.com

TS:   while (i < 10) { i++; }
来源：http://wuo.yongpay.top

Java: while (i < 10) { i++; }
来源：http://ehq.ctjpmb.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://inq.haohaochexian.top

Ruby: while i < 10; i += 1; end
来源：http://xlv.zhengqikj.top

C#:   while (i < 10) { i++; }
来源：http://tls.daria6918.cn

[B08] do-while（至少执行一次）
来源：http://zgl.c1oappe.top

Py:   # 无 do-while：用 while True + break
来源：http://vjp.ydzc1.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vnr.jinqigfzy.top

JS:   do { i++; } while (i < 10);
来源：http://xoq.kuanghao11.cn

TS:   do { i++; } while (i < 10);
来源：http://osw.tanke756.top

Java: do { i++; } while (i < 10);
来源：http://riq.dianchejie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gzq.zhoulong.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://hfn.nanxuanxn.top

C#:   do { i++; } while (i < 10);
来源：http://dlt.daria6918.cn

[B09] break 与 continue
来源：http://wax.0kj1m.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rpd.nanxinkj.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uct.jianghu66.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wae.sweek.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xzu.52xcode.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://seq.xylfe.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lwb.yfazqb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ajr.jinqigfzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ihm.9152youxi.cn

[B10] 遍历同时拿索引
来源：http://kti.feifeiyinyue.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xnk.shuidangran.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mhp.0kj1m.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ueb.ppjwa.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fyq.vqdsnc.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ccz.andypj.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sts.ybcxt.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://szs.pycfn.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://swh.shanyushiyangkeji.top

[B11] 生成数字序列 / 区间
来源：http://xwn.guannengcc.top

Py:   list(range(0, 10, 2))
来源：http://gys.yongpay.top

PHP:  range(0, 10, 2);
来源：http://ppi.redwolf501.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wno.haohaochexian.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yhe.hysaishi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ado.guannengcc.top


<!-- 参考信息 -->