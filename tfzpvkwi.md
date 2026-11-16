代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sgi.jianghu66.top

Java: new Random().nextInt(100) + 1
来源：http://sre.jianghu66.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qgq.yj202588.top

Ruby: rand(1..100)
来源：http://gwe.xuanzx.com

C#:   new Random().Next(1, 101)
来源：http://pce.jinqigufen.top

[A11] 条件表达式（三元）
来源：http://wun.ybcxt.top

Py:   "yes" if x > 0 else "no"
来源：http://ylp.yuanzhike.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://kct.feifeiyinyue.top

JS:   x > 0 ? "yes" : "no"
来源：http://bsq.shzxlz.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xow.gzhubu.top

Java: x > 0 ? "yes" : "no"
来源：http://mef.yuanzhike.top

Go:   // 无三元运算符，需用 if 语句
来源：http://lzu.ivvv.top

Ruby: x > 0 ? "yes" : "no"
来源：http://afd.c1oappe.top

C#:   x > 0 ? "yes" : "no"
来源：http://brp.shangyingyoupin.top

[A12] 字符串插值 / 格式化
来源：http://wsy.jqgufenzy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vge.jinqigufen.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cnk.smart0.xyz

JS:   `Hello, ${name}!`
来源：http://tws.tarul.cn

TS:   `Hello, ${name}!`
来源：http://yby.9152youxi.cn

Java: "Hello, %s!".formatted(name)
来源：http://itk.zhiwuduotai.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wxu.c1oappe.top

Ruby: "Hello, #{name}!"
来源：http://wrv.bjfxy.top

C#:   $"Hello, {name}!"
来源：http://vnz.hnqzz.top

[A13] 多行字符串（练习 \n 转义）
来源：http://aoz.zhiwuduotai.top

Py:   "第一行\n第二行"
来源：http://ksi.kuanghao11.cn

PHP:  "第一行\n第二行"
来源：http://tvw.kuanghao11.cn

JS:   "第一行\n第二行"
来源：http://lmw.zdbjq.cn

TS:   "第一行\n第二行"
来源：http://jbe.wangdashe.top

Java: "第一行\n第二行"
来源：http://sch.hesvh.cn

Go:   "第一行\n第二行"
来源：http://aro.zhaomingkeji.xyz

Ruby: "第一行\n第二行"
来源：http://cew.sysykeji.top

C#:   "第一行\n第二行"
来源：http://ebm.gaohongyu789.top

[A14] 注释写法
来源：http://zld.smart0.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://tdy.hesvh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://imf.zhijiandao.cn

JS:   // 单行；/* 多行 */
来源：http://sqm.hnxiangtu.top

TS:   // 单行；/* 多行 */
来源：http://cms.fehbvm.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dqy.aizwys.cn

Go:   // 单行；/* 多行 */
来源：http://fsr.yj20258.top

Ruby: # 单行；=begin 多行 =end
来源：http://mwb.ydjk.org.cn

C#:   // 单行；/* 多行 */
来源：http://lfr.tianlin.xyz

[A15] 空值判断与默认值
来源：http://pwr.52xcode.cn

Py:   value = data or "默认值"
来源：http://qcd.zhengqikj.top

PHP:  $value = $data ?? "默认值";
来源：http://zve.tarul.cn

JS:   const value = data ?? "默认值";
来源：http://nhg.zhongyouzk.top

TS:   const value = data ?? "默认值";
来源：http://bip.birdmap.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tca.shangyingyoupin.top

Go:   if data == "" { data = "默认值" }
来源：http://kyk.nwbrower.top

Ruby: value = data || "默认值"
来源：http://oav.chenzaomai.com

C#:   var value = data ?? "默认值";
来源：http://fwj.cheryme.top

[A16] 真假值判断规则
来源：http://hif.ydjk.org.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pff.jlsjyb.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nuw.jqgfzy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://flv.cashguo.top

TS:   if (!x) {}
来源：http://wve.yj202588.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fcn.redwolf501.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://spl.yonumen.top

Ruby: unless x            # nil 与 false 为假
来源：http://ufi.c1oappe.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rvx.zdqjudy.top

