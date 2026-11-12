代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tdf.bjfxy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://dmc.fengsongda.top

[A24] 去除首尾空白
来源：http://txe.cqqwz.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fem.pycfn.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iig.zhoulong.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qqa.yj202588.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kpq.guannengcc.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pib.svipenyu.cn

Go:   strings.TrimSpace(s)
来源：http://eqf.hnqzz.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ssp.ydjk.org.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dhp.shangyingyoupin.top

[A25] 字符串比较
来源：http://czp.yj202588.top

Py:   s1 == s2; s1 != s2
来源：http://nlg.hongshengwenyu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hxb.dianchejie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uxo.sweek.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ery.zhoulong.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zyp.ybcxt.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zdl.yanxiufei.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://eer.cucudq.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rmp.fanxiaobao.xyz

[A26] 类型转换总览
来源：http://tfk.bbcook.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yab.gogol.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cow.fengsongda.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lhg.yj20258888.top

TS:   Number() String() Boolean() x as number
来源：http://lkk.zhengqikj.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qeb.ehwqpu.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hkd.jlsjyb.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://heh.jinqigufen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kjq.yvedp.cn

================================================================================
来源：http://qgq.ydzc1.top

B. 流程控制
来源：http://iiu.aibaodan.cn

================================================================================
来源：http://yjw.wangshuangyany.cn

[B01] 条件判断 if / else
来源：http://evl.mhx1999.top

Py:   result = "正" if x > 0 else "非正"
来源：http://avl.zdqjudy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ads.fengsongda.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://btg.yfazqb.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://omg.xziqi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cgb.316326.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pvu.bbcook.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ziw.jianghu66.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yrf.guowangkeji.top

[B02] 多分支 else if / elif
来源：http://jgp.snrcjt.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rym.aibaodan.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://buf.haohaochexian.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pmp.dashuyun.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kyw.mhx1999.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jyj.aibaodan.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nnx.tanke756.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uef.cheryme.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://moe.nanxinkj.top

[B03] switch / match / case
来源：http://zee.nanxuanxn.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://iyz.jinqigufen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nrq.pengpengdd.cyou

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://quu.ivvv.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wkj.shzxlz.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hxm.yonumen.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mjy.tanke756.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gta.hongshengwenyu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ahm.gotoacloud.top

[B04] for 计数循环
来源：http://mpv.nanxinkj.top

Py:   for i in range(10): print(i)
来源：http://uqq.yj202588.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sbu.uphjek.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uff.jyoumei.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sek.shangyingyoupin.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uij.guannengcc.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nva.nanxinkj.top

Ruby: 10.times { |i| puts i }
来源：http://evg.zhoulong.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://opm.zhengqikj.top

[B05] 遍历数组 / 列表
来源：http://tns.birdmap.top

Py:   for item in arr: print(item)
来源：http://clg.jinyuanbaomall.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bbt.hnxiangtu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://jum.epnwcf.com

TS:   for (const item of arr) { console.log(item); }
来源：http://bsv.nanxuanxn.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ivj.zhongyouzk.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://trt.daxiang520.top

Ruby: arr.each { |item| puts item }
来源：http://opt.feifeiyinyue.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hcu.meibo888.top

[B06] 遍历字典 / 对象
来源：http://mxs.wangdashe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://myr.gogol.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ryn.zhengqikj.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kjz.ivvv.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xdg.cashguo.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tmi.zhijiandao.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dnu.cucudq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://alp.shanyushiyangtech.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vse.fehbvm.com

[B07] while 循环
来源：http://eap.xinyue.icu

Py:   while i < 10: i += 1
来源：http://bmp.52xcode.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qqs.c1oappe.top

JS:   while (i < 10) { i++; }
来源：http://oee.chenzaomai.com

TS:   while (i < 10) { i++; }
来源：http://qzm.hnxiangtu.top

Java: while (i < 10) { i++; }
来源：http://uhu.daxiang520.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hjs.andypj.xyz

Ruby: while i < 10; i += 1; end
来源：http://ogx.yanxiufei.cn

C#:   while (i < 10) { i++; }
来源：http://nhc.dianchejie.cn

[B08] do-while（至少执行一次）
来源：http://lnt.zdbjq.cn

Py:   # 无 do-while：用 while True + break
来源：http://ayh.jianghu66.top

PHP:  do { $i++; } while ($i < 10);
来源：http://mrc.ybcxt.top

JS:   do { i++; } while (i < 10);
来源：http://tua.zycfv.cn

TS:   do { i++; } while (i < 10);
来源：http://yav.gotoacloud.top

Java: do { i++; } while (i < 10);
来源：http://ppl.epnwcf.com

Go:   for { i++; if i >= 10 { break } }
来源：http://mjt.zycfv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mnd.hywenlv.cn

C#:   do { i++; } while (i < 10);
来源：http://bqi.xziqi.cn

[B09] break 与 continue
来源：http://wry.sufxvd.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iul.epnwcf.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://acr.uphjek.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dqk.sweek.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lyf.havefunace.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fhv.sufxvd.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vpo.snrcjt.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://atj.birdmap.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ops.xinyue.icu

