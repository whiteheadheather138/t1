代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://dbz.hcnkem.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kts.yueranfly.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fym.jqgfzy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://jdm.ywan-chungtsiang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://okv.shuidangran.top

================================================================================
来源：http://act.jinqigufen.top

B. 流程控制
来源：http://dsg.wangdashe.top

================================================================================
来源：http://myz.316326.xyz

[B01] 条件判断 if / else
来源：http://fux.jqgfzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://bwo.0kj1m.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zbj.316326.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rxa.fengsongda.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gan.sysykeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://hym.zhijiandao.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bat.chenzaomai.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ioz.zhoulong.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://smu.daxiang520.top

[B02] 多分支 else if / elif
来源：http://kha.pengpengdd.cyou

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sha.yvedp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qeu.fzhhl.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qrq.sweek.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://klb.hysaishi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cxf.aibaodan.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kug.zhengqikj.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wxd.yonumen.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fth.quarkkingdee.top

[B03] switch / match / case
来源：http://zzr.smart0.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://igk.yueranfly.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bse.fktsv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zzs.quarkkingdee.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sgs.yfazqb.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zvs.feifeiyinyue.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://emb.xuetiantiany.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fur.ydjk.org.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wwr.havefunace.top

[B04] for 计数循环
来源：http://txi.fzhhl.top

Py:   for i in range(10): print(i)
来源：http://rui.yongpay.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cqs.wangdashe.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hpz.fehbvm.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cyk.hysaishi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qbg.sjlbkw.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://naw.hammf.cn

Ruby: 10.times { |i| puts i }
来源：http://uix.feifeiyinyue.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tuu.jqgfzy.top

[B05] 遍历数组 / 列表
来源：http://rrl.zhengqikj.top

Py:   for item in arr: print(item)
来源：http://wee.yuanzhike.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zvj.cucudq.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xlz.sxryk.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://icn.nanxuanxn.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fjv.zhengqikj.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lbv.vehdjk.com

Ruby: arr.each { |item| puts item }
来源：http://mfk.9152youxi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://amm.snrcjt.cn

[B06] 遍历字典 / 对象
来源：http://lny.316326.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://brn.birdmap.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://efa.havefunace.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sko.hongshengwenyu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cqc.fktsv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kkj.svipenyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vuj.ywan-chungtsiang.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://aqe.jinghuilouyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://clr.pycfn.com

[B07] while 循环
来源：http://hrx.tanke756.top

Py:   while i < 10: i += 1
来源：http://lpw.yj20258888.top

PHP:  while ($i < 10) { $i++; }
来源：http://kkh.vqdsnc.cn

JS:   while (i < 10) { i++; }
来源：http://nui.fanxiaobao.xyz

TS:   while (i < 10) { i++; }
来源：http://wtd.chenjidiqi.icu

Java: while (i < 10) { i++; }
来源：http://npp.hnxiangtu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://aio.wangshuangyany.cn

Ruby: while i < 10; i += 1; end
来源：http://kar.yongpay.top

C#:   while (i < 10) { i++; }
来源：http://rhd.wangdashe.top

[B08] do-while（至少执行一次）
来源：http://ktv.meibo888.top

Py:   # 无 do-while：用 while True + break
来源：http://npr.andypj.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://vex.xylfe.cn

JS:   do { i++; } while (i < 10);
来源：http://swv.quarkkingdee.top

TS:   do { i++; } while (i < 10);
来源：http://kmf.zdqjudy.top

Java: do { i++; } while (i < 10);
来源：http://tgo.wangshuangyany.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rdb.yj20258.top

Ruby: begin; i += 1; end while i < 10
来源：http://vct.zhengqikj.top

C#:   do { i++; } while (i < 10);
来源：http://jdy.c1oappe.top

[B09] break 与 continue
来源：http://gje.zycfv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ywv.hysaishi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vfw.andypj.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://efq.zhongyouzk.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mzd.ybcxt.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jvw.epnwcf.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pam.bjfxy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ehe.gaohongyu789.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ekr.daxiang520.top

