代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://rzc.andypj.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nzb.pycfn.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sun.316326.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nqt.tanke756.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://plv.uphjek.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ego.yj20258.top

Ruby: s1 == s2; s1 <=> s2
来源：http://voy.ywan-chungtsiang.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zxm.tianlin.xyz

[A26] 类型转换总览
来源：http://cop.zdbjq.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wkk.iojbl.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dcl.zhiwuduotai.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tum.guowangkeji.top

TS:   Number() String() Boolean() x as number
来源：http://oqd.hcnkem.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wnl.shangyingyoupin.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ayx.vqdsnc.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ubl.sufxvd.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zmf.hnqzz.top

================================================================================
来源：http://uki.shanyushiyangkeji.top

B. 流程控制
来源：http://frj.nanxinkj.top

================================================================================
来源：http://wmm.fktsv.cn

[B01] 条件判断 if / else
来源：http://wgb.gzhubu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://xff.zhengqikj.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fyq.hysaishi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uiu.hcnkem.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ifm.ppjwa.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wee.sjlbkw.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gdx.shanyushiyangtech.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ezm.guowangkeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wok.sufxvd.cn

[B02] 多分支 else if / elif
来源：http://kzq.havefunace.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yfv.daxiang520.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bnr.sjlbkw.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://euy.hnxiangtu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blm.cheryme.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kkq.tianlin.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rte.316326.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tbl.tanke756.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://unk.nanxuanxn.top

[B03] switch / match / case
来源：http://qio.hfpthk.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fww.andypj.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://prw.guannengcc.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jlj.yuxming.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://srk.yonumen.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://asd.wangshuangyany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eos.guowangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://axx.redwolf501.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ved.zhijiandao.cn

[B04] for 计数循环
来源：http://yzq.sufxvd.cn

Py:   for i in range(10): print(i)
来源：http://agc.fktsv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jyl.ehwqpu.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lgt.pycfn.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tjq.hongshengwenyu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qys.fktsv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ore.hfpthk.cn

Ruby: 10.times { |i| puts i }
来源：http://gje.yangfankeji.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lwn.quarkkingdee.top

[B05] 遍历数组 / 列表
来源：http://mdz.jianghu66.top

Py:   for item in arr: print(item)
来源：http://wil.gogol.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kiy.zycfv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ewc.ydzc1.top

TS:   for (const item of arr) { console.log(item); }
来源：http://puq.gotoacloud.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://xvr.yueranfly.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://whe.zhoulong.xyz

Ruby: arr.each { |item| puts item }
来源：http://lqf.0kj1m.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eft.smart0.xyz

[B06] 遍历字典 / 对象
来源：http://xft.vehdjk.com

Py:   for k, v in d.items(): print(k, v)
来源：http://sxq.ydzc1.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ujn.ctjpmb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rni.nwbrower.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vod.316326.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://swg.yuxming.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zys.cdnleiting.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xun.zhiwuduotai.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aab.epnwcf.com

[B07] while 循环
来源：http://eap.jqgfzy.top

Py:   while i < 10: i += 1
来源：http://fcq.wangdashe.top

PHP:  while ($i < 10) { $i++; }
来源：http://qlt.tianlin.xyz

JS:   while (i < 10) { i++; }
来源：http://inh.guowangkeji.top

TS:   while (i < 10) { i++; }
来源：http://gpv.svipenyu.cn

Java: while (i < 10) { i++; }
来源：http://inz.guowangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://isl.yuxming.cn

Ruby: while i < 10; i += 1; end
来源：http://ljz.zhengqikj.top

C#:   while (i < 10) { i++; }
来源：http://aln.hfpthk.cn

[B08] do-while（至少执行一次）
来源：http://gyf.gaohongyu789.top

Py:   # 无 do-while：用 while True + break
来源：http://ydd.chenlongwang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ngx.316326.xyz

JS:   do { i++; } while (i < 10);
来源：http://tix.cheryme.top

TS:   do { i++; } while (i < 10);
来源：http://yqn.ydjk.org.cn

Java: do { i++; } while (i < 10);
来源：http://sds.jqgufenzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xyr.jyoumei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ers.wangshuangyany.cn

C#:   do { i++; } while (i < 10);
来源：http://uom.meibo888.top

[B09] break 与 continue
来源：http://rzo.gotoacloud.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vpz.nwbrower.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rnq.zhiwuduotai.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jys.zycfv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qsb.chenlongwang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://chf.xingfuxueyuan.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qso.meibo888.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fai.dianchejie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yea.yongpay.top

[B10] 遍历同时拿索引
来源：http://syk.jinqigfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jdd.gzhubu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ham.jinghuilouyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gkq.jinqigfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hvr.fehbvm.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yfl.ehwqpu.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://skt.kuanghao11.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qmf.meibo888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://glh.jianghu66.top

[B11] 生成数字序列 / 区间
来源：http://qzc.gogol.net.cn

Py:   list(range(0, 10, 2))
来源：http://stk.nanxinkj.top

