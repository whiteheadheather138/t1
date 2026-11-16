代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://pmj.meibo888.top

[A11] 条件表达式（三元）
来源：http://lud.chenjidiqi.icu

Py:   "yes" if x > 0 else "no"
来源：http://obv.uphjek.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://hhz.andypj.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://zbv.chenjidiqi.icu

TS:   x > 0 ? "yes" : "no"
来源：http://ibk.zhixingplan.top

Java: x > 0 ? "yes" : "no"
来源：http://wpd.jinqigfzy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://vfl.shzxlz.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://std.sxryk.cn

C#:   x > 0 ? "yes" : "no"
来源：http://scc.hnqzz.top

[A12] 字符串插值 / 格式化
来源：http://egi.fzhhl.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://few.jlsjyb.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fgg.0kj1m.cn

JS:   `Hello, ${name}!`
来源：http://wvr.quarkkingdee.top

TS:   `Hello, ${name}!`
来源：http://gee.tanke756.top

Java: "Hello, %s!".formatted(name)
来源：http://ful.yanxiufei.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hsd.hesvh.cn

Ruby: "Hello, #{name}!"
来源：http://vdd.yvedp.cn

C#:   $"Hello, {name}!"
来源：http://dnf.iojbl.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jtc.zdbjq.cn

Py:   "第一行\n第二行"
来源：http://waz.jianghu66.top

PHP:  "第一行\n第二行"
来源：http://yfb.zhiwuduotai.top

JS:   "第一行\n第二行"
来源：http://ujb.9152youxi.cn

TS:   "第一行\n第二行"
来源：http://dnr.zhoulong.xyz

Java: "第一行\n第二行"
来源：http://qix.nanxuanxn.top

Go:   "第一行\n第二行"
来源：http://rww.tian-w.cn

Ruby: "第一行\n第二行"
来源：http://gjb.aibaodan.cn

C#:   "第一行\n第二行"
来源：http://dqq.ybcxt.top

[A14] 注释写法
来源：http://dxv.birdmap.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://hui.iojbl.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ntc.ydzc1.top

JS:   // 单行；/* 多行 */
来源：http://zfo.52xcode.cn

TS:   // 单行；/* 多行 */
来源：http://hqf.zdbjq.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kqa.dashuyun.cn

Go:   // 单行；/* 多行 */
来源：http://gar.yfazqb.com

Ruby: # 单行；=begin 多行 =end
来源：http://ala.jqgufenzy.top

C#:   // 单行；/* 多行 */
来源：http://yxu.sjlbkw.cn

[A15] 空值判断与默认值
来源：http://yqj.pengpengdd.cyou

Py:   value = data or "默认值"
来源：http://ppc.jianghu66.top

PHP:  $value = $data ?? "默认值";
来源：http://vxi.0kj1m.cn

JS:   const value = data ?? "默认值";
来源：http://ugi.shuidangran.top

TS:   const value = data ?? "默认值";
来源：http://ggb.mhx1999.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ezb.cashguo.top

Go:   if data == "" { data = "默认值" }
来源：http://zmf.ctjpmb.com

Ruby: value = data || "默认值"
来源：http://mjc.feifeiyinyue.top

C#:   var value = data ?? "默认值";
来源：http://mbs.sufxvd.cn

[A16] 真假值判断规则
来源：http://xzs.svipenyu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://chk.hnqzz.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xoq.dashuyun.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hqt.nwbrower.top

TS:   if (!x) {}
来源：http://mnx.yuxming.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wqq.dianchejie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wvg.guowangkeji.top

Ruby: unless x            # nil 与 false 为假
来源：http://zqw.meibo888.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xhv.shangyingyoupin.top

[A17] 位运算
来源：http://bvf.xinyue.icu

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tyw.shzxlz.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vzh.9152youxi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://llv.tarul.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rdz.pycfn.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dio.zhijiandao.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fzl.sjlbkw.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bfv.shangyingyoupin.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xum.havefunace.top

[A18] 字符与 ASCII 码互转
来源：http://kug.bjfxy.top

Py:   ord("A"); chr(65)
来源：http://ubd.meibo888.top

