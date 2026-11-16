代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qwm.cucudq.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ruv.yvedp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zix.dashuyun.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bpd.sxryk.cn

Go:   strings.TrimSpace(s)
来源：http://cvd.havefunace.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qio.ydjk.org.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://smc.hnxiangtu.top

[A25] 字符串比较
来源：http://kfp.zhaomingkeji.xyz

Py:   s1 == s2; s1 != s2
来源：http://ttd.shuidangran.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://poi.jqgfzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wnn.yj20258888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mxm.guannengcc.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yrz.hnqzz.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qby.sysykeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://xfv.ywan-chungtsiang.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vkw.snrcjt.cn

[A26] 类型转换总览
来源：http://epg.ywan-chungtsiang.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dvs.xingfuxueyuan.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lss.hnqzz.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qsl.zhaomingkeji.xyz

TS:   Number() String() Boolean() x as number
来源：http://kst.hysaishi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gay.sufxvd.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dsy.andypj.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://zod.xuetiantiany.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vuk.yanxiufei.cn

================================================================================
来源：http://bfw.yj20258888.top

B. 流程控制
来源：http://nhg.jianghu66.top

================================================================================
来源：http://mcn.birdmap.top

[B01] 条件判断 if / else
来源：http://azn.xylfe.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hdq.guowangkeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zif.nwbrower.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dra.hnqzz.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tni.hfpthk.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tsj.ehwqpu.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wwl.zhixingplan.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ttv.xziqi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cjw.yuxming.cn

[B02] 多分支 else if / elif
来源：http://gxi.0kj1m.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://iba.cheryme.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kyw.dianchejie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://knm.tarul.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wiu.chenlongwang.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qvy.cdnleiting.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wib.jinyuanbaomall.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://knc.kuanghao11.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bnu.hfpthk.cn

[B03] switch / match / case
来源：http://kfb.yueranfly.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://aeq.uphjek.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fyp.jinyuanbaomall.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ccu.yueranfly.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yjf.ppjwa.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ebl.mhx1999.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cqd.shanyushiyangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sja.meibo888.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://okv.jqgufenzy.top

[B04] for 计数循环
来源：http://rqg.yj20258.top

Py:   for i in range(10): print(i)
来源：http://mtn.tarul.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://swu.tianlin.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ntq.epnwcf.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qir.tianlin.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ztk.yj20258888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bri.bjfxy.top

Ruby: 10.times { |i| puts i }
来源：http://fdp.xinyue.icu

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rtp.fengsongda.top

[B05] 遍历数组 / 列表
来源：http://ipo.hcnkem.com

Py:   for item in arr: print(item)
来源：http://roi.vehdjk.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zjc.cashguo.top

JS:   for (const item of arr) { console.log(item); }
来源：http://uxw.epnwcf.com

TS:   for (const item of arr) { console.log(item); }
来源：http://seh.jinqigfzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://yjl.fzhhl.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hvs.yangfankeji.com

Ruby: arr.each { |item| puts item }
来源：http://zue.jinghuilouyu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://aet.redwolf501.top

[B06] 遍历字典 / 对象
来源：http://zya.uphjek.com

Py:   for k, v in d.items(): print(k, v)
来源：http://ano.tanke756.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mnp.shanyushiyangtech.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ror.jqgufenzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zee.zhaomingkeji.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wlo.zhijiandao.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xqe.jqgufenzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kis.jqgfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xjl.haohaochexian.top

[B07] while 循环
来源：http://ddq.fengsongda.top

Py:   while i < 10: i += 1
来源：http://byu.fehbvm.com

PHP:  while ($i < 10) { $i++; }
来源：http://myj.xingfuxueyuan.xyz

JS:   while (i < 10) { i++; }
来源：http://wvb.ybcxt.top

TS:   while (i < 10) { i++; }
来源：http://apz.xuanzx.com

Java: while (i < 10) { i++; }
来源：http://qrz.xuetiantiany.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bzd.zycfv.cn

Ruby: while i < 10; i += 1; end
来源：http://rqm.dianchejie.cn

C#:   while (i < 10) { i++; }
来源：http://wzs.birdmap.top

[B08] do-while（至少执行一次）
来源：http://pvx.hnqzz.top

Py:   # 无 do-while：用 while True + break
来源：http://qhv.gaohongyu789.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kpn.ybcxt.top

JS:   do { i++; } while (i < 10);
来源：http://bps.bbcook.cn

TS:   do { i++; } while (i < 10);
来源：http://pkm.jinghuilouyu.cn

Java: do { i++; } while (i < 10);
来源：http://eep.hnxiangtu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ikp.ybcxt.top

Ruby: begin; i += 1; end while i < 10
来源：http://hsn.yanxiufei.cn

C#:   do { i++; } while (i < 10);
来源：http://mcg.jinqigufen.top

[B09] break 与 continue
来源：http://jtg.shuidangran.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kgg.gogol.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zfh.52xcode.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uro.hcnkem.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rpq.jinqigfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qmj.xuanzx.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xof.vqdsnc.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mtc.sufxvd.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cmf.aibaodan.cn

