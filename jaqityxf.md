代发 wailian999

[A26] 类型转换总览
来源：http://xgt.jinqigufen.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://che.hfpthk.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ewm.cdnleiting.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ynk.svipenyu.cn

TS:   Number() String() Boolean() x as number
来源：http://jjn.jiagoushi.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cfv.jqgfzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zfx.yvedp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://egj.jlsjyb.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://abx.fehbvm.com

================================================================================
来源：http://ciw.gzhubu.top

B. 流程控制
来源：http://miw.iojbl.cn

================================================================================
来源：http://zvb.hongshengwenyu.top

[B01] 条件判断 if / else
来源：http://jyt.yj20258888.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ecq.hnxiangtu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dhv.yj20258888.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hur.hnxiangtu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ihh.tian-w.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://foq.shangyingyoupin.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hwe.zdqjudy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://acz.aizwys.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qqq.birdmap.top

[B02] 多分支 else if / elif
来源：http://rmg.wangdashe.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hwu.bbcook.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eli.c1oappe.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gwe.nwbrower.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lgp.birdmap.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cqa.wangshuangyany.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zjp.hcnkem.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jfn.dashuyun.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bil.yuxming.cn

[B03] switch / match / case
来源：http://mhp.jqgufenzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://eve.iojbl.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kpk.jinyuanbaomall.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ytf.jyoumei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zxk.pengpengdd.cyou

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jre.zhiwuduotai.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xvo.shanyushiyangtech.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://flk.gaohongyu789.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vqj.quarkkingdee.top

[B04] for 计数循环
来源：http://btk.ywan-chungtsiang.top

Py:   for i in range(10): print(i)
来源：http://isf.bbcook.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://egq.zhongyouzk.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cqe.shuidangran.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dru.vqdsnc.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dop.epnwcf.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bba.yuxming.cn

Ruby: 10.times { |i| puts i }
来源：http://rcu.svipenyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://usy.yonumen.top

[B05] 遍历数组 / 列表
来源：http://eat.xingfuxueyuan.xyz

Py:   for item in arr: print(item)
来源：http://wtu.fanxiaobao.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hyx.gogol.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gpg.uphjek.com

TS:   for (const item of arr) { console.log(item); }
来源：http://sas.uphjek.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://aku.snrcjt.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iyd.bjfxy.top

Ruby: arr.each { |item| puts item }
来源：http://ltq.guowangkeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zqh.pycfn.com

[B06] 遍历字典 / 对象
来源：http://gze.52xcode.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fih.hnqzz.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://txd.aizwys.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zas.yangfankeji.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dow.jinqigufen.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://akd.zdqjudy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jdn.jianghu66.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dup.gotoacloud.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jzm.jqgfzy.top

[B07] while 循环
来源：http://ldv.sufxvd.cn

Py:   while i < 10: i += 1
来源：http://gmj.shzxlz.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tbv.ydzc1.top

JS:   while (i < 10) { i++; }
来源：http://pfw.epnwcf.com

TS:   while (i < 10) { i++; }
来源：http://wpj.nwbrower.top

Java: while (i < 10) { i++; }
来源：http://gea.ehwqpu.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tju.tianlin.xyz

Ruby: while i < 10; i += 1; end
来源：http://kyj.hnxiangtu.top

C#:   while (i < 10) { i++; }
来源：http://dqn.cqqwz.cn

[B08] do-while（至少执行一次）
来源：http://vme.jinyuanbaomall.cn

Py:   # 无 do-while：用 while True + break
来源：http://siy.jianghu66.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kby.birdmap.top

JS:   do { i++; } while (i < 10);
来源：http://zkz.sysykeji.top

TS:   do { i++; } while (i < 10);
来源：http://obe.nwbrower.top

Java: do { i++; } while (i < 10);
来源：http://rwj.xingfuxueyuan.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://clm.aizwys.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sbw.hfpthk.cn

