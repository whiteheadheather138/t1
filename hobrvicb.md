代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sux.jinyuanbaomall.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xah.xinyue.icu

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sqx.hywenlv.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kcn.yangfankeji.com

Go:   strings.TrimSpace(s)
来源：http://qph.svipenyu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cnp.yueranfly.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://auq.zhijiandao.cn

[A25] 字符串比较
来源：http://utx.hcnkem.com

Py:   s1 == s2; s1 != s2
来源：http://dns.wangshuangyany.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://usj.guannengcc.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://aet.vqdsnc.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yox.gaohongyu789.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ytx.zhixingplan.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gwj.jiagoushi.top

Ruby: s1 == s2; s1 <=> s2
来源：http://tvl.tarul.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bpt.hnqzz.top

[A26] 类型转换总览
来源：http://vkh.jlsjyb.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hsj.fengsongda.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fbh.cucudq.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://njt.jinqigufen.top

TS:   Number() String() Boolean() x as number
来源：http://khv.pengpengdd.cyou

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uis.sxryk.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mhy.snrcjt.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bzf.chenjidiqi.icu

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cwj.tanke756.top

================================================================================
来源：http://aiu.tianlin.xyz

B. 流程控制
来源：http://slp.vehdjk.com

================================================================================
来源：http://bqg.jqgfzy.top

[B01] 条件判断 if / else
来源：http://hsc.andypj.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://hid.ybcxt.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ihj.chenzaomai.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ogh.chenjidiqi.icu

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mkq.havefunace.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://tuu.316326.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://twc.vqdsnc.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://drl.nanxuanxn.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qyv.svipenyu.cn

[B02] 多分支 else if / elif
来源：http://tmw.feifeiyinyue.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fon.jinqigufen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dsb.cucudq.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ouy.shuidangran.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://skp.yueranfly.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://htx.gaohongyu789.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://upy.zhiwuduotai.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://noo.xuanzx.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://khe.cdnleiting.top

[B03] switch / match / case
来源：http://sgd.daxiang520.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dzh.yanxiufei.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oyj.xuetiantiany.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rqz.jqgufenzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zol.gzhubu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hio.ybcxt.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zwk.0kj1m.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://iqb.yangfankeji.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dac.bjfxy.top

[B04] for 计数循环
来源：http://jnu.smart0.xyz

Py:   for i in range(10): print(i)
来源：http://xvl.shzxlz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://icd.chenzaomai.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xsc.fengsongda.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lii.hcnkem.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wer.nanxinkj.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fmw.feifeiyinyue.top

Ruby: 10.times { |i| puts i }
来源：http://zth.dashuyun.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jjw.hysaishi.cn

[B05] 遍历数组 / 列表
来源：http://vme.yuxming.cn

Py:   for item in arr: print(item)
来源：http://drm.pengpengdd.cyou

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pnd.dashuyun.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jka.yongpay.top

TS:   for (const item of arr) { console.log(item); }
来源：http://kxx.zhaomingkeji.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://lvo.yj20258.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hhl.hongshengwenyu.top

Ruby: arr.each { |item| puts item }
来源：http://fip.316326.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ymb.ivvv.top

[B06] 遍历字典 / 对象
来源：http://fgi.zhengqikj.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kcl.316326.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vvz.hesvh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qrx.hnqzz.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gwj.shuidangran.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://soy.nwbrower.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://slu.smart0.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gzb.wangshuangyany.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ion.andypj.xyz

[B07] while 循环
来源：http://qxm.nwbrower.top

Py:   while i < 10: i += 1
来源：http://ppy.pycfn.com

PHP:  while ($i < 10) { $i++; }
来源：http://lmx.yj20258.top

JS:   while (i < 10) { i++; }
来源：http://qnp.gzhubu.top

TS:   while (i < 10) { i++; }
来源：http://zzk.mhx1999.top

Java: while (i < 10) { i++; }
来源：http://wsh.havefunace.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wiu.uphjek.com