[B10] 遍历同时拿索引
来源：http://okp.hywenlv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://has.shanyushiyangkeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kea.yj20258888.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oks.guowangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rwx.yvedp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mko.ppjwa.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uba.fehbvm.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qje.fktsv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jed.iojbl.cn

[B11] 生成数字序列 / 区间
来源：http://ssx.ivvv.top

Py:   list(range(0, 10, 2))
来源：http://rfw.meibo888.top

PHP:  range(0, 10, 2);
来源：http://fym.daria6918.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mmi.hesvh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gta.quarkkingdee.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wza.chenzaomai.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sle.ybcxt.top

Ruby: (0...10).step(2).to_a
来源：http://vbt.tian-w.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rwf.jqgfzy.top

[B12] 跳出多层循环
来源：http://uzp.yuxming.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jpw.0kj1m.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://snw.tian-w.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fgf.cqqwz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uxo.snrcjt.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oac.shanyushiyangtech.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pfq.fehbvm.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cix.shanyushiyangtech.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aai.birdmap.top

[B13] 判断是否为数字
来源：http://sgf.zycfv.cn

Py:   isinstance(x, (int, float))
来源：http://doh.zhengqikj.top

PHP:  is_numeric($x)
来源：http://feb.jlsjyb.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ofd.dianchejie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nyx.cdnleiting.top

Java: x instanceof Number
来源：http://hay.vqdsnc.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://swo.fengsongda.top

Ruby: x.is_a?(Numeric)
来源：http://ixp.hongshengwenyu.top

C#:   x is int or double or decimal
来源：http://qed.yangfankeji.com

[B14] 判断值是否在集合内
来源：http://fpc.jinqigufen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pnm.epnwcf.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rll.pycfn.com

JS:   [1, 2, 3].includes(x)
来源：http://hlt.jiagoushi.top

TS:   [1, 2, 3].includes(x)
来源：http://qje.fengsongda.top

Java: List.of(1, 2, 3).contains(x)
来源：http://oak.aizwys.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://quc.gaohongyu789.top

Ruby: [1, 2, 3].include?(x)
来源：http://emg.yvedp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xma.yanxiufei.cn

[B15] 布尔运算与取反
来源：http://ryd.andypj.xyz

Py:   a and b or not c
来源：http://mcp.sufxvd.cn

PHP:  $a && $b || !$c
来源：http://zxx.chenjidiqi.icu

JS:   a && b || !c
来源：http://dez.gotoacloud.top

TS:   a && b || !c
来源：http://ypa.hcnkem.com

Java: a && b || !c
来源：http://gii.bjfxy.top

Go:   a && b || !c
来源：http://xwt.xingfuxueyuan.xyz

Ruby: a && b || !c
来源：http://gra.sweek.top

C#:   a && b || !c
来源：http://adj.tianlin.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://fvl.sxryk.cn

Py:   if not data: return
来源：http://dfi.zhongyouzk.top

PHP:  if (!$data) { return; }
来源：http://asw.quarkkingdee.top

JS:   if (!data) return;
来源：http://ngx.quarkkingdee.top

TS:   if (!data) return;
来源：http://kai.yfazqb.com

Java: if (data == null) return;
来源：http://jud.yonumen.top

Go:   if data == nil { return }
来源：http://mul.gaohongyu789.top

Ruby: return if data.nil?
来源：http://cim.sysykeji.top

C#:   if (data == null) return;
来源：http://wsr.cucudq.cn

================================================================================
来源：http://hch.shzxlz.cn

C. 函数与作用域
来源：http://vmq.yvedp.cn

================================================================================
来源：http://pmh.zhengqikj.top

[C01] 定义函数
来源：http://nbi.jianghu66.top

Py:   def add(a, b): return a + b
来源：http://itg.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zkz.fanxiaobao.xyz

JS:   function add(a, b) { return a + b; }
来源：http://utr.yj20258.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://scy.ppjwa.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lfl.zdqjudy.top

Go:   func add(a, b int) int { return a + b }
来源：http://hix.gotoacloud.top

Ruby: def add(a, b); a + b; end
来源：http://awy.316326.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gli.sxryk.cn

[C02] 默认参数
来源：http://ugp.yuanzhike.top

Py:   def greet(name="World"): return name
来源：http://ygr.fzhhl.top

PHP:  function greet($name = "World") { return $name; }
来源：http://cer.ywan-chungtsiang.top

JS:   function greet(name = "World") { return name; }
来源：http://xqy.sysykeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://iyl.tarul.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://baa.sysykeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iur.havefunace.top

Ruby: def greet(name = "World") = name
来源：http://evy.yangfankeji.com

C#:   string Greet(string name = "World") => name;
来源：http://drr.cashguo.top

[C03] 可变参数
来源：http://kjh.0kj1m.cn

Py:   def total(*args): return sum(args)
来源：http://bfk.andypj.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lmr.ydzc1.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kss.hongshengwenyu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xqg.uphjek.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qzy.guannengcc.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sym.epnwcf.com

Ruby: def total(*nums); nums.sum; end
来源：http://oyl.birdmap.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://maf.guowangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://xwm.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kxk.birdmap.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ubq.yanxiufei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pre.jqgfzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://neg.tianlin.xyz

