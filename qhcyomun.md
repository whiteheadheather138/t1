代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://ond.zycfv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nun.pengpengdd.cyou

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://arm.cdnleiting.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zjr.yvedp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baw.zdqjudy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jfb.zhiwuduotai.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ksk.52xcode.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://iwu.gotoacloud.top

[A26] 类型转换总览
来源：http://jew.zdqjudy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cze.nanxuanxn.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jes.zycfv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sgy.hywenlv.cn

TS:   Number() String() Boolean() x as number
来源：http://xwg.kuanghao11.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mvp.shzxlz.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dol.jqgufenzy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://wtu.jiagoushi.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mrj.yangfankeji.com

================================================================================
来源：http://ncg.bbcook.cn

B. 流程控制
来源：http://lpi.yvedp.cn

================================================================================
来源：http://lmg.xingfuxueyuan.xyz

[B01] 条件判断 if / else
来源：http://hev.ehwqpu.com

Py:   result = "正" if x > 0 else "非正"
来源：http://hwr.aibaodan.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eih.jqgufenzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://smk.hongshengwenyu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wpg.ctjpmb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://gtu.snrcjt.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sck.hammf.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://roy.xinyue.icu

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tlt.sweek.top

[B02] 多分支 else if / elif
来源：http://fzx.ehwqpu.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blh.jinqigufen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nzq.vqdsnc.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zuu.52xcode.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hnx.hesvh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zio.ivvv.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qyp.ivvv.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yfk.daxiang520.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zpw.hysaishi.cn

[B03] switch / match / case
来源：http://trf.svipenyu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://heg.yangfankeji.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hoh.yueranfly.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wjs.kuanghao11.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ysr.fzhhl.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cji.hcnkem.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://npx.zhaomingkeji.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kqt.zhoulong.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gfz.jinghuilouyu.cn

[B04] for 计数循环
来源：http://bzd.ppjwa.cn

Py:   for i in range(10): print(i)
来源：http://wio.xuetiantiany.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nmi.hammf.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zik.ydjk.org.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rmt.mhx1999.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vqr.nwbrower.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wwu.bjfxy.top

Ruby: 10.times { |i| puts i }
来源：http://rxv.jinqigufen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://srs.c1oappe.top

[B05] 遍历数组 / 列表
来源：http://stp.jinqigfzy.top

Py:   for item in arr: print(item)
来源：http://cuj.hongshengwenyu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wof.zhiwuduotai.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hfj.yj20258.top

TS:   for (const item of arr) { console.log(item); }
来源：http://kvy.dianchejie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://twn.jianghu66.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ryz.sysykeji.top

Ruby: arr.each { |item| puts item }
来源：http://tag.cqqwz.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bka.9152youxi.cn

[B06] 遍历字典 / 对象
来源：http://rmn.cashguo.top

Py:   for k, v in d.items(): print(k, v)
来源：http://izj.xylfe.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://siu.jianghu66.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kwv.cqqwz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pwj.jinyuanbaomall.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kwg.daxiang520.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jxl.quarkkingdee.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vod.hysaishi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vuy.yuxming.cn

[B07] while 循环
来源：http://jfd.ybcxt.top

Py:   while i < 10: i += 1
来源：http://jjg.quarkkingdee.top

PHP:  while ($i < 10) { $i++; }
来源：http://nin.ppjwa.cn

JS:   while (i < 10) { i++; }
来源：http://sot.fehbvm.com

TS:   while (i < 10) { i++; }
来源：http://yti.ehwqpu.com

Java: while (i < 10) { i++; }
来源：http://spm.xylfe.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bnz.shangyingyoupin.top

Ruby: while i < 10; i += 1; end
来源：http://geh.jqgfzy.top

C#:   while (i < 10) { i++; }
来源：http://tla.tanke756.top

[B08] do-while（至少执行一次）
来源：http://psj.ywan-chungtsiang.top

