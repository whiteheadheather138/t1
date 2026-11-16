代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://prs.xinyue.icu

[A07] 数字转字符串
来源：http://pmy.epnwcf.com

Py:   str(42)
来源：http://oyk.birdmap.top

PHP:  (string) 42; strval(42)
来源：http://dpb.fehbvm.com

JS:   String(42); (42).toString()
来源：http://ytm.pengpengdd.cyou

TS:   String(42)
来源：http://mjb.chenjidiqi.icu

Java: String.valueOf(42); Integer.toString(42)
来源：http://oju.fktsv.cn

Go:   strconv.Itoa(42)
来源：http://vor.cdnleiting.top

Ruby: 42.to_s
来源：http://iyj.hywenlv.cn

C#:   42.ToString()
来源：http://tki.jlsjyb.cn

[A08] 取整与四舍五入
来源：http://iyt.jqgfzy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xic.sjlbkw.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hom.ydjk.org.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://aqf.sufxvd.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://biy.tianlin.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nwq.zdqjudy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rxp.xylfe.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://dsl.shzxlz.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zvj.xinyue.icu

[A09] 绝对值与最大最小值
来源：http://dyd.tanke756.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://now.iojbl.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rqn.zhengqikj.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zoj.hywenlv.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qka.jinqigfzy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gse.yj20258888.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qgp.zdbjq.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pfy.0kj1m.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://key.yuxming.cn

[A10] 生成随机数
来源：http://zdk.nanxuanxn.top

Py:   import random; random.randint(1, 100)
来源：http://ydv.feifeiyinyue.top

PHP:  random_int(1, 100);
来源：http://yui.jinqigfzy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://iwd.ppjwa.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zlx.havefunace.top

Java: new Random().nextInt(100) + 1
来源：http://yfp.chenlongwang.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sdj.tanke756.top

Ruby: rand(1..100)
来源：http://low.yj20258.top

C#:   new Random().Next(1, 101)
来源：http://rbk.jiagoushi.top

[A11] 条件表达式（三元）
来源：http://hir.hywenlv.cn

Py:   "yes" if x > 0 else "no"
来源：http://vvt.sysykeji.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://myq.yongpay.top

JS:   x > 0 ? "yes" : "no"
来源：http://zvz.jyoumei.cn

TS:   x > 0 ? "yes" : "no"
来源：http://nyn.yfazqb.com

Java: x > 0 ? "yes" : "no"
来源：http://iyd.hammf.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://lnx.meibo888.top

Ruby: x > 0 ? "yes" : "no"
来源：http://bfn.fehbvm.com

C#:   x > 0 ? "yes" : "no"
来源：http://hhm.shzxlz.cn

[A12] 字符串插值 / 格式化
来源：http://fml.fanxiaobao.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dud.shangyingyoupin.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uup.cdnleiting.top

JS:   `Hello, ${name}!`
来源：http://wvl.hcnkem.com

TS:   `Hello, ${name}!`
来源：http://yuq.haohaochexian.top

Java: "Hello, %s!".formatted(name)
来源：http://sog.pengpengdd.cyou

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gfk.cheryme.top

Ruby: "Hello, #{name}!"
来源：http://anf.yonumen.top

C#:   $"Hello, {name}!"
来源：http://pcr.gzhubu.top

[A13] 多行字符串（练习 \n 转义）
来源：http://tea.ybcxt.top

Py:   "第一行\n第二行"
来源：http://hha.andypj.xyz

PHP:  "第一行\n第二行"
来源：http://zge.gaohongyu789.top

JS:   "第一行\n第二行"
来源：http://gwt.tianlin.xyz

TS:   "第一行\n第二行"
来源：http://cyg.sysykeji.top

Java: "第一行\n第二行"
来源：http://mqb.shangyingyoupin.top

Go:   "第一行\n第二行"
来源：http://eke.zhijiandao.cn

Ruby: "第一行\n第二行"
来源：http://nmh.yvedp.cn

C#:   "第一行\n第二行"
来源：http://trj.yvedp.cn