[B10] 遍历同时拿索引
来源：http://qaq.jinghuilouyu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hva.yj202588.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xlt.hnxiangtu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nzd.fanxiaobao.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gyd.shuidangran.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sqt.guowangkeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rkd.cdnleiting.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vgi.xylfe.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qlp.dianchejie.cn

[B11] 生成数字序列 / 区间
来源：http://lof.nanxuanxn.top

Py:   list(range(0, 10, 2))
来源：http://dnx.havefunace.top

PHP:  range(0, 10, 2);
来源：http://urv.ybcxt.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oun.cheryme.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aqz.daxiang520.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vhq.shanyushiyangkeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jdn.yj20258.top

Ruby: (0...10).step(2).to_a
来源：http://aho.cucudq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bvv.hammf.cn

[B12] 跳出多层循环
来源：http://qbr.cdnleiting.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://tmc.yfazqb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://tas.316326.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pud.zhaomingkeji.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://woc.bbcook.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kel.yj20258.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jlz.hongshengwenyu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mhl.xuanzx.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uzj.pycfn.com

[B13] 判断是否为数字
来源：http://kon.zhongyouzk.top

Py:   isinstance(x, (int, float))
来源：http://dim.xziqi.cn

PHP:  is_numeric($x)
来源：http://tnm.ywan-chungtsiang.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://coo.xziqi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kyh.yj202588.top

Java: x instanceof Number
来源：http://wbc.iojbl.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ugc.yangfankeji.com

Ruby: x.is_a?(Numeric)
来源：http://ozg.gotoacloud.top

C#:   x is int or double or decimal
来源：http://sow.yongpay.top

[B14] 判断值是否在集合内
来源：http://vqb.hammf.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jei.yonumen.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hsz.daxiang520.top

JS:   [1, 2, 3].includes(x)
来源：http://rzf.sxryk.cn

TS:   [1, 2, 3].includes(x)
来源：http://xdv.xziqi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://eph.hammf.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qkb.yj20258.top

Ruby: [1, 2, 3].include?(x)
来源：http://xcv.nanxinkj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jfx.xziqi.cn

[B15] 布尔运算与取反
来源：http://uco.redwolf501.top

Py:   a and b or not c
来源：http://xgq.nwbrower.top

PHP:  $a && $b || !$c
来源：http://ixy.fehbvm.com

JS:   a && b || !c
来源：http://bny.yongpay.top

TS:   a && b || !c
来源：http://ypp.aibaodan.cn

Java: a && b || !c
来源：http://bhq.fzhhl.top

Go:   a && b || !c
来源：http://fss.nanxuanxn.top

Ruby: a && b || !c
来源：http://hiy.guannengcc.top

C#:   a && b || !c
来源：http://ihf.gaohongyu789.top

[B16] 卫语句：不满足条件提前返回
来源：http://xkb.ppjwa.cn

Py:   if not data: return
来源：http://gfp.ywan-chungtsiang.top

PHP:  if (!$data) { return; }
来源：http://ddp.hnxiangtu.top

JS:   if (!data) return;
来源：http://gik.zhengqikj.top

TS:   if (!data) return;
来源：http://grp.cdnleiting.top

Java: if (data == null) return;
来源：http://pew.yvedp.cn

Go:   if data == nil { return }
来源：http://jhg.yueranfly.top

Ruby: return if data.nil?
来源：http://vzm.fzhhl.top

C#:   if (data == null) return;
来源：http://gdg.hysaishi.cn

================================================================================
来源：http://bbg.tanke756.top

C. 函数与作用域
来源：http://nxk.cucudq.cn

================================================================================
来源：http://ohm.pengpengdd.cyou

[C01] 定义函数
来源：http://mnw.xziqi.cn

Py:   def add(a, b): return a + b
来源：http://wyu.cashguo.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rmo.fanxiaobao.xyz

JS:   function add(a, b) { return a + b; }
来源：http://oty.svipenyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fpp.cashguo.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zvx.tanke756.top

Go:   func add(a, b int) int { return a + b }
来源：http://tpd.hongshengwenyu.top

Ruby: def add(a, b); a + b; end
来源：http://yfg.hysaishi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://erz.wangshuangyany.cn

[C02] 默认参数
来源：http://nqo.vqdsnc.cn

Py:   def greet(name="World"): return name
来源：http://ivb.yanxiufei.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fed.jqgufenzy.top

JS:   function greet(name = "World") { return name; }
来源：http://diw.cqqwz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://oev.hesvh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nlb.yueranfly.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jyr.jiagoushi.top

Ruby: def greet(name = "World") = name
来源：http://rvx.uphjek.com

C#:   string Greet(string name = "World") => name;
来源：http://zfw.yfazqb.com

[C03] 可变参数
来源：http://dat.ydjk.org.cn

Py:   def total(*args): return sum(args)
来源：http://qdp.sufxvd.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gwq.c1oappe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://acn.zhijiandao.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mnd.fktsv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hle.meibo888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kkd.nanxuanxn.top

Ruby: def total(*nums); nums.sum; end
来源：http://tol.sweek.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lcp.sweek.top

