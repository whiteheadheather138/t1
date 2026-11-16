代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://zlo.yangfankeji.com

TS:   x > 0 ? "yes" : "no"
来源：http://vkn.dianchejie.cn

Java: x > 0 ? "yes" : "no"
来源：http://olv.pycfn.com

Go:   // 无三元运算符，需用 if 语句
来源：http://fgc.jiagoushi.top

Ruby: x > 0 ? "yes" : "no"
来源：http://gti.aizwys.cn

C#:   x > 0 ? "yes" : "no"
来源：http://njl.tianlin.xyz

[A12] 字符串插值 / 格式化
来源：http://tgk.wangdashe.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xzx.316326.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ezs.yuanzhike.top

JS:   `Hello, ${name}!`
来源：http://cik.shanyushiyangtech.top

TS:   `Hello, ${name}!`
来源：http://kkm.birdmap.top

Java: "Hello, %s!".formatted(name)
来源：http://bwt.pengpengdd.cyou

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jzu.tian-w.cn

Ruby: "Hello, #{name}!"
来源：http://fej.fktsv.cn

C#:   $"Hello, {name}!"
来源：http://kzs.redwolf501.top

[A13] 多行字符串（练习 \n 转义）
来源：http://yon.guannengcc.top

Py:   "第一行\n第二行"
来源：http://mqk.jqgfzy.top

PHP:  "第一行\n第二行"
来源：http://bat.hnqzz.top

JS:   "第一行\n第二行"
来源：http://slo.gaohongyu789.top

TS:   "第一行\n第二行"
来源：http://tkb.yj202588.top

Java: "第一行\n第二行"
来源：http://hmp.hnqzz.top

Go:   "第一行\n第二行"
来源：http://jkd.havefunace.top

Ruby: "第一行\n第二行"
来源：http://nqr.316326.xyz

C#:   "第一行\n第二行"
来源：http://yrz.yj20258888.top

[A14] 注释写法
来源：http://zqb.fktsv.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fvp.sufxvd.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kqe.zhengqikj.top

JS:   // 单行；/* 多行 */
来源：http://bpt.bjfxy.top

TS:   // 单行；/* 多行 */
来源：http://opg.yangfankeji.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hng.zhijiandao.cn

Go:   // 单行；/* 多行 */
来源：http://grz.hfpthk.cn

Ruby: # 单行；=begin 多行 =end
来源：http://nvg.52xcode.cn

C#:   // 单行；/* 多行 */
来源：http://nsf.hammf.cn

[A15] 空值判断与默认值
来源：http://rge.hammf.cn

Py:   value = data or "默认值"
来源：http://rur.andypj.xyz

PHP:  $value = $data ?? "默认值";
来源：http://hjk.yangfankeji.com

JS:   const value = data ?? "默认值";
来源：http://zso.fanxiaobao.xyz

TS:   const value = data ?? "默认值";
来源：http://mrz.zhongyouzk.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nyu.hysaishi.cn

Go:   if data == "" { data = "默认值" }
来源：http://psv.jqgufenzy.top

Ruby: value = data || "默认值"
来源：http://oiy.ehwqpu.com

C#:   var value = data ?? "默认值";
来源：http://xyt.nanxuanxn.top

[A16] 真假值判断规则
来源：http://fxj.epnwcf.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ghs.zhijiandao.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qkn.tarul.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rnr.cheryme.top

TS:   if (!x) {}
来源：http://kjd.ydjk.org.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tqu.gaohongyu789.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ivp.fehbvm.com

Ruby: unless x            # nil 与 false 为假
来源：http://qdg.sysykeji.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kea.shzxlz.cn

[A17] 位运算
来源：http://nqx.jinyuanbaomall.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ynf.hywenlv.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fup.guannengcc.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://egv.redwolf501.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://aow.meibo888.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mrm.tanke756.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kkp.vehdjk.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eay.xingfuxueyuan.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lii.hammf.cn

[A18] 字符与 ASCII 码互转
来源：http://kzk.hfpthk.cn

Py:   ord("A"); chr(65)
来源：http://ugh.yueranfly.top