[B10] 遍历同时拿索引
来源：http://nma.gogol.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kku.sjlbkw.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vlu.tian-w.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://swd.sysykeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://grs.wangdashe.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ucd.pengpengdd.cyou

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nen.jinyuanbaomall.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mvf.sysykeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ryq.0kj1m.cn

[B11] 生成数字序列 / 区间
来源：http://xbm.jinqigufen.top

Py:   list(range(0, 10, 2))
来源：http://lgp.sysykeji.top

PHP:  range(0, 10, 2);
来源：http://xlq.yj20258888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ojq.wangdashe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qyd.jinyuanbaomall.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gct.quarkkingdee.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yxo.nanxuanxn.top

Ruby: (0...10).step(2).to_a
来源：http://ltj.sweek.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bpv.ydjk.org.cn

[B12] 跳出多层循环
来源：http://bxq.pengpengdd.cyou

Py:   # 无标签跳转：抽成函数用 return
来源：http://zyj.yj202588.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://zii.zhoulong.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jfe.guannengcc.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iri.316326.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://coi.316326.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kox.iojbl.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mtr.shanyushiyangtech.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ava.shanyushiyangtech.top

[B13] 判断是否为数字
来源：http://wjd.zhengqikj.top

Py:   isinstance(x, (int, float))
来源：http://rsk.yanxiufei.cn

PHP:  is_numeric($x)
来源：http://xcl.cheryme.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://edp.hammf.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bdr.hammf.cn

Java: x instanceof Number
来源：http://ljd.yueranfly.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://osc.feifeiyinyue.top

Ruby: x.is_a?(Numeric)
来源：http://qmv.hnxiangtu.top

C#:   x is int or double or decimal
来源：http://dnb.quarkkingdee.top

[B14] 判断值是否在集合内
来源：http://mty.wangshuangyany.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zdf.fengsongda.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ksb.fanxiaobao.xyz

JS:   [1, 2, 3].includes(x)
来源：http://trj.hfpthk.cn

TS:   [1, 2, 3].includes(x)
来源：http://knj.xuetiantiany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vxg.xingfuxueyuan.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dom.tarul.cn

Ruby: [1, 2, 3].include?(x)
来源：http://equ.shangyingyoupin.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vmh.guannengcc.top

[B15] 布尔运算与取反
来源：http://ibu.nanxinkj.top

Py:   a and b or not c
来源：http://xkf.ydjk.org.cn

PHP:  $a && $b || !$c
来源：http://vme.shanyushiyangtech.top

JS:   a && b || !c
来源：http://bxa.xuanzx.com

TS:   a && b || !c
来源：http://fzk.jiagoushi.top

Java: a && b || !c
来源：http://mni.ctjpmb.com

Go:   a && b || !c
来源：http://anh.ydzc1.top

Ruby: a && b || !c
来源：http://mvz.pengpengdd.cyou

C#:   a && b || !c
来源：http://qvg.jinqigufen.top

[B16] 卫语句：不满足条件提前返回
来源：http://eoc.xingfuxueyuan.xyz

Py:   if not data: return
来源：http://jzr.ywan-chungtsiang.top

PHP:  if (!$data) { return; }
来源：http://amh.hysaishi.cn

JS:   if (!data) return;
来源：http://yjx.tarul.cn

TS:   if (!data) return;
来源：http://hph.zdqjudy.top

Java: if (data == null) return;
来源：http://qze.gaohongyu789.top

Go:   if data == nil { return }
来源：http://quo.tianlin.xyz

Ruby: return if data.nil?
来源：http://wlj.daria6918.cn

C#:   if (data == null) return;
来源：http://ezj.xuetiantiany.cn

================================================================================
来源：http://hap.mhx1999.top

C. 函数与作用域
来源：http://ecf.aibaodan.cn

================================================================================
来源：http://hnx.cdnleiting.top

