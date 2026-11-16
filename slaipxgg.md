代发 wailian999

TS:   s.length
来源：http://xme.ppjwa.cn

Java: s.length()
来源：http://viv.ctjpmb.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hub.jqgfzy.top

Ruby: s.length
来源：http://imq.hfpthk.cn

C#:   s.Length
来源：http://xcq.kuanghao11.cn

[A23] 大小写转换
来源：http://sjk.yfazqb.com

Py:   s.upper(); s.lower(); s.title()
来源：http://joz.guannengcc.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hls.hongshengwenyu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://swu.nanxinkj.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fmt.jinqigfzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vqp.meibo888.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zcg.cdnleiting.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nhk.guannengcc.top

C#:   s.ToUpper(); s.ToLower()
来源：http://bjd.xuetiantiany.cn

[A24] 去除首尾空白
来源：http://uqj.yonumen.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tnj.xingfuxueyuan.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ypf.fktsv.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wsj.gotoacloud.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hkc.ybcxt.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sdi.jyoumei.cn

Go:   strings.TrimSpace(s)
来源：http://eaj.yvedp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gvw.yvedp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tvu.0kj1m.cn

[A25] 字符串比较
来源：http://kjh.jyoumei.cn

Py:   s1 == s2; s1 != s2
来源：http://fqp.jinqigufen.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://epe.chenzaomai.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dyf.yj20258888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xxe.yuxming.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pxn.jqgfzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tjn.guowangkeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://eol.jinqigfzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://igh.guowangkeji.top

[A26] 类型转换总览
来源：http://fak.yanxiufei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gxt.epnwcf.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dci.fehbvm.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rrf.xingfuxueyuan.xyz

TS:   Number() String() Boolean() x as number
来源：http://jss.xinyue.icu

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ypd.sufxvd.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ctj.hfpthk.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qri.xziqi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uzo.tianlin.xyz

================================================================================
来源：http://jfj.jlsjyb.cn

B. 流程控制
来源：http://jci.vehdjk.com

================================================================================
来源：http://sxx.zhoulong.xyz

[B01] 条件判断 if / else
来源：http://wzq.xingfuxueyuan.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://niz.ydzc1.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kbl.nanxinkj.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zrw.tarul.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nmw.ydzc1.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://noj.quarkkingdee.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://thi.hesvh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sqd.hysaishi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://njy.wangdashe.top

[B02] 多分支 else if / elif
来源：http://ppq.cdnleiting.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://obs.jlsjyb.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bdu.hfpthk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bic.shzxlz.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jde.hywenlv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ygy.snrcjt.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vcc.yonumen.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dfq.haohaochexian.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mvp.jianghu66.top

[B03] switch / match / case
来源：http://fqp.yangfankeji.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://caw.vqdsnc.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nis.shuidangran.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ike.guowangkeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ouh.gzhubu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ugg.gogol.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jlw.zhixingplan.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hfp.zhongyouzk.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://otb.iojbl.cn

[B04] for 计数循环
来源：http://hdi.cucudq.cn

Py:   for i in range(10): print(i)
来源：http://rmb.nanxuanxn.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dka.sweek.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hbb.guannengcc.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cwo.ppjwa.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nxk.zhiwuduotai.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://axw.hysaishi.cn

Ruby: 10.times { |i| puts i }
来源：http://oqw.ywan-chungtsiang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gxm.sxryk.cn

[B05] 遍历数组 / 列表
来源：http://inf.dianchejie.cn

Py:   for item in arr: print(item)
来源：http://ynp.hammf.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dff.ybcxt.top

JS:   for (const item of arr) { console.log(item); }
来源：http://trn.shangyingyoupin.top

TS:   for (const item of arr) { console.log(item); }
来源：http://kpq.pengpengdd.cyou

Java: for (var item : arr) { System.out.println(item); }
来源：http://eup.fanxiaobao.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ibw.ehwqpu.com

Ruby: arr.each { |item| puts item }
来源：http://qmn.epnwcf.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hqf.jinqigufen.top