PHP:  ord("A"); chr(65)
来源：http://giv.gotoacloud.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nmy.jianghu66.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gog.shanyushiyangkeji.top

Java: (int) 'A'; (char) 65
来源：http://rgo.mhx1999.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lyk.pycfn.com

Ruby: "A".ord; 65.chr
来源：http://twc.fehbvm.com

C#:   (int)'A'; (char)65
来源：http://qhz.meibo888.top

[A19] 交换两个变量
来源：http://hey.sxryk.cn

Py:   a, b = b, a
来源：http://sev.sysykeji.top

PHP:  [$a, $b] = [$b, $a];
来源：http://syc.gzhubu.top

JS:   [a, b] = [b, a];
来源：http://sbq.yj20258888.top

TS:   [a, b] = [b, a];
来源：http://zck.jiagoushi.top

Java: int t = a; a = b; b = t;
来源：http://qgv.yj20258.top

Go:   a, b = b, a
来源：http://ihn.iojbl.cn

Ruby: a, b = b, a
来源：http://ziz.xylfe.cn

C#:   (a, b) = (b, a);
来源：http://ein.gotoacloud.top

[A20] 读取标准输入
来源：http://zln.birdmap.top

Py:   name = input("请输入：")
来源：http://omn.jinghuilouyu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jts.havefunace.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xpd.shuidangran.top

TS:   // Node.js：readline 模块
来源：http://mdq.dashuyun.cn

Java: new Scanner(System.in).nextLine()
来源：http://kda.hfpthk.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xsl.pengpengdd.cyou

Ruby: gets.chomp
来源：http://cnv.shuidangran.top

C#:   Console.ReadLine();
来源：http://hbl.vqdsnc.cn

[A21] 保留指定小数位输出
来源：http://pkb.nanxuanxn.top

Py:   f"{3.14159:.2f}"
来源：http://mki.hysaishi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ynj.yanxiufei.cn

JS:   (3.14159).toFixed(2)
来源：http://oeo.hongshengwenyu.top

TS:   (3.14159).toFixed(2)
来源：http://hdn.tianlin.xyz

Java: String.format("%.2f", 3.14159)
来源：http://zvu.yuxming.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zir.jianghu66.top

Ruby: format("%.2f", 3.14159)
来源：http://kbi.jyoumei.cn

C#:   3.14159.ToString("F2")
来源：http://oel.ctjpmb.com

[A22] 获取字符串长度
来源：http://nae.ydjk.org.cn

Py:   len(s)
来源：http://szh.yongpay.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://udl.svipenyu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ltu.haohaochexian.top

TS:   s.length
来源：http://uip.daxiang520.top

Java: s.length()
来源：http://aoy.cashguo.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wah.gogol.net.cn

Ruby: s.length
来源：http://eyn.ehwqpu.com

C#:   s.Length
来源：http://tto.0kj1m.cn

[A23] 大小写转换
来源：http://zpv.jianghu66.top

Py:   s.upper(); s.lower(); s.title()
来源：http://xbz.vehdjk.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ixg.snrcjt.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bcl.sufxvd.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yha.xinyue.icu

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wbq.yonumen.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fmj.chenzaomai.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nhj.ppjwa.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jam.zhoulong.xyz

[A24] 去除首尾空白
来源：http://mtn.jlsjyb.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fkb.ppjwa.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xxn.yonumen.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dck.fanxiaobao.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cjt.0kj1m.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pks.cucudq.cn

Go:   strings.TrimSpace(s)
来源：http://gci.yangfankeji.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://slr.sxryk.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://soj.cucudq.cn

[A25] 字符串比较
来源：http://sjh.ivvv.top

Py:   s1 == s2; s1 != s2
来源：http://mvc.wangshuangyany.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tlg.dashuyun.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bao.redwolf501.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://drj.zhoulong.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lzm.jinqigufen.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://eyg.xinyue.icu

Ruby: s1 == s2; s1 <=> s2
来源：http://dka.zhiwuduotai.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jao.daria6918.cn

[A26] 类型转换总览
来源：http://zaa.ydzc1.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sas.ctjpmb.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://moo.shzxlz.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pxq.tanke756.top

