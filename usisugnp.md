代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ybt.fengsongda.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://aqy.shzxlz.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kov.shanyushiyangkeji.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rib.nanxuanxn.top

[A10] 生成随机数
来源：http://mrt.tanke756.top

Py:   import random; random.randint(1, 100)
来源：http://zop.guannengcc.top

PHP:  random_int(1, 100);
来源：http://ufv.9152youxi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ian.jlsjyb.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ojh.jqgufenzy.top

Java: new Random().nextInt(100) + 1
来源：http://dgn.wangdashe.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qtf.chenlongwang.top

Ruby: rand(1..100)
来源：http://iub.aizwys.cn

C#:   new Random().Next(1, 101)
来源：http://raj.daria6918.cn

[A11] 条件表达式（三元）
来源：http://xmb.jinqigufen.top

Py:   "yes" if x > 0 else "no"
来源：http://yul.c1oappe.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://sqm.0kj1m.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bqd.hongshengwenyu.top

TS:   x > 0 ? "yes" : "no"
来源：http://ibn.xinyue.icu

Java: x > 0 ? "yes" : "no"
来源：http://iml.uphjek.com

Go:   // 无三元运算符，需用 if 语句
来源：http://ycl.redwolf501.top

Ruby: x > 0 ? "yes" : "no"
来源：http://dqq.zhongyouzk.top

C#:   x > 0 ? "yes" : "no"
来源：http://avo.wangdashe.top

[A12] 字符串插值 / 格式化
来源：http://iem.shanyushiyangtech.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://eqd.xingfuxueyuan.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fpo.cdnleiting.top

JS:   `Hello, ${name}!`
来源：http://fej.ppjwa.cn

TS:   `Hello, ${name}!`
来源：http://xwk.tian-w.cn

Java: "Hello, %s!".formatted(name)
来源：http://rhc.yj202588.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fsb.yongpay.top

Ruby: "Hello, #{name}!"
来源：http://ffa.jlsjyb.cn

C#:   $"Hello, {name}!"
来源：http://nop.cashguo.top

[A13] 多行字符串（练习 \n 转义）
来源：http://mip.guannengcc.top

Py:   "第一行\n第二行"
来源：http://zab.cdnleiting.top

PHP:  "第一行\n第二行"
来源：http://slo.vqdsnc.cn

JS:   "第一行\n第二行"
来源：http://dhs.iojbl.cn

TS:   "第一行\n第二行"
来源：http://xeh.yonumen.top

Java: "第一行\n第二行"
来源：http://utd.ivvv.top

Go:   "第一行\n第二行"
来源：http://cse.cheryme.top

Ruby: "第一行\n第二行"
来源：http://smj.sjlbkw.cn

C#:   "第一行\n第二行"
来源：http://qny.shanyushiyangtech.top

[A14] 注释写法
来源：http://cqx.zdqjudy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://txm.guowangkeji.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://gop.sysykeji.top

JS:   // 单行；/* 多行 */
来源：http://mms.cashguo.top

TS:   // 单行；/* 多行 */
来源：http://txv.jqgfzy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nlf.bbcook.cn

Go:   // 单行；/* 多行 */
来源：http://uip.vqdsnc.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vey.sweek.top

C#:   // 单行；/* 多行 */
来源：http://buf.tianlin.xyz

[A15] 空值判断与默认值
来源：http://rvg.gaohongyu789.top

Py:   value = data or "默认值"
来源：http://lsd.chenlongwang.top

PHP:  $value = $data ?? "默认值";
来源：http://ygd.dianchejie.cn

JS:   const value = data ?? "默认值";
来源：http://mwg.yongpay.top

TS:   const value = data ?? "默认值";
来源：http://nzf.tian-w.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ntf.gzhubu.top

Go:   if data == "" { data = "默认值" }
来源：http://psw.zdbjq.cn

Ruby: value = data || "默认值"
来源：http://xvy.yonumen.top

C#:   var value = data ?? "默认值";
来源：http://zoe.ivvv.top

[A16] 真假值判断规则
来源：http://elq.tian-w.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://enk.nanxuanxn.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vmz.yuxming.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://abd.ybcxt.top

