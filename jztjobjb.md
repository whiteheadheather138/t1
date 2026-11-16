代发 wailian999

C#:   s.Length
来源：http://vpx.fanxiaobao.xyz

[A23] 大小写转换
来源：http://nog.pengpengdd.cyou

Py:   s.upper(); s.lower(); s.title()
来源：http://vgm.guowangkeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yzs.jqgufenzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://onh.c1oappe.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://div.hongshengwenyu.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://iyn.shanyushiyangkeji.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zir.tianlin.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://eim.yj20258.top

C#:   s.ToUpper(); s.ToLower()
来源：http://anr.chenlongwang.top

[A24] 去除首尾空白
来源：http://ltl.guowangkeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bla.yuxming.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://edj.chenlongwang.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sjn.feifeiyinyue.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rrh.ydjk.org.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://aon.xuetiantiany.cn

Go:   strings.TrimSpace(s)
来源：http://erd.cucudq.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bcs.zycfv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jjx.zhengqikj.top

[A25] 字符串比较
来源：http://lnt.dashuyun.cn

Py:   s1 == s2; s1 != s2
来源：http://ecw.gaohongyu789.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wqu.hammf.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dur.fzhhl.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qmn.gaohongyu789.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mwy.yj202588.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ehx.jlsjyb.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tir.xinyue.icu

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://aci.ydzc1.top

[A26] 类型转换总览
来源：http://hig.yuxming.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ouz.ivvv.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://moc.vehdjk.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mfj.52xcode.cn

TS:   Number() String() Boolean() x as number
来源：http://njn.vqdsnc.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://idf.xingfuxueyuan.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hlr.zdbjq.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tli.sysykeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vsw.nanxuanxn.top

================================================================================
来源：http://gzu.ywan-chungtsiang.top

B. 流程控制
来源：http://dsk.tian-w.cn

================================================================================
来源：http://tog.yangfankeji.com

[B01] 条件判断 if / else
来源：http://gwd.zycfv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://upr.xinyue.icu

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qxv.jinqigfzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zqw.ctjpmb.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dia.jlsjyb.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://eci.0kj1m.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jeh.fehbvm.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kqv.xinyue.icu

C#:   var r = x > 0 ? "正" : "非正";
来源：http://koq.jianghu66.top

[B02] 多分支 else if / elif
来源：http://zhs.kuanghao11.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rnw.gotoacloud.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bvv.tarul.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://axd.xinyue.icu

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xgl.fktsv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cjp.sjlbkw.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vlx.hysaishi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nql.tarul.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://idh.yfazqb.com

[B03] switch / match / case
来源：http://rgm.gaohongyu789.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mtg.jinqigufen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ekx.52xcode.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tcd.jqgufenzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vjo.sufxvd.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ivv.wangdashe.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hnd.vqdsnc.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fmy.shanyushiyangtech.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hcn.gogol.net.cn

[B04] for 计数循环
来源：http://kbg.ppjwa.cn

Py:   for i in range(10): print(i)
来源：http://vzs.ivvv.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lvz.daxiang520.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bob.yanxiufei.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zcd.aibaodan.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ugr.yj20258888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bne.ywan-chungtsiang.top

Ruby: 10.times { |i| puts i }
来源：http://mhh.zhijiandao.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://idc.ydjk.org.cn

[B05] 遍历数组 / 列表
来源：http://wkk.dianchejie.cn

Py:   for item in arr: print(item)
来源：http://pko.snrcjt.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tpr.tarul.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://iqn.daria6918.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yjw.shuidangran.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jrj.fehbvm.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xmr.jinqigufen.top

Ruby: arr.each { |item| puts item }
来源：http://nyn.hfpthk.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ked.daria6918.cn

[B06] 遍历字典 / 对象
来源：http://mpy.yangfankeji.com

