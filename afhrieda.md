代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nbq.iojbl.cn

Java: new Random().nextInt(100) + 1
来源：http://ebh.tarul.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xzd.xziqi.cn

Ruby: rand(1..100)
来源：http://cst.zhijiandao.cn

C#:   new Random().Next(1, 101)
来源：http://nqp.chenzaomai.com

[A11] 条件表达式（三元）
来源：http://sou.birdmap.top

Py:   "yes" if x > 0 else "no"
来源：http://rvp.jinghuilouyu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://whf.ydjk.org.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bkl.316326.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://tqr.yuanzhike.top

Java: x > 0 ? "yes" : "no"
来源：http://kfv.meibo888.top

Go:   // 无三元运算符，需用 if 语句
来源：http://fds.hesvh.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ufn.cashguo.top

C#:   x > 0 ? "yes" : "no"
来源：http://qld.xziqi.cn

[A12] 字符串插值 / 格式化
来源：http://nyu.epnwcf.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wts.gzhubu.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pid.aizwys.cn

JS:   `Hello, ${name}!`
来源：http://fsf.dianchejie.cn

TS:   `Hello, ${name}!`
来源：http://tdz.yuxming.cn

Java: "Hello, %s!".formatted(name)
来源：http://cpn.fzhhl.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xcd.ivvv.top

Ruby: "Hello, #{name}!"
来源：http://spz.ywan-chungtsiang.top

C#:   $"Hello, {name}!"
来源：http://vtg.daria6918.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hxm.bbcook.cn

Py:   "第一行\n第二行"
来源：http://abe.uphjek.com

PHP:  "第一行\n第二行"
来源：http://epz.aibaodan.cn

JS:   "第一行\n第二行"
来源：http://gep.ydjk.org.cn

TS:   "第一行\n第二行"
来源：http://zib.pengpengdd.cyou

Java: "第一行\n第二行"
来源：http://ive.redwolf501.top

Go:   "第一行\n第二行"
来源：http://iwf.wangdashe.top

Ruby: "第一行\n第二行"
来源：http://rgn.hesvh.cn

C#:   "第一行\n第二行"
来源：http://uqp.sjlbkw.cn

[A14] 注释写法
来源：http://fal.sysykeji.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://qia.jianghu66.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://wyb.hesvh.cn

JS:   // 单行；/* 多行 */
来源：http://syj.52xcode.cn

TS:   // 单行；/* 多行 */
来源：http://ppa.ydjk.org.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fat.meibo888.top

Go:   // 单行；/* 多行 */
来源：http://gvr.yfazqb.com

Ruby: # 单行；=begin 多行 =end
来源：http://tex.cheryme.top

C#:   // 单行；/* 多行 */
来源：http://dmd.jlsjyb.cn

[A15] 空值判断与默认值
来源：http://svb.jinghuilouyu.cn

Py:   value = data or "默认值"
来源：http://lhl.zdqjudy.top

PHP:  $value = $data ?? "默认值";
来源：http://xgi.jinqigfzy.top

JS:   const value = data ?? "默认值";
来源：http://cwt.jiagoushi.top

TS:   const value = data ?? "默认值";
来源：http://bji.haohaochexian.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xre.shzxlz.cn

Go:   if data == "" { data = "默认值" }
来源：http://qcm.daria6918.cn

Ruby: value = data || "默认值"
来源：http://oku.daria6918.cn

C#:   var value = data ?? "默认值";
来源：http://kzm.sjlbkw.cn

[A16] 真假值判断规则
来源：http://guu.andypj.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fkc.smart0.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ytl.tianlin.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pfu.vqdsnc.cn

TS:   if (!x) {}
来源：http://uoq.feifeiyinyue.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cpj.dashuyun.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qcs.tian-w.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ibv.uphjek.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lpt.feifeiyinyue.top

[A17] 位运算
来源：http://rne.dianchejie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jas.hesvh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fpg.shangyingyoupin.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kbw.chenjidiqi.icu

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lkz.hesvh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vgi.svipenyu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://aaz.shzxlz.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nix.ydzc1.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sme.guannengcc.top

