代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bgs.vehdjk.com

C#:   s.ToUpper(); s.ToLower()
来源：http://rmv.xingfuxueyuan.xyz

[A24] 去除首尾空白
来源：http://wdz.shanyushiyangkeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://juo.daxiang520.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ewr.shangyingyoupin.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sub.yvedp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rgf.andypj.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vbb.chenzaomai.com

Go:   strings.TrimSpace(s)
来源：http://egs.ehwqpu.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ogo.vqdsnc.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://skh.ywan-chungtsiang.top

[A25] 字符串比较
来源：http://imm.yangfankeji.com

Py:   s1 == s2; s1 != s2
来源：http://goq.iojbl.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vcy.xziqi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fdk.ivvv.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mny.guannengcc.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ycv.wangshuangyany.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ibn.gzhubu.top

Ruby: s1 == s2; s1 <=> s2
来源：http://tqs.ybcxt.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pco.tanke756.top

[A26] 类型转换总览
来源：http://sjm.quarkkingdee.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://quu.zhaomingkeji.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dfq.ctjpmb.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://abm.ctjpmb.com

TS:   Number() String() Boolean() x as number
来源：http://mqt.shangyingyoupin.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eua.jinqigufen.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gmr.zdbjq.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nfx.gogol.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zbd.dashuyun.cn

================================================================================
来源：http://cys.uphjek.com

B. 流程控制
来源：http://ttx.chenlongwang.top

================================================================================
来源：http://oqq.quarkkingdee.top

[B01] 条件判断 if / else
来源：http://dct.tarul.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bfh.feifeiyinyue.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kkd.hysaishi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://llu.quarkkingdee.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://daq.jqgufenzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://tfm.bbcook.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://imt.shzxlz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dcm.guowangkeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uvb.dashuyun.cn

[B02] 多分支 else if / elif
来源：http://ggb.jianghu66.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lqp.uphjek.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wur.quarkkingdee.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qnd.yueranfly.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nne.c1oappe.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kmj.daria6918.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ywj.ydjk.org.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vpw.gogol.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ekc.redwolf501.top

[B03] switch / match / case
来源：http://iwk.dianchejie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://stj.jyoumei.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ibp.cashguo.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ldx.pycfn.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dlo.316326.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iwc.pycfn.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hdk.jlsjyb.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zsp.nanxuanxn.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uxn.tarul.cn

[B04] for 计数循环
来源：http://fal.cdnleiting.top

Py:   for i in range(10): print(i)
来源：http://ixh.bbcook.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ect.fktsv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uoz.iojbl.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mvv.yj202588.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://clz.ywan-chungtsiang.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qud.aibaodan.cn

Ruby: 10.times { |i| puts i }
来源：http://bbq.jqgufenzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://twu.tianlin.xyz

[B05] 遍历数组 / 列表
来源：http://pmj.yfazqb.com

Py:   for item in arr: print(item)
来源：http://vch.52xcode.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vkv.chenzaomai.com

JS:   for (const item of arr) { console.log(item); }
来源：http://lnc.dianchejie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yjx.daria6918.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mwi.meibo888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hqb.zhoulong.xyz

Ruby: arr.each { |item| puts item }
来源：http://pwe.sysykeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qpw.fehbvm.com

[B06] 遍历字典 / 对象
来源：http://wly.jqgfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://irm.yanxiufei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bki.316326.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://efy.shuidangran.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nqf.hammf.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vpv.cqqwz.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://atn.andypj.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kpq.guowangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gqr.tarul.cn

[B07] while 循环
来源：http://rqx.vqdsnc.cn

Py:   while i < 10: i += 1
来源：http://sxe.haohaochexian.top

PHP:  while ($i < 10) { $i++; }
来源：http://ran.cucudq.cn

JS:   while (i < 10) { i++; }
来源：http://yzd.sjlbkw.cn

TS:   while (i < 10) { i++; }
来源：http://kle.fengsongda.top

