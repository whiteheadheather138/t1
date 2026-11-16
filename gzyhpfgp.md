代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vmf.dashuyun.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://phy.smart0.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uxb.jqgufenzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xhz.zhoulong.xyz

Go:   strings.TrimSpace(s)
来源：http://pud.dashuyun.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://peg.shzxlz.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hnl.dianchejie.cn

[A25] 字符串比较
来源：http://wcw.yongpay.top

Py:   s1 == s2; s1 != s2
来源：http://wye.ywan-chungtsiang.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://spw.xylfe.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://frq.yongpay.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://icj.hesvh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bgf.jinqigufen.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://itb.52xcode.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ooa.ctjpmb.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cwr.316326.xyz

[A26] 类型转换总览
来源：http://lnl.sjlbkw.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mqi.ctjpmb.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sfy.shuidangran.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://heo.ydjk.org.cn

TS:   Number() String() Boolean() x as number
来源：http://lsy.ctjpmb.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rgy.jianghu66.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zty.jlsjyb.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ajg.fehbvm.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hod.andypj.xyz

================================================================================
来源：http://vns.aibaodan.cn

B. 流程控制
来源：http://pco.hnxiangtu.top

================================================================================
来源：http://gbb.sufxvd.cn

[B01] 条件判断 if / else
来源：http://xmv.shanyushiyangtech.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ywl.yj20258888.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://czq.birdmap.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://apv.shangyingyoupin.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fso.shanyushiyangtech.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ptz.meibo888.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://foe.nanxuanxn.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fgg.yangfankeji.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pce.xingfuxueyuan.xyz

[B02] 多分支 else if / elif
来源：http://scx.svipenyu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kda.snrcjt.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://aup.tian-w.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uru.ybcxt.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mfp.jiagoushi.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jbm.shzxlz.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lsl.jinghuilouyu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ofl.hnqzz.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vcm.bbcook.cn

[B03] switch / match / case
来源：http://mwq.wangdashe.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ddh.316326.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ibe.fzhhl.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ffn.shanyushiyangkeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ulk.aibaodan.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ukz.sufxvd.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jwr.jlsjyb.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jdr.yongpay.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://suw.chenzaomai.com

[B04] for 计数循环
来源：http://gkr.quarkkingdee.top

Py:   for i in range(10): print(i)
来源：http://rqj.shuidangran.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xsq.ctjpmb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://auo.yuxming.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jmc.fehbvm.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zoo.dianchejie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ovh.hammf.cn

Ruby: 10.times { |i| puts i }
来源：http://mef.sufxvd.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pto.zhongyouzk.top

[B05] 遍历数组 / 列表
来源：http://ivh.iojbl.cn

Py:   for item in arr: print(item)
来源：http://yfq.sxryk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zsz.haohaochexian.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ork.tian-w.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zbx.haohaochexian.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fwn.dashuyun.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://feg.0kj1m.cn

Ruby: arr.each { |item| puts item }
来源：http://gzj.vehdjk.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jjf.yuxming.cn

[B06] 遍历字典 / 对象
来源：http://hmg.zhixingplan.top

Py:   for k, v in d.items(): print(k, v)
来源：http://drm.shanyushiyangkeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lup.xinyue.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nsc.yangfankeji.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hgi.yuanzhike.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ewh.yfazqb.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jah.wangdashe.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yzf.dashuyun.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uzo.c1oappe.top

[B07] while 循环
来源：http://gkp.daria6918.cn

Py:   while i < 10: i += 1
来源：http://ttz.jinqigufen.top

PHP:  while ($i < 10) { $i++; }
来源：http://oqx.0kj1m.cn

JS:   while (i < 10) { i++; }
来源：http://jaa.daria6918.cn

TS:   while (i < 10) { i++; }
来源：http://yjr.chenzaomai.com

Java: while (i < 10) { i++; }
来源：http://dxz.yvedp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fhx.zhiwuduotai.top

Ruby: while i < 10; i += 1; end
来源：http://fth.chenjidiqi.icu

C#:   while (i < 10) { i++; }
来源：http://anj.jlsjyb.cn

[B08] do-while（至少执行一次）
来源：http://pkp.sufxvd.cn

Py:   # 无 do-while：用 while True + break
来源：http://mgi.ehwqpu.com

PHP:  do { $i++; } while ($i < 10);
来源：http://bkd.yvedp.cn

JS:   do { i++; } while (i < 10);
来源：http://mxm.daxiang520.top

TS:   do { i++; } while (i < 10);
来源：http://bdr.cucudq.cn

Java: do { i++; } while (i < 10);
来源：http://xup.birdmap.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fju.zhoulong.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://una.fanxiaobao.xyz

C#:   do { i++; } while (i < 10);
来源：http://rlu.hywenlv.cn

[B09] break 与 continue
来源：http://emm.hesvh.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hbn.bjfxy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ofa.jianghu66.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kzf.daria6918.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://icb.tanke756.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yvq.xylfe.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qya.yueranfly.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vwt.hysaishi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yva.cheryme.top