TS:   if (!x) {}
来源：http://ijt.hnxiangtu.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jpi.nanxuanxn.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wvc.zhongyouzk.top

Ruby: unless x            # nil 与 false 为假
来源：http://acs.andypj.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ydt.yj20258888.top

[A17] 位运算
来源：http://coa.dashuyun.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yps.xuanzx.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ifz.tian-w.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yrg.hongshengwenyu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ezl.hesvh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rbe.vqdsnc.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kah.wangshuangyany.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ruy.iojbl.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://clw.hnxiangtu.top

[A18] 字符与 ASCII 码互转
来源：http://sbx.chenzaomai.com

Py:   ord("A"); chr(65)
来源：http://fvb.yj20258888.top

PHP:  ord("A"); chr(65)
来源：http://alq.sysykeji.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wvr.tanke756.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ywe.zhengqikj.top

Java: (int) 'A'; (char) 65
来源：http://tfx.zhongyouzk.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lrc.jyoumei.cn

Ruby: "A".ord; 65.chr
来源：http://uef.svipenyu.cn

C#:   (int)'A'; (char)65
来源：http://drn.fengsongda.top

[A19] 交换两个变量
来源：http://leq.shuidangran.top

Py:   a, b = b, a
来源：http://tkd.aibaodan.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://upl.zdqjudy.top

JS:   [a, b] = [b, a];
来源：http://dex.ydjk.org.cn

TS:   [a, b] = [b, a];
来源：http://joz.fktsv.cn

Java: int t = a; a = b; b = t;
来源：http://kxa.yj20258888.top

Go:   a, b = b, a
来源：http://tqq.ehwqpu.com

Ruby: a, b = b, a
来源：http://kwu.ppjwa.cn

C#:   (a, b) = (b, a);
来源：http://mto.daria6918.cn

[A20] 读取标准输入
来源：http://owb.jiagoushi.top

Py:   name = input("请输入：")
来源：http://umy.ctjpmb.com

PHP:  $name = trim(fgets(STDIN));
来源：http://uhz.shangyingyoupin.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://eri.wangdashe.top

TS:   // Node.js：readline 模块
来源：http://fbb.mhx1999.top

Java: new Scanner(System.in).nextLine()
来源：http://uvz.yangfankeji.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://prz.xingfuxueyuan.xyz

Ruby: gets.chomp
来源：http://piq.hnqzz.top

C#:   Console.ReadLine();
来源：http://utk.feifeiyinyue.top

[A21] 保留指定小数位输出
来源：http://lod.birdmap.top

Py:   f"{3.14159:.2f}"
来源：http://qhe.vehdjk.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gen.kuanghao11.cn

JS:   (3.14159).toFixed(2)
来源：http://qhp.tanke756.top

TS:   (3.14159).toFixed(2)
来源：http://gye.tanke756.top

Java: String.format("%.2f", 3.14159)
来源：http://gby.sweek.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://shs.wangdashe.top

Ruby: format("%.2f", 3.14159)
来源：http://gby.kuanghao11.cn

C#:   3.14159.ToString("F2")
来源：http://ehe.birdmap.top

[A22] 获取字符串长度
来源：http://gpw.nwbrower.top

Py:   len(s)
来源：http://aum.xuanzx.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lhd.bbcook.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mww.sufxvd.cn

TS:   s.length
来源：http://vio.fzhhl.top

Java: s.length()
来源：http://nym.snrcjt.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hae.andypj.xyz

Ruby: s.length
来源：http://vgn.zhongyouzk.top

C#:   s.Length
来源：http://evc.feifeiyinyue.top

[A23] 大小写转换
来源：http://zcd.vehdjk.com

Py:   s.upper(); s.lower(); s.title()
来源：http://kpy.zdbjq.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://oxl.vehdjk.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mca.hnqzz.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ddj.yonumen.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://eig.zhiwuduotai.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xae.gogol.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://emk.ydjk.org.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zet.shanyushiyangkeji.top

[A24] 去除首尾空白
来源：http://otx.zhijiandao.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vco.cucudq.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tag.guowangkeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tke.yanxiufei.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kpp.sysykeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jnl.hongshengwenyu.top

