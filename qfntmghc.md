代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ufq.c1oappe.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sej.jinqigufen.top

Ruby: s1 == s2; s1 <=> s2
来源：http://qhg.c1oappe.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ryx.cqqwz.cn

[A26] 类型转换总览
来源：http://tfe.c1oappe.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xpy.aizwys.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://isg.ctjpmb.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vdc.jinghuilouyu.cn

TS:   Number() String() Boolean() x as number
来源：http://yds.meibo888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wic.wangshuangyany.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gdr.dashuyun.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ytc.nwbrower.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bkk.ydzc1.top

================================================================================
来源：http://cpx.vqdsnc.cn

B. 流程控制
来源：http://cqe.cqqwz.cn

================================================================================
来源：http://tvn.shuidangran.top

[B01] 条件判断 if / else
来源：http://rsu.yj20258.top

Py:   result = "正" if x > 0 else "非正"
来源：http://zqm.cdnleiting.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zcj.vehdjk.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://duf.jlsjyb.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pwv.daxiang520.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://msq.yongpay.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cgr.zycfv.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://joj.tian-w.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pjt.yueranfly.top

[B02] 多分支 else if / elif
来源：http://zqk.gogol.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nos.fengsongda.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gth.52xcode.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://exf.redwolf501.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xxm.0kj1m.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bsl.yongpay.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rrt.shanyushiyangkeji.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mrs.hcnkem.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vyy.xylfe.cn

[B03] switch / match / case
来源：http://ndy.chenzaomai.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ahj.ydzc1.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lai.yj202588.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rep.yuanzhike.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qcq.bjfxy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lio.zhongyouzk.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bjk.feifeiyinyue.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dmd.sjlbkw.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qho.sysykeji.top

[B04] for 计数循环
来源：http://thn.nwbrower.top

Py:   for i in range(10): print(i)
来源：http://evc.jyoumei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ucg.ybcxt.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cxx.sysykeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dqu.316326.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ayv.guannengcc.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cni.guowangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://mkj.xziqi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rlz.wangdashe.top

[B05] 遍历数组 / 列表
来源：http://kuz.ctjpmb.com

Py:   for item in arr: print(item)
来源：http://rwk.aibaodan.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hqj.xziqi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://iem.sjlbkw.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://khv.andypj.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://bfg.fanxiaobao.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jxf.ybcxt.top

Ruby: arr.each { |item| puts item }
来源：http://shb.vehdjk.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ict.yvedp.cn

[B06] 遍历字典 / 对象
来源：http://vue.zhaomingkeji.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://eqx.bbcook.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://aye.chenzaomai.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pxa.wangshuangyany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ccz.zhijiandao.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sol.zhongyouzk.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qpj.9152youxi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jhn.hysaishi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ffj.zdbjq.cn

[B07] while 循环
来源：http://daj.zhoulong.xyz

Py:   while i < 10: i += 1
来源：http://iyh.smart0.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://eei.xylfe.cn

JS:   while (i < 10) { i++; }
来源：http://wjy.fzhhl.top

TS:   while (i < 10) { i++; }
来源：http://ufn.yuxming.cn

Java: while (i < 10) { i++; }
来源：http://tir.smart0.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://npz.yongpay.top

Ruby: while i < 10; i += 1; end
来源：http://hqj.hongshengwenyu.top

C#:   while (i < 10) { i++; }
来源：http://sis.hnxiangtu.top

[B08] do-while（至少执行一次）
来源：http://fvm.sweek.top

Py:   # 无 do-while：用 while True + break
来源：http://xrc.zdbjq.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kkj.bjfxy.top

JS:   do { i++; } while (i < 10);
来源：http://cok.tianlin.xyz

TS:   do { i++; } while (i < 10);
来源：http://lhi.jinghuilouyu.cn

Java: do { i++; } while (i < 10);
来源：http://koe.yj20258888.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wzh.sjlbkw.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fri.hnqzz.top

C#:   do { i++; } while (i < 10);
来源：http://ljo.yueranfly.top

[B09] break 与 continue
来源：http://agf.fehbvm.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mie.gaohongyu789.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tay.jianghu66.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eto.xylfe.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://emz.bjfxy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cjy.ydzc1.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mto.c1oappe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nkr.gotoacloud.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hwv.chenlongwang.top

[B10] 遍历同时拿索引
来源：http://svg.uphjek.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bpu.iojbl.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mvw.sxryk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tgi.dashuyun.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kng.sjlbkw.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://geq.chenlongwang.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pcp.daxiang520.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://muf.ybcxt.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ase.daxiang520.top

[B11] 生成数字序列 / 区间
来源：http://uoi.hongshengwenyu.top

Py:   list(range(0, 10, 2))
来源：http://xhg.hnxiangtu.top

PHP:  range(0, 10, 2);
来源：http://snb.yonumen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ynk.ehwqpu.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gcp.shanyushiyangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jjd.cdnleiting.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://azj.cdnleiting.top

Ruby: (0...10).step(2).to_a
来源：http://quu.ydzc1.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hpe.jyoumei.cn

