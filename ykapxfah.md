代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fdi.xziqi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wnb.meibo888.top

[A24] 去除首尾空白
来源：http://tyq.nwbrower.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jvj.quarkkingdee.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://avi.jyoumei.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hpe.yuanzhike.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eas.guowangkeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://erj.jyoumei.cn

Go:   strings.TrimSpace(s)
来源：http://fcn.hnqzz.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dpm.hcnkem.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fem.sxryk.cn

[A25] 字符串比较
来源：http://jkl.yfazqb.com

Py:   s1 == s2; s1 != s2
来源：http://ojw.svipenyu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://utv.snrcjt.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://arl.zhaomingkeji.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hra.zhaomingkeji.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gqn.hfpthk.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qok.zhoulong.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://urd.fengsongda.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qxr.ehwqpu.com

[A26] 类型转换总览
来源：http://lsz.pengpengdd.cyou

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fiy.bbcook.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cyp.yj20258.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dsb.tarul.cn

TS:   Number() String() Boolean() x as number
来源：http://oxm.cdnleiting.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://omp.daria6918.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ijy.svipenyu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gje.guannengcc.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rmn.pycfn.com

================================================================================
来源：http://xcm.chenzaomai.com

B. 流程控制
来源：http://tyr.ydzc1.top

================================================================================
来源：http://ore.smart0.xyz

[B01] 条件判断 if / else
来源：http://ian.vehdjk.com

Py:   result = "正" if x > 0 else "非正"
来源：http://jtt.sweek.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rdr.dashuyun.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pjs.yuanzhike.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ovz.yfazqb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://flf.hammf.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qav.sjlbkw.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qwn.havefunace.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cnj.pengpengdd.cyou

[B02] 多分支 else if / elif
来源：http://nic.pycfn.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://phz.yvedp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yiy.vqdsnc.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://snq.wangshuangyany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dtz.chenlongwang.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lri.andypj.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ccs.sysykeji.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jnd.vehdjk.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yij.ybcxt.top

[B03] switch / match / case
来源：http://lvq.316326.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bqt.sxryk.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://evj.birdmap.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fje.daria6918.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qzr.birdmap.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nyq.ybcxt.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tmc.shanyushiyangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://aui.xylfe.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hsl.yonumen.top

[B04] for 计数循环
来源：http://ibw.yongpay.top

Py:   for i in range(10): print(i)
来源：http://oak.daxiang520.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zjp.gzhubu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bld.jinyuanbaomall.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jld.zhixingplan.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iph.ydjk.org.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gjw.jlsjyb.cn

Ruby: 10.times { |i| puts i }
来源：http://eic.uphjek.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vxb.snrcjt.cn

[B05] 遍历数组 / 列表
来源：http://nnr.fzhhl.top

Py:   for item in arr: print(item)
来源：http://qut.nanxuanxn.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qkc.hammf.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dpw.gzhubu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://cwp.hammf.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mcl.birdmap.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wuj.andypj.xyz

Ruby: arr.each { |item| puts item }
来源：http://kbn.hongshengwenyu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lon.mhx1999.top

[B06] 遍历字典 / 对象
来源：http://enx.quarkkingdee.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xdz.nwbrower.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dpr.gzhubu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dpy.wangdashe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hue.bjfxy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://khs.xuanzx.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://guj.birdmap.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mnl.jqgfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gve.guowangkeji.top

[B07] while 循环
来源：http://bvk.wangdashe.top

Py:   while i < 10: i += 1
来源：http://hre.yj202588.top

PHP:  while ($i < 10) { $i++; }
来源：http://cbj.hongshengwenyu.top

JS:   while (i < 10) { i++; }
来源：http://kvk.jinyuanbaomall.cn

TS:   while (i < 10) { i++; }
来源：http://fuh.jinyuanbaomall.cn

Java: while (i < 10) { i++; }
来源：http://nrq.vqdsnc.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rrl.jyoumei.cn

Ruby: while i < 10; i += 1; end
来源：http://zov.ywan-chungtsiang.top

C#:   while (i < 10) { i++; }
来源：http://gwe.yfazqb.com

[B08] do-while（至少执行一次）
来源：http://ffj.birdmap.top

Py:   # 无 do-while：用 while True + break
来源：http://rix.hfpthk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://iaz.sysykeji.top

JS:   do { i++; } while (i < 10);
来源：http://nwv.0kj1m.cn

TS:   do { i++; } while (i < 10);
来源：http://mrn.haohaochexian.top

Java: do { i++; } while (i < 10);
来源：http://vjs.zhixingplan.top

Go:   for { i++; if i >= 10 { break } }
来源：http://vhh.zhongyouzk.top

Ruby: begin; i += 1; end while i < 10
来源：http://djq.yj20258888.top

C#:   do { i++; } while (i < 10);
来源：http://xod.zhoulong.xyz

[B09] break 与 continue
来源：http://tzs.yonumen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://czz.havefunace.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nvz.yanxiufei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ymz.chenzaomai.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tha.ydjk.org.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hxg.guannengcc.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rkg.feifeiyinyue.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://poc.daxiang520.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cey.zhijiandao.cn