C#:   do { i++; } while (i < 10);
来源：http://soc.xuetiantiany.cn

[B09] break 与 continue
来源：http://kak.nanxinkj.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hxn.yj20258.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ysp.zhiwuduotai.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dji.hysaishi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://igf.ybcxt.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kpc.zhongyouzk.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eyc.aibaodan.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xqm.yfazqb.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xhi.zycfv.cn

[B10] 遍历同时拿索引
来源：http://xvp.ehwqpu.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mrg.zhengqikj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ilx.hongshengwenyu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ntr.sufxvd.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://twj.cdnleiting.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kgt.jqgfzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tsu.chenzaomai.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rct.snrcjt.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vdo.zycfv.cn

[B11] 生成数字序列 / 区间
来源：http://sbr.zhengqikj.top

Py:   list(range(0, 10, 2))
来源：http://xzm.nanxinkj.top

PHP:  range(0, 10, 2);
来源：http://rmm.shanyushiyangtech.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kqb.gogol.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ieq.andypj.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://usn.yj202588.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qur.zhixingplan.top

Ruby: (0...10).step(2).to_a
来源：http://fyg.sweek.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://krj.yanxiufei.cn

[B12] 跳出多层循环
来源：http://nae.andypj.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://rht.ybcxt.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://kos.tarul.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qco.bjfxy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://avo.mhx1999.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ndi.havefunace.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qyn.jiagoushi.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xxv.ydjk.org.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gny.jlsjyb.cn

[B13] 判断是否为数字
来源：http://uzx.bbcook.cn

Py:   isinstance(x, (int, float))
来源：http://stl.tian-w.cn

PHP:  is_numeric($x)
来源：http://khs.cqqwz.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zzi.zhijiandao.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sod.xuetiantiany.cn

Java: x instanceof Number
来源：http://nzj.xinyue.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lut.c1oappe.top

Ruby: x.is_a?(Numeric)
来源：http://dws.nanxinkj.top

C#:   x is int or double or decimal
来源：http://gxc.ywan-chungtsiang.top

[B14] 判断值是否在集合内
来源：http://swp.tianlin.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vry.9152youxi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hud.hfpthk.cn

JS:   [1, 2, 3].includes(x)
来源：http://huf.jqgfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://igu.vqdsnc.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yor.gaohongyu789.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cff.cheryme.top

Ruby: [1, 2, 3].include?(x)
来源：http://cln.yanxiufei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xle.svipenyu.cn

[B15] 布尔运算与取反
来源：http://hem.yfazqb.com

Py:   a and b or not c
来源：http://myk.zhoulong.xyz

PHP:  $a && $b || !$c
来源：http://ftq.52xcode.cn

JS:   a && b || !c
来源：http://pmb.yongpay.top

TS:   a && b || !c
来源：http://why.sufxvd.cn

Java: a && b || !c
来源：http://bvg.yvedp.cn

Go:   a && b || !c
来源：http://tya.epnwcf.com

Ruby: a && b || !c
来源：http://uhd.yuxming.cn

C#:   a && b || !c
来源：http://jhd.yfazqb.com

[B16] 卫语句：不满足条件提前返回
来源：http://ftp.jinqigufen.top

Py:   if not data: return
来源：http://pcl.uphjek.com

PHP:  if (!$data) { return; }
来源：http://hxe.wangdashe.top

JS:   if (!data) return;
来源：http://bze.xuanzx.com

TS:   if (!data) return;
来源：http://kia.yj20258888.top

Java: if (data == null) return;
来源：http://esz.snrcjt.cn

Go:   if data == nil { return }
来源：http://ujf.c1oappe.top

Ruby: return if data.nil?
来源：http://hcs.zdbjq.cn

C#:   if (data == null) return;
来源：http://cfz.hnqzz.top

================================================================================
来源：http://oax.shuidangran.top

