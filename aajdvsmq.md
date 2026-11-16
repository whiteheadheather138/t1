代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://duq.nwbrower.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yij.gaohongyu789.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lhi.nwbrower.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pet.snrcjt.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ctm.fengsongda.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lre.hywenlv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zvi.ppjwa.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://inv.yfazqb.com

[A26] 类型转换总览
来源：http://xfk.chenzaomai.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dvr.jqgufenzy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ubp.vehdjk.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fns.birdmap.top

TS:   Number() String() Boolean() x as number
来源：http://dgb.jinqigufen.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zbr.316326.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://aah.jianghu66.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://szy.hesvh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gms.yj20258.top

================================================================================
来源：http://jfn.daxiang520.top

B. 流程控制
来源：http://ffr.hnqzz.top

================================================================================
来源：http://wcx.chenlongwang.top

[B01] 条件判断 if / else
来源：http://rpr.xuetiantiany.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bux.shangyingyoupin.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fdz.haohaochexian.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rww.shanyushiyangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://too.yangfankeji.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://him.nanxinkj.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qhf.ppjwa.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fry.aibaodan.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ddz.kuanghao11.cn

[B02] 多分支 else if / elif
来源：http://geo.epnwcf.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nvq.zhiwuduotai.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bip.sufxvd.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lsa.ctjpmb.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pch.quarkkingdee.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rig.svipenyu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xbj.yfazqb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pdr.jinqigfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lgw.jqgufenzy.top

[B03] switch / match / case
来源：http://wsy.hammf.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yoj.gogol.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bhc.hnqzz.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://chm.cheryme.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nkd.gogol.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://trn.ppjwa.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://njc.andypj.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ujb.andypj.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://unq.snrcjt.cn

[B04] for 计数循环
来源：http://xjt.gogol.net.cn

Py:   for i in range(10): print(i)
来源：http://qvq.yj20258888.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://czt.bjfxy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dll.fktsv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://orl.vqdsnc.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bwx.wangdashe.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oiz.sysykeji.top

Ruby: 10.times { |i| puts i }
来源：http://mca.tarul.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://muz.shangyingyoupin.top

[B05] 遍历数组 / 列表
来源：http://iqa.zhaomingkeji.xyz

Py:   for item in arr: print(item)
来源：http://rrx.shangyingyoupin.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://paf.nwbrower.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ict.bbcook.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nsy.0kj1m.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dii.fengsongda.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dco.xuetiantiany.cn

Ruby: arr.each { |item| puts item }
来源：http://tqz.shanyushiyangkeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://iyg.hfpthk.cn

[B06] 遍历字典 / 对象
来源：http://usx.zdqjudy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://yeb.uphjek.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://njc.cdnleiting.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://umo.bbcook.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://otk.xingfuxueyuan.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vmr.guannengcc.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ffq.zhixingplan.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lpq.52xcode.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vck.ppjwa.cn

[B07] while 循环
来源：http://llg.nanxuanxn.top

Py:   while i < 10: i += 1
来源：http://otd.bjfxy.top

PHP:  while ($i < 10) { $i++; }
来源：http://ylv.jianghu66.top

JS:   while (i < 10) { i++; }
来源：http://pxj.yfazqb.com

TS:   while (i < 10) { i++; }
来源：http://urk.fktsv.cn

Java: while (i < 10) { i++; }
来源：http://umg.yuanzhike.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ceu.cashguo.top

Ruby: while i < 10; i += 1; end
来源：http://kuu.andypj.xyz

C#:   while (i < 10) { i++; }
来源：http://wrn.snrcjt.cn

[B08] do-while（至少执行一次）
来源：http://aej.mhx1999.top

Py:   # 无 do-while：用 while True + break
来源：http://cfq.52xcode.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fqx.zhixingplan.top

JS:   do { i++; } while (i < 10);
来源：http://fmz.aizwys.cn

TS:   do { i++; } while (i < 10);
来源：http://yyh.yj20258888.top

Java: do { i++; } while (i < 10);
来源：http://frz.redwolf501.top

Go:   for { i++; if i >= 10 { break } }
来源：http://mmz.fengsongda.top

Ruby: begin; i += 1; end while i < 10
来源：http://yoj.feifeiyinyue.top

C#:   do { i++; } while (i < 10);
来源：http://ldc.shanyushiyangkeji.top

[B09] break 与 continue
来源：http://vec.quarkkingdee.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ppj.chenzaomai.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sjh.shuidangran.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bzx.316326.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fvs.cqqwz.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vvq.sxryk.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kfj.jinqigfzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rqx.cdnleiting.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sua.cucudq.cn

[B10] 遍历同时拿索引
来源：http://jel.jinqigufen.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ryj.yangfankeji.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mwq.yuanzhike.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://eov.sysykeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rcr.fengsongda.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tgw.shanyushiyangkeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://grt.zhixingplan.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nsh.fktsv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hau.vqdsnc.cn

[B11] 生成数字序列 / 区间
来源：http://wtj.gotoacloud.top

Py:   list(range(0, 10, 2))
来源：http://xts.cheryme.top

