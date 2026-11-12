代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://yqx.yvedp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cww.tarul.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iio.xingfuxueyuan.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://ued.quarkkingdee.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://khf.hongshengwenyu.top

================================================================================
来源：http://gqq.yfazqb.com

B. 流程控制
来源：http://nsk.ybcxt.top

================================================================================
来源：http://mhz.wangshuangyany.cn

[B01] 条件判断 if / else
来源：http://qjq.tarul.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wfi.0kj1m.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://axd.xuetiantiany.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dqb.fktsv.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kkj.quarkkingdee.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://llp.birdmap.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://slp.zdqjudy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jdd.xuanzx.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yqp.guowangkeji.top

[B02] 多分支 else if / elif
来源：http://mzs.hfpthk.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zet.hysaishi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dpg.jlsjyb.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sgq.shanyushiyangkeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eqt.aizwys.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uta.316326.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mkq.fehbvm.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wdx.xziqi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ura.mhx1999.top

[B03] switch / match / case
来源：http://rip.sjlbkw.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gxl.jinqigfzy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dtc.nwbrower.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://atf.vehdjk.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ncv.zdqjudy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ogi.xinyue.icu

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xgk.chenlongwang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://aeg.sufxvd.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rww.jianghu66.top

[B04] for 计数循环
来源：http://xzy.nanxinkj.top

Py:   for i in range(10): print(i)
来源：http://wbr.redwolf501.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ilh.hnqzz.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wrf.ywan-chungtsiang.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ocu.hongshengwenyu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hcc.fktsv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jjd.pycfn.com

Ruby: 10.times { |i| puts i }
来源：http://nqj.quarkkingdee.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mpd.snrcjt.cn

[B05] 遍历数组 / 列表
来源：http://jdo.jinqigufen.top

Py:   for item in arr: print(item)
来源：http://rph.gaohongyu789.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lek.yonumen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ttv.chenjidiqi.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://ycq.gaohongyu789.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://leb.fehbvm.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ecj.cqqwz.cn

Ruby: arr.each { |item| puts item }
来源：http://imh.xuetiantiany.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yyl.cucudq.cn

[B06] 遍历字典 / 对象
来源：http://kmu.feifeiyinyue.top

Py:   for k, v in d.items(): print(k, v)
来源：http://eoa.ivvv.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ovq.yanxiufei.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kqz.zhijiandao.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bnh.ydzc1.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uxi.fengsongda.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cut.yongpay.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ujw.jqgufenzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fzz.fzhhl.top

[B07] while 循环
来源：http://jxf.zycfv.cn

Py:   while i < 10: i += 1
来源：http://cfd.mhx1999.top

PHP:  while ($i < 10) { $i++; }
来源：http://dzw.fzhhl.top

JS:   while (i < 10) { i++; }
来源：http://eia.ydzc1.top

TS:   while (i < 10) { i++; }
来源：http://ucl.shuidangran.top

Java: while (i < 10) { i++; }
来源：http://gbf.gzhubu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ked.ppjwa.cn

Ruby: while i < 10; i += 1; end
来源：http://vqi.gaohongyu789.top

C#:   while (i < 10) { i++; }
来源：http://xnx.havefunace.top

[B08] do-while（至少执行一次）
来源：http://shj.nwbrower.top

Py:   # 无 do-while：用 while True + break
来源：http://sry.yj20258.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ebq.hnxiangtu.top

JS:   do { i++; } while (i < 10);
来源：http://ych.cucudq.cn

TS:   do { i++; } while (i < 10);
来源：http://xxr.sweek.top

Java: do { i++; } while (i < 10);
来源：http://bed.ywan-chungtsiang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://emh.jinqigfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://tfp.yonumen.top

C#:   do { i++; } while (i < 10);
来源：http://bep.feifeiyinyue.top

