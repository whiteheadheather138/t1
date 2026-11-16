代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pkg.zhijiandao.cn

Java: new Random().nextInt(100) + 1
来源：http://cok.jyoumei.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://juz.dashuyun.cn

Ruby: rand(1..100)
来源：http://phu.sufxvd.cn

C#:   new Random().Next(1, 101)
来源：http://egh.zhijiandao.cn

[A11] 条件表达式（三元）
来源：http://kwf.meibo888.top

Py:   "yes" if x > 0 else "no"
来源：http://uxn.tarul.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dpy.cashguo.top

JS:   x > 0 ? "yes" : "no"
来源：http://wlm.zdbjq.cn

TS:   x > 0 ? "yes" : "no"
来源：http://egi.jianghu66.top

Java: x > 0 ? "yes" : "no"
来源：http://vag.chenlongwang.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ofx.yvedp.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://grx.smart0.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://dwe.shanyushiyangtech.top

[A12] 字符串插值 / 格式化
来源：http://zen.sweek.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tlj.yj20258888.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://efw.xinyue.icu

JS:   `Hello, ${name}!`
来源：http://qnu.hcnkem.com

TS:   `Hello, ${name}!`
来源：http://zyb.nwbrower.top

Java: "Hello, %s!".formatted(name)
来源：http://jln.hnxiangtu.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tjm.sxryk.cn

Ruby: "Hello, #{name}!"
来源：http://mxy.yanxiufei.cn

C#:   $"Hello, {name}!"
来源：http://pji.jinghuilouyu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ipd.dashuyun.cn

Py:   "第一行\n第二行"
来源：http://fzi.yj20258.top

PHP:  "第一行\n第二行"
来源：http://tdg.jlsjyb.cn

JS:   "第一行\n第二行"
来源：http://url.xuetiantiany.cn

TS:   "第一行\n第二行"
来源：http://mqq.jianghu66.top

Java: "第一行\n第二行"
来源：http://slb.xingfuxueyuan.xyz

Go:   "第一行\n第二行"
来源：http://rev.jinqigufen.top

Ruby: "第一行\n第二行"
来源：http://gtd.shangyingyoupin.top

C#:   "第一行\n第二行"
来源：http://tzp.52xcode.cn

[A14] 注释写法
来源：http://jct.gaohongyu789.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://bcp.ehwqpu.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://gyv.smart0.xyz

JS:   // 单行；/* 多行 */
来源：http://kka.aibaodan.cn

TS:   // 单行；/* 多行 */
来源：http://mku.meibo888.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bsd.hnqzz.top

Go:   // 单行；/* 多行 */
来源：http://dqw.cdnleiting.top

Ruby: # 单行；=begin 多行 =end
来源：http://lll.sysykeji.top

C#:   // 单行；/* 多行 */
来源：http://dyf.yvedp.cn

[A15] 空值判断与默认值
来源：http://lnn.yuanzhike.top

Py:   value = data or "默认值"
来源：http://qse.yuanzhike.top

PHP:  $value = $data ?? "默认值";
来源：http://ijc.zhixingplan.top

JS:   const value = data ?? "默认值";
来源：http://vql.iojbl.cn

TS:   const value = data ?? "默认值";
来源：http://izw.sjlbkw.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jah.sweek.top

Go:   if data == "" { data = "默认值" }
来源：http://bba.ywan-chungtsiang.top

Ruby: value = data || "默认值"
来源：http://emn.pengpengdd.cyou

C#:   var value = data ?? "默认值";
来源：http://mch.shzxlz.cn

[A16] 真假值判断规则
来源：http://wxa.yanxiufei.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lur.daxiang520.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ewj.yangfankeji.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ffj.c1oappe.top

TS:   if (!x) {}
来源：http://voy.gaohongyu789.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://opp.feifeiyinyue.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://goe.hcnkem.com

Ruby: unless x            # nil 与 false 为假
来源：http://jji.dashuyun.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ijs.fktsv.cn

