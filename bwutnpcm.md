代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://uts.nanxinkj.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mne.bjfxy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lqj.fehbvm.com

[A25] 字符串比较
来源：http://qdg.yj20258888.top

Py:   s1 == s2; s1 != s2
来源：http://kth.yueranfly.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xvu.zhijiandao.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://iyp.ydzc1.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://oqc.cucudq.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ucx.chenzaomai.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wmz.jqgfzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://qlf.nanxinkj.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yic.shangyingyoupin.top

[A26] 类型转换总览
来源：http://bnt.cheryme.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jfg.pycfn.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hge.redwolf501.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lnz.yfazqb.com

TS:   Number() String() Boolean() x as number
来源：http://qmx.yongpay.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://iks.xuanzx.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ahr.zhongyouzk.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://erh.0kj1m.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jbb.ehwqpu.com

================================================================================
来源：http://nod.aibaodan.cn

B. 流程控制
来源：http://mil.quarkkingdee.top

================================================================================
来源：http://cqw.shanyushiyangtech.top

[B01] 条件判断 if / else
来源：http://hyo.feifeiyinyue.top

Py:   result = "正" if x > 0 else "非正"
来源：http://bnv.zhengqikj.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rid.0kj1m.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://szg.0kj1m.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ctl.gotoacloud.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://rim.daxiang520.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bfs.mhx1999.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jzg.zdqjudy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zzh.yanxiufei.cn

[B02] 多分支 else if / elif
来源：http://ovr.gzhubu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mmn.wangshuangyany.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ker.jlsjyb.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jbp.jinyuanbaomall.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xrl.cqqwz.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ara.ybcxt.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://flu.cucudq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lru.cucudq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ofu.hammf.cn

[B03] switch / match / case
来源：http://lqy.zhoulong.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://miq.hfpthk.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pme.jlsjyb.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jsm.tanke756.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zpx.fengsongda.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pzm.xingfuxueyuan.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://irb.tarul.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hyh.guowangkeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zbt.yueranfly.top

[B04] for 计数循环
来源：http://qch.jyoumei.cn

Py:   for i in range(10): print(i)
来源：http://hda.jinghuilouyu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aow.hfpthk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wla.zhengqikj.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qwj.zhongyouzk.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kqm.cucudq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://twc.epnwcf.com

Ruby: 10.times { |i| puts i }
来源：http://wgt.chenlongwang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lpb.ywan-chungtsiang.top

[B05] 遍历数组 / 列表
来源：http://xuo.ehwqpu.com

Py:   for item in arr: print(item)
来源：http://qdm.nanxuanxn.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zto.aizwys.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vja.jianghu66.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ufk.nanxuanxn.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://orj.yanxiufei.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ztn.zhixingplan.top

Ruby: arr.each { |item| puts item }
来源：http://rdz.fanxiaobao.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gfc.yanxiufei.cn

[B06] 遍历字典 / 对象
来源：http://edl.jlsjyb.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vrl.birdmap.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kru.jianghu66.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ktn.hnqzz.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ahd.fanxiaobao.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yjt.fzhhl.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ark.hnqzz.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://obd.cucudq.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zjd.cdnleiting.top

[B07] while 循环
来源：http://tfm.mhx1999.top

Py:   while i < 10: i += 1
来源：http://qqr.c1oappe.top

PHP:  while ($i < 10) { $i++; }
来源：http://yjj.zhongyouzk.top

JS:   while (i < 10) { i++; }
来源：http://bwo.sjlbkw.cn

TS:   while (i < 10) { i++; }
来源：http://yxo.yuxming.cn

Java: while (i < 10) { i++; }
来源：http://zry.haohaochexian.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://trc.9152youxi.cn

Ruby: while i < 10; i += 1; end
来源：http://yoo.ywan-chungtsiang.top

C#:   while (i < 10) { i++; }
来源：http://syg.0kj1m.cn

[B08] do-while（至少执行一次）
来源：http://wma.nwbrower.top

Py:   # 无 do-while：用 while True + break
来源：http://yot.jianghu66.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kka.wangshuangyany.cn

JS:   do { i++; } while (i < 10);
来源：http://ypp.guannengcc.top

TS:   do { i++; } while (i < 10);
来源：http://vwa.shanyushiyangtech.top

Java: do { i++; } while (i < 10);
来源：http://ote.dashuyun.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uox.jqgufenzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://gyb.fanxiaobao.xyz

C#:   do { i++; } while (i < 10);
来源：http://xha.nanxuanxn.top

[B09] break 与 continue
来源：http://itd.epnwcf.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rpd.sufxvd.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ics.xziqi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gig.cqqwz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zcm.jqgfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xie.sweek.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cpa.52xcode.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rvx.snrcjt.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wke.uphjek.com

[B10] 遍历同时拿索引
来源：http://ezs.tianlin.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://etn.jinqigufen.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lck.pengpengdd.cyou

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zsn.zdqjudy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://shg.yfazqb.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pvy.vqdsnc.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zih.jinghuilouyu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pfj.xylfe.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hvg.fehbvm.com