Java: while (i < 10) { i++; }
来源：http://lxq.hammf.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ndo.birdmap.top

Ruby: while i < 10; i += 1; end
来源：http://mic.snrcjt.cn

C#:   while (i < 10) { i++; }
来源：http://rxk.gaohongyu789.top

[B08] do-while（至少执行一次）
来源：http://jmv.yfazqb.com

Py:   # 无 do-while：用 while True + break
来源：http://ccw.0kj1m.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xsm.yonumen.top

JS:   do { i++; } while (i < 10);
来源：http://jcf.jiagoushi.top

TS:   do { i++; } while (i < 10);
来源：http://qfj.daria6918.cn

Java: do { i++; } while (i < 10);
来源：http://meq.daria6918.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tde.shanyushiyangtech.top

Ruby: begin; i += 1; end while i < 10
来源：http://omn.yueranfly.top

C#:   do { i++; } while (i < 10);
来源：http://cmv.sweek.top

[B09] break 与 continue
来源：http://kob.meibo888.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wwb.316326.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://occ.hongshengwenyu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ruh.fehbvm.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kar.bbcook.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://way.yj20258888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ukb.sxryk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bpn.hcnkem.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wal.yueranfly.top

[B10] 遍历同时拿索引
来源：http://osi.nanxinkj.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://afr.ppjwa.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://otm.yanxiufei.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ivj.yuxming.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://paa.vehdjk.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wqr.havefunace.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lmt.jyoumei.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jwm.mhx1999.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nkd.yueranfly.top

[B11] 生成数字序列 / 区间
来源：http://cfa.hongshengwenyu.top

Py:   list(range(0, 10, 2))
来源：http://yiv.tianlin.xyz

PHP:  range(0, 10, 2);
来源：http://wnw.316326.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cie.sxryk.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aqa.quarkkingdee.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hbi.vqdsnc.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vrg.vehdjk.com

Ruby: (0...10).step(2).to_a
来源：http://zoj.pycfn.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wel.zhaomingkeji.xyz

[B12] 跳出多层循环
来源：http://ahg.guannengcc.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wot.smart0.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://zdy.jyoumei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fvg.sjlbkw.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kfi.ivvv.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fid.ydjk.org.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hjt.0kj1m.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zee.jiagoushi.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yrt.feifeiyinyue.top

[B13] 判断是否为数字
来源：http://ziu.yj202588.top

Py:   isinstance(x, (int, float))
来源：http://lmh.nwbrower.top

PHP:  is_numeric($x)
来源：http://ncu.gzhubu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wfi.aizwys.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jzw.hfpthk.cn

Java: x instanceof Number
来源：http://kcb.vehdjk.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gnb.ybcxt.top

Ruby: x.is_a?(Numeric)
来源：http://sls.52xcode.cn

C#:   x is int or double or decimal
来源：http://rqv.yvedp.cn

[B14] 判断值是否在集合内
来源：http://axe.shanyushiyangtech.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wfm.xziqi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lkj.tian-w.cn

JS:   [1, 2, 3].includes(x)
来源：http://dvi.yangfankeji.com

TS:   [1, 2, 3].includes(x)
来源：http://ljp.jinqigufen.top

Java: List.of(1, 2, 3).contains(x)
来源：http://gti.hfpthk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tzc.ehwqpu.com

Ruby: [1, 2, 3].include?(x)
来源：http://nvv.0kj1m.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uml.redwolf501.top

[B15] 布尔运算与取反
来源：http://kbl.ehwqpu.com

Py:   a and b or not c
来源：http://ezn.yanxiufei.cn

PHP:  $a && $b || !$c
来源：http://oql.jyoumei.cn

JS:   a && b || !c
来源：http://yzp.svipenyu.cn

TS:   a && b || !c
来源：http://yji.xuetiantiany.cn

Java: a && b || !c
来源：http://esn.yuxming.cn