Go:   strings.TrimSpace(s)
来源：http://sat.yuanzhike.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ubb.vqdsnc.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://avc.jinghuilouyu.cn

[A25] 字符串比较
来源：http://ogs.cucudq.cn

Py:   s1 == s2; s1 != s2
来源：http://frs.dashuyun.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vav.xuetiantiany.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ykt.kuanghao11.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zdf.zhongyouzk.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oqs.birdmap.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://obn.316326.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://gum.zdbjq.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nfn.xylfe.cn

[A26] 类型转换总览
来源：http://tnk.0kj1m.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qxh.0kj1m.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lxm.sjlbkw.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pgm.cucudq.cn

TS:   Number() String() Boolean() x as number
来源：http://obl.ehwqpu.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hae.shangyingyoupin.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ovj.yj202588.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://wzz.hesvh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pmv.daxiang520.top

================================================================================
来源：http://npc.nanxuanxn.top

B. 流程控制
来源：http://ess.shanyushiyangkeji.top

================================================================================
来源：http://pnw.chenzaomai.com

[B01] 条件判断 if / else
来源：http://qwv.cucudq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://aek.hnqzz.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uvl.yongpay.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ioy.birdmap.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ucz.yuanzhike.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://wuu.ywan-chungtsiang.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zwr.wangshuangyany.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://whg.dashuyun.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zma.gzhubu.top

[B02] 多分支 else if / elif
来源：http://ils.uphjek.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://piq.snrcjt.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rqj.hongshengwenyu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mcv.sufxvd.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ard.tarul.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kws.sjlbkw.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wsn.jiagoushi.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://okj.andypj.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nlx.andypj.xyz

[B03] switch / match / case
来源：http://ttg.ctjpmb.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://geu.xziqi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wxq.52xcode.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zgm.zhoulong.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xlt.cucudq.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oed.shanyushiyangkeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lwr.bbcook.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xvc.fehbvm.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xjq.c1oappe.top

[B04] for 计数循环
来源：http://pwa.zdqjudy.top

Py:   for i in range(10): print(i)
来源：http://xij.fktsv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rqg.aibaodan.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://izf.snrcjt.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://drq.shzxlz.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sqf.feifeiyinyue.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bor.bjfxy.top

Ruby: 10.times { |i| puts i }
来源：http://xey.xinyue.icu

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://spz.ydzc1.top

[B05] 遍历数组 / 列表
来源：http://hju.svipenyu.cn

Py:   for item in arr: print(item)
来源：http://tqu.yongpay.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ans.zhengqikj.top

JS:   for (const item of arr) { console.log(item); }
来源：http://spk.iojbl.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vgp.52xcode.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://esy.jlsjyb.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lvd.sufxvd.cn

Ruby: arr.each { |item| puts item }
来源：http://mll.ywan-chungtsiang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://llb.yuanzhike.top

[B06] 遍历字典 / 对象
来源：http://ygy.ctjpmb.com

Py:   for k, v in d.items(): print(k, v)
来源：http://hjq.9152youxi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wyp.fzhhl.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wnv.pycfn.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xuk.meibo888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yhw.quarkkingdee.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oxs.yj20258888.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iwg.hywenlv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kvu.kuanghao11.cn

[B07] while 循环
来源：http://iyu.havefunace.top

Py:   while i < 10: i += 1
来源：http://irb.smart0.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://ncy.ydjk.org.cn

JS:   while (i < 10) { i++; }
来源：http://uhj.sjlbkw.cn

TS:   while (i < 10) { i++; }
来源：http://luy.fanxiaobao.xyz

Java: while (i < 10) { i++; }
来源：http://qgt.hcnkem.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://npc.hfpthk.cn

Ruby: while i < 10; i += 1; end
来源：http://mhy.jqgufenzy.top

C#:   while (i < 10) { i++; }
来源：http://ypc.pycfn.com

[B08] do-while（至少执行一次）
来源：http://vix.mhx1999.top

Py:   # 无 do-while：用 while True + break
来源：http://vhp.tanke756.top

