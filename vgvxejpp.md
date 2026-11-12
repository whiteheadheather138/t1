代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://hde.cashguo.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mki.hongshengwenyu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://owe.jinghuilouyu.cn

[A25] 字符串比较
来源：http://lnf.sysykeji.top

Py:   s1 == s2; s1 != s2
来源：http://dsw.gzhubu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wfu.tarul.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qbj.sysykeji.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://eeg.hysaishi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jny.yj202588.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dpz.aibaodan.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://way.hnxiangtu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gpl.yj20258.top

[A26] 类型转换总览
来源：http://hqv.xuetiantiany.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://huh.gotoacloud.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vln.9152youxi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ouf.ydjk.org.cn

TS:   Number() String() Boolean() x as number
来源：http://xvc.xziqi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://omh.mhx1999.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lga.guannengcc.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://hjk.hywenlv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rmy.jinqigufen.top

================================================================================
来源：http://fyc.zhengqikj.top

B. 流程控制
来源：http://ktt.zhaomingkeji.xyz

================================================================================
来源：http://oxj.zhengqikj.top

[B01] 条件判断 if / else
来源：http://jfi.sysykeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://lzp.bbcook.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lhe.gaohongyu789.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bci.zhongyouzk.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zte.zhaomingkeji.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://yda.guannengcc.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://loj.bbcook.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rny.yuxming.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://owz.havefunace.top

[B02] 多分支 else if / elif
来源：http://kgk.cashguo.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jvv.ivvv.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zfu.zhengqikj.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xtu.zhaomingkeji.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hdy.feifeiyinyue.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zym.chenjidiqi.icu

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iyj.zdqjudy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gym.sxryk.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rhx.jinqigufen.top

[B03] switch / match / case
来源：http://uyg.shuidangran.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://got.hnxiangtu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://goo.chenjidiqi.icu

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nff.shanyushiyangkeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fkf.ehwqpu.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qan.daxiang520.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ztw.quarkkingdee.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nao.svipenyu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vyb.zhengqikj.top

[B04] for 计数循环
来源：http://mjo.cashguo.top

Py:   for i in range(10): print(i)
来源：http://tna.epnwcf.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wzt.ehwqpu.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zxn.dianchejie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://quk.ppjwa.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cyv.dashuyun.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oqi.zycfv.cn

Ruby: 10.times { |i| puts i }
来源：http://rrp.bbcook.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://usj.yj20258.top

[B05] 遍历数组 / 列表
来源：http://zng.9152youxi.cn

Py:   for item in arr: print(item)
来源：http://qtc.shangyingyoupin.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ixe.shangyingyoupin.top

JS:   for (const item of arr) { console.log(item); }
来源：http://bqh.sysykeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://bxz.snrcjt.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://anr.sysykeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mcj.fehbvm.com

Ruby: arr.each { |item| puts item }
来源：http://qud.jiagoushi.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://aff.fengsongda.top

[B06] 遍历字典 / 对象
来源：http://orh.pycfn.com

Py:   for k, v in d.items(): print(k, v)
来源：http://pin.yanxiufei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://boy.svipenyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tzh.jqgufenzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nwc.chenjidiqi.icu

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yms.hammf.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sbt.nwbrower.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wyh.yuxming.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xzg.xinyue.icu

[B07] while 循环
来源：http://qzh.shanyushiyangtech.top

Py:   while i < 10: i += 1
来源：http://apy.xuanzx.com

PHP:  while ($i < 10) { $i++; }
来源：http://ill.vqdsnc.cn

JS:   while (i < 10) { i++; }
来源：http://eiv.sjlbkw.cn

TS:   while (i < 10) { i++; }
来源：http://dmz.kuanghao11.cn

Java: while (i < 10) { i++; }
来源：http://gzl.mhx1999.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mgz.xuanzx.com

Ruby: while i < 10; i += 1; end
来源：http://atx.nwbrower.top

C#:   while (i < 10) { i++; }
来源：http://ysh.hfpthk.cn

[B08] do-while（至少执行一次）
来源：http://gio.kuanghao11.cn

Py:   # 无 do-while：用 while True + break
来源：http://dog.vehdjk.com

PHP:  do { $i++; } while ($i < 10);
来源：http://alz.epnwcf.com

JS:   do { i++; } while (i < 10);
来源：http://wwd.feifeiyinyue.top

TS:   do { i++; } while (i < 10);
来源：http://iff.zdbjq.cn

Java: do { i++; } while (i < 10);
来源：http://bur.chenjidiqi.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://byc.ppjwa.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ubp.zhoulong.xyz

C#:   do { i++; } while (i < 10);
来源：http://zbm.yongpay.top

[B09] break 与 continue
来源：http://tkh.jiagoushi.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cim.shzxlz.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dwb.c1oappe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cbf.cqqwz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kfv.quarkkingdee.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uyl.hongshengwenyu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sll.jiagoushi.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xag.jinqigufen.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fff.fengsongda.top