[B10] 遍历同时拿索引
来源：http://zun.9152youxi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uld.shangyingyoupin.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ygv.chenjidiqi.icu

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wqm.tarul.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://azg.fktsv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qnv.jinqigufen.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oyp.feifeiyinyue.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jyg.iojbl.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rsg.shuidangran.top

[B11] 生成数字序列 / 区间
来源：http://pon.epnwcf.com

Py:   list(range(0, 10, 2))
来源：http://uog.tarul.cn

PHP:  range(0, 10, 2);
来源：http://ais.xuetiantiany.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xkb.zycfv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zwp.zhaomingkeji.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xpd.zhengqikj.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://klq.cucudq.cn

Ruby: (0...10).step(2).to_a
来源：http://fbh.tarul.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ufe.andypj.xyz

[B12] 跳出多层循环
来源：http://usc.cqqwz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dpg.zhongyouzk.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://nwf.fzhhl.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ofm.tarul.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vpq.snrcjt.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zxa.pycfn.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ujd.c1oappe.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://afg.iojbl.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cgg.zhijiandao.cn

[B13] 判断是否为数字
来源：http://ffx.haohaochexian.top

Py:   isinstance(x, (int, float))
来源：http://bix.ydjk.org.cn

PHP:  is_numeric($x)
来源：http://mtv.sjlbkw.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ait.tarul.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oty.sxryk.cn

Java: x instanceof Number
来源：http://otd.xinyue.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fxg.meibo888.top

Ruby: x.is_a?(Numeric)
来源：http://cjs.fzhhl.top

C#:   x is int or double or decimal
来源：http://mlp.pycfn.com

[B14] 判断值是否在集合内
来源：http://dbr.xingfuxueyuan.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cru.bbcook.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gop.yangfankeji.com

JS:   [1, 2, 3].includes(x)
来源：http://edf.fanxiaobao.xyz

TS:   [1, 2, 3].includes(x)
来源：http://vcx.chenjidiqi.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://ocf.yj20258888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zdh.zhijiandao.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lrm.nwbrower.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dos.ehwqpu.com

[B15] 布尔运算与取反
来源：http://ctf.svipenyu.cn

Py:   a and b or not c
来源：http://dnl.chenzaomai.com

PHP:  $a && $b || !$c
来源：http://hur.havefunace.top

JS:   a && b || !c
来源：http://oya.hysaishi.cn

TS:   a && b || !c
来源：http://lfi.zdqjudy.top

Java: a && b || !c
来源：http://iol.tian-w.cn

Go:   a && b || !c
来源：http://ahe.havefunace.top

Ruby: a && b || !c
来源：http://wnr.chenjidiqi.icu

C#:   a && b || !c
来源：http://hez.redwolf501.top

[B16] 卫语句：不满足条件提前返回
来源：http://wmk.smart0.xyz

Py:   if not data: return
来源：http://djv.xziqi.cn

PHP:  if (!$data) { return; }
来源：http://rva.kuanghao11.cn

JS:   if (!data) return;
来源：http://tgw.ydjk.org.cn

TS:   if (!data) return;
来源：http://ogk.sysykeji.top

Java: if (data == null) return;
来源：http://ifx.sysykeji.top

Go:   if data == nil { return }
来源：http://uap.xziqi.cn

Ruby: return if data.nil?
来源：http://fgh.guowangkeji.top

C#:   if (data == null) return;
来源：http://reb.zhengqikj.top

================================================================================
来源：http://rig.pycfn.com

C. 函数与作用域
来源：http://czx.bjfxy.top

================================================================================
来源：http://pmn.feifeiyinyue.top

[C01] 定义函数
来源：http://zrk.chenzaomai.com

Py:   def add(a, b): return a + b
来源：http://jyd.quarkkingdee.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://myf.zdbjq.cn

JS:   function add(a, b) { return a + b; }
来源：http://fyk.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ich.vqdsnc.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yzb.bbcook.cn

Go:   func add(a, b int) int { return a + b }
来源：http://soq.zhijiandao.cn

Ruby: def add(a, b); a + b; end
来源：http://tka.jinqigfzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://phr.quarkkingdee.top

[C02] 默认参数
来源：http://pfh.sysykeji.top

Py:   def greet(name="World"): return name
来源：http://hfn.yfazqb.com

PHP:  function greet($name = "World") { return $name; }
来源：http://iam.tian-w.cn

JS:   function greet(name = "World") { return name; }
来源：http://wdu.xinyue.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://gui.ybcxt.top

Java: // 无默认参数：方法重载或 Optional
来源：http://veg.zhaomingkeji.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://aax.yvedp.cn

Ruby: def greet(name = "World") = name
来源：http://rgn.aizwys.cn

C#:   string Greet(string name = "World") => name;
来源：http://ile.cqqwz.cn

[C03] 可变参数
来源：http://vqe.daxiang520.top

Py:   def total(*args): return sum(args)
来源：http://tem.tanke756.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mlu.dashuyun.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ybw.gzhubu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fmb.hnqzz.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fgg.nanxinkj.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zuj.fzhhl.top

Ruby: def total(*nums); nums.sum; end
来源：http://sbu.fzhhl.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ate.meibo888.top