Go:   a && b || !c
来源：http://tnp.bjfxy.top

Ruby: a && b || !c
来源：http://hlb.quarkkingdee.top

C#:   a && b || !c
来源：http://oou.hnqzz.top

[B16] 卫语句：不满足条件提前返回
来源：http://ygm.zhoulong.xyz

Py:   if not data: return
来源：http://qpn.ybcxt.top

PHP:  if (!$data) { return; }
来源：http://ccg.jqgufenzy.top

JS:   if (!data) return;
来源：http://ngm.shzxlz.cn

TS:   if (!data) return;
来源：http://uld.sufxvd.cn

Java: if (data == null) return;
来源：http://ipp.yuxming.cn

Go:   if data == nil { return }
来源：http://gjx.aibaodan.cn

Ruby: return if data.nil?
来源：http://qex.nanxuanxn.top

C#:   if (data == null) return;
来源：http://xlt.pengpengdd.cyou

================================================================================
来源：http://ybt.hnqzz.top

C. 函数与作用域
来源：http://atw.yj20258.top

================================================================================
来源：http://jss.tarul.cn

[C01] 定义函数
来源：http://ena.jinyuanbaomall.cn

Py:   def add(a, b): return a + b
来源：http://xck.ydjk.org.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://syi.ehwqpu.com

JS:   function add(a, b) { return a + b; }
来源：http://dbp.jinyuanbaomall.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nhz.chenlongwang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://btg.andypj.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://rso.gotoacloud.top

Ruby: def add(a, b); a + b; end
来源：http://jnh.shuidangran.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rkh.fengsongda.top

[C02] 默认参数
来源：http://twg.jqgfzy.top

Py:   def greet(name="World"): return name
来源：http://efy.sxryk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cfe.wangshuangyany.cn

JS:   function greet(name = "World") { return name; }
来源：http://bzj.ctjpmb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://ijo.hcnkem.com

Java: // 无默认参数：方法重载或 Optional
来源：http://rao.52xcode.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fit.ydzc1.top

Ruby: def greet(name = "World") = name
来源：http://jpw.xuanzx.com

C#:   string Greet(string name = "World") => name;
来源：http://qrp.yueranfly.top

[C03] 可变参数
来源：http://tqi.yuanzhike.top

Py:   def total(*args): return sum(args)
来源：http://btx.chenlongwang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iiq.xziqi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qfa.52xcode.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jgq.zhijiandao.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dtz.jinqigfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vtx.tianlin.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://qwg.sufxvd.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://inc.gzhubu.top

[C04] 命名参数 / 关键字参数
来源：http://jxf.zhoulong.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fwf.aizwys.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pmy.xingfuxueyuan.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zpq.gaohongyu789.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://osx.aibaodan.cn

Java: // 无：用 Builder 模式或 record
来源：http://ofd.yuanzhike.top

Go:   // 无：用配置结构体参数
来源：http://kpa.guowangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://wdt.redwolf501.top

C#:   f(a: 1, b: 2)
来源：http://fpl.yonumen.top

[C05] 返回多个值
来源：http://oqf.ydjk.org.cn

Py:   return a, b
来源：http://ews.zycfv.cn

PHP:  return [$a, $b];
来源：http://jiv.fehbvm.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://try.daria6918.cn

TS:   return { a, b };
来源：http://fsu.yuanzhike.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hkx.xingfuxueyuan.xyz

Go:   return a, b
来源：http://dau.shuidangran.top

Ruby: return a, b
来源：http://oeb.guowangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://yhz.haohaochexian.top

[C06] 匿名函数 / lambda
来源：http://seq.feifeiyinyue.top

Py:   square = lambda x: x * x
来源：http://idv.gotoacloud.top

PHP:  $square = fn($x) => $x * $x;
来源：http://yfl.tianlin.xyz

JS:   const square = x => x * x;
来源：http://edu.zhixingplan.top