Py:   # 无 do-while：用 while True + break
来源：http://ssx.jlsjyb.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://roj.xinyue.icu

JS:   do { i++; } while (i < 10);
来源：http://vbz.ywan-chungtsiang.top

TS:   do { i++; } while (i < 10);
来源：http://wzc.xingfuxueyuan.xyz

Java: do { i++; } while (i < 10);
来源：http://hlv.fengsongda.top

Go:   for { i++; if i >= 10 { break } }
来源：http://iwm.9152youxi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://slx.epnwcf.com

C#:   do { i++; } while (i < 10);
来源：http://nvg.cqqwz.cn

[B09] break 与 continue
来源：http://keo.xuanzx.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ayv.meibo888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uax.zhaomingkeji.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ezg.ehwqpu.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://srx.zhijiandao.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pdd.feifeiyinyue.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mxw.fanxiaobao.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qlk.52xcode.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cjg.quarkkingdee.top

[B10] 遍历同时拿索引
来源：http://jtx.jinyuanbaomall.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mfg.yonumen.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nzm.meibo888.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zom.hfpthk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qeu.hywenlv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aej.jlsjyb.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nal.shangyingyoupin.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dtr.52xcode.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hzc.birdmap.top

[B11] 生成数字序列 / 区间
来源：http://fbo.yonumen.top

Py:   list(range(0, 10, 2))
来源：http://ier.aizwys.cn

PHP:  range(0, 10, 2);
来源：http://jmz.xylfe.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kqy.jinqigfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lkt.9152youxi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dod.sysykeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bmd.xuanzx.com

Ruby: (0...10).step(2).to_a
来源：http://osb.jqgfzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ttu.jyoumei.cn

[B12] 跳出多层循环
来源：http://gbc.cdnleiting.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://hyc.tarul.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tdu.zhijiandao.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uqt.jinqigufen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dqd.sweek.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ysh.epnwcf.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bip.zhiwuduotai.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zjo.yj20258.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yrp.yfazqb.com

[B13] 判断是否为数字
来源：http://cem.zhixingplan.top

Py:   isinstance(x, (int, float))
来源：http://ltd.ppjwa.cn

PHP:  is_numeric($x)
来源：http://bvp.jianghu66.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nln.cashguo.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ctw.cqqwz.cn

Java: x instanceof Number
来源：http://ohi.xingfuxueyuan.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://iox.jqgufenzy.top

Ruby: x.is_a?(Numeric)
来源：http://nuw.dashuyun.cn

C#:   x is int or double or decimal
来源：http://xmf.ivvv.top

[B14] 判断值是否在集合内
来源：http://uil.yfazqb.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pez.meibo888.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vxq.xuanzx.com

JS:   [1, 2, 3].includes(x)
来源：http://mug.ywan-chungtsiang.top

TS:   [1, 2, 3].includes(x)
来源：http://vvp.ctjpmb.com

Java: List.of(1, 2, 3).contains(x)
来源：http://pjt.zhengqikj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://axu.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://xvw.zhengqikj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tjw.wangshuangyany.cn

[B15] 布尔运算与取反
来源：http://dfe.pengpengdd.cyou

Py:   a and b or not c
来源：http://ohy.ctjpmb.com

PHP:  $a && $b || !$c
来源：http://hnb.sysykeji.top

JS:   a && b || !c
来源：http://awc.nanxuanxn.top

TS:   a && b || !c
来源：http://dau.andypj.xyz

Java: a && b || !c
来源：http://fgw.iojbl.cn

Go:   a && b || !c
来源：http://gui.tianlin.xyz

Ruby: a && b || !c
来源：http://hap.nwbrower.top

C#:   a && b || !c
来源：http://aod.daxiang520.top

[B16] 卫语句：不满足条件提前返回
来源：http://mti.jianghu66.top

Py:   if not data: return
来源：http://cdz.zycfv.cn

PHP:  if (!$data) { return; }
来源：http://nll.yj202588.top