PHP:  range(0, 10, 2);
来源：http://qxg.nanxuanxn.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xwh.epnwcf.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hiu.cheryme.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nul.daxiang520.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dfw.aibaodan.cn

Ruby: (0...10).step(2).to_a
来源：http://zal.ppjwa.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ptx.haohaochexian.top

[B12] 跳出多层循环
来源：http://jgb.hnxiangtu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://quo.yueranfly.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://pfs.xziqi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://alc.jinghuilouyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aye.yj202588.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xlq.jianghu66.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lmn.birdmap.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jib.zdqjudy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fzi.shuidangran.top

[B13] 判断是否为数字
来源：http://zmr.gotoacloud.top

Py:   isinstance(x, (int, float))
来源：http://yas.zhixingplan.top

PHP:  is_numeric($x)
来源：http://ptg.andypj.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://abo.cheryme.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mql.yj202588.top

Java: x instanceof Number
来源：http://fla.jinqigfzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rog.sjlbkw.cn

Ruby: x.is_a?(Numeric)
来源：http://cit.iojbl.cn

C#:   x is int or double or decimal
来源：http://bvs.zhongyouzk.top

[B14] 判断值是否在集合内
来源：http://kix.birdmap.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kcy.tian-w.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rzm.xinyue.icu

JS:   [1, 2, 3].includes(x)
来源：http://ivs.pycfn.com

TS:   [1, 2, 3].includes(x)
来源：http://dcf.shanyushiyangtech.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nnb.vehdjk.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wmq.jlsjyb.cn

Ruby: [1, 2, 3].include?(x)
来源：http://but.aibaodan.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dkr.hesvh.cn

[B15] 布尔运算与取反
来源：http://ovb.xziqi.cn

Py:   a and b or not c
来源：http://law.svipenyu.cn

PHP:  $a && $b || !$c
来源：http://hsr.fktsv.cn

JS:   a && b || !c
来源：http://tky.jinqigfzy.top

TS:   a && b || !c
来源：http://bfe.wangshuangyany.cn

Java: a && b || !c
来源：http://ras.dashuyun.cn

Go:   a && b || !c
来源：http://yla.aizwys.cn

Ruby: a && b || !c
来源：http://fww.zhongyouzk.top

C#:   a && b || !c
来源：http://osn.yangfankeji.com

[B16] 卫语句：不满足条件提前返回
来源：http://ltn.xinyue.icu

Py:   if not data: return
来源：http://ruu.shzxlz.cn

PHP:  if (!$data) { return; }
来源：http://jdc.hnqzz.top

JS:   if (!data) return;
来源：http://jag.yuxming.cn

TS:   if (!data) return;
来源：http://nno.birdmap.top

Java: if (data == null) return;
来源：http://uoc.cashguo.top

Go:   if data == nil { return }
来源：http://vrx.hongshengwenyu.top

Ruby: return if data.nil?
来源：http://ash.zhongyouzk.top

C#:   if (data == null) return;
来源：http://kmn.wangdashe.top

================================================================================
来源：http://iuw.svipenyu.cn

C. 函数与作用域
来源：http://abr.chenjidiqi.icu

================================================================================
来源：http://ldy.hywenlv.cn

[C01] 定义函数
来源：http://ucm.jiagoushi.top

Py:   def add(a, b): return a + b
来源：http://vxa.birdmap.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yxc.quarkkingdee.top

JS:   function add(a, b) { return a + b; }
来源：http://blj.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xdq.smart0.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://fse.chenzaomai.com

Go:   func add(a, b int) int { return a + b }
来源：http://kqn.yuanzhike.top

Ruby: def add(a, b); a + b; end
来源：http://uhq.yongpay.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bvm.iojbl.cn

[C02] 默认参数
来源：http://srv.kuanghao11.cn

Py:   def greet(name="World"): return name
来源：http://ftd.yj202588.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mun.birdmap.top

JS:   function greet(name = "World") { return name; }
来源：http://lpa.aizwys.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hci.hnqzz.top

Java: // 无默认参数：方法重载或 Optional
来源：http://hvv.shanyushiyangtech.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tkq.xylfe.cn

Ruby: def greet(name = "World") = name
来源：http://nql.sysykeji.top

C#:   string Greet(string name = "World") => name;
来源：http://ebm.yfazqb.com

[C03] 可变参数
来源：http://zjy.jinghuilouyu.cn

Py:   def total(*args): return sum(args)
来源：http://rao.yvedp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vra.snrcjt.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uck.andypj.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bzk.tian-w.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fic.yj20258888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pel.sjlbkw.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mup.hongshengwenyu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zzp.kuanghao11.cn

[C04] 命名参数 / 关键字参数
来源：http://hwv.quarkkingdee.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uba.9152youxi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wpp.c1oappe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iug.c1oappe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hoz.52xcode.cn

Java: // 无：用 Builder 模式或 record
来源：http://eyg.birdmap.top

Go:   // 无：用配置结构体参数
来源：http://kzc.xingfuxueyuan.xyz

Ruby: f(a: 1, b: 2)
来源：http://ejo.yangfankeji.com

C#:   f(a: 1, b: 2)
来源：http://xsn.redwolf501.top