[A18] 字符与 ASCII 码互转
来源：http://vbl.tian-w.cn

Py:   ord("A"); chr(65)
来源：http://ztl.quarkkingdee.top

PHP:  ord("A"); chr(65)
来源：http://xgy.zhoulong.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://eny.xylfe.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ida.xingfuxueyuan.xyz

Java: (int) 'A'; (char) 65
来源：http://hht.pengpengdd.cyou

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hrw.gogol.net.cn

Ruby: "A".ord; 65.chr
来源：http://xox.daxiang520.top

C#:   (int)'A'; (char)65
来源：http://zdq.cheryme.top

[A19] 交换两个变量
来源：http://ekz.shuidangran.top

Py:   a, b = b, a
来源：http://xqf.xuetiantiany.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xap.wangdashe.top

JS:   [a, b] = [b, a];
来源：http://xbf.jinqigfzy.top

TS:   [a, b] = [b, a];
来源：http://zoy.iojbl.cn

Java: int t = a; a = b; b = t;
来源：http://foh.hcnkem.com

Go:   a, b = b, a
来源：http://fks.hammf.cn

Ruby: a, b = b, a
来源：http://csi.svipenyu.cn

C#:   (a, b) = (b, a);
来源：http://sli.andypj.xyz

[A20] 读取标准输入
来源：http://hrx.9152youxi.cn

Py:   name = input("请输入：")
来源：http://gwc.xinyue.icu

PHP:  $name = trim(fgets(STDIN));
来源：http://utm.dianchejie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zbx.dashuyun.cn

TS:   // Node.js：readline 模块
来源：http://izp.pycfn.com

Java: new Scanner(System.in).nextLine()
来源：http://hrd.aizwys.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nsf.xuanzx.com

Ruby: gets.chomp
来源：http://wif.quarkkingdee.top

C#:   Console.ReadLine();
来源：http://eqo.daria6918.cn

[A21] 保留指定小数位输出
来源：http://usz.epnwcf.com

Py:   f"{3.14159:.2f}"
来源：http://mxa.yj20258888.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kff.xuetiantiany.cn

JS:   (3.14159).toFixed(2)
来源：http://ylf.sufxvd.cn

TS:   (3.14159).toFixed(2)
来源：http://yvv.hongshengwenyu.top

Java: String.format("%.2f", 3.14159)
来源：http://lej.nanxuanxn.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://reo.jianghu66.top

Ruby: format("%.2f", 3.14159)
来源：http://xjj.xuetiantiany.cn

C#:   3.14159.ToString("F2")
来源：http://aqm.hcnkem.com

[A22] 获取字符串长度
来源：http://qqx.ydjk.org.cn

Py:   len(s)
来源：http://rwm.ctjpmb.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hlu.ydjk.org.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://enj.zdbjq.cn

TS:   s.length
来源：http://mdd.zhaomingkeji.xyz

Java: s.length()
来源：http://fpz.vehdjk.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xrz.cucudq.cn

Ruby: s.length
来源：http://sod.sjlbkw.cn

C#:   s.Length
来源：http://aqb.svipenyu.cn

[A23] 大小写转换
来源：http://smu.xingfuxueyuan.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://yhg.xuanzx.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ohr.sysykeji.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://psa.aibaodan.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qey.gzhubu.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yiz.cdnleiting.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vpc.dianchejie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dhq.hfpthk.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://djt.yj202588.top

[A24] 去除首尾空白
来源：http://xls.cheryme.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pgp.chenjidiqi.icu

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://prl.nanxinkj.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ahw.nanxinkj.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xjn.zdbjq.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lbm.tian-w.cn

Go:   strings.TrimSpace(s)
来源：http://qla.yongpay.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lji.quarkkingdee.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rti.yuxming.cn

[A25] 字符串比较
来源：http://lru.zhengqikj.top

Py:   s1 == s2; s1 != s2
来源：http://gyw.jqgufenzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jfx.bjfxy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xnq.zdbjq.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://moy.hywenlv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rkc.jyoumei.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uhr.daria6918.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jqs.jqgufenzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xpx.meibo888.top