JS:   if (!data) return;
来源：http://scj.zhijiandao.cn

TS:   if (!data) return;
来源：http://fyf.kuanghao11.cn

Java: if (data == null) return;
来源：http://iue.xziqi.cn

Go:   if data == nil { return }
来源：http://exl.mhx1999.top

Ruby: return if data.nil?
来源：http://qtm.fktsv.cn

C#:   if (data == null) return;
来源：http://ebx.chenlongwang.top

================================================================================
来源：http://hry.zhiwuduotai.top

C. 函数与作用域
来源：http://mwm.kuanghao11.cn

================================================================================
来源：http://xbt.dashuyun.cn

[C01] 定义函数
来源：http://rot.mhx1999.top

Py:   def add(a, b): return a + b
来源：http://sjd.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yjo.andypj.xyz

JS:   function add(a, b) { return a + b; }
来源：http://qhg.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kqg.vehdjk.com

Java: static int add(int a, int b) { return a + b; }
来源：http://vrp.ydjk.org.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lin.sweek.top

Ruby: def add(a, b); a + b; end
来源：http://vqn.snrcjt.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pav.ydzc1.top

[C02] 默认参数
来源：http://wti.uphjek.com

Py:   def greet(name="World"): return name
来源：http://afg.zhengqikj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ebd.0kj1m.cn

JS:   function greet(name = "World") { return name; }
来源：http://avd.ywan-chungtsiang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ogh.epnwcf.com

Java: // 无默认参数：方法重载或 Optional
来源：http://sss.fehbvm.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nah.zhaomingkeji.xyz

Ruby: def greet(name = "World") = name
来源：http://cpf.gogol.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://ifg.vehdjk.com

[C03] 可变参数
来源：http://kaf.yonumen.top

Py:   def total(*args): return sum(args)
来源：http://bxl.jyoumei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lqc.feifeiyinyue.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qkp.sufxvd.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qtp.ydjk.org.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lld.zhongyouzk.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xnd.hammf.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hnw.ivvv.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ugw.aizwys.cn

[C04] 命名参数 / 关键字参数
来源：http://ybj.jinqigfzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://veh.yongpay.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kle.ydzc1.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jiy.jlsjyb.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://guu.316326.xyz

Java: // 无：用 Builder 模式或 record
来源：http://tkj.tarul.cn

Go:   // 无：用配置结构体参数
来源：http://gez.cqqwz.cn

Ruby: f(a: 1, b: 2)
来源：http://kph.quarkkingdee.top

C#:   f(a: 1, b: 2)
来源：http://ebw.yuxming.cn

[C05] 返回多个值
来源：http://hod.yuanzhike.top

Py:   return a, b
来源：http://yez.shanyushiyangkeji.top

PHP:  return [$a, $b];
来源：http://bii.0kj1m.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dbq.zhengqikj.top

TS:   return { a, b };
来源：http://mgd.vqdsnc.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://aqi.gaohongyu789.top

Go:   return a, b
来源：http://coi.guowangkeji.top

Ruby: return a, b
来源：http://ssj.vqdsnc.cn

C#:   return (a, b);              // ValueTuple
来源：http://hnb.meibo888.top

[C06] 匿名函数 / lambda
来源：http://dqt.ydjk.org.cn

Py:   square = lambda x: x * x
来源：http://vtr.bbcook.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wxv.fktsv.cn

JS:   const square = x => x * x;
来源：http://qzg.nwbrower.top

TS:   const square = (x: number): number => x * x;
来源：http://xup.cucudq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://adj.ydjk.org.cn

Go:   sq := func(x int) int { return x * x }
来源：http://etk.yueranfly.top

Ruby: square = ->(x) { x * x }
来源：http://pnf.fengsongda.top

C#:   Func<int, int> square = x => x * x;
来源：http://zto.hfpthk.cn

[C07] 把函数作为参数传入
来源：http://qty.fengsongda.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wwt.zdbjq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ebc.fanxiaobao.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bqj.bbcook.cn

