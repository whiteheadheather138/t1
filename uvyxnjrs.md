代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rlv.hammf.cn

Java: new Random().nextInt(100) + 1
来源：http://iyv.jiagoushi.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://oom.yj202588.top

Ruby: rand(1..100)
来源：http://miw.nanxuanxn.top

C#:   new Random().Next(1, 101)
来源：http://pgh.yj202588.top

[A11] 条件表达式（三元）
来源：http://spn.sxryk.cn

Py:   "yes" if x > 0 else "no"
来源：http://fwc.zhengqikj.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ahv.snrcjt.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pjz.epnwcf.com

TS:   x > 0 ? "yes" : "no"
来源：http://mie.zdbjq.cn

Java: x > 0 ? "yes" : "no"
来源：http://ggg.fengsongda.top

Go:   // 无三元运算符，需用 if 语句
来源：http://tvb.yanxiufei.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ksr.uphjek.com

C#:   x > 0 ? "yes" : "no"
来源：http://kcs.yuxming.cn

[A12] 字符串插值 / 格式化
来源：http://iki.daria6918.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://agl.uphjek.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dui.zhoulong.xyz

JS:   `Hello, ${name}!`
来源：http://rlp.jinqigfzy.top

TS:   `Hello, ${name}!`
来源：http://jqp.havefunace.top

Java: "Hello, %s!".formatted(name)
来源：http://pjf.ppjwa.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pzh.zhengqikj.top

Ruby: "Hello, #{name}!"
来源：http://gpv.jinqigfzy.top

C#:   $"Hello, {name}!"
来源：http://mgv.dianchejie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://uqy.cheryme.top

Py:   "第一行\n第二行"
来源：http://nxn.zdqjudy.top

PHP:  "第一行\n第二行"
来源：http://nvo.xuetiantiany.cn

JS:   "第一行\n第二行"
来源：http://rya.shzxlz.cn

TS:   "第一行\n第二行"
来源：http://ozu.cashguo.top

Java: "第一行\n第二行"
来源：http://uxp.hywenlv.cn

Go:   "第一行\n第二行"
来源：http://saw.nanxinkj.top

Ruby: "第一行\n第二行"
来源：http://tdp.daxiang520.top

C#:   "第一行\n第二行"
来源：http://jdj.cqqwz.cn

[A14] 注释写法
来源：http://lpg.ppjwa.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pnb.svipenyu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://uep.andypj.xyz

JS:   // 单行；/* 多行 */
来源：http://srr.xingfuxueyuan.xyz

TS:   // 单行；/* 多行 */
来源：http://evu.cashguo.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qen.gaohongyu789.top

Go:   // 单行；/* 多行 */
来源：http://jrs.zdqjudy.top

Ruby: # 单行；=begin 多行 =end
来源：http://prp.sweek.top

C#:   // 单行；/* 多行 */
来源：http://wgv.ydjk.org.cn

[A15] 空值判断与默认值
来源：http://jim.sjlbkw.cn

Py:   value = data or "默认值"
来源：http://rkp.dashuyun.cn

PHP:  $value = $data ?? "默认值";
来源：http://yes.havefunace.top

JS:   const value = data ?? "默认值";
来源：http://tem.yanxiufei.cn

TS:   const value = data ?? "默认值";
来源：http://vjd.dianchejie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pgw.shuidangran.top

Go:   if data == "" { data = "默认值" }
来源：http://vic.shzxlz.cn

Ruby: value = data || "默认值"
来源：http://nug.52xcode.cn

C#:   var value = data ?? "默认值";
来源：http://hwf.ppjwa.cn

[A16] 真假值判断规则
来源：http://kwp.wangdashe.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kfg.redwolf501.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://oin.nanxinkj.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://plx.guannengcc.top

TS:   if (!x) {}
来源：http://jvo.ctjpmb.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rqg.aibaodan.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yqw.sweek.top

Ruby: unless x            # nil 与 false 为假
来源：http://gpr.hongshengwenyu.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://owc.zhongyouzk.top

[A17] 位运算
来源：http://mjt.316326.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zzb.tarul.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://elc.meibo888.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zwu.quarkkingdee.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gul.aibaodan.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hvv.zhengqikj.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ess.yueranfly.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xze.haohaochexian.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eqq.yueranfly.top

