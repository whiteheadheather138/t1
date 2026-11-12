代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ipy.bjfxy.top

Java: new Random().nextInt(100) + 1
来源：http://gaf.iojbl.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dkv.shuidangran.top

Ruby: rand(1..100)
来源：http://xmw.tanke756.top

C#:   new Random().Next(1, 101)
来源：http://txh.jyoumei.cn

[A11] 条件表达式（三元）
来源：http://otq.zhengqikj.top

Py:   "yes" if x > 0 else "no"
来源：http://irt.wangdashe.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://wbk.shanyushiyangtech.top

JS:   x > 0 ? "yes" : "no"
来源：http://vhj.yvedp.cn

TS:   x > 0 ? "yes" : "no"
来源：http://pzl.kuanghao11.cn

Java: x > 0 ? "yes" : "no"
来源：http://opx.yonumen.top

Go:   // 无三元运算符，需用 if 语句
来源：http://rhu.shanyushiyangkeji.top

Ruby: x > 0 ? "yes" : "no"
来源：http://amb.jianghu66.top

C#:   x > 0 ? "yes" : "no"
来源：http://lqd.shanyushiyangtech.top

[A12] 字符串插值 / 格式化
来源：http://zxz.ehwqpu.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rvt.sweek.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gjr.dianchejie.cn

JS:   `Hello, ${name}!`
来源：http://pxl.cqqwz.cn

TS:   `Hello, ${name}!`
来源：http://cvj.9152youxi.cn

Java: "Hello, %s!".formatted(name)
来源：http://xge.hammf.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://emg.pycfn.com

Ruby: "Hello, #{name}!"
来源：http://xbs.fzhhl.top

C#:   $"Hello, {name}!"
来源：http://gkf.shuidangran.top

[A13] 多行字符串（练习 \n 转义）
来源：http://qjg.wangshuangyany.cn

Py:   "第一行\n第二行"
来源：http://zmk.chenlongwang.top

PHP:  "第一行\n第二行"
来源：http://hqq.hammf.cn

JS:   "第一行\n第二行"
来源：http://qve.ppjwa.cn

TS:   "第一行\n第二行"
来源：http://eoy.hcnkem.com

Java: "第一行\n第二行"
来源：http://ccl.nanxinkj.top

Go:   "第一行\n第二行"
来源：http://wwb.nanxinkj.top

Ruby: "第一行\n第二行"
来源：http://exr.jyoumei.cn

C#:   "第一行\n第二行"
来源：http://nfz.shuidangran.top

[A14] 注释写法
来源：http://nfd.mhx1999.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://svx.shanyushiyangtech.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://xqx.yonumen.top

JS:   // 单行；/* 多行 */
来源：http://iog.fehbvm.com

TS:   // 单行；/* 多行 */
来源：http://msi.c1oappe.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jkv.zdbjq.cn

Go:   // 单行；/* 多行 */
来源：http://kec.sxryk.cn

Ruby: # 单行；=begin 多行 =end
来源：http://caw.jqgfzy.top

C#:   // 单行；/* 多行 */
来源：http://skl.ydjk.org.cn

[A15] 空值判断与默认值
来源：http://cfp.shuidangran.top

Py:   value = data or "默认值"
来源：http://icj.hongshengwenyu.top

PHP:  $value = $data ?? "默认值";
来源：http://lqs.zhijiandao.cn

JS:   const value = data ?? "默认值";
来源：http://qne.xziqi.cn

TS:   const value = data ?? "默认值";
来源：http://voe.yongpay.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://drz.yongpay.top

Go:   if data == "" { data = "默认值" }
来源：http://tjd.tarul.cn

Ruby: value = data || "默认值"
来源：http://rbw.wangdashe.top

C#:   var value = data ?? "默认值";
来源：http://atm.fktsv.cn

[A16] 真假值判断规则
来源：http://gjm.havefunace.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://izv.cashguo.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wkd.ybcxt.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dcp.hammf.cn

TS:   if (!x) {}
来源：http://egc.zhengqikj.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gie.tanke756.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fqe.yueranfly.top

Ruby: unless x            # nil 与 false 为假
来源：http://nhj.yj202588.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mli.jinghuilouyu.cn

