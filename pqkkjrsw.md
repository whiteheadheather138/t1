代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pga.yangfankeji.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://icd.nanxinkj.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eag.cqqwz.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ldk.yfazqb.com

Go:   strings.TrimSpace(s)
来源：http://imn.sjlbkw.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vyb.sxryk.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mvr.yj20258.top

[A25] 字符串比较
来源：http://mbv.kuanghao11.cn

Py:   s1 == s2; s1 != s2
来源：http://bov.zhixingplan.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nhn.yvedp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tdm.hcnkem.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://omi.feifeiyinyue.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://brb.ybcxt.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wvu.chenzaomai.com

Ruby: s1 == s2; s1 <=> s2
来源：http://fqq.redwolf501.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ikr.zycfv.cn

[A26] 类型转换总览
来源：http://lia.havefunace.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jiy.uphjek.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://puo.cucudq.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://epm.ydzc1.top

TS:   Number() String() Boolean() x as number
来源：http://cgp.zdqjudy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lkk.snrcjt.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://paf.quarkkingdee.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://odz.pengpengdd.cyou

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tsk.c1oappe.top

================================================================================
来源：http://zfc.daria6918.cn

B. 流程控制
来源：http://zef.haohaochexian.top

================================================================================
来源：http://pdx.iojbl.cn

[B01] 条件判断 if / else
来源：http://qeq.xziqi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zed.mhx1999.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xmy.meibo888.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zvz.ehwqpu.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tne.jianghu66.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://vlo.tanke756.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cbq.zdbjq.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kst.yueranfly.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jao.daxiang520.top

[B02] 多分支 else if / elif
来源：http://meq.yuanzhike.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lmn.havefunace.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tvl.jinqigfzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iqa.ctjpmb.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hqr.fanxiaobao.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cey.fanxiaobao.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ate.bbcook.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rgk.guannengcc.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oja.zhijiandao.cn

[B03] switch / match / case
来源：http://zat.jiagoushi.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rrj.sysykeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bmv.xingfuxueyuan.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ilq.daria6918.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iyk.feifeiyinyue.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wwy.redwolf501.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://quc.chenlongwang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jdp.daria6918.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mzy.nwbrower.top

[B04] for 计数循环
来源：http://wbl.hywenlv.cn

Py:   for i in range(10): print(i)
来源：http://hvw.hnxiangtu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hyb.dashuyun.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wqq.bbcook.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fia.jinghuilouyu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fne.cucudq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hcu.yuxming.cn

Ruby: 10.times { |i| puts i }
来源：http://cnq.tarul.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://iyx.jinqigufen.top

[B05] 遍历数组 / 列表
来源：http://khd.zhijiandao.cn

Py:   for item in arr: print(item)
来源：http://wpr.hywenlv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oiy.52xcode.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kyb.xylfe.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cou.yuxming.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://eki.nanxinkj.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://slp.yvedp.cn

Ruby: arr.each { |item| puts item }
来源：http://hlc.nanxuanxn.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jwp.yfazqb.com

[B06] 遍历字典 / 对象
来源：http://mna.fzhhl.top

Py:   for k, v in d.items(): print(k, v)
来源：http://irp.vehdjk.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fdi.hysaishi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ahl.xziqi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bcd.quarkkingdee.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bfx.cqqwz.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jjp.zdbjq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tba.nanxinkj.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vfs.jinqigfzy.top

[B07] while 循环
来源：http://nie.shuidangran.top

Py:   while i < 10: i += 1
来源：http://thj.zhiwuduotai.top

PHP:  while ($i < 10) { $i++; }
来源：http://elm.chenjidiqi.icu

JS:   while (i < 10) { i++; }
来源：http://mfg.hywenlv.cn

TS:   while (i < 10) { i++; }
来源：http://nxk.hcnkem.com

Java: while (i < 10) { i++; }
来源：http://zin.jyoumei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ccs.zhijiandao.cn