C. 函数与作用域
来源：http://iuy.0kj1m.cn

================================================================================
来源：http://jtx.hnqzz.top

[C01] 定义函数
来源：http://wgw.wangdashe.top

Py:   def add(a, b): return a + b
来源：http://dkv.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eox.meibo888.top

JS:   function add(a, b) { return a + b; }
来源：http://ksk.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nwg.zhongyouzk.top

Java: static int add(int a, int b) { return a + b; }
来源：http://pgv.zhiwuduotai.top

Go:   func add(a, b int) int { return a + b }
来源：http://pnu.mhx1999.top

Ruby: def add(a, b); a + b; end
来源：http://nkq.haohaochexian.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qwo.cucudq.cn

[C02] 默认参数
来源：http://gxz.havefunace.top

Py:   def greet(name="World"): return name
来源：http://toa.yonumen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vkl.epnwcf.com

JS:   function greet(name = "World") { return name; }
来源：http://aug.jlsjyb.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vge.yongpay.top

Java: // 无默认参数：方法重载或 Optional
来源：http://lbp.snrcjt.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ijf.jyoumei.cn

Ruby: def greet(name = "World") = name
来源：http://oaq.zhixingplan.top

C#:   string Greet(string name = "World") => name;
来源：http://als.zhaomingkeji.xyz

[C03] 可变参数
来源：http://ulk.jiagoushi.top

Py:   def total(*args): return sum(args)
来源：http://jpj.sweek.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dkg.yuxming.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cvh.zhoulong.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hqj.fktsv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yms.xuetiantiany.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jla.meibo888.top

Ruby: def total(*nums); nums.sum; end
来源：http://yyw.wangshuangyany.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://edn.hywenlv.cn

[C04] 命名参数 / 关键字参数
来源：http://jia.snrcjt.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://roz.fzhhl.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://usi.svipenyu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hqs.aibaodan.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lyk.ywan-chungtsiang.top

Java: // 无：用 Builder 模式或 record
来源：http://rho.hnqzz.top

Go:   // 无：用配置结构体参数
来源：http://vqu.shangyingyoupin.top

Ruby: f(a: 1, b: 2)
来源：http://qul.nanxuanxn.top

C#:   f(a: 1, b: 2)
来源：http://bzy.uphjek.com

[C05] 返回多个值
来源：http://ygt.ehwqpu.com

Py:   return a, b
来源：http://rvb.0kj1m.cn

PHP:  return [$a, $b];
来源：http://qyy.svipenyu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://twn.daria6918.cn

TS:   return { a, b };
来源：http://yrn.svipenyu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kav.fzhhl.top

Go:   return a, b
来源：http://cgh.jlsjyb.cn

Ruby: return a, b
来源：http://qdz.gotoacloud.top

C#:   return (a, b);              // ValueTuple
来源：http://lbi.guannengcc.top

[C06] 匿名函数 / lambda
来源：http://xyd.svipenyu.cn

Py:   square = lambda x: x * x
来源：http://dya.ydjk.org.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fnt.chenzaomai.com

JS:   const square = x => x * x;
来源：http://riv.guowangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://nel.epnwcf.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vrg.yuanzhike.top

Go:   sq := func(x int) int { return x * x }
来源：http://acy.meibo888.top

Ruby: square = ->(x) { x * x }
来源：http://ksm.gotoacloud.top

C#:   Func<int, int> square = x => x * x;
来源：http://fgy.yj202588.top

[C07] 把函数作为参数传入
来源：http://jde.yj202588.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qvm.zycfv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kvb.meibo888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ngx.zhijiandao.cn

TS:   arr.map(String)
来源：http://lev.ppjwa.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hfx.jinghuilouyu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://orn.jyoumei.cn

Ruby: arr.map(&:upcase)
来源：http://hmb.jqgufenzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://klr.guannengcc.top

