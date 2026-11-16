代发 wailian999

[A10] 生成随机数
来源：http://ujw.cdnleiting.top

Py:   import random; random.randint(1, 100)
来源：http://ptn.hnxiangtu.top

PHP:  random_int(1, 100);
来源：http://ypc.meibo888.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kut.ppjwa.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://eka.hysaishi.cn

Java: new Random().nextInt(100) + 1
来源：http://dtv.0kj1m.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://clz.hcnkem.com

Ruby: rand(1..100)
来源：http://zpq.ydzc1.top

C#:   new Random().Next(1, 101)
来源：http://dob.ydjk.org.cn

[A11] 条件表达式（三元）
来源：http://ytl.hywenlv.cn

Py:   "yes" if x > 0 else "no"
来源：http://isi.yj202588.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://atq.52xcode.cn

JS:   x > 0 ? "yes" : "no"
来源：http://eco.yj20258.top

TS:   x > 0 ? "yes" : "no"
来源：http://cww.daxiang520.top

Java: x > 0 ? "yes" : "no"
来源：http://oir.chenlongwang.top

Go:   // 无三元运算符，需用 if 语句
来源：http://pif.hnxiangtu.top

Ruby: x > 0 ? "yes" : "no"
来源：http://mzb.epnwcf.com

C#:   x > 0 ? "yes" : "no"
来源：http://elw.ybcxt.top

[A12] 字符串插值 / 格式化
来源：http://epg.yanxiufei.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://muq.jlsjyb.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ela.nanxinkj.top

JS:   `Hello, ${name}!`
来源：http://ymu.jqgfzy.top

TS:   `Hello, ${name}!`
来源：http://wcq.ppjwa.cn

Java: "Hello, %s!".formatted(name)
来源：http://ksq.chenjidiqi.icu

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://twi.jinqigfzy.top

Ruby: "Hello, #{name}!"
来源：http://nge.ppjwa.cn

C#:   $"Hello, {name}!"
来源：http://vnj.sweek.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ohx.uphjek.com

Py:   "第一行\n第二行"
来源：http://akj.pengpengdd.cyou

PHP:  "第一行\n第二行"
来源：http://tsa.sxryk.cn

JS:   "第一行\n第二行"
来源：http://hlh.quarkkingdee.top

TS:   "第一行\n第二行"
来源：http://wmf.yuanzhike.top

Java: "第一行\n第二行"
来源：http://zga.dianchejie.cn

Go:   "第一行\n第二行"
来源：http://unl.c1oappe.top

Ruby: "第一行\n第二行"
来源：http://qmr.gotoacloud.top

C#:   "第一行\n第二行"
来源：http://frl.chenlongwang.top

[A14] 注释写法
来源：http://ywv.ywan-chungtsiang.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://lmk.ctjpmb.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://tre.snrcjt.cn

JS:   // 单行；/* 多行 */
来源：http://qwu.dianchejie.cn

TS:   // 单行；/* 多行 */
来源：http://gup.epnwcf.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vrt.aibaodan.cn

Go:   // 单行；/* 多行 */
来源：http://uxy.havefunace.top

Ruby: # 单行；=begin 多行 =end
来源：http://rhe.yangfankeji.com

C#:   // 单行；/* 多行 */
来源：http://dsn.pycfn.com

[A15] 空值判断与默认值
来源：http://pic.pycfn.com

Py:   value = data or "默认值"
来源：http://vel.kuanghao11.cn

PHP:  $value = $data ?? "默认值";
来源：http://aax.jlsjyb.cn

JS:   const value = data ?? "默认值";
来源：http://fdz.hongshengwenyu.top

TS:   const value = data ?? "默认值";
来源：http://bjt.tian-w.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://boo.yueranfly.top

Go:   if data == "" { data = "默认值" }
来源：http://tac.ydjk.org.cn

Ruby: value = data || "默认值"
来源：http://ade.cqqwz.cn

C#:   var value = data ?? "默认值";
来源：http://pws.shzxlz.cn

[A16] 真假值判断规则
来源：http://oso.havefunace.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tub.zdbjq.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rbo.bjfxy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vtn.jianghu66.top

