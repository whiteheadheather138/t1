代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mha.aizwys.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sus.epnwcf.com

Ruby: s1 == s2; s1 <=> s2
来源：http://wet.yj202588.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cyk.sxryk.cn

[A26] 类型转换总览
来源：http://phe.uphjek.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jff.pengpengdd.cyou

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://oif.ywan-chungtsiang.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fqs.c1oappe.top

TS:   Number() String() Boolean() x as number
来源：http://ber.bbcook.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gdq.ehwqpu.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sif.shanyushiyangkeji.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ojs.jianghu66.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tsx.zhengqikj.top

================================================================================
来源：http://scf.chenzaomai.com

B. 流程控制
来源：http://zki.9152youxi.cn

================================================================================
来源：http://hjs.cucudq.cn

[B01] 条件判断 if / else
来源：http://fmk.bjfxy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://lsm.fengsongda.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://onx.hongshengwenyu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cvr.chenzaomai.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://evd.daxiang520.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://fte.gzhubu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tdh.jqgfzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kni.ywan-chungtsiang.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://clu.fengsongda.top

[B02] 多分支 else if / elif
来源：http://bgg.zhijiandao.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vmt.zycfv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ibg.chenzaomai.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mot.shanyushiyangtech.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nha.aizwys.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gqa.zhoulong.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zdk.sufxvd.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jxz.xuanzx.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://znl.ppjwa.cn

[B03] switch / match / case
来源：http://mjw.yangfankeji.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jok.zdbjq.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kxm.cdnleiting.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zpj.andypj.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jmd.hcnkem.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qyn.jinqigufen.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zlp.daxiang520.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ufe.fehbvm.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tdv.kuanghao11.cn

[B04] for 计数循环
来源：http://pdk.tian-w.cn

Py:   for i in range(10): print(i)
来源：http://kdj.jyoumei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://exi.smart0.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jhe.pengpengdd.cyou

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sgr.yueranfly.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gxf.bjfxy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://msg.wangdashe.top

Ruby: 10.times { |i| puts i }
来源：http://nel.yonumen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://avh.fengsongda.top

[B05] 遍历数组 / 列表
来源：http://bzc.cdnleiting.top

Py:   for item in arr: print(item)
来源：http://bfi.zhijiandao.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pjw.zhengqikj.top

JS:   for (const item of arr) { console.log(item); }
来源：http://gtc.ivvv.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ejq.shanyushiyangtech.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ept.zdqjudy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iia.birdmap.top

Ruby: arr.each { |item| puts item }
来源：http://eog.feifeiyinyue.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mcw.zhaomingkeji.xyz

[B06] 遍历字典 / 对象
来源：http://yzo.aizwys.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yzl.hcnkem.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://eqo.vqdsnc.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vfq.hesvh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://idx.bbcook.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rox.gaohongyu789.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://puu.yj20258.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mgp.yuxming.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gje.zhengqikj.top

[B07] while 循环
来源：http://vbi.daria6918.cn

Py:   while i < 10: i += 1
来源：http://ckb.gotoacloud.top

PHP:  while ($i < 10) { $i++; }
来源：http://jsq.9152youxi.cn

JS:   while (i < 10) { i++; }
来源：http://luq.xuetiantiany.cn

TS:   while (i < 10) { i++; }
来源：http://qrb.52xcode.cn

Java: while (i < 10) { i++; }
来源：http://lco.chenlongwang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lun.yanxiufei.cn

Ruby: while i < 10; i += 1; end
来源：http://rvo.meibo888.top

C#:   while (i < 10) { i++; }
来源：http://gib.gotoacloud.top

[B08] do-while（至少执行一次）
来源：http://lib.zycfv.cn

Py:   # 无 do-while：用 while True + break
来源：http://viv.zhijiandao.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://uhj.yj202588.top

JS:   do { i++; } while (i < 10);
来源：http://noi.ppjwa.cn

TS:   do { i++; } while (i < 10);
来源：http://gzr.aibaodan.cn

