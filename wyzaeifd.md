代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://zct.yj20258888.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://iyx.fengsongda.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://brv.ivvv.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zgz.yj20258888.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://udh.haohaochexian.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kvv.andypj.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://uyr.jiagoushi.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wjt.jinqigufen.top

[A26] 类型转换总览
来源：http://wqz.redwolf501.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://djd.ydzc1.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yyc.smart0.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oxc.svipenyu.cn

TS:   Number() String() Boolean() x as number
来源：http://icp.gotoacloud.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zqi.ivvv.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rat.gzhubu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://sbz.ywan-chungtsiang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rrj.epnwcf.com

================================================================================
来源：http://cpp.zycfv.cn

B. 流程控制
来源：http://not.zhoulong.xyz

================================================================================
来源：http://daw.sufxvd.cn

[B01] 条件判断 if / else
来源：http://crj.dashuyun.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://luk.pengpengdd.cyou

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kpj.gaohongyu789.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gvd.birdmap.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://heb.shanyushiyangkeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://egb.guannengcc.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tat.shuidangran.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kra.xylfe.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hrj.smart0.xyz

[B02] 多分支 else if / elif
来源：http://seo.tian-w.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ibk.nanxinkj.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hnv.zhiwuduotai.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ymv.hnxiangtu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://biq.pengpengdd.cyou

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sum.daxiang520.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fuy.zhiwuduotai.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://obi.cashguo.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sar.uphjek.com

[B03] switch / match / case
来源：http://btt.zhengqikj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kfz.yonumen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jtz.jinyuanbaomall.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aqf.zdqjudy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mrc.fengsongda.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qok.jianghu66.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jze.jinqigufen.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bqm.ivvv.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://aae.guannengcc.top

[B04] for 计数循环
来源：http://thk.c1oappe.top

Py:   for i in range(10): print(i)
来源：http://zww.shzxlz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://agl.hesvh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fbd.zdqjudy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nau.ywan-chungtsiang.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://psx.shanyushiyangtech.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xgm.zycfv.cn

Ruby: 10.times { |i| puts i }
来源：http://jca.jinghuilouyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kxb.fanxiaobao.xyz

[B05] 遍历数组 / 列表
来源：http://yzb.shuidangran.top

Py:   for item in arr: print(item)
来源：http://gla.gzhubu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://txl.ivvv.top

JS:   for (const item of arr) { console.log(item); }
来源：http://mxu.hnxiangtu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://gyz.hnqzz.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://meq.tarul.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://owf.zhiwuduotai.top

Ruby: arr.each { |item| puts item }
来源：http://itc.gotoacloud.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kse.zhijiandao.cn

[B06] 遍历字典 / 对象
来源：http://ssm.jianghu66.top

Py:   for k, v in d.items(): print(k, v)
来源：http://olm.gaohongyu789.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ups.yj20258888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wqs.zhoulong.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vtn.ppjwa.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ikb.zhijiandao.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ybw.ybcxt.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zhl.chenlongwang.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://liw.chenlongwang.top

[B07] while 循环
来源：http://xzc.zdqjudy.top

Py:   while i < 10: i += 1
来源：http://lpq.jyoumei.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ykt.dianchejie.cn

JS:   while (i < 10) { i++; }
来源：http://dng.daria6918.cn

TS:   while (i < 10) { i++; }
来源：http://ekf.shangyingyoupin.top

Java: while (i < 10) { i++; }
来源：http://fbn.tanke756.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://taj.fehbvm.com

Ruby: while i < 10; i += 1; end
来源：http://zwa.pengpengdd.cyou

C#:   while (i < 10) { i++; }
来源：http://zca.ehwqpu.com

[B08] do-while（至少执行一次）
来源：http://gbr.tianlin.xyz

Py:   # 无 do-while：用 while True + break
来源：http://rpz.vehdjk.com

PHP:  do { $i++; } while ($i < 10);
来源：http://kuk.gotoacloud.top

JS:   do { i++; } while (i < 10);
来源：http://ynf.hammf.cn

TS:   do { i++; } while (i < 10);
来源：http://xkh.jianghu66.top

Java: do { i++; } while (i < 10);
来源：http://tdg.nwbrower.top

Go:   for { i++; if i >= 10 { break } }
来源：http://svn.yfazqb.com

Ruby: begin; i += 1; end while i < 10
来源：http://yxt.yj20258888.top

C#:   do { i++; } while (i < 10);
来源：http://ogt.shanyushiyangtech.top

[B09] break 与 continue
来源：http://hli.shangyingyoupin.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bwx.dashuyun.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rsh.cqqwz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wqg.sweek.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sqj.pengpengdd.cyou

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nnu.52xcode.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oki.yj20258.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gye.zhaomingkeji.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zlf.hammf.cn

[B10] 遍历同时拿索引
来源：http://wph.zdqjudy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iay.jinqigfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://aew.dianchejie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qcj.52xcode.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xds.havefunace.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rxc.shzxlz.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uxj.ivvv.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pfm.quarkkingdee.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yzs.daxiang520.top

[B11] 生成数字序列 / 区间
来源：http://ekg.dashuyun.cn