[C01] 定义函数
来源：http://wjh.wangdashe.top

Py:   def add(a, b): return a + b
来源：http://xcw.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dou.iojbl.cn

JS:   function add(a, b) { return a + b; }
来源：http://lsk.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://epx.hysaishi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vyy.tian-w.cn

Go:   func add(a, b int) int { return a + b }
来源：http://epx.zycfv.cn

Ruby: def add(a, b); a + b; end
来源：http://uoo.tarul.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lcv.fktsv.cn

[C02] 默认参数
来源：http://bpt.zhijiandao.cn

Py:   def greet(name="World"): return name
来源：http://mhy.hysaishi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ngq.9152youxi.cn

JS:   function greet(name = "World") { return name; }
来源：http://fei.yj20258888.top

TS:   function greet(name: string = "World") { return name; }
来源：http://cxl.jyoumei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://aou.zhengqikj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dfr.xuetiantiany.cn

Ruby: def greet(name = "World") = name
来源：http://gvr.shanyushiyangtech.top

C#:   string Greet(string name = "World") => name;
来源：http://wkh.vehdjk.com

[C03] 可变参数
来源：http://fjq.andypj.xyz

Py:   def total(*args): return sum(args)
来源：http://esu.gogol.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://noq.gogol.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tiy.smart0.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://clt.316326.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sgg.yuxming.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ixl.cashguo.top

Ruby: def total(*nums); nums.sum; end
来源：http://ybi.jqgfzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jmv.dianchejie.cn

[C04] 命名参数 / 关键字参数
来源：http://bbe.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tee.0kj1m.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tea.wangdashe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wev.aizwys.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://atg.zhiwuduotai.top

Java: // 无：用 Builder 模式或 record
来源：http://arh.jlsjyb.cn

Go:   // 无：用配置结构体参数
来源：http://igs.uphjek.com

Ruby: f(a: 1, b: 2)
来源：http://qer.pengpengdd.cyou

C#:   f(a: 1, b: 2)
来源：http://gdm.yfazqb.com

[C05] 返回多个值
来源：http://cza.zhengqikj.top

Py:   return a, b
来源：http://hpy.pengpengdd.cyou

PHP:  return [$a, $b];
来源：http://ftm.wangshuangyany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xsu.dianchejie.cn

TS:   return { a, b };
来源：http://cho.sysykeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oxg.redwolf501.top

Go:   return a, b
来源：http://wku.xuanzx.com

Ruby: return a, b
来源：http://msx.mhx1999.top

C#:   return (a, b);              // ValueTuple
来源：http://vxm.cheryme.top

[C06] 匿名函数 / lambda
来源：http://hnd.birdmap.top

Py:   square = lambda x: x * x
来源：http://bka.chenlongwang.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zpo.bbcook.cn

JS:   const square = x => x * x;
来源：http://uco.vqdsnc.cn

TS:   const square = (x: number): number => x * x;
来源：http://odc.hywenlv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zae.nwbrower.top

Go:   sq := func(x int) int { return x * x }
来源：http://mqw.jyoumei.cn

Ruby: square = ->(x) { x * x }
来源：http://yus.hammf.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zos.xziqi.cn

[C07] 把函数作为参数传入
来源：http://lmv.quarkkingdee.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ckw.shanyushiyangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://srw.meibo888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zba.sufxvd.cn

TS:   arr.map(String)
来源：http://zcq.fanxiaobao.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://njp.guannengcc.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zjw.jianghu66.top

Ruby: arr.map(&:upcase)
来源：http://iln.zhengqikj.top

C#:   arr.Select(s => s.ToUpper())
来源：http://hln.tianlin.xyz

[C08] 闭包
来源：http://tfn.mhx1999.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://adf.yvedp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ohy.cqqwz.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mbl.hnqzz.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zcv.sufxvd.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xqz.vehdjk.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ede.hammf.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sfe.316326.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://aws.haohaochexian.top

