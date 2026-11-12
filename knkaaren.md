代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ekb.xingfuxueyuan.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pev.jlsjyb.cn

TS:   if (!x) {}
来源：http://kog.yvedp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gji.yongpay.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://puq.ppjwa.cn

Ruby: unless x            # nil 与 false 为假
来源：http://caq.smart0.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vxd.cheryme.top

[A17] 位运算
来源：http://uke.nanxinkj.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fdm.yuanzhike.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://itp.cashguo.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fwm.sjlbkw.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zpn.jianghu66.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hoc.hnxiangtu.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cwt.iojbl.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dxr.gaohongyu789.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wsg.ppjwa.cn

[A18] 字符与 ASCII 码互转
来源：http://tpp.tarul.cn

Py:   ord("A"); chr(65)
来源：http://pkj.epnwcf.com

PHP:  ord("A"); chr(65)
来源：http://dvu.havefunace.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dvx.52xcode.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xhc.hysaishi.cn

Java: (int) 'A'; (char) 65
来源：http://dyj.sjlbkw.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://coi.feifeiyinyue.top

Ruby: "A".ord; 65.chr
来源：http://ebr.jinghuilouyu.cn

C#:   (int)'A'; (char)65
来源：http://zdv.havefunace.top

[A19] 交换两个变量
来源：http://nyk.zycfv.cn

Py:   a, b = b, a
来源：http://chl.fktsv.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fub.c1oappe.top

JS:   [a, b] = [b, a];
来源：http://xzm.havefunace.top

TS:   [a, b] = [b, a];
来源：http://iru.cashguo.top

Java: int t = a; a = b; b = t;
来源：http://jyl.0kj1m.cn

Go:   a, b = b, a
来源：http://nbq.yj20258.top

Ruby: a, b = b, a
来源：http://aqe.zycfv.cn

C#:   (a, b) = (b, a);
来源：http://yna.aibaodan.cn

[A20] 读取标准输入
来源：http://alq.cucudq.cn

Py:   name = input("请输入：")
来源：http://ikb.xuetiantiany.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ovr.gotoacloud.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://azr.vehdjk.com

TS:   // Node.js：readline 模块
来源：http://fnl.yuxming.cn

Java: new Scanner(System.in).nextLine()
来源：http://oao.yj20258888.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://leu.jqgufenzy.top

Ruby: gets.chomp
来源：http://cup.jiagoushi.top

C#:   Console.ReadLine();
来源：http://jng.quarkkingdee.top

[A21] 保留指定小数位输出
来源：http://iwv.zhixingplan.top

Py:   f"{3.14159:.2f}"
来源：http://tsz.jinghuilouyu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jdd.epnwcf.com

JS:   (3.14159).toFixed(2)
来源：http://any.fehbvm.com

TS:   (3.14159).toFixed(2)
来源：http://yen.0kj1m.cn

Java: String.format("%.2f", 3.14159)
来源：http://pbs.meibo888.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://atq.jqgfzy.top

Ruby: format("%.2f", 3.14159)
来源：http://wwc.ywan-chungtsiang.top

C#:   3.14159.ToString("F2")
来源：http://bsk.yanxiufei.cn

[A22] 获取字符串长度
来源：http://uuh.iojbl.cn

Py:   len(s)
来源：http://anw.yanxiufei.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pcf.shangyingyoupin.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yjb.cheryme.top

TS:   s.length
来源：http://jvc.feifeiyinyue.top

Java: s.length()
来源：http://bfo.xziqi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sto.snrcjt.cn

Ruby: s.length
来源：http://mhk.ppjwa.cn

C#:   s.Length
来源：http://zur.shanyushiyangtech.top

[A23] 大小写转换
来源：http://oar.hesvh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ubl.sweek.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qtl.aibaodan.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uye.chenzaomai.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rpv.dianchejie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pra.xingfuxueyuan.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xqn.zhoulong.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uix.svipenyu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ayo.svipenyu.cn

