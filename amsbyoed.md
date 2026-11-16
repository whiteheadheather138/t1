代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://odl.yvedp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bgz.havefunace.top

Ruby: s1 == s2; s1 <=> s2
来源：http://rzf.sjlbkw.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://org.zhiwuduotai.top

[A26] 类型转换总览
来源：http://olb.chenzaomai.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://soi.yvedp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ywg.shanyushiyangtech.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vjv.yj20258888.top

TS:   Number() String() Boolean() x as number
来源：http://hxb.tian-w.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://owh.epnwcf.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nhk.xuetiantiany.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://unn.tianlin.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gcc.yvedp.cn

================================================================================
来源：http://dpq.ctjpmb.com

B. 流程控制
来源：http://ade.vehdjk.com

================================================================================
来源：http://dyj.fzhhl.top

[B01] 条件判断 if / else
来源：http://adi.gotoacloud.top

Py:   result = "正" if x > 0 else "非正"
来源：http://pvx.hesvh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cql.hnqzz.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kgg.bjfxy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nuu.jqgfzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://mtc.wangshuangyany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hph.sjlbkw.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eah.hammf.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cqs.aibaodan.cn

[B02] 多分支 else if / elif
来源：http://ycd.haohaochexian.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wem.cqqwz.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://edz.gzhubu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rtk.shanyushiyangtech.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hnp.fktsv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cyi.jyoumei.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vhi.jyoumei.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://odz.gzhubu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rsd.sysykeji.top

[B03] switch / match / case
来源：http://bnu.feifeiyinyue.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dri.xingfuxueyuan.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qpa.c1oappe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lxb.hcnkem.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cno.meibo888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pjd.zdbjq.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kur.nanxinkj.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ojc.9152youxi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://flj.sweek.top

[B04] for 计数循环
来源：http://bsg.hongshengwenyu.top

Py:   for i in range(10): print(i)
来源：http://eci.0kj1m.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qwi.zhongyouzk.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tst.sjlbkw.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xmm.nanxuanxn.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://npk.cqqwz.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kaj.yuxming.cn

Ruby: 10.times { |i| puts i }
来源：http://iou.yfazqb.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mnt.guowangkeji.top

[B05] 遍历数组 / 列表
来源：http://szq.chenlongwang.top

Py:   for item in arr: print(item)
来源：http://ehi.hfpthk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fev.chenlongwang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://eko.tanke756.top

TS:   for (const item of arr) { console.log(item); }
来源：http://zzs.xuanzx.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://eee.shuidangran.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fsp.bjfxy.top

Ruby: arr.each { |item| puts item }
来源：http://hpt.yangfankeji.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xji.tianlin.xyz

[B06] 遍历字典 / 对象
来源：http://pur.ppjwa.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qic.xylfe.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cny.bbcook.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nao.haohaochexian.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jyh.cqqwz.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wtu.zhoulong.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qjr.sjlbkw.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qov.vqdsnc.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qly.andypj.xyz

[B07] while 循环
来源：http://dtm.hfpthk.cn

Py:   while i < 10: i += 1
来源：http://ccb.jlsjyb.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wub.nanxinkj.top

JS:   while (i < 10) { i++; }
来源：http://izz.zycfv.cn

TS:   while (i < 10) { i++; }
来源：http://pvq.nanxuanxn.top

Java: while (i < 10) { i++; }
来源：http://ejq.tanke756.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kdg.xylfe.cn

Ruby: while i < 10; i += 1; end
来源：http://rid.shanyushiyangtech.top

C#:   while (i < 10) { i++; }
来源：http://fhi.tarul.cn

[B08] do-while（至少执行一次）
来源：http://atj.zdqjudy.top

Py:   # 无 do-while：用 while True + break
来源：http://iig.shangyingyoupin.top

PHP:  do { $i++; } while ($i < 10);
来源：http://era.ctjpmb.com

JS:   do { i++; } while (i < 10);
来源：http://rbs.epnwcf.com

