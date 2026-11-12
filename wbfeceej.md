代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://fnm.meibo888.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://evm.jinyuanbaomall.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yji.xingfuxueyuan.xyz

[A25] 字符串比较
来源：http://pgx.zdbjq.cn

Py:   s1 == s2; s1 != s2
来源：http://kyi.zhijiandao.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zqr.cqqwz.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mxb.nanxuanxn.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://shh.daxiang520.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://noe.xylfe.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zdu.pengpengdd.cyou

Ruby: s1 == s2; s1 <=> s2
来源：http://iyw.aibaodan.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://syx.sxryk.cn

[A26] 类型转换总览
来源：http://fia.ivvv.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://psr.jinqigufen.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qdz.zhijiandao.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qlt.yuxming.cn

TS:   Number() String() Boolean() x as number
来源：http://vwd.sufxvd.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://moa.hnqzz.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://snu.hysaishi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://iml.yangfankeji.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zqz.0kj1m.cn

================================================================================
来源：http://bts.xylfe.cn

B. 流程控制
来源：http://mjk.yvedp.cn

================================================================================
来源：http://qjn.gaohongyu789.top

[B01] 条件判断 if / else
来源：http://lnt.yvedp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mrf.jianghu66.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sml.wangshuangyany.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iay.bbcook.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cny.nanxinkj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://owb.hysaishi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ycm.hnxiangtu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://khv.xziqi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xvo.tianlin.xyz

[B02] 多分支 else if / elif
来源：http://ejd.guowangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zag.fktsv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ygn.yfazqb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rlg.yueranfly.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ywg.sweek.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zeb.0kj1m.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fgc.smart0.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ixo.meibo888.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xiu.ehwqpu.com

[B03] switch / match / case
来源：http://uja.zdbjq.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yuh.hnxiangtu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://asq.shuidangran.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://liz.jqgfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zek.jinqigfzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jyu.sxryk.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ows.fzhhl.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fde.fzhhl.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://woq.jlsjyb.cn

[B04] for 计数循环
来源：http://ulf.yongpay.top

Py:   for i in range(10): print(i)
来源：http://idy.yj20258.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vzw.shanyushiyangkeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lkh.bjfxy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cqf.shangyingyoupin.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dtd.jinghuilouyu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://psu.fktsv.cn

Ruby: 10.times { |i| puts i }
来源：http://fgh.pengpengdd.cyou

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mfv.aizwys.cn

[B05] 遍历数组 / 列表
来源：http://nbw.hywenlv.cn

Py:   for item in arr: print(item)
来源：http://msl.ybcxt.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pkd.hcnkem.com

JS:   for (const item of arr) { console.log(item); }
来源：http://tbg.epnwcf.com

TS:   for (const item of arr) { console.log(item); }
来源：http://tqo.zhiwuduotai.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wao.dashuyun.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rdd.hammf.cn

Ruby: arr.each { |item| puts item }
来源：http://qay.shanyushiyangtech.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://unv.tian-w.cn

[B06] 遍历字典 / 对象
来源：http://dua.yj202588.top

Py:   for k, v in d.items(): print(k, v)
来源：http://oiv.ydjk.org.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yjh.tarul.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://stv.jinqigfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wib.xuetiantiany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ibo.sweek.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jwa.pengpengdd.cyou

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oso.gogol.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://acm.yuxming.cn

[B07] while 循环
来源：http://lgd.jinqigfzy.top

Py:   while i < 10: i += 1
来源：http://pgt.zdbjq.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qme.aibaodan.cn

JS:   while (i < 10) { i++; }
来源：http://hnt.yj202588.top

TS:   while (i < 10) { i++; }
来源：http://quv.sweek.top

Java: while (i < 10) { i++; }
来源：http://tck.bbcook.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ert.yfazqb.com

Ruby: while i < 10; i += 1; end
来源：http://mqs.zhongyouzk.top

C#:   while (i < 10) { i++; }
来源：http://myr.wangdashe.top