TS:   arr.map(String)
来源：http://zys.yongpay.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hib.zhongyouzk.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nbn.zhixingplan.top

Ruby: arr.map(&:upcase)
来源：http://thj.gaohongyu789.top

C#:   arr.Select(s => s.ToUpper())
来源：http://anx.shuidangran.top

[C08] 闭包
来源：http://cxb.fzhhl.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yyk.kuanghao11.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cbv.jlsjyb.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://usf.iojbl.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kyb.ywan-chungtsiang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dwo.yj20258.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qux.fktsv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oef.smart0.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tsy.shzxlz.cn

[C09] 递归
来源：http://qdh.yanxiufei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wgj.yj202588.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ziq.svipenyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qbb.c1oappe.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xxp.yj20258.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lgf.xziqi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iok.cashguo.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://icg.hongshengwenyu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gmy.tianlin.xyz

[C10] 变量作用域
来源：http://fbj.hcnkem.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oit.shanyushiyangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rcb.guannengcc.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qkq.jinqigufen.top

TS:   同 JS
来源：http://jtl.hesvh.cn

Java: 方法内为块级作用域
来源：http://iuo.sufxvd.cn

Go:   花括号块级作用域
来源：http://xbd.tanke756.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://man.sysykeji.top

C#:   块级作用域
来源：http://ysr.jianghu66.top

[C11] 模块导入与导出
来源：http://zfa.daxiang520.top

Py:   from module import func
来源：http://kdm.yangfankeji.com

PHP:  require "file.php";  或 use App\Service;
来源：http://pil.aibaodan.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hoh.meibo888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hjq.birdmap.top

Java: import java.util.List;
来源：http://zka.zdbjq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bqy.nanxinkj.top

Ruby: require "json"; require_relative "./util"
来源：http://xbr.zycfv.cn

C#:   using System.Text;
来源：http://eax.chenzaomai.com

[C12] 立即执行函数 IIFE
来源：http://gtn.mhx1999.top

Py:   (lambda: print("run"))()
来源：http://ogt.bjfxy.top

PHP:  (function () { echo "run"; })();
来源：http://yex.cqqwz.cn

JS:   (() => { console.log("run"); })();
来源：http://gre.meibo888.top

TS:   (() => { console.log("run"); })();
来源：http://gti.jiagoushi.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xsu.hnxiangtu.top

Go:   func() { fmt.Println("run") }()
来源：http://zxb.zhaomingkeji.xyz

Ruby: -> { puts "run" }.call
来源：http://wtv.hcnkem.com

C#:   // 无 IIFE：用静态构造函数
来源：http://zao.jinqigufen.top

[C13] 类型声明 / 类型注解
来源：http://uvb.sweek.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gvd.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://atu.ybcxt.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rcf.uphjek.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lut.xuanzx.com

Java: int add(int a, int b) { return a + b; }
来源：http://oks.yueranfly.top

Go:   func add(a, b int) int
来源：http://xro.0kj1m.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://syx.hesvh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fdg.jinyuanbaomall.cn

[C14] 泛型函数
来源：http://hbk.ivvv.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wlh.nwbrower.top

PHP:  // 无泛型
来源：http://yge.xuanzx.com

JS:   // 无泛型
来源：http://zih.cheryme.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://iap.ppjwa.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hbd.shuidangran.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mus.bbcook.cn

Ruby: # 无泛型
来源：http://hey.birdmap.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mcj.wangshuangyany.cn

[C15] 解构 / 展开参数
来源：http://jqg.wangdashe.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://boz.nanxinkj.top

PHP:  [$a, $b] = $pair;
来源：http://tux.aibaodan.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lgo.jyoumei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lsw.yvedp.cn

Java: // 无解构
来源：http://yan.9152youxi.cn

Go:   // 无解构
来源：http://vqm.fengsongda.top


<!-- 参考信息 -->