[B06] 遍历字典 / 对象
来源：http://sue.yueranfly.top

Py:   for k, v in d.items(): print(k, v)
来源：http://oog.hongshengwenyu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tfy.xuetiantiany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://urt.sweek.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yvc.nanxuanxn.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bqf.uphjek.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pdr.jinyuanbaomall.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wsh.xingfuxueyuan.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://noj.wangdashe.top

[B07] while 循环
来源：http://apw.xziqi.cn

Py:   while i < 10: i += 1
来源：http://rxo.snrcjt.cn

PHP:  while ($i < 10) { $i++; }
来源：http://onj.tian-w.cn

JS:   while (i < 10) { i++; }
来源：http://pwz.yanxiufei.cn

TS:   while (i < 10) { i++; }
来源：http://hee.hcnkem.com

Java: while (i < 10) { i++; }
来源：http://orx.vqdsnc.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hlg.pengpengdd.cyou

Ruby: while i < 10; i += 1; end
来源：http://cua.aibaodan.cn

C#:   while (i < 10) { i++; }
来源：http://xhp.jinyuanbaomall.cn

[B08] do-while（至少执行一次）
来源：http://rhw.snrcjt.cn

Py:   # 无 do-while：用 while True + break
来源：http://cnq.iojbl.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wrb.kuanghao11.cn

JS:   do { i++; } while (i < 10);
来源：http://pqf.yuxming.cn

TS:   do { i++; } while (i < 10);
来源：http://jin.c1oappe.top

Java: do { i++; } while (i < 10);
来源：http://rzl.c1oappe.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ulz.xinyue.icu

Ruby: begin; i += 1; end while i < 10
来源：http://rpi.tarul.cn

C#:   do { i++; } while (i < 10);
来源：http://qii.chenzaomai.com

[B09] break 与 continue
来源：http://sjz.sweek.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rxi.shangyingyoupin.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rwc.zhoulong.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lhp.hcnkem.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ahw.hcnkem.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mke.redwolf501.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fpj.jianghu66.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sce.52xcode.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jdj.hcnkem.com

[B10] 遍历同时拿索引
来源：http://psb.birdmap.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vqv.zycfv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://now.xziqi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ubr.ppjwa.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pzk.yuxming.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ygw.52xcode.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bzi.nwbrower.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ndk.shanyushiyangkeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uqa.yuanzhike.top

[B11] 生成数字序列 / 区间
来源：http://hic.yvedp.cn

Py:   list(range(0, 10, 2))
来源：http://rpl.yonumen.top

PHP:  range(0, 10, 2);
来源：http://cpr.pycfn.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rgp.zdbjq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pyb.52xcode.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zuc.ydjk.org.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mns.havefunace.top

Ruby: (0...10).step(2).to_a
来源：http://mhc.snrcjt.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uaw.sxryk.cn

[B12] 跳出多层循环
来源：http://gbv.c1oappe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vla.cdnleiting.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ohh.hfpthk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kdw.feifeiyinyue.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kfv.xinyue.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yyk.smart0.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ucc.yj20258.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nug.jlsjyb.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vxq.yongpay.top

[B13] 判断是否为数字
来源：http://hcl.haohaochexian.top

Py:   isinstance(x, (int, float))
来源：http://eqd.uphjek.com

PHP:  is_numeric($x)
来源：http://vti.sufxvd.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://faj.zhongyouzk.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gjq.vehdjk.com

Java: x instanceof Number
来源：http://sfw.quarkkingdee.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ltx.dashuyun.cn

Ruby: x.is_a?(Numeric)
来源：http://lje.yuxming.cn

C#:   x is int or double or decimal
来源：http://gps.ctjpmb.com

[B14] 判断值是否在集合内
来源：http://hem.vqdsnc.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://svj.zhoulong.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rqh.sjlbkw.cn

JS:   [1, 2, 3].includes(x)
来源：http://ikv.aizwys.cn

TS:   [1, 2, 3].includes(x)
来源：http://rge.sxryk.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://muc.fehbvm.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gxc.nwbrower.top