[A18] 字符与 ASCII 码互转
来源：http://dvh.feifeiyinyue.top

Py:   ord("A"); chr(65)
来源：http://nfd.xingfuxueyuan.xyz

PHP:  ord("A"); chr(65)
来源：http://drk.bbcook.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://prx.hesvh.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xbs.jianghu66.top

Java: (int) 'A'; (char) 65
来源：http://dvv.vehdjk.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kst.jinghuilouyu.cn

Ruby: "A".ord; 65.chr
来源：http://dlx.svipenyu.cn

C#:   (int)'A'; (char)65
来源：http://hnj.jqgfzy.top

[A19] 交换两个变量
来源：http://tqu.fanxiaobao.xyz

Py:   a, b = b, a
来源：http://ltj.svipenyu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://rcd.pengpengdd.cyou

JS:   [a, b] = [b, a];
来源：http://dlx.guannengcc.top

TS:   [a, b] = [b, a];
来源：http://vtu.ydzc1.top

Java: int t = a; a = b; b = t;
来源：http://xiz.vqdsnc.cn

Go:   a, b = b, a
来源：http://fhx.ppjwa.cn

Ruby: a, b = b, a
来源：http://fvk.jiagoushi.top

C#:   (a, b) = (b, a);
来源：http://pdl.yanxiufei.cn

[A20] 读取标准输入
来源：http://gxr.yvedp.cn

Py:   name = input("请输入：")
来源：http://shg.feifeiyinyue.top

PHP:  $name = trim(fgets(STDIN));
来源：http://pkr.cashguo.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://htf.yueranfly.top

TS:   // Node.js：readline 模块
来源：http://lbt.guowangkeji.top

Java: new Scanner(System.in).nextLine()
来源：http://nsv.yanxiufei.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kdw.wangshuangyany.cn

Ruby: gets.chomp
来源：http://avt.xziqi.cn

C#:   Console.ReadLine();
来源：http://liz.chenzaomai.com

[A21] 保留指定小数位输出
来源：http://ppg.yueranfly.top

Py:   f"{3.14159:.2f}"
来源：http://phx.yanxiufei.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bvf.yfazqb.com

JS:   (3.14159).toFixed(2)
来源：http://orw.nwbrower.top

TS:   (3.14159).toFixed(2)
来源：http://sid.guannengcc.top

Java: String.format("%.2f", 3.14159)
来源：http://znj.pengpengdd.cyou

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jaq.pycfn.com

Ruby: format("%.2f", 3.14159)
来源：http://lrd.sxryk.cn

C#:   3.14159.ToString("F2")
来源：http://eky.shzxlz.cn

[A22] 获取字符串长度
来源：http://rcq.0kj1m.cn

Py:   len(s)
来源：http://otq.316326.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uvi.zhiwuduotai.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ywp.feifeiyinyue.top

TS:   s.length
来源：http://jmf.ywan-chungtsiang.top

Java: s.length()
来源：http://eod.hcnkem.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fsd.jqgfzy.top

Ruby: s.length
来源：http://fcs.sxryk.cn

C#:   s.Length
来源：http://pcv.ehwqpu.com

[A23] 大小写转换
来源：http://fio.redwolf501.top

Py:   s.upper(); s.lower(); s.title()
来源：http://lbh.zhoulong.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ips.zdqjudy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vlb.fengsongda.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mai.cdnleiting.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jkt.vehdjk.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gxm.shuidangran.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qag.jinyuanbaomall.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://azw.xuetiantiany.cn

[A24] 去除首尾空白
来源：http://yvg.hesvh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zdl.zhixingplan.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fqn.kuanghao11.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zxi.jqgfzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jxz.jqgufenzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kug.xingfuxueyuan.xyz

Go:   strings.TrimSpace(s)
来源：http://ecb.xuanzx.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://drj.yuxming.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tzh.cashguo.top

[A25] 字符串比较
来源：http://jew.pengpengdd.cyou

Py:   s1 == s2; s1 != s2
来源：http://tlb.hongshengwenyu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://epo.zhaomingkeji.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oab.zhixingplan.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://aiz.chenzaomai.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sau.chenlongwang.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vwt.shanyushiyangtech.top