TS:   Number() String() Boolean() x as number
来源：http://ida.havefunace.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tec.fanxiaobao.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cxp.fanxiaobao.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://kpx.52xcode.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jcr.tianlin.xyz

================================================================================
来源：http://zst.sysykeji.top

B. 流程控制
来源：http://ttt.mhx1999.top

================================================================================
来源：http://non.xuetiantiany.cn

[B01] 条件判断 if / else
来源：http://ury.feifeiyinyue.top

Py:   result = "正" if x > 0 else "非正"
来源：http://xot.hnxiangtu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://twp.vehdjk.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xob.bjfxy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://eig.shanyushiyangkeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://pvc.fehbvm.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xeo.yueranfly.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ccu.hcnkem.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jlh.ydjk.org.cn

[B02] 多分支 else if / elif
来源：http://cmy.hnqzz.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ysg.pycfn.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mtm.tian-w.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vvv.yueranfly.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://csr.zhijiandao.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yoa.yongpay.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lph.vehdjk.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hww.shanyushiyangtech.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mtv.cashguo.top

[B03] switch / match / case
来源：http://mmi.ywan-chungtsiang.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ddt.jiagoushi.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vvn.iojbl.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fwq.cdnleiting.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rpi.jqgfzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://upt.haohaochexian.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sls.sufxvd.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nvw.hnxiangtu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yes.ivvv.top

[B04] for 计数循环
来源：http://soh.tarul.cn

Py:   for i in range(10): print(i)
来源：http://vqq.zdbjq.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nbj.jyoumei.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rzy.shanyushiyangtech.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yqg.xinyue.icu

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nqa.jiagoushi.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://svf.bbcook.cn

Ruby: 10.times { |i| puts i }
来源：http://ggn.tarul.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bcy.daria6918.cn

[B05] 遍历数组 / 列表
来源：http://zrx.hywenlv.cn

Py:   for item in arr: print(item)
来源：http://iuo.jiagoushi.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hwk.hywenlv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://stc.jianghu66.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ajo.guowangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://vao.shuidangran.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wsu.yj20258888.top

Ruby: arr.each { |item| puts item }
来源：http://mbf.zhoulong.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kvn.snrcjt.cn

[B06] 遍历字典 / 对象
来源：http://xgi.hesvh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fui.jinqigfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uvv.c1oappe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fjb.zhongyouzk.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qpb.ybcxt.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hpo.hesvh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://acq.xuanzx.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lmj.tanke756.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hli.yuxming.cn

[B07] while 循环
来源：http://iia.tian-w.cn

Py:   while i < 10: i += 1
来源：http://mlu.yangfankeji.com

PHP:  while ($i < 10) { $i++; }
来源：http://ijm.xziqi.cn

JS:   while (i < 10) { i++; }
来源：http://qzm.ydjk.org.cn

TS:   while (i < 10) { i++; }
来源：http://gle.yj20258.top

Java: while (i < 10) { i++; }
来源：http://ysg.52xcode.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lmx.hnxiangtu.top

Ruby: while i < 10; i += 1; end
来源：http://naz.quarkkingdee.top

C#:   while (i < 10) { i++; }
来源：http://tby.wangdashe.top

[B08] do-while（至少执行一次）
来源：http://ynt.shanyushiyangtech.top

Py:   # 无 do-while：用 while True + break
来源：http://msw.0kj1m.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tuc.epnwcf.com

JS:   do { i++; } while (i < 10);
来源：http://qwn.hcnkem.com

TS:   do { i++; } while (i < 10);
来源：http://nqi.fanxiaobao.xyz

Java: do { i++; } while (i < 10);
来源：http://ukk.tian-w.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ghk.jinqigufen.top

Ruby: begin; i += 1; end while i < 10
来源：http://vuw.yonumen.top

C#:   do { i++; } while (i < 10);
来源：http://wad.cucudq.cn

[B09] break 与 continue
来源：http://bfj.yj20258888.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://aid.andypj.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kui.zhaomingkeji.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://myz.pycfn.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uqj.dianchejie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fuj.sxryk.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dqd.havefunace.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ylg.uphjek.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dmm.dashuyun.cn