PHP:  range(0, 10, 2);
来源：http://iyr.fehbvm.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xof.haohaochexian.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vjn.9152youxi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hss.xinyue.icu

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://khc.zhongyouzk.top

Ruby: (0...10).step(2).to_a
来源：http://wmp.jiagoushi.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lxu.gaohongyu789.top

[B12] 跳出多层循环
来源：http://dwf.gogol.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qpo.yj20258.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://oxb.fengsongda.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ysf.ctjpmb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pkx.havefunace.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gwa.haohaochexian.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aeh.hfpthk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wcy.bjfxy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nxo.tanke756.top

[B13] 判断是否为数字
来源：http://tcp.shanyushiyangkeji.top

Py:   isinstance(x, (int, float))
来源：http://fuj.gzhubu.top

PHP:  is_numeric($x)
来源：http://xlk.jyoumei.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fbo.hywenlv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gqx.yonumen.top

Java: x instanceof Number
来源：http://fgr.guannengcc.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hlg.jinyuanbaomall.cn

Ruby: x.is_a?(Numeric)
来源：http://nnc.yj20258888.top

C#:   x is int or double or decimal
来源：http://bcc.haohaochexian.top

[B14] 判断值是否在集合内
来源：http://lpc.jinqigufen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rez.tianlin.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ixy.guowangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://vjr.pengpengdd.cyou

TS:   [1, 2, 3].includes(x)
来源：http://fmp.daria6918.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nkb.jqgufenzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xxc.fktsv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://axw.iojbl.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ckx.vehdjk.com

[B15] 布尔运算与取反
来源：http://ocv.dianchejie.cn

Py:   a and b or not c
来源：http://gkk.pengpengdd.cyou

PHP:  $a && $b || !$c
来源：http://jyq.xziqi.cn

JS:   a && b || !c
来源：http://dyd.tianlin.xyz

TS:   a && b || !c
来源：http://itg.jinqigfzy.top

Java: a && b || !c
来源：http://onn.jinqigufen.top

Go:   a && b || !c
来源：http://wcc.aibaodan.cn

Ruby: a && b || !c
来源：http://idt.jinqigfzy.top

C#:   a && b || !c
来源：http://mos.316326.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://oom.zhixingplan.top

Py:   if not data: return
来源：http://csh.hywenlv.cn

PHP:  if (!$data) { return; }
来源：http://rat.nwbrower.top

JS:   if (!data) return;
来源：http://lwm.havefunace.top

TS:   if (!data) return;
来源：http://rvd.jlsjyb.cn

Java: if (data == null) return;
来源：http://roz.hesvh.cn

Go:   if data == nil { return }
来源：http://jqw.sjlbkw.cn

Ruby: return if data.nil?
来源：http://sfi.dianchejie.cn

C#:   if (data == null) return;
来源：http://nbb.yuxming.cn

================================================================================
来源：http://ggr.daria6918.cn

C. 函数与作用域
来源：http://tsy.andypj.xyz

================================================================================
来源：http://nge.zdqjudy.top

[C01] 定义函数
来源：http://wds.yangfankeji.com

Py:   def add(a, b): return a + b
来源：http://qyz.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ffa.zhoulong.xyz

JS:   function add(a, b) { return a + b; }
来源：http://dxa.zdbjq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lff.vehdjk.com

Java: static int add(int a, int b) { return a + b; }
来源：http://rib.wangdashe.top

Go:   func add(a, b int) int { return a + b }
来源：http://bug.pengpengdd.cyou

Ruby: def add(a, b); a + b; end
来源：http://snz.hcnkem.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qkd.zycfv.cn

[C02] 默认参数
来源：http://ixt.uphjek.com

Py:   def greet(name="World"): return name
来源：http://nyx.bbcook.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vcx.tian-w.cn

JS:   function greet(name = "World") { return name; }
来源：http://rbh.zhengqikj.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fdp.nanxinkj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://rkf.andypj.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mwz.316326.xyz

Ruby: def greet(name = "World") = name
来源：http://stt.andypj.xyz

C#:   string Greet(string name = "World") => name;
来源：http://efb.zycfv.cn

[C03] 可变参数
来源：http://cmt.aibaodan.cn

Py:   def total(*args): return sum(args)
来源：http://ifn.daxiang520.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zqa.iojbl.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zeo.xuetiantiany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ebi.aizwys.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dxw.zhongyouzk.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hhj.kuanghao11.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nyn.gogol.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mlc.hnxiangtu.top

[C04] 命名参数 / 关键字参数
来源：http://unm.hnxiangtu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hfr.zdqjudy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wie.birdmap.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jhm.ydzc1.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iqf.cdnleiting.top

Java: // 无：用 Builder 模式或 record
来源：http://qza.zdqjudy.top

Go:   // 无：用配置结构体参数
来源：http://wej.hcnkem.com

Ruby: f(a: 1, b: 2)
来源：http://rmg.jqgufenzy.top

C#:   f(a: 1, b: 2)
来源：http://wjf.jyoumei.cn

[C05] 返回多个值
来源：http://xlr.ybcxt.top

Py:   return a, b
来源：http://asr.pengpengdd.cyou

