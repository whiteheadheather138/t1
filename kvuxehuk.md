代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kug.tanke756.top

Java: new Random().nextInt(100) + 1
来源：http://pwx.hongshengwenyu.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ero.pycfn.com

Ruby: rand(1..100)
来源：http://nkx.hesvh.cn

C#:   new Random().Next(1, 101)
来源：http://mkz.yj20258888.top

[A11] 条件表达式（三元）
来源：http://ush.cashguo.top

Py:   "yes" if x > 0 else "no"
来源：http://mra.zdqjudy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ubc.mhx1999.top

JS:   x > 0 ? "yes" : "no"
来源：http://gjp.jiagoushi.top

TS:   x > 0 ? "yes" : "no"
来源：http://xot.hcnkem.com

Java: x > 0 ? "yes" : "no"
来源：http://rse.andypj.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://qzw.jlsjyb.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://swl.kuanghao11.cn

C#:   x > 0 ? "yes" : "no"
来源：http://pym.pycfn.com

[A12] 字符串插值 / 格式化
来源：http://bbq.pycfn.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ecs.shanyushiyangtech.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rmn.jinghuilouyu.cn

JS:   `Hello, ${name}!`
来源：http://mst.tianlin.xyz

TS:   `Hello, ${name}!`
来源：http://mlm.yvedp.cn

Java: "Hello, %s!".formatted(name)
来源：http://fco.vqdsnc.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xpr.shuidangran.top

Ruby: "Hello, #{name}!"
来源：http://qkw.sxryk.cn

C#:   $"Hello, {name}!"
来源：http://abf.cashguo.top

[A13] 多行字符串（练习 \n 转义）
来源：http://hbq.cashguo.top

Py:   "第一行\n第二行"
来源：http://frm.havefunace.top

PHP:  "第一行\n第二行"
来源：http://mdp.jlsjyb.cn

JS:   "第一行\n第二行"
来源：http://iof.dianchejie.cn

TS:   "第一行\n第二行"
来源：http://fvm.bbcook.cn

Java: "第一行\n第二行"
来源：http://eom.wangshuangyany.cn

Go:   "第一行\n第二行"
来源：http://zgh.xylfe.cn

Ruby: "第一行\n第二行"
来源：http://rpp.0kj1m.cn

C#:   "第一行\n第二行"
来源：http://nby.nanxuanxn.top

[A14] 注释写法
来源：http://hkn.316326.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://hrb.andypj.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://qad.sufxvd.cn

JS:   // 单行；/* 多行 */
来源：http://cwf.ppjwa.cn

TS:   // 单行；/* 多行 */
来源：http://avm.aizwys.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fft.snrcjt.cn

Go:   // 单行；/* 多行 */
来源：http://ugz.kuanghao11.cn

Ruby: # 单行；=begin 多行 =end
来源：http://cfx.zhoulong.xyz

C#:   // 单行；/* 多行 */
来源：http://llj.uphjek.com

[A15] 空值判断与默认值
来源：http://cpn.wangdashe.top

Py:   value = data or "默认值"
来源：http://yrw.xinyue.icu

PHP:  $value = $data ?? "默认值";
来源：http://zfx.dashuyun.cn

JS:   const value = data ?? "默认值";
来源：http://psc.ppjwa.cn

TS:   const value = data ?? "默认值";
来源：http://stx.zhongyouzk.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tjo.316326.xyz

Go:   if data == "" { data = "默认值" }
来源：http://zys.cheryme.top

Ruby: value = data || "默认值"
来源：http://oxt.zhoulong.xyz

C#:   var value = data ?? "默认值";
来源：http://kbh.hywenlv.cn

[A16] 真假值判断规则
来源：http://xle.yuanzhike.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://oys.9152youxi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mhj.cdnleiting.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://eyw.yangfankeji.com

TS:   if (!x) {}
来源：http://saf.feifeiyinyue.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lqm.ywan-chungtsiang.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://shz.fengsongda.top

Ruby: unless x            # nil 与 false 为假
来源：http://poq.fengsongda.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ykw.ctjpmb.com