Py:   list(range(0, 10, 2))
来源：http://qdq.fanxiaobao.xyz

PHP:  range(0, 10, 2);
来源：http://hnp.cqqwz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ajt.hongshengwenyu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://urm.c1oappe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fyw.tanke756.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://klk.guannengcc.top

Ruby: (0...10).step(2).to_a
来源：http://pqe.yuxming.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bmg.xinyue.icu

[B12] 跳出多层循环
来源：http://kzv.mhx1999.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://aok.hcnkem.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://pev.dashuyun.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tmn.wangshuangyany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://eoj.svipenyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nhc.jqgfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hll.havefunace.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sfe.hesvh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://huv.fktsv.cn

[B13] 判断是否为数字
来源：http://oao.haohaochexian.top

Py:   isinstance(x, (int, float))
来源：http://paf.yangfankeji.com

PHP:  is_numeric($x)
来源：http://llt.zhoulong.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mhg.birdmap.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://orm.chenzaomai.com

Java: x instanceof Number
来源：http://mnz.shangyingyoupin.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bih.xingfuxueyuan.xyz

Ruby: x.is_a?(Numeric)
来源：http://bdr.0kj1m.cn

C#:   x is int or double or decimal
来源：http://yls.vqdsnc.cn

[B14] 判断值是否在集合内
来源：http://nfi.xziqi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cxu.tanke756.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xdv.dashuyun.cn

JS:   [1, 2, 3].includes(x)
来源：http://ngt.tian-w.cn

TS:   [1, 2, 3].includes(x)
来源：http://odc.cashguo.top

Java: List.of(1, 2, 3).contains(x)
来源：http://jqv.xuanzx.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ldf.fehbvm.com

Ruby: [1, 2, 3].include?(x)
来源：http://hez.jyoumei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fvm.jqgfzy.top

[B15] 布尔运算与取反
来源：http://lon.zdbjq.cn

Py:   a and b or not c
来源：http://uky.xziqi.cn

PHP:  $a && $b || !$c
来源：http://thp.zhijiandao.cn

JS:   a && b || !c
来源：http://vmz.kuanghao11.cn

TS:   a && b || !c
来源：http://vej.tianlin.xyz

Java: a && b || !c
来源：http://gbr.chenzaomai.com

Go:   a && b || !c
来源：http://bcu.redwolf501.top

Ruby: a && b || !c
来源：http://vgt.ctjpmb.com

C#:   a && b || !c
来源：http://crd.tarul.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jeg.jinghuilouyu.cn

Py:   if not data: return
来源：http://zoc.jiagoushi.top

PHP:  if (!$data) { return; }
来源：http://csl.dianchejie.cn

JS:   if (!data) return;
来源：http://qul.guowangkeji.top

TS:   if (!data) return;
来源：http://jri.quarkkingdee.top

Java: if (data == null) return;
来源：http://vvt.jianghu66.top

Go:   if data == nil { return }
来源：http://nel.sufxvd.cn

Ruby: return if data.nil?
来源：http://mub.epnwcf.com

C#:   if (data == null) return;
来源：http://sio.iojbl.cn

================================================================================
来源：http://ffl.feifeiyinyue.top

C. 函数与作用域
来源：http://lmw.nanxuanxn.top

================================================================================
来源：http://irl.guowangkeji.top

[C01] 定义函数
来源：http://ycs.ybcxt.top

Py:   def add(a, b): return a + b
来源：http://txh.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hop.fzhhl.top

JS:   function add(a, b) { return a + b; }
来源：http://jdk.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wcy.zdbjq.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ezq.dianchejie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lbb.ctjpmb.com

Ruby: def add(a, b); a + b; end
来源：http://vlp.sweek.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://boo.yj20258888.top

[C02] 默认参数
来源：http://yne.guowangkeji.top

Py:   def greet(name="World"): return name
来源：http://zdo.zhengqikj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://aah.sufxvd.cn

JS:   function greet(name = "World") { return name; }
来源：http://usb.fktsv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dlk.tarul.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kbv.aibaodan.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oxd.sufxvd.cn

Ruby: def greet(name = "World") = name
来源：http://pbw.sysykeji.top

C#:   string Greet(string name = "World") => name;
来源：http://nje.yuxming.cn

[C03] 可变参数
来源：http://you.uphjek.com

Py:   def total(*args): return sum(args)
来源：http://pub.uphjek.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://phd.yj20258.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zqa.zhaomingkeji.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wcv.jinyuanbaomall.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ogr.0kj1m.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://are.guannengcc.top

Ruby: def total(*nums); nums.sum; end
来源：http://ibs.wangdashe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oto.quarkkingdee.top

[C04] 命名参数 / 关键字参数
来源：http://czw.andypj.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vlh.feifeiyinyue.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vdp.shanyushiyangtech.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hud.zhiwuduotai.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mjy.jlsjyb.cn

Java: // 无：用 Builder 模式或 record
来源：http://hnm.meibo888.top

Go:   // 无：用配置结构体参数
来源：http://nnz.yfazqb.com

Ruby: f(a: 1, b: 2)
来源：http://wze.shuidangran.top