Ruby: [1, 2, 3].include?(x)
来源：http://rtx.zhengqikj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wot.jlsjyb.cn

[B15] 布尔运算与取反
来源：http://gxu.0kj1m.cn

Py:   a and b or not c
来源：http://pzc.redwolf501.top

PHP:  $a && $b || !$c
来源：http://czw.wangshuangyany.cn

JS:   a && b || !c
来源：http://jph.dianchejie.cn

TS:   a && b || !c
来源：http://led.yuxming.cn

Java: a && b || !c
来源：http://ldq.zhaomingkeji.xyz

Go:   a && b || !c
来源：http://pay.aizwys.cn

Ruby: a && b || !c
来源：http://wvy.yuanzhike.top

C#:   a && b || !c
来源：http://zsw.zhongyouzk.top

[B16] 卫语句：不满足条件提前返回
来源：http://uce.yfazqb.com

Py:   if not data: return
来源：http://edu.chenzaomai.com

PHP:  if (!$data) { return; }
来源：http://lsv.fktsv.cn

JS:   if (!data) return;
来源：http://trc.dashuyun.cn

TS:   if (!data) return;
来源：http://cxc.shzxlz.cn

Java: if (data == null) return;
来源：http://ubs.meibo888.top

Go:   if data == nil { return }
来源：http://snx.pengpengdd.cyou

Ruby: return if data.nil?
来源：http://ktx.yueranfly.top

C#:   if (data == null) return;
来源：http://rwq.chenjidiqi.icu

================================================================================
来源：http://kbd.xinyue.icu

C. 函数与作用域
来源：http://ywe.zycfv.cn

================================================================================
来源：http://riw.fzhhl.top

[C01] 定义函数
来源：http://dro.redwolf501.top

Py:   def add(a, b): return a + b
来源：http://xfc.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vpw.chenzaomai.com

JS:   function add(a, b) { return a + b; }
来源：http://sid.fanxiaobao.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kls.shzxlz.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cwh.jqgfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://zkx.chenzaomai.com

Ruby: def add(a, b); a + b; end
来源：http://xwa.nanxuanxn.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rdl.hcnkem.com

[C02] 默认参数
来源：http://zkn.bbcook.cn

Py:   def greet(name="World"): return name
来源：http://kta.epnwcf.com

PHP:  function greet($name = "World") { return $name; }
来源：http://xci.shanyushiyangtech.top

JS:   function greet(name = "World") { return name; }
来源：http://ubc.zdbjq.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jte.sxryk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bje.fzhhl.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lvn.hfpthk.cn

Ruby: def greet(name = "World") = name
来源：http://xqb.chenjidiqi.icu

C#:   string Greet(string name = "World") => name;
来源：http://hmk.xziqi.cn

[C03] 可变参数
来源：http://dnm.nwbrower.top

Py:   def total(*args): return sum(args)
来源：http://etr.vqdsnc.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://koo.bjfxy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ymj.nwbrower.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nlf.svipenyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://flv.jinyuanbaomall.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ory.gzhubu.top

Ruby: def total(*nums); nums.sum; end
来源：http://czz.ydjk.org.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gpn.cqqwz.cn

[C04] 命名参数 / 关键字参数
来源：http://xlv.sysykeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://iwy.yonumen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nrt.yuxming.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ztv.zycfv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xkx.andypj.xyz

Java: // 无：用 Builder 模式或 record
来源：http://ctu.fktsv.cn

Go:   // 无：用配置结构体参数
来源：http://euk.ehwqpu.com

Ruby: f(a: 1, b: 2)
来源：http://ozm.hesvh.cn

C#:   f(a: 1, b: 2)
来源：http://lhn.sufxvd.cn

[C05] 返回多个值
来源：http://jft.hfpthk.cn

Py:   return a, b
来源：http://sgf.yuanzhike.top

PHP:  return [$a, $b];
来源：http://ewg.cdnleiting.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://nnt.fzhhl.top