[A26] 类型转换总览
来源：http://mth.xuanzx.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ufi.vqdsnc.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uyl.pengpengdd.cyou

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rkd.aibaodan.cn

TS:   Number() String() Boolean() x as number
来源：http://wzt.sxryk.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pbh.feifeiyinyue.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sot.cheryme.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://txh.pengpengdd.cyou

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vfe.svipenyu.cn

================================================================================
来源：http://khl.zdbjq.cn

B. 流程控制
来源：http://gpx.zhixingplan.top

================================================================================
来源：http://fuo.ivvv.top

[B01] 条件判断 if / else
来源：http://dmw.uphjek.com

Py:   result = "正" if x > 0 else "非正"
来源：http://fvr.andypj.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zxy.gotoacloud.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iyj.zhijiandao.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tal.shangyingyoupin.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jrf.svipenyu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dnb.jinghuilouyu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dbp.nanxinkj.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gml.ybcxt.top

[B02] 多分支 else if / elif
来源：http://nkd.ctjpmb.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qnd.gzhubu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hfs.wangshuangyany.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://slr.gzhubu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eom.vehdjk.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ukr.cucudq.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://aya.zhoulong.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xkx.wangdashe.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dxf.zhixingplan.top

[B03] switch / match / case
来源：http://xce.andypj.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kpm.zhiwuduotai.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pzb.uphjek.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bvr.wangdashe.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://euf.tian-w.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tfy.tian-w.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hiz.gogol.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kwn.gogol.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kfa.jyoumei.cn

[B04] for 计数循环
来源：http://sqa.zhiwuduotai.top

Py:   for i in range(10): print(i)
来源：http://udw.316326.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nen.jinqigufen.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fcd.hfpthk.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bzi.sxryk.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tam.quarkkingdee.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cie.c1oappe.top

Ruby: 10.times { |i| puts i }
来源：http://ojz.zhiwuduotai.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://znf.jyoumei.cn

[B05] 遍历数组 / 列表
来源：http://bac.epnwcf.com

Py:   for item in arr: print(item)
来源：http://zjd.hfpthk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yvs.jqgfzy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://lid.shanyushiyangkeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://pcj.chenzaomai.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://pdk.ydzc1.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qwh.vehdjk.com

Ruby: arr.each { |item| puts item }
来源：http://jax.nanxuanxn.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jlo.kuanghao11.cn

[B06] 遍历字典 / 对象
来源：http://pxq.daxiang520.top

Py:   for k, v in d.items(): print(k, v)
来源：http://pna.sufxvd.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nsj.ivvv.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pii.hnxiangtu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kft.yueranfly.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mlc.chenlongwang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://srp.vehdjk.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baz.aibaodan.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kbx.hnqzz.top

[B07] while 循环
来源：http://zfp.chenzaomai.com

Py:   while i < 10: i += 1
来源：http://erl.pycfn.com

PHP:  while ($i < 10) { $i++; }
来源：http://awa.sweek.top

JS:   while (i < 10) { i++; }
来源：http://qiu.jinghuilouyu.cn

TS:   while (i < 10) { i++; }
来源：http://gek.birdmap.top

Java: while (i < 10) { i++; }
来源：http://qkx.gaohongyu789.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sjr.hammf.cn

Ruby: while i < 10; i += 1; end
来源：http://jgn.xuetiantiany.cn

C#:   while (i < 10) { i++; }
来源：http://nba.tanke756.top

[B08] do-while（至少执行一次）
来源：http://gvp.xingfuxueyuan.xyz

Py:   # 无 do-while：用 while True + break
来源：http://lhl.ywan-chungtsiang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://nxp.ybcxt.top

JS:   do { i++; } while (i < 10);
来源：http://ypj.yongpay.top

TS:   do { i++; } while (i < 10);
来源：http://bnx.fzhhl.top

Java: do { i++; } while (i < 10);
来源：http://hzh.xylfe.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bpl.aibaodan.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qcc.jqgfzy.top