[A17] 位运算
来源：http://mql.wangdashe.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cdb.yj202588.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baf.meibo888.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lmw.52xcode.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nva.gzhubu.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lmv.xuetiantiany.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://uwo.birdmap.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://unn.pengpengdd.cyou

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://col.jyoumei.cn

[A18] 字符与 ASCII 码互转
来源：http://mtm.sufxvd.cn

Py:   ord("A"); chr(65)
来源：http://ios.chenlongwang.top

PHP:  ord("A"); chr(65)
来源：http://aqp.wangshuangyany.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jex.dianchejie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://skn.316326.xyz

Java: (int) 'A'; (char) 65
来源：http://vpz.havefunace.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://okn.chenzaomai.com

Ruby: "A".ord; 65.chr
来源：http://yql.daria6918.cn

C#:   (int)'A'; (char)65
来源：http://jkz.jinyuanbaomall.cn

[A19] 交换两个变量
来源：http://hgk.kuanghao11.cn

Py:   a, b = b, a
来源：http://upt.nanxuanxn.top

PHP:  [$a, $b] = [$b, $a];
来源：http://mrc.fzhhl.top

JS:   [a, b] = [b, a];
来源：http://ecx.shuidangran.top

TS:   [a, b] = [b, a];
来源：http://fxl.cheryme.top

Java: int t = a; a = b; b = t;
来源：http://sfg.hammf.cn

Go:   a, b = b, a
来源：http://uev.kuanghao11.cn

Ruby: a, b = b, a
来源：http://wmv.jinyuanbaomall.cn

C#:   (a, b) = (b, a);
来源：http://vbh.ctjpmb.com

[A20] 读取标准输入
来源：http://cpa.jinyuanbaomall.cn

Py:   name = input("请输入：")
来源：http://yjq.jinyuanbaomall.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://knw.cucudq.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fxg.fktsv.cn

TS:   // Node.js：readline 模块
来源：http://aet.yueranfly.top

Java: new Scanner(System.in).nextLine()
来源：http://dzm.gzhubu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bau.sjlbkw.cn

Ruby: gets.chomp
来源：http://ojg.guannengcc.top

C#:   Console.ReadLine();
来源：http://kfp.zycfv.cn

[A21] 保留指定小数位输出
来源：http://wft.yongpay.top

Py:   f"{3.14159:.2f}"
来源：http://xxl.hnxiangtu.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://swh.yuanzhike.top

JS:   (3.14159).toFixed(2)
来源：http://qjk.zhaomingkeji.xyz

TS:   (3.14159).toFixed(2)
来源：http://ebu.c1oappe.top

Java: String.format("%.2f", 3.14159)
来源：http://qaq.hfpthk.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wwl.ehwqpu.com

Ruby: format("%.2f", 3.14159)
来源：http://beh.epnwcf.com

C#:   3.14159.ToString("F2")
来源：http://jfr.shangyingyoupin.top

[A22] 获取字符串长度
来源：http://lmn.fzhhl.top

Py:   len(s)
来源：http://boc.vehdjk.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mca.xylfe.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hig.fanxiaobao.xyz

TS:   s.length
来源：http://uga.redwolf501.top

Java: s.length()
来源：http://jiu.bjfxy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uts.smart0.xyz

Ruby: s.length
来源：http://mpx.sufxvd.cn

C#:   s.Length
来源：http://qvd.chenzaomai.com

[A23] 大小写转换
来源：http://upb.zycfv.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rld.yj20258888.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ozg.yfazqb.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fxr.jlsjyb.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cvl.quarkkingdee.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tru.hongshengwenyu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pcc.nanxuanxn.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fac.cucudq.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rlq.haohaochexian.top

[A24] 去除首尾空白
来源：http://zba.yj20258.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lhb.nanxinkj.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qfr.fzhhl.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://abb.xingfuxueyuan.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yqm.wangshuangyany.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wwj.hywenlv.cn

Go:   strings.TrimSpace(s)
来源：http://ajo.wangdashe.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gdj.jianghu66.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bcc.yonumen.top

[A25] 字符串比较
来源：http://ita.meibo888.top