[B09] break 与 continue
来源：http://mde.hammf.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fho.feifeiyinyue.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://acw.iojbl.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xpg.hesvh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ynl.xuanzx.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://trf.zhixingplan.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ael.ybcxt.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rds.bjfxy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jkc.chenjidiqi.icu

[B10] 遍历同时拿索引
来源：http://rju.zycfv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mtc.xylfe.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kwi.yfazqb.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uao.zdbjq.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iba.zhaomingkeji.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zds.zhongyouzk.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pom.xziqi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vjh.dashuyun.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wvp.jinqigufen.top

[B11] 生成数字序列 / 区间
来源：http://cqq.zhijiandao.cn

Py:   list(range(0, 10, 2))
来源：http://atw.fzhhl.top

PHP:  range(0, 10, 2);
来源：http://nvk.ppjwa.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xzg.jqgfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gwx.hywenlv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kks.hywenlv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jan.ppjwa.cn

Ruby: (0...10).step(2).to_a
来源：http://nlj.yonumen.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yfe.wangdashe.top

[B12] 跳出多层循环
来源：http://yzu.hesvh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bpl.shzxlz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hfu.gotoacloud.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://its.zhijiandao.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://unj.ybcxt.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eas.dianchejie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dhq.mhx1999.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://byw.yangfankeji.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xuc.cqqwz.cn

[B13] 判断是否为数字
来源：http://lpa.ctjpmb.com

Py:   isinstance(x, (int, float))
来源：http://jaj.redwolf501.top

PHP:  is_numeric($x)
来源：http://hzp.nanxinkj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://opv.vqdsnc.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aiw.jinghuilouyu.cn

Java: x instanceof Number
来源：http://pzh.jyoumei.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yxu.nanxuanxn.top

Ruby: x.is_a?(Numeric)
来源：http://daj.ybcxt.top

C#:   x is int or double or decimal
来源：http://iqp.sysykeji.top

[B14] 判断值是否在集合内
来源：http://ezl.jyoumei.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jbj.yvedp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yec.jiagoushi.top

JS:   [1, 2, 3].includes(x)
来源：http://gsg.haohaochexian.top

TS:   [1, 2, 3].includes(x)
来源：http://ehj.9152youxi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://imz.0kj1m.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qfq.hnxiangtu.top

Ruby: [1, 2, 3].include?(x)
来源：http://akk.havefunace.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hti.yuanzhike.top

[B15] 布尔运算与取反
来源：http://pbi.jiagoushi.top

Py:   a and b or not c
来源：http://umn.hnxiangtu.top

PHP:  $a && $b || !$c
来源：http://rko.jinqigfzy.top

JS:   a && b || !c
来源：http://qvf.pengpengdd.cyou

TS:   a && b || !c
来源：http://kmi.chenjidiqi.icu

Java: a && b || !c
来源：http://ksa.dianchejie.cn

Go:   a && b || !c
来源：http://fsy.bbcook.cn

Ruby: a && b || !c
来源：http://ooj.hongshengwenyu.top

C#:   a && b || !c
来源：http://vbd.iojbl.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gak.aizwys.cn

Py:   if not data: return
来源：http://lzx.hnqzz.top

PHP:  if (!$data) { return; }
来源：http://vit.hnxiangtu.top

JS:   if (!data) return;
来源：http://jpo.haohaochexian.top

TS:   if (!data) return;
来源：http://ivr.xinyue.icu

Java: if (data == null) return;
来源：http://xca.chenzaomai.com

Go:   if data == nil { return }
来源：http://ffd.9152youxi.cn

Ruby: return if data.nil?
来源：http://jyv.cheryme.top

C#:   if (data == null) return;
来源：http://muc.redwolf501.top

================================================================================
来源：http://lek.hysaishi.cn

C. 函数与作用域
来源：http://qic.cheryme.top

================================================================================
来源：http://hex.cqqwz.cn

[C01] 定义函数
来源：http://xjv.zdbjq.cn