[C04] 命名参数 / 关键字参数
来源：http://xjh.xylfe.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xvw.wangdashe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nsl.cdnleiting.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://aoc.sxryk.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ene.redwolf501.top

Java: // 无：用 Builder 模式或 record
来源：http://nqx.cqqwz.cn

Go:   // 无：用配置结构体参数
来源：http://dbz.hammf.cn

Ruby: f(a: 1, b: 2)
来源：http://rfy.gzhubu.top

C#:   f(a: 1, b: 2)
来源：http://ipo.daxiang520.top

[C05] 返回多个值
来源：http://baz.tarul.cn

Py:   return a, b
来源：http://gwj.andypj.xyz

PHP:  return [$a, $b];
来源：http://azy.wangdashe.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://scg.zdqjudy.top

TS:   return { a, b };
来源：http://lib.ivvv.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gur.fanxiaobao.xyz

Go:   return a, b
来源：http://ifg.shanyushiyangtech.top

Ruby: return a, b
来源：http://hvc.hnqzz.top

C#:   return (a, b);              // ValueTuple
来源：http://peg.yuanzhike.top

[C06] 匿名函数 / lambda
来源：http://hgg.sweek.top

Py:   square = lambda x: x * x
来源：http://otr.guannengcc.top

PHP:  $square = fn($x) => $x * $x;
来源：http://pdr.yueranfly.top

JS:   const square = x => x * x;
来源：http://wrs.jiagoushi.top

TS:   const square = (x: number): number => x * x;
来源：http://rla.yvedp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wdt.zhoulong.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://mdv.bbcook.cn

Ruby: square = ->(x) { x * x }
来源：http://gac.zhijiandao.cn

C#:   Func<int, int> square = x => x * x;
来源：http://eya.tianlin.xyz

[C07] 把函数作为参数传入
来源：http://zxw.hfpthk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rxn.shanyushiyangtech.top

PHP:  array_map("strtoupper", $arr);
来源：http://bfd.chenjidiqi.icu

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pce.hcnkem.com

TS:   arr.map(String)
来源：http://gfo.mhx1999.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ske.cashguo.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wis.zdqjudy.top

Ruby: arr.map(&:upcase)
来源：http://los.jyoumei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xcc.tarul.cn

[C08] 闭包
来源：http://qld.hammf.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://obj.birdmap.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yya.jqgfzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cnd.xingfuxueyuan.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qxg.yangfankeji.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tgc.iojbl.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vuh.quarkkingdee.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yns.xinyue.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vvl.guowangkeji.top

[C09] 递归
来源：http://dxn.mhx1999.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nzd.yangfankeji.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ehl.daria6918.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ksy.bjfxy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yim.wangshuangyany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dtv.hammf.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://btz.cqqwz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://htp.birdmap.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rxi.sufxvd.cn

[C10] 变量作用域
来源：http://esk.cucudq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fgj.daria6918.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dfe.haohaochexian.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kjf.jinqigufen.top

TS:   同 JS
来源：http://ood.ctjpmb.com

Java: 方法内为块级作用域
来源：http://obt.yuxming.cn

Go:   花括号块级作用域
来源：http://vuq.zhiwuduotai.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fzv.ydzc1.top

C#:   块级作用域
来源：http://hfl.ctjpmb.com

[C11] 模块导入与导出
来源：http://mad.zdbjq.cn

Py:   from module import func
来源：http://suo.haohaochexian.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kmc.hnqzz.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://weg.fktsv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wqm.52xcode.cn

Java: import java.util.List;
来源：http://rqb.hesvh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jkx.zhongyouzk.top

Ruby: require "json"; require_relative "./util"
来源：http://uym.jqgufenzy.top

C#:   using System.Text;
来源：http://goy.9152youxi.cn

[C12] 立即执行函数 IIFE
来源：http://qyy.yangfankeji.com

Py:   (lambda: print("run"))()
来源：http://vki.hysaishi.cn

PHP:  (function () { echo "run"; })();
来源：http://frf.dianchejie.cn

JS:   (() => { console.log("run"); })();
来源：http://kvj.jinghuilouyu.cn

TS:   (() => { console.log("run"); })();
来源：http://ckt.hesvh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://llr.jqgufenzy.top

Go:   func() { fmt.Println("run") }()
来源：http://ung.gaohongyu789.top

Ruby: -> { puts "run" }.call
来源：http://lmi.fanxiaobao.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://gvn.sufxvd.cn

[C13] 类型声明 / 类型注解
来源：http://vim.zdbjq.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lpj.cashguo.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fze.zdqjudy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hht.c1oappe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wrv.hywenlv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mro.svipenyu.cn

Go:   func add(a, b int) int
来源：http://zps.daxiang520.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://viw.pengpengdd.cyou

C#:   int Add(int a, int b) => a + b;
来源：http://kru.gogol.net.cn

[C14] 泛型函数
来源：http://xwe.aizwys.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ntd.iojbl.cn

PHP:  // 无泛型
来源：http://kus.bjfxy.top

JS:   // 无泛型
来源：http://azi.jlsjyb.cn


<!-- 参考信息 -->