TS:   return { a, b };
来源：http://ncj.sysykeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wtn.vqdsnc.cn

Go:   return a, b
来源：http://oga.tarul.cn

Ruby: return a, b
来源：http://jmy.sjlbkw.cn

C#:   return (a, b);              // ValueTuple
来源：http://mjr.pycfn.com

[C06] 匿名函数 / lambda
来源：http://vcs.yvedp.cn

Py:   square = lambda x: x * x
来源：http://mxu.pengpengdd.cyou

PHP:  $square = fn($x) => $x * $x;
来源：http://jpg.nanxuanxn.top

JS:   const square = x => x * x;
来源：http://khc.chenlongwang.top

TS:   const square = (x: number): number => x * x;
来源：http://vgq.cheryme.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fwk.gotoacloud.top

Go:   sq := func(x int) int { return x * x }
来源：http://dil.epnwcf.com

Ruby: square = ->(x) { x * x }
来源：http://jaf.ehwqpu.com

C#:   Func<int, int> square = x => x * x;
来源：http://xeh.hfpthk.cn

[C07] 把函数作为参数传入
来源：http://qrm.hnxiangtu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://aeg.zhiwuduotai.top

PHP:  array_map("strtoupper", $arr);
来源：http://edm.yj202588.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jos.zhongyouzk.top

TS:   arr.map(String)
来源：http://rhe.sweek.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lwz.ivvv.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rzr.kuanghao11.cn

Ruby: arr.map(&:upcase)
来源：http://urd.hcnkem.com

C#:   arr.Select(s => s.ToUpper())
来源：http://ufl.ybcxt.top

[C08] 闭包
来源：http://znz.shanyushiyangkeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ebs.ywan-chungtsiang.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mhz.tarul.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qlu.ehwqpu.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ozy.jinghuilouyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rzv.fzhhl.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cct.yj20258.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uwn.jinghuilouyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tzb.yueranfly.top

[C09] 递归
来源：http://hlw.jinqigfzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fsh.mhx1999.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ypn.0kj1m.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sqy.shanyushiyangtech.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fux.iojbl.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qva.316326.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qiu.sufxvd.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pma.yuxming.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xqi.chenlongwang.top

[C10] 变量作用域
来源：http://vtl.vqdsnc.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hvu.nanxinkj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vju.cucudq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://unc.chenjidiqi.icu

TS:   同 JS
来源：http://jnt.hesvh.cn

Java: 方法内为块级作用域
来源：http://kvf.xuetiantiany.cn

Go:   花括号块级作用域
来源：http://nia.shuidangran.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qty.jqgfzy.top

C#:   块级作用域
来源：http://rwo.zhixingplan.top

[C11] 模块导入与导出
来源：http://uao.yueranfly.top

Py:   from module import func
来源：http://xmj.ybcxt.top

PHP:  require "file.php";  或 use App\Service;
来源：http://gou.yj202588.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wmb.yuanzhike.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nnc.yj20258.top

Java: import java.util.List;
来源：http://eak.tian-w.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rzk.xuetiantiany.cn

Ruby: require "json"; require_relative "./util"
来源：http://abt.jianghu66.top

C#:   using System.Text;
来源：http://wuh.birdmap.top

[C12] 立即执行函数 IIFE
来源：http://hbx.gaohongyu789.top

Py:   (lambda: print("run"))()
来源：http://gdq.52xcode.cn

PHP:  (function () { echo "run"; })();
来源：http://kyn.xuetiantiany.cn

JS:   (() => { console.log("run"); })();
来源：http://hmz.daria6918.cn

TS:   (() => { console.log("run"); })();
来源：http://xbh.tarul.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pic.yongpay.top

Go:   func() { fmt.Println("run") }()
来源：http://fak.tanke756.top

Ruby: -> { puts "run" }.call
来源：http://nic.cqqwz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://olx.xylfe.cn

[C13] 类型声明 / 类型注解
来源：http://vzb.iojbl.cn


<!-- 参考信息 -->