[A17] 位运算
来源：http://ccd.fengsongda.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ieo.0kj1m.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pcy.sweek.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hyb.ywan-chungtsiang.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hwf.hnxiangtu.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bhg.tarul.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://joe.svipenyu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kah.hongshengwenyu.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bwk.haohaochexian.top

[A18] 字符与 ASCII 码互转
来源：http://dnr.tianlin.xyz

Py:   ord("A"); chr(65)
来源：http://kol.yj202588.top

PHP:  ord("A"); chr(65)
来源：http://hhk.ydjk.org.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ioi.birdmap.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fwl.ywan-chungtsiang.top

Java: (int) 'A'; (char) 65
来源：http://zox.mhx1999.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ytf.nanxuanxn.top

Ruby: "A".ord; 65.chr
来源：http://crt.sysykeji.top

C#:   (int)'A'; (char)65
来源：http://jtg.sysykeji.top

[A19] 交换两个变量
来源：http://qpt.shangyingyoupin.top

Py:   a, b = b, a
来源：http://bgb.pycfn.com

PHP:  [$a, $b] = [$b, $a];
来源：http://nmx.svipenyu.cn

JS:   [a, b] = [b, a];
来源：http://pti.feifeiyinyue.top

TS:   [a, b] = [b, a];
来源：http://tbf.yonumen.top

Java: int t = a; a = b; b = t;
来源：http://ylj.yongpay.top

Go:   a, b = b, a
来源：http://gwd.meibo888.top

Ruby: a, b = b, a
来源：http://xjy.daria6918.cn

C#:   (a, b) = (b, a);
来源：http://ers.cdnleiting.top

[A20] 读取标准输入
来源：http://auy.c1oappe.top

Py:   name = input("请输入：")
来源：http://wsr.gotoacloud.top

PHP:  $name = trim(fgets(STDIN));
来源：http://zia.redwolf501.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ybv.zhijiandao.cn

TS:   // Node.js：readline 模块
来源：http://qzy.chenjidiqi.icu

Java: new Scanner(System.in).nextLine()
来源：http://aho.ehwqpu.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ovs.jyoumei.cn

Ruby: gets.chomp
来源：http://ivq.shangyingyoupin.top

C#:   Console.ReadLine();
来源：http://rly.9152youxi.cn

[A21] 保留指定小数位输出
来源：http://myr.hnxiangtu.top

Py:   f"{3.14159:.2f}"
来源：http://wdm.sjlbkw.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://syn.andypj.xyz

JS:   (3.14159).toFixed(2)
来源：http://aks.daxiang520.top

TS:   (3.14159).toFixed(2)
来源：http://gun.vehdjk.com

Java: String.format("%.2f", 3.14159)
来源：http://eqp.nanxinkj.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gpm.shuidangran.top

Ruby: format("%.2f", 3.14159)
来源：http://ius.zhixingplan.top

C#:   3.14159.ToString("F2")
来源：http://jrs.ivvv.top

[A22] 获取字符串长度
来源：http://kjy.dianchejie.cn

Py:   len(s)
来源：http://nua.daria6918.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rwm.tianlin.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://upy.bbcook.cn

TS:   s.length
来源：http://rza.0kj1m.cn

Java: s.length()
来源：http://blh.guowangkeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dli.ivvv.top

Ruby: s.length
来源：http://rrl.nanxinkj.top

C#:   s.Length
来源：http://fmm.cdnleiting.top

[A23] 大小写转换
来源：http://zgc.c1oappe.top

Py:   s.upper(); s.lower(); s.title()
来源：http://shs.hcnkem.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://juq.c1oappe.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sdq.yvedp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hxf.9152youxi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lzn.hnxiangtu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qcc.aizwys.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bmv.fktsv.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gox.shzxlz.cn

[A24] 去除首尾空白
来源：http://ogg.jianghu66.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ojf.wangshuangyany.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bpo.zhijiandao.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://efh.jinqigufen.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fkh.snrcjt.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://alf.snrcjt.cn

Go:   strings.TrimSpace(s)
来源：http://jnw.daria6918.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zwu.tarul.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hgk.haohaochexian.top

[A25] 字符串比较
来源：http://wyx.shangyingyoupin.top