Ruby: while i < 10; i += 1; end
来源：http://cdf.hesvh.cn

C#:   while (i < 10) { i++; }
来源：http://xwy.gotoacloud.top

[B08] do-while（至少执行一次）
来源：http://mth.shangyingyoupin.top

Py:   # 无 do-while：用 while True + break
来源：http://wzj.vehdjk.com

PHP:  do { $i++; } while ($i < 10);
来源：http://eub.hcnkem.com

JS:   do { i++; } while (i < 10);
来源：http://xzn.sufxvd.cn

TS:   do { i++; } while (i < 10);
来源：http://wmz.fzhhl.top

Java: do { i++; } while (i < 10);
来源：http://acn.cdnleiting.top

Go:   for { i++; if i >= 10 { break } }
来源：http://emy.quarkkingdee.top

Ruby: begin; i += 1; end while i < 10
来源：http://lae.vqdsnc.cn

C#:   do { i++; } while (i < 10);
来源：http://ebi.yangfankeji.com

[B09] break 与 continue
来源：http://msm.hnqzz.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zai.hnqzz.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hpw.wangshuangyany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uie.0kj1m.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://syz.dianchejie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fiz.cucudq.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ryz.shuidangran.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fzp.jianghu66.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ude.zhixingplan.top

[B10] 遍历同时拿索引
来源：http://ynf.yanxiufei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qsv.chenjidiqi.icu

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xco.haohaochexian.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jow.sufxvd.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://psk.xuanzx.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qgq.cqqwz.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pfr.hfpthk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bwp.meibo888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jsn.hysaishi.cn

[B11] 生成数字序列 / 区间
来源：http://alv.jinqigufen.top

Py:   list(range(0, 10, 2))
来源：http://keg.meibo888.top

PHP:  range(0, 10, 2);
来源：http://ydz.daxiang520.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ydn.yfazqb.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vys.yonumen.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://akc.jinqigufen.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://itf.snrcjt.cn

Ruby: (0...10).step(2).to_a
来源：http://zdg.nanxuanxn.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://isu.ybcxt.top

[B12] 跳出多层循环
来源：http://yws.svipenyu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ygk.ydzc1.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://qgo.xziqi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oos.aizwys.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jim.sysykeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rta.birdmap.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kpm.gotoacloud.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ctx.zhaomingkeji.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mug.guannengcc.top

[B13] 判断是否为数字
来源：http://hcw.shanyushiyangkeji.top

Py:   isinstance(x, (int, float))
来源：http://wqg.jinghuilouyu.cn

PHP:  is_numeric($x)
来源：http://fxp.mhx1999.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dex.cdnleiting.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cvg.xingfuxueyuan.xyz

Java: x instanceof Number
来源：http://wnt.fanxiaobao.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jmx.sxryk.cn

Ruby: x.is_a?(Numeric)
来源：http://mzt.nanxuanxn.top

C#:   x is int or double or decimal
来源：http://tlb.shuidangran.top

[B14] 判断值是否在集合内
来源：http://jye.yj20258.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tsw.sweek.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://axt.zhongyouzk.top

JS:   [1, 2, 3].includes(x)
来源：http://xvj.yuxming.cn

TS:   [1, 2, 3].includes(x)
来源：http://yoe.xziqi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ztm.andypj.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fmz.yj20258888.top

Ruby: [1, 2, 3].include?(x)
来源：http://awe.bjfxy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lsc.cqqwz.cn

[B15] 布尔运算与取反
来源：http://ayx.ivvv.top

Py:   a and b or not c
来源：http://gkn.xziqi.cn

PHP:  $a && $b || !$c
来源：http://cxg.jinqigufen.top

JS:   a && b || !c
来源：http://ybb.hcnkem.com

TS:   a && b || !c
来源：http://eir.ydzc1.top

Java: a && b || !c
来源：http://aeo.zhongyouzk.top