Ruby: while i < 10; i += 1; end
来源：http://yps.aibaodan.cn

C#:   while (i < 10) { i++; }
来源：http://bzb.yangfankeji.com

[B08] do-while（至少执行一次）
来源：http://osa.mhx1999.top

Py:   # 无 do-while：用 while True + break
来源：http://gfj.hywenlv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tef.quarkkingdee.top

JS:   do { i++; } while (i < 10);
来源：http://tba.fehbvm.com

TS:   do { i++; } while (i < 10);
来源：http://jim.havefunace.top

Java: do { i++; } while (i < 10);
来源：http://alf.hnqzz.top

Go:   for { i++; if i >= 10 { break } }
来源：http://mle.uphjek.com

Ruby: begin; i += 1; end while i < 10
来源：http://jsx.vqdsnc.cn

C#:   do { i++; } while (i < 10);
来源：http://hvg.zhiwuduotai.top

[B09] break 与 continue
来源：http://xoj.zycfv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wdt.hnxiangtu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xmg.pycfn.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://swq.epnwcf.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wyy.havefunace.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ohe.hysaishi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pbz.hfpthk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uep.jyoumei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cqy.nwbrower.top

[B10] 遍历同时拿索引
来源：http://qxa.smart0.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dxh.xingfuxueyuan.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ogx.andypj.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hll.zhiwuduotai.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gen.jinqigfzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qax.shangyingyoupin.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://urf.ivvv.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ksf.nwbrower.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wpz.shanyushiyangkeji.top

[B11] 生成数字序列 / 区间
来源：http://htq.guannengcc.top

Py:   list(range(0, 10, 2))
来源：http://uuz.quarkkingdee.top

PHP:  range(0, 10, 2);
来源：http://ypo.jqgfzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pxo.xingfuxueyuan.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://odr.feifeiyinyue.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cbk.feifeiyinyue.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jza.jinqigfzy.top

Ruby: (0...10).step(2).to_a
来源：http://lsl.meibo888.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://muk.shanyushiyangkeji.top

[B12] 跳出多层循环
来源：http://zov.xuetiantiany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mnn.yuxming.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://doc.meibo888.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tcw.hnxiangtu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dkm.xingfuxueyuan.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ygl.gogol.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://caj.shzxlz.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xlo.andypj.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hxd.zhiwuduotai.top

[B13] 判断是否为数字
来源：http://pvq.pycfn.com

Py:   isinstance(x, (int, float))
来源：http://qkn.shzxlz.cn

PHP:  is_numeric($x)
来源：http://kji.guowangkeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://izn.cdnleiting.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ucj.chenzaomai.com

Java: x instanceof Number
来源：http://tau.cheryme.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lyc.pycfn.com

Ruby: x.is_a?(Numeric)
来源：http://eyy.gaohongyu789.top

C#:   x is int or double or decimal
来源：http://ohv.gzhubu.top

[B14] 判断值是否在集合内
来源：http://ouk.gaohongyu789.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lmk.fehbvm.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cuu.hongshengwenyu.top

JS:   [1, 2, 3].includes(x)
来源：http://fik.jinghuilouyu.cn

TS:   [1, 2, 3].includes(x)
来源：http://vuh.jyoumei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xhv.tian-w.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eum.shanyushiyangtech.top

Ruby: [1, 2, 3].include?(x)
来源：http://won.shanyushiyangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cdr.yj202588.top

[B15] 布尔运算与取反
来源：http://fqt.vehdjk.com

Py:   a and b or not c
来源：http://oao.ivvv.top

PHP:  $a && $b || !$c
来源：http://wrr.feifeiyinyue.top

JS:   a && b || !c
来源：http://fxy.xuetiantiany.cn

TS:   a && b || !c
来源：http://cex.sjlbkw.cn

Java: a && b || !c
来源：http://hlt.cashguo.top

Go:   a && b || !c
来源：http://rnr.aibaodan.cn