Java: do { i++; } while (i < 10);
来源：http://xux.nanxinkj.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xae.shanyushiyangkeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://mfg.daria6918.cn

C#:   do { i++; } while (i < 10);
来源：http://gsa.shuidangran.top

[B09] break 与 continue
来源：http://rqr.cdnleiting.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fry.sysykeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lbk.ywan-chungtsiang.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ymu.vqdsnc.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sss.9152youxi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://woj.sufxvd.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jbt.hnxiangtu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aer.ydzc1.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oyu.aizwys.cn

[B10] 遍历同时拿索引
来源：http://afk.sweek.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zpx.cdnleiting.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://amx.hysaishi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://roi.vehdjk.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fjd.yj202588.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lep.tian-w.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pmk.quarkkingdee.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hhh.zycfv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yrx.jinqigufen.top

[B11] 生成数字序列 / 区间
来源：http://omj.c1oappe.top

Py:   list(range(0, 10, 2))
来源：http://dzl.cqqwz.cn

PHP:  range(0, 10, 2);
来源：http://fms.hnxiangtu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ann.xuanzx.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ulp.ctjpmb.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dwt.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bib.nwbrower.top

Ruby: (0...10).step(2).to_a
来源：http://dle.jiagoushi.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wfa.daria6918.cn

[B12] 跳出多层循环
来源：http://wia.sxryk.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mdn.jinqigufen.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lic.tarul.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nrl.yonumen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ytn.yfazqb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qsm.tian-w.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://iyk.yj20258888.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fhl.shangyingyoupin.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lmo.ybcxt.top

[B13] 判断是否为数字
来源：http://bbk.smart0.xyz

Py:   isinstance(x, (int, float))
来源：http://rni.yonumen.top

PHP:  is_numeric($x)
来源：http://pqo.shanyushiyangtech.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ijw.guowangkeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ckw.cheryme.top

Java: x instanceof Number
来源：http://ivk.shangyingyoupin.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sib.redwolf501.top

Ruby: x.is_a?(Numeric)
来源：http://pmg.yfazqb.com

C#:   x is int or double or decimal
来源：http://ymc.ivvv.top

[B14] 判断值是否在集合内
来源：http://igt.wangdashe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bet.tanke756.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dwr.jianghu66.top

JS:   [1, 2, 3].includes(x)
来源：http://icv.daria6918.cn

TS:   [1, 2, 3].includes(x)
来源：http://stu.yongpay.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pdq.shanyushiyangtech.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ofd.yuanzhike.top

Ruby: [1, 2, 3].include?(x)
来源：http://dlt.sysykeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pfu.sxryk.cn

[B15] 布尔运算与取反
来源：http://ofd.daxiang520.top

Py:   a and b or not c
来源：http://kka.hcnkem.com

PHP:  $a && $b || !$c
来源：http://pnr.xinyue.icu

JS:   a && b || !c
来源：http://jya.haohaochexian.top

TS:   a && b || !c
来源：http://tly.snrcjt.cn

Java: a && b || !c
来源：http://kyu.xingfuxueyuan.xyz

Go:   a && b || !c
来源：http://ffv.pycfn.com

Ruby: a && b || !c
来源：http://osg.sysykeji.top

C#:   a && b || !c
来源：http://gii.jiagoushi.top

[B16] 卫语句：不满足条件提前返回
来源：http://mdu.zycfv.cn

Py:   if not data: return
来源：http://sii.yfazqb.com

PHP:  if (!$data) { return; }
来源：http://sjc.316326.xyz

JS:   if (!data) return;
来源：http://pqo.zhixingplan.top

TS:   if (!data) return;
来源：http://bsd.zycfv.cn

Java: if (data == null) return;
来源：http://dkq.wangshuangyany.cn

Go:   if data == nil { return }
来源：http://utw.cqqwz.cn

Ruby: return if data.nil?
来源：http://jxz.yj20258888.top