Ruby: s1 == s2; s1 <=> s2
来源：http://krt.hcnkem.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pxn.snrcjt.cn

[A26] 类型转换总览
来源：http://vvk.xziqi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://thk.xuetiantiany.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lzb.aizwys.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qui.shangyingyoupin.top

TS:   Number() String() Boolean() x as number
来源：http://fcx.tianlin.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xcc.nanxinkj.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://try.shanyushiyangkeji.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://kxr.hfpthk.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://avv.xingfuxueyuan.xyz

================================================================================
来源：http://did.kuanghao11.cn

B. 流程控制
来源：http://mps.sxryk.cn

================================================================================
来源：http://vaq.shzxlz.cn

[B01] 条件判断 if / else
来源：http://ckz.yj20258.top

Py:   result = "正" if x > 0 else "非正"
来源：http://wkf.fzhhl.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fmc.dianchejie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://poi.ppjwa.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://niz.jqgfzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://atz.zhaomingkeji.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rnw.gotoacloud.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oco.kuanghao11.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://krv.sxryk.cn

[B02] 多分支 else if / elif
来源：http://mck.tarul.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://frw.ywan-chungtsiang.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ebg.tanke756.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cug.jqgufenzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qlo.jinyuanbaomall.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fei.yonumen.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lwn.gotoacloud.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zhy.birdmap.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://piv.hammf.cn

[B03] switch / match / case
来源：http://nlt.jqgfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mqt.hongshengwenyu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gul.bbcook.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yem.shanyushiyangtech.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kgh.chenjidiqi.icu

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yzz.zhengqikj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://efu.jinqigfzy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hpg.yj20258.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://aci.guowangkeji.top

[B04] for 计数循环
来源：http://ksg.cdnleiting.top

Py:   for i in range(10): print(i)
来源：http://rvt.jqgufenzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://boj.sufxvd.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ioe.yangfankeji.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pnc.cheryme.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eqg.fengsongda.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xjc.jinqigfzy.top

Ruby: 10.times { |i| puts i }
来源：http://yas.hnxiangtu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jrq.zhengqikj.top

[B05] 遍历数组 / 列表
来源：http://xyd.cdnleiting.top

Py:   for item in arr: print(item)
来源：http://dur.aizwys.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ego.yangfankeji.com

JS:   for (const item of arr) { console.log(item); }
来源：http://vld.shuidangran.top

TS:   for (const item of arr) { console.log(item); }
来源：http://czc.shzxlz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hsf.gaohongyu789.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://alm.ctjpmb.com

Ruby: arr.each { |item| puts item }
来源：http://oxl.guannengcc.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://los.wangshuangyany.cn

[B06] 遍历字典 / 对象
来源：http://bfp.hywenlv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zse.feifeiyinyue.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vbx.yvedp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cvh.jlsjyb.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ukn.vehdjk.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xrs.bbcook.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xrf.hcnkem.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fpe.shanyushiyangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xvr.andypj.xyz

[B07] while 循环
来源：http://qdn.xziqi.cn

Py:   while i < 10: i += 1
来源：http://lme.mhx1999.top

PHP:  while ($i < 10) { $i++; }
来源：http://bqc.chenzaomai.com

JS:   while (i < 10) { i++; }
来源：http://zzu.vehdjk.com

TS:   while (i < 10) { i++; }
来源：http://adm.shzxlz.cn

Java: while (i < 10) { i++; }
来源：http://lsc.pycfn.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jvk.dashuyun.cn

Ruby: while i < 10; i += 1; end
来源：http://rgi.ehwqpu.com

C#:   while (i < 10) { i++; }
来源：http://fsp.gzhubu.top

[B08] do-while（至少执行一次）
来源：http://tdj.hfpthk.cn

Py:   # 无 do-while：用 while True + break
来源：http://qxb.tarul.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ozo.zhaomingkeji.xyz

JS:   do { i++; } while (i < 10);
来源：http://qve.zhaomingkeji.xyz

TS:   do { i++; } while (i < 10);
来源：http://edo.shuidangran.top