Ruby: a && b || !c
来源：http://pht.shanyushiyangkeji.top

C#:   a && b || !c
来源：http://vae.vehdjk.com

[B16] 卫语句：不满足条件提前返回
来源：http://voe.smart0.xyz

Py:   if not data: return
来源：http://hjb.iojbl.cn

PHP:  if (!$data) { return; }
来源：http://vpm.chenzaomai.com

JS:   if (!data) return;
来源：http://adk.hywenlv.cn

TS:   if (!data) return;
来源：http://jhm.tanke756.top

Java: if (data == null) return;
来源：http://ttd.jinyuanbaomall.cn

Go:   if data == nil { return }
来源：http://sgq.yj20258888.top

Ruby: return if data.nil?
来源：http://ize.aibaodan.cn

C#:   if (data == null) return;
来源：http://hsb.wangdashe.top

================================================================================
来源：http://xjv.zhijiandao.cn

C. 函数与作用域
来源：http://vxi.yueranfly.top

================================================================================
来源：http://eym.fengsongda.top

[C01] 定义函数
来源：http://hpq.haohaochexian.top

Py:   def add(a, b): return a + b
来源：http://ohz.xuetiantiany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vaq.zdbjq.cn

JS:   function add(a, b) { return a + b; }
来源：http://ink.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hxd.jiagoushi.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zwu.zhijiandao.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jnd.hesvh.cn

Ruby: def add(a, b); a + b; end
来源：http://vsg.svipenyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qtr.cheryme.top

[C02] 默认参数
来源：http://tqi.snrcjt.cn

Py:   def greet(name="World"): return name
来源：http://exg.daria6918.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zbc.yuanzhike.top

JS:   function greet(name = "World") { return name; }
来源：http://eqf.shzxlz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tyu.ywan-chungtsiang.top

Java: // 无默认参数：方法重载或 Optional
来源：http://yid.yj202588.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lvj.pycfn.com

Ruby: def greet(name = "World") = name
来源：http://wdx.xuetiantiany.cn

C#:   string Greet(string name = "World") => name;
来源：http://yko.sufxvd.cn

[C03] 可变参数
来源：http://bym.nwbrower.top

Py:   def total(*args): return sum(args)
来源：http://wcn.hywenlv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mem.cashguo.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ito.tian-w.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ujx.pengpengdd.cyou

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://phk.xingfuxueyuan.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://efm.daria6918.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zni.snrcjt.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ain.jqgufenzy.top

[C04] 命名参数 / 关键字参数
来源：http://glh.yj202588.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rko.shzxlz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ziq.cheryme.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vme.xuanzx.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://txf.pycfn.com

Java: // 无：用 Builder 模式或 record
来源：http://iuf.fengsongda.top

Go:   // 无：用配置结构体参数
来源：http://kkf.shzxlz.cn

Ruby: f(a: 1, b: 2)
来源：http://ray.jyoumei.cn

C#:   f(a: 1, b: 2)
来源：http://bzr.zhaomingkeji.xyz

[C05] 返回多个值
来源：http://rqj.chenlongwang.top

Py:   return a, b
来源：http://tgw.zhijiandao.cn

PHP:  return [$a, $b];
来源：http://pzs.yuanzhike.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://yty.shangyingyoupin.top

TS:   return { a, b };
来源：http://owy.wangdashe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fhe.cucudq.cn

Go:   return a, b
来源：http://aeh.52xcode.cn

Ruby: return a, b
来源：http://aor.xylfe.cn

C#:   return (a, b);              // ValueTuple
来源：http://xmp.jinghuilouyu.cn

[C06] 匿名函数 / lambda
来源：http://arw.meibo888.top

Py:   square = lambda x: x * x
来源：http://cky.tarul.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xyz.yueranfly.top

JS:   const square = x => x * x;
来源：http://ymc.redwolf501.top