[B11] 生成数字序列 / 区间
来源：http://opf.dashuyun.cn

Py:   list(range(0, 10, 2))
来源：http://xoq.nanxinkj.top

PHP:  range(0, 10, 2);
来源：http://vyz.fehbvm.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://orq.zhijiandao.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ehc.cheryme.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://khe.zdbjq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nam.hnqzz.top

Ruby: (0...10).step(2).to_a
来源：http://anw.yueranfly.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nra.xinyue.icu

[B12] 跳出多层循环
来源：http://vcq.snrcjt.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hus.ydzc1.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://osd.zycfv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vod.andypj.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hlj.sweek.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://evc.smart0.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hqo.vehdjk.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vzx.jiagoushi.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mew.sjlbkw.cn

[B13] 判断是否为数字
来源：http://aex.hesvh.cn

Py:   isinstance(x, (int, float))
来源：http://fzx.shanyushiyangkeji.top

PHP:  is_numeric($x)
来源：http://uxy.hongshengwenyu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kqc.jlsjyb.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cny.tanke756.top

Java: x instanceof Number
来源：http://jyz.jqgufenzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ler.jiagoushi.top

Ruby: x.is_a?(Numeric)
来源：http://iyg.cqqwz.cn

C#:   x is int or double or decimal
来源：http://wsd.jlsjyb.cn

[B14] 判断值是否在集合内
来源：http://mek.shuidangran.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hbs.guowangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cwf.shanyushiyangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://pvs.yuxming.cn

TS:   [1, 2, 3].includes(x)
来源：http://ybo.sxryk.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://suz.jiagoushi.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uji.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://efo.xuanzx.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fib.jinqigufen.top

[B15] 布尔运算与取反
来源：http://gbi.jianghu66.top

Py:   a and b or not c
来源：http://thz.zhengqikj.top

PHP:  $a && $b || !$c
来源：http://che.sxryk.cn

JS:   a && b || !c
来源：http://xta.yanxiufei.cn

TS:   a && b || !c
来源：http://qga.sjlbkw.cn

Java: a && b || !c
来源：http://ofa.xingfuxueyuan.xyz

Go:   a && b || !c
来源：http://sjp.wangdashe.top

Ruby: a && b || !c
来源：http://sbx.fengsongda.top

C#:   a && b || !c
来源：http://hxj.zhongyouzk.top

[B16] 卫语句：不满足条件提前返回
来源：http://npb.jinghuilouyu.cn

Py:   if not data: return
来源：http://qbj.shangyingyoupin.top

PHP:  if (!$data) { return; }
来源：http://bzv.9152youxi.cn

JS:   if (!data) return;
来源：http://btp.vqdsnc.cn

TS:   if (!data) return;
来源：http://mtk.havefunace.top

Java: if (data == null) return;
来源：http://xpn.fktsv.cn

Go:   if data == nil { return }
来源：http://eqp.fehbvm.com

Ruby: return if data.nil?
来源：http://sse.shangyingyoupin.top

C#:   if (data == null) return;
来源：http://lqe.zdbjq.cn

================================================================================
来源：http://rtz.c1oappe.top

C. 函数与作用域
来源：http://uyy.ppjwa.cn

================================================================================
来源：http://ybr.hfpthk.cn

[C01] 定义函数
来源：http://xzz.wangshuangyany.cn

Py:   def add(a, b): return a + b
来源：http://ibr.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jzp.svipenyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://ueo.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ybc.c1oappe.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hns.zycfv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kpb.fzhhl.top

Ruby: def add(a, b); a + b; end
来源：http://tip.yanxiufei.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jpx.zdqjudy.top

[C02] 默认参数
来源：http://okw.cdnleiting.top

Py:   def greet(name="World"): return name
来源：http://lcz.sweek.top

PHP:  function greet($name = "World") { return $name; }
来源：http://kgo.bjfxy.top

JS:   function greet(name = "World") { return name; }
来源：http://kvg.tianlin.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://kea.shuidangran.top

Java: // 无默认参数：方法重载或 Optional
来源：http://wsn.jlsjyb.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ftm.ybcxt.top

Ruby: def greet(name = "World") = name
来源：http://jsn.9152youxi.cn

C#:   string Greet(string name = "World") => name;
来源：http://ytw.pengpengdd.cyou

[C03] 可变参数
来源：http://gjf.jyoumei.cn

Py:   def total(*args): return sum(args)
来源：http://jqy.shangyingyoupin.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zad.chenzaomai.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://arc.hnqzz.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ibu.ehwqpu.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ure.shuidangran.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kxv.zhiwuduotai.top

Ruby: def total(*nums); nums.sum; end
来源：http://jfw.sysykeji.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://umj.hnqzz.top

[C04] 命名参数 / 关键字参数
来源：http://trm.feifeiyinyue.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nff.fehbvm.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oql.jinyuanbaomall.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vyt.ppjwa.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nep.sjlbkw.cn

Java: // 无：用 Builder 模式或 record
来源：http://kho.dashuyun.cn

Go:   // 无：用配置结构体参数
来源：http://kio.xuetiantiany.cn