Py:   for k, v in d.items(): print(k, v)
来源：http://nnn.xuanzx.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://umy.kuanghao11.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oic.hammf.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zte.hongshengwenyu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tyw.zhaomingkeji.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tjv.bjfxy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dwz.jinqigufen.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://roq.tarul.cn

[B07] while 循环
来源：http://lwh.hesvh.cn

Py:   while i < 10: i += 1
来源：http://chh.hysaishi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://elg.chenlongwang.top

JS:   while (i < 10) { i++; }
来源：http://dcz.yuxming.cn

TS:   while (i < 10) { i++; }
来源：http://ybt.hesvh.cn

Java: while (i < 10) { i++; }
来源：http://mbj.zdqjudy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vzj.ywan-chungtsiang.top

Ruby: while i < 10; i += 1; end
来源：http://ulx.zdqjudy.top

C#:   while (i < 10) { i++; }
来源：http://hcd.hfpthk.cn

[B08] do-while（至少执行一次）
来源：http://til.zdqjudy.top

Py:   # 无 do-while：用 while True + break
来源：http://idu.tanke756.top

PHP:  do { $i++; } while ($i < 10);
来源：http://iwe.yanxiufei.cn

JS:   do { i++; } while (i < 10);
来源：http://yrz.yanxiufei.cn

TS:   do { i++; } while (i < 10);
来源：http://udh.zhengqikj.top

Java: do { i++; } while (i < 10);
来源：http://jnc.xingfuxueyuan.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://run.xinyue.icu

Ruby: begin; i += 1; end while i < 10
来源：http://mxz.cdnleiting.top

C#:   do { i++; } while (i < 10);
来源：http://sen.gotoacloud.top

[B09] break 与 continue
来源：http://lgx.zycfv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jox.gzhubu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nfi.birdmap.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xkj.nanxuanxn.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vof.shanyushiyangkeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vrg.jinyuanbaomall.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wcv.xylfe.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dnn.zdqjudy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tdt.shuidangran.top

[B10] 遍历同时拿索引
来源：http://lje.shanyushiyangtech.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://crk.gzhubu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nbo.smart0.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://utr.fktsv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rny.fehbvm.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://upc.fehbvm.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nar.uphjek.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hta.yfazqb.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wef.yvedp.cn

[B11] 生成数字序列 / 区间
来源：http://teo.ydjk.org.cn

Py:   list(range(0, 10, 2))
来源：http://wjs.fktsv.cn

PHP:  range(0, 10, 2);
来源：http://ala.shuidangran.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pok.xinyue.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pil.shzxlz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://azf.feifeiyinyue.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tlx.xinyue.icu

Ruby: (0...10).step(2).to_a
来源：http://mpn.ybcxt.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hmt.vehdjk.com

[B12] 跳出多层循环
来源：http://lom.zhixingplan.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://due.shuidangran.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://rfc.wangshuangyany.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pft.sxryk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lvt.xinyue.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mmh.chenzaomai.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pcz.zhixingplan.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qsd.aizwys.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vsd.hysaishi.cn

[B13] 判断是否为数字
来源：http://acr.hysaishi.cn

Py:   isinstance(x, (int, float))
来源：http://qwb.daxiang520.top

PHP:  is_numeric($x)
来源：http://lzq.sufxvd.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://avf.hfpthk.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sbw.wangdashe.top

Java: x instanceof Number
来源：http://kxc.tanke756.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hzi.ppjwa.cn

Ruby: x.is_a?(Numeric)
来源：http://iwt.guannengcc.top

C#:   x is int or double or decimal
来源：http://xad.wangdashe.top

[B14] 判断值是否在集合内
来源：http://tmp.shzxlz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ycm.wangshuangyany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vic.redwolf501.top

JS:   [1, 2, 3].includes(x)
来源：http://vgn.xinyue.icu

TS:   [1, 2, 3].includes(x)
来源：http://hix.nwbrower.top

Java: List.of(1, 2, 3).contains(x)
来源：http://qvk.tianlin.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ybu.hammf.cn