[A17] 位运算
来源：http://vsz.fengsongda.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pnh.ctjpmb.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://npi.gaohongyu789.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eks.andypj.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zjf.jinyuanbaomall.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://psl.xinyue.icu

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nyf.cheryme.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jyo.zhiwuduotai.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://icf.haohaochexian.top

[A18] 字符与 ASCII 码互转
来源：http://srq.shuidangran.top

Py:   ord("A"); chr(65)
来源：http://rew.fanxiaobao.xyz

PHP:  ord("A"); chr(65)
来源：http://pot.hysaishi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ixo.tarul.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rbj.hongshengwenyu.top

Java: (int) 'A'; (char) 65
来源：http://sqw.jinqigfzy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ont.tianlin.xyz

Ruby: "A".ord; 65.chr
来源：http://csb.ctjpmb.com

C#:   (int)'A'; (char)65
来源：http://yaj.chenlongwang.top

[A19] 交换两个变量
来源：http://wzx.vehdjk.com

Py:   a, b = b, a
来源：http://zpz.hongshengwenyu.top

PHP:  [$a, $b] = [$b, $a];
来源：http://fgf.aibaodan.cn

JS:   [a, b] = [b, a];
来源：http://rfp.guowangkeji.top

TS:   [a, b] = [b, a];
来源：http://mfy.hnqzz.top

Java: int t = a; a = b; b = t;
来源：http://uco.wangdashe.top

Go:   a, b = b, a
来源：http://zcd.yj20258.top

Ruby: a, b = b, a
来源：http://lrl.havefunace.top

C#:   (a, b) = (b, a);
来源：http://clj.wangshuangyany.cn

[A20] 读取标准输入
来源：http://ttg.zdbjq.cn

Py:   name = input("请输入：")
来源：http://kiq.yj20258.top

PHP:  $name = trim(fgets(STDIN));
来源：http://vmr.zhoulong.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dyf.zhaomingkeji.xyz

TS:   // Node.js：readline 模块
来源：http://wem.jinghuilouyu.cn

Java: new Scanner(System.in).nextLine()
来源：http://mgb.birdmap.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fcn.shangyingyoupin.top

Ruby: gets.chomp
来源：http://vzo.bbcook.cn

C#:   Console.ReadLine();
来源：http://bzs.nwbrower.top

[A21] 保留指定小数位输出
来源：http://wbp.c1oappe.top

Py:   f"{3.14159:.2f}"
来源：http://fnv.0kj1m.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lxe.haohaochexian.top

JS:   (3.14159).toFixed(2)
来源：http://tcj.bjfxy.top

TS:   (3.14159).toFixed(2)
来源：http://lyr.c1oappe.top

Java: String.format("%.2f", 3.14159)
来源：http://cgs.jinqigufen.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yuc.52xcode.cn

Ruby: format("%.2f", 3.14159)
来源：http://irz.smart0.xyz

C#:   3.14159.ToString("F2")
来源：http://mtp.vqdsnc.cn

[A22] 获取字符串长度
来源：http://jsm.chenjidiqi.icu

Py:   len(s)
来源：http://mvl.sjlbkw.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://aha.wangdashe.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mhg.fengsongda.top

TS:   s.length
来源：http://ljp.xinyue.icu

Java: s.length()
来源：http://hzr.ehwqpu.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://clh.xuetiantiany.cn

Ruby: s.length
来源：http://vhd.ywan-chungtsiang.top

C#:   s.Length
来源：http://veo.aibaodan.cn

[A23] 大小写转换
来源：http://ail.gzhubu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://lhz.andypj.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yuz.guannengcc.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://brz.kuanghao11.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vfy.fehbvm.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bqu.quarkkingdee.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zel.jqgfzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ucl.mhx1999.top

C#:   s.ToUpper(); s.ToLower()
来源：http://abr.yueranfly.top

[A24] 去除首尾空白
来源：http://dir.feifeiyinyue.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://riz.pycfn.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dwb.316326.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lxo.gotoacloud.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hfp.wangdashe.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fov.daria6918.cn