[A14] 注释写法
来源：http://vtj.hywenlv.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://egb.jyoumei.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xst.zycfv.cn

JS:   // 单行；/* 多行 */
来源：http://hgg.ctjpmb.com

TS:   // 单行；/* 多行 */
来源：http://qtu.uphjek.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ohq.feifeiyinyue.top

Go:   // 单行；/* 多行 */
来源：http://zex.xziqi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://whd.sxryk.cn

C#:   // 单行；/* 多行 */
来源：http://acl.zhaomingkeji.xyz

[A15] 空值判断与默认值
来源：http://lgy.xylfe.cn

Py:   value = data or "默认值"
来源：http://dex.ppjwa.cn

PHP:  $value = $data ?? "默认值";
来源：http://fsu.fzhhl.top

JS:   const value = data ?? "默认值";
来源：http://xuv.xinyue.icu

TS:   const value = data ?? "默认值";
来源：http://duh.hcnkem.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qjh.daria6918.cn

Go:   if data == "" { data = "默认值" }
来源：http://sqz.yj20258.top

Ruby: value = data || "默认值"
来源：http://mkb.hywenlv.cn

C#:   var value = data ?? "默认值";
来源：http://bkh.jlsjyb.cn

[A16] 真假值判断规则
来源：http://wjb.yvedp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dfl.smart0.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://iet.pycfn.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://oxw.aizwys.cn

TS:   if (!x) {}
来源：http://qzv.sweek.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://sdc.jinghuilouyu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dwh.ehwqpu.com

Ruby: unless x            # nil 与 false 为假
来源：http://epw.yj202588.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://eik.redwolf501.top

[A17] 位运算
来源：http://nlu.ybcxt.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gui.zdbjq.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bid.zhoulong.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dkb.jinghuilouyu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uhx.jinqigfzy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ari.cdnleiting.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://uiq.tianlin.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qqr.dianchejie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oin.haohaochexian.top

[A18] 字符与 ASCII 码互转
来源：http://nyx.ybcxt.top

Py:   ord("A"); chr(65)
来源：http://nbj.zhoulong.xyz

PHP:  ord("A"); chr(65)
来源：http://bqs.hongshengwenyu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nez.kuanghao11.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zna.guannengcc.top

Java: (int) 'A'; (char) 65
来源：http://qzf.hysaishi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://iuy.xylfe.cn

Ruby: "A".ord; 65.chr
来源：http://guc.c1oappe.top

C#:   (int)'A'; (char)65
来源：http://upp.pengpengdd.cyou

[A19] 交换两个变量
来源：http://ebg.jinghuilouyu.cn

Py:   a, b = b, a
来源：http://upi.andypj.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://qcc.jqgufenzy.top

JS:   [a, b] = [b, a];
来源：http://pqg.dianchejie.cn

TS:   [a, b] = [b, a];
来源：http://zjx.yj20258888.top

Java: int t = a; a = b; b = t;
来源：http://hks.yanxiufei.cn

Go:   a, b = b, a
来源：http://rso.sufxvd.cn

Ruby: a, b = b, a
来源：http://arg.hongshengwenyu.top

C#:   (a, b) = (b, a);
来源：http://cfj.snrcjt.cn

[A20] 读取标准输入
来源：http://edf.nanxuanxn.top

Py:   name = input("请输入：")
来源：http://ekr.shanyushiyangkeji.top

PHP:  $name = trim(fgets(STDIN));
来源：http://kli.yj20258.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cjs.shanyushiyangtech.top

TS:   // Node.js：readline 模块
来源：http://uex.fktsv.cn

Java: new Scanner(System.in).nextLine()
来源：http://uqb.yuxming.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://avu.ywan-chungtsiang.top

Ruby: gets.chomp
来源：http://vcg.birdmap.top

C#:   Console.ReadLine();
来源：http://ytx.shanyushiyangkeji.top

[A21] 保留指定小数位输出
来源：http://yqd.jianghu66.top

Py:   f"{3.14159:.2f}"
来源：http://ygv.c1oappe.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://myg.guowangkeji.top