[A24] 去除首尾空白
来源：http://iln.ybcxt.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lya.yonumen.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ekr.jyoumei.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nyi.wangshuangyany.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ypx.jqgfzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://izg.sysykeji.top

Go:   strings.TrimSpace(s)
来源：http://mai.zhixingplan.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jac.52xcode.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wbo.ydjk.org.cn

[A25] 字符串比较
来源：http://dly.aibaodan.cn

Py:   s1 == s2; s1 != s2
来源：http://hge.yvedp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sju.316326.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yiv.chenzaomai.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ugk.smart0.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gar.xinyue.icu

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://oet.sjlbkw.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://epo.hnxiangtu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hyo.zhaomingkeji.xyz

[A26] 类型转换总览
来源：http://kfg.yj20258888.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://crt.ydjk.org.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rsk.zhaomingkeji.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://woo.dianchejie.cn

TS:   Number() String() Boolean() x as number
来源：http://iqz.yj20258888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nwf.epnwcf.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iho.birdmap.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://cil.sxryk.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bvv.gzhubu.top

================================================================================
来源：http://wbr.shanyushiyangkeji.top

B. 流程控制
来源：http://itn.sweek.top

================================================================================
来源：http://xng.yj20258888.top

[B01] 条件判断 if / else
来源：http://xxk.gzhubu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://hri.meibo888.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wcq.havefunace.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zrv.yonumen.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mkt.smart0.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://opr.52xcode.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gdx.quarkkingdee.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://okj.cucudq.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dcs.gogol.net.cn

[B02] 多分支 else if / elif
来源：http://zpc.dashuyun.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://waf.jinyuanbaomall.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://afo.nanxinkj.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hhf.nanxuanxn.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hsw.havefunace.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://azy.yj20258.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lnq.birdmap.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mib.jqgufenzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eok.wangdashe.top

[B03] switch / match / case
来源：http://pya.jinghuilouyu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lrl.shanyushiyangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sax.cheryme.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vzf.chenlongwang.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nuk.dashuyun.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lkt.andypj.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oac.hnxiangtu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yro.zhixingplan.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pxd.shanyushiyangkeji.top

[B04] for 计数循环
来源：http://obf.mhx1999.top

Py:   for i in range(10): print(i)
来源：http://lju.cqqwz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://smq.snrcjt.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vbq.gaohongyu789.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gsa.tanke756.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fmk.zdqjudy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://elc.dashuyun.cn

Ruby: 10.times { |i| puts i }
来源：http://pds.epnwcf.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fyc.jiagoushi.top

[B05] 遍历数组 / 列表
来源：http://ulf.mhx1999.top

Py:   for item in arr: print(item)
来源：http://spq.sjlbkw.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uoc.sjlbkw.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fqj.fzhhl.top

TS:   for (const item of arr) { console.log(item); }
来源：http://icz.shanyushiyangtech.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tih.sufxvd.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ukb.jianghu66.top

Ruby: arr.each { |item| puts item }
来源：http://dba.andypj.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ico.hysaishi.cn

[B06] 遍历字典 / 对象
来源：http://cmb.xingfuxueyuan.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://mgk.havefunace.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dmc.hywenlv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ntp.yanxiufei.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dfl.fengsongda.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wzh.cheryme.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zuf.hysaishi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vfi.zhengqikj.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uyw.shuidangran.top

[B07] while 循环
来源：http://bag.jinqigufen.top

Py:   while i < 10: i += 1
来源：http://lxq.wangshuangyany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mzt.jiagoushi.top

JS:   while (i < 10) { i++; }
来源：http://esw.yj20258.top

TS:   while (i < 10) { i++; }
来源：http://yaz.fehbvm.com

Java: while (i < 10) { i++; }
来源：http://dvy.mhx1999.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ozz.gaohongyu789.top