PHP:  do { $i++; } while ($i < 10);
来源：http://hyq.ehwqpu.com

JS:   do { i++; } while (i < 10);
来源：http://nzq.cucudq.cn

TS:   do { i++; } while (i < 10);
来源：http://bfa.yj202588.top

Java: do { i++; } while (i < 10);
来源：http://epl.haohaochexian.top

Go:   for { i++; if i >= 10 { break } }
来源：http://rtr.xinyue.icu

Ruby: begin; i += 1; end while i < 10
来源：http://smj.ppjwa.cn

C#:   do { i++; } while (i < 10);
来源：http://rxv.tianlin.xyz

[B09] break 与 continue
来源：http://isq.zhoulong.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://you.chenlongwang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uvn.cashguo.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nrk.c1oappe.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fzd.xylfe.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vpn.pycfn.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://leb.nanxuanxn.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ssn.ppjwa.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aud.jiagoushi.top

[B10] 遍历同时拿索引
来源：http://xfs.zhiwuduotai.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zri.andypj.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kqr.hesvh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hnw.yj20258888.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://urx.fehbvm.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dcr.xuetiantiany.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jzv.ywan-chungtsiang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ejg.iojbl.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://eiq.hnxiangtu.top

[B11] 生成数字序列 / 区间
来源：http://zrr.birdmap.top

Py:   list(range(0, 10, 2))
来源：http://zjf.gotoacloud.top

PHP:  range(0, 10, 2);
来源：http://zcm.tian-w.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uck.epnwcf.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://enc.gaohongyu789.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ent.shzxlz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vag.mhx1999.top

Ruby: (0...10).step(2).to_a
来源：http://gaa.jqgufenzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gix.hnqzz.top

[B12] 跳出多层循环
来源：http://xgi.ppjwa.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://isk.nanxinkj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://jle.hysaishi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dai.nanxuanxn.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ofv.aibaodan.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oat.zhongyouzk.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gas.hammf.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ntm.52xcode.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xzv.ydzc1.top

[B13] 判断是否为数字
来源：http://rfx.cqqwz.cn

Py:   isinstance(x, (int, float))
来源：http://hng.dianchejie.cn

PHP:  is_numeric($x)
来源：http://meb.daxiang520.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mpc.ivvv.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ywg.xylfe.cn

Java: x instanceof Number
来源：http://bai.kuanghao11.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ocn.hysaishi.cn

Ruby: x.is_a?(Numeric)
来源：http://vpj.quarkkingdee.top

C#:   x is int or double or decimal
来源：http://qlq.dianchejie.cn

[B14] 判断值是否在集合内
来源：http://sot.ydjk.org.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yjp.gogol.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://iak.ivvv.top

JS:   [1, 2, 3].includes(x)
来源：http://quk.bbcook.cn

TS:   [1, 2, 3].includes(x)
来源：http://qsn.xingfuxueyuan.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://lij.gaohongyu789.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vak.zhijiandao.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yvc.vehdjk.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vfy.gotoacloud.top

[B15] 布尔运算与取反
来源：http://meq.fanxiaobao.xyz

Py:   a and b or not c
来源：http://phr.fehbvm.com

PHP:  $a && $b || !$c
来源：http://gdi.zhoulong.xyz

JS:   a && b || !c
来源：http://rue.fktsv.cn

TS:   a && b || !c
来源：http://voy.bjfxy.top

Java: a && b || !c
来源：http://otu.shangyingyoupin.top

Go:   a && b || !c
来源：http://zar.jlsjyb.cn

Ruby: a && b || !c
来源：http://tkn.svipenyu.cn

C#:   a && b || !c
来源：http://tih.nanxuanxn.top

[B16] 卫语句：不满足条件提前返回
来源：http://fmf.jinqigufen.top

Py:   if not data: return
来源：http://dws.hnqzz.top

PHP:  if (!$data) { return; }
来源：http://ska.cucudq.cn

JS:   if (!data) return;
来源：http://sca.zdqjudy.top

TS:   if (!data) return;
来源：http://uly.fktsv.cn


<!-- 参考信息 -->