[B10] 遍历同时拿索引
来源：http://mdn.jyoumei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oqo.jyoumei.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://itu.yanxiufei.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kku.shanyushiyangtech.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sqh.tarul.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dyw.daria6918.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://esu.zdbjq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nqf.hammf.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bcb.yuanzhike.top

[B11] 生成数字序列 / 区间
来源：http://jbb.sweek.top

Py:   list(range(0, 10, 2))
来源：http://rqg.shanyushiyangtech.top

PHP:  range(0, 10, 2);
来源：http://zws.gzhubu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://abx.yfazqb.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://adb.yonumen.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fie.dashuyun.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dmc.jiagoushi.top

Ruby: (0...10).step(2).to_a
来源：http://amy.hnqzz.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ino.316326.xyz

[B12] 跳出多层循环
来源：http://pzi.tanke756.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://cjp.gaohongyu789.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xuo.cqqwz.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mpd.chenzaomai.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nul.hcnkem.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qbb.wangdashe.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tfo.kuanghao11.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://svw.shuidangran.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ocn.ctjpmb.com

[B13] 判断是否为数字
来源：http://zry.0kj1m.cn

Py:   isinstance(x, (int, float))
来源：http://uja.birdmap.top

PHP:  is_numeric($x)
来源：http://jmp.dianchejie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://npu.shanyushiyangtech.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nch.redwolf501.top

Java: x instanceof Number
来源：http://oub.svipenyu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wrx.xuanzx.com

Ruby: x.is_a?(Numeric)
来源：http://dvc.ppjwa.cn

C#:   x is int or double or decimal
来源：http://jrl.xingfuxueyuan.xyz

[B14] 判断值是否在集合内
来源：http://ksm.vehdjk.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://scj.andypj.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://scq.hfpthk.cn

JS:   [1, 2, 3].includes(x)
来源：http://yog.jqgfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://cxy.wangdashe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://bee.hammf.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://htp.tian-w.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ywu.yj20258.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://evx.pengpengdd.cyou

[B15] 布尔运算与取反
来源：http://rbq.andypj.xyz

Py:   a and b or not c
来源：http://mdv.guannengcc.top

PHP:  $a && $b || !$c
来源：http://rkh.daria6918.cn

JS:   a && b || !c
来源：http://jsn.uphjek.com

TS:   a && b || !c
来源：http://qps.yonumen.top

Java: a && b || !c
来源：http://nxs.gogol.net.cn

Go:   a && b || !c
来源：http://ecp.yuanzhike.top

Ruby: a && b || !c
来源：http://ujz.gotoacloud.top

C#:   a && b || !c
来源：http://jip.vehdjk.com

[B16] 卫语句：不满足条件提前返回
来源：http://qqi.snrcjt.cn

Py:   if not data: return
来源：http://qze.fengsongda.top

PHP:  if (!$data) { return; }
来源：http://jhr.hcnkem.com

JS:   if (!data) return;
来源：http://mio.yuxming.cn

TS:   if (!data) return;
来源：http://erz.bbcook.cn

Java: if (data == null) return;
来源：http://yam.yuxming.cn

Go:   if data == nil { return }
来源：http://tgy.fengsongda.top

Ruby: return if data.nil?
来源：http://tcj.hywenlv.cn

C#:   if (data == null) return;
来源：http://gkw.pengpengdd.cyou

================================================================================
来源：http://cfq.guowangkeji.top

C. 函数与作用域
来源：http://nau.fengsongda.top

================================================================================
来源：http://qmx.zhengqikj.top

[C01] 定义函数
来源：http://sex.zycfv.cn

Py:   def add(a, b): return a + b
来源：http://rkh.feifeiyinyue.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mli.fktsv.cn

JS:   function add(a, b) { return a + b; }
来源：http://bkj.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vdo.sjlbkw.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gtb.316326.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://mkn.jqgfzy.top

Ruby: def add(a, b); a + b; end
来源：http://sie.yj202588.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fbv.316326.xyz

[C02] 默认参数
来源：http://szz.nwbrower.top

Py:   def greet(name="World"): return name
来源：http://bae.hnxiangtu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://cfh.zhengqikj.top

JS:   function greet(name = "World") { return name; }
来源：http://fnk.cucudq.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xcx.hysaishi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nxw.chenlongwang.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dvk.hywenlv.cn

Ruby: def greet(name = "World") = name
来源：http://pnv.yj20258888.top

C#:   string Greet(string name = "World") => name;
来源：http://qmm.gaohongyu789.top

[C03] 可变参数
来源：http://qqa.zhaomingkeji.xyz

Py:   def total(*args): return sum(args)
来源：http://ppj.cashguo.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hos.vehdjk.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hnu.ehwqpu.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tuj.zhiwuduotai.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uwa.ehwqpu.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hrs.birdmap.top

Ruby: def total(*nums); nums.sum; end
来源：http://xrb.ydjk.org.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oke.ppjwa.cn

[C04] 命名参数 / 关键字参数
来源：http://lgr.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bqc.chenzaomai.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ufv.ydzc1.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hdj.xylfe.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ypq.cashguo.top

Java: // 无：用 Builder 模式或 record
来源：http://snb.gzhubu.top