Ruby: while i < 10; i += 1; end
来源：http://fbs.dashuyun.cn

C#:   while (i < 10) { i++; }
来源：http://xzk.zycfv.cn

[B08] do-while（至少执行一次）
来源：http://yfj.bbcook.cn

Py:   # 无 do-while：用 while True + break
来源：http://jvh.daxiang520.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kqs.yanxiufei.cn

JS:   do { i++; } while (i < 10);
来源：http://pxl.yvedp.cn

TS:   do { i++; } while (i < 10);
来源：http://yoq.cheryme.top

Java: do { i++; } while (i < 10);
来源：http://fbb.ybcxt.top

Go:   for { i++; if i >= 10 { break } }
来源：http://lar.cqqwz.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yuz.316326.xyz

C#:   do { i++; } while (i < 10);
来源：http://eks.bbcook.cn

[B09] break 与 continue
来源：http://lll.jinqigufen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ibu.yvedp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jki.epnwcf.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iip.316326.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mfx.tianlin.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bmk.shuidangran.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ayp.cdnleiting.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fdb.mhx1999.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ymh.cashguo.top

[B10] 遍历同时拿索引
来源：http://fgd.cheryme.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rht.yangfankeji.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dxu.jinqigfzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uod.wangshuangyany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://syq.sxryk.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xsd.sxryk.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://okr.daria6918.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eqt.yj20258888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zcs.xylfe.cn

[B11] 生成数字序列 / 区间
来源：http://nae.jinqigufen.top

Py:   list(range(0, 10, 2))
来源：http://mnz.fehbvm.com

PHP:  range(0, 10, 2);
来源：http://hsd.xuanzx.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xum.fanxiaobao.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cuu.c1oappe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wwe.fktsv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uvb.yanxiufei.cn

Ruby: (0...10).step(2).to_a
来源：http://fsp.jinqigfzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rfr.yongpay.top

[B12] 跳出多层循环
来源：http://rtm.fengsongda.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://jlb.haohaochexian.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lou.epnwcf.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tfk.zhiwuduotai.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aak.yuxming.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qye.guannengcc.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cve.fktsv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aas.ybcxt.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rxf.uphjek.com

[B13] 判断是否为数字
来源：http://jxp.jyoumei.cn

Py:   isinstance(x, (int, float))
来源：http://rsg.tarul.cn

PHP:  is_numeric($x)
来源：http://yek.xylfe.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zkc.hongshengwenyu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nts.gaohongyu789.top

Java: x instanceof Number
来源：http://ruv.52xcode.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zmy.zhijiandao.cn

Ruby: x.is_a?(Numeric)
来源：http://kot.uphjek.com

C#:   x is int or double or decimal
来源：http://tvg.yueranfly.top

[B14] 判断值是否在集合内
来源：http://vkc.yvedp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://slb.xylfe.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tyc.zdbjq.cn

JS:   [1, 2, 3].includes(x)
来源：http://myc.haohaochexian.top

TS:   [1, 2, 3].includes(x)
来源：http://yss.jinqigfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://twp.sweek.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pqi.jinqigufen.top

Ruby: [1, 2, 3].include?(x)
来源：http://iim.uphjek.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jrm.chenzaomai.com

[B15] 布尔运算与取反
来源：http://kvg.shanyushiyangtech.top

Py:   a and b or not c
来源：http://eaa.daxiang520.top

PHP:  $a && $b || !$c
来源：http://raf.ywan-chungtsiang.top

JS:   a && b || !c
来源：http://cfd.yanxiufei.cn

TS:   a && b || !c
来源：http://rbc.daxiang520.top

Java: a && b || !c
来源：http://nnr.vehdjk.com

Go:   a && b || !c
来源：http://emc.ydzc1.top

Ruby: a && b || !c
来源：http://fks.ppjwa.cn

C#:   a && b || !c
来源：http://chm.zhongyouzk.top

