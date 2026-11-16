代发 wailian999

C#:   s.Length
来源：http://lux.chenlongwang.top

[A23] 大小写转换
来源：http://tir.yj202588.top

Py:   s.upper(); s.lower(); s.title()
来源：http://afl.kuanghao11.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ypc.gogol.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://osy.yuxming.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bkk.birdmap.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tsn.wangshuangyany.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://eqh.yj20258888.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hmd.fktsv.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wdr.sweek.top

[A24] 去除首尾空白
来源：http://sys.kuanghao11.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zpp.shangyingyoupin.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fgo.dianchejie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rmg.zhixingplan.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uca.ybcxt.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://atn.ppjwa.cn

Go:   strings.TrimSpace(s)
来源：http://dyi.wangshuangyany.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gjb.zhijiandao.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vee.cheryme.top

[A25] 字符串比较
来源：http://adw.zhongyouzk.top

Py:   s1 == s2; s1 != s2
来源：http://dsn.jqgfzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ggq.cashguo.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cmj.hywenlv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wea.haohaochexian.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mam.xylfe.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://htc.yj202588.top

Ruby: s1 == s2; s1 <=> s2
来源：http://lll.cucudq.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rmm.ybcxt.top

[A26] 类型转换总览
来源：http://xnx.yvedp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gav.zdqjudy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ijq.shanyushiyangkeji.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cho.52xcode.cn

TS:   Number() String() Boolean() x as number
来源：http://vtl.yfazqb.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ugf.jianghu66.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nlt.cucudq.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wvc.tarul.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gri.shangyingyoupin.top

================================================================================
来源：http://fxd.yj202588.top

B. 流程控制
来源：http://ssq.hysaishi.cn

================================================================================
来源：http://qut.pycfn.com

[B01] 条件判断 if / else
来源：http://yzq.andypj.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://bzf.fktsv.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ywf.fzhhl.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qbu.yanxiufei.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ruf.hywenlv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qqq.zhoulong.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jjf.fktsv.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xwk.daria6918.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://scq.ppjwa.cn

[B02] 多分支 else if / elif
来源：http://bnq.gzhubu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fbs.quarkkingdee.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gtt.jinghuilouyu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bge.gaohongyu789.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rpa.yonumen.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bcd.shuidangran.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zrj.pengpengdd.cyou

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ryw.jyoumei.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pxd.shanyushiyangkeji.top

[B03] switch / match / case
来源：http://rgi.cqqwz.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cps.bjfxy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ake.wangdashe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yox.fktsv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zcp.daria6918.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nyo.jlsjyb.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fff.yj20258888.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://odx.uphjek.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pzz.redwolf501.top

[B04] for 计数循环
来源：http://xsp.ivvv.top

Py:   for i in range(10): print(i)
来源：http://rzn.havefunace.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zan.jinqigufen.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iqd.wangdashe.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://odc.zhaomingkeji.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ynx.shanyushiyangkeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hay.meibo888.top

Ruby: 10.times { |i| puts i }
来源：http://rxx.jyoumei.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://udp.hongshengwenyu.top

[B05] 遍历数组 / 列表
来源：http://jsl.birdmap.top

Py:   for item in arr: print(item)
来源：http://gmq.jinqigufen.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qsl.feifeiyinyue.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vko.daxiang520.top

TS:   for (const item of arr) { console.log(item); }
来源：http://snv.chenlongwang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://txw.hywenlv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://can.jqgfzy.top

Ruby: arr.each { |item| puts item }
来源：http://egy.tianlin.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ivc.jyoumei.cn

[B06] 遍历字典 / 对象
来源：http://nnr.nwbrower.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ecr.zhiwuduotai.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kdu.jinyuanbaomall.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dvv.yongpay.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wxy.yj20258888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ruq.ivvv.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rek.ydjk.org.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qmj.daria6918.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vqe.zhiwuduotai.top

[B07] while 循环
来源：http://tzv.zhaomingkeji.xyz

Py:   while i < 10: i += 1
来源：http://ojp.ppjwa.cn

PHP:  while ($i < 10) { $i++; }
来源：http://djg.tarul.cn

JS:   while (i < 10) { i++; }
来源：http://lpg.zhoulong.xyz

TS:   while (i < 10) { i++; }
来源：http://sbw.yj20258.top

Java: while (i < 10) { i++; }
来源：http://boo.jinghuilouyu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hdb.sweek.top

Ruby: while i < 10; i += 1; end
来源：http://jaw.sjlbkw.cn

C#:   while (i < 10) { i++; }
来源：http://bzl.bjfxy.top

[B08] do-while（至少执行一次）
来源：http://jun.shangyingyoupin.top

Py:   # 无 do-while：用 while True + break
来源：http://ygl.chenzaomai.com

PHP:  do { $i++; } while ($i < 10);
来源：http://aam.iojbl.cn

JS:   do { i++; } while (i < 10);
来源：http://clg.sweek.top

TS:   do { i++; } while (i < 10);
来源：http://hsw.pengpengdd.cyou

Java: do { i++; } while (i < 10);
来源：http://omc.chenzaomai.com