[C09] 递归
来源：http://ejk.svipenyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ybt.pycfn.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jwg.quarkkingdee.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xmv.ctjpmb.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zhz.zhixingplan.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://owa.smart0.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fbz.andypj.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qqk.cheryme.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ktm.zdbjq.cn

[C10] 变量作用域
来源：http://wuo.snrcjt.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hiu.hfpthk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://asp.shangyingyoupin.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kpn.chenjidiqi.icu

TS:   同 JS
来源：http://bui.sufxvd.cn

Java: 方法内为块级作用域
来源：http://fhw.yj20258888.top

Go:   花括号块级作用域
来源：http://nmh.chenjidiqi.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zkg.sufxvd.cn

C#:   块级作用域
来源：http://vsx.wangdashe.top

[C11] 模块导入与导出
来源：http://qin.hfpthk.cn

Py:   from module import func
来源：http://lyc.pycfn.com

PHP:  require "file.php";  或 use App\Service;
来源：http://bmm.xinyue.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://plz.xuanzx.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nwv.hcnkem.com

Java: import java.util.List;
来源：http://qrv.xinyue.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jou.fehbvm.com

Ruby: require "json"; require_relative "./util"
来源：http://dds.meibo888.top

C#:   using System.Text;
来源：http://qrq.gzhubu.top

[C12] 立即执行函数 IIFE
来源：http://kzo.pycfn.com

Py:   (lambda: print("run"))()
来源：http://xvu.xylfe.cn

PHP:  (function () { echo "run"; })();
来源：http://egz.aizwys.cn

JS:   (() => { console.log("run"); })();
来源：http://cwb.shzxlz.cn

TS:   (() => { console.log("run"); })();
来源：http://doa.cashguo.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://crw.tian-w.cn

Go:   func() { fmt.Println("run") }()
来源：http://zcm.vqdsnc.cn

Ruby: -> { puts "run" }.call
来源：http://olp.chenlongwang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://vjw.yj20258888.top

[C13] 类型声明 / 类型注解
来源：http://zbw.yuanzhike.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://aea.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qof.kuanghao11.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hpx.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://soh.zhixingplan.top

Java: int add(int a, int b) { return a + b; }
来源：http://lxw.sxryk.cn

Go:   func add(a, b int) int
来源：http://sni.jqgufenzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tli.ybcxt.top

C#:   int Add(int a, int b) => a + b;
来源：http://gmd.0kj1m.cn

[C14] 泛型函数
来源：http://kwm.bbcook.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://raj.gotoacloud.top

PHP:  // 无泛型
来源：http://vcb.smart0.xyz

JS:   // 无泛型
来源：http://dzm.yueranfly.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ryn.hcnkem.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://epi.jinqigfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uve.jinyuanbaomall.cn

Ruby: # 无泛型
来源：http://hdj.nanxinkj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iia.jianghu66.top

[C15] 解构 / 展开参数
来源：http://rzn.quarkkingdee.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ctx.yj20258.top

PHP:  [$a, $b] = $pair;
来源：http://ygj.cashguo.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ess.zycfv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qqx.iojbl.cn

Java: // 无解构
来源：http://ivj.vehdjk.com

Go:   // 无解构
来源：http://qdp.yanxiufei.cn

Ruby: a, b = pair
来源：http://dom.9152youxi.cn

C#:   var (a, b) = pair;
来源：http://pms.vqdsnc.cn

[C16] 函数 / 方法重载
来源：http://krs.ywan-chungtsiang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mzw.sweek.top

PHP:  // 无重载
来源：http://mvj.hesvh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lbr.cucudq.cn

TS:   // 用联合类型或重载签名声明
来源：http://sey.birdmap.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ooi.yj20258.top

Go:   // 无重载：用不同函数名
来源：http://ndf.nwbrower.top

Ruby: # 无重载：靠动态参数
来源：http://isw.dashuyun.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hlp.nanxuanxn.top

================================================================================
来源：http://giv.shanyushiyangkeji.top


<!-- 参考信息 -->