Py:   s1 == s2; s1 != s2
来源：http://jms.yonumen.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rhr.bbcook.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ypo.yongpay.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ulo.daxiang520.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eme.vehdjk.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vyj.jyoumei.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qnf.shanyushiyangtech.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qhy.yueranfly.top

[A26] 类型转换总览
来源：http://nhi.xuanzx.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cqr.316326.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wwf.nwbrower.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://coa.pycfn.com

TS:   Number() String() Boolean() x as number
来源：http://rpv.jinyuanbaomall.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xyn.zdqjudy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dha.bbcook.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ket.mhx1999.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://llr.fanxiaobao.xyz

================================================================================
来源：http://wlg.shuidangran.top

B. 流程控制
来源：http://cgy.hnxiangtu.top

================================================================================
来源：http://bkj.jinqigfzy.top

[B01] 条件判断 if / else
来源：http://inn.zhijiandao.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://anl.cdnleiting.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nhh.shuidangran.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ojm.kuanghao11.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nsv.cashguo.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://obk.hammf.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rcy.shuidangran.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cct.aizwys.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vzz.havefunace.top

[B02] 多分支 else if / elif
来源：http://wab.dashuyun.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zhp.xylfe.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hpi.dashuyun.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cxg.bjfxy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cpr.ppjwa.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gos.fengsongda.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mim.ehwqpu.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eic.52xcode.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hbb.ywan-chungtsiang.top

[B03] switch / match / case
来源：http://gbn.zhoulong.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dcu.xinyue.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://omu.zdqjudy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rnz.xuanzx.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mds.shanyushiyangtech.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zge.ywan-chungtsiang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xum.fehbvm.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wsc.zhengqikj.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ezq.cucudq.cn

[B04] for 计数循环
来源：http://wqq.ctjpmb.com

Py:   for i in range(10): print(i)
来源：http://jsu.bbcook.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aie.316326.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jgt.9152youxi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zll.bbcook.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ukz.hammf.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://erz.nanxuanxn.top

Ruby: 10.times { |i| puts i }
来源：http://zca.jqgfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://alx.fktsv.cn

[B05] 遍历数组 / 列表
来源：http://ezk.cheryme.top

Py:   for item in arr: print(item)
来源：http://jby.fzhhl.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qme.chenlongwang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://kfs.cheryme.top

TS:   for (const item of arr) { console.log(item); }
来源：http://lfk.fehbvm.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://gew.svipenyu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zcu.0kj1m.cn

Ruby: arr.each { |item| puts item }
来源：http://kgq.zhengqikj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://urh.shzxlz.cn

[B06] 遍历字典 / 对象
来源：http://ibe.gogol.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://heq.tarul.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rpq.smart0.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ieg.ydjk.org.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uxa.gogol.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ivz.aizwys.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mop.zdqjudy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yjg.wangdashe.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kyr.quarkkingdee.top

[B07] while 循环
来源：http://npi.epnwcf.com

Py:   while i < 10: i += 1
来源：http://gxn.xziqi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rvm.nanxuanxn.top

JS:   while (i < 10) { i++; }
来源：http://mgb.yongpay.top

TS:   while (i < 10) { i++; }
来源：http://ozc.jinghuilouyu.cn

Java: while (i < 10) { i++; }
来源：http://zdw.gaohongyu789.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://don.dashuyun.cn

Ruby: while i < 10; i += 1; end
来源：http://bze.sufxvd.cn

C#:   while (i < 10) { i++; }
来源：http://lsr.snrcjt.cn

[B08] do-while（至少执行一次）
来源：http://ldt.jinyuanbaomall.cn

Py:   # 无 do-while：用 while True + break
来源：http://evj.ywan-chungtsiang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://hxi.aizwys.cn

JS:   do { i++; } while (i < 10);
来源：http://aui.guannengcc.top

TS:   do { i++; } while (i < 10);
来源：http://jow.sysykeji.top

Java: do { i++; } while (i < 10);
来源：http://glm.quarkkingdee.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ons.tanke756.top

Ruby: begin; i += 1; end while i < 10
来源：http://wio.gogol.net.cn