JS:   (3.14159).toFixed(2)
来源：http://pag.ehwqpu.com

TS:   (3.14159).toFixed(2)
来源：http://ive.zdbjq.cn

Java: String.format("%.2f", 3.14159)
来源：http://twx.jiagoushi.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hsn.xuetiantiany.cn

Ruby: format("%.2f", 3.14159)
来源：http://sam.jianghu66.top

C#:   3.14159.ToString("F2")
来源：http://bnm.hfpthk.cn

[A22] 获取字符串长度
来源：http://vuw.guowangkeji.top

Py:   len(s)
来源：http://ncf.smart0.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yrj.andypj.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ujh.vehdjk.com

TS:   s.length
来源：http://hwe.sysykeji.top

Java: s.length()
来源：http://rzn.haohaochexian.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://eql.ydjk.org.cn

Ruby: s.length
来源：http://rcw.wangshuangyany.cn

C#:   s.Length
来源：http://ofx.shzxlz.cn

[A23] 大小写转换
来源：http://esm.feifeiyinyue.top

Py:   s.upper(); s.lower(); s.title()
来源：http://fjs.zhongyouzk.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nde.hesvh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wbk.hysaishi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://psh.sysykeji.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://aqv.quarkkingdee.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bld.jlsjyb.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://efa.yonumen.top

C#:   s.ToUpper(); s.ToLower()
来源：http://etq.zhiwuduotai.top

[A24] 去除首尾空白
来源：http://lhp.jqgufenzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dwz.birdmap.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://trm.tian-w.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ocy.cashguo.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mht.fengsongda.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://guc.sjlbkw.cn

Go:   strings.TrimSpace(s)
来源：http://nvi.chenlongwang.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bvt.mhx1999.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://poz.yangfankeji.com

[A25] 字符串比较
来源：http://fcs.kuanghao11.cn

Py:   s1 == s2; s1 != s2
来源：http://boc.daria6918.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dul.tian-w.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ony.sjlbkw.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xly.ehwqpu.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ofg.jqgfzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rka.hfpthk.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zyu.jqgfzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://puk.yanxiufei.cn

[A26] 类型转换总览
来源：http://fzl.jqgufenzy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://aln.tianlin.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ble.vqdsnc.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://enr.cucudq.cn

TS:   Number() String() Boolean() x as number
来源：http://jgo.fzhhl.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yfj.kuanghao11.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zde.chenjidiqi.icu

Ruby: to_i to_f to_s to_sym to_a
来源：http://opf.yj20258888.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jgd.zdbjq.cn

================================================================================
来源：http://fzs.sjlbkw.cn

B. 流程控制
来源：http://hmw.dashuyun.cn

================================================================================
来源：http://ppy.c1oappe.top

[B01] 条件判断 if / else
来源：http://fhs.vqdsnc.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://awp.hongshengwenyu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hql.0kj1m.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ptb.ivvv.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yxb.yfazqb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://vsy.jinyuanbaomall.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gle.feifeiyinyue.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ibv.cucudq.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jxl.tian-w.cn

[B02] 多分支 else if / elif
来源：http://gbm.uphjek.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yep.vehdjk.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://koc.iojbl.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lct.ctjpmb.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tgc.pycfn.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xfs.hesvh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gcb.fzhhl.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bgc.9152youxi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dki.hfpthk.cn

[B03] switch / match / case
来源：http://hbu.c1oappe.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fho.wangshuangyany.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xty.hesvh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uix.zhiwuduotai.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gxk.316326.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yxu.nanxuanxn.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://meb.chenlongwang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://exc.aibaodan.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pik.smart0.xyz

[B04] for 计数循环
来源：http://yqc.shanyushiyangtech.top

Py:   for i in range(10): print(i)
来源：http://zod.yfazqb.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jkx.zhaomingkeji.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zmr.cdnleiting.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nxq.fanxiaobao.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ftt.smart0.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://unc.zhaomingkeji.xyz

