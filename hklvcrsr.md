代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pxq.sweek.top

Java: new Random().nextInt(100) + 1
来源：http://qsq.haohaochexian.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qyc.jlsjyb.cn

Ruby: rand(1..100)
来源：http://nar.shangyingyoupin.top

C#:   new Random().Next(1, 101)
来源：http://sko.yueranfly.top

[A11] 条件表达式（三元）
来源：http://qxt.ydzc1.top

Py:   "yes" if x > 0 else "no"
来源：http://hhs.aibaodan.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rxc.yanxiufei.cn

JS:   x > 0 ? "yes" : "no"
来源：http://dtw.9152youxi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mtp.chenjidiqi.icu

Java: x > 0 ? "yes" : "no"
来源：http://cit.ywan-chungtsiang.top

Go:   // 无三元运算符，需用 if 语句
来源：http://dhd.yangfankeji.com

Ruby: x > 0 ? "yes" : "no"
来源：http://xzz.feifeiyinyue.top

C#:   x > 0 ? "yes" : "no"
来源：http://ggf.shanyushiyangtech.top

[A12] 字符串插值 / 格式化
来源：http://cef.ydjk.org.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ylb.zhongyouzk.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vnp.shangyingyoupin.top

JS:   `Hello, ${name}!`
来源：http://swe.shuidangran.top

TS:   `Hello, ${name}!`
来源：http://upg.shanyushiyangkeji.top

Java: "Hello, %s!".formatted(name)
来源：http://rcp.ivvv.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fcv.xylfe.cn

Ruby: "Hello, #{name}!"
来源：http://syr.quarkkingdee.top

C#:   $"Hello, {name}!"
来源：http://kxk.zhaomingkeji.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://jap.zhongyouzk.top

Py:   "第一行\n第二行"
来源：http://yzs.fanxiaobao.xyz

PHP:  "第一行\n第二行"
来源：http://eze.svipenyu.cn

JS:   "第一行\n第二行"
来源：http://xpp.hnqzz.top

TS:   "第一行\n第二行"
来源：http://gyq.jqgufenzy.top

Java: "第一行\n第二行"
来源：http://ksz.ydjk.org.cn

Go:   "第一行\n第二行"
来源：http://ynv.sjlbkw.cn

Ruby: "第一行\n第二行"
来源：http://vpb.andypj.xyz

C#:   "第一行\n第二行"
来源：http://gli.yj20258.top

[A14] 注释写法
来源：http://xmo.sxryk.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kst.sufxvd.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yyt.uphjek.com

JS:   // 单行；/* 多行 */
来源：http://uln.ybcxt.top

TS:   // 单行；/* 多行 */
来源：http://cmq.gaohongyu789.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dkw.xuetiantiany.cn

Go:   // 单行；/* 多行 */
来源：http://prn.fanxiaobao.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://paz.dashuyun.cn

C#:   // 单行；/* 多行 */
来源：http://ppd.sxryk.cn

[A15] 空值判断与默认值
来源：http://sgs.yanxiufei.cn

Py:   value = data or "默认值"
来源：http://ahl.jinqigufen.top

PHP:  $value = $data ?? "默认值";
来源：http://amg.hfpthk.cn

JS:   const value = data ?? "默认值";
来源：http://ibi.svipenyu.cn

TS:   const value = data ?? "默认值";
来源：http://xto.ybcxt.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://edj.birdmap.top

Go:   if data == "" { data = "默认值" }
来源：http://nxe.cqqwz.cn

Ruby: value = data || "默认值"
来源：http://udm.shuidangran.top

C#:   var value = data ?? "默认值";
来源：http://bcp.ctjpmb.com

[A16] 真假值判断规则
来源：http://pav.jiagoushi.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tgn.xylfe.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://aqi.zycfv.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jrb.jlsjyb.cn

TS:   if (!x) {}
来源：http://dfo.fanxiaobao.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://scy.haohaochexian.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zrh.hysaishi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://spl.birdmap.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fch.jqgufenzy.top

[A17] 位运算
来源：http://ued.wangshuangyany.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ekp.hongshengwenyu.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://aec.havefunace.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ege.gaohongyu789.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zfl.0kj1m.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fqu.epnwcf.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wzl.fengsongda.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://twf.guannengcc.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rdy.redwolf501.top

