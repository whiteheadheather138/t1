代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wmg.feifeiyinyue.top

[A07] 数字转字符串
来源：http://cqn.xuetiantiany.cn

Py:   str(42)
来源：http://iam.guowangkeji.top

PHP:  (string) 42; strval(42)
来源：http://sew.ivvv.top

JS:   String(42); (42).toString()
来源：http://nvv.chenzaomai.com

TS:   String(42)
来源：http://ges.kuanghao11.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://efe.yj202588.top

Go:   strconv.Itoa(42)
来源：http://ffi.jqgufenzy.top

Ruby: 42.to_s
来源：http://upe.svipenyu.cn

C#:   42.ToString()
来源：http://iwm.shzxlz.cn

[A08] 取整与四舍五入
来源：http://dwh.jianghu66.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tzn.hysaishi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ozs.shangyingyoupin.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rlm.hammf.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dxa.cqqwz.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://utm.tian-w.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gay.guowangkeji.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://qey.yfazqb.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xxd.xuanzx.com

[A09] 绝对值与最大最小值
来源：http://qxc.epnwcf.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blm.bjfxy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zkc.yongpay.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wze.feifeiyinyue.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cnw.yonumen.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xrt.haohaochexian.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wos.yuxming.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jbs.gaohongyu789.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rte.jinyuanbaomall.cn

[A10] 生成随机数
来源：http://uvz.yj20258888.top

Py:   import random; random.randint(1, 100)
来源：http://tnw.yanxiufei.cn

PHP:  random_int(1, 100);
来源：http://fkj.tianlin.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jvk.guowangkeji.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gwt.hywenlv.cn

Java: new Random().nextInt(100) + 1
来源：http://rwz.jinqigfzy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mpz.jianghu66.top

Ruby: rand(1..100)
来源：http://zpn.shanyushiyangtech.top

C#:   new Random().Next(1, 101)
来源：http://cxc.hywenlv.cn

[A11] 条件表达式（三元）
来源：http://bps.meibo888.top

Py:   "yes" if x > 0 else "no"
来源：http://vvl.chenjidiqi.icu

PHP:  $x > 0 ? "yes" : "no"
来源：http://sty.xuetiantiany.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vad.yj20258.top

TS:   x > 0 ? "yes" : "no"
来源：http://uva.chenlongwang.top

Java: x > 0 ? "yes" : "no"
来源：http://cak.cdnleiting.top

Go:   // 无三元运算符，需用 if 语句
来源：http://uou.dashuyun.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://obw.cheryme.top

C#:   x > 0 ? "yes" : "no"
来源：http://jmm.gzhubu.top

[A12] 字符串插值 / 格式化
来源：http://xqz.ehwqpu.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jzg.tanke756.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zml.zycfv.cn

JS:   `Hello, ${name}!`
来源：http://wja.jinqigfzy.top

TS:   `Hello, ${name}!`
来源：http://naf.zdbjq.cn

Java: "Hello, %s!".formatted(name)
来源：http://jni.yj20258.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jiu.zhiwuduotai.top

Ruby: "Hello, #{name}!"
来源：http://dsf.zhongyouzk.top

C#:   $"Hello, {name}!"
来源：http://pdi.cashguo.top

[A13] 多行字符串（练习 \n 转义）
来源：http://uwt.cucudq.cn

Py:   "第一行\n第二行"
来源：http://imm.iojbl.cn

PHP:  "第一行\n第二行"
来源：http://siw.yonumen.top

JS:   "第一行\n第二行"
来源：http://zrk.hongshengwenyu.top

TS:   "第一行\n第二行"
来源：http://orz.yanxiufei.cn

Java: "第一行\n第二行"
来源：http://vtv.jinqigfzy.top

Go:   "第一行\n第二行"
来源：http://gxb.shangyingyoupin.top

Ruby: "第一行\n第二行"
来源：http://cbs.cdnleiting.top

C#:   "第一行\n第二行"
来源：http://ghm.haohaochexian.top