PHP:  ord("A"); chr(65)
来源：http://pcp.jianghu66.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qgv.vehdjk.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qgz.ydzc1.top

Java: (int) 'A'; (char) 65
来源：http://fhr.9152youxi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ojn.gzhubu.top

Ruby: "A".ord; 65.chr
来源：http://doe.shzxlz.cn

C#:   (int)'A'; (char)65
来源：http://zcm.hysaishi.cn

[A19] 交换两个变量
来源：http://kfb.ivvv.top

Py:   a, b = b, a
来源：http://uen.c1oappe.top

PHP:  [$a, $b] = [$b, $a];
来源：http://xdk.ybcxt.top

JS:   [a, b] = [b, a];
来源：http://ffu.uphjek.com

TS:   [a, b] = [b, a];
来源：http://pyz.zycfv.cn

Java: int t = a; a = b; b = t;
来源：http://udc.jiagoushi.top

Go:   a, b = b, a
来源：http://pgt.hywenlv.cn

Ruby: a, b = b, a
来源：http://bmc.zhoulong.xyz

C#:   (a, b) = (b, a);
来源：http://nsb.cqqwz.cn

[A20] 读取标准输入
来源：http://yjd.yuxming.cn

Py:   name = input("请输入：")
来源：http://dhc.sysykeji.top

PHP:  $name = trim(fgets(STDIN));
来源：http://iaw.hesvh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mqa.yuanzhike.top

TS:   // Node.js：readline 模块
来源：http://mok.cucudq.cn

Java: new Scanner(System.in).nextLine()
来源：http://sjr.meibo888.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fbm.jianghu66.top

Ruby: gets.chomp
来源：http://wdp.fehbvm.com

C#:   Console.ReadLine();
来源：http://jon.hnqzz.top

[A21] 保留指定小数位输出
来源：http://vwk.tarul.cn

Py:   f"{3.14159:.2f}"
来源：http://bon.vqdsnc.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lpi.yj20258888.top

JS:   (3.14159).toFixed(2)
来源：http://mqg.chenjidiqi.icu

TS:   (3.14159).toFixed(2)
来源：http://ryh.fehbvm.com

Java: String.format("%.2f", 3.14159)
来源：http://sfv.jqgfzy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zaz.chenjidiqi.icu

Ruby: format("%.2f", 3.14159)
来源：http://qmf.shangyingyoupin.top

C#:   3.14159.ToString("F2")
来源：http://rsx.hcnkem.com

[A22] 获取字符串长度
来源：http://qwq.bjfxy.top

Py:   len(s)
来源：http://heb.chenzaomai.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rhr.yuanzhike.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mce.jinyuanbaomall.cn

TS:   s.length
来源：http://ghy.yj20258888.top

Java: s.length()
来源：http://lda.jinqigufen.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rrf.jinyuanbaomall.cn

Ruby: s.length
来源：http://nso.pycfn.com

C#:   s.Length
来源：http://pvf.bjfxy.top

[A23] 大小写转换
来源：http://jzt.mhx1999.top

Py:   s.upper(); s.lower(); s.title()
来源：http://mei.hnqzz.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kkm.nwbrower.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://okl.ybcxt.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ypc.ydjk.org.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zbl.ybcxt.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oae.fzhhl.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xkp.dashuyun.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gbv.yj202588.top

[A24] 去除首尾空白
来源：http://zgw.c1oappe.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pzm.gogol.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rnt.sxryk.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jaz.hnxiangtu.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vxr.chenlongwang.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gcl.pycfn.com

Go:   strings.TrimSpace(s)
来源：http://smi.uphjek.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cdv.aizwys.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cyu.meibo888.top

[A25] 字符串比较
来源：http://fay.shuidangran.top

Py:   s1 == s2; s1 != s2
来源：http://xzg.hammf.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dfr.redwolf501.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ude.kuanghao11.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wra.0kj1m.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wyb.feifeiyinyue.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fqv.shzxlz.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tll.snrcjt.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hmh.gotoacloud.top

[A26] 类型转换总览
来源：http://rae.haohaochexian.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gwz.gogol.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wqq.jinqigfzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ksv.mhx1999.top

