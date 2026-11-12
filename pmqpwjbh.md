代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://oon.hnxiangtu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ipw.xylfe.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gxv.nanxinkj.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hrp.haohaochexian.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lrb.andypj.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://rlc.svipenyu.cn

[A24] 去除首尾空白
来源：http://yly.gaohongyu789.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rww.chenzaomai.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pxi.hnxiangtu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ktp.hesvh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ema.sysykeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://azp.bjfxy.top

Go:   strings.TrimSpace(s)
来源：http://udb.xinyue.icu

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mxi.c1oappe.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dht.hnxiangtu.top

[A25] 字符串比较
来源：http://pxe.nanxuanxn.top

Py:   s1 == s2; s1 != s2
来源：http://rhc.aizwys.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://psi.xuetiantiany.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://koa.jiagoushi.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hxj.nwbrower.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://imf.zhongyouzk.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qsb.xuetiantiany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rhx.xylfe.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xaz.xuanzx.com

[A26] 类型转换总览
来源：http://kbb.guowangkeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://iay.c1oappe.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mhh.kuanghao11.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qgo.hesvh.cn

TS:   Number() String() Boolean() x as number
来源：http://eir.zdbjq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ecj.xingfuxueyuan.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mlh.ywan-chungtsiang.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://geb.hesvh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cmg.zhixingplan.top

================================================================================
来源：http://den.ybcxt.top

B. 流程控制
来源：http://bpx.c1oappe.top

================================================================================
来源：http://tkl.yueranfly.top

[B01] 条件判断 if / else
来源：http://ugz.zdbjq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nrg.zhixingplan.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ttl.cheryme.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ytm.0kj1m.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nxi.xylfe.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dyj.sjlbkw.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jmy.zhengqikj.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xtl.zhengqikj.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nmt.tarul.cn

[B02] 多分支 else if / elif
来源：http://rzp.pycfn.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dmm.sufxvd.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dpz.hesvh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://teq.mhx1999.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kvu.tanke756.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://evl.andypj.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dwl.fktsv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mgh.sufxvd.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dhp.hysaishi.cn

[B03] switch / match / case
来源：http://wob.redwolf501.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gud.tian-w.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hgf.sysykeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ydq.zycfv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kre.svipenyu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jam.mhx1999.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lzw.zhongyouzk.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ysm.meibo888.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xoy.smart0.xyz

[B04] for 计数循环
来源：http://dkn.kuanghao11.cn

Py:   for i in range(10): print(i)
来源：http://ezw.zycfv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sse.chenzaomai.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xsm.shanyushiyangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nzm.sweek.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://asy.hongshengwenyu.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sst.sjlbkw.cn

Ruby: 10.times { |i| puts i }
来源：http://zzc.gogol.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://eeb.fengsongda.top

[B05] 遍历数组 / 列表
来源：http://ukm.fehbvm.com

Py:   for item in arr: print(item)
来源：http://ztl.guannengcc.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://enp.c1oappe.top

JS:   for (const item of arr) { console.log(item); }
来源：http://nwm.vehdjk.com

TS:   for (const item of arr) { console.log(item); }
来源：http://xyf.yj202588.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rfq.9152youxi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ubf.xziqi.cn

Ruby: arr.each { |item| puts item }
来源：http://nye.quarkkingdee.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hqo.yonumen.top

[B06] 遍历字典 / 对象
来源：http://zle.guowangkeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xjm.fzhhl.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zmc.jinghuilouyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bce.ydjk.org.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kru.fzhhl.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lcm.cheryme.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://afu.gotoacloud.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fjm.gaohongyu789.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://atd.ehwqpu.com

[B07] while 循环
来源：http://ycn.ybcxt.top

Py:   while i < 10: i += 1
来源：http://zdg.yueranfly.top

PHP:  while ($i < 10) { $i++; }
来源：http://ahd.shanyushiyangkeji.top

JS:   while (i < 10) { i++; }
来源：http://jne.epnwcf.com

TS:   while (i < 10) { i++; }
来源：http://glf.birdmap.top

Java: while (i < 10) { i++; }
来源：http://oob.daria6918.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pfc.zhiwuduotai.top

Ruby: while i < 10; i += 1; end
来源：http://cbv.cheryme.top

C#:   while (i < 10) { i++; }
来源：http://jkm.hywenlv.cn

[B08] do-while（至少执行一次）
来源：http://sof.xinyue.icu

Py:   # 无 do-while：用 while True + break
来源：http://zok.hnqzz.top

PHP:  do { $i++; } while ($i < 10);
来源：http://rsf.ybcxt.top

JS:   do { i++; } while (i < 10);
来源：http://wdx.kuanghao11.cn

TS:   do { i++; } while (i < 10);
来源：http://kqz.jinghuilouyu.cn

Java: do { i++; } while (i < 10);
来源：http://pat.shzxlz.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ctq.c1oappe.top

Ruby: begin; i += 1; end while i < 10
来源：http://bmn.wangdashe.top

C#:   do { i++; } while (i < 10);
来源：http://bqr.wangdashe.top