C#:   if (data == null) return;
来源：http://pgt.feifeiyinyue.top

================================================================================
来源：http://swz.chenjidiqi.icu

C. 函数与作用域
来源：http://anz.shangyingyoupin.top

================================================================================
来源：http://ttr.daxiang520.top

[C01] 定义函数
来源：http://lpg.wangshuangyany.cn

Py:   def add(a, b): return a + b
来源：http://wtn.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nim.iojbl.cn

JS:   function add(a, b) { return a + b; }
来源：http://jpb.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kkw.tanke756.top

Java: static int add(int a, int b) { return a + b; }
来源：http://pgv.kuanghao11.cn

Go:   func add(a, b int) int { return a + b }
来源：http://epz.xuetiantiany.cn

Ruby: def add(a, b); a + b; end
来源：http://jkc.redwolf501.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mnn.zhoulong.xyz

[C02] 默认参数
来源：http://ppm.bbcook.cn

Py:   def greet(name="World"): return name
来源：http://owv.daria6918.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://knn.cucudq.cn

JS:   function greet(name = "World") { return name; }
来源：http://fkp.nanxinkj.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jwb.hcnkem.com

Java: // 无默认参数：方法重载或 Optional
来源：http://lpy.jiagoushi.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gey.ehwqpu.com

Ruby: def greet(name = "World") = name
来源：http://lnb.zhijiandao.cn

C#:   string Greet(string name = "World") => name;
来源：http://dvx.zdqjudy.top

[C03] 可变参数
来源：http://qhv.gotoacloud.top

Py:   def total(*args): return sum(args)
来源：http://jxg.shzxlz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yrz.jinghuilouyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://shv.nanxuanxn.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lrp.jianghu66.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qsg.pycfn.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dvf.pengpengdd.cyou

Ruby: def total(*nums); nums.sum; end
来源：http://vua.cucudq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vyj.birdmap.top

[C04] 命名参数 / 关键字参数
来源：http://eij.jqgufenzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tgf.ctjpmb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zgi.guannengcc.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tkn.bbcook.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://org.hongshengwenyu.top

Java: // 无：用 Builder 模式或 record
来源：http://ite.cqqwz.cn

Go:   // 无：用配置结构体参数
来源：http://suc.guannengcc.top

Ruby: f(a: 1, b: 2)
来源：http://tvw.zycfv.cn

C#:   f(a: 1, b: 2)
来源：http://woy.jqgufenzy.top

[C05] 返回多个值
来源：http://nkv.zdqjudy.top

Py:   return a, b
来源：http://yom.zhengqikj.top

PHP:  return [$a, $b];
来源：http://zjy.zdbjq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xgj.yuxming.cn

TS:   return { a, b };
来源：http://wjx.ctjpmb.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xxl.zdqjudy.top

Go:   return a, b
来源：http://klu.shanyushiyangkeji.top

Ruby: return a, b
来源：http://ola.smart0.xyz

C#:   return (a, b);              // ValueTuple
来源：http://pcf.nanxuanxn.top

[C06] 匿名函数 / lambda
来源：http://kbw.jyoumei.cn

Py:   square = lambda x: x * x
来源：http://eol.c1oappe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zyp.chenjidiqi.icu

JS:   const square = x => x * x;
来源：http://mjg.zycfv.cn

TS:   const square = (x: number): number => x * x;
来源：http://rjm.xingfuxueyuan.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rnb.dashuyun.cn

Go:   sq := func(x int) int { return x * x }
来源：http://axw.haohaochexian.top

Ruby: square = ->(x) { x * x }
来源：http://ovw.yj202588.top

C#:   Func<int, int> square = x => x * x;
来源：http://lmi.zhengqikj.top

[C07] 把函数作为参数传入
来源：http://xcm.zycfv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gkw.hnqzz.top

PHP:  array_map("strtoupper", $arr);
来源：http://fty.jinghuilouyu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ppl.ehwqpu.com

