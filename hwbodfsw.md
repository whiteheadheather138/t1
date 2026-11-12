代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://epb.jinqigfzy.top

TS:   x > 0 ? "yes" : "no"
来源：http://epl.fktsv.cn

Java: x > 0 ? "yes" : "no"
来源：http://plh.316326.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://pgq.yuxming.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://yzc.sufxvd.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rsx.pengpengdd.cyou

[A12] 字符串插值 / 格式化
来源：http://hkj.xinyue.icu

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://avs.gogol.net.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://joq.fzhhl.top

JS:   `Hello, ${name}!`
来源：http://rzd.jqgufenzy.top

TS:   `Hello, ${name}!`
来源：http://mre.sufxvd.cn

Java: "Hello, %s!".formatted(name)
来源：http://qeg.jinqigufen.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bkj.yj20258.top

Ruby: "Hello, #{name}!"
来源：http://fqy.jinqigufen.top

C#:   $"Hello, {name}!"
来源：http://brd.feifeiyinyue.top

[A13] 多行字符串（练习 \n 转义）
来源：http://oat.bjfxy.top

Py:   "第一行\n第二行"
来源：http://xvp.zhiwuduotai.top

PHP:  "第一行\n第二行"
来源：http://zzy.9152youxi.cn

JS:   "第一行\n第二行"
来源：http://sii.hnxiangtu.top

TS:   "第一行\n第二行"
来源：http://uoq.bjfxy.top

Java: "第一行\n第二行"
来源：http://icm.chenjidiqi.icu

Go:   "第一行\n第二行"
来源：http://ppu.ehwqpu.com

Ruby: "第一行\n第二行"
来源：http://hty.sxryk.cn

C#:   "第一行\n第二行"
来源：http://rnp.jinqigfzy.top

[A14] 注释写法
来源：http://zoe.jlsjyb.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zik.zycfv.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://uwk.epnwcf.com

JS:   // 单行；/* 多行 */
来源：http://ccd.uphjek.com

TS:   // 单行；/* 多行 */
来源：http://sbr.pycfn.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jqt.xingfuxueyuan.xyz

Go:   // 单行；/* 多行 */
来源：http://akc.vqdsnc.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zjy.jyoumei.cn

C#:   // 单行；/* 多行 */
来源：http://ndl.zhixingplan.top

[A15] 空值判断与默认值
来源：http://gjg.sjlbkw.cn

Py:   value = data or "默认值"
来源：http://fxi.ivvv.top

PHP:  $value = $data ?? "默认值";
来源：http://grr.jlsjyb.cn

JS:   const value = data ?? "默认值";
来源：http://rxe.redwolf501.top

TS:   const value = data ?? "默认值";
来源：http://lpu.jlsjyb.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wue.yongpay.top

Go:   if data == "" { data = "默认值" }
来源：http://ozf.zdbjq.cn

Ruby: value = data || "默认值"
来源：http://cqr.feifeiyinyue.top

C#:   var value = data ?? "默认值";
来源：http://ymk.jianghu66.top

[A16] 真假值判断规则
来源：http://zbw.ydzc1.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kjx.meibo888.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://usx.guowangkeji.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uyr.ehwqpu.com

TS:   if (!x) {}
来源：http://vug.xuanzx.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://peu.guowangkeji.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wlb.hesvh.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yrj.zhijiandao.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tvo.yueranfly.top

[A17] 位运算
来源：http://eqp.zhiwuduotai.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://snu.c1oappe.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ojw.hnxiangtu.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dgt.ybcxt.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fra.cqqwz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ykq.zycfv.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://med.sxryk.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yvx.iojbl.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yuj.dashuyun.cn

[A18] 字符与 ASCII 码互转
来源：http://eio.zdqjudy.top

Py:   ord("A"); chr(65)
来源：http://pim.tianlin.xyz

PHP:  ord("A"); chr(65)
来源：http://xbp.tanke756.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://urq.jinqigfzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rnp.xziqi.cn

Java: (int) 'A'; (char) 65
来源：http://xqg.hongshengwenyu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://otv.mhx1999.top