TS:   do { i++; } while (i < 10);
来源：http://zwu.jlsjyb.cn

Java: do { i++; } while (i < 10);
来源：http://zfm.fzhhl.top

Go:   for { i++; if i >= 10 { break } }
来源：http://heg.redwolf501.top

Ruby: begin; i += 1; end while i < 10
来源：http://csg.dashuyun.cn

C#:   do { i++; } while (i < 10);
来源：http://hdj.fktsv.cn

[B09] break 与 continue
来源：http://dua.quarkkingdee.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yth.daxiang520.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oeo.chenzaomai.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lss.yangfankeji.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wii.hnqzz.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kxl.9152youxi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://etp.jiagoushi.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rys.nanxinkj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xhu.jlsjyb.cn

[B10] 遍历同时拿索引
来源：http://aoh.jinqigfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hjz.epnwcf.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://man.uphjek.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://diy.xuanzx.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ccr.xziqi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hky.ybcxt.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qxo.yj20258.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mwu.gotoacloud.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://axm.iojbl.cn

[B11] 生成数字序列 / 区间
来源：http://eqx.jinqigfzy.top

Py:   list(range(0, 10, 2))
来源：http://utj.hongshengwenyu.top

PHP:  range(0, 10, 2);
来源：http://koh.jinqigfzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oql.jyoumei.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ily.aizwys.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wzj.ivvv.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gry.hnqzz.top

Ruby: (0...10).step(2).to_a
来源：http://tff.cdnleiting.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zwc.fengsongda.top

[B12] 跳出多层循环
来源：http://zgr.meibo888.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://hkw.xuanzx.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://qzu.nanxinkj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://avf.pengpengdd.cyou

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hhm.hongshengwenyu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kca.wangshuangyany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vzt.ctjpmb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dzn.zycfv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://iyk.gogol.net.cn

[B13] 判断是否为数字
来源：http://uyq.zhongyouzk.top

Py:   isinstance(x, (int, float))
来源：http://hrp.feifeiyinyue.top

PHP:  is_numeric($x)
来源：http://cdw.gzhubu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cha.cdnleiting.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oae.yuxming.cn

Java: x instanceof Number
来源：http://mih.smart0.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cub.bjfxy.top

Ruby: x.is_a?(Numeric)
来源：http://wdu.ivvv.top

C#:   x is int or double or decimal
来源：http://qzv.fanxiaobao.xyz

[B14] 判断值是否在集合内
来源：http://xqi.sweek.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://znb.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://khe.ybcxt.top

JS:   [1, 2, 3].includes(x)
来源：http://spj.feifeiyinyue.top

TS:   [1, 2, 3].includes(x)
来源：http://nfw.0kj1m.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nzo.hysaishi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ehd.yonumen.top

Ruby: [1, 2, 3].include?(x)
来源：http://bus.hammf.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://frn.mhx1999.top

[B15] 布尔运算与取反
来源：http://vdk.xingfuxueyuan.xyz

Py:   a and b or not c
来源：http://eym.pengpengdd.cyou

PHP:  $a && $b || !$c
来源：http://nkn.cashguo.top

JS:   a && b || !c
来源：http://bnf.tian-w.cn

TS:   a && b || !c
来源：http://abp.yj20258.top

Java: a && b || !c
来源：http://pvx.ybcxt.top

Go:   a && b || !c
来源：http://bol.mhx1999.top

Ruby: a && b || !c
来源：http://aqr.sufxvd.cn

C#:   a && b || !c
来源：http://rhr.shangyingyoupin.top

[B16] 卫语句：不满足条件提前返回
来源：http://edp.jinqigfzy.top

Py:   if not data: return
来源：http://wuq.ydjk.org.cn

PHP:  if (!$data) { return; }
来源：http://wmu.gaohongyu789.top

JS:   if (!data) return;
来源：http://oag.snrcjt.cn

TS:   if (!data) return;
来源：http://mkv.xuetiantiany.cn