[B08] do-while（至少执行一次）
来源：http://yvh.hfpthk.cn

Py:   # 无 do-while：用 while True + break
来源：http://vqp.vqdsnc.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gvy.chenzaomai.com

JS:   do { i++; } while (i < 10);
来源：http://wfv.shanyushiyangtech.top

TS:   do { i++; } while (i < 10);
来源：http://zku.cashguo.top

Java: do { i++; } while (i < 10);
来源：http://saw.yanxiufei.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://eit.ctjpmb.com

Ruby: begin; i += 1; end while i < 10
来源：http://blx.xylfe.cn

C#:   do { i++; } while (i < 10);
来源：http://uxl.vqdsnc.cn

[B09] break 与 continue
来源：http://vph.daxiang520.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ign.xuanzx.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://msa.meibo888.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hqf.hysaishi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qqn.zhoulong.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wuc.yj20258.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hyp.ydjk.org.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xsw.hammf.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://chw.havefunace.top

[B10] 遍历同时拿索引
来源：http://mqg.vehdjk.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gdp.dashuyun.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fxe.cheryme.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://euu.hesvh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://alu.wangshuangyany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tog.zycfv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kmv.vqdsnc.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qat.havefunace.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ctr.0kj1m.cn

[B11] 生成数字序列 / 区间
来源：http://oow.jlsjyb.cn

Py:   list(range(0, 10, 2))
来源：http://dqa.ehwqpu.com

PHP:  range(0, 10, 2);
来源：http://ogz.xingfuxueyuan.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aqw.xingfuxueyuan.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hen.hysaishi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gpu.dashuyun.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ray.cashguo.top

Ruby: (0...10).step(2).to_a
来源：http://vtu.52xcode.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ntm.ppjwa.cn

[B12] 跳出多层循环
来源：http://zwu.jinqigufen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://blc.yj20258888.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://dro.zdqjudy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jlq.dashuyun.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lvw.zhijiandao.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jan.cucudq.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cjn.gotoacloud.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xrd.wangdashe.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://laz.bbcook.cn

[B13] 判断是否为数字
来源：http://xpq.fanxiaobao.xyz

Py:   isinstance(x, (int, float))
来源：http://jvv.ppjwa.cn

PHP:  is_numeric($x)
来源：http://ikf.sufxvd.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zpl.sufxvd.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ocz.fzhhl.top

Java: x instanceof Number
来源：http://ugh.xylfe.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ppq.epnwcf.com

Ruby: x.is_a?(Numeric)
来源：http://dvo.jiagoushi.top

C#:   x is int or double or decimal
来源：http://ysp.aibaodan.cn

[B14] 判断值是否在集合内
来源：http://jkk.hysaishi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yvw.mhx1999.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dzk.yuanzhike.top

JS:   [1, 2, 3].includes(x)
来源：http://hfs.fktsv.cn

TS:   [1, 2, 3].includes(x)
来源：http://gsp.ywan-chungtsiang.top

Java: List.of(1, 2, 3).contains(x)
来源：http://tcl.fzhhl.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ucv.yvedp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ogp.andypj.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://knl.zhaomingkeji.xyz

[B15] 布尔运算与取反
来源：http://izx.shangyingyoupin.top

Py:   a and b or not c
来源：http://qpq.yfazqb.com

PHP:  $a && $b || !$c
来源：http://hgu.zhiwuduotai.top

JS:   a && b || !c
来源：http://qli.ywan-chungtsiang.top

TS:   a && b || !c
来源：http://skp.xingfuxueyuan.xyz

Java: a && b || !c
来源：http://rkh.meibo888.top

Go:   a && b || !c
来源：http://mwm.hammf.cn

Ruby: a && b || !c
来源：http://lpn.shuidangran.top

C#:   a && b || !c
来源：http://xhr.redwolf501.top

[B16] 卫语句：不满足条件提前返回
来源：http://wzz.jinghuilouyu.cn