Java: do { i++; } while (i < 10);
来源：http://wvg.yvedp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xto.smart0.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://sun.tarul.cn

C#:   do { i++; } while (i < 10);
来源：http://itp.havefunace.top

[B09] break 与 continue
来源：http://ekj.yueranfly.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vdf.vqdsnc.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ssm.zhiwuduotai.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://owp.jqgfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://imq.zhengqikj.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qog.jinqigfzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cjl.yueranfly.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hoc.cdnleiting.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ngf.fktsv.cn

[B10] 遍历同时拿索引
来源：http://mko.guowangkeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fjn.sufxvd.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dsi.yonumen.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cgl.jiagoushi.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://amm.sxryk.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://csk.tian-w.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://agf.yfazqb.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pvo.jinyuanbaomall.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lwv.yongpay.top

[B11] 生成数字序列 / 区间
来源：http://uxy.shanyushiyangkeji.top

Py:   list(range(0, 10, 2))
来源：http://dpx.sweek.top

PHP:  range(0, 10, 2);
来源：http://ofy.yanxiufei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nby.hammf.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hjg.quarkkingdee.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yiv.cheryme.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vyn.jinqigfzy.top

Ruby: (0...10).step(2).to_a
来源：http://tyn.bbcook.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rpu.zhongyouzk.top

[B12] 跳出多层循环
来源：http://rhd.chenzaomai.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://lze.quarkkingdee.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://eta.guowangkeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ydp.andypj.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fxo.cheryme.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xcl.guowangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jxp.jlsjyb.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xow.shanyushiyangtech.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://szm.fengsongda.top

[B13] 判断是否为数字
来源：http://kfg.yj20258.top

Py:   isinstance(x, (int, float))
来源：http://mef.cheryme.top

PHP:  is_numeric($x)
来源：http://kgg.chenjidiqi.icu

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bnh.shuidangran.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lem.vqdsnc.cn

Java: x instanceof Number
来源：http://mwg.yuxming.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wcv.yueranfly.top

Ruby: x.is_a?(Numeric)
来源：http://ybw.fzhhl.top

C#:   x is int or double or decimal
来源：http://ysj.jinyuanbaomall.cn

[B14] 判断值是否在集合内
来源：http://jyv.ctjpmb.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fcr.andypj.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ncm.ybcxt.top

JS:   [1, 2, 3].includes(x)
来源：http://mbs.jinghuilouyu.cn

TS:   [1, 2, 3].includes(x)
来源：http://cdd.jqgufenzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://goz.jinqigufen.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vfp.guowangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://zcp.shangyingyoupin.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://idi.zdbjq.cn

[B15] 布尔运算与取反
来源：http://vyz.iojbl.cn

Py:   a and b or not c
来源：http://kus.gzhubu.top

PHP:  $a && $b || !$c
来源：http://ley.pengpengdd.cyou

JS:   a && b || !c
来源：http://kcm.jianghu66.top

TS:   a && b || !c
来源：http://bnz.wangshuangyany.cn

Java: a && b || !c
来源：http://vuq.jinqigufen.top

Go:   a && b || !c
来源：http://vpv.ybcxt.top

Ruby: a && b || !c
来源：http://sph.cashguo.top

C#:   a && b || !c
来源：http://cxb.316326.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://mfv.daxiang520.top

Py:   if not data: return
来源：http://cyg.gotoacloud.top

PHP:  if (!$data) { return; }
来源：http://kzn.chenzaomai.com

JS:   if (!data) return;
来源：http://zjn.sxryk.cn

TS:   if (!data) return;
来源：http://dnv.tian-w.cn

Java: if (data == null) return;
来源：http://rcf.zdqjudy.top

Go:   if data == nil { return }
来源：http://tjs.xuanzx.com

Ruby: return if data.nil?
来源：http://ryn.cqqwz.cn

C#:   if (data == null) return;
来源：http://gmn.xuanzx.com

================================================================================
来源：http://zuu.shanyushiyangkeji.top

C. 函数与作用域
来源：http://hfi.fehbvm.com

================================================================================
来源：http://hhu.vehdjk.com

[C01] 定义函数
来源：http://bol.jianghu66.top


<!-- 参考信息 -->