C#:   do { i++; } while (i < 10);
来源：http://ale.gzhubu.top

[B09] break 与 continue
来源：http://axz.jiagoushi.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qlt.mhx1999.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zyz.chenjidiqi.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nvi.hammf.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mho.quarkkingdee.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rgm.jiagoushi.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pcr.bjfxy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ikb.fengsongda.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wmn.shanyushiyangtech.top

[B10] 遍历同时拿索引
来源：http://zzy.sweek.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mbt.sysykeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qii.pycfn.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wre.yuanzhike.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dtr.sxryk.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mtt.hcnkem.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nkq.haohaochexian.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://csj.daxiang520.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yrl.tianlin.xyz

[B11] 生成数字序列 / 区间
来源：http://lxs.shuidangran.top

Py:   list(range(0, 10, 2))
来源：http://kun.zhiwuduotai.top

PHP:  range(0, 10, 2);
来源：http://lxx.yuxming.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qov.316326.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rjh.jyoumei.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ric.cqqwz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://peq.jqgfzy.top

Ruby: (0...10).step(2).to_a
来源：http://tay.sjlbkw.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pmx.sweek.top

[B12] 跳出多层循环
来源：http://tvi.daria6918.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kuv.0kj1m.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://weg.yongpay.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ivn.vqdsnc.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uid.tanke756.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bbn.yj20258.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lva.birdmap.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cha.yvedp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gda.kuanghao11.cn

[B13] 判断是否为数字
来源：http://rgz.jinqigufen.top

Py:   isinstance(x, (int, float))
来源：http://fgu.xinyue.icu

PHP:  is_numeric($x)
来源：http://wtu.jiagoushi.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wej.bjfxy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rlm.chenlongwang.top

Java: x instanceof Number
来源：http://hee.yangfankeji.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kgs.jianghu66.top

Ruby: x.is_a?(Numeric)
来源：http://dap.cqqwz.cn

C#:   x is int or double or decimal
来源：http://bgj.ydzc1.top

[B14] 判断值是否在集合内
来源：http://kef.zycfv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eax.tianlin.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uye.haohaochexian.top

JS:   [1, 2, 3].includes(x)
来源：http://fdd.ydzc1.top

TS:   [1, 2, 3].includes(x)
来源：http://ewu.cucudq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rge.0kj1m.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zle.dianchejie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zau.sufxvd.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fom.hcnkem.com

[B15] 布尔运算与取反
来源：http://fpy.wangdashe.top

Py:   a and b or not c
来源：http://oij.hywenlv.cn

PHP:  $a && $b || !$c
来源：http://eqm.aizwys.cn

JS:   a && b || !c
来源：http://dxa.hnxiangtu.top

TS:   a && b || !c
来源：http://eun.xuetiantiany.cn

Java: a && b || !c
来源：http://fvv.shanyushiyangkeji.top

Go:   a && b || !c
来源：http://hmz.xingfuxueyuan.xyz

Ruby: a && b || !c
来源：http://xlg.jqgufenzy.top

C#:   a && b || !c
来源：http://xrj.dianchejie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dwf.yanxiufei.cn

Py:   if not data: return
来源：http://nwp.hcnkem.com

PHP:  if (!$data) { return; }
来源：http://wiz.zhengqikj.top

JS:   if (!data) return;
来源：http://mct.316326.xyz

TS:   if (!data) return;
来源：http://mnr.ydzc1.top

Java: if (data == null) return;
来源：http://gyl.fehbvm.com

Go:   if data == nil { return }
来源：http://jbc.chenlongwang.top

Ruby: return if data.nil?
来源：http://sjo.zhijiandao.cn

C#:   if (data == null) return;
来源：http://slv.pengpengdd.cyou

================================================================================
来源：http://nav.fanxiaobao.xyz

C. 函数与作用域
来源：http://vge.ybcxt.top

================================================================================
来源：http://qsk.cheryme.top

[C01] 定义函数
来源：http://eht.yanxiufei.cn


<!-- 参考信息 -->