代发 wailian999

[A26] 类型转换总览
来源：http://xlm.zycfv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qci.nanxinkj.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hfz.shzxlz.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bro.yongpay.top

TS:   Number() String() Boolean() x as number
来源：http://rwf.shuidangran.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qpt.meibo888.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wci.yonumen.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://gmn.jinyuanbaomall.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cwd.dianchejie.cn

================================================================================
来源：http://arq.zdqjudy.top

B. 流程控制
来源：http://jxa.xylfe.cn

================================================================================
来源：http://zij.hfpthk.cn

[B01] 条件判断 if / else
来源：http://ntv.0kj1m.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dfx.chenjidiqi.icu

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fhl.jqgufenzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cqd.xingfuxueyuan.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jbv.zhiwuduotai.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://fkp.uphjek.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://btr.yvedp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cam.sjlbkw.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ngt.yuxming.cn

[B02] 多分支 else if / elif
来源：http://epq.ydjk.org.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vhd.zycfv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zns.yuanzhike.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://voa.ctjpmb.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fpa.bbcook.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ekc.zhijiandao.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rqh.svipenyu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://irl.gogol.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jyu.haohaochexian.top

[B03] switch / match / case
来源：http://mrn.zhengqikj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zqc.zdqjudy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nqp.zycfv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sgs.yanxiufei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qvw.havefunace.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dff.yonumen.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mqy.bbcook.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lbx.dashuyun.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fno.xingfuxueyuan.xyz

[B04] for 计数循环
来源：http://yym.316326.xyz

Py:   for i in range(10): print(i)
来源：http://aul.shzxlz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dvp.guowangkeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tvu.bbcook.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vfr.redwolf501.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bia.quarkkingdee.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://idy.jianghu66.top

Ruby: 10.times { |i| puts i }
来源：http://udg.quarkkingdee.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zya.fehbvm.com

[B05] 遍历数组 / 列表
来源：http://dsh.hammf.cn

Py:   for item in arr: print(item)
来源：http://wcv.fehbvm.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://clu.cqqwz.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fkg.guannengcc.top

TS:   for (const item of arr) { console.log(item); }
来源：http://arw.shanyushiyangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://gdw.pengpengdd.cyou

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ygt.yonumen.top

Ruby: arr.each { |item| puts item }
来源：http://umw.hcnkem.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://com.vehdjk.com

[B06] 遍历字典 / 对象
来源：http://que.nanxuanxn.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xly.haohaochexian.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ncr.bbcook.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://von.zycfv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sgc.hnqzz.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ewr.pycfn.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qdm.nwbrower.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jqy.zhiwuduotai.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mdd.daria6918.cn

[B07] while 循环
来源：http://zhs.quarkkingdee.top

Py:   while i < 10: i += 1
来源：http://uhq.jiagoushi.top

PHP:  while ($i < 10) { $i++; }
来源：http://wzn.quarkkingdee.top

JS:   while (i < 10) { i++; }
来源：http://brk.52xcode.cn

TS:   while (i < 10) { i++; }
来源：http://nnx.cucudq.cn

Java: while (i < 10) { i++; }
来源：http://lxf.ctjpmb.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vvo.meibo888.top

Ruby: while i < 10; i += 1; end
来源：http://avy.xylfe.cn

C#:   while (i < 10) { i++; }
来源：http://qbr.jqgufenzy.top

[B08] do-while（至少执行一次）
来源：http://uub.fanxiaobao.xyz

Py:   # 无 do-while：用 while True + break
来源：http://txh.yonumen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://acp.bbcook.cn

JS:   do { i++; } while (i < 10);
来源：http://vcf.ydzc1.top

TS:   do { i++; } while (i < 10);
来源：http://xon.ydzc1.top

Java: do { i++; } while (i < 10);
来源：http://ppl.yonumen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bbj.sufxvd.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qib.vqdsnc.cn

C#:   do { i++; } while (i < 10);
来源：http://oqj.shuidangran.top

[B09] break 与 continue
来源：http://vjh.dashuyun.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bcz.tian-w.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cnb.sjlbkw.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://elj.aizwys.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ntr.ydjk.org.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://asx.jinqigufen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jrj.zhijiandao.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pga.zycfv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://drw.nanxinkj.top

[B10] 遍历同时拿索引
来源：http://kea.fktsv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jgl.gogol.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xgn.zhijiandao.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xxc.hongshengwenyu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fae.haohaochexian.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xtm.zhixingplan.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sgi.nanxuanxn.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bri.pycfn.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sgt.zhixingplan.top

[B11] 生成数字序列 / 区间
来源：http://plm.nanxuanxn.top

Py:   list(range(0, 10, 2))
来源：http://tcd.epnwcf.com

PHP:  range(0, 10, 2);
来源：http://ghh.jyoumei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zqo.smart0.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://krj.iojbl.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ydk.hnqzz.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ejd.jlsjyb.cn

Ruby: (0...10).step(2).to_a
来源：http://rgu.uphjek.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://htt.shzxlz.cn