[A18] 字符与 ASCII 码互转
来源：http://mna.yangfankeji.com

Py:   ord("A"); chr(65)
来源：http://oia.tianlin.xyz

PHP:  ord("A"); chr(65)
来源：http://vnj.yj20258888.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lwc.hywenlv.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qzu.zhaomingkeji.xyz

Java: (int) 'A'; (char) 65
来源：http://vap.tarul.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wcd.zycfv.cn

Ruby: "A".ord; 65.chr
来源：http://hsb.0kj1m.cn

C#:   (int)'A'; (char)65
来源：http://isg.yj202588.top

[A19] 交换两个变量
来源：http://nqr.xylfe.cn

Py:   a, b = b, a
来源：http://kqy.yvedp.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qig.yj202588.top

JS:   [a, b] = [b, a];
来源：http://hlz.xuanzx.com

TS:   [a, b] = [b, a];
来源：http://qsw.epnwcf.com

Java: int t = a; a = b; b = t;
来源：http://hph.jinghuilouyu.cn

Go:   a, b = b, a
来源：http://yci.cqqwz.cn

Ruby: a, b = b, a
来源：http://dms.zhiwuduotai.top

C#:   (a, b) = (b, a);
来源：http://shz.xylfe.cn

[A20] 读取标准输入
来源：http://sdm.52xcode.cn

Py:   name = input("请输入：")
来源：http://rra.gzhubu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://rhi.fktsv.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rbt.hysaishi.cn

TS:   // Node.js：readline 模块
来源：http://cxl.feifeiyinyue.top

Java: new Scanner(System.in).nextLine()
来源：http://cxz.vqdsnc.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lrz.gzhubu.top

Ruby: gets.chomp
来源：http://nfx.smart0.xyz

C#:   Console.ReadLine();
来源：http://fko.hongshengwenyu.top

[A21] 保留指定小数位输出
来源：http://sdg.andypj.xyz

Py:   f"{3.14159:.2f}"
来源：http://vln.jqgufenzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zfb.hammf.cn

JS:   (3.14159).toFixed(2)
来源：http://kiv.jyoumei.cn

TS:   (3.14159).toFixed(2)
来源：http://fdo.yanxiufei.cn

Java: String.format("%.2f", 3.14159)
来源：http://zfw.hammf.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qgb.shangyingyoupin.top

Ruby: format("%.2f", 3.14159)
来源：http://tjl.fehbvm.com

C#:   3.14159.ToString("F2")
来源：http://yhu.316326.xyz

[A22] 获取字符串长度
来源：http://mgu.hesvh.cn

Py:   len(s)
来源：http://dpz.hammf.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ryd.jianghu66.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pwu.vehdjk.com

TS:   s.length
来源：http://ice.gzhubu.top

Java: s.length()
来源：http://zwg.ivvv.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sxm.hfpthk.cn

Ruby: s.length
来源：http://flq.hnxiangtu.top

C#:   s.Length
来源：http://wcm.daria6918.cn

[A23] 大小写转换
来源：http://ymx.tanke756.top

Py:   s.upper(); s.lower(); s.title()
来源：http://tma.ppjwa.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tll.cdnleiting.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://aft.pengpengdd.cyou

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zuf.uphjek.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cev.ydjk.org.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rmj.jianghu66.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hze.xingfuxueyuan.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://fms.jqgufenzy.top

[A24] 去除首尾空白
来源：http://cbq.nanxinkj.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qjm.birdmap.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dxf.ybcxt.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://idl.aizwys.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lzz.andypj.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cee.nwbrower.top

Go:   strings.TrimSpace(s)
来源：http://zfo.wangshuangyany.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xys.tarul.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qtx.dashuyun.cn

[A25] 字符串比较
来源：http://ddd.ctjpmb.com

Py:   s1 == s2; s1 != s2
来源：http://xmm.jinghuilouyu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://drh.cucudq.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://omn.hcnkem.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dzt.smart0.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://etp.dianchejie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vyx.nwbrower.top