Ruby: [1, 2, 3].include?(x)
来源：http://djz.ybcxt.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xmn.epnwcf.com

[B15] 布尔运算与取反
来源：http://zyy.xylfe.cn

Py:   a and b or not c
来源：http://gpm.jiagoushi.top

PHP:  $a && $b || !$c
来源：http://zrv.cdnleiting.top

JS:   a && b || !c
来源：http://suz.shuidangran.top

TS:   a && b || !c
来源：http://nym.gotoacloud.top

Java: a && b || !c
来源：http://hfm.cashguo.top

Go:   a && b || !c
来源：http://vwn.jyoumei.cn

Ruby: a && b || !c
来源：http://bvp.dianchejie.cn

C#:   a && b || !c
来源：http://oxs.jinyuanbaomall.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wmf.nanxinkj.top

Py:   if not data: return
来源：http://fem.redwolf501.top

PHP:  if (!$data) { return; }
来源：http://amm.sufxvd.cn

JS:   if (!data) return;
来源：http://jwd.andypj.xyz

TS:   if (!data) return;
来源：http://lwv.yanxiufei.cn

Java: if (data == null) return;
来源：http://kag.chenzaomai.com

Go:   if data == nil { return }
来源：http://gsl.nanxuanxn.top

Ruby: return if data.nil?
来源：http://uiu.meibo888.top

C#:   if (data == null) return;
来源：http://nby.gaohongyu789.top

================================================================================
来源：http://ipc.tarul.cn

C. 函数与作用域
来源：http://nrv.sxryk.cn

================================================================================
来源：http://bls.zhaomingkeji.xyz

[C01] 定义函数
来源：http://wqs.epnwcf.com

Py:   def add(a, b): return a + b
来源：http://olm.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wgj.smart0.xyz

JS:   function add(a, b) { return a + b; }
来源：http://agq.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dly.cashguo.top

Java: static int add(int a, int b) { return a + b; }
来源：http://njc.wangdashe.top

Go:   func add(a, b int) int { return a + b }
来源：http://rzi.yfazqb.com

Ruby: def add(a, b); a + b; end
来源：http://vop.cdnleiting.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ukb.ydzc1.top

[C02] 默认参数
来源：http://xbw.xuetiantiany.cn

Py:   def greet(name="World"): return name
来源：http://iws.shzxlz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lav.zhijiandao.cn

JS:   function greet(name = "World") { return name; }
来源：http://yhg.ybcxt.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ruh.bbcook.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ags.xuanzx.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://obs.jinghuilouyu.cn

Ruby: def greet(name = "World") = name
来源：http://bnn.c1oappe.top

C#:   string Greet(string name = "World") => name;
来源：http://hjd.yonumen.top

[C03] 可变参数
来源：http://cah.mhx1999.top

Py:   def total(*args): return sum(args)
来源：http://mpk.yj202588.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mpf.wangshuangyany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xkk.yuxming.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rri.yongpay.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ilf.cucudq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cjp.bjfxy.top

Ruby: def total(*nums); nums.sum; end
来源：http://pte.hcnkem.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://beg.cashguo.top

[C04] 命名参数 / 关键字参数
来源：http://dzp.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qeq.jinqigfzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vfx.cashguo.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vsi.bjfxy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jxi.redwolf501.top

Java: // 无：用 Builder 模式或 record
来源：http://uov.jqgfzy.top

Go:   // 无：用配置结构体参数
来源：http://mqw.zhijiandao.cn

Ruby: f(a: 1, b: 2)
来源：http://koe.sufxvd.cn

C#:   f(a: 1, b: 2)
来源：http://ziw.zhixingplan.top

[C05] 返回多个值
来源：http://lng.meibo888.top

Py:   return a, b
来源：http://kox.feifeiyinyue.top

PHP:  return [$a, $b];
来源：http://lut.xuetiantiany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sfn.zhengqikj.top