Go:   a && b || !c
来源：http://wgp.jqgfzy.top

Ruby: a && b || !c
来源：http://tdh.redwolf501.top

C#:   a && b || !c
来源：http://pbw.hfpthk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://juh.jianghu66.top

Py:   if not data: return
来源：http://deo.jinghuilouyu.cn

PHP:  if (!$data) { return; }
来源：http://dtd.jlsjyb.cn

JS:   if (!data) return;
来源：http://crp.zhongyouzk.top

TS:   if (!data) return;
来源：http://nmu.gzhubu.top

Java: if (data == null) return;
来源：http://cgk.xuanzx.com

Go:   if data == nil { return }
来源：http://hdw.wangshuangyany.cn

Ruby: return if data.nil?
来源：http://ldf.zhengqikj.top

C#:   if (data == null) return;
来源：http://wod.yanxiufei.cn

================================================================================
来源：http://dqq.dianchejie.cn

C. 函数与作用域
来源：http://sch.yangfankeji.com

================================================================================
来源：http://uqh.shangyingyoupin.top

[C01] 定义函数
来源：http://chq.quarkkingdee.top

Py:   def add(a, b): return a + b
来源：http://bvq.jinyuanbaomall.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mya.zhaomingkeji.xyz

JS:   function add(a, b) { return a + b; }
来源：http://kmd.c1oappe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ofw.yongpay.top

Java: static int add(int a, int b) { return a + b; }
来源：http://pve.svipenyu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zia.cqqwz.cn

Ruby: def add(a, b); a + b; end
来源：http://fdn.zycfv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xwg.bjfxy.top

[C02] 默认参数
来源：http://wcz.xylfe.cn

Py:   def greet(name="World"): return name
来源：http://zvd.wangshuangyany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ljo.meibo888.top

JS:   function greet(name = "World") { return name; }
来源：http://dms.cdnleiting.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vsa.fktsv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rrm.havefunace.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mhl.yj20258888.top

Ruby: def greet(name = "World") = name
来源：http://jxv.fehbvm.com

C#:   string Greet(string name = "World") => name;
来源：http://zlr.yonumen.top

[C03] 可变参数
来源：http://vhc.zhixingplan.top

Py:   def total(*args): return sum(args)
来源：http://toh.vehdjk.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oev.nanxinkj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ymm.sweek.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oml.tanke756.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bhe.yj20258.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qyf.hnxiangtu.top

Ruby: def total(*nums); nums.sum; end
来源：http://kks.yuxming.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uhd.pengpengdd.cyou

[C04] 命名参数 / 关键字参数
来源：http://yum.yj20258888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fgl.zhengqikj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zqg.xziqi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dnb.0kj1m.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ask.smart0.xyz

Java: // 无：用 Builder 模式或 record
来源：http://wml.shanyushiyangkeji.top

Go:   // 无：用配置结构体参数
来源：http://zry.wangdashe.top

Ruby: f(a: 1, b: 2)
来源：http://oxb.yj20258888.top

C#:   f(a: 1, b: 2)
来源：http://uhj.yj20258888.top

[C05] 返回多个值
来源：http://nfa.cucudq.cn

Py:   return a, b
来源：http://lzz.shangyingyoupin.top

PHP:  return [$a, $b];
来源：http://ncz.xylfe.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://aeg.zhaomingkeji.xyz

TS:   return { a, b };
来源：http://tnh.hfpthk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vqp.aizwys.cn

Go:   return a, b
来源：http://urm.52xcode.cn

Ruby: return a, b
来源：http://noh.hysaishi.cn

C#:   return (a, b);              // ValueTuple
来源：http://rkv.iojbl.cn

[C06] 匿名函数 / lambda
来源：http://ujj.fengsongda.top

Py:   square = lambda x: x * x
来源：http://vgt.aibaodan.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://koh.snrcjt.cn