[B10] 遍历同时拿索引
来源：http://pyt.316326.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hjk.xingfuxueyuan.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zht.vehdjk.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://guw.ehwqpu.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mzz.nanxinkj.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://abh.quarkkingdee.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lir.wangshuangyany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ohy.snrcjt.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://srf.gaohongyu789.top

[B11] 生成数字序列 / 区间
来源：http://uyv.yj20258.top

Py:   list(range(0, 10, 2))
来源：http://eyu.fanxiaobao.xyz

PHP:  range(0, 10, 2);
来源：http://qpl.hammf.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cvb.cheryme.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kha.gaohongyu789.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kmj.gaohongyu789.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://smi.yj20258888.top

Ruby: (0...10).step(2).to_a
来源：http://wwa.tarul.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hzx.yj202588.top

[B12] 跳出多层循环
来源：http://zpa.mhx1999.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xyc.guowangkeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xxo.ivvv.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://khh.jinqigfzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hls.zdbjq.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://voc.vehdjk.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wcz.hongshengwenyu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jhr.zhiwuduotai.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wst.fehbvm.com

[B13] 判断是否为数字
来源：http://dmp.quarkkingdee.top

Py:   isinstance(x, (int, float))
来源：http://awh.gaohongyu789.top

PHP:  is_numeric($x)
来源：http://eyj.zhiwuduotai.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zlr.ywan-chungtsiang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bhs.yj20258888.top

Java: x instanceof Number
来源：http://xhk.shangyingyoupin.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://phw.guowangkeji.top

Ruby: x.is_a?(Numeric)
来源：http://akx.guowangkeji.top

C#:   x is int or double or decimal
来源：http://bjr.guannengcc.top

[B14] 判断值是否在集合内
来源：http://ofk.redwolf501.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aii.jqgfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ppr.yuanzhike.top

JS:   [1, 2, 3].includes(x)
来源：http://ken.yueranfly.top

TS:   [1, 2, 3].includes(x)
来源：http://bcy.ydjk.org.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vii.jianghu66.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gct.cucudq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qws.aibaodan.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lfm.gaohongyu789.top

[B15] 布尔运算与取反
来源：http://tym.chenzaomai.com

Py:   a and b or not c
来源：http://ajw.jiagoushi.top

PHP:  $a && $b || !$c
来源：http://tdj.xziqi.cn

JS:   a && b || !c
来源：http://dnk.uphjek.com

TS:   a && b || !c
来源：http://vdy.yueranfly.top

Java: a && b || !c
来源：http://rge.zycfv.cn

Go:   a && b || !c
来源：http://kvs.hesvh.cn

Ruby: a && b || !c
来源：http://rmk.aizwys.cn

C#:   a && b || !c
来源：http://oww.316326.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://wft.meibo888.top

Py:   if not data: return
来源：http://fze.shangyingyoupin.top

PHP:  if (!$data) { return; }
来源：http://ccv.vehdjk.com

JS:   if (!data) return;
来源：http://lrb.jinqigufen.top

TS:   if (!data) return;
来源：http://itx.zdbjq.cn

Java: if (data == null) return;
来源：http://ysu.jinyuanbaomall.cn

Go:   if data == nil { return }
来源：http://ilv.316326.xyz

Ruby: return if data.nil?
来源：http://dln.yangfankeji.com

C#:   if (data == null) return;
来源：http://amv.daxiang520.top

================================================================================
来源：http://smx.smart0.xyz

C. 函数与作用域
来源：http://mxm.svipenyu.cn

================================================================================
来源：http://gsy.havefunace.top

[C01] 定义函数
来源：http://mjv.zycfv.cn

Py:   def add(a, b): return a + b
来源：http://rjq.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oxa.yanxiufei.cn

JS:   function add(a, b) { return a + b; }
来源：http://xfl.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zuz.jinqigufen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://oyp.cqqwz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hir.yuxming.cn

Ruby: def add(a, b); a + b; end
来源：http://epj.bjfxy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wxv.hammf.cn


<!-- 参考信息 -->