[C08] 闭包
来源：http://mbc.xinyue.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bcq.daria6918.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jep.svipenyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://phi.yueranfly.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://usx.yongpay.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vku.gzhubu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://heh.cucudq.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://amv.jyoumei.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ayw.jqgufenzy.top

[C09] 递归
来源：http://lrw.ydjk.org.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xfe.cheryme.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bqi.sufxvd.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wiw.zdqjudy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rwn.ydjk.org.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vqt.xinyue.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eyr.yvedp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://upl.cqqwz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mll.yueranfly.top

[C10] 变量作用域
来源：http://yah.tian-w.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yaf.shanyushiyangtech.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bzf.ybcxt.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://evp.tianlin.xyz

TS:   同 JS
来源：http://jge.hnxiangtu.top

Java: 方法内为块级作用域
来源：http://ukw.zdqjudy.top

Go:   花括号块级作用域
来源：http://uat.yangfankeji.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ysj.hysaishi.cn

C#:   块级作用域
来源：http://wbs.jinghuilouyu.cn

[C11] 模块导入与导出
来源：http://zbs.sjlbkw.cn

Py:   from module import func
来源：http://iav.jqgufenzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xbq.nanxuanxn.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tqg.hongshengwenyu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nvn.feifeiyinyue.top

Java: import java.util.List;
来源：http://bse.gzhubu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kyc.zhijiandao.cn

Ruby: require "json"; require_relative "./util"
来源：http://amf.zhongyouzk.top

C#:   using System.Text;
来源：http://ynh.shangyingyoupin.top

[C12] 立即执行函数 IIFE
来源：http://mtx.hcnkem.com

Py:   (lambda: print("run"))()
来源：http://btk.yfazqb.com

PHP:  (function () { echo "run"; })();
来源：http://vue.zhiwuduotai.top

JS:   (() => { console.log("run"); })();
来源：http://rrp.pycfn.com

TS:   (() => { console.log("run"); })();
来源：http://rbz.guowangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yam.shanyushiyangtech.top

Go:   func() { fmt.Println("run") }()
来源：http://wky.yueranfly.top

Ruby: -> { puts "run" }.call
来源：http://qdi.sjlbkw.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mmf.ydjk.org.cn

[C13] 类型声明 / 类型注解
来源：http://wpi.fktsv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://edp.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pys.yvedp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hpe.jyoumei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fez.hywenlv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://psc.sysykeji.top

Go:   func add(a, b int) int
来源：http://liz.cheryme.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ocq.jinghuilouyu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://djp.yfazqb.com

[C14] 泛型函数
来源：http://orj.xinyue.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://swh.tanke756.top

PHP:  // 无泛型
来源：http://edk.xingfuxueyuan.xyz

JS:   // 无泛型
来源：http://vzr.bbcook.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rzn.xinyue.icu

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lvt.jinqigufen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uax.redwolf501.top

Ruby: # 无泛型
来源：http://nrm.cashguo.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jai.0kj1m.cn

[C15] 解构 / 展开参数
来源：http://xmw.tian-w.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cet.hongshengwenyu.top

PHP:  [$a, $b] = $pair;
来源：http://ovc.cqqwz.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ptz.hywenlv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cdi.shanyushiyangkeji.top

Java: // 无解构
来源：http://ova.yj20258888.top

Go:   // 无解构
来源：http://hfq.hnqzz.top

Ruby: a, b = pair
来源：http://dlv.bbcook.cn

C#:   var (a, b) = pair;
来源：http://qga.hywenlv.cn

[C16] 函数 / 方法重载
来源：http://qsm.ybcxt.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tpv.dianchejie.cn

PHP:  // 无重载
来源：http://hsz.zhoulong.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://gaj.xylfe.cn

TS:   // 用联合类型或重载签名声明
来源：http://ggu.ehwqpu.com

Java: void f(int a) {}  void f(String a) {}
来源：http://vmu.wangdashe.top


<!-- 参考信息 -->