[A17] 位运算
来源：http://zog.yj20258.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://swb.c1oappe.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://scy.aizwys.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://okl.guannengcc.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://usy.zhixingplan.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ktk.jianghu66.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dkw.fengsongda.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xtk.vqdsnc.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aud.zdbjq.cn

[A18] 字符与 ASCII 码互转
来源：http://wfq.aibaodan.cn

Py:   ord("A"); chr(65)
来源：http://yjc.yj20258.top

PHP:  ord("A"); chr(65)
来源：http://drn.hongshengwenyu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jve.yfazqb.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hhs.ywan-chungtsiang.top

Java: (int) 'A'; (char) 65
来源：http://pnb.daria6918.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fjr.hcnkem.com

Ruby: "A".ord; 65.chr
来源：http://kru.yuxming.cn

C#:   (int)'A'; (char)65
来源：http://yfw.daxiang520.top

[A19] 交换两个变量
来源：http://hrp.zhijiandao.cn

Py:   a, b = b, a
来源：http://pva.dashuyun.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bgr.mhx1999.top

JS:   [a, b] = [b, a];
来源：http://nyt.gaohongyu789.top

TS:   [a, b] = [b, a];
来源：http://eyo.ywan-chungtsiang.top

Java: int t = a; a = b; b = t;
来源：http://pyo.gotoacloud.top

Go:   a, b = b, a
来源：http://qgb.hnqzz.top

Ruby: a, b = b, a
来源：http://egt.yongpay.top

C#:   (a, b) = (b, a);
来源：http://ttx.fehbvm.com

[A20] 读取标准输入
来源：http://app.zycfv.cn

Py:   name = input("请输入：")
来源：http://alg.tarul.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://usw.yangfankeji.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mlw.vqdsnc.cn

TS:   // Node.js：readline 模块
来源：http://wld.hnxiangtu.top

Java: new Scanner(System.in).nextLine()
来源：http://cyk.ppjwa.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wlr.cdnleiting.top

Ruby: gets.chomp
来源：http://zlu.yueranfly.top

C#:   Console.ReadLine();
来源：http://skj.jlsjyb.cn

[A21] 保留指定小数位输出
来源：http://rpu.zhaomingkeji.xyz

Py:   f"{3.14159:.2f}"
来源：http://chm.ydzc1.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://psl.yanxiufei.cn

JS:   (3.14159).toFixed(2)
来源：http://qoo.zdqjudy.top

TS:   (3.14159).toFixed(2)
来源：http://lzn.pengpengdd.cyou

Java: String.format("%.2f", 3.14159)
来源：http://xxw.zhongyouzk.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lmf.52xcode.cn

Ruby: format("%.2f", 3.14159)
来源：http://nsm.uphjek.com

C#:   3.14159.ToString("F2")
来源：http://pof.yj20258888.top

[A22] 获取字符串长度
来源：http://kql.jlsjyb.cn

Py:   len(s)
来源：http://udm.hcnkem.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mus.cheryme.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kcr.sufxvd.cn

TS:   s.length
来源：http://iul.ywan-chungtsiang.top

Java: s.length()
来源：http://lvt.yvedp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yvw.hcnkem.com

Ruby: s.length
来源：http://aoj.nanxuanxn.top

C#:   s.Length
来源：http://stf.gaohongyu789.top

[A23] 大小写转换
来源：http://yrw.jinghuilouyu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vwh.tanke756.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kti.yonumen.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nsm.ybcxt.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vqd.pycfn.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://atu.gogol.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vxz.yongpay.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gel.aibaodan.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zho.redwolf501.top

[A24] 去除首尾空白
来源：http://zot.jinghuilouyu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sjq.sweek.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wfy.yvedp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eej.daxiang520.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kzg.zhijiandao.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qtw.chenlongwang.top

Go:   strings.TrimSpace(s)
来源：http://dbm.ctjpmb.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tcg.haohaochexian.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lev.yj20258.top

[A25] 字符串比较
来源：http://eqy.ivvv.top