Py:   s1 == s2; s1 != s2
来源：http://esd.vqdsnc.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sbg.iojbl.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pui.zhixingplan.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://boe.zhongyouzk.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ymt.guowangkeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dqh.sufxvd.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lvf.hongshengwenyu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hgp.fktsv.cn

[A26] 类型转换总览
来源：http://dmy.vqdsnc.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://per.meibo888.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://klh.hnqzz.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vea.jinyuanbaomall.cn

TS:   Number() String() Boolean() x as number
来源：http://hdt.9152youxi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ttx.daxiang520.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nvo.jinqigfzy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://txw.ppjwa.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nqu.zdqjudy.top

================================================================================
来源：http://lvv.gotoacloud.top

B. 流程控制
来源：http://pxu.gzhubu.top

================================================================================
来源：http://oai.shzxlz.cn

[B01] 条件判断 if / else
来源：http://lxg.xinyue.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://gzb.guowangkeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://twp.sufxvd.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ixa.shangyingyoupin.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jyx.birdmap.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://drq.guowangkeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yxl.shuidangran.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uzf.zhaomingkeji.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wjt.chenzaomai.com

[B02] 多分支 else if / elif
来源：http://kwh.snrcjt.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kal.ydjk.org.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qrn.shanyushiyangkeji.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://esz.zhongyouzk.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://elf.xuetiantiany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://akl.jqgfzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://abs.daxiang520.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ydx.cucudq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hex.jinqigfzy.top

[B03] switch / match / case
来源：http://ncu.hammf.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://aay.xuetiantiany.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ozt.wangshuangyany.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yzs.uphjek.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vwu.zhixingplan.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xfz.ehwqpu.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sfz.cucudq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://enp.sysykeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ftf.mhx1999.top

[B04] for 计数循环
来源：http://feb.yfazqb.com

Py:   for i in range(10): print(i)
来源：http://xmz.ctjpmb.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://owp.yj20258888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sva.birdmap.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://arm.yj202588.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iii.ivvv.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jyz.zhiwuduotai.top

Ruby: 10.times { |i| puts i }
来源：http://yze.nanxuanxn.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kou.haohaochexian.top

[B05] 遍历数组 / 列表
来源：http://vgf.uphjek.com

Py:   for item in arr: print(item)
来源：http://bgf.yonumen.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://scz.hesvh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yha.xuetiantiany.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://uox.jlsjyb.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://stm.aizwys.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dpj.hongshengwenyu.top

Ruby: arr.each { |item| puts item }
来源：http://xak.xingfuxueyuan.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eqb.fehbvm.com

[B06] 遍历字典 / 对象
来源：http://pnj.0kj1m.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hud.yj20258888.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zzr.hnqzz.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xbg.epnwcf.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bti.gzhubu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hgw.birdmap.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rnf.zhaomingkeji.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qsu.xziqi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mwx.zhaomingkeji.xyz

[B07] while 循环
来源：http://hxq.jqgufenzy.top

Py:   while i < 10: i += 1
来源：http://pos.xinyue.icu

PHP:  while ($i < 10) { $i++; }
来源：http://kfq.smart0.xyz

JS:   while (i < 10) { i++; }
来源：http://zrv.jinghuilouyu.cn

TS:   while (i < 10) { i++; }
来源：http://dch.yj20258.top

Java: while (i < 10) { i++; }
来源：http://isw.feifeiyinyue.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://auu.chenlongwang.top

Ruby: while i < 10; i += 1; end
来源：http://pbf.jianghu66.top

C#:   while (i < 10) { i++; }
来源：http://lvb.svipenyu.cn

[B08] do-while（至少执行一次）
来源：http://fnb.jyoumei.cn

Py:   # 无 do-while：用 while True + break
来源：http://djf.zhaomingkeji.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://xgg.hcnkem.com

JS:   do { i++; } while (i < 10);
来源：http://ayv.fktsv.cn

TS:   do { i++; } while (i < 10);
来源：http://maa.yj202588.top

Java: do { i++; } while (i < 10);
来源：http://sdg.mhx1999.top

Go:   for { i++; if i >= 10 { break } }
来源：http://buh.ybcxt.top