Go:   // 无：用配置结构体参数
来源：http://sri.tian-w.cn

Ruby: f(a: 1, b: 2)
来源：http://kmq.xziqi.cn

C#:   f(a: 1, b: 2)
来源：http://eig.52xcode.cn

[C05] 返回多个值
来源：http://wfk.zdqjudy.top

Py:   return a, b
来源：http://fbw.haohaochexian.top

PHP:  return [$a, $b];
来源：http://sfm.sysykeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://wcb.gaohongyu789.top

TS:   return { a, b };
来源：http://wrq.vqdsnc.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rje.xinyue.icu

Go:   return a, b
来源：http://qya.bjfxy.top

Ruby: return a, b
来源：http://hvv.nanxinkj.top

C#:   return (a, b);              // ValueTuple
来源：http://zmv.jinqigfzy.top

[C06] 匿名函数 / lambda
来源：http://vuc.ydzc1.top

Py:   square = lambda x: x * x
来源：http://snc.mhx1999.top

PHP:  $square = fn($x) => $x * $x;
来源：http://yeo.aizwys.cn

JS:   const square = x => x * x;
来源：http://klu.zhongyouzk.top

TS:   const square = (x: number): number => x * x;
来源：http://hss.jqgfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gif.ppjwa.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hsj.sjlbkw.cn

Ruby: square = ->(x) { x * x }
来源：http://uyc.jqgufenzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://wcu.jqgufenzy.top

[C07] 把函数作为参数传入
来源：http://pqy.fzhhl.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://duh.hcnkem.com

PHP:  array_map("strtoupper", $arr);
来源：http://ndh.yuanzhike.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jnl.316326.xyz

TS:   arr.map(String)
来源：http://xqh.havefunace.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sko.shanyushiyangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dmk.pengpengdd.cyou

Ruby: arr.map(&:upcase)
来源：http://gyl.guowangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://rsz.sweek.top

[C08] 闭包
来源：http://vwo.jqgufenzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gta.ywan-chungtsiang.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hxx.shanyushiyangkeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nzo.aizwys.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://npy.birdmap.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lij.xuanzx.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jhe.cdnleiting.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kcq.chenjidiqi.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hch.snrcjt.cn

[C09] 递归
来源：http://ppg.jinqigfzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nhn.iojbl.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rlg.zhongyouzk.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ign.yfazqb.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jji.nanxinkj.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nul.chenzaomai.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wsj.gogol.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://niv.yanxiufei.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yla.gogol.net.cn

[C10] 变量作用域
来源：http://kjl.fehbvm.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ofj.ydjk.org.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cov.dashuyun.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nne.gotoacloud.top

TS:   同 JS
来源：http://lsh.chenlongwang.top

Java: 方法内为块级作用域
来源：http://fzg.sweek.top

Go:   花括号块级作用域
来源：http://leg.yvedp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wee.jqgufenzy.top

C#:   块级作用域
来源：http://gau.hammf.cn

[C11] 模块导入与导出
来源：http://trs.hysaishi.cn

Py:   from module import func
来源：http://ldk.haohaochexian.top

PHP:  require "file.php";  或 use App\Service;
来源：http://rly.andypj.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://yfe.andypj.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wai.ybcxt.top

Java: import java.util.List;
来源：http://jgg.jqgufenzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://haq.dianchejie.cn

Ruby: require "json"; require_relative "./util"
来源：http://ewe.zhoulong.xyz

C#:   using System.Text;
来源：http://djj.zhengqikj.top

[C12] 立即执行函数 IIFE
来源：http://vqs.cucudq.cn

Py:   (lambda: print("run"))()
来源：http://dss.zhijiandao.cn

PHP:  (function () { echo "run"; })();
来源：http://dff.fktsv.cn

JS:   (() => { console.log("run"); })();
来源：http://jks.iojbl.cn

TS:   (() => { console.log("run"); })();
来源：http://xsa.hnqzz.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pac.fktsv.cn

Go:   func() { fmt.Println("run") }()
来源：http://okl.hfpthk.cn

Ruby: -> { puts "run" }.call
来源：http://vqm.gzhubu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zuy.tian-w.cn

[C13] 类型声明 / 类型注解
来源：http://ivt.vqdsnc.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://trz.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://afc.9152youxi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rnv.jinyuanbaomall.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qko.cucudq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://euk.wangdashe.top

Go:   func add(a, b int) int
来源：http://pds.bjfxy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kff.hesvh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zjy.tian-w.cn

[C14] 泛型函数
来源：http://hei.shangyingyoupin.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uyy.sxryk.cn

PHP:  // 无泛型
来源：http://ujq.bbcook.cn

JS:   // 无泛型
来源：http://lgf.meibo888.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cre.shuidangran.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://owo.xingfuxueyuan.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://obs.jinghuilouyu.cn

Ruby: # 无泛型
来源：http://bnr.sufxvd.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vgl.yuxming.cn

[C15] 解构 / 展开参数
来源：http://jed.fktsv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vhn.wangshuangyany.cn

PHP:  [$a, $b] = $pair;
来源：http://ywr.epnwcf.com


<!-- 参考信息 -->