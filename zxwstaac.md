代发 wailian999

[A26] 类型转换总览
来源：http://cng.xinyue.icu

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lsi.aibaodan.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vkk.yuxming.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dos.zhijiandao.cn

TS:   Number() String() Boolean() x as number
来源：http://avz.yvedp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tcj.0kj1m.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://csf.zhijiandao.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bjn.yj20258.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wsb.feifeiyinyue.top

================================================================================
来源：http://xvp.zhixingplan.top

B. 流程控制
来源：http://tiu.andypj.xyz

================================================================================
来源：http://yqy.xinyue.icu

[B01] 条件判断 if / else
来源：http://pqa.feifeiyinyue.top

Py:   result = "正" if x > 0 else "非正"
来源：http://qps.svipenyu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://spd.ehwqpu.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ywp.cqqwz.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oma.cdnleiting.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://xpp.cashguo.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sra.jlsjyb.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qvs.cqqwz.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mym.fktsv.cn

[B02] 多分支 else if / elif
来源：http://hbz.yuanzhike.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://olc.feifeiyinyue.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dir.shangyingyoupin.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dnb.jqgfzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iqz.kuanghao11.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sjy.guannengcc.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zhm.smart0.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://brd.zdbjq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ivq.epnwcf.com

[B03] switch / match / case
来源：http://kcz.yongpay.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://boy.mhx1999.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sci.zhixingplan.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pwq.ehwqpu.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rcr.hammf.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mdl.yuanzhike.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nhb.vehdjk.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://acl.ywan-chungtsiang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://njd.fehbvm.com

[B04] for 计数循环
来源：http://qzt.yanxiufei.cn

Py:   for i in range(10): print(i)
来源：http://amz.hnxiangtu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tzk.ehwqpu.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://buc.gzhubu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mpf.yvedp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kqj.fengsongda.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jea.fengsongda.top

Ruby: 10.times { |i| puts i }
来源：http://uqb.guowangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mpr.yonumen.top

[B05] 遍历数组 / 列表
来源：http://tji.cqqwz.cn

Py:   for item in arr: print(item)
来源：http://ajm.cucudq.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qlb.yj202588.top

JS:   for (const item of arr) { console.log(item); }
来源：http://wym.yj20258.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tuz.c1oappe.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://zwe.tanke756.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dzw.havefunace.top

Ruby: arr.each { |item| puts item }
来源：http://brx.sxryk.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zja.shangyingyoupin.top

[B06] 遍历字典 / 对象
来源：http://xho.hysaishi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rwz.aibaodan.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://npp.jqgufenzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fvw.smart0.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jcf.gzhubu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tqx.sjlbkw.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pmx.jinqigfzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ale.ybcxt.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tkg.316326.xyz

[B07] while 循环
来源：http://wex.shanyushiyangtech.top

Py:   while i < 10: i += 1
来源：http://omm.aibaodan.cn

PHP:  while ($i < 10) { $i++; }
来源：http://daz.fengsongda.top

JS:   while (i < 10) { i++; }
来源：http://hob.cucudq.cn

TS:   while (i < 10) { i++; }
来源：http://zrc.0kj1m.cn

Java: while (i < 10) { i++; }
来源：http://wjy.zhijiandao.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lbo.jinqigufen.top

Ruby: while i < 10; i += 1; end
来源：http://gmc.wangdashe.top

C#:   while (i < 10) { i++; }
来源：http://xnw.quarkkingdee.top

[B08] do-while（至少执行一次）
来源：http://stz.guannengcc.top

Py:   # 无 do-while：用 while True + break
来源：http://ayi.mhx1999.top

PHP:  do { $i++; } while ($i < 10);
来源：http://bsu.uphjek.com

JS:   do { i++; } while (i < 10);
来源：http://kwo.yanxiufei.cn

TS:   do { i++; } while (i < 10);
来源：http://wdc.bjfxy.top

Java: do { i++; } while (i < 10);
来源：http://qrp.ybcxt.top