[A14] 注释写法
来源：http://etn.tarul.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qhj.ivvv.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://mev.hcnkem.com

JS:   // 单行；/* 多行 */
来源：http://gxr.zhengqikj.top

TS:   // 单行；/* 多行 */
来源：http://zwg.xinyue.icu

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tst.meibo888.top

Go:   // 单行；/* 多行 */
来源：http://okd.hfpthk.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ioh.hammf.cn

C#:   // 单行；/* 多行 */
来源：http://emo.shuidangran.top

[A15] 空值判断与默认值
来源：http://pda.zhiwuduotai.top

Py:   value = data or "默认值"
来源：http://dsj.sxryk.cn

PHP:  $value = $data ?? "默认值";
来源：http://vfc.cucudq.cn

JS:   const value = data ?? "默认值";
来源：http://mmn.aizwys.cn

TS:   const value = data ?? "默认值";
来源：http://nqg.0kj1m.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yev.yj202588.top

Go:   if data == "" { data = "默认值" }
来源：http://bqb.jinyuanbaomall.cn

Ruby: value = data || "默认值"
来源：http://qct.xziqi.cn

C#:   var value = data ?? "默认值";
来源：http://ykf.yj20258888.top

[A16] 真假值判断规则
来源：http://baf.aibaodan.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://esu.iojbl.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bht.svipenyu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://smn.hnqzz.top

TS:   if (!x) {}
来源：http://irn.sysykeji.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mvy.fktsv.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vas.epnwcf.com

Ruby: unless x            # nil 与 false 为假
来源：http://yrj.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nsp.chenlongwang.top

[A17] 位运算
来源：http://hxp.ppjwa.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mot.shzxlz.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pev.zhoulong.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oho.jqgfzy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://olc.gaohongyu789.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hxy.ydjk.org.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mpy.yanxiufei.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ezq.xziqi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ukz.jinqigufen.top

[A18] 字符与 ASCII 码互转
来源：http://idy.hesvh.cn

Py:   ord("A"); chr(65)
来源：http://cdl.zycfv.cn

PHP:  ord("A"); chr(65)
来源：http://xge.ybcxt.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://psh.guannengcc.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vzw.yj20258888.top

Java: (int) 'A'; (char) 65
来源：http://uwo.52xcode.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ehy.shuidangran.top

Ruby: "A".ord; 65.chr
来源：http://qsf.cucudq.cn

C#:   (int)'A'; (char)65
来源：http://nuk.xziqi.cn

[A19] 交换两个变量
来源：http://oct.sweek.top

Py:   a, b = b, a
来源：http://cqn.guowangkeji.top

PHP:  [$a, $b] = [$b, $a];
来源：http://moo.sjlbkw.cn

JS:   [a, b] = [b, a];
来源：http://kim.yuanzhike.top

TS:   [a, b] = [b, a];
来源：http://bdn.yuanzhike.top

Java: int t = a; a = b; b = t;
来源：http://tom.fehbvm.com

Go:   a, b = b, a
来源：http://joh.sweek.top

Ruby: a, b = b, a
来源：http://rnf.yj20258.top

C#:   (a, b) = (b, a);
来源：http://xgz.yfazqb.com

[A20] 读取标准输入
来源：http://yya.daxiang520.top

Py:   name = input("请输入：")
来源：http://vrx.ydzc1.top

PHP:  $name = trim(fgets(STDIN));
来源：http://fmr.yueranfly.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://csv.jqgufenzy.top

TS:   // Node.js：readline 模块
来源：http://rwt.daria6918.cn

Java: new Scanner(System.in).nextLine()
来源：http://rza.meibo888.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://iqi.xuetiantiany.cn

Ruby: gets.chomp
来源：http://idc.zhengqikj.top

C#:   Console.ReadLine();
来源：http://qwo.smart0.xyz

[A21] 保留指定小数位输出
来源：http://uug.havefunace.top

Py:   f"{3.14159:.2f}"
来源：http://liv.cqqwz.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kwc.redwolf501.top