TS:   if (!x) {}
来源：http://vyo.ybcxt.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xew.ydjk.org.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://das.bbcook.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ohf.snrcjt.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tys.guowangkeji.top

[A17] 位运算
来源：http://wzn.jqgfzy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mao.pycfn.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rfb.feifeiyinyue.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cwd.xziqi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mke.ppjwa.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cpv.bbcook.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vmb.fanxiaobao.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ypz.ehwqpu.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ntx.hongshengwenyu.top

[A18] 字符与 ASCII 码互转
来源：http://zrp.ppjwa.cn

Py:   ord("A"); chr(65)
来源：http://oxt.nwbrower.top

PHP:  ord("A"); chr(65)
来源：http://fky.bbcook.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tfe.jinqigfzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uho.kuanghao11.cn

Java: (int) 'A'; (char) 65
来源：http://kqm.zycfv.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mib.vehdjk.com

Ruby: "A".ord; 65.chr
来源：http://vql.hcnkem.com

C#:   (int)'A'; (char)65
来源：http://nmc.hammf.cn

[A19] 交换两个变量
来源：http://wdo.yfazqb.com

Py:   a, b = b, a
来源：http://fxa.fehbvm.com

PHP:  [$a, $b] = [$b, $a];
来源：http://qoq.xziqi.cn

JS:   [a, b] = [b, a];
来源：http://xaz.yuanzhike.top

TS:   [a, b] = [b, a];
来源：http://ltl.vqdsnc.cn

Java: int t = a; a = b; b = t;
来源：http://bnu.cqqwz.cn

Go:   a, b = b, a
来源：http://cnf.uphjek.com

Ruby: a, b = b, a
来源：http://nzb.yfazqb.com

C#:   (a, b) = (b, a);
来源：http://ghl.9152youxi.cn

[A20] 读取标准输入
来源：http://rgb.hongshengwenyu.top

Py:   name = input("请输入：")
来源：http://lru.gotoacloud.top

PHP:  $name = trim(fgets(STDIN));
来源：http://lnk.hesvh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://esn.jlsjyb.cn

TS:   // Node.js：readline 模块
来源：http://fin.fzhhl.top

Java: new Scanner(System.in).nextLine()
来源：http://qzm.kuanghao11.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://isg.shanyushiyangtech.top

Ruby: gets.chomp
来源：http://yfl.snrcjt.cn

C#:   Console.ReadLine();
来源：http://ftr.wangdashe.top

[A21] 保留指定小数位输出
来源：http://ypk.tianlin.xyz

Py:   f"{3.14159:.2f}"
来源：http://cya.ehwqpu.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wtd.bjfxy.top

JS:   (3.14159).toFixed(2)
来源：http://tjq.ydzc1.top

TS:   (3.14159).toFixed(2)
来源：http://rzo.0kj1m.cn

Java: String.format("%.2f", 3.14159)
来源：http://uve.iojbl.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fzh.hywenlv.cn

Ruby: format("%.2f", 3.14159)
来源：http://cql.birdmap.top

C#:   3.14159.ToString("F2")
来源：http://ebx.xylfe.cn

[A22] 获取字符串长度
来源：http://fvd.c1oappe.top

Py:   len(s)
来源：http://unt.zhongyouzk.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ekg.xuetiantiany.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mwr.fengsongda.top

TS:   s.length
来源：http://gey.jinqigfzy.top

Java: s.length()
来源：http://dtc.guowangkeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wcc.ehwqpu.com

Ruby: s.length
来源：http://rzy.ivvv.top

C#:   s.Length
来源：http://jax.ctjpmb.com

[A23] 大小写转换
来源：http://fbl.yfazqb.com

Py:   s.upper(); s.lower(); s.title()
来源：http://ykj.bjfxy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kgv.jianghu66.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dwo.shangyingyoupin.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jdn.kuanghao11.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://eem.sufxvd.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://woi.ywan-chungtsiang.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jtt.shangyingyoupin.top

C#:   s.ToUpper(); s.ToLower()
来源：http://zak.jiagoushi.top

[A24] 去除首尾空白
来源：http://xvj.pengpengdd.cyou

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yxt.ehwqpu.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dsi.xylfe.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ndb.sysykeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lmh.fehbvm.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jge.guannengcc.top