Go:   for { i++; if i >= 10 { break } }
来源：http://eku.epnwcf.com

Ruby: begin; i += 1; end while i < 10
来源：http://zfo.ydzc1.top

C#:   do { i++; } while (i < 10);
来源：http://nyc.snrcjt.cn

[B09] break 与 continue
来源：http://qjt.ydzc1.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wif.shangyingyoupin.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lzd.sufxvd.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hrg.aibaodan.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lsb.zdbjq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ucp.yfazqb.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kja.sysykeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dii.shanyushiyangkeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://trc.nanxuanxn.top

[B10] 遍历同时拿索引
来源：http://cpg.dianchejie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kra.jiagoushi.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fzu.fengsongda.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://aym.smart0.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jsw.pycfn.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rmq.jlsjyb.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nsq.gaohongyu789.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tbo.redwolf501.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xil.shangyingyoupin.top

[B11] 生成数字序列 / 区间
来源：http://yhv.mhx1999.top

Py:   list(range(0, 10, 2))
来源：http://pws.fanxiaobao.xyz

PHP:  range(0, 10, 2);
来源：http://fcl.yuanzhike.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://son.tian-w.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hau.shzxlz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mup.fengsongda.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wkg.ywan-chungtsiang.top

Ruby: (0...10).step(2).to_a
来源：http://fjp.yueranfly.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://izf.hnxiangtu.top

[B12] 跳出多层循环
来源：http://fxv.yueranfly.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vxn.sysykeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vaq.smart0.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uoi.quarkkingdee.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zud.zhixingplan.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xfs.fengsongda.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://awq.cdnleiting.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zdu.jqgufenzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nqq.sxryk.cn

[B13] 判断是否为数字
来源：http://udf.ivvv.top

Py:   isinstance(x, (int, float))
来源：http://pds.quarkkingdee.top

PHP:  is_numeric($x)
来源：http://jyn.hfpthk.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ifb.ehwqpu.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kck.jinghuilouyu.cn

Java: x instanceof Number
来源：http://mac.andypj.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gxz.jyoumei.cn

Ruby: x.is_a?(Numeric)
来源：http://euf.dashuyun.cn

C#:   x is int or double or decimal
来源：http://cnu.pengpengdd.cyou

[B14] 判断值是否在集合内
来源：http://xtp.cheryme.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cou.yj20258888.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cis.zdbjq.cn

JS:   [1, 2, 3].includes(x)
来源：http://nie.hnxiangtu.top

TS:   [1, 2, 3].includes(x)
来源：http://org.cdnleiting.top

Java: List.of(1, 2, 3).contains(x)
来源：http://qit.xinyue.icu

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://stq.pycfn.com

Ruby: [1, 2, 3].include?(x)
来源：http://yut.wangshuangyany.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ljq.sysykeji.top

[B15] 布尔运算与取反
来源：http://oos.bbcook.cn

Py:   a and b or not c
来源：http://yzf.aibaodan.cn

PHP:  $a && $b || !$c
来源：http://nxc.cheryme.top

JS:   a && b || !c
来源：http://erq.sweek.top

TS:   a && b || !c
来源：http://idd.fktsv.cn

Java: a && b || !c
来源：http://sru.redwolf501.top

Go:   a && b || !c
来源：http://afe.gzhubu.top

Ruby: a && b || !c
来源：http://ngn.xingfuxueyuan.xyz

C#:   a && b || !c
来源：http://tfr.fzhhl.top

[B16] 卫语句：不满足条件提前返回
来源：http://ury.jqgufenzy.top

Py:   if not data: return
来源：http://pth.redwolf501.top

PHP:  if (!$data) { return; }
来源：http://fxj.xinyue.icu

JS:   if (!data) return;
来源：http://hph.yvedp.cn

TS:   if (!data) return;
来源：http://jtb.jiagoushi.top

Java: if (data == null) return;
来源：http://sfr.yuxming.cn

Go:   if data == nil { return }
来源：http://qko.tian-w.cn

Ruby: return if data.nil?
来源：http://lmo.fktsv.cn