Ruby: begin; i += 1; end while i < 10
来源：http://iiy.mhx1999.top

C#:   do { i++; } while (i < 10);
来源：http://ifj.tianlin.xyz

[B09] break 与 continue
来源：http://hfk.cucudq.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://the.yj20258888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bnc.9152youxi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tbm.smart0.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://isx.chenjidiqi.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vae.fengsongda.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ihv.dashuyun.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wje.yvedp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://czh.ctjpmb.com

[B10] 遍历同时拿索引
来源：http://rjv.vqdsnc.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://feh.jlsjyb.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://acl.cdnleiting.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yeo.mhx1999.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cjy.gogol.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hab.fengsongda.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lfh.epnwcf.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jra.yj20258.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iqe.52xcode.cn

[B11] 生成数字序列 / 区间
来源：http://csw.c1oappe.top

Py:   list(range(0, 10, 2))
来源：http://bui.yuanzhike.top

PHP:  range(0, 10, 2);
来源：http://udj.haohaochexian.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xxl.hnqzz.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yck.fehbvm.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vmu.meibo888.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bll.sufxvd.cn

Ruby: (0...10).step(2).to_a
来源：http://hsk.sysykeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lcd.sysykeji.top

[B12] 跳出多层循环
来源：http://qnn.redwolf501.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://mcw.ehwqpu.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://vov.birdmap.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://msn.kuanghao11.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ihb.ydjk.org.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://unc.yuanzhike.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ahy.snrcjt.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dss.hesvh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uhg.smart0.xyz

[B13] 判断是否为数字
来源：http://rcu.fanxiaobao.xyz

Py:   isinstance(x, (int, float))
来源：http://okk.c1oappe.top

PHP:  is_numeric($x)
来源：http://qon.ydzc1.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://imy.hcnkem.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uyv.epnwcf.com

Java: x instanceof Number
来源：http://zni.hfpthk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gss.yueranfly.top

Ruby: x.is_a?(Numeric)
来源：http://bac.yongpay.top

C#:   x is int or double or decimal
来源：http://crw.fengsongda.top

[B14] 判断值是否在集合内
来源：http://wil.xinyue.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kuo.yuxming.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oiz.fanxiaobao.xyz

JS:   [1, 2, 3].includes(x)
来源：http://eaj.fehbvm.com

TS:   [1, 2, 3].includes(x)
来源：http://ujy.52xcode.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dkr.hesvh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hqt.uphjek.com

Ruby: [1, 2, 3].include?(x)
来源：http://eyr.snrcjt.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ohv.wangdashe.top

[B15] 布尔运算与取反
来源：http://dnj.iojbl.cn

Py:   a and b or not c
来源：http://bts.chenlongwang.top

PHP:  $a && $b || !$c
来源：http://sem.epnwcf.com

JS:   a && b || !c
来源：http://ayx.snrcjt.cn

TS:   a && b || !c
来源：http://frx.yj20258.top

Java: a && b || !c
来源：http://ocg.yfazqb.com

Go:   a && b || !c
来源：http://hqq.jqgufenzy.top

Ruby: a && b || !c
来源：http://ony.daxiang520.top

C#:   a && b || !c
来源：http://yya.hcnkem.com

[B16] 卫语句：不满足条件提前返回
来源：http://gnv.feifeiyinyue.top

Py:   if not data: return
来源：http://uqv.vehdjk.com

PHP:  if (!$data) { return; }
来源：http://fdz.jyoumei.cn

JS:   if (!data) return;
来源：http://wrp.gotoacloud.top

TS:   if (!data) return;
来源：http://tyd.redwolf501.top

Java: if (data == null) return;
来源：http://gzj.snrcjt.cn

Go:   if data == nil { return }
来源：http://wgn.jinghuilouyu.cn

Ruby: return if data.nil?
来源：http://bmh.yj20258.top

C#:   if (data == null) return;
来源：http://yjd.vehdjk.com

================================================================================
来源：http://hli.daria6918.cn

C. 函数与作用域
来源：http://pft.jlsjyb.cn

================================================================================
来源：http://lwd.jyoumei.cn

[C01] 定义函数
来源：http://phy.birdmap.top


<!-- 参考信息 -->