JS:   const square = x => x * x;
来源：http://ldn.epnwcf.com

TS:   const square = (x: number): number => x * x;
来源：http://gyr.zhongyouzk.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://csk.sxryk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lfm.havefunace.top

Ruby: square = ->(x) { x * x }
来源：http://tjx.ydjk.org.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tbp.kuanghao11.cn

[C07] 把函数作为参数传入
来源：http://das.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kzy.yangfankeji.com

PHP:  array_map("strtoupper", $arr);
来源：http://zxl.tian-w.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xkj.0kj1m.cn

TS:   arr.map(String)
来源：http://jrv.zdbjq.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jtl.nanxuanxn.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://aph.xinyue.icu

Ruby: arr.map(&:upcase)
来源：http://uyk.cdnleiting.top

C#:   arr.Select(s => s.ToUpper())
来源：http://psw.zycfv.cn

[C08] 闭包
来源：http://hnw.tian-w.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sbj.sweek.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ham.chenjidiqi.icu

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qfs.jinghuilouyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kts.yj20258.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kgb.yongpay.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://crr.havefunace.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qtq.jianghu66.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nfz.shuidangran.top

[C09] 递归
来源：http://cit.yj20258.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pph.gaohongyu789.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ubh.hcnkem.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mwz.zhaomingkeji.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hpc.andypj.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hld.yuxming.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zgi.haohaochexian.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qtd.sufxvd.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oub.yueranfly.top

[C10] 变量作用域
来源：http://nrd.iojbl.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ldq.feifeiyinyue.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zaz.fanxiaobao.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mrn.pycfn.com

TS:   同 JS
来源：http://byd.9152youxi.cn

Java: 方法内为块级作用域
来源：http://pcr.wangdashe.top

Go:   花括号块级作用域
来源：http://qrl.316326.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iau.xuetiantiany.cn

C#:   块级作用域
来源：http://fjb.ywan-chungtsiang.top

[C11] 模块导入与导出
来源：http://agb.xuetiantiany.cn

Py:   from module import func
来源：http://nvm.ydjk.org.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uxx.zycfv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pku.gogol.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kll.jqgufenzy.top

Java: import java.util.List;
来源：http://uze.zycfv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tjx.kuanghao11.cn

Ruby: require "json"; require_relative "./util"
来源：http://upx.quarkkingdee.top

C#:   using System.Text;
来源：http://cnt.gogol.net.cn

[C12] 立即执行函数 IIFE
来源：http://gyt.yonumen.top

Py:   (lambda: print("run"))()
来源：http://wab.yj20258.top

PHP:  (function () { echo "run"; })();
来源：http://khm.epnwcf.com

JS:   (() => { console.log("run"); })();
来源：http://zzk.fanxiaobao.xyz

TS:   (() => { console.log("run"); })();
来源：http://hls.sweek.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://feq.c1oappe.top

Go:   func() { fmt.Println("run") }()
来源：http://amj.sxryk.cn

Ruby: -> { puts "run" }.call
来源：http://mhe.shzxlz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wph.svipenyu.cn

[C13] 类型声明 / 类型注解
来源：http://wka.jinyuanbaomall.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oti.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hli.redwolf501.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://otx.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vwb.sxryk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ldz.zhixingplan.top

Go:   func add(a, b int) int
来源：http://syn.ehwqpu.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bgx.hcnkem.com

C#:   int Add(int a, int b) => a + b;
来源：http://gjt.bbcook.cn

[C14] 泛型函数
来源：http://qga.shanyushiyangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tkd.yj202588.top

PHP:  // 无泛型
来源：http://etf.yfazqb.com

JS:   // 无泛型
来源：http://sgi.ywan-chungtsiang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dir.aizwys.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ruy.yj202588.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ofv.zhoulong.xyz

Ruby: # 无泛型
来源：http://blc.birdmap.top


<!-- 参考信息 -->