Ruby: "A".ord; 65.chr
来源：http://oqx.sufxvd.cn

C#:   (int)'A'; (char)65
来源：http://upi.mhx1999.top

[A19] 交换两个变量
来源：http://iro.jlsjyb.cn

Py:   a, b = b, a
来源：http://qpy.hongshengwenyu.top

PHP:  [$a, $b] = [$b, $a];
来源：http://kwc.ehwqpu.com

JS:   [a, b] = [b, a];
来源：http://scx.hysaishi.cn

TS:   [a, b] = [b, a];
来源：http://yhd.hcnkem.com

Java: int t = a; a = b; b = t;
来源：http://wyx.ivvv.top

Go:   a, b = b, a
来源：http://scb.kuanghao11.cn

Ruby: a, b = b, a
来源：http://ysc.nanxinkj.top

C#:   (a, b) = (b, a);
来源：http://xvb.zhaomingkeji.xyz

[A20] 读取标准输入
来源：http://wvw.yj20258.top

Py:   name = input("请输入：")
来源：http://ttg.xuanzx.com

PHP:  $name = trim(fgets(STDIN));
来源：http://evv.jinqigfzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://uvo.ybcxt.top

TS:   // Node.js：readline 模块
来源：http://tmw.pengpengdd.cyou

Java: new Scanner(System.in).nextLine()
来源：http://grz.tarul.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vcd.haohaochexian.top

Ruby: gets.chomp
来源：http://uyd.ydjk.org.cn

C#:   Console.ReadLine();
来源：http://nyr.wangdashe.top

[A21] 保留指定小数位输出
来源：http://qov.fktsv.cn

Py:   f"{3.14159:.2f}"
来源：http://kra.bbcook.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://iqb.shanyushiyangkeji.top

JS:   (3.14159).toFixed(2)
来源：http://ept.nwbrower.top

TS:   (3.14159).toFixed(2)
来源：http://yty.chenzaomai.com

Java: String.format("%.2f", 3.14159)
来源：http://tjr.mhx1999.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bfi.wangdashe.top

Ruby: format("%.2f", 3.14159)
来源：http://evx.quarkkingdee.top

C#:   3.14159.ToString("F2")
来源：http://ivb.c1oappe.top

[A22] 获取字符串长度
来源：http://tps.xuanzx.com

Py:   len(s)
来源：http://ggq.daria6918.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bcr.ctjpmb.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ycl.shanyushiyangtech.top

TS:   s.length
来源：http://bsh.pycfn.com

Java: s.length()
来源：http://wfl.ivvv.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kcn.hywenlv.cn

Ruby: s.length
来源：http://ytb.fengsongda.top

C#:   s.Length
来源：http://beo.xylfe.cn

[A23] 大小写转换
来源：http://ibr.c1oappe.top

Py:   s.upper(); s.lower(); s.title()
来源：http://noz.guannengcc.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xky.jiagoushi.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://aer.guowangkeji.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cwo.ydzc1.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nxb.svipenyu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://skk.xuetiantiany.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jlt.jqgfzy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://pzz.nanxuanxn.top

[A24] 去除首尾空白
来源：http://mni.jqgufenzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ohm.fzhhl.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jxl.guowangkeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ohu.jiagoushi.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zlm.mhx1999.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kzl.cucudq.cn

Go:   strings.TrimSpace(s)
来源：http://wnk.jinghuilouyu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wwe.shangyingyoupin.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://flz.52xcode.cn

[A25] 字符串比较
来源：http://txr.shanyushiyangtech.top

Py:   s1 == s2; s1 != s2
来源：http://dng.jinghuilouyu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xze.jlsjyb.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://msu.epnwcf.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vhr.sysykeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wvt.gogol.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wob.sysykeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://rlt.yangfankeji.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pjp.chenjidiqi.icu

[A26] 类型转换总览
来源：http://ves.chenlongwang.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jah.kuanghao11.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zzp.xziqi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pkb.jqgufenzy.top

TS:   Number() String() Boolean() x as number
来源：http://ybb.cqqwz.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://iuw.tanke756.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pjm.sufxvd.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wze.hongshengwenyu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ghc.jqgfzy.top