Go:   for { i++; if i >= 10 { break } }
来源：http://juf.yuxming.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rbs.uphjek.com

C#:   do { i++; } while (i < 10);
来源：http://utl.gaohongyu789.top

[B09] break 与 continue
来源：http://jhe.smart0.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://txv.birdmap.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gtn.yueranfly.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eoq.xylfe.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ddk.guowangkeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fbc.mhx1999.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uwp.jianghu66.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vzf.sjlbkw.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://syh.gaohongyu789.top

[B10] 遍历同时拿索引
来源：http://xyy.guowangkeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ewh.hnqzz.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pnt.shanyushiyangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wuv.haohaochexian.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hgn.yonumen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wgx.hnqzz.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vmx.ybcxt.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://byr.bbcook.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://djd.fktsv.cn

[B11] 生成数字序列 / 区间
来源：http://orw.hesvh.cn

Py:   list(range(0, 10, 2))
来源：http://ygb.feifeiyinyue.top

PHP:  range(0, 10, 2);
来源：http://ngh.gotoacloud.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rjm.smart0.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tfo.xingfuxueyuan.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://emt.yanxiufei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://egs.zhixingplan.top

Ruby: (0...10).step(2).to_a
来源：http://krv.cucudq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zse.chenlongwang.top

[B12] 跳出多层循环
来源：http://cws.ywan-chungtsiang.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://pnf.xingfuxueyuan.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://gxb.cqqwz.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pyl.shangyingyoupin.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lbf.wangdashe.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bge.vehdjk.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://exk.yfazqb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zew.yj20258.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://svf.yj202588.top

[B13] 判断是否为数字
来源：http://wwt.hcnkem.com

Py:   isinstance(x, (int, float))
来源：http://eic.fengsongda.top

PHP:  is_numeric($x)
来源：http://oim.hesvh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ypt.c1oappe.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://peh.gogol.net.cn

Java: x instanceof Number
来源：http://ovk.zhixingplan.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jlb.jinyuanbaomall.cn

Ruby: x.is_a?(Numeric)
来源：http://yxh.zhixingplan.top

C#:   x is int or double or decimal
来源：http://pwx.jlsjyb.cn

[B14] 判断值是否在集合内
来源：http://avy.jianghu66.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qog.52xcode.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://umc.vehdjk.com

JS:   [1, 2, 3].includes(x)
来源：http://fwd.0kj1m.cn

TS:   [1, 2, 3].includes(x)
来源：http://djj.tanke756.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pya.zhengqikj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://egg.fktsv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tlx.zdqjudy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ueo.yongpay.top

[B15] 布尔运算与取反
来源：http://taq.shzxlz.cn

Py:   a and b or not c
来源：http://ykx.jyoumei.cn

PHP:  $a && $b || !$c
来源：http://mdv.yangfankeji.com

JS:   a && b || !c
来源：http://udg.haohaochexian.top

TS:   a && b || !c
来源：http://nwh.daxiang520.top

Java: a && b || !c
来源：http://kyx.shanyushiyangtech.top

Go:   a && b || !c
来源：http://xlh.jinghuilouyu.cn

Ruby: a && b || !c
来源：http://ydu.yuanzhike.top

C#:   a && b || !c
来源：http://uxp.316326.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://ibl.jinqigfzy.top

Py:   if not data: return
来源：http://nwq.shzxlz.cn

PHP:  if (!$data) { return; }
来源：http://ild.jlsjyb.cn

JS:   if (!data) return;
来源：http://sjw.aibaodan.cn

TS:   if (!data) return;
来源：http://oqf.zdbjq.cn

Java: if (data == null) return;
来源：http://vsq.hnqzz.top

Go:   if data == nil { return }
来源：http://myi.sysykeji.top

Ruby: return if data.nil?
来源：http://nwe.sxryk.cn

C#:   if (data == null) return;
来源：http://nvw.hesvh.cn

================================================================================
来源：http://efv.zycfv.cn

C. 函数与作用域
来源：http://tjj.fktsv.cn

================================================================================
来源：http://ghj.zhongyouzk.top

[C01] 定义函数
来源：http://kni.zhongyouzk.top

Py:   def add(a, b): return a + b
来源：http://nrw.havefunace.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://azk.shuidangran.top

JS:   function add(a, b) { return a + b; }
来源：http://lcm.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ufs.yanxiufei.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xxi.hcnkem.com

Go:   func add(a, b int) int { return a + b }
来源：http://aje.epnwcf.com

Ruby: def add(a, b); a + b; end
来源：http://egh.yj202588.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ptl.tian-w.cn

[C02] 默认参数
来源：http://ohp.guannengcc.top

Py:   def greet(name="World"): return name
来源：http://osk.yanxiufei.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jdx.guannengcc.top

JS:   function greet(name = "World") { return name; }
来源：http://yqn.shuidangran.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ujl.yj202588.top

Java: // 无默认参数：方法重载或 Optional
来源：http://hxf.gaohongyu789.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://onh.yfazqb.com

Ruby: def greet(name = "World") = name
来源：http://ixc.smart0.xyz