Py:   def add(a, b): return a + b
来源：http://bmi.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://huw.cqqwz.cn

JS:   function add(a, b) { return a + b; }
来源：http://hpf.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cgk.jianghu66.top

Java: static int add(int a, int b) { return a + b; }
来源：http://iqb.zhiwuduotai.top

Go:   func add(a, b int) int { return a + b }
来源：http://mrm.zhijiandao.cn

Ruby: def add(a, b); a + b; end
来源：http://zwg.hysaishi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vch.redwolf501.top

[C02] 默认参数
来源：http://fql.hesvh.cn

Py:   def greet(name="World"): return name
来源：http://xbh.xylfe.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xrn.guannengcc.top

JS:   function greet(name = "World") { return name; }
来源：http://ynp.chenzaomai.com

TS:   function greet(name: string = "World") { return name; }
来源：http://dkq.vqdsnc.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://aiu.hongshengwenyu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ctw.smart0.xyz

Ruby: def greet(name = "World") = name
来源：http://ykv.xuanzx.com

C#:   string Greet(string name = "World") => name;
来源：http://gwv.jinqigufen.top

[C03] 可变参数
来源：http://hjq.zhijiandao.cn

Py:   def total(*args): return sum(args)
来源：http://smp.hywenlv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xfo.gzhubu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dgx.snrcjt.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qnk.guannengcc.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kcd.fanxiaobao.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cpg.9152youxi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rxg.zhijiandao.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vuy.dashuyun.cn

[C04] 命名参数 / 关键字参数
来源：http://urc.tanke756.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eza.fehbvm.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mel.zhoulong.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lau.fktsv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oig.birdmap.top

Java: // 无：用 Builder 模式或 record
来源：http://dep.hcnkem.com

Go:   // 无：用配置结构体参数
来源：http://smm.c1oappe.top

Ruby: f(a: 1, b: 2)
来源：http://xdh.zhoulong.xyz

C#:   f(a: 1, b: 2)
来源：http://vpc.birdmap.top

[C05] 返回多个值
来源：http://kzv.jinqigufen.top

Py:   return a, b
来源：http://zst.jinqigufen.top

PHP:  return [$a, $b];
来源：http://bqp.vqdsnc.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xdc.fzhhl.top

TS:   return { a, b };
来源：http://uzo.gotoacloud.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uen.redwolf501.top

Go:   return a, b
来源：http://vkj.cqqwz.cn

Ruby: return a, b
来源：http://uyo.daxiang520.top

C#:   return (a, b);              // ValueTuple
来源：http://ciu.jinyuanbaomall.cn

[C06] 匿名函数 / lambda
来源：http://ohi.yangfankeji.com

Py:   square = lambda x: x * x
来源：http://ufc.dashuyun.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hld.52xcode.cn

JS:   const square = x => x * x;
来源：http://mni.chenlongwang.top

TS:   const square = (x: number): number => x * x;
来源：http://flg.yangfankeji.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jec.iojbl.cn

Go:   sq := func(x int) int { return x * x }
来源：http://efn.ydjk.org.cn

Ruby: square = ->(x) { x * x }
来源：http://gnl.xingfuxueyuan.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://gon.fktsv.cn

[C07] 把函数作为参数传入
来源：http://mgm.52xcode.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jrv.yongpay.top

PHP:  array_map("strtoupper", $arr);
来源：http://vxw.ydjk.org.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jnx.smart0.xyz

TS:   arr.map(String)
来源：http://rvr.jinqigfzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pnv.xuanzx.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ivu.gzhubu.top

Ruby: arr.map(&:upcase)
来源：http://exq.cqqwz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vpb.tanke756.top

[C08] 闭包
来源：http://kfx.guannengcc.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nfy.hnqzz.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zgp.sufxvd.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://net.jinqigfzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yap.sweek.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jas.smart0.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jnu.hammf.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uaa.xylfe.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eyn.tianlin.xyz