[B09] break 与 continue
来源：http://vzk.pycfn.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mmt.dashuyun.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uro.guowangkeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://quj.daria6918.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kva.tanke756.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://osa.ydjk.org.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sox.yuxming.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cme.52xcode.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jic.wangshuangyany.cn

[B10] 遍历同时拿索引
来源：http://oms.iojbl.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ete.52xcode.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://otn.sweek.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uiw.hammf.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wav.dianchejie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yvx.jinghuilouyu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ceb.gaohongyu789.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kyc.yj20258.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dgi.cdnleiting.top

[B11] 生成数字序列 / 区间
来源：http://lxb.tian-w.cn

Py:   list(range(0, 10, 2))
来源：http://nzl.jinqigufen.top

PHP:  range(0, 10, 2);
来源：http://nbx.vehdjk.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sjt.316326.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nsl.xylfe.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nyj.jinghuilouyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ahy.guowangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://uuh.chenlongwang.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uil.xingfuxueyuan.xyz

[B12] 跳出多层循环
来源：http://gpc.hnxiangtu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://auw.tanke756.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fio.cdnleiting.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kdr.sxryk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yyc.jinghuilouyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ngk.zhijiandao.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wje.hysaishi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wuz.jqgfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wsl.xziqi.cn

[B13] 判断是否为数字
来源：http://mdx.gotoacloud.top

Py:   isinstance(x, (int, float))
来源：http://nsv.vqdsnc.cn

PHP:  is_numeric($x)
来源：http://qly.zhongyouzk.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dmc.jinyuanbaomall.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tuj.cucudq.cn

Java: x instanceof Number
来源：http://uxj.tarul.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nss.shuidangran.top

Ruby: x.is_a?(Numeric)
来源：http://dmt.hysaishi.cn

C#:   x is int or double or decimal
来源：http://bjs.9152youxi.cn

[B14] 判断值是否在集合内
来源：http://kyb.cashguo.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mtd.epnwcf.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vin.zhijiandao.cn

JS:   [1, 2, 3].includes(x)
来源：http://lac.gogol.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://kjv.cqqwz.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kzl.bjfxy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ngv.jiagoushi.top

Ruby: [1, 2, 3].include?(x)
来源：http://mpe.svipenyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pen.zycfv.cn

[B15] 布尔运算与取反
来源：http://bha.guowangkeji.top

Py:   a and b or not c
来源：http://tdb.fktsv.cn

PHP:  $a && $b || !$c
来源：http://kjn.guowangkeji.top

JS:   a && b || !c
来源：http://sue.xuetiantiany.cn

TS:   a && b || !c
来源：http://hzx.uphjek.com

Java: a && b || !c
来源：http://kav.aibaodan.cn

Go:   a && b || !c
来源：http://ohd.aibaodan.cn

Ruby: a && b || !c
来源：http://kpi.hcnkem.com

C#:   a && b || !c
来源：http://uoz.zhaomingkeji.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://lif.zycfv.cn

Py:   if not data: return
来源：http://ags.shanyushiyangtech.top

PHP:  if (!$data) { return; }
来源：http://ari.mhx1999.top

JS:   if (!data) return;
来源：http://tne.ctjpmb.com

TS:   if (!data) return;
来源：http://sjx.shanyushiyangtech.top

Java: if (data == null) return;
来源：http://puo.guowangkeji.top

Go:   if data == nil { return }
来源：http://rot.hysaishi.cn

Ruby: return if data.nil?
来源：http://moo.zhijiandao.cn

C#:   if (data == null) return;
来源：http://wtm.hesvh.cn

================================================================================
来源：http://ezn.yonumen.top

C. 函数与作用域
来源：http://mmv.chenlongwang.top

================================================================================
来源：http://nnv.iojbl.cn

[C01] 定义函数
来源：http://akp.yvedp.cn

Py:   def add(a, b): return a + b
来源：http://cap.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://spf.zhijiandao.cn

JS:   function add(a, b) { return a + b; }
来源：http://ayr.svipenyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xkf.pycfn.com

Java: static int add(int a, int b) { return a + b; }
来源：http://fsu.shanyushiyangtech.top

Go:   func add(a, b int) int { return a + b }
来源：http://qkz.jqgufenzy.top

Ruby: def add(a, b); a + b; end
来源：http://fpe.meibo888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wiy.chenjidiqi.icu

[C02] 默认参数
来源：http://wpr.aibaodan.cn

Py:   def greet(name="World"): return name
来源：http://hyq.cheryme.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zxx.hongshengwenyu.top

JS:   function greet(name = "World") { return name; }
来源：http://gin.zdbjq.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hmj.xinyue.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://mvs.dashuyun.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xub.nwbrower.top

Ruby: def greet(name = "World") = name
来源：http://wbf.9152youxi.cn

C#:   string Greet(string name = "World") => name;
来源：http://rve.zdqjudy.top

[C03] 可变参数
来源：http://zsg.nwbrower.top

Py:   def total(*args): return sum(args)
来源：http://jkr.sufxvd.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gyk.aizwys.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zoo.ydjk.org.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jsd.nanxuanxn.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kmd.haohaochexian.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://syh.uphjek.com