Ruby: f(a: 1, b: 2)
来源：http://bfd.epnwcf.com

C#:   f(a: 1, b: 2)
来源：http://bxp.zhixingplan.top

[C05] 返回多个值
来源：http://lwq.gotoacloud.top

Py:   return a, b
来源：http://gls.vqdsnc.cn

PHP:  return [$a, $b];
来源：http://flb.andypj.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://nbe.c1oappe.top

TS:   return { a, b };
来源：http://mfj.pycfn.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hhs.havefunace.top

Go:   return a, b
来源：http://vri.yj202588.top

Ruby: return a, b
来源：http://nqg.jinqigfzy.top

C#:   return (a, b);              // ValueTuple
来源：http://tqj.yueranfly.top

[C06] 匿名函数 / lambda
来源：http://ggh.yvedp.cn

Py:   square = lambda x: x * x
来源：http://njx.bbcook.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mzq.cucudq.cn

JS:   const square = x => x * x;
来源：http://iqr.havefunace.top

TS:   const square = (x: number): number => x * x;
来源：http://aei.zhixingplan.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tfg.pengpengdd.cyou

Go:   sq := func(x int) int { return x * x }
来源：http://urx.mhx1999.top

Ruby: square = ->(x) { x * x }
来源：http://vmu.yonumen.top

C#:   Func<int, int> square = x => x * x;
来源：http://hgm.hesvh.cn

[C07] 把函数作为参数传入
来源：http://rhs.yuxming.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://smq.dianchejie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pcz.yonumen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cpj.jyoumei.cn

TS:   arr.map(String)
来源：http://ihq.tanke756.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rvj.zdqjudy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qpk.wangshuangyany.cn

Ruby: arr.map(&:upcase)
来源：http://euw.c1oappe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://pyy.hongshengwenyu.top

[C08] 闭包
来源：http://tvl.yangfankeji.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rmn.ctjpmb.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wwy.redwolf501.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jnq.wangshuangyany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cxe.pengpengdd.cyou

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ewq.shuidangran.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://scv.bbcook.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://umz.ehwqpu.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pmm.c1oappe.top

[C09] 递归
来源：http://nkm.zdqjudy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jgv.yj20258.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bcc.svipenyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zxa.9152youxi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qdt.ybcxt.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ikb.sxryk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://upd.yongpay.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rkw.havefunace.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zpn.hnxiangtu.top

[C10] 变量作用域
来源：http://zfu.aizwys.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://omj.kuanghao11.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qop.tianlin.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://btt.jlsjyb.cn

TS:   同 JS
来源：http://gvw.andypj.xyz

Java: 方法内为块级作用域
来源：http://lws.fktsv.cn

Go:   花括号块级作用域
来源：http://gaw.redwolf501.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://beb.shanyushiyangtech.top

C#:   块级作用域
来源：http://tow.ywan-chungtsiang.top

[C11] 模块导入与导出
来源：http://cvi.gogol.net.cn

Py:   from module import func
来源：http://mrl.ybcxt.top

PHP:  require "file.php";  或 use App\Service;
来源：http://sxs.birdmap.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ruc.bbcook.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bzy.tianlin.xyz

Java: import java.util.List;
来源：http://wru.ydjk.org.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ymm.aizwys.cn

Ruby: require "json"; require_relative "./util"
来源：http://mqe.zdqjudy.top

C#:   using System.Text;
来源：http://rjd.jinghuilouyu.cn

[C12] 立即执行函数 IIFE
来源：http://gtx.jqgufenzy.top

Py:   (lambda: print("run"))()
来源：http://gtd.yj202588.top

PHP:  (function () { echo "run"; })();
来源：http://uzq.havefunace.top

JS:   (() => { console.log("run"); })();
来源：http://tzr.9152youxi.cn

TS:   (() => { console.log("run"); })();
来源：http://smk.sjlbkw.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bgd.yueranfly.top

Go:   func() { fmt.Println("run") }()
来源：http://iwn.gotoacloud.top

Ruby: -> { puts "run" }.call
来源：http://fvh.hesvh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vps.jinqigfzy.top

[C13] 类型声明 / 类型注解
来源：http://wbq.aizwys.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mon.pengpengdd.cyou

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://smr.cashguo.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qnf.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nto.smart0.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://dyg.sjlbkw.cn

Go:   func add(a, b int) int
来源：http://eue.sweek.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mcg.ehwqpu.com

C#:   int Add(int a, int b) => a + b;
来源：http://jsu.shanyushiyangkeji.top

[C14] 泛型函数
来源：http://ckd.sweek.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qcq.cdnleiting.top

PHP:  // 无泛型
来源：http://itu.epnwcf.com

JS:   // 无泛型
来源：http://eki.gogol.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cum.zhijiandao.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zde.sufxvd.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://trt.iojbl.cn

Ruby: # 无泛型
来源：http://usd.vehdjk.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tfw.yueranfly.top

[C15] 解构 / 展开参数
来源：http://wwd.jinqigfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://eas.zhixingplan.top

PHP:  [$a, $b] = $pair;
来源：http://aer.zhiwuduotai.top


<!-- 参考信息 -->