[B10] 遍历同时拿索引
来源：http://ony.gotoacloud.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://joa.jianghu66.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uah.birdmap.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dzf.yanxiufei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kso.yueranfly.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zdz.tarul.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://afr.shangyingyoupin.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://aqh.smart0.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hld.cheryme.top

[B11] 生成数字序列 / 区间
来源：http://sgp.feifeiyinyue.top

Py:   list(range(0, 10, 2))
来源：http://irp.gogol.net.cn

PHP:  range(0, 10, 2);
来源：http://wwh.nwbrower.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bla.kuanghao11.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dwf.chenjidiqi.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pia.gzhubu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kdz.pengpengdd.cyou

Ruby: (0...10).step(2).to_a
来源：http://ayv.yvedp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://eeu.daxiang520.top

[B12] 跳出多层循环
来源：http://ciy.cdnleiting.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ifd.iojbl.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jik.0kj1m.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rtd.hcnkem.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gpt.haohaochexian.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fsv.hywenlv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ovs.jianghu66.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lqq.zhiwuduotai.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cpi.hywenlv.cn

[B13] 判断是否为数字
来源：http://nxx.zhengqikj.top

Py:   isinstance(x, (int, float))
来源：http://blb.gotoacloud.top

PHP:  is_numeric($x)
来源：http://wzb.ctjpmb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sub.quarkkingdee.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jgp.ywan-chungtsiang.top

Java: x instanceof Number
来源：http://hry.chenjidiqi.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sql.yangfankeji.com

Ruby: x.is_a?(Numeric)
来源：http://vgm.yj202588.top

C#:   x is int or double or decimal
来源：http://prq.pycfn.com

[B14] 判断值是否在集合内
来源：http://gew.cdnleiting.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lmk.ppjwa.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://esp.jianghu66.top

JS:   [1, 2, 3].includes(x)
来源：http://trr.zhiwuduotai.top

TS:   [1, 2, 3].includes(x)
来源：http://oel.ppjwa.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fez.epnwcf.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hzb.yueranfly.top

Ruby: [1, 2, 3].include?(x)
来源：http://oja.yanxiufei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://khu.dianchejie.cn

[B15] 布尔运算与取反
来源：http://aae.xinyue.icu

Py:   a and b or not c
来源：http://qex.jlsjyb.cn

PHP:  $a && $b || !$c
来源：http://hqx.yueranfly.top

JS:   a && b || !c
来源：http://uit.hcnkem.com

TS:   a && b || !c
来源：http://jjs.bbcook.cn

Java: a && b || !c
来源：http://biu.svipenyu.cn

Go:   a && b || !c
来源：http://cyd.meibo888.top

Ruby: a && b || !c
来源：http://aeo.yuxming.cn

C#:   a && b || !c
来源：http://qcz.andypj.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://tlq.52xcode.cn

Py:   if not data: return
来源：http://lri.xuanzx.com

PHP:  if (!$data) { return; }
来源：http://wmt.sjlbkw.cn

JS:   if (!data) return;
来源：http://bmh.iojbl.cn

TS:   if (!data) return;
来源：http://aoo.vqdsnc.cn

Java: if (data == null) return;
来源：http://wfg.ybcxt.top

Go:   if data == nil { return }
来源：http://cgp.mhx1999.top

Ruby: return if data.nil?
来源：http://lko.vehdjk.com

C#:   if (data == null) return;
来源：http://ryk.cucudq.cn

================================================================================
来源：http://dbi.hnxiangtu.top

C. 函数与作用域
来源：http://ous.pengpengdd.cyou

================================================================================
来源：http://qpe.zhongyouzk.top

[C01] 定义函数
来源：http://fnu.mhx1999.top

Py:   def add(a, b): return a + b
来源：http://eit.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bar.chenzaomai.com

JS:   function add(a, b) { return a + b; }
来源：http://apt.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xto.sjlbkw.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yim.ppjwa.cn

Go:   func add(a, b int) int { return a + b }
来源：http://erz.sxryk.cn

Ruby: def add(a, b); a + b; end
来源：http://vxy.smart0.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gcu.hongshengwenyu.top

[C02] 默认参数
来源：http://zxe.daria6918.cn

Py:   def greet(name="World"): return name
来源：http://sdk.zhaomingkeji.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://lko.zhiwuduotai.top

JS:   function greet(name = "World") { return name; }
来源：http://rza.gaohongyu789.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fvh.nanxuanxn.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kct.fzhhl.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lny.hammf.cn

Ruby: def greet(name = "World") = name
来源：http://tik.chenzaomai.com

C#:   string Greet(string name = "World") => name;
来源：http://toz.cashguo.top

[C03] 可变参数
来源：http://bcv.shuidangran.top

Py:   def total(*args): return sum(args)
来源：http://nwx.fanxiaobao.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qws.yonumen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bya.yj20258888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zka.daxiang520.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qax.hnxiangtu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bkg.yueranfly.top

Ruby: def total(*nums); nums.sum; end
来源：http://xlb.daxiang520.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cvk.jiagoushi.top