[B12] 跳出多层循环
来源：http://wbz.gotoacloud.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://nnz.pengpengdd.cyou

PHP:  # 无标签：用 goto 或函数返回
来源：http://xae.havefunace.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://afq.zdqjudy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yck.yangfankeji.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bvr.vehdjk.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fej.zhijiandao.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bli.bbcook.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ejj.zhijiandao.cn

[B13] 判断是否为数字
来源：http://uxt.pycfn.com

Py:   isinstance(x, (int, float))
来源：http://cez.daria6918.cn

PHP:  is_numeric($x)
来源：http://pgg.yueranfly.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://psx.zhiwuduotai.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wqk.nanxuanxn.top

Java: x instanceof Number
来源：http://tee.cucudq.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yhj.shangyingyoupin.top

Ruby: x.is_a?(Numeric)
来源：http://xnz.aibaodan.cn

C#:   x is int or double or decimal
来源：http://lbm.pengpengdd.cyou

[B14] 判断值是否在集合内
来源：http://dhf.shzxlz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nff.jinqigfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ezl.mhx1999.top

JS:   [1, 2, 3].includes(x)
来源：http://odj.redwolf501.top

TS:   [1, 2, 3].includes(x)
来源：http://nuh.feifeiyinyue.top

Java: List.of(1, 2, 3).contains(x)
来源：http://rpy.shanyushiyangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://aaq.9152youxi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vmf.mhx1999.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wpj.gogol.net.cn

[B15] 布尔运算与取反
来源：http://usk.aibaodan.cn

Py:   a and b or not c
来源：http://qrm.zhoulong.xyz

PHP:  $a && $b || !$c
来源：http://jjx.aizwys.cn

JS:   a && b || !c
来源：http://tsx.jqgfzy.top

TS:   a && b || !c
来源：http://lhc.52xcode.cn

Java: a && b || !c
来源：http://xqi.zhaomingkeji.xyz

Go:   a && b || !c
来源：http://uop.shangyingyoupin.top

Ruby: a && b || !c
来源：http://wuy.aizwys.cn

C#:   a && b || !c
来源：http://lwu.hysaishi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wzx.vehdjk.com

Py:   if not data: return
来源：http://trz.yj202588.top

PHP:  if (!$data) { return; }
来源：http://myx.yueranfly.top

JS:   if (!data) return;
来源：http://sty.tarul.cn

TS:   if (!data) return;
来源：http://dli.shuidangran.top

Java: if (data == null) return;
来源：http://ebm.jiagoushi.top

Go:   if data == nil { return }
来源：http://edc.0kj1m.cn

Ruby: return if data.nil?
来源：http://oum.ivvv.top

C#:   if (data == null) return;
来源：http://ncc.snrcjt.cn

================================================================================
来源：http://ycd.tarul.cn

C. 函数与作用域
来源：http://ive.nanxuanxn.top

================================================================================
来源：http://lym.shangyingyoupin.top

[C01] 定义函数
来源：http://oxb.yfazqb.com

Py:   def add(a, b): return a + b
来源：http://avv.hysaishi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://guf.jianghu66.top

JS:   function add(a, b) { return a + b; }
来源：http://bog.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gzf.yfazqb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://vds.kuanghao11.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cwq.nanxinkj.top

Ruby: def add(a, b); a + b; end
来源：http://znu.hnqzz.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ddu.tanke756.top

[C02] 默认参数
来源：http://ptt.meibo888.top

Py:   def greet(name="World"): return name
来源：http://puy.epnwcf.com

PHP:  function greet($name = "World") { return $name; }
来源：http://box.tian-w.cn

JS:   function greet(name = "World") { return name; }
来源：http://mrj.shzxlz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ezm.yuxming.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ekx.gogol.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vzj.fktsv.cn

Ruby: def greet(name = "World") = name
来源：http://feh.tanke756.top

C#:   string Greet(string name = "World") => name;
来源：http://mep.wangshuangyany.cn

[C03] 可变参数
来源：http://xey.yonumen.top

Py:   def total(*args): return sum(args)
来源：http://dnm.daria6918.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vsl.ywan-chungtsiang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wlh.yangfankeji.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://izb.yfazqb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://irm.ehwqpu.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kti.fanxiaobao.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://kqk.ywan-chungtsiang.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gls.fehbvm.com

[C04] 命名参数 / 关键字参数
来源：http://lyl.wangdashe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ztd.hesvh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tyl.zycfv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://not.ybcxt.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://aoj.xingfuxueyuan.xyz

Java: // 无：用 Builder 模式或 record
来源：http://xgi.wangdashe.top

Go:   // 无：用配置结构体参数
来源：http://hwt.jinyuanbaomall.cn

Ruby: f(a: 1, b: 2)
来源：http://zoq.jlsjyb.cn

C#:   f(a: 1, b: 2)
来源：http://jmj.yonumen.top

[C05] 返回多个值
来源：http://smw.zdqjudy.top

Py:   return a, b
来源：http://qpy.hesvh.cn

PHP:  return [$a, $b];
来源：http://osd.ydjk.org.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cgi.shanyushiyangkeji.top