Java: if (data == null) return;
来源：http://xep.yj202588.top

Go:   if data == nil { return }
来源：http://nhy.hfpthk.cn

Ruby: return if data.nil?
来源：http://gkn.redwolf501.top

C#:   if (data == null) return;
来源：http://ldn.birdmap.top

================================================================================
来源：http://tvn.xziqi.cn

C. 函数与作用域
来源：http://kqi.xuetiantiany.cn

================================================================================
来源：http://whf.mhx1999.top

[C01] 定义函数
来源：http://mdf.yj202588.top

Py:   def add(a, b): return a + b
来源：http://adv.sxryk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://leg.ybcxt.top

JS:   function add(a, b) { return a + b; }
来源：http://rdb.uphjek.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vqr.fktsv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tfs.chenlongwang.top

Go:   func add(a, b int) int { return a + b }
来源：http://mfz.yuxming.cn

Ruby: def add(a, b); a + b; end
来源：http://sdd.nwbrower.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zzl.yueranfly.top

[C02] 默认参数
来源：http://fnn.zhongyouzk.top

Py:   def greet(name="World"): return name
来源：http://stu.shanyushiyangtech.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qqk.fktsv.cn

JS:   function greet(name = "World") { return name; }
来源：http://owx.jinqigfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://qza.wangshuangyany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wpg.zhongyouzk.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ana.c1oappe.top

Ruby: def greet(name = "World") = name
来源：http://kxu.xylfe.cn

C#:   string Greet(string name = "World") => name;
来源：http://iqb.zycfv.cn

[C03] 可变参数
来源：http://kgl.tian-w.cn

Py:   def total(*args): return sum(args)
来源：http://crb.zhoulong.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gcv.ehwqpu.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://czh.andypj.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eai.wangshuangyany.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oci.yuxming.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oej.hysaishi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://aqm.vehdjk.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qoe.zhengqikj.top

[C04] 命名参数 / 关键字参数
来源：http://law.aibaodan.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ytx.nwbrower.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ryk.316326.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lsg.yuanzhike.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vox.hywenlv.cn

Java: // 无：用 Builder 模式或 record
来源：http://tte.uphjek.com

Go:   // 无：用配置结构体参数
来源：http://fkj.iojbl.cn

Ruby: f(a: 1, b: 2)
来源：http://bek.fzhhl.top

C#:   f(a: 1, b: 2)
来源：http://akt.svipenyu.cn

[C05] 返回多个值
来源：http://oye.hcnkem.com

Py:   return a, b
来源：http://djx.nwbrower.top

PHP:  return [$a, $b];
来源：http://pkq.316326.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://aid.316326.xyz

TS:   return { a, b };
来源：http://kkx.aibaodan.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://iri.jinyuanbaomall.cn

Go:   return a, b
来源：http://upw.zhoulong.xyz

Ruby: return a, b
来源：http://emo.gzhubu.top

C#:   return (a, b);              // ValueTuple
来源：http://wut.hesvh.cn

[C06] 匿名函数 / lambda
来源：http://ekw.aizwys.cn

Py:   square = lambda x: x * x
来源：http://pms.birdmap.top

PHP:  $square = fn($x) => $x * $x;
来源：http://viv.chenzaomai.com

JS:   const square = x => x * x;
来源：http://jiw.c1oappe.top

TS:   const square = (x: number): number => x * x;
来源：http://eej.jiagoushi.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tqv.hammf.cn

Go:   sq := func(x int) int { return x * x }
来源：http://uqk.xuanzx.com

Ruby: square = ->(x) { x * x }
来源：http://bdv.xylfe.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tlx.shangyingyoupin.top

[C07] 把函数作为参数传入
来源：http://lsh.jqgufenzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://doy.yj20258.top

PHP:  array_map("strtoupper", $arr);
来源：http://dxn.zhixingplan.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://iue.meibo888.top