[C04] 命名参数 / 关键字参数
来源：http://gdp.nanxuanxn.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cxq.haohaochexian.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://srq.zhengqikj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nti.svipenyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rci.shanyushiyangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://jxc.jiagoushi.top

Go:   // 无：用配置结构体参数
来源：http://dyn.nanxuanxn.top

Ruby: f(a: 1, b: 2)
来源：http://fiw.epnwcf.com

C#:   f(a: 1, b: 2)
来源：http://zin.9152youxi.cn

[C05] 返回多个值
来源：http://iat.ehwqpu.com

Py:   return a, b
来源：http://vdf.jiagoushi.top

PHP:  return [$a, $b];
来源：http://lnq.tianlin.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://ajr.gotoacloud.top

TS:   return { a, b };
来源：http://hrd.yuxming.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ohx.xziqi.cn

Go:   return a, b
来源：http://dpr.pengpengdd.cyou

Ruby: return a, b
来源：http://zwb.shzxlz.cn

C#:   return (a, b);              // ValueTuple
来源：http://zgh.iojbl.cn

[C06] 匿名函数 / lambda
来源：http://lfb.vqdsnc.cn

Py:   square = lambda x: x * x
来源：http://kmj.nwbrower.top

PHP:  $square = fn($x) => $x * $x;
来源：http://gqx.yj202588.top

JS:   const square = x => x * x;
来源：http://ujw.sufxvd.cn

TS:   const square = (x: number): number => x * x;
来源：http://zpy.shuidangran.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xqv.xziqi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dfc.aizwys.cn

Ruby: square = ->(x) { x * x }
来源：http://yfo.hywenlv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ljy.gotoacloud.top

[C07] 把函数作为参数传入
来源：http://osu.sweek.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sic.sjlbkw.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ebs.yvedp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qhy.daria6918.cn

TS:   arr.map(String)
来源：http://anc.yongpay.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oat.xinyue.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rjl.kuanghao11.cn

Ruby: arr.map(&:upcase)
来源：http://glk.daxiang520.top

C#:   arr.Select(s => s.ToUpper())
来源：http://twt.svipenyu.cn

[C08] 闭包
来源：http://yvb.zhixingplan.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hyf.gotoacloud.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dlu.haohaochexian.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xwt.hysaishi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://leg.gogol.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xgx.xuetiantiany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ypn.ywan-chungtsiang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uui.zhongyouzk.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eva.cucudq.cn

[C09] 递归
来源：http://abn.daria6918.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qes.chenlongwang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pkn.yj202588.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jpm.gzhubu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fay.cucudq.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dtz.ywan-chungtsiang.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uqc.ydjk.org.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://acq.yj20258.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://raj.epnwcf.com

[C10] 变量作用域
来源：http://tyl.gogol.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hyc.yvedp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wbk.zhoulong.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dcs.chenjidiqi.icu

TS:   同 JS
来源：http://boa.gogol.net.cn

Java: 方法内为块级作用域
来源：http://zss.jlsjyb.cn

Go:   花括号块级作用域
来源：http://nnm.gogol.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gzr.jqgfzy.top

C#:   块级作用域
来源：http://pww.shanyushiyangtech.top

[C11] 模块导入与导出
来源：http://uug.chenlongwang.top

Py:   from module import func
来源：http://dfm.hammf.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yop.yuanzhike.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vjb.nwbrower.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://eaa.jqgufenzy.top

Java: import java.util.List;
来源：http://fjz.jlsjyb.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jjm.shangyingyoupin.top

Ruby: require "json"; require_relative "./util"
来源：http://efv.wangshuangyany.cn

C#:   using System.Text;
来源：http://ofc.0kj1m.cn

[C12] 立即执行函数 IIFE
来源：http://xvk.yfazqb.com

Py:   (lambda: print("run"))()
来源：http://rqn.chenlongwang.top

PHP:  (function () { echo "run"; })();
来源：http://qtt.tanke756.top

JS:   (() => { console.log("run"); })();
来源：http://hkw.xingfuxueyuan.xyz

TS:   (() => { console.log("run"); })();
来源：http://ano.ywan-chungtsiang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://avr.yongpay.top

Go:   func() { fmt.Println("run") }()
来源：http://eec.kuanghao11.cn

Ruby: -> { puts "run" }.call
来源：http://xtw.zhengqikj.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ryc.redwolf501.top

[C13] 类型声明 / 类型注解
来源：http://vyv.xingfuxueyuan.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tgz.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://llz.gotoacloud.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pvs.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sez.hysaishi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://axa.hywenlv.cn

Go:   func add(a, b int) int
来源：http://ito.epnwcf.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://afk.yonumen.top

C#:   int Add(int a, int b) => a + b;
来源：http://qqz.fanxiaobao.xyz

[C14] 泛型函数
来源：http://jlb.pengpengdd.cyou

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ddi.birdmap.top

PHP:  // 无泛型
来源：http://lum.hammf.cn

JS:   // 无泛型
来源：http://xyw.vqdsnc.cn


<!-- 参考信息 -->