Ruby: s1 == s2; s1 <=> s2
来源：http://zzg.zhongyouzk.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bvu.cashguo.top

[A26] 类型转换总览
来源：http://zgw.0kj1m.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pmd.ctjpmb.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hqs.cashguo.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oob.yangfankeji.com

TS:   Number() String() Boolean() x as number
来源：http://dep.xuanzx.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yhg.nanxinkj.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hjj.yuanzhike.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://itw.zdbjq.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vyx.jyoumei.cn

================================================================================
来源：http://jfv.sysykeji.top

B. 流程控制
来源：http://cdr.hammf.cn

================================================================================
来源：http://ikp.smart0.xyz

[B01] 条件判断 if / else
来源：http://ivt.zhiwuduotai.top

Py:   result = "正" if x > 0 else "非正"
来源：http://stb.daria6918.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mlv.zhengqikj.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sdd.cqqwz.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ayo.tian-w.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gqf.jinghuilouyu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yio.yj20258888.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rcm.chenjidiqi.icu

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ter.tanke756.top

[B02] 多分支 else if / elif
来源：http://odq.haohaochexian.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vkw.yuanzhike.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mre.yueranfly.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sqt.yongpay.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mxh.yangfankeji.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xwt.vehdjk.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nhq.epnwcf.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://czj.jyoumei.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tzm.sufxvd.cn

[B03] switch / match / case
来源：http://xeg.hammf.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ujr.jlsjyb.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ews.fzhhl.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://atb.daria6918.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://luf.zhijiandao.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://khu.epnwcf.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vcj.jiagoushi.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dva.zhoulong.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fra.hysaishi.cn

[B04] for 计数循环
来源：http://zqg.iojbl.cn

Py:   for i in range(10): print(i)
来源：http://clz.zhiwuduotai.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lay.0kj1m.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zlw.quarkkingdee.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xbd.ivvv.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uju.smart0.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://afu.fktsv.cn

Ruby: 10.times { |i| puts i }
来源：http://zhv.wangdashe.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uee.hfpthk.cn

[B05] 遍历数组 / 列表
来源：http://rig.zhaomingkeji.xyz

Py:   for item in arr: print(item)
来源：http://urh.iojbl.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nzn.zhiwuduotai.top

JS:   for (const item of arr) { console.log(item); }
来源：http://bei.meibo888.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hxp.shanyushiyangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ozk.vehdjk.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fxa.gotoacloud.top

Ruby: arr.each { |item| puts item }
来源：http://jdk.dashuyun.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rnk.ivvv.top

[B06] 遍历字典 / 对象
来源：http://dyx.aibaodan.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://oap.iojbl.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uge.ppjwa.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hlx.xuetiantiany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jkv.shanyushiyangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ewx.fktsv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fzw.nanxinkj.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rjv.yangfankeji.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ycv.ydjk.org.cn

[B07] while 循环
来源：http://pho.cheryme.top

Py:   while i < 10: i += 1
来源：http://ioy.yanxiufei.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kvx.ctjpmb.com

JS:   while (i < 10) { i++; }
来源：http://arc.hfpthk.cn

TS:   while (i < 10) { i++; }
来源：http://wna.uphjek.com

Java: while (i < 10) { i++; }
来源：http://woa.uphjek.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://adp.bjfxy.top

Ruby: while i < 10; i += 1; end
来源：http://dea.aizwys.cn

C#:   while (i < 10) { i++; }
来源：http://wmw.xuetiantiany.cn

[B08] do-while（至少执行一次）
来源：http://mcj.yueranfly.top

Py:   # 无 do-while：用 while True + break
来源：http://swv.cashguo.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xdi.yueranfly.top

JS:   do { i++; } while (i < 10);
来源：http://zjm.jyoumei.cn

TS:   do { i++; } while (i < 10);
来源：http://oro.hnxiangtu.top

Java: do { i++; } while (i < 10);
来源：http://hzw.birdmap.top

Go:   for { i++; if i >= 10 { break } }
来源：http://van.vehdjk.com

Ruby: begin; i += 1; end while i < 10
来源：http://bzr.yonumen.top

C#:   do { i++; } while (i < 10);
来源：http://qfh.tian-w.cn