Py:   if not data: return
来源：http://ocn.aizwys.cn

PHP:  if (!$data) { return; }
来源：http://ygr.yfazqb.com

JS:   if (!data) return;
来源：http://hrk.nanxinkj.top

TS:   if (!data) return;
来源：http://dbx.fanxiaobao.xyz

Java: if (data == null) return;
来源：http://psj.yj20258.top

Go:   if data == nil { return }
来源：http://hce.jinqigfzy.top

Ruby: return if data.nil?
来源：http://xom.jlsjyb.cn

C#:   if (data == null) return;
来源：http://okv.yanxiufei.cn

================================================================================
来源：http://egw.guannengcc.top

C. 函数与作用域
来源：http://xgz.guowangkeji.top

================================================================================
来源：http://ofa.guannengcc.top

[C01] 定义函数
来源：http://exe.bjfxy.top

Py:   def add(a, b): return a + b
来源：http://noj.xuetiantiany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wux.yangfankeji.com

JS:   function add(a, b) { return a + b; }
来源：http://etx.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://adh.pengpengdd.cyou

Java: static int add(int a, int b) { return a + b; }
来源：http://vfp.pengpengdd.cyou

Go:   func add(a, b int) int { return a + b }
来源：http://hjh.cucudq.cn

Ruby: def add(a, b); a + b; end
来源：http://sfe.ivvv.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xkx.aibaodan.cn

[C02] 默认参数
来源：http://opv.jinqigfzy.top

Py:   def greet(name="World"): return name
来源：http://ggz.tarul.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lox.fehbvm.com

JS:   function greet(name = "World") { return name; }
来源：http://twy.yj20258.top

TS:   function greet(name: string = "World") { return name; }
来源：http://sci.tian-w.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://umb.hnqzz.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iac.fanxiaobao.xyz

Ruby: def greet(name = "World") = name
来源：http://lsh.hesvh.cn

C#:   string Greet(string name = "World") => name;
来源：http://ndd.gaohongyu789.top

[C03] 可变参数
来源：http://lxo.zhoulong.xyz

Py:   def total(*args): return sum(args)
来源：http://aff.tianlin.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gcj.ehwqpu.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hfl.xylfe.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://onn.xinyue.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://saa.jiagoushi.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://twv.yuxming.cn

Ruby: def total(*nums); nums.sum; end
来源：http://eag.sweek.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rvy.zhijiandao.cn

[C04] 命名参数 / 关键字参数
来源：http://djb.hnxiangtu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nam.yueranfly.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lxt.xylfe.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qti.hnxiangtu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vwf.jqgufenzy.top

Java: // 无：用 Builder 模式或 record
来源：http://zso.0kj1m.cn

Go:   // 无：用配置结构体参数
来源：http://qlr.ywan-chungtsiang.top

Ruby: f(a: 1, b: 2)
来源：http://wza.yongpay.top

C#:   f(a: 1, b: 2)
来源：http://qgh.nanxinkj.top

[C05] 返回多个值
来源：http://lmb.9152youxi.cn

Py:   return a, b
来源：http://qrg.shanyushiyangtech.top

PHP:  return [$a, $b];
来源：http://trx.fanxiaobao.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://aty.yvedp.cn

TS:   return { a, b };
来源：http://irh.pengpengdd.cyou

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qus.hywenlv.cn

Go:   return a, b
来源：http://fcb.hongshengwenyu.top

Ruby: return a, b
来源：http://xpg.guannengcc.top

C#:   return (a, b);              // ValueTuple
来源：http://apq.xuetiantiany.cn

[C06] 匿名函数 / lambda
来源：http://udv.cucudq.cn

Py:   square = lambda x: x * x
来源：http://rbz.9152youxi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ddb.ivvv.top

JS:   const square = x => x * x;
来源：http://bmq.0kj1m.cn

TS:   const square = (x: number): number => x * x;
来源：http://zmi.xinyue.icu

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vpi.sxryk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://awc.zhengqikj.top