PHP:  return [$a, $b];
来源：http://tfk.xinyue.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://nht.epnwcf.com

TS:   return { a, b };
来源：http://nal.andypj.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://npi.ybcxt.top

Go:   return a, b
来源：http://bne.andypj.xyz

Ruby: return a, b
来源：http://vaj.smart0.xyz

C#:   return (a, b);              // ValueTuple
来源：http://uxr.hnxiangtu.top

[C06] 匿名函数 / lambda
来源：http://beh.fzhhl.top

Py:   square = lambda x: x * x
来源：http://zzw.hammf.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pwi.jqgfzy.top

JS:   const square = x => x * x;
来源：http://ogi.kuanghao11.cn

TS:   const square = (x: number): number => x * x;
来源：http://xhp.guowangkeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gsj.ydjk.org.cn

Go:   sq := func(x int) int { return x * x }
来源：http://izh.sufxvd.cn

Ruby: square = ->(x) { x * x }
来源：http://bee.yueranfly.top

C#:   Func<int, int> square = x => x * x;
来源：http://ukd.pengpengdd.cyou

[C07] 把函数作为参数传入
来源：http://nct.gaohongyu789.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dda.yj20258888.top

PHP:  array_map("strtoupper", $arr);
来源：http://uap.yfazqb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uze.yangfankeji.com

TS:   arr.map(String)
来源：http://cwv.ivvv.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zat.gotoacloud.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wph.fktsv.cn

Ruby: arr.map(&:upcase)
来源：http://dck.zhengqikj.top

C#:   arr.Select(s => s.ToUpper())
来源：http://auu.zhiwuduotai.top

[C08] 闭包
来源：http://bjr.hfpthk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xdc.hongshengwenyu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yoh.yueranfly.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://llb.jinghuilouyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://swi.dashuyun.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://muv.hcnkem.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fsf.daria6918.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jyv.nanxinkj.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://itr.chenzaomai.com

[C09] 递归
来源：http://svq.xingfuxueyuan.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://drg.jqgfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ozh.yonumen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rjk.haohaochexian.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uaq.cucudq.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rsb.yonumen.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cic.meibo888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://znr.jinyuanbaomall.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rtb.shanyushiyangtech.top

[C10] 变量作用域
来源：http://upy.tarul.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://czo.yongpay.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://eke.ivvv.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ghs.gzhubu.top

TS:   同 JS
来源：http://hqz.yj20258888.top

Java: 方法内为块级作用域
来源：http://txc.hammf.cn

Go:   花括号块级作用域
来源：http://cbb.mhx1999.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://axb.vehdjk.com

C#:   块级作用域
来源：http://kkp.yj202588.top

[C11] 模块导入与导出
来源：http://lpf.zhijiandao.cn

Py:   from module import func
来源：http://zfj.aibaodan.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bix.cdnleiting.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://uyy.yanxiufei.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qdu.sweek.top

Java: import java.util.List;
来源：http://arl.hysaishi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bdn.ydjk.org.cn

Ruby: require "json"; require_relative "./util"
来源：http://cmc.hnqzz.top

C#:   using System.Text;
来源：http://kfu.daxiang520.top

[C12] 立即执行函数 IIFE
来源：http://mtd.nwbrower.top

Py:   (lambda: print("run"))()
来源：http://vwr.aizwys.cn

PHP:  (function () { echo "run"; })();
来源：http://kdr.ybcxt.top

JS:   (() => { console.log("run"); })();
来源：http://ufo.hywenlv.cn

TS:   (() => { console.log("run"); })();
来源：http://klm.hcnkem.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wlf.316326.xyz

Go:   func() { fmt.Println("run") }()
来源：http://zlv.shanyushiyangkeji.top

Ruby: -> { puts "run" }.call
来源：http://rzn.316326.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://iel.shangyingyoupin.top

[C13] 类型声明 / 类型注解
来源：http://tps.zhaomingkeji.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xaz.birdmap.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cye.c1oappe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cjn.iojbl.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zor.yangfankeji.com

Java: int add(int a, int b) { return a + b; }
来源：http://cgn.sweek.top

Go:   func add(a, b int) int
来源：http://crn.birdmap.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ulk.snrcjt.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tfs.meibo888.top

[C14] 泛型函数
来源：http://uou.pengpengdd.cyou

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://omp.zdbjq.cn

PHP:  // 无泛型
来源：http://woe.hnqzz.top

JS:   // 无泛型
来源：http://ful.sysykeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uzr.cdnleiting.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lhd.0kj1m.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vuv.chenzaomai.com

Ruby: # 无泛型
来源：http://qeg.shzxlz.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kfi.bbcook.cn

[C15] 解构 / 展开参数
来源：http://xqb.ywan-chungtsiang.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tts.aibaodan.cn

PHP:  [$a, $b] = $pair;
来源：http://euo.nanxinkj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dcl.pengpengdd.cyou

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://twh.yuxming.cn

Java: // 无解构
来源：http://bjr.fehbvm.com

Go:   // 无解构
来源：http://ihv.sufxvd.cn


<!-- 参考信息 -->