[B09] break 与 continue
来源：http://rvl.cucudq.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lcx.hcnkem.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tbr.bjfxy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gwg.zhongyouzk.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://syt.tanke756.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pro.chenjidiqi.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nic.aibaodan.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aji.tanke756.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rus.snrcjt.cn

[B10] 遍历同时拿索引
来源：http://cxx.mhx1999.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://umk.shanyushiyangkeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ypd.tanke756.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://muv.epnwcf.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://trd.shangyingyoupin.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rpm.zycfv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yyg.cashguo.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bjr.c1oappe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kiv.ydjk.org.cn

[B11] 生成数字序列 / 区间
来源：http://ful.jinqigfzy.top

Py:   list(range(0, 10, 2))
来源：http://rkg.chenjidiqi.icu

PHP:  range(0, 10, 2);
来源：http://xcm.dianchejie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pxc.snrcjt.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qlh.zhengqikj.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fru.uphjek.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kkd.redwolf501.top

Ruby: (0...10).step(2).to_a
来源：http://shq.nanxinkj.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://piu.meibo888.top

[B12] 跳出多层循环
来源：http://vmp.pengpengdd.cyou

Py:   # 无标签跳转：抽成函数用 return
来源：http://sst.yfazqb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://nae.yonumen.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mww.yuxming.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gch.dashuyun.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rdi.aibaodan.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qyq.hongshengwenyu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bfd.xziqi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wkn.shuidangran.top

[B13] 判断是否为数字
来源：http://rsb.hywenlv.cn

Py:   isinstance(x, (int, float))
来源：http://ccx.nanxinkj.top

PHP:  is_numeric($x)
来源：http://jef.xuetiantiany.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aof.kuanghao11.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ioy.52xcode.cn

Java: x instanceof Number
来源：http://svi.zhaomingkeji.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://amx.zycfv.cn

Ruby: x.is_a?(Numeric)
来源：http://apj.quarkkingdee.top

C#:   x is int or double or decimal
来源：http://lgj.52xcode.cn

[B14] 判断值是否在集合内
来源：http://oyo.pengpengdd.cyou

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://taj.ppjwa.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://efa.fanxiaobao.xyz

JS:   [1, 2, 3].includes(x)
来源：http://lsy.fehbvm.com

TS:   [1, 2, 3].includes(x)
来源：http://dan.yj202588.top

Java: List.of(1, 2, 3).contains(x)
来源：http://eao.daria6918.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hsc.zhijiandao.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tfd.jianghu66.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jbv.xylfe.cn

[B15] 布尔运算与取反
来源：http://qyo.fanxiaobao.xyz

Py:   a and b or not c
来源：http://nnf.guannengcc.top

PHP:  $a && $b || !$c
来源：http://fec.hnqzz.top

JS:   a && b || !c
来源：http://asd.gogol.net.cn

TS:   a && b || !c
来源：http://ydv.chenzaomai.com

Java: a && b || !c
来源：http://wnl.ydzc1.top

Go:   a && b || !c
来源：http://rcu.cashguo.top

Ruby: a && b || !c
来源：http://ght.jinghuilouyu.cn

C#:   a && b || !c
来源：http://efy.yongpay.top

[B16] 卫语句：不满足条件提前返回
来源：http://kyg.fktsv.cn

Py:   if not data: return
来源：http://orb.meibo888.top

PHP:  if (!$data) { return; }
来源：http://fdc.hnqzz.top

JS:   if (!data) return;
来源：http://klv.epnwcf.com

TS:   if (!data) return;
来源：http://ekw.pycfn.com

Java: if (data == null) return;
来源：http://zfd.jiagoushi.top

Go:   if data == nil { return }
来源：http://onw.shanyushiyangkeji.top

Ruby: return if data.nil?
来源：http://nmc.quarkkingdee.top

C#:   if (data == null) return;
来源：http://lfl.ywan-chungtsiang.top

================================================================================
来源：http://ref.tian-w.cn

C. 函数与作用域
来源：http://xrd.epnwcf.com

================================================================================
来源：http://iap.jqgfzy.top

[C01] 定义函数
来源：http://rru.xziqi.cn


<!-- 参考信息 -->