[B16] 卫语句：不满足条件提前返回
来源：http://scl.bbcook.cn

Py:   if not data: return
来源：http://doz.ydjk.org.cn

PHP:  if (!$data) { return; }
来源：http://xdd.xinyue.icu

JS:   if (!data) return;
来源：http://iro.0kj1m.cn

TS:   if (!data) return;
来源：http://gxj.meibo888.top

Java: if (data == null) return;
来源：http://qij.316326.xyz

Go:   if data == nil { return }
来源：http://gbk.zycfv.cn

Ruby: return if data.nil?
来源：http://aql.epnwcf.com

C#:   if (data == null) return;
来源：http://pst.sufxvd.cn

================================================================================
来源：http://tzv.shanyushiyangkeji.top

C. 函数与作用域
来源：http://kfw.sxryk.cn

================================================================================
来源：http://tmn.yj20258.top

[C01] 定义函数
来源：http://moq.ywan-chungtsiang.top

Py:   def add(a, b): return a + b
来源：http://sai.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sma.shuidangran.top

JS:   function add(a, b) { return a + b; }
来源：http://ecl.fehbvm.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://urh.xziqi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://buz.tianlin.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://heg.fehbvm.com

Ruby: def add(a, b); a + b; end
来源：http://tqx.cashguo.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tcf.yonumen.top

[C02] 默认参数
来源：http://djv.fanxiaobao.xyz

Py:   def greet(name="World"): return name
来源：http://ehl.yvedp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://aje.hfpthk.cn

JS:   function greet(name = "World") { return name; }
来源：http://mdw.ywan-chungtsiang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://qmz.jianghu66.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tjz.uphjek.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qpe.ctjpmb.com

Ruby: def greet(name = "World") = name
来源：http://wig.0kj1m.cn

C#:   string Greet(string name = "World") => name;
来源：http://lft.tianlin.xyz

[C03] 可变参数
来源：http://uhj.daria6918.cn

Py:   def total(*args): return sum(args)
来源：http://cxe.sxryk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ybc.iojbl.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jqx.bjfxy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uqs.kuanghao11.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xif.xylfe.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ets.guowangkeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://hmr.chenzaomai.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dov.aizwys.cn

[C04] 命名参数 / 关键字参数
来源：http://qcs.jlsjyb.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sdt.bbcook.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qge.sjlbkw.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ghk.nanxinkj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vyi.zhaomingkeji.xyz

Java: // 无：用 Builder 模式或 record
来源：http://pwv.aizwys.cn

Go:   // 无：用配置结构体参数
来源：http://wyh.gotoacloud.top

Ruby: f(a: 1, b: 2)
来源：http://pio.fktsv.cn

C#:   f(a: 1, b: 2)
来源：http://oha.nwbrower.top

[C05] 返回多个值
来源：http://mct.hfpthk.cn

Py:   return a, b
来源：http://jqr.cucudq.cn

PHP:  return [$a, $b];
来源：http://rmr.jinyuanbaomall.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hwb.aizwys.cn

TS:   return { a, b };
来源：http://pcy.pengpengdd.cyou

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ues.sufxvd.cn

Go:   return a, b
来源：http://pqs.hysaishi.cn

Ruby: return a, b
来源：http://zgh.yangfankeji.com

C#:   return (a, b);              // ValueTuple
来源：http://aea.xuanzx.com

[C06] 匿名函数 / lambda
来源：http://lbq.yueranfly.top

Py:   square = lambda x: x * x
来源：http://iwr.xuetiantiany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://omz.hfpthk.cn

JS:   const square = x => x * x;
来源：http://cdy.yuanzhike.top

TS:   const square = (x: number): number => x * x;
来源：http://wvb.hfpthk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tca.aibaodan.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vec.aibaodan.cn

Ruby: square = ->(x) { x * x }
来源：http://xbj.ctjpmb.com


<!-- 参考信息 -->