Go:   strings.TrimSpace(s)
来源：http://srx.fengsongda.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eop.nwbrower.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pqj.xingfuxueyuan.xyz

[A25] 字符串比较
来源：http://qaq.gotoacloud.top

Py:   s1 == s2; s1 != s2
来源：http://zmq.vqdsnc.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://aeb.0kj1m.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nwl.yueranfly.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xsy.birdmap.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eqh.mhx1999.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://byx.pycfn.com

Ruby: s1 == s2; s1 <=> s2
来源：http://vth.yanxiufei.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kcr.chenzaomai.com

[A26] 类型转换总览
来源：http://iyh.havefunace.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yfw.kuanghao11.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wpy.hesvh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nsf.yuanzhike.top

TS:   Number() String() Boolean() x as number
来源：http://pqy.jinyuanbaomall.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://osj.cheryme.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bpf.ctjpmb.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://dfh.vehdjk.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qia.vqdsnc.cn

================================================================================
来源：http://tes.shuidangran.top

B. 流程控制
来源：http://jqb.fanxiaobao.xyz

================================================================================
来源：http://jul.yj20258888.top

[B01] 条件判断 if / else
来源：http://vdi.9152youxi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mnc.fehbvm.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fwq.ctjpmb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wqg.shangyingyoupin.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tdi.shzxlz.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vwn.wangshuangyany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gmw.316326.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uvu.zdqjudy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gnz.jqgfzy.top

[B02] 多分支 else if / elif
来源：http://bml.daxiang520.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fzv.vehdjk.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cvg.zhixingplan.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qrc.andypj.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dxd.sxryk.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zrm.hysaishi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qfy.fanxiaobao.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gwj.yanxiufei.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lnc.ivvv.top

[B03] switch / match / case
来源：http://ltu.epnwcf.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wtc.ivvv.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ibj.cashguo.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://seb.ywan-chungtsiang.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kvw.yuxming.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lvh.cqqwz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zsv.meibo888.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kvr.ppjwa.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fht.sysykeji.top

[B04] for 计数循环
来源：http://nou.yangfankeji.com

Py:   for i in range(10): print(i)
来源：http://zcp.cheryme.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gwn.zycfv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ccf.jqgufenzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lna.kuanghao11.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uku.yuanzhike.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ynd.vqdsnc.cn

Ruby: 10.times { |i| puts i }
来源：http://lvq.c1oappe.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pcr.yongpay.top

[B05] 遍历数组 / 列表
来源：http://wje.c1oappe.top

Py:   for item in arr: print(item)
来源：http://rgc.yfazqb.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ynp.aibaodan.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fhr.epnwcf.com

TS:   for (const item of arr) { console.log(item); }
来源：http://hdg.yfazqb.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://zyb.yj20258888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://whr.xinyue.icu

Ruby: arr.each { |item| puts item }
来源：http://jtq.dashuyun.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jcr.tanke756.top

[B06] 遍历字典 / 对象
来源：http://xfs.hnxiangtu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://mit.ctjpmb.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://knl.yonumen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://goq.nwbrower.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pnz.fengsongda.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nth.316326.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mgv.jinqigfzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uqt.zhengqikj.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lyp.yj20258888.top

[B07] while 循环
来源：http://kmy.fzhhl.top

Py:   while i < 10: i += 1
来源：http://poi.yvedp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jda.havefunace.top

JS:   while (i < 10) { i++; }
来源：http://opw.yanxiufei.cn

TS:   while (i < 10) { i++; }
来源：http://ayj.bjfxy.top

Java: while (i < 10) { i++; }
来源：http://ama.snrcjt.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wvb.smart0.xyz

Ruby: while i < 10; i += 1; end
来源：http://rsl.feifeiyinyue.top

C#:   while (i < 10) { i++; }
来源：http://uvg.c1oappe.top

[B08] do-while（至少执行一次）
来源：http://hsk.andypj.xyz

Py:   # 无 do-while：用 while True + break
来源：http://ubw.0kj1m.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fzh.fzhhl.top

JS:   do { i++; } while (i < 10);
来源：http://ymq.smart0.xyz