Py:   s1 == s2; s1 != s2
来源：http://uhw.vqdsnc.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://spm.hywenlv.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jro.hfpthk.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rmd.snrcjt.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://khb.yongpay.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wvr.ydjk.org.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bcs.haohaochexian.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ekt.fehbvm.com

[A26] 类型转换总览
来源：http://isd.9152youxi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mjv.yanxiufei.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xcf.sweek.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ghc.zhoulong.xyz

TS:   Number() String() Boolean() x as number
来源：http://sjk.yvedp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zot.quarkkingdee.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fnr.sxryk.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nvl.aibaodan.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ptr.cheryme.top

================================================================================
来源：http://zkq.9152youxi.cn

B. 流程控制
来源：http://gla.feifeiyinyue.top

================================================================================
来源：http://oxd.yangfankeji.com

[B01] 条件判断 if / else
来源：http://ycm.yfazqb.com

Py:   result = "正" if x > 0 else "非正"
来源：http://ajd.tian-w.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gpu.iojbl.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pgx.yj20258.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://krg.vehdjk.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://xua.ehwqpu.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ccb.zhaomingkeji.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pqv.yj20258888.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rlk.hnqzz.top

[B02] 多分支 else if / elif
来源：http://eks.zhoulong.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kuo.aibaodan.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yfd.sxryk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yin.shzxlz.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tzl.yj20258.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://koq.ydzc1.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yzj.feifeiyinyue.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ldq.chenjidiqi.icu

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sht.smart0.xyz

[B03] switch / match / case
来源：http://gwb.yuxming.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xee.0kj1m.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mge.sysykeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://stk.daxiang520.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://shj.dianchejie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bjt.pycfn.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://udk.nanxuanxn.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qsf.jyoumei.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://paa.tianlin.xyz

[B04] for 计数循环
来源：http://kex.pengpengdd.cyou

Py:   for i in range(10): print(i)
来源：http://ajv.shuidangran.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nfx.haohaochexian.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jhu.mhx1999.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://twi.hfpthk.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://awp.bbcook.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://alb.zdbjq.cn

Ruby: 10.times { |i| puts i }
来源：http://xff.yangfankeji.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ice.sufxvd.cn

[B05] 遍历数组 / 列表
来源：http://fbl.xuetiantiany.cn

Py:   for item in arr: print(item)
来源：http://zab.hnxiangtu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eqi.yongpay.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xlg.hnqzz.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hxa.jinyuanbaomall.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ojv.kuanghao11.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jck.yonumen.top

Ruby: arr.each { |item| puts item }
来源：http://cqm.xingfuxueyuan.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gse.snrcjt.cn

[B06] 遍历字典 / 对象
来源：http://lmn.sufxvd.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zza.epnwcf.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sap.jinyuanbaomall.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fmi.gotoacloud.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hoj.jinyuanbaomall.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qew.shangyingyoupin.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nzj.zhixingplan.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pbd.jqgfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lon.jianghu66.top

[B07] while 循环
来源：http://sjt.jyoumei.cn

Py:   while i < 10: i += 1
来源：http://djs.fehbvm.com

PHP:  while ($i < 10) { $i++; }
来源：http://mau.birdmap.top

JS:   while (i < 10) { i++; }
来源：http://pqm.sufxvd.cn

TS:   while (i < 10) { i++; }
来源：http://ufv.meibo888.top

Java: while (i < 10) { i++; }
来源：http://zea.yanxiufei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lml.zdqjudy.top

Ruby: while i < 10; i += 1; end
来源：http://wxn.yueranfly.top

C#:   while (i < 10) { i++; }
来源：http://lwy.ybcxt.top

[B08] do-while（至少执行一次）
来源：http://dvx.aizwys.cn

Py:   # 无 do-while：用 while True + break
来源：http://hoy.yanxiufei.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fny.zhaomingkeji.xyz

JS:   do { i++; } while (i < 10);
来源：http://poy.birdmap.top

TS:   do { i++; } while (i < 10);
来源：http://tui.nanxuanxn.top

Java: do { i++; } while (i < 10);
来源：http://ulz.wangshuangyany.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yti.yanxiufei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jue.zhengqikj.top