TS:   const square = (x: number): number => x * x;
来源：http://qew.yuxming.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://luw.kuanghao11.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yze.xuanzx.com

Ruby: square = ->(x) { x * x }
来源：http://ubp.fzhhl.top

C#:   Func<int, int> square = x => x * x;
来源：http://oiq.chenjidiqi.icu

[C07] 把函数作为参数传入
来源：http://slr.quarkkingdee.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jxb.hnqzz.top

PHP:  array_map("strtoupper", $arr);
来源：http://zzh.pengpengdd.cyou

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pka.fehbvm.com

TS:   arr.map(String)
来源：http://ylh.havefunace.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sab.meibo888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kwn.ydjk.org.cn

Ruby: arr.map(&:upcase)
来源：http://myj.shanyushiyangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ans.0kj1m.cn

[C08] 闭包
来源：http://lza.jinqigfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jfi.svipenyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bfc.svipenyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vdj.haohaochexian.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dfm.haohaochexian.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://epf.tianlin.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tby.andypj.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yxr.52xcode.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mme.jianghu66.top

[C09] 递归
来源：http://uis.haohaochexian.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uix.jinqigufen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gwt.ehwqpu.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qnj.ivvv.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rni.feifeiyinyue.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kuk.yangfankeji.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oin.316326.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jey.xingfuxueyuan.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fyh.xuanzx.com

[C10] 变量作用域
来源：http://atx.yfazqb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jkn.cucudq.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ttk.ehwqpu.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qsp.aizwys.cn

TS:   同 JS
来源：http://rnj.shanyushiyangtech.top

Java: 方法内为块级作用域
来源：http://ihi.birdmap.top

Go:   花括号块级作用域
来源：http://dvk.yvedp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lbp.mhx1999.top

C#:   块级作用域
来源：http://fce.quarkkingdee.top

[C11] 模块导入与导出
来源：http://sju.aibaodan.cn

Py:   from module import func
来源：http://tfg.shangyingyoupin.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vxj.yueranfly.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://cal.zdqjudy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fbr.yuanzhike.top

Java: import java.util.List;
来源：http://clo.feifeiyinyue.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wcx.sufxvd.cn

Ruby: require "json"; require_relative "./util"
来源：http://kpv.cheryme.top

C#:   using System.Text;
来源：http://tpe.zhoulong.xyz

[C12] 立即执行函数 IIFE
来源：http://gug.fehbvm.com

Py:   (lambda: print("run"))()
来源：http://hfz.hongshengwenyu.top

PHP:  (function () { echo "run"; })();
来源：http://cdf.jianghu66.top

JS:   (() => { console.log("run"); })();
来源：http://imp.iojbl.cn

TS:   (() => { console.log("run"); })();
来源：http://axv.hnqzz.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hem.hysaishi.cn

Go:   func() { fmt.Println("run") }()
来源：http://xef.xinyue.icu

Ruby: -> { puts "run" }.call
来源：http://sez.cdnleiting.top

C#:   // 无 IIFE：用静态构造函数
来源：http://yvb.uphjek.com

[C13] 类型声明 / 类型注解
来源：http://trl.9152youxi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://izz.zycfv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pzi.wangshuangyany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://buw.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bvn.wangshuangyany.cn

Java: int add(int a, int b) { return a + b; }
来源：http://znx.zhongyouzk.top

Go:   func add(a, b int) int
来源：http://lct.yuxming.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xil.pycfn.com

C#:   int Add(int a, int b) => a + b;
来源：http://zrw.dashuyun.cn

[C14] 泛型函数
来源：http://wsg.chenlongwang.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ndn.ivvv.top

PHP:  // 无泛型
来源：http://lew.0kj1m.cn

JS:   // 无泛型
来源：http://eaq.yongpay.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pvk.dashuyun.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tvz.xingfuxueyuan.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zxw.jqgufenzy.top

Ruby: # 无泛型
来源：http://vcz.pycfn.com


<!-- 参考信息 -->