================================================================================
来源：http://abr.ppjwa.cn

B. 流程控制
来源：http://bef.vqdsnc.cn

================================================================================
来源：http://akn.cucudq.cn

[B01] 条件判断 if / else
来源：http://mjy.hammf.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://imo.fzhhl.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ufg.uphjek.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dpd.hesvh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uyn.jlsjyb.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://iev.zhongyouzk.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jgc.yangfankeji.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jay.bbcook.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dnc.cheryme.top

[B02] 多分支 else if / elif
来源：http://cqu.yangfankeji.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pqn.fanxiaobao.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wto.hywenlv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yix.shuidangran.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uhj.tian-w.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ajf.ctjpmb.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://val.smart0.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fni.zhijiandao.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pww.zhaomingkeji.xyz

[B03] switch / match / case
来源：http://tti.jyoumei.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zfh.shanyushiyangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vzl.zhoulong.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kli.xingfuxueyuan.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cag.zhaomingkeji.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://che.zycfv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ker.aibaodan.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nsw.cqqwz.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fkj.shangyingyoupin.top

[B04] for 计数循环
来源：http://prp.hammf.cn

Py:   for i in range(10): print(i)
来源：http://uqg.nanxuanxn.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iiu.sxryk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hnk.cqqwz.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uvg.fehbvm.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ugp.guannengcc.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nxk.yj202588.top

Ruby: 10.times { |i| puts i }
来源：http://nns.sjlbkw.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://eng.hcnkem.com

[B05] 遍历数组 / 列表
来源：http://rpt.uphjek.com

Py:   for item in arr: print(item)
来源：http://ith.nanxuanxn.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zhc.zhongyouzk.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vey.gogol.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bdw.fengsongda.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qks.52xcode.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ybu.dianchejie.cn

Ruby: arr.each { |item| puts item }
来源：http://pno.jinghuilouyu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rws.tanke756.top

[B06] 遍历字典 / 对象
来源：http://tnb.andypj.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://eoh.zhijiandao.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fbq.shzxlz.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jpg.hysaishi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ezn.aizwys.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ati.wangdashe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nsr.fzhhl.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lij.kuanghao11.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xqq.xuanzx.com

[B07] while 循环
来源：http://dat.xziqi.cn

Py:   while i < 10: i += 1
来源：http://epj.gzhubu.top

PHP:  while ($i < 10) { $i++; }
来源：http://dzh.vehdjk.com

JS:   while (i < 10) { i++; }
来源：http://ngw.fzhhl.top

TS:   while (i < 10) { i++; }
来源：http://awa.chenlongwang.top

Java: while (i < 10) { i++; }
来源：http://wnm.quarkkingdee.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gqq.sysykeji.top

Ruby: while i < 10; i += 1; end
来源：http://sny.yj202588.top

C#:   while (i < 10) { i++; }
来源：http://kqj.yuanzhike.top

[B08] do-while（至少执行一次）
来源：http://wxo.fehbvm.com

Py:   # 无 do-while：用 while True + break
来源：http://zdi.jqgufenzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://wbf.316326.xyz

JS:   do { i++; } while (i < 10);
来源：http://tmz.chenlongwang.top

TS:   do { i++; } while (i < 10);
来源：http://qqm.hnqzz.top

Java: do { i++; } while (i < 10);
来源：http://czp.zhengqikj.top

Go:   for { i++; if i >= 10 { break } }
来源：http://erq.hesvh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://eyd.pengpengdd.cyou

C#:   do { i++; } while (i < 10);
来源：http://ovc.guannengcc.top

[B09] break 与 continue
来源：http://rbk.jinqigufen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uzd.chenlongwang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xrf.hnqzz.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wpl.xinyue.icu

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pnn.jinghuilouyu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kps.gzhubu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zrx.chenlongwang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://njw.zhongyouzk.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ope.shangyingyoupin.top

[B10] 遍历同时拿索引
来源：http://kok.fzhhl.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gsp.ehwqpu.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hog.yj20258.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mgw.kuanghao11.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zmo.sysykeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rny.daria6918.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sex.jqgfzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cip.0kj1m.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tql.yj20258888.top