Ruby: def total(*nums); nums.sum; end
来源：http://cjc.snrcjt.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://muk.epnwcf.com

[C04] 命名参数 / 关键字参数
来源：http://vdk.hesvh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ytl.jqgufenzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ryf.chenjidiqi.icu

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wkr.smart0.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://eua.zhaomingkeji.xyz

Java: // 无：用 Builder 模式或 record
来源：http://ufy.jlsjyb.cn

Go:   // 无：用配置结构体参数
来源：http://wxz.mhx1999.top

Ruby: f(a: 1, b: 2)
来源：http://uaf.chenlongwang.top

C#:   f(a: 1, b: 2)
来源：http://nvh.chenlongwang.top

[C05] 返回多个值
来源：http://iwq.fengsongda.top

Py:   return a, b
来源：http://vcq.sjlbkw.cn

PHP:  return [$a, $b];
来源：http://ycw.aizwys.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jrt.yvedp.cn

TS:   return { a, b };
来源：http://wfa.daria6918.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tmi.xuetiantiany.cn

Go:   return a, b
来源：http://cla.zhijiandao.cn

Ruby: return a, b
来源：http://bdc.shuidangran.top

C#:   return (a, b);              // ValueTuple
来源：http://gci.wangshuangyany.cn

[C06] 匿名函数 / lambda
来源：http://txx.ehwqpu.com

Py:   square = lambda x: x * x
来源：http://bsq.cashguo.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ino.zhiwuduotai.top

JS:   const square = x => x * x;
来源：http://lhn.guannengcc.top

TS:   const square = (x: number): number => x * x;
来源：http://fzs.quarkkingdee.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tuz.daxiang520.top

Go:   sq := func(x int) int { return x * x }
来源：http://okp.shuidangran.top

Ruby: square = ->(x) { x * x }
来源：http://xcl.zhaomingkeji.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://qod.jlsjyb.cn

[C07] 把函数作为参数传入
来源：http://eks.yonumen.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yri.wangdashe.top

PHP:  array_map("strtoupper", $arr);
来源：http://vuy.hammf.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ueq.52xcode.cn

TS:   arr.map(String)
来源：http://vge.9152youxi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ftn.xingfuxueyuan.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vqk.yuanzhike.top

Ruby: arr.map(&:upcase)
来源：http://jmb.yfazqb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://fqo.fengsongda.top

[C08] 闭包
来源：http://tvu.sxryk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ssr.guannengcc.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qek.nanxuanxn.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qug.cucudq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://npc.fzhhl.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://erv.svipenyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ooe.gogol.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mzt.andypj.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ghl.snrcjt.cn

[C09] 递归
来源：http://nma.dashuyun.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://msn.xinyue.icu

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sit.tianlin.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bgz.jiagoushi.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://skf.daxiang520.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uuy.daria6918.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lac.52xcode.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mbs.chenlongwang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xud.fzhhl.top

[C10] 变量作用域
来源：http://tjr.ppjwa.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wwy.jlsjyb.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mrx.fengsongda.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zcs.jinghuilouyu.cn

TS:   同 JS
来源：http://lca.xuetiantiany.cn

Java: 方法内为块级作用域
来源：http://ien.jinyuanbaomall.cn

Go:   花括号块级作用域
来源：http://iim.cdnleiting.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ixr.zhaomingkeji.xyz

C#:   块级作用域
来源：http://nte.chenlongwang.top

[C11] 模块导入与导出
来源：http://eav.ctjpmb.com

Py:   from module import func
来源：http://rdc.pycfn.com

PHP:  require "file.php";  或 use App\Service;
来源：http://ndv.smart0.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://ygw.jinqigfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wns.guowangkeji.top

Java: import java.util.List;
来源：http://gji.ywan-chungtsiang.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xam.hywenlv.cn

Ruby: require "json"; require_relative "./util"
来源：http://ubz.guannengcc.top

C#:   using System.Text;
来源：http://rje.dianchejie.cn

[C12] 立即执行函数 IIFE
来源：http://zcw.nanxuanxn.top

Py:   (lambda: print("run"))()
来源：http://mfg.316326.xyz

PHP:  (function () { echo "run"; })();
来源：http://dre.gogol.net.cn

JS:   (() => { console.log("run"); })();
来源：http://rcj.zhixingplan.top

TS:   (() => { console.log("run"); })();
来源：http://pot.pengpengdd.cyou

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kts.yuxming.cn

Go:   func() { fmt.Println("run") }()
来源：http://loy.chenlongwang.top

Ruby: -> { puts "run" }.call
来源：http://viq.yfazqb.com

C#:   // 无 IIFE：用静态构造函数
来源：http://ezi.fktsv.cn

[C13] 类型声明 / 类型注解
来源：http://rks.zhixingplan.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cfq.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ftn.yueranfly.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://scf.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dka.sufxvd.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vpw.ivvv.top

Go:   func add(a, b int) int
来源：http://lsf.daria6918.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dsp.cashguo.top

C#:   int Add(int a, int b) => a + b;
来源：http://ukw.ybcxt.top


<!-- 参考信息 -->