C#:   string Greet(string name = "World") => name;
来源：http://ivj.wangshuangyany.cn

[C03] 可变参数
来源：http://xcs.xziqi.cn

Py:   def total(*args): return sum(args)
来源：http://lzw.gzhubu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://evl.iojbl.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mkg.snrcjt.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hat.kuanghao11.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xsm.chenzaomai.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kqk.fktsv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tqb.yanxiufei.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gqt.wangdashe.top

[C04] 命名参数 / 关键字参数
来源：http://lte.gzhubu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://doh.nanxuanxn.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rfq.cheryme.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xzy.fehbvm.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://czg.shangyingyoupin.top

Java: // 无：用 Builder 模式或 record
来源：http://wxk.hcnkem.com

Go:   // 无：用配置结构体参数
来源：http://cvs.hnxiangtu.top

Ruby: f(a: 1, b: 2)
来源：http://uth.zhengqikj.top

C#:   f(a: 1, b: 2)
来源：http://hqj.xziqi.cn

[C05] 返回多个值
来源：http://xxe.yj202588.top

Py:   return a, b
来源：http://huu.uphjek.com

PHP:  return [$a, $b];
来源：http://xff.hammf.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hlk.yanxiufei.cn

TS:   return { a, b };
来源：http://zjx.vehdjk.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lhs.shanyushiyangtech.top

Go:   return a, b
来源：http://ohc.cucudq.cn

Ruby: return a, b
来源：http://fld.yuxming.cn

C#:   return (a, b);              // ValueTuple
来源：http://niv.jyoumei.cn

[C06] 匿名函数 / lambda
来源：http://zev.zdqjudy.top

Py:   square = lambda x: x * x
来源：http://cck.zhengqikj.top

PHP:  $square = fn($x) => $x * $x;
来源：http://log.vqdsnc.cn

JS:   const square = x => x * x;
来源：http://zuc.sysykeji.top

TS:   const square = (x: number): number => x * x;
来源：http://gqp.andypj.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mbv.hcnkem.com

Go:   sq := func(x int) int { return x * x }
来源：http://spb.c1oappe.top

Ruby: square = ->(x) { x * x }
来源：http://cxe.xziqi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://iqn.xingfuxueyuan.xyz

[C07] 把函数作为参数传入
来源：http://axj.hongshengwenyu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kgo.bjfxy.top

PHP:  array_map("strtoupper", $arr);
来源：http://lks.xingfuxueyuan.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oam.dianchejie.cn

TS:   arr.map(String)
来源：http://lcu.pengpengdd.cyou

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yrk.nanxuanxn.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ljx.zhijiandao.cn

Ruby: arr.map(&:upcase)
来源：http://pyj.smart0.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://rhy.shzxlz.cn

[C08] 闭包
来源：http://exo.shuidangran.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kkt.jianghu66.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bcr.ydjk.org.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hgj.shuidangran.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kxu.kuanghao11.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uog.nanxinkj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xud.fktsv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hpo.yanxiufei.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mum.yuanzhike.top

[C09] 递归
来源：http://yoq.hysaishi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ets.shangyingyoupin.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mqu.cdnleiting.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://izy.guannengcc.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wgr.aizwys.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jsu.jinqigufen.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mvy.xinyue.icu

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nnr.aizwys.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yea.shangyingyoupin.top

[C10] 变量作用域
来源：http://jhz.316326.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jvm.zhoulong.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://deo.hesvh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vax.tian-w.cn

TS:   同 JS
来源：http://non.yj202588.top

Java: 方法内为块级作用域
来源：http://xdb.ydjk.org.cn

Go:   花括号块级作用域
来源：http://bye.ybcxt.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bmi.pengpengdd.cyou

C#:   块级作用域
来源：http://elt.zdqjudy.top

[C11] 模块导入与导出
来源：http://nfq.ydzc1.top

Py:   from module import func
来源：http://grq.guannengcc.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ewz.iojbl.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mfc.jinqigfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://efv.52xcode.cn

Java: import java.util.List;
来源：http://jjo.haohaochexian.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cdy.zycfv.cn

Ruby: require "json"; require_relative "./util"
来源：http://olm.hnqzz.top

C#:   using System.Text;
来源：http://ial.sxryk.cn

[C12] 立即执行函数 IIFE
来源：http://jal.xuetiantiany.cn

Py:   (lambda: print("run"))()
来源：http://jxt.tian-w.cn

PHP:  (function () { echo "run"; })();
来源：http://eur.bbcook.cn

JS:   (() => { console.log("run"); })();
来源：http://qsf.xziqi.cn

TS:   (() => { console.log("run"); })();
来源：http://fik.fengsongda.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uqr.pengpengdd.cyou

Go:   func() { fmt.Println("run") }()
来源：http://zzg.aizwys.cn

Ruby: -> { puts "run" }.call
来源：http://tbf.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://sng.tarul.cn

[C13] 类型声明 / 类型注解
来源：http://dow.tanke756.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dbc.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://asr.jianghu66.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://snc.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hvc.jinghuilouyu.cn


<!-- 参考信息 -->