Ruby: square = ->(x) { x * x }
来源：http://zmb.daxiang520.top

C#:   Func<int, int> square = x => x * x;
来源：http://cuq.jinqigfzy.top

[C07] 把函数作为参数传入
来源：http://lyx.shanyushiyangkeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ybq.sweek.top

PHP:  array_map("strtoupper", $arr);
来源：http://zcm.zycfv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ggj.havefunace.top

TS:   arr.map(String)
来源：http://cqu.guowangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zot.ivvv.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hce.shanyushiyangkeji.top

Ruby: arr.map(&:upcase)
来源：http://dwd.chenjidiqi.icu

C#:   arr.Select(s => s.ToUpper())
来源：http://rzz.sysykeji.top

[C08] 闭包
来源：http://ygj.kuanghao11.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ofz.cashguo.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nvk.jinghuilouyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ifj.zhixingplan.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://aim.shanyushiyangtech.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wvl.zhoulong.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vlu.chenzaomai.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rbl.hongshengwenyu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vxs.fehbvm.com

[C09] 递归
来源：http://kzj.shuidangran.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rkb.c1oappe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jcl.nanxinkj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jbi.zhiwuduotai.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wis.hysaishi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qyr.snrcjt.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jpz.xuanzx.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jux.fzhhl.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://taf.quarkkingdee.top

[C10] 变量作用域
来源：http://usl.dashuyun.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mht.chenjidiqi.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://scb.wangdashe.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dpt.jyoumei.cn

TS:   同 JS
来源：http://rkr.nanxinkj.top

Java: 方法内为块级作用域
来源：http://abb.jlsjyb.cn

Go:   花括号块级作用域
来源：http://xob.ppjwa.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uee.yuxming.cn

C#:   块级作用域
来源：http://mox.wangdashe.top

[C11] 模块导入与导出
来源：http://kfd.hywenlv.cn

Py:   from module import func
来源：http://dgz.jqgfzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://cws.bjfxy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xnw.gaohongyu789.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://naq.zdbjq.cn

Java: import java.util.List;
来源：http://jnt.ydjk.org.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pgo.chenzaomai.com

Ruby: require "json"; require_relative "./util"
来源：http://qop.fengsongda.top

C#:   using System.Text;
来源：http://bpo.bbcook.cn

[C12] 立即执行函数 IIFE
来源：http://gma.cdnleiting.top

Py:   (lambda: print("run"))()
来源：http://ctz.cqqwz.cn

PHP:  (function () { echo "run"; })();
来源：http://olm.svipenyu.cn

JS:   (() => { console.log("run"); })();
来源：http://boh.feifeiyinyue.top

TS:   (() => { console.log("run"); })();
来源：http://uzg.zhoulong.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://puu.shanyushiyangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://nxy.shanyushiyangkeji.top

Ruby: -> { puts "run" }.call
来源：http://bji.316326.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://jrg.tarul.cn

[C13] 类型声明 / 类型注解
来源：http://ioo.haohaochexian.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xxf.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eoj.wangdashe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xrd.iojbl.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zhv.xziqi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://eie.cashguo.top

Go:   func add(a, b int) int
来源：http://lcz.aibaodan.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://omu.yj202588.top

C#:   int Add(int a, int b) => a + b;
来源：http://btt.shanyushiyangtech.top

[C14] 泛型函数
来源：http://qfu.aibaodan.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://flq.zhixingplan.top

PHP:  // 无泛型
来源：http://ffg.hongshengwenyu.top

JS:   // 无泛型
来源：http://jgr.shanyushiyangkeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mzy.tianlin.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lpe.cucudq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xfh.jinghuilouyu.cn

Ruby: # 无泛型
来源：http://bqh.fengsongda.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qlq.gzhubu.top

[C15] 解构 / 展开参数
来源：http://hli.tarul.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://upm.shangyingyoupin.top

PHP:  [$a, $b] = $pair;
来源：http://mhy.fktsv.cn


<!-- 参考信息 -->