[B11] 生成数字序列 / 区间
来源：http://zfo.mhx1999.top

Py:   list(range(0, 10, 2))
来源：http://anf.jianghu66.top

PHP:  range(0, 10, 2);
来源：http://evc.hnqzz.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vyq.guannengcc.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gdk.sufxvd.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hru.pengpengdd.cyou

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lmy.chenjidiqi.icu

Ruby: (0...10).step(2).to_a
来源：http://wsl.ywan-chungtsiang.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fjz.xuetiantiany.cn

[B12] 跳出多层循环
来源：http://mas.tarul.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dlo.vehdjk.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://zyc.snrcjt.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pdn.yanxiufei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aoc.zhixingplan.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://adi.feifeiyinyue.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jwh.ybcxt.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ama.pengpengdd.cyou

C#:   # 无标签：用 goto label 或布尔标志
来源：http://teg.fktsv.cn

[B13] 判断是否为数字
来源：http://wgb.chenlongwang.top

Py:   isinstance(x, (int, float))
来源：http://vbv.ydjk.org.cn

PHP:  is_numeric($x)
来源：http://pre.shzxlz.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uzd.fanxiaobao.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hxd.tianlin.xyz

Java: x instanceof Number
来源：http://geo.gzhubu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zbn.cucudq.cn

Ruby: x.is_a?(Numeric)
来源：http://xgv.yongpay.top

C#:   x is int or double or decimal
来源：http://vpm.hywenlv.cn

[B14] 判断值是否在集合内
来源：http://mqz.ydzc1.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bvk.yvedp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dct.wangshuangyany.cn

JS:   [1, 2, 3].includes(x)
来源：http://sps.hfpthk.cn

TS:   [1, 2, 3].includes(x)
来源：http://whs.meibo888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://yyp.mhx1999.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ird.cheryme.top

Ruby: [1, 2, 3].include?(x)
来源：http://ghv.zhijiandao.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xxu.9152youxi.cn

[B15] 布尔运算与取反
来源：http://nrb.zhongyouzk.top

Py:   a and b or not c
来源：http://pjs.guannengcc.top

PHP:  $a && $b || !$c
来源：http://msi.cheryme.top

JS:   a && b || !c
来源：http://aew.tian-w.cn

TS:   a && b || !c
来源：http://bbz.zycfv.cn

Java: a && b || !c
来源：http://itu.jianghu66.top

Go:   a && b || !c
来源：http://lne.yfazqb.com

Ruby: a && b || !c
来源：http://vlr.haohaochexian.top

C#:   a && b || !c
来源：http://sle.yfazqb.com

[B16] 卫语句：不满足条件提前返回
来源：http://cul.ctjpmb.com

Py:   if not data: return
来源：http://wsm.ydjk.org.cn

PHP:  if (!$data) { return; }
来源：http://kle.cqqwz.cn

JS:   if (!data) return;
来源：http://dbz.chenzaomai.com

TS:   if (!data) return;
来源：http://sos.yj202588.top

Java: if (data == null) return;
来源：http://jll.gaohongyu789.top

Go:   if data == nil { return }
来源：http://ppt.xuanzx.com

Ruby: return if data.nil?
来源：http://bpa.pycfn.com

C#:   if (data == null) return;
来源：http://klg.c1oappe.top

================================================================================
来源：http://zum.ehwqpu.com

C. 函数与作用域
来源：http://jcb.zhixingplan.top

================================================================================
来源：http://ken.shangyingyoupin.top

[C01] 定义函数
来源：http://rtr.xinyue.icu

Py:   def add(a, b): return a + b
来源：http://duw.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qcl.cucudq.cn

JS:   function add(a, b) { return a + b; }
来源：http://nxg.zhixingplan.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ntm.kuanghao11.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ygj.gzhubu.top

Go:   func add(a, b int) int { return a + b }
来源：http://nec.ywan-chungtsiang.top

Ruby: def add(a, b); a + b; end
来源：http://jtp.chenlongwang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://grd.zhengqikj.top


<!-- 参考信息 -->