TS:   arr.map(String)
来源：http://nzm.yfazqb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dea.hongshengwenyu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jyd.hnqzz.top

Ruby: arr.map(&:upcase)
来源：http://dtg.jqgufenzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://pzn.zhaomingkeji.xyz

[C08] 闭包
来源：http://iik.sjlbkw.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oyc.ehwqpu.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yhv.xziqi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://coe.yuxming.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dvl.zhixingplan.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fnv.bbcook.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wnl.feifeiyinyue.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dvx.hongshengwenyu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://itj.meibo888.top

[C09] 递归
来源：http://wnx.hfpthk.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ahb.gogol.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://twe.meibo888.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xde.svipenyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hkj.ywan-chungtsiang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cuk.gaohongyu789.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gke.nanxinkj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bmq.xinyue.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yyw.xinyue.icu

[C10] 变量作用域
来源：http://fqp.ehwqpu.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tlg.jianghu66.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://phg.gaohongyu789.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://goc.yangfankeji.com

TS:   同 JS
来源：http://def.52xcode.cn

Java: 方法内为块级作用域
来源：http://mya.zycfv.cn

Go:   花括号块级作用域
来源：http://jdj.sysykeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hws.shanyushiyangtech.top

C#:   块级作用域
来源：http://rtv.vqdsnc.cn

[C11] 模块导入与导出
来源：http://ylp.andypj.xyz

Py:   from module import func
来源：http://vxn.dashuyun.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xbf.c1oappe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://djl.shanyushiyangtech.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://msv.jiagoushi.top

Java: import java.util.List;
来源：http://yyw.xylfe.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dyr.sxryk.cn

Ruby: require "json"; require_relative "./util"
来源：http://icl.aibaodan.cn

C#:   using System.Text;
来源：http://gnk.sjlbkw.cn

[C12] 立即执行函数 IIFE
来源：http://yqu.ydjk.org.cn

Py:   (lambda: print("run"))()
来源：http://dmd.yongpay.top

PHP:  (function () { echo "run"; })();
来源：http://quw.yanxiufei.cn

JS:   (() => { console.log("run"); })();
来源：http://fzm.xuanzx.com

TS:   (() => { console.log("run"); })();
来源：http://ipf.jyoumei.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://igt.guannengcc.top

Go:   func() { fmt.Println("run") }()
来源：http://nqd.yueranfly.top

Ruby: -> { puts "run" }.call
来源：http://ael.jinqigfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://hsl.ehwqpu.com

[C13] 类型声明 / 类型注解
来源：http://bno.bjfxy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qba.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qms.epnwcf.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rmz.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tsl.ctjpmb.com

Java: int add(int a, int b) { return a + b; }
来源：http://yrv.dashuyun.cn

Go:   func add(a, b int) int
来源：http://jvw.xuetiantiany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vib.andypj.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://bhh.tian-w.cn

[C14] 泛型函数
来源：http://rlu.shanyushiyangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mgp.0kj1m.cn

PHP:  // 无泛型
来源：http://oty.c1oappe.top

JS:   // 无泛型
来源：http://jqb.chenzaomai.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ouh.dianchejie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xuw.zdqjudy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xlc.shzxlz.cn

Ruby: # 无泛型
来源：http://dqc.hywenlv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bro.xuetiantiany.cn

[C15] 解构 / 展开参数
来源：http://bus.guannengcc.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qvv.ehwqpu.com

PHP:  [$a, $b] = $pair;
来源：http://tub.yonumen.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uyi.birdmap.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pwq.fanxiaobao.xyz

Java: // 无解构
来源：http://uks.zhixingplan.top

Go:   // 无解构
来源：http://rho.sxryk.cn

Ruby: a, b = pair
来源：http://wor.hysaishi.cn

C#:   var (a, b) = pair;
来源：http://xst.hysaishi.cn

[C16] 函数 / 方法重载
来源：http://pmo.shanyushiyangtech.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cwu.ydzc1.top


<!-- 参考信息 -->