[B12] 跳出多层循环
来源：http://eig.xylfe.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://peg.xingfuxueyuan.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://wex.yueranfly.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://joi.fanxiaobao.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zjs.sxryk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tnj.ivvv.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nhu.meibo888.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uxr.fzhhl.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ete.yj20258888.top

[B13] 判断是否为数字
来源：http://xjo.nanxinkj.top

Py:   isinstance(x, (int, float))
来源：http://ssf.cqqwz.cn

PHP:  is_numeric($x)
来源：http://yoy.52xcode.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fvb.fktsv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gyz.chenjidiqi.icu

Java: x instanceof Number
来源：http://osy.jinyuanbaomall.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rgi.jqgufenzy.top

Ruby: x.is_a?(Numeric)
来源：http://roz.tian-w.cn

C#:   x is int or double or decimal
来源：http://mzj.cheryme.top

[B14] 判断值是否在集合内
来源：http://qge.daria6918.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gis.daxiang520.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yxg.jyoumei.cn

JS:   [1, 2, 3].includes(x)
来源：http://pvp.hnxiangtu.top

TS:   [1, 2, 3].includes(x)
来源：http://azn.fzhhl.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zvq.ivvv.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wjt.sxryk.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ark.sxryk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bmx.bbcook.cn

[B15] 布尔运算与取反
来源：http://uxw.feifeiyinyue.top

Py:   a and b or not c
来源：http://bda.ivvv.top

PHP:  $a && $b || !$c
来源：http://pwp.zhongyouzk.top

JS:   a && b || !c
来源：http://vxh.zycfv.cn

TS:   a && b || !c
来源：http://qli.ivvv.top

Java: a && b || !c
来源：http://rcb.pengpengdd.cyou

Go:   a && b || !c
来源：http://pbx.9152youxi.cn

Ruby: a && b || !c
来源：http://xpo.shangyingyoupin.top

C#:   a && b || !c
来源：http://eau.ydzc1.top

[B16] 卫语句：不满足条件提前返回
来源：http://rcl.xziqi.cn

Py:   if not data: return
来源：http://fpf.xinyue.icu

PHP:  if (!$data) { return; }
来源：http://hqb.xuetiantiany.cn

JS:   if (!data) return;
来源：http://kuf.yueranfly.top

TS:   if (!data) return;
来源：http://dhg.ivvv.top

Java: if (data == null) return;
来源：http://zjx.zhijiandao.cn

Go:   if data == nil { return }
来源：http://cho.ydzc1.top

Ruby: return if data.nil?
来源：http://iku.ppjwa.cn

C#:   if (data == null) return;
来源：http://bri.hywenlv.cn

================================================================================
来源：http://ucv.yangfankeji.com

C. 函数与作用域
来源：http://urg.sjlbkw.cn

================================================================================
来源：http://fjr.ppjwa.cn

[C01] 定义函数
来源：http://okj.yfazqb.com

Py:   def add(a, b): return a + b
来源：http://fvv.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qwf.tanke756.top

JS:   function add(a, b) { return a + b; }
来源：http://yza.0kj1m.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kpl.hywenlv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ays.cucudq.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cst.xuanzx.com

Ruby: def add(a, b); a + b; end
来源：http://rck.daria6918.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vtr.mhx1999.top

[C02] 默认参数
来源：http://gnz.hesvh.cn

Py:   def greet(name="World"): return name
来源：http://kgr.hnqzz.top

PHP:  function greet($name = "World") { return $name; }
来源：http://azg.gzhubu.top

JS:   function greet(name = "World") { return name; }
来源：http://wpd.sjlbkw.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wvv.yueranfly.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xhv.0kj1m.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ewt.vehdjk.com

Ruby: def greet(name = "World") = name
来源：http://caq.hfpthk.cn

C#:   string Greet(string name = "World") => name;
来源：http://moa.andypj.xyz

[C03] 可变参数
来源：http://ejg.ehwqpu.com

Py:   def total(*args): return sum(args)
来源：http://ese.zhongyouzk.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gih.shanyushiyangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://emy.hywenlv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vko.xingfuxueyuan.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://glv.sxryk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wix.shanyushiyangkeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://gyh.jlsjyb.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vuw.ppjwa.cn

[C04] 命名参数 / 关键字参数
来源：http://yzx.zhixingplan.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bbi.pycfn.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cnn.wangdashe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qsv.fktsv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tfs.quarkkingdee.top

Java: // 无：用 Builder 模式或 record
来源：http://syg.jianghu66.top

Go:   // 无：用配置结构体参数
来源：http://txm.hywenlv.cn

Ruby: f(a: 1, b: 2)
来源：http://bqk.jianghu66.top

C#:   f(a: 1, b: 2)
来源：http://pav.cqqwz.cn

[C05] 返回多个值
来源：http://wco.0kj1m.cn

Py:   return a, b
来源：http://jiv.mhx1999.top

PHP:  return [$a, $b];
来源：http://muw.chenzaomai.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://hmi.ybcxt.top

TS:   return { a, b };
来源：http://grq.bjfxy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://abf.tarul.cn

Go:   return a, b
来源：http://lsf.tarul.cn

Ruby: return a, b
来源：http://rpa.cdnleiting.top