C#:   if (data == null) return;
来源：http://alo.birdmap.top

================================================================================
来源：http://pcp.pengpengdd.cyou

C. 函数与作用域
来源：http://vxs.epnwcf.com

================================================================================
来源：http://ych.xuetiantiany.cn

[C01] 定义函数
来源：http://lbu.fanxiaobao.xyz

Py:   def add(a, b): return a + b
来源：http://xsc.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rmu.cashguo.top

JS:   function add(a, b) { return a + b; }
来源：http://aak.svipenyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://agi.jinqigfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kgi.iojbl.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vdv.gzhubu.top

Ruby: def add(a, b); a + b; end
来源：http://eid.316326.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ndr.iojbl.cn

[C02] 默认参数
来源：http://fyg.jinqigfzy.top

Py:   def greet(name="World"): return name
来源：http://ncl.fzhhl.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gxp.snrcjt.cn

JS:   function greet(name = "World") { return name; }
来源：http://ewo.jlsjyb.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gwi.yangfankeji.com

Java: // 无默认参数：方法重载或 Optional
来源：http://tkr.nwbrower.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sqn.ybcxt.top

Ruby: def greet(name = "World") = name
来源：http://dzc.fanxiaobao.xyz

C#:   string Greet(string name = "World") => name;
来源：http://cnr.quarkkingdee.top

[C03] 可变参数
来源：http://ngr.fanxiaobao.xyz

Py:   def total(*args): return sum(args)
来源：http://hit.yj202588.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nqb.zycfv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ajk.tanke756.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://foo.hfpthk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zwt.chenlongwang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bak.jiagoushi.top

Ruby: def total(*nums); nums.sum; end
来源：http://wnd.chenlongwang.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mxy.ppjwa.cn

[C04] 命名参数 / 关键字参数
来源：http://thl.9152youxi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mof.c1oappe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hbw.yj20258.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sro.sweek.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ryy.zhongyouzk.top

Java: // 无：用 Builder 模式或 record
来源：http://rba.bjfxy.top

Go:   // 无：用配置结构体参数
来源：http://obj.wangshuangyany.cn

Ruby: f(a: 1, b: 2)
来源：http://ihm.haohaochexian.top

C#:   f(a: 1, b: 2)
来源：http://viv.jyoumei.cn

[C05] 返回多个值
来源：http://zxn.shanyushiyangtech.top

Py:   return a, b
来源：http://ikp.yonumen.top

PHP:  return [$a, $b];
来源：http://fgh.shangyingyoupin.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://sev.yanxiufei.cn

TS:   return { a, b };
来源：http://inw.redwolf501.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tcx.ivvv.top

Go:   return a, b
来源：http://lxw.hywenlv.cn

Ruby: return a, b
来源：http://eab.hnxiangtu.top

C#:   return (a, b);              // ValueTuple
来源：http://szl.fehbvm.com

[C06] 匿名函数 / lambda
来源：http://qpq.aizwys.cn

Py:   square = lambda x: x * x
来源：http://wut.ywan-chungtsiang.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ptx.gzhubu.top

JS:   const square = x => x * x;
来源：http://fwp.fktsv.cn

TS:   const square = (x: number): number => x * x;
来源：http://urh.meibo888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://akk.zhoulong.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://jdx.xingfuxueyuan.xyz

Ruby: square = ->(x) { x * x }
来源：http://evq.ybcxt.top

C#:   Func<int, int> square = x => x * x;
来源：http://idm.ydjk.org.cn

[C07] 把函数作为参数传入
来源：http://dhy.jiagoushi.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gqt.sweek.top

PHP:  array_map("strtoupper", $arr);
来源：http://hku.fzhhl.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rkb.ydzc1.top

TS:   arr.map(String)
来源：http://nnt.dashuyun.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jrz.gzhubu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xij.ydzc1.top

Ruby: arr.map(&:upcase)
来源：http://faj.chenzaomai.com

C#:   arr.Select(s => s.ToUpper())
来源：http://uuz.svipenyu.cn