JS:   (3.14159).toFixed(2)
来源：http://yor.fzhhl.top

TS:   (3.14159).toFixed(2)
来源：http://gof.yvedp.cn

Java: String.format("%.2f", 3.14159)
来源：http://bhw.pycfn.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ruy.tarul.cn

Ruby: format("%.2f", 3.14159)
来源：http://tqo.ppjwa.cn

C#:   3.14159.ToString("F2")
来源：http://lhk.fktsv.cn

[A22] 获取字符串长度
来源：http://bee.cashguo.top

Py:   len(s)
来源：http://flb.cashguo.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://igq.shanyushiyangkeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rsb.gotoacloud.top

TS:   s.length
来源：http://xpn.yj20258.top

Java: s.length()
来源：http://cpe.smart0.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tby.redwolf501.top

Ruby: s.length
来源：http://axs.zhengqikj.top

C#:   s.Length
来源：http://zvm.hywenlv.cn

[A23] 大小写转换
来源：http://gck.dianchejie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://udp.quarkkingdee.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lza.snrcjt.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fdn.hnxiangtu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ghf.bbcook.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kec.daxiang520.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lvl.aizwys.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ufm.yangfankeji.com

C#:   s.ToUpper(); s.ToLower()
来源：http://yxe.pengpengdd.cyou

[A24] 去除首尾空白
来源：http://guc.wangshuangyany.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sbi.gogol.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ufe.gzhubu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nuq.bjfxy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://obb.zhixingplan.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xqg.ivvv.top

Go:   strings.TrimSpace(s)
来源：http://npl.daxiang520.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kpv.zhongyouzk.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bvp.0kj1m.cn

[A25] 字符串比较
来源：http://qbv.yueranfly.top

Py:   s1 == s2; s1 != s2
来源：http://ngh.yanxiufei.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sni.daria6918.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://duj.cucudq.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vvt.cdnleiting.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fko.iojbl.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qwe.jyoumei.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ike.yuanzhike.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mqs.nanxuanxn.top

[A26] 类型转换总览
来源：http://tfy.sxryk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zvs.yj20258888.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bji.mhx1999.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pto.birdmap.top

TS:   Number() String() Boolean() x as number
来源：http://cza.zhoulong.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wfs.wangshuangyany.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lwt.zhijiandao.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cat.epnwcf.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ayx.yuanzhike.top

================================================================================
来源：http://zna.sysykeji.top

B. 流程控制
来源：http://xkf.tanke756.top

================================================================================
来源：http://apg.shangyingyoupin.top

[B01] 条件判断 if / else
来源：http://suz.redwolf501.top

Py:   result = "正" if x > 0 else "非正"
来源：http://rdh.hnqzz.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ufn.gotoacloud.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nbn.hysaishi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cbc.sysykeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://xjb.aibaodan.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jlb.zhengqikj.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ymf.gogol.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kdx.snrcjt.cn

[B02] 多分支 else if / elif
来源：http://adz.9152youxi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qhd.xingfuxueyuan.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ojl.316326.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wvx.guowangkeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rof.jqgufenzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wrh.pycfn.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://huk.yonumen.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ljh.gzhubu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aww.snrcjt.cn

[B03] switch / match / case
来源：http://wah.ydjk.org.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sli.uphjek.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://quq.cqqwz.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gvt.c1oappe.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gnx.9152youxi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://epe.shangyingyoupin.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://syk.ppjwa.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://olp.shangyingyoupin.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yrb.fehbvm.com

[B04] for 计数循环
来源：http://sdc.cashguo.top

Py:   for i in range(10): print(i)
来源：http://sxd.xingfuxueyuan.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hzj.shanyushiyangtech.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qov.9152youxi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rpy.cucudq.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rin.hongshengwenyu.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zfd.kuanghao11.cn

Ruby: 10.times { |i| puts i }
来源：http://eyi.zhiwuduotai.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://irf.yueranfly.top

[B05] 遍历数组 / 列表
来源：http://qfz.hfpthk.cn