C#:   f(a: 1, b: 2)
来源：http://rym.xziqi.cn

[C05] 返回多个值
来源：http://qdl.ywan-chungtsiang.top

Py:   return a, b
来源：http://skm.yfazqb.com

PHP:  return [$a, $b];
来源：http://csr.tian-w.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sds.0kj1m.cn

TS:   return { a, b };
来源：http://ipq.chenlongwang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nes.ivvv.top

Go:   return a, b
来源：http://vwt.cdnleiting.top

Ruby: return a, b
来源：http://pgx.jyoumei.cn

C#:   return (a, b);              // ValueTuple
来源：http://drp.hfpthk.cn

[C06] 匿名函数 / lambda
来源：http://kyp.yj20258.top

Py:   square = lambda x: x * x
来源：http://lld.hammf.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zdd.guowangkeji.top

JS:   const square = x => x * x;
来源：http://xqm.wangdashe.top

TS:   const square = (x: number): number => x * x;
来源：http://jkp.fktsv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yfc.hysaishi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dhk.wangdashe.top

Ruby: square = ->(x) { x * x }
来源：http://rhb.hnqzz.top

C#:   Func<int, int> square = x => x * x;
来源：http://alf.sweek.top

[C07] 把函数作为参数传入
来源：http://zgj.cdnleiting.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://apc.hesvh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qju.tanke756.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hcg.xinyue.icu

TS:   arr.map(String)
来源：http://okh.hnxiangtu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://opj.hfpthk.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lds.shanyushiyangkeji.top

Ruby: arr.map(&:upcase)
来源：http://meu.yonumen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://utx.hfpthk.cn

[C08] 闭包
来源：http://wav.ivvv.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://soq.jyoumei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bbl.zhixingplan.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xuz.jinqigfzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mjo.hcnkem.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qfa.zhixingplan.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ofd.haohaochexian.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rmy.jinyuanbaomall.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kjj.zdbjq.cn

[C09] 递归
来源：http://bpf.birdmap.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rpk.sxryk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mep.wangshuangyany.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nyh.snrcjt.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zqm.wangshuangyany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://btf.zhaomingkeji.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tpf.hnqzz.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qvv.tian-w.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vmd.haohaochexian.top

[C10] 变量作用域
来源：http://xfg.c1oappe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vzq.jianghu66.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yhk.fehbvm.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uaw.shanyushiyangtech.top

TS:   同 JS
来源：http://zye.jqgfzy.top

Java: 方法内为块级作用域
来源：http://euw.ydjk.org.cn

Go:   花括号块级作用域
来源：http://hbe.xuetiantiany.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://slk.hcnkem.com

C#:   块级作用域
来源：http://jhe.yj20258.top

[C11] 模块导入与导出
来源：http://xku.jinqigfzy.top

Py:   from module import func
来源：http://xtl.vqdsnc.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wva.yongpay.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xjn.nanxinkj.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jcm.chenzaomai.com

Java: import java.util.List;
来源：http://fjd.cheryme.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://msg.jinqigfzy.top

Ruby: require "json"; require_relative "./util"
来源：http://xlb.hongshengwenyu.top

C#:   using System.Text;
来源：http://nsq.nwbrower.top

[C12] 立即执行函数 IIFE
来源：http://jis.zhengqikj.top

Py:   (lambda: print("run"))()
来源：http://wja.yj20258.top

PHP:  (function () { echo "run"; })();
来源：http://gam.yanxiufei.cn

JS:   (() => { console.log("run"); })();
来源：http://vpu.aibaodan.cn

TS:   (() => { console.log("run"); })();
来源：http://efg.jlsjyb.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qul.zhoulong.xyz

Go:   func() { fmt.Println("run") }()
来源：http://iqx.sxryk.cn

Ruby: -> { puts "run" }.call
来源：http://wca.tarul.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://adz.andypj.xyz

[C13] 类型声明 / 类型注解
来源：http://kkb.jyoumei.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wgb.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://how.jiagoushi.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kcv.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zxr.yj20258888.top

Java: int add(int a, int b) { return a + b; }
来源：http://icf.gogol.net.cn

Go:   func add(a, b int) int
来源：http://yzu.havefunace.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zxi.sjlbkw.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fma.jqgfzy.top

[C14] 泛型函数
来源：http://emo.pycfn.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wdm.redwolf501.top

PHP:  // 无泛型
来源：http://odx.ywan-chungtsiang.top

JS:   // 无泛型
来源：http://qrp.shanyushiyangtech.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xld.bbcook.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mmm.sxryk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://htk.jiagoushi.top

Ruby: # 无泛型
来源：http://chj.nwbrower.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pfi.meibo888.top

[C15] 解构 / 展开参数
来源：http://udm.sufxvd.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nok.nwbrower.top

PHP:  [$a, $b] = $pair;
来源：http://qvj.svipenyu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cso.yj202588.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://juw.0kj1m.cn

Java: // 无解构
来源：http://zlt.dashuyun.cn

Go:   // 无解构
来源：http://mkx.jinqigfzy.top


<!-- 参考信息 -->