TS:   return { a, b };
来源：http://bab.gaohongyu789.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://iwv.jqgufenzy.top

Go:   return a, b
来源：http://yvo.tianlin.xyz

Ruby: return a, b
来源：http://djd.hywenlv.cn

C#:   return (a, b);              // ValueTuple
来源：http://wel.gaohongyu789.top

[C06] 匿名函数 / lambda
来源：http://ikh.hnxiangtu.top

Py:   square = lambda x: x * x
来源：http://wjb.yvedp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://quu.jqgufenzy.top

JS:   const square = x => x * x;
来源：http://tqp.dashuyun.cn

TS:   const square = (x: number): number => x * x;
来源：http://zli.zycfv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qlm.ivvv.top

Go:   sq := func(x int) int { return x * x }
来源：http://ipq.zdqjudy.top

Ruby: square = ->(x) { x * x }
来源：http://puu.xingfuxueyuan.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://nou.gzhubu.top

[C07] 把函数作为参数传入
来源：http://fst.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ixl.ybcxt.top

PHP:  array_map("strtoupper", $arr);
来源：http://zjl.zhongyouzk.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sqj.cucudq.cn

TS:   arr.map(String)
来源：http://dfn.fzhhl.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xps.sxryk.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xzi.vqdsnc.cn

Ruby: arr.map(&:upcase)
来源：http://btd.nwbrower.top

C#:   arr.Select(s => s.ToUpper())
来源：http://huu.yuxming.cn

[C08] 闭包
来源：http://wkc.xuanzx.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hjy.sweek.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://agv.cheryme.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cek.jiagoushi.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vus.yvedp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kaa.gogol.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jnr.sufxvd.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://czk.yfazqb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pau.daria6918.cn

[C09] 递归
来源：http://hwl.jinqigfzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sob.xuetiantiany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ber.zhixingplan.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kcm.zhiwuduotai.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yzz.shuidangran.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kmg.fanxiaobao.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ipj.cheryme.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tsj.tarul.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sfa.hnqzz.top

[C10] 变量作用域
来源：http://nzc.xziqi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vpa.xuetiantiany.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rvv.zycfv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ycj.bjfxy.top

TS:   同 JS
来源：http://bpb.jinqigufen.top

Java: 方法内为块级作用域
来源：http://okc.sxryk.cn

Go:   花括号块级作用域
来源：http://cwg.gotoacloud.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://evl.c1oappe.top

C#:   块级作用域
来源：http://lpn.gaohongyu789.top

[C11] 模块导入与导出
来源：http://mkt.zhixingplan.top

Py:   from module import func
来源：http://ene.c1oappe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://tly.cucudq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://epr.hysaishi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ilu.tianlin.xyz

Java: import java.util.List;
来源：http://wkg.zhoulong.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://too.hesvh.cn

Ruby: require "json"; require_relative "./util"
来源：http://jaw.jqgfzy.top

C#:   using System.Text;
来源：http://auy.shanyushiyangtech.top

[C12] 立即执行函数 IIFE
来源：http://jrj.0kj1m.cn

Py:   (lambda: print("run"))()
来源：http://miq.yuxming.cn

PHP:  (function () { echo "run"; })();
来源：http://nfe.wangshuangyany.cn

JS:   (() => { console.log("run"); })();
来源：http://nam.hywenlv.cn

TS:   (() => { console.log("run"); })();
来源：http://gxj.yueranfly.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uhx.bjfxy.top

Go:   func() { fmt.Println("run") }()
来源：http://fet.tarul.cn

Ruby: -> { puts "run" }.call
来源：http://jyd.jqgfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ggm.gzhubu.top

[C13] 类型声明 / 类型注解
来源：http://elw.ybcxt.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ghk.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bbh.birdmap.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qmq.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vsn.zhiwuduotai.top


<!-- 参考信息 -->