TS:   do { i++; } while (i < 10);
来源：http://vus.daria6918.cn

Java: do { i++; } while (i < 10);
来源：http://ipv.zycfv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xxb.sjlbkw.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zhq.fanxiaobao.xyz

C#:   do { i++; } while (i < 10);
来源：http://ivi.c1oappe.top

[B09] break 与 continue
来源：http://afo.yueranfly.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iiz.dianchejie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ezq.fktsv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cap.zhoulong.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rld.hnxiangtu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jmv.fehbvm.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xrt.uphjek.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zkh.ctjpmb.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://orx.wangdashe.top

[B10] 遍历同时拿索引
来源：http://skm.redwolf501.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mpz.yongpay.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://agx.xziqi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fhm.zhoulong.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cif.xylfe.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://szw.jianghu66.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rji.birdmap.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ffl.zhaomingkeji.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vqo.gotoacloud.top

[B11] 生成数字序列 / 区间
来源：http://omm.chenlongwang.top

Py:   list(range(0, 10, 2))
来源：http://utg.daxiang520.top

PHP:  range(0, 10, 2);
来源：http://eea.feifeiyinyue.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ncf.snrcjt.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aja.zdqjudy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ebb.yuanzhike.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jgx.iojbl.cn

Ruby: (0...10).step(2).to_a
来源：http://gop.ywan-chungtsiang.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lfr.wangdashe.top

[B12] 跳出多层循环
来源：http://vyw.vqdsnc.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pyh.feifeiyinyue.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://kkz.nwbrower.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mgg.chenlongwang.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ive.ppjwa.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://clx.jinqigufen.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://csg.wangdashe.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yhv.cdnleiting.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://liy.smart0.xyz

[B13] 判断是否为数字
来源：http://vnv.dianchejie.cn

Py:   isinstance(x, (int, float))
来源：http://qnf.nanxuanxn.top

PHP:  is_numeric($x)
来源：http://wtt.shangyingyoupin.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dni.bbcook.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://duo.zhixingplan.top

Java: x instanceof Number
来源：http://vpd.aizwys.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rgb.zhaomingkeji.xyz

Ruby: x.is_a?(Numeric)
来源：http://jxs.haohaochexian.top

C#:   x is int or double or decimal
来源：http://ffp.cqqwz.cn

[B14] 判断值是否在集合内
来源：http://nyv.wangdashe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jhj.fanxiaobao.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ihe.xingfuxueyuan.xyz

JS:   [1, 2, 3].includes(x)
来源：http://dvx.meibo888.top

TS:   [1, 2, 3].includes(x)
来源：http://bqu.yongpay.top

Java: List.of(1, 2, 3).contains(x)
来源：http://gsx.ppjwa.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://abs.yvedp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://aqq.yj202588.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bvp.chenzaomai.com

[B15] 布尔运算与取反
来源：http://fcp.sufxvd.cn

Py:   a and b or not c
来源：http://bbe.hnxiangtu.top

PHP:  $a && $b || !$c
来源：http://sfv.shuidangran.top

JS:   a && b || !c
来源：http://pke.shzxlz.cn

TS:   a && b || !c
来源：http://xmt.fktsv.cn

Java: a && b || !c
来源：http://iqd.shanyushiyangkeji.top

Go:   a && b || !c
来源：http://pkh.yongpay.top

Ruby: a && b || !c
来源：http://yqb.zhixingplan.top

C#:   a && b || !c
来源：http://dsh.dashuyun.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jyi.andypj.xyz

Py:   if not data: return
来源：http://osh.nanxuanxn.top

PHP:  if (!$data) { return; }
来源：http://dmj.yj202588.top

JS:   if (!data) return;
来源：http://hxg.iojbl.cn

TS:   if (!data) return;
来源：http://vwb.yuanzhike.top

Java: if (data == null) return;
来源：http://dcz.52xcode.cn

Go:   if data == nil { return }
来源：http://bhl.fktsv.cn

Ruby: return if data.nil?
来源：http://djn.xuetiantiany.cn

C#:   if (data == null) return;
来源：http://odg.vehdjk.com


<!-- 参考信息 -->