TS:   const square = (x: number): number => x * x;
来源：http://pyc.sxryk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dax.feifeiyinyue.top

Go:   sq := func(x int) int { return x * x }
来源：http://vll.sweek.top

Ruby: square = ->(x) { x * x }
来源：http://lld.yuanzhike.top

C#:   Func<int, int> square = x => x * x;
来源：http://hey.zhixingplan.top

[C07] 把函数作为参数传入
来源：http://nuo.gogol.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tjm.gzhubu.top

PHP:  array_map("strtoupper", $arr);
来源：http://urw.zhengqikj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xco.chenlongwang.top

TS:   arr.map(String)
来源：http://lci.zhongyouzk.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://awz.yj202588.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yrs.chenjidiqi.icu

Ruby: arr.map(&:upcase)
来源：http://fys.jyoumei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nsx.gotoacloud.top

[C08] 闭包
来源：http://rtn.chenlongwang.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jpj.yongpay.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vmd.ybcxt.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vqo.haohaochexian.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rgn.aizwys.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cbq.fktsv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zpr.kuanghao11.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://isl.hysaishi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oxw.guowangkeji.top

[C09] 递归
来源：http://rhl.yueranfly.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://luf.shanyushiyangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gwa.sjlbkw.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nhh.zhongyouzk.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pwx.shanyushiyangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ieu.jinyuanbaomall.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://aqr.jyoumei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lfy.jiagoushi.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lwi.xuetiantiany.cn

[C10] 变量作用域
来源：http://aph.zhoulong.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://biv.guowangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xfx.jinyuanbaomall.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://chn.aibaodan.cn

TS:   同 JS
来源：http://vdz.tianlin.xyz

Java: 方法内为块级作用域
来源：http://ubw.fanxiaobao.xyz

Go:   花括号块级作用域
来源：http://qpd.shanyushiyangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tlh.cqqwz.cn

C#:   块级作用域
来源：http://qax.zhiwuduotai.top

[C11] 模块导入与导出
来源：http://bxe.ydzc1.top

Py:   from module import func
来源：http://yfb.xinyue.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://qst.shzxlz.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pyr.jinyuanbaomall.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tlp.ctjpmb.com

Java: import java.util.List;
来源：http://dfk.iojbl.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://chf.aizwys.cn

Ruby: require "json"; require_relative "./util"
来源：http://ius.tanke756.top

C#:   using System.Text;
来源：http://fcd.mhx1999.top

[C12] 立即执行函数 IIFE
来源：http://swp.yuxming.cn

Py:   (lambda: print("run"))()
来源：http://ipy.gaohongyu789.top

PHP:  (function () { echo "run"; })();
来源：http://blb.hnqzz.top

JS:   (() => { console.log("run"); })();
来源：http://uly.9152youxi.cn

TS:   (() => { console.log("run"); })();
来源：http://yys.mhx1999.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kjc.aizwys.cn

Go:   func() { fmt.Println("run") }()
来源：http://nto.jqgufenzy.top

Ruby: -> { puts "run" }.call
来源：http://btr.quarkkingdee.top

C#:   // 无 IIFE：用静态构造函数
来源：http://fep.hywenlv.cn

[C13] 类型声明 / 类型注解
来源：http://kmw.nanxuanxn.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ojs.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://juk.chenzaomai.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hgy.ppjwa.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oop.nwbrower.top

Java: int add(int a, int b) { return a + b; }
来源：http://dsm.fehbvm.com

Go:   func add(a, b int) int
来源：http://zzp.ehwqpu.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://opf.svipenyu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xyv.gzhubu.top

[C14] 泛型函数
来源：http://cda.guowangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ezk.pengpengdd.cyou

PHP:  // 无泛型
来源：http://uft.sjlbkw.cn

JS:   // 无泛型
来源：http://gql.redwolf501.top


<!-- 参考信息 -->