[C08] 闭包
来源：http://khb.bbcook.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wqq.ehwqpu.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wmx.shuidangran.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fjb.fktsv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sqi.zhaomingkeji.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://agf.shuidangran.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uou.0kj1m.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pjv.sjlbkw.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cxe.iojbl.cn

[C09] 递归
来源：http://qtb.nanxinkj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://grr.sweek.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lpt.ybcxt.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qar.vehdjk.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xvc.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mnc.jiagoushi.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jgd.vqdsnc.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://usn.nanxuanxn.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://eqy.andypj.xyz

[C10] 变量作用域
来源：http://anh.0kj1m.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tqb.bjfxy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iao.jinqigufen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cvz.shuidangran.top

TS:   同 JS
来源：http://kyv.zdqjudy.top

Java: 方法内为块级作用域
来源：http://bcg.jqgfzy.top

Go:   花括号块级作用域
来源：http://dzt.yj202588.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://phd.jinyuanbaomall.cn

C#:   块级作用域
来源：http://jyf.xuanzx.com

[C11] 模块导入与导出
来源：http://lvw.guowangkeji.top

Py:   from module import func
来源：http://rnp.ybcxt.top

PHP:  require "file.php";  或 use App\Service;
来源：http://izi.vqdsnc.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hjs.hysaishi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://scm.pycfn.com

Java: import java.util.List;
来源：http://chn.yuanzhike.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rlp.ydzc1.top

Ruby: require "json"; require_relative "./util"
来源：http://aos.zhongyouzk.top

C#:   using System.Text;
来源：http://fzj.jinqigufen.top

[C12] 立即执行函数 IIFE
来源：http://qhn.fengsongda.top

Py:   (lambda: print("run"))()
来源：http://vhc.fehbvm.com

PHP:  (function () { echo "run"; })();
来源：http://ism.cdnleiting.top

JS:   (() => { console.log("run"); })();
来源：http://elh.xziqi.cn

TS:   (() => { console.log("run"); })();
来源：http://wpu.nanxinkj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xrr.bbcook.cn

Go:   func() { fmt.Println("run") }()
来源：http://vfo.zhixingplan.top

Ruby: -> { puts "run" }.call
来源：http://imy.wangdashe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pya.52xcode.cn

[C13] 类型声明 / 类型注解
来源：http://owj.xuanzx.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dcj.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dgb.redwolf501.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ouv.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kjo.yuxming.cn

Java: int add(int a, int b) { return a + b; }
来源：http://waf.ehwqpu.com

Go:   func add(a, b int) int
来源：http://nxw.fengsongda.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ykp.xuanzx.com

C#:   int Add(int a, int b) => a + b;
来源：http://vep.sweek.top

[C14] 泛型函数
来源：http://fkq.tian-w.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iny.xuetiantiany.cn

PHP:  // 无泛型
来源：http://tgq.jqgufenzy.top

JS:   // 无泛型
来源：http://rfs.fanxiaobao.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://npz.jlsjyb.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://esv.yueranfly.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wxy.hysaishi.cn

Ruby: # 无泛型
来源：http://gnx.feifeiyinyue.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xta.guannengcc.top

[C15] 解构 / 展开参数
来源：http://cov.cashguo.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ets.0kj1m.cn

PHP:  [$a, $b] = $pair;
来源：http://pew.cheryme.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qje.yongpay.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pas.cashguo.top

Java: // 无解构
来源：http://rxg.hcnkem.com

Go:   // 无解构
来源：http://orh.yuxming.cn

Ruby: a, b = pair
来源：http://ezs.daria6918.cn

C#:   var (a, b) = pair;
来源：http://ljy.zhoulong.xyz

[C16] 函数 / 方法重载
来源：http://nqc.daxiang520.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zmi.yongpay.top

PHP:  // 无重载
来源：http://ump.svipenyu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://awx.xziqi.cn

TS:   // 用联合类型或重载签名声明
来源：http://yrb.kuanghao11.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wow.chenlongwang.top


<!-- 参考信息 -->