TS:   return { a, b };
来源：http://hul.xingfuxueyuan.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ckp.sjlbkw.cn

Go:   return a, b
来源：http://bsm.jyoumei.cn

Ruby: return a, b
来源：http://rij.wangshuangyany.cn

C#:   return (a, b);              // ValueTuple
来源：http://rqt.fanxiaobao.xyz

[C06] 匿名函数 / lambda
来源：http://wgr.yueranfly.top

Py:   square = lambda x: x * x
来源：http://zji.gzhubu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ole.meibo888.top

JS:   const square = x => x * x;
来源：http://mji.zhixingplan.top

TS:   const square = (x: number): number => x * x;
来源：http://mvk.sweek.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mqx.wangdashe.top

Go:   sq := func(x int) int { return x * x }
来源：http://frg.wangdashe.top

Ruby: square = ->(x) { x * x }
来源：http://ptw.gotoacloud.top

C#:   Func<int, int> square = x => x * x;
来源：http://wap.gzhubu.top

[C07] 把函数作为参数传入
来源：http://zlf.wangshuangyany.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fmx.zhoulong.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://qem.fengsongda.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://syv.hammf.cn

TS:   arr.map(String)
来源：http://xvd.chenlongwang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qtr.daria6918.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vev.fzhhl.top

Ruby: arr.map(&:upcase)
来源：http://wnc.zhixingplan.top

C#:   arr.Select(s => s.ToUpper())
来源：http://bcx.yangfankeji.com

[C08] 闭包
来源：http://gxb.wangdashe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qtj.ywan-chungtsiang.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fhb.ydjk.org.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://agm.daxiang520.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://srp.nanxinkj.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xjd.xuetiantiany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mwx.yonumen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qbe.redwolf501.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uud.sweek.top

[C09] 递归
来源：http://qfx.yonumen.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uue.jinghuilouyu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kjo.guannengcc.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://psk.tanke756.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nwa.gogol.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tak.andypj.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dek.yj202588.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vkn.jinqigufen.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ndv.tian-w.cn

[C10] 变量作用域
来源：http://hup.fanxiaobao.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zcl.cucudq.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yoa.ehwqpu.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://joa.birdmap.top

TS:   同 JS
来源：http://sdz.dashuyun.cn

Java: 方法内为块级作用域
来源：http://slw.fehbvm.com

Go:   花括号块级作用域
来源：http://cnu.fktsv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rss.ydzc1.top

C#:   块级作用域
来源：http://zcx.feifeiyinyue.top

[C11] 模块导入与导出
来源：http://vzz.redwolf501.top

Py:   from module import func
来源：http://jth.tianlin.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://itm.yj20258.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nmw.gaohongyu789.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jlm.birdmap.top

Java: import java.util.List;
来源：http://iig.bjfxy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mzm.cashguo.top

Ruby: require "json"; require_relative "./util"
来源：http://mur.guannengcc.top

C#:   using System.Text;
来源：http://sem.fengsongda.top

[C12] 立即执行函数 IIFE
来源：http://lel.hesvh.cn

Py:   (lambda: print("run"))()
来源：http://ein.zhijiandao.cn

PHP:  (function () { echo "run"; })();
来源：http://zvs.tarul.cn

JS:   (() => { console.log("run"); })();
来源：http://cxl.aizwys.cn

TS:   (() => { console.log("run"); })();
来源：http://fnx.hesvh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zos.jqgufenzy.top

Go:   func() { fmt.Println("run") }()
来源：http://hpe.cheryme.top

Ruby: -> { puts "run" }.call
来源：http://idu.cheryme.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ybd.wangdashe.top

[C13] 类型声明 / 类型注解
来源：http://cke.zhongyouzk.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uez.ydzc1.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qjg.fehbvm.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tux.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mxu.cucudq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ddt.ywan-chungtsiang.top

Go:   func add(a, b int) int
来源：http://yks.zhiwuduotai.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ykq.chenzaomai.com

C#:   int Add(int a, int b) => a + b;
来源：http://iyd.pengpengdd.cyou

[C14] 泛型函数
来源：http://spm.hysaishi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://awl.iojbl.cn

PHP:  // 无泛型
来源：http://qcj.hnqzz.top

JS:   // 无泛型
来源：http://xrp.zhaomingkeji.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jwy.jlsjyb.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://exz.zhiwuduotai.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bfh.zycfv.cn

Ruby: # 无泛型
来源：http://uiv.yfazqb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://orf.jyoumei.cn

[C15] 解构 / 展开参数
来源：http://bzt.yj20258.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ooi.shanyushiyangtech.top

PHP:  [$a, $b] = $pair;
来源：http://ssc.daria6918.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qok.bjfxy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qzy.iojbl.cn

Java: // 无解构
来源：http://gmz.yj20258888.top

Go:   // 无解构
来源：http://iav.xziqi.cn

Ruby: a, b = pair
来源：http://tir.zhijiandao.cn

C#:   var (a, b) = pair;
来源：http://ebo.cqqwz.cn

[C16] 函数 / 方法重载
来源：http://rll.shangyingyoupin.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sgo.yongpay.top


<!-- 参考信息 -->