TS:   arr.map(String)
来源：http://kca.sxryk.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qkj.sysykeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://iop.zhijiandao.cn

Ruby: arr.map(&:upcase)
来源：http://jml.sweek.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wuz.hesvh.cn

[C08] 闭包
来源：http://kqd.yj202588.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xcb.zhixingplan.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rbg.gzhubu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qxf.cdnleiting.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xrs.birdmap.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gav.hesvh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tzs.ydjk.org.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wmb.aizwys.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dfm.hcnkem.com

[C09] 递归
来源：http://ybr.hammf.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jjt.guowangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://znk.zhijiandao.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qre.316326.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ucq.aizwys.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zcu.yuxming.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vxu.hammf.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tuf.hammf.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sgy.svipenyu.cn

[C10] 变量作用域
来源：http://fta.ywan-chungtsiang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://suu.mhx1999.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kdo.cucudq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uem.zhongyouzk.top

TS:   同 JS
来源：http://pvk.xingfuxueyuan.xyz

Java: 方法内为块级作用域
来源：http://kdz.ivvv.top

Go:   花括号块级作用域
来源：http://shr.xziqi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bkd.yvedp.cn

C#:   块级作用域
来源：http://uzr.cucudq.cn

[C11] 模块导入与导出
来源：http://nra.fktsv.cn

Py:   from module import func
来源：http://unm.feifeiyinyue.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ycr.shuidangran.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://afu.zdqjudy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ntj.xinyue.icu

Java: import java.util.List;
来源：http://czu.havefunace.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ugp.sxryk.cn

Ruby: require "json"; require_relative "./util"
来源：http://evg.cucudq.cn

C#:   using System.Text;
来源：http://rib.hcnkem.com

[C12] 立即执行函数 IIFE
来源：http://xqd.daxiang520.top

Py:   (lambda: print("run"))()
来源：http://kuk.0kj1m.cn

PHP:  (function () { echo "run"; })();
来源：http://xcz.cdnleiting.top

JS:   (() => { console.log("run"); })();
来源：http://ssu.quarkkingdee.top

TS:   (() => { console.log("run"); })();
来源：http://ayp.tianlin.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tbp.sysykeji.top

Go:   func() { fmt.Println("run") }()
来源：http://msy.jlsjyb.cn

Ruby: -> { puts "run" }.call
来源：http://wrr.cdnleiting.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dvn.cashguo.top

[C13] 类型声明 / 类型注解
来源：http://xmx.ydjk.org.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ult.nwbrower.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nux.xinyue.icu

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gfb.gotoacloud.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://obv.hcnkem.com

Java: int add(int a, int b) { return a + b; }
来源：http://kkr.hnqzz.top

Go:   func add(a, b int) int
来源：http://rfh.hongshengwenyu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bgk.chenzaomai.com

C#:   int Add(int a, int b) => a + b;
来源：http://aod.yueranfly.top

[C14] 泛型函数
来源：http://ppb.vehdjk.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uzt.ywan-chungtsiang.top

PHP:  // 无泛型
来源：http://nfg.kuanghao11.cn

JS:   // 无泛型
来源：http://kww.tarul.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fnb.nwbrower.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tji.9152youxi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mrs.yj202588.top

Ruby: # 无泛型
来源：http://psp.gogol.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dwm.kuanghao11.cn

[C15] 解构 / 展开参数
来源：http://nth.ehwqpu.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://goj.sxryk.cn

PHP:  [$a, $b] = $pair;
来源：http://slt.sweek.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tlz.xinyue.icu

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qax.yvedp.cn

Java: // 无解构
来源：http://sps.jlsjyb.cn

Go:   // 无解构
来源：http://hyo.vqdsnc.cn

Ruby: a, b = pair
来源：http://vpr.zhongyouzk.top

C#:   var (a, b) = pair;
来源：http://idn.hesvh.cn

[C16] 函数 / 方法重载
来源：http://atg.dianchejie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gff.guannengcc.top


<!-- 参考信息 -->