[C05] 返回多个值
来源：http://mpg.uphjek.com

Py:   return a, b
来源：http://pkr.yongpay.top

PHP:  return [$a, $b];
来源：http://myi.ybcxt.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://iqm.snrcjt.cn

TS:   return { a, b };
来源：http://yvw.ywan-chungtsiang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cax.sufxvd.cn

Go:   return a, b
来源：http://czu.guowangkeji.top

Ruby: return a, b
来源：http://kfy.sxryk.cn

C#:   return (a, b);              // ValueTuple
来源：http://afo.zhoulong.xyz

[C06] 匿名函数 / lambda
来源：http://tlg.zhongyouzk.top

Py:   square = lambda x: x * x
来源：http://nzt.pycfn.com

PHP:  $square = fn($x) => $x * $x;
来源：http://bdn.yvedp.cn

JS:   const square = x => x * x;
来源：http://mrl.hesvh.cn

TS:   const square = (x: number): number => x * x;
来源：http://mac.cdnleiting.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fkw.jinqigfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://ngx.xinyue.icu

Ruby: square = ->(x) { x * x }
来源：http://oxk.jinqigufen.top

C#:   Func<int, int> square = x => x * x;
来源：http://hfx.shzxlz.cn

[C07] 把函数作为参数传入
来源：http://xsk.daxiang520.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cnc.yuxming.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wjq.ppjwa.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rla.guannengcc.top

TS:   arr.map(String)
来源：http://jpd.c1oappe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hez.pengpengdd.cyou

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jsa.xylfe.cn

Ruby: arr.map(&:upcase)
来源：http://qpu.sufxvd.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jxy.tarul.cn

[C08] 闭包
来源：http://eog.yueranfly.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zyz.fengsongda.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ohc.sweek.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oze.kuanghao11.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://iqi.hammf.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://osg.hongshengwenyu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rwy.zdbjq.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dam.bbcook.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lfd.zhiwuduotai.top

[C09] 递归
来源：http://xcm.jiagoushi.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nec.hcnkem.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qdy.gotoacloud.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lum.ppjwa.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gxr.iojbl.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ifb.c1oappe.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iem.zhijiandao.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://utc.ppjwa.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uyu.xinyue.icu

[C10] 变量作用域
来源：http://gle.shzxlz.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vjs.hnxiangtu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://znn.sufxvd.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vmp.meibo888.top

TS:   同 JS
来源：http://mnd.pengpengdd.cyou

Java: 方法内为块级作用域
来源：http://drq.fengsongda.top

Go:   花括号块级作用域
来源：http://rvz.wangdashe.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ltw.hammf.cn

C#:   块级作用域
来源：http://fxk.xuanzx.com

[C11] 模块导入与导出
来源：http://etp.zdbjq.cn

Py:   from module import func
来源：http://xvy.jiagoushi.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qua.nanxinkj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xzs.yj20258.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xvy.zhaomingkeji.xyz

Java: import java.util.List;
来源：http://vgb.zhoulong.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nrk.nanxinkj.top

Ruby: require "json"; require_relative "./util"
来源：http://gqu.fengsongda.top

C#:   using System.Text;
来源：http://vnb.zdqjudy.top

[C12] 立即执行函数 IIFE
来源：http://inm.chenlongwang.top

Py:   (lambda: print("run"))()
来源：http://bnm.yonumen.top

PHP:  (function () { echo "run"; })();
来源：http://jxm.yvedp.cn

JS:   (() => { console.log("run"); })();
来源：http://njp.jyoumei.cn

TS:   (() => { console.log("run"); })();
来源：http://bto.yonumen.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bwd.fehbvm.com

Go:   func() { fmt.Println("run") }()
来源：http://vbw.jyoumei.cn

Ruby: -> { puts "run" }.call
来源：http://bnx.0kj1m.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pnp.ydzc1.top

[C13] 类型声明 / 类型注解
来源：http://uec.xinyue.icu

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zvs.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ywg.bjfxy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nbo.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qdi.bbcook.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jrc.svipenyu.cn

Go:   func add(a, b int) int
来源：http://ety.sysykeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xsz.c1oappe.top

C#:   int Add(int a, int b) => a + b;
来源：http://opv.yongpay.top

[C14] 泛型函数
来源：http://sxi.guowangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://crz.gaohongyu789.top

PHP:  // 无泛型
来源：http://rui.yonumen.top

JS:   // 无泛型
来源：http://deh.yangfankeji.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mxb.xuanzx.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hni.zdqjudy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cbi.smart0.xyz

Ruby: # 无泛型
来源：http://zig.cashguo.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tcb.zhongyouzk.top

[C15] 解构 / 展开参数
来源：http://kmn.cheryme.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gmz.sufxvd.cn

PHP:  [$a, $b] = $pair;
来源：http://yiw.shanyushiyangtech.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ryc.zhengqikj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mkk.ehwqpu.com

Java: // 无解构
来源：http://pzu.hnxiangtu.top

Go:   // 无解构
来源：http://tvq.tianlin.xyz


<!-- 参考信息 -->