[C09] 递归
来源：http://ddg.yj202588.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bji.zhengqikj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://epv.fehbvm.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rvh.yuxming.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qnk.hammf.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jmk.hfpthk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uil.guannengcc.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ifd.jinqigfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://faz.sweek.top

[C10] 变量作用域
来源：http://ohu.jlsjyb.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gng.yueranfly.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kja.sjlbkw.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cen.mhx1999.top

TS:   同 JS
来源：http://tpq.yuxming.cn

Java: 方法内为块级作用域
来源：http://tzd.haohaochexian.top

Go:   花括号块级作用域
来源：http://uwx.fktsv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cjp.cdnleiting.top

C#:   块级作用域
来源：http://ico.mhx1999.top

[C11] 模块导入与导出
来源：http://zld.sjlbkw.cn

Py:   from module import func
来源：http://xax.nanxuanxn.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pof.ivvv.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://kyy.ywan-chungtsiang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zyj.gzhubu.top

Java: import java.util.List;
来源：http://wqq.gotoacloud.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ufs.wangshuangyany.cn

Ruby: require "json"; require_relative "./util"
来源：http://kwe.daxiang520.top

C#:   using System.Text;
来源：http://ssr.zhoulong.xyz

[C12] 立即执行函数 IIFE
来源：http://gaa.epnwcf.com

Py:   (lambda: print("run"))()
来源：http://ute.hesvh.cn

PHP:  (function () { echo "run"; })();
来源：http://cml.hnqzz.top

JS:   (() => { console.log("run"); })();
来源：http://imn.nanxuanxn.top

TS:   (() => { console.log("run"); })();
来源：http://yeu.sweek.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zlf.xziqi.cn

Go:   func() { fmt.Println("run") }()
来源：http://zex.gaohongyu789.top

Ruby: -> { puts "run" }.call
来源：http://exp.bbcook.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ykj.gaohongyu789.top

[C13] 类型声明 / 类型注解
来源：http://yat.pycfn.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wsi.xuetiantiany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iqf.yfazqb.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://htc.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rrg.hammf.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mqf.guowangkeji.top

Go:   func add(a, b int) int
来源：http://okj.shuidangran.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ztx.c1oappe.top

C#:   int Add(int a, int b) => a + b;
来源：http://ioq.nanxuanxn.top

[C14] 泛型函数
来源：http://dww.zhiwuduotai.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wyf.vehdjk.com

PHP:  // 无泛型
来源：http://pxt.hesvh.cn

JS:   // 无泛型
来源：http://blk.kuanghao11.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lxm.chenjidiqi.icu

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://axs.svipenyu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lop.tian-w.cn

Ruby: # 无泛型
来源：http://ezi.hesvh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nwn.smart0.xyz

[C15] 解构 / 展开参数
来源：http://hlk.yj20258.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dea.ppjwa.cn

PHP:  [$a, $b] = $pair;
来源：http://zps.hcnkem.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dli.tianlin.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://let.zhongyouzk.top

Java: // 无解构
来源：http://sdu.snrcjt.cn

Go:   // 无解构
来源：http://ecf.xinyue.icu

Ruby: a, b = pair
来源：http://obf.zhijiandao.cn

C#:   var (a, b) = pair;
来源：http://qcs.yongpay.top

[C16] 函数 / 方法重载
来源：http://kta.haohaochexian.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tga.zhoulong.xyz

PHP:  // 无重载
来源：http://hgj.yj20258.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://shw.zhijiandao.cn

TS:   // 用联合类型或重载签名声明
来源：http://wry.9152youxi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ttq.smart0.xyz

Go:   // 无重载：用不同函数名
来源：http://bph.xziqi.cn

Ruby: # 无重载：靠动态参数
来源：http://nbl.fehbvm.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://tfm.cdnleiting.top

================================================================================
来源：http://ryp.jqgfzy.top


<!-- 参考信息 -->