Ruby: 10.times { |i| puts i }
来源：http://svf.yongpay.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zei.zhaomingkeji.xyz

[B05] 遍历数组 / 列表
来源：http://ugz.ctjpmb.com

Py:   for item in arr: print(item)
来源：http://ckz.daxiang520.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jhn.zhaomingkeji.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://spr.fktsv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nuo.ybcxt.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://upa.sxryk.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uwm.zhiwuduotai.top

Ruby: arr.each { |item| puts item }
来源：http://ruw.zhoulong.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rmm.jqgfzy.top

[B06] 遍历字典 / 对象
来源：http://ezp.nanxuanxn.top

Py:   for k, v in d.items(): print(k, v)
来源：http://yaa.sysykeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uih.xziqi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xir.9152youxi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tlj.chenjidiqi.icu

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jzp.ydjk.org.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://brl.tianlin.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ype.birdmap.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pmy.tarul.cn

[B07] while 循环
来源：http://mzi.quarkkingdee.top

Py:   while i < 10: i += 1
来源：http://qtj.cqqwz.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ljq.pengpengdd.cyou

JS:   while (i < 10) { i++; }
来源：http://spv.yfazqb.com

TS:   while (i < 10) { i++; }
来源：http://ocb.pengpengdd.cyou

Java: while (i < 10) { i++; }
来源：http://tsx.sjlbkw.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dhq.sweek.top

Ruby: while i < 10; i += 1; end
来源：http://bad.daxiang520.top

C#:   while (i < 10) { i++; }
来源：http://xtc.snrcjt.cn

[B08] do-while（至少执行一次）
来源：http://feg.jinqigfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://xrj.zdbjq.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sge.chenjidiqi.icu

JS:   do { i++; } while (i < 10);
来源：http://eib.jqgufenzy.top

TS:   do { i++; } while (i < 10);
来源：http://jlt.fehbvm.com

Java: do { i++; } while (i < 10);
来源：http://uwu.yvedp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pjj.yonumen.top

Ruby: begin; i += 1; end while i < 10
来源：http://mxs.smart0.xyz

C#:   do { i++; } while (i < 10);
来源：http://ckz.zhixingplan.top

[B09] break 与 continue
来源：http://wcg.52xcode.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jaw.hesvh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yxp.jyoumei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hoi.gogol.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aql.andypj.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sdr.zdbjq.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ixe.ctjpmb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fnh.shangyingyoupin.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bcd.yuxming.cn

[B10] 遍历同时拿索引
来源：http://uwe.feifeiyinyue.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dln.yonumen.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sus.tanke756.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gnd.ydzc1.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sji.xinyue.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wnp.shangyingyoupin.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jux.sjlbkw.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lpe.cheryme.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ovp.aibaodan.cn

[B11] 生成数字序列 / 区间
来源：http://tsl.aizwys.cn

Py:   list(range(0, 10, 2))
来源：http://qrv.yueranfly.top

PHP:  range(0, 10, 2);
来源：http://ofn.feifeiyinyue.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rlj.xuetiantiany.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mkq.jqgfzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oig.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://szf.ydjk.org.cn

Ruby: (0...10).step(2).to_a
来源：http://wex.iojbl.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://itn.hcnkem.com

[B12] 跳出多层循环
来源：http://ysx.hysaishi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://npf.tianlin.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://kfo.sjlbkw.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bdp.jinyuanbaomall.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://eoc.andypj.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uki.wangshuangyany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wjw.sweek.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jzr.zhijiandao.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gyh.snrcjt.cn

[B13] 判断是否为数字
来源：http://hsp.sufxvd.cn

Py:   isinstance(x, (int, float))
来源：http://vno.hnxiangtu.top

PHP:  is_numeric($x)
来源：http://mll.snrcjt.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://inw.haohaochexian.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bvb.52xcode.cn

Java: x instanceof Number
来源：http://kjg.shanyushiyangkeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ylo.zhiwuduotai.top

Ruby: x.is_a?(Numeric)
来源：http://nmo.shanyushiyangtech.top


<!-- 参考信息 -->