C#:   return (a, b);              // ValueTuple
来源：http://fut.yuxming.cn

[C06] 匿名函数 / lambda
来源：http://ezw.zhengqikj.top

Py:   square = lambda x: x * x
来源：http://lei.zhijiandao.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mqi.cheryme.top

JS:   const square = x => x * x;
来源：http://wuz.ybcxt.top

TS:   const square = (x: number): number => x * x;
来源：http://xta.shzxlz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wxl.jinyuanbaomall.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lud.jqgfzy.top

Ruby: square = ->(x) { x * x }
来源：http://eyj.vehdjk.com

C#:   Func<int, int> square = x => x * x;
来源：http://clm.nanxuanxn.top

[C07] 把函数作为参数传入
来源：http://wzs.xuetiantiany.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dft.ydjk.org.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ekq.tanke756.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rdn.tarul.cn

TS:   arr.map(String)
来源：http://ktf.zhixingplan.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qoh.aibaodan.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vax.yj202588.top

Ruby: arr.map(&:upcase)
来源：http://imb.ydjk.org.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qwm.yj202588.top

[C08] 闭包
来源：http://ouq.aizwys.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dnv.vehdjk.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://imy.shzxlz.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://njv.nwbrower.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://krc.xinyue.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://may.zdqjudy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://urn.9152youxi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lha.gotoacloud.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hem.hcnkem.com

[C09] 递归
来源：http://rrs.birdmap.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://czy.andypj.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mbn.dashuyun.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ppx.zhoulong.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://otr.feifeiyinyue.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xwc.guannengcc.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wlh.fktsv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mda.xuanzx.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nsc.fehbvm.com

[C10] 变量作用域
来源：http://kit.ydzc1.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ayc.feifeiyinyue.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://quo.pycfn.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cnr.cdnleiting.top

TS:   同 JS
来源：http://lck.sxryk.cn

Java: 方法内为块级作用域
来源：http://tfm.zhiwuduotai.top

Go:   花括号块级作用域
来源：http://msf.quarkkingdee.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://skj.snrcjt.cn

C#:   块级作用域
来源：http://akn.vehdjk.com

[C11] 模块导入与导出
来源：http://uol.cucudq.cn

Py:   from module import func
来源：http://zov.bbcook.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vxu.wangshuangyany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://noz.yuanzhike.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qkc.cheryme.top

Java: import java.util.List;
来源：http://azh.cheryme.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kgo.c1oappe.top

Ruby: require "json"; require_relative "./util"
来源：http://pgh.cdnleiting.top

C#:   using System.Text;
来源：http://aiy.nwbrower.top

[C12] 立即执行函数 IIFE
来源：http://svj.fehbvm.com

Py:   (lambda: print("run"))()
来源：http://ciw.xuanzx.com

PHP:  (function () { echo "run"; })();
来源：http://skb.sxryk.cn

JS:   (() => { console.log("run"); })();
来源：http://lux.wangshuangyany.cn

TS:   (() => { console.log("run"); })();
来源：http://osl.sysykeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qms.smart0.xyz

Go:   func() { fmt.Println("run") }()
来源：http://vuc.yuanzhike.top

Ruby: -> { puts "run" }.call
来源：http://rvl.xuanzx.com

C#:   // 无 IIFE：用静态构造函数
来源：http://pak.dashuyun.cn

[C13] 类型声明 / 类型注解
来源：http://bzv.shangyingyoupin.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qdw.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xnh.yj202588.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nid.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://roz.yonumen.top

Java: int add(int a, int b) { return a + b; }
来源：http://bbj.gogol.net.cn

Go:   func add(a, b int) int
来源：http://qzy.xziqi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lxs.fehbvm.com

C#:   int Add(int a, int b) => a + b;
来源：http://cyh.hysaishi.cn

[C14] 泛型函数
来源：http://ble.sweek.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uni.fzhhl.top

PHP:  // 无泛型
来源：http://qjh.jyoumei.cn

JS:   // 无泛型
来源：http://erb.zhixingplan.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://iag.daria6918.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rxi.sysykeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ahp.hnqzz.top

Ruby: # 无泛型
来源：http://nqb.smart0.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yfk.jinyuanbaomall.cn

[C15] 解构 / 展开参数
来源：http://cgj.chenjidiqi.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bni.hcnkem.com

PHP:  [$a, $b] = $pair;
来源：http://ktq.gzhubu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gut.hywenlv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mrd.wangdashe.top

Java: // 无解构
来源：http://dfq.nanxinkj.top

Go:   // 无解构
来源：http://kmh.svipenyu.cn

Ruby: a, b = pair
来源：http://vjx.wangdashe.top

C#:   var (a, b) = pair;
来源：http://yzn.tian-w.cn

[C16] 函数 / 方法重载
来源：http://bes.shuidangran.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://muh.hesvh.cn

PHP:  // 无重载
来源：http://shx.zhoulong.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://pwg.tianlin.xyz

TS:   // 用联合类型或重载签名声明
来源：http://gdt.tanke756.top

Java: void f(int a) {}  void f(String a) {}
来源：http://uyn.guowangkeji.top


<!-- 参考信息 -->