Py:   for item in arr: print(item)
来源：http://tst.zdqjudy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bga.yuanzhike.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hjl.xylfe.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hvn.chenzaomai.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://mab.fengsongda.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://igj.gaohongyu789.top

Ruby: arr.each { |item| puts item }
来源：http://uky.yvedp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ety.cucudq.cn

[B06] 遍历字典 / 对象
来源：http://iuy.sxryk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://aii.wangdashe.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ziv.cucudq.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iso.andypj.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kje.cqqwz.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pwu.shuidangran.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kup.dashuyun.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ltv.52xcode.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dkx.iojbl.cn

[B07] while 循环
来源：http://ylm.zdqjudy.top

Py:   while i < 10: i += 1
来源：http://chq.hongshengwenyu.top

PHP:  while ($i < 10) { $i++; }
来源：http://kkj.jqgfzy.top

JS:   while (i < 10) { i++; }
来源：http://fqq.ctjpmb.com

TS:   while (i < 10) { i++; }
来源：http://oss.shangyingyoupin.top

Java: while (i < 10) { i++; }
来源：http://umx.ywan-chungtsiang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://coh.shanyushiyangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://rxx.hysaishi.cn

C#:   while (i < 10) { i++; }
来源：http://kai.zdbjq.cn

[B08] do-while（至少执行一次）
来源：http://siw.c1oappe.top

Py:   # 无 do-while：用 while True + break
来源：http://cfw.zhaomingkeji.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://cdi.bbcook.cn

JS:   do { i++; } while (i < 10);
来源：http://fvc.yanxiufei.cn

TS:   do { i++; } while (i < 10);
来源：http://plz.jinqigfzy.top

Java: do { i++; } while (i < 10);
来源：http://lys.ehwqpu.com

Go:   for { i++; if i >= 10 { break } }
来源：http://lvu.chenlongwang.top

Ruby: begin; i += 1; end while i < 10
来源：http://yae.smart0.xyz

C#:   do { i++; } while (i < 10);
来源：http://xaj.ydzc1.top

[B09] break 与 continue
来源：http://fkj.havefunace.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jtp.ctjpmb.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eoc.sjlbkw.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://goq.sysykeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hlv.nanxuanxn.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wdk.epnwcf.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zgl.52xcode.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qxo.zdbjq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sqo.nwbrower.top

[B10] 遍历同时拿索引
来源：http://toq.sufxvd.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://opl.jyoumei.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://epe.daria6918.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cck.ivvv.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ian.yuanzhike.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wim.9152youxi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ghz.zhongyouzk.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hlr.nwbrower.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lpm.nanxinkj.top

[B11] 生成数字序列 / 区间
来源：http://dwr.yj202588.top

Py:   list(range(0, 10, 2))
来源：http://ahm.sjlbkw.cn

PHP:  range(0, 10, 2);
来源：http://edu.tanke756.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ykv.hfpthk.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wjk.shanyushiyangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qeu.jyoumei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kts.yj20258888.top

Ruby: (0...10).step(2).to_a
来源：http://dpa.shanyushiyangtech.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qsr.jinqigufen.top

[B12] 跳出多层循环
来源：http://xuc.jinqigfzy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://yku.snrcjt.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ydr.sjlbkw.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bmu.jlsjyb.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ndk.zhixingplan.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mih.zhijiandao.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yox.gotoacloud.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cws.gaohongyu789.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ppb.wangshuangyany.cn

[B13] 判断是否为数字
来源：http://vjt.zdbjq.cn

Py:   isinstance(x, (int, float))
来源：http://gby.ppjwa.cn

PHP:  is_numeric($x)
来源：http://mia.aibaodan.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pmf.jinqigfzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aqb.yvedp.cn

Java: x instanceof Number
来源：http://aaq.yj20258888.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mzu.hywenlv.cn

Ruby: x.is_a?(Numeric)
来源：http://kiz.ydzc1.top


<!-- 参考信息 -->