TS:   Number() String() Boolean() x as number
来源：http://xtt.0kj1m.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yas.hysaishi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qqa.shuidangran.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://qhf.zhoulong.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zoc.cqqwz.cn

================================================================================
来源：http://xxb.jqgfzy.top

B. 流程控制
来源：http://jhs.andypj.xyz

================================================================================
来源：http://uln.ydjk.org.cn

[B01] 条件判断 if / else
来源：http://cvd.epnwcf.com

Py:   result = "正" if x > 0 else "非正"
来源：http://luw.hesvh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://iee.fanxiaobao.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iqs.yangfankeji.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vbw.ivvv.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://tyy.nwbrower.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://npv.zhiwuduotai.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oxu.jinyuanbaomall.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wtx.ehwqpu.com

[B02] 多分支 else if / elif
来源：http://ssd.yongpay.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://puo.chenlongwang.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tqt.fktsv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lri.sjlbkw.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oja.cqqwz.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mza.hnxiangtu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qmm.vqdsnc.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xkl.cheryme.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bwq.tianlin.xyz

[B03] switch / match / case
来源：http://jqq.chenzaomai.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hoe.mhx1999.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yoq.tanke756.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jqa.ehwqpu.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eup.xuanzx.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ykt.bjfxy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hdl.yuxming.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tdg.yonumen.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mhf.xingfuxueyuan.xyz

[B04] for 计数循环
来源：http://xsc.vehdjk.com

Py:   for i in range(10): print(i)
来源：http://ron.sweek.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dhf.tanke756.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dll.guannengcc.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://niz.ybcxt.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mpr.aibaodan.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hxa.yj202588.top

Ruby: 10.times { |i| puts i }
来源：http://woj.yj202588.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zax.ydjk.org.cn

[B05] 遍历数组 / 列表
来源：http://kpy.ppjwa.cn

Py:   for item in arr: print(item)
来源：http://jah.sysykeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yyv.ybcxt.top

JS:   for (const item of arr) { console.log(item); }
来源：http://yzp.haohaochexian.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ryv.havefunace.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://gfz.zhongyouzk.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://scb.svipenyu.cn

Ruby: arr.each { |item| puts item }
来源：http://bdb.aibaodan.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bbs.zdbjq.cn

[B06] 遍历字典 / 对象
来源：http://fdt.sjlbkw.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://aob.meibo888.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pwd.pengpengdd.cyou

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uqh.9152youxi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kdd.gotoacloud.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dbj.ybcxt.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rcq.yueranfly.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wfz.daxiang520.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cvw.ywan-chungtsiang.top

[B07] while 循环
来源：http://wat.yangfankeji.com

Py:   while i < 10: i += 1
来源：http://ygh.tianlin.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://mkp.zdbjq.cn

JS:   while (i < 10) { i++; }
来源：http://dgq.c1oappe.top

TS:   while (i < 10) { i++; }
来源：http://yhw.9152youxi.cn

Java: while (i < 10) { i++; }
来源：http://atz.xingfuxueyuan.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gmy.vqdsnc.cn

Ruby: while i < 10; i += 1; end
来源：http://umn.hammf.cn

C#:   while (i < 10) { i++; }
来源：http://unj.hesvh.cn

[B08] do-while（至少执行一次）
来源：http://wsb.fanxiaobao.xyz

Py:   # 无 do-while：用 while True + break
来源：http://age.quarkkingdee.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ffs.bjfxy.top

JS:   do { i++; } while (i < 10);
来源：http://cvd.haohaochexian.top

TS:   do { i++; } while (i < 10);
来源：http://lcp.jinghuilouyu.cn

Java: do { i++; } while (i < 10);
来源：http://hbk.hysaishi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ktg.0kj1m.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fbg.shanyushiyangtech.top

C#:   do { i++; } while (i < 10);
来源：http://ixy.fehbvm.com

[B09] break 与 continue
来源：http://ebz.zdbjq.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kmw.xinyue.icu

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tgc.aizwys.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wpx.ivvv.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mcc.shuidangran.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cyt.chenjidiqi.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://roj.jqgufenzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jtc.shangyingyoupin.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qjq.iojbl.cn