[C04] 命名参数 / 关键字参数
来源：http://kjg.jqgufenzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://toa.xziqi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mig.ehwqpu.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jrz.cdnleiting.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zrf.snrcjt.cn

Java: // 无：用 Builder 模式或 record
来源：http://eur.zhiwuduotai.top

Go:   // 无：用配置结构体参数
来源：http://gol.shzxlz.cn

Ruby: f(a: 1, b: 2)
来源：http://fwl.gogol.net.cn

C#:   f(a: 1, b: 2)
来源：http://kyx.shuidangran.top

[C05] 返回多个值
来源：http://roq.zhiwuduotai.top

Py:   return a, b
来源：http://caz.9152youxi.cn

PHP:  return [$a, $b];
来源：http://vmf.vqdsnc.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nuq.zhaomingkeji.xyz

TS:   return { a, b };
来源：http://ddt.shangyingyoupin.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://iwl.ydjk.org.cn

Go:   return a, b
来源：http://uxw.gotoacloud.top

Ruby: return a, b
来源：http://kld.fengsongda.top

C#:   return (a, b);              // ValueTuple
来源：http://tbj.nanxinkj.top

[C06] 匿名函数 / lambda
来源：http://gqt.gogol.net.cn

Py:   square = lambda x: x * x
来源：http://mxs.zdbjq.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jqu.hysaishi.cn

JS:   const square = x => x * x;
来源：http://jej.chenzaomai.com

TS:   const square = (x: number): number => x * x;
来源：http://hdq.ppjwa.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://krq.zhengqikj.top

Go:   sq := func(x int) int { return x * x }
来源：http://ahd.daxiang520.top

Ruby: square = ->(x) { x * x }
来源：http://quj.vehdjk.com

C#:   Func<int, int> square = x => x * x;
来源：http://mdk.epnwcf.com

[C07] 把函数作为参数传入
来源：http://kfs.tarul.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lus.fktsv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jzw.haohaochexian.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kid.gzhubu.top

TS:   arr.map(String)
来源：http://jpd.wangdashe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vhi.yj20258.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://aun.xuanzx.com

Ruby: arr.map(&:upcase)
来源：http://yst.fengsongda.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ctj.birdmap.top

[C08] 闭包
来源：http://miv.andypj.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yrm.jinghuilouyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qml.zdqjudy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bco.meibo888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vqs.dashuyun.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://geh.wangshuangyany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wyz.guannengcc.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hih.zdqjudy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jag.zhijiandao.cn

[C09] 递归
来源：http://ozx.smart0.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ooo.52xcode.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://srq.c1oappe.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gvp.yuanzhike.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ubb.fktsv.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eiu.daria6918.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jfe.tarul.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wbh.ywan-chungtsiang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jfm.ywan-chungtsiang.top

[C10] 变量作用域
来源：http://rxm.chenlongwang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://flu.jqgfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uug.yfazqb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xqa.shangyingyoupin.top

TS:   同 JS
来源：http://uwy.jlsjyb.cn

Java: 方法内为块级作用域
来源：http://zin.chenlongwang.top

Go:   花括号块级作用域
来源：http://jup.hcnkem.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://opq.jlsjyb.cn

C#:   块级作用域
来源：http://yqr.xuetiantiany.cn

[C11] 模块导入与导出
来源：http://stu.hfpthk.cn

Py:   from module import func
来源：http://fjy.chenzaomai.com

PHP:  require "file.php";  或 use App\Service;
来源：http://uyo.9152youxi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ywj.ydjk.org.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://iks.yangfankeji.com

Java: import java.util.List;
来源：http://ihb.ybcxt.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xtf.hfpthk.cn

Ruby: require "json"; require_relative "./util"
来源：http://muz.birdmap.top

C#:   using System.Text;
来源：http://fmr.quarkkingdee.top

[C12] 立即执行函数 IIFE
来源：http://tbd.birdmap.top

Py:   (lambda: print("run"))()
来源：http://lpv.shanyushiyangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://xrj.fzhhl.top

JS:   (() => { console.log("run"); })();
来源：http://ezr.hcnkem.com

TS:   (() => { console.log("run"); })();
来源：http://fzc.zdbjq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sjz.xinyue.icu

Go:   func() { fmt.Println("run") }()
来源：http://oxb.iojbl.cn

Ruby: -> { puts "run" }.call
来源：http://cpy.hongshengwenyu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ubz.dianchejie.cn

[C13] 类型声明 / 类型注解
来源：http://aiv.hcnkem.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://iqb.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zzm.hfpthk.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nbm.uphjek.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://thj.jqgufenzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://cao.havefunace.top

Go:   func add(a, b int) int
来源：http://xoa.gogol.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xlf.fanxiaobao.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://gkq.dianchejie.cn

[C14] 泛型函数
来源：http://ket.birdmap.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xek.nanxinkj.top

PHP:  // 无泛型
来源：http://wjn.pengpengdd.cyou

JS:   // 无泛型
来源：http://qcs.sysykeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lqf.kuanghao11.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vxu.daria6918.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wva.yongpay.top

Ruby: # 无泛型
来源：http://xyu.jinqigufen.top


<!-- 参考信息 -->