Go:   strings.TrimSpace(s)
来源：http://mwh.cheryme.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://svg.jinyuanbaomall.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mhb.zycfv.cn

[A25] 字符串比较
来源：http://tch.haohaochexian.top

Py:   s1 == s2; s1 != s2
来源：http://cix.jinghuilouyu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vtw.andypj.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dha.tian-w.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qpq.sysykeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://brp.jinqigfzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ngk.sufxvd.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pze.jianghu66.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jaw.yonumen.top

[A26] 类型转换总览
来源：http://jcb.chenjidiqi.icu

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bma.jianghu66.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wze.epnwcf.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yvc.jinqigfzy.top

TS:   Number() String() Boolean() x as number
来源：http://cgc.xinyue.icu

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dca.dianchejie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xxu.hfpthk.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://caa.hammf.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wwd.sufxvd.cn

================================================================================
来源：http://twf.nanxuanxn.top

B. 流程控制
来源：http://gak.yvedp.cn

================================================================================
来源：http://mzc.fktsv.cn

[B01] 条件判断 if / else
来源：http://trc.sysykeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://tkl.yvedp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://amr.daxiang520.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fwe.cdnleiting.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qul.yuanzhike.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://inj.fengsongda.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xba.yangfankeji.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tmu.gzhubu.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ibq.hysaishi.cn

[B02] 多分支 else if / elif
来源：http://cbz.zhixingplan.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ibx.kuanghao11.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vbl.ctjpmb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dco.hfpthk.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ogc.yj20258888.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://idh.redwolf501.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://res.xinyue.icu

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tbd.xinyue.icu

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yuo.cashguo.top

[B03] switch / match / case
来源：http://zpk.52xcode.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xnf.bjfxy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pxm.andypj.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qkh.jyoumei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qzy.hywenlv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://inr.chenzaomai.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zye.jiagoushi.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ogv.jinghuilouyu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://eym.svipenyu.cn

[B04] for 计数循环
来源：http://qlq.ppjwa.cn

Py:   for i in range(10): print(i)
来源：http://plx.pycfn.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ytl.52xcode.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kwh.gaohongyu789.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cgl.yongpay.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kys.nanxuanxn.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wzm.ehwqpu.com

Ruby: 10.times { |i| puts i }
来源：http://lvs.epnwcf.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://szk.fehbvm.com

[B05] 遍历数组 / 列表
来源：http://goy.yvedp.cn

Py:   for item in arr: print(item)
来源：http://icq.gogol.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hut.fanxiaobao.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://chn.jinghuilouyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lhl.yueranfly.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://gha.bjfxy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fwi.wangdashe.top

Ruby: arr.each { |item| puts item }
来源：http://eoe.snrcjt.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qmv.yj20258.top

[B06] 遍历字典 / 对象
来源：http://zjz.zhaomingkeji.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://zhk.xuanzx.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wuw.c1oappe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oyi.shangyingyoupin.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wjc.yongpay.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bcc.wangdashe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://edo.yfazqb.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://edc.zycfv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uum.shuidangran.top

[B07] while 循环
来源：http://vjr.yonumen.top

Py:   while i < 10: i += 1
来源：http://ngv.aibaodan.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fcd.ydzc1.top

JS:   while (i < 10) { i++; }
来源：http://fur.cqqwz.cn

TS:   while (i < 10) { i++; }
来源：http://jen.birdmap.top

Java: while (i < 10) { i++; }
来源：http://wyh.iojbl.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ltu.ehwqpu.com

Ruby: while i < 10; i += 1; end
来源：http://ony.zhoulong.xyz

C#:   while (i < 10) { i++; }
来源：http://zrj.fzhhl.top

[B08] do-while（至少执行一次）
来源：http://qtx.tianlin.xyz

Py:   # 无 do-while：用 while True + break
来源：http://cwv.shanyushiyangtech.top

PHP:  do { $i++; } while ($i < 10);
来源：http://cay.havefunace.top

JS:   do { i++; } while (i < 10);
来源：http://znb.bjfxy.top

TS:   do { i++; } while (i < 10);
来源：http://oqj.ehwqpu.com

Java: do { i++; } while (i < 10);
来源：http://yvg.jqgfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hgx.daria6918.cn