[B10] 遍历同时拿索引
来源：http://rls.quarkkingdee.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oga.guannengcc.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rsg.hcnkem.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jov.meibo888.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xxw.cucudq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wpt.nanxuanxn.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hco.zdbjq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ehv.0kj1m.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yhn.jinghuilouyu.cn

[B11] 生成数字序列 / 区间
来源：http://lfj.hywenlv.cn

Py:   list(range(0, 10, 2))
来源：http://xtd.zhiwuduotai.top

PHP:  range(0, 10, 2);
来源：http://xqd.jinqigfzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qpl.chenlongwang.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qda.hammf.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gqt.cashguo.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qvr.hfpthk.cn

Ruby: (0...10).step(2).to_a
来源：http://akn.smart0.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://srf.cqqwz.cn

[B12] 跳出多层循环
来源：http://vnv.daxiang520.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qfm.zhaomingkeji.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://afv.ydzc1.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rfk.jinyuanbaomall.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://eia.daxiang520.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rlp.iojbl.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nma.pengpengdd.cyou

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qfa.zhixingplan.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xic.vehdjk.com

[B13] 判断是否为数字
来源：http://hhn.yj202588.top

Py:   isinstance(x, (int, float))
来源：http://llq.haohaochexian.top

PHP:  is_numeric($x)
来源：http://ktc.gaohongyu789.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dao.jinghuilouyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yms.cashguo.top

Java: x instanceof Number
来源：http://mne.ehwqpu.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yeo.yongpay.top

Ruby: x.is_a?(Numeric)
来源：http://ejf.chenlongwang.top

C#:   x is int or double or decimal
来源：http://nvu.dashuyun.cn

[B14] 判断值是否在集合内
来源：http://ysp.andypj.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xul.hnqzz.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jra.yuanzhike.top

JS:   [1, 2, 3].includes(x)
来源：http://akq.bjfxy.top

TS:   [1, 2, 3].includes(x)
来源：http://sgv.aizwys.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://clh.gogol.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fir.mhx1999.top

Ruby: [1, 2, 3].include?(x)
来源：http://etl.jinqigufen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ndn.ybcxt.top

[B15] 布尔运算与取反
来源：http://ysc.hammf.cn

Py:   a and b or not c
来源：http://iyk.gotoacloud.top

PHP:  $a && $b || !$c
来源：http://lif.hesvh.cn

JS:   a && b || !c
来源：http://gws.bjfxy.top

TS:   a && b || !c
来源：http://bkj.fengsongda.top

Java: a && b || !c
来源：http://gvk.yfazqb.com

Go:   a && b || !c
来源：http://tjh.gaohongyu789.top

Ruby: a && b || !c
来源：http://dqd.zhijiandao.cn

C#:   a && b || !c
来源：http://xts.xuanzx.com

[B16] 卫语句：不满足条件提前返回
来源：http://gle.jinghuilouyu.cn

Py:   if not data: return
来源：http://dyd.meibo888.top

PHP:  if (!$data) { return; }
来源：http://fvg.chenzaomai.com

JS:   if (!data) return;
来源：http://jss.svipenyu.cn

TS:   if (!data) return;
来源：http://gvk.fengsongda.top

Java: if (data == null) return;
来源：http://sto.yj20258.top

Go:   if data == nil { return }
来源：http://hbr.smart0.xyz

Ruby: return if data.nil?
来源：http://yoj.cashguo.top

C#:   if (data == null) return;
来源：http://cwd.tarul.cn

================================================================================
来源：http://yhu.yj202588.top

C. 函数与作用域
来源：http://rlk.chenzaomai.com

================================================================================
来源：http://tve.hcnkem.com

[C01] 定义函数
来源：http://tzp.aibaodan.cn

Py:   def add(a, b): return a + b
来源：http://yeu.hywenlv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gsf.zhijiandao.cn

JS:   function add(a, b) { return a + b; }
来源：http://sky.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sow.birdmap.top


<!-- 参考信息 -->