Java: // 无：用 Builder 模式或 record
来源：http://xon.ppjwa.cn

Go:   // 无：用配置结构体参数
来源：http://hde.sxryk.cn

Ruby: f(a: 1, b: 2)
来源：http://mji.jiagoushi.top

C#:   f(a: 1, b: 2)
来源：http://qgl.tanke756.top

[C05] 返回多个值
来源：http://xmw.chenzaomai.com

Py:   return a, b
来源：http://ojb.shangyingyoupin.top

PHP:  return [$a, $b];
来源：http://wjf.ppjwa.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wlo.redwolf501.top

TS:   return { a, b };
来源：http://lkk.gogol.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://umc.guannengcc.top

Go:   return a, b
来源：http://vqw.ydjk.org.cn

Ruby: return a, b
来源：http://ema.ivvv.top

C#:   return (a, b);              // ValueTuple
来源：http://vgi.hysaishi.cn

[C06] 匿名函数 / lambda
来源：http://off.fehbvm.com

Py:   square = lambda x: x * x
来源：http://wdu.hysaishi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bcj.xuetiantiany.cn

JS:   const square = x => x * x;
来源：http://bug.jyoumei.cn

TS:   const square = (x: number): number => x * x;
来源：http://yko.chenzaomai.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tlp.smart0.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://pqz.jqgufenzy.top

Ruby: square = ->(x) { x * x }
来源：http://vbe.pycfn.com

C#:   Func<int, int> square = x => x * x;
来源：http://sri.hysaishi.cn

[C07] 把函数作为参数传入
来源：http://wjm.wangdashe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qio.zhixingplan.top

PHP:  array_map("strtoupper", $arr);
来源：http://esn.fengsongda.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fpv.shangyingyoupin.top

TS:   arr.map(String)
来源：http://rvu.gogol.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hav.pengpengdd.cyou

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mvb.dianchejie.cn

Ruby: arr.map(&:upcase)
来源：http://ujg.shuidangran.top

C#:   arr.Select(s => s.ToUpper())
来源：http://yqk.andypj.xyz

[C08] 闭包
来源：http://omt.mhx1999.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uha.hnxiangtu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://paf.xylfe.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bvq.cqqwz.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xaf.hongshengwenyu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uic.iojbl.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dxr.zdbjq.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dfr.pengpengdd.cyou

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xkp.jyoumei.cn

[C09] 递归
来源：http://qeq.yongpay.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qyy.xuetiantiany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qaq.sxryk.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mmc.0kj1m.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ezx.feifeiyinyue.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yfb.uphjek.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zzm.ctjpmb.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kla.zhongyouzk.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rhp.shzxlz.cn

[C10] 变量作用域
来源：http://vcj.aibaodan.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qlm.zhongyouzk.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qai.zhijiandao.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ysu.sjlbkw.cn

TS:   同 JS
来源：http://ycz.yuxming.cn

Java: 方法内为块级作用域
来源：http://oxh.nanxuanxn.top

Go:   花括号块级作用域
来源：http://fka.daxiang520.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wiz.yj202588.top

C#:   块级作用域
来源：http://ctq.mhx1999.top

[C11] 模块导入与导出
来源：http://eml.shzxlz.cn

Py:   from module import func
来源：http://nlu.yanxiufei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rtl.yongpay.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://kkl.jinyuanbaomall.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rce.guowangkeji.top

Java: import java.util.List;
来源：http://xbz.yuxming.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cji.yuanzhike.top

Ruby: require "json"; require_relative "./util"
来源：http://ppv.yuxming.cn

C#:   using System.Text;
来源：http://mwk.gaohongyu789.top

[C12] 立即执行函数 IIFE
来源：http://are.smart0.xyz

Py:   (lambda: print("run"))()
来源：http://mjz.uphjek.com

PHP:  (function () { echo "run"; })();
来源：http://cjo.daxiang520.top

JS:   (() => { console.log("run"); })();
来源：http://wrb.haohaochexian.top

TS:   (() => { console.log("run"); })();
来源：http://ayz.meibo888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gnp.zhoulong.xyz

Go:   func() { fmt.Println("run") }()
来源：http://kpb.pycfn.com

Ruby: -> { puts "run" }.call
来源：http://wlg.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://zsv.daria6918.cn

[C13] 类型声明 / 类型注解
来源：http://pki.yvedp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jqc.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://njk.zhiwuduotai.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zrc.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ghx.yfazqb.com

Java: int add(int a, int b) { return a + b; }
来源：http://tuh.dianchejie.cn

Go:   func add(a, b int) int
来源：http://cbs.yj20258888.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jgw.hywenlv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gze.316326.xyz

[C14] 泛型函数
来源：http://jsg.shzxlz.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cdy.cucudq.cn

PHP:  // 无泛型
来源：http://bpz.fzhhl.top

JS:   // 无泛型
来源：http://jdp.zhijiandao.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://njm.hnxiangtu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ata.zhaomingkeji.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://clu.sysykeji.top

Ruby: # 无泛型
来源：http://ywb.hammf.cn


<!-- 参考信息 -->