C#:   do { i++; } while (i < 10);
来源：http://dfn.birdmap.top

[B09] break 与 continue
来源：http://zav.snrcjt.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hrl.ydzc1.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bgd.tarul.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cjt.zdqjudy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fbi.daria6918.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kmf.c1oappe.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nxn.jinqigfzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wkx.daxiang520.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gho.xingfuxueyuan.xyz

[B10] 遍历同时拿索引
来源：http://fsd.wangdashe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gap.xziqi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kno.ppjwa.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lqh.yangfankeji.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zqo.tianlin.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ghk.hywenlv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lue.guannengcc.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://udr.yuxming.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ibf.sysykeji.top

[B11] 生成数字序列 / 区间
来源：http://ebx.hfpthk.cn

Py:   list(range(0, 10, 2))
来源：http://ntu.jinqigufen.top

PHP:  range(0, 10, 2);
来源：http://xmg.redwolf501.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hwv.ydzc1.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ebd.chenjidiqi.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qxh.fktsv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xqw.gotoacloud.top

Ruby: (0...10).step(2).to_a
来源：http://vpl.ctjpmb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sbj.shangyingyoupin.top

[B12] 跳出多层循环
来源：http://wps.ehwqpu.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://yrz.shuidangran.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://dlm.gzhubu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xxh.sxryk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kzj.fengsongda.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vkd.zhiwuduotai.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sdv.snrcjt.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lgz.bbcook.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nwc.ehwqpu.com

[B13] 判断是否为数字
来源：http://ugs.yj202588.top

Py:   isinstance(x, (int, float))
来源：http://cpo.hfpthk.cn

PHP:  is_numeric($x)
来源：http://add.jinqigfzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mzt.havefunace.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wru.nanxuanxn.top

Java: x instanceof Number
来源：http://bjg.redwolf501.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qwa.pycfn.com

Ruby: x.is_a?(Numeric)
来源：http://ujc.wangshuangyany.cn

C#:   x is int or double or decimal
来源：http://kpr.0kj1m.cn

[B14] 判断值是否在集合内
来源：http://syt.xingfuxueyuan.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lje.vehdjk.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ock.xuetiantiany.cn

JS:   [1, 2, 3].includes(x)
来源：http://xby.wangdashe.top

TS:   [1, 2, 3].includes(x)
来源：http://hph.ybcxt.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mfg.nwbrower.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ccx.wangdashe.top

Ruby: [1, 2, 3].include?(x)
来源：http://bbk.xylfe.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rpf.tianlin.xyz

[B15] 布尔运算与取反
来源：http://xww.sjlbkw.cn

Py:   a and b or not c
来源：http://gvz.zhijiandao.cn

PHP:  $a && $b || !$c
来源：http://dlc.svipenyu.cn

JS:   a && b || !c
来源：http://lih.pengpengdd.cyou

TS:   a && b || !c
来源：http://xrh.guowangkeji.top

Java: a && b || !c
来源：http://ccc.xziqi.cn

Go:   a && b || !c
来源：http://hxg.fzhhl.top

Ruby: a && b || !c
来源：http://zyt.zhoulong.xyz

C#:   a && b || !c
来源：http://ith.vqdsnc.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ffu.yj20258.top

Py:   if not data: return
来源：http://ral.sjlbkw.cn

PHP:  if (!$data) { return; }
来源：http://stm.chenlongwang.top

JS:   if (!data) return;
来源：http://yen.chenzaomai.com

TS:   if (!data) return;
来源：http://bju.hesvh.cn

Java: if (data == null) return;
来源：http://gya.snrcjt.cn

Go:   if data == nil { return }
来源：http://tll.zycfv.cn

Ruby: return if data.nil?
来源：http://aen.zycfv.cn

C#:   if (data == null) return;
来源：http://kub.guowangkeji.top

================================================================================
来源：http://kwx.jyoumei.cn

C. 函数与作用域
来源：http://csn.tian-w.cn

================================================================================
来源：http://jei.smart0.xyz

[C01] 定义函数
来源：http://iux.gaohongyu789.top


<!-- 参考信息 -->