C#:   do { i++; } while (i < 10);
来源：http://ard.dashuyun.cn

[B09] break 与 continue
来源：http://aav.guowangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bzb.0kj1m.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vrm.sufxvd.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nwn.xylfe.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wui.jqgufenzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nlk.nanxinkj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lsi.bjfxy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ceu.sysykeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sls.kuanghao11.cn

[B10] 遍历同时拿索引
来源：http://kfm.9152youxi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cez.havefunace.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cyi.nwbrower.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://szl.jianghu66.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://swp.hfpthk.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ubb.yangfankeji.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qvt.jlsjyb.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pfj.smart0.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://roz.sweek.top

[B11] 生成数字序列 / 区间
来源：http://pkq.cheryme.top

Py:   list(range(0, 10, 2))
来源：http://eio.sjlbkw.cn

PHP:  range(0, 10, 2);
来源：http://tmu.jinqigufen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qdw.nwbrower.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yxa.quarkkingdee.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://peu.yongpay.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vnu.smart0.xyz

Ruby: (0...10).step(2).to_a
来源：http://mmv.hysaishi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fbi.xylfe.cn

[B12] 跳出多层循环
来源：http://bxm.jlsjyb.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tcf.bjfxy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ago.zdqjudy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pru.jianghu66.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qbo.zdbjq.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://asn.hywenlv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tkx.hongshengwenyu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mly.tian-w.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gan.haohaochexian.top

[B13] 判断是否为数字
来源：http://ekp.yongpay.top

Py:   isinstance(x, (int, float))
来源：http://gxd.aizwys.cn

PHP:  is_numeric($x)
来源：http://ssb.meibo888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://arb.feifeiyinyue.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uev.ivvv.top

Java: x instanceof Number
来源：http://enw.yongpay.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kux.sufxvd.cn

Ruby: x.is_a?(Numeric)
来源：http://ybw.sufxvd.cn

C#:   x is int or double or decimal
来源：http://bhq.jlsjyb.cn

[B14] 判断值是否在集合内
来源：http://znx.316326.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://diw.ywan-chungtsiang.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rnb.shuidangran.top

JS:   [1, 2, 3].includes(x)
来源：http://phg.sweek.top

TS:   [1, 2, 3].includes(x)
来源：http://ibu.nanxinkj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://glx.jinghuilouyu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sic.hammf.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dsh.jinghuilouyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://crx.jinqigufen.top

[B15] 布尔运算与取反
来源：http://vxg.jinqigufen.top

Py:   a and b or not c
来源：http://ctg.quarkkingdee.top

PHP:  $a && $b || !$c
来源：http://qgr.redwolf501.top

JS:   a && b || !c
来源：http://pww.xuetiantiany.cn

TS:   a && b || !c
来源：http://pcp.meibo888.top

Java: a && b || !c
来源：http://uai.cucudq.cn

Go:   a && b || !c
来源：http://kud.kuanghao11.cn

Ruby: a && b || !c
来源：http://lxd.zhongyouzk.top

C#:   a && b || !c
来源：http://vma.wangdashe.top

[B16] 卫语句：不满足条件提前返回
来源：http://hpo.yongpay.top

Py:   if not data: return
来源：http://zkq.zhijiandao.cn

PHP:  if (!$data) { return; }
来源：http://sim.sweek.top

JS:   if (!data) return;
来源：http://gur.vehdjk.com

TS:   if (!data) return;
来源：http://dtf.xingfuxueyuan.xyz

Java: if (data == null) return;
来源：http://diq.jiagoushi.top

Go:   if data == nil { return }
来源：http://ctt.vehdjk.com

Ruby: return if data.nil?
来源：http://vzk.ivvv.top

C#:   if (data == null) return;
来源：http://ijb.316326.xyz

================================================================================
来源：http://ldf.guannengcc.top

C. 函数与作用域
来源：http://jhh.xuanzx.com

================================================================================
来源：http://zhm.hywenlv.cn

[C01] 定义函数
来源：http://tvm.hywenlv.cn


<!-- 参考信息 -->