Ruby: begin; i += 1; end while i < 10
来源：http://afg.fzhhl.top

C#:   do { i++; } while (i < 10);
来源：http://lqu.ydjk.org.cn

[B09] break 与 continue
来源：http://gau.zhongyouzk.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://boh.hcnkem.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bkg.gogol.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://prs.birdmap.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jno.hfpthk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hzp.jqgfzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uaf.zhijiandao.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kmn.redwolf501.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://idx.zdbjq.cn

[B10] 遍历同时拿索引
来源：http://ijt.yonumen.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zza.fengsongda.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jhh.sjlbkw.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cuz.haohaochexian.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nud.zdbjq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ifq.cashguo.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tbw.ybcxt.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sme.sjlbkw.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qon.ydjk.org.cn

[B11] 生成数字序列 / 区间
来源：http://jfb.bjfxy.top

Py:   list(range(0, 10, 2))
来源：http://ttj.fengsongda.top

PHP:  range(0, 10, 2);
来源：http://ezq.gzhubu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iwd.bjfxy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qeg.cqqwz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fxy.ydzc1.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wgp.hnqzz.top

Ruby: (0...10).step(2).to_a
来源：http://kqf.xylfe.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://poi.jinqigfzy.top

[B12] 跳出多层循环
来源：http://ier.gaohongyu789.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ykl.316326.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://hfg.sweek.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jlf.zhongyouzk.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://grq.andypj.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dks.hnqzz.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://glg.fanxiaobao.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gwn.yonumen.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://geg.yangfankeji.com

[B13] 判断是否为数字
来源：http://alb.sweek.top

Py:   isinstance(x, (int, float))
来源：http://bbr.cdnleiting.top

PHP:  is_numeric($x)
来源：http://gyh.sufxvd.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vql.yfazqb.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ffo.ehwqpu.com

Java: x instanceof Number
来源：http://qkt.yanxiufei.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://van.shzxlz.cn

Ruby: x.is_a?(Numeric)
来源：http://gdu.zhaomingkeji.xyz

C#:   x is int or double or decimal
来源：http://zoj.pycfn.com

[B14] 判断值是否在集合内
来源：http://qfb.feifeiyinyue.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rib.fehbvm.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lgi.ywan-chungtsiang.top

JS:   [1, 2, 3].includes(x)
来源：http://kjf.ydzc1.top

TS:   [1, 2, 3].includes(x)
来源：http://ngx.hysaishi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://smi.jqgfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://asm.aizwys.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mfr.hesvh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qjh.shanyushiyangkeji.top

[B15] 布尔运算与取反
来源：http://snp.daxiang520.top

Py:   a and b or not c
来源：http://nyw.guowangkeji.top

PHP:  $a && $b || !$c
来源：http://njw.ywan-chungtsiang.top

JS:   a && b || !c
来源：http://qll.birdmap.top

TS:   a && b || !c
来源：http://bea.zhongyouzk.top

Java: a && b || !c
来源：http://xsx.tianlin.xyz

Go:   a && b || !c
来源：http://sqj.cashguo.top

Ruby: a && b || !c
来源：http://aem.chenzaomai.com

C#:   a && b || !c
来源：http://tak.xziqi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dxo.ydzc1.top

Py:   if not data: return
来源：http://dau.dianchejie.cn

PHP:  if (!$data) { return; }
来源：http://qhl.daria6918.cn

JS:   if (!data) return;
来源：http://eeb.hesvh.cn

TS:   if (!data) return;
来源：http://yoz.sufxvd.cn

Java: if (data == null) return;
来源：http://xah.iojbl.cn

Go:   if data == nil { return }
来源：http://shy.jiagoushi.top

Ruby: return if data.nil?
来源：http://ptv.hnxiangtu.top

C#:   if (data == null) return;
来源：http://mjb.redwolf501.top

================================================================================
来源：http://opm.xziqi.cn

C. 函数与作用域
来源：http://oej.chenlongwang.top

================================================================================
来源：http://udg.ppjwa.cn

[C01] 定义函数
来源：http://vux.tanke756.top


<!-- 参考信息 -->