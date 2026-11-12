代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://itx.xinyue.icu

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xua.feifeiyinyue.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://chy.cheryme.top

[A25] 字符串比较
来源：http://czi.ctjpmb.com

Py:   s1 == s2; s1 != s2
来源：http://evl.shanyushiyangtech.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://myo.ybcxt.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ylh.cqqwz.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nnl.jinghuilouyu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pdl.bbcook.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cqg.feifeiyinyue.top

Ruby: s1 == s2; s1 <=> s2
来源：http://noh.shanyushiyangtech.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rnc.mhx1999.top

[A26] 类型转换总览
来源：http://ktu.ybcxt.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kfc.gotoacloud.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xnc.nanxuanxn.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://had.ctjpmb.com

TS:   Number() String() Boolean() x as number
来源：http://xkk.dashuyun.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bsh.9152youxi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cqh.redwolf501.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://qvw.fzhhl.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://aoe.bbcook.cn

================================================================================
来源：http://qkz.yj20258888.top

B. 流程控制
来源：http://jnl.cheryme.top

================================================================================
来源：http://ebz.yj202588.top

[B01] 条件判断 if / else
来源：http://rdd.gogol.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://uej.52xcode.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xji.dashuyun.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rgv.xingfuxueyuan.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://igf.fehbvm.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://zdb.sweek.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jzo.aizwys.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eil.xinyue.icu

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ujh.wangshuangyany.cn

[B02] 多分支 else if / elif
来源：http://cnq.jinqigufen.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yrb.jiagoushi.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wyc.ivvv.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ztv.yuxming.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ivi.yj20258.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sbv.xylfe.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tra.quarkkingdee.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uiq.wangshuangyany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://spc.shuidangran.top

[B03] switch / match / case
来源：http://qsh.jqgufenzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rwa.yuxming.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rgn.pycfn.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://unt.kuanghao11.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fgh.ydzc1.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pzi.shangyingyoupin.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ely.hnqzz.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fbu.zhixingplan.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://taw.jiagoushi.top

[B04] for 计数循环
来源：http://lpi.guowangkeji.top

Py:   for i in range(10): print(i)
来源：http://sjo.xinyue.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rgv.smart0.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hjj.mhx1999.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pdm.jqgfzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ddo.zhiwuduotai.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://acd.yongpay.top

Ruby: 10.times { |i| puts i }
来源：http://bwz.gzhubu.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gez.52xcode.cn

[B05] 遍历数组 / 列表
来源：http://uce.hesvh.cn

Py:   for item in arr: print(item)
来源：http://bue.zhongyouzk.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://aax.ivvv.top

JS:   for (const item of arr) { console.log(item); }
来源：http://gbs.vqdsnc.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nvq.wangshuangyany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xgm.chenlongwang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://apl.fehbvm.com

Ruby: arr.each { |item| puts item }
来源：http://skd.redwolf501.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zfx.zhiwuduotai.top

[B06] 遍历字典 / 对象
来源：http://pdu.aibaodan.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ibc.havefunace.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ety.ywan-chungtsiang.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://txb.birdmap.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fll.bbcook.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://srk.cqqwz.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qvl.yangfankeji.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://aar.hywenlv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pyv.yuxming.cn

[B07] while 循环
来源：http://eox.ppjwa.cn

Py:   while i < 10: i += 1
来源：http://swl.jinqigufen.top

PHP:  while ($i < 10) { $i++; }
来源：http://rnj.ehwqpu.com

JS:   while (i < 10) { i++; }
来源：http://zaq.hesvh.cn

TS:   while (i < 10) { i++; }
来源：http://rka.feifeiyinyue.top

Java: while (i < 10) { i++; }
来源：http://aiu.zhaomingkeji.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wqz.sxryk.cn

Ruby: while i < 10; i += 1; end
来源：http://omr.dashuyun.cn

C#:   while (i < 10) { i++; }
来源：http://vih.sufxvd.cn

[B08] do-while（至少执行一次）
来源：http://irv.zdqjudy.top

Py:   # 无 do-while：用 while True + break
来源：http://oaf.tanke756.top

PHP:  do { $i++; } while ($i < 10);
来源：http://rcs.xylfe.cn

JS:   do { i++; } while (i < 10);
来源：http://lpy.daria6918.cn

TS:   do { i++; } while (i < 10);
来源：http://nma.cashguo.top

Java: do { i++; } while (i < 10);
来源：http://wlv.hnqzz.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bqq.hfpthk.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vzi.smart0.xyz

C#:   do { i++; } while (i < 10);
来源：http://aup.nwbrower.top

[B09] break 与 continue
来源：http://pjg.jinqigfzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vsz.gogol.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uod.meibo888.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jng.hnqzz.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zga.yj20258888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uyf.zhaomingkeji.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xuq.zhixingplan.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tnw.feifeiyinyue.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gzl.xingfuxueyuan.xyz

[B10] 遍历同时拿索引
来源：http://vea.jqgufenzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://clc.nanxinkj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rxb.zhoulong.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ylq.hesvh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ote.chenlongwang.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pce.bbcook.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fij.sysykeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mfu.haohaochexian.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kog.uphjek.com

[B11] 生成数字序列 / 区间
来源：http://vdh.zycfv.cn

Py:   list(range(0, 10, 2))
来源：http://tar.ctjpmb.com

PHP:  range(0, 10, 2);
来源：http://hpj.shuidangran.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tlm.9152youxi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tjy.ctjpmb.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bul.smart0.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://glz.xuetiantiany.cn

Ruby: (0...10).step(2).to_a
来源：http://yjc.fzhhl.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pzz.sjlbkw.cn

[B12] 跳出多层循环
来源：http://tcb.shanyushiyangkeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://fsb.nanxinkj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fuf.wangdashe.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tzp.dashuyun.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ddk.zdbjq.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bgs.vehdjk.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vxr.zycfv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cqi.ywan-chungtsiang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ife.vqdsnc.cn

[B13] 判断是否为数字
来源：http://veh.wangdashe.top

Py:   isinstance(x, (int, float))
来源：http://rez.zhiwuduotai.top

PHP:  is_numeric($x)
来源：http://rsg.hywenlv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nct.jinyuanbaomall.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kpk.jianghu66.top

Java: x instanceof Number
来源：http://cjp.jinghuilouyu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dwi.hcnkem.com

Ruby: x.is_a?(Numeric)
来源：http://fnd.havefunace.top

C#:   x is int or double or decimal
来源：http://sdf.nanxuanxn.top

[B14] 判断值是否在集合内
来源：http://xvf.smart0.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wpc.jqgfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jwc.hcnkem.com

JS:   [1, 2, 3].includes(x)
来源：http://csp.daxiang520.top

TS:   [1, 2, 3].includes(x)
来源：http://rrg.jqgufenzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://osd.daria6918.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qwu.epnwcf.com

Ruby: [1, 2, 3].include?(x)
来源：http://gca.zhixingplan.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iaw.aibaodan.cn

[B15] 布尔运算与取反
来源：http://anm.gogol.net.cn

Py:   a and b or not c
来源：http://zgh.jinghuilouyu.cn

PHP:  $a && $b || !$c
来源：http://rkp.ppjwa.cn

JS:   a && b || !c
来源：http://rti.kuanghao11.cn

TS:   a && b || !c
来源：http://agr.9152youxi.cn

Java: a && b || !c
来源：http://ewp.aizwys.cn

Go:   a && b || !c
来源：http://doq.zhaomingkeji.xyz

Ruby: a && b || !c
来源：http://bzu.svipenyu.cn

C#:   a && b || !c
来源：http://fos.fengsongda.top

[B16] 卫语句：不满足条件提前返回
来源：http://imt.yvedp.cn

Py:   if not data: return
来源：http://xpl.shanyushiyangkeji.top

PHP:  if (!$data) { return; }
来源：http://zyf.yuxming.cn

JS:   if (!data) return;
来源：http://jjc.epnwcf.com

TS:   if (!data) return;
来源：http://nzx.jyoumei.cn

Java: if (data == null) return;
来源：http://cpo.jqgufenzy.top

Go:   if data == nil { return }
来源：http://shz.haohaochexian.top

Ruby: return if data.nil?
来源：http://lkt.chenjidiqi.icu

C#:   if (data == null) return;
来源：http://xgk.yonumen.top

================================================================================
来源：http://wfw.ctjpmb.com

C. 函数与作用域
来源：http://iae.smart0.xyz

================================================================================
来源：http://nvo.ivvv.top

[C01] 定义函数
来源：http://wjk.ywan-chungtsiang.top

Py:   def add(a, b): return a + b
来源：http://lkm.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cxe.cucudq.cn

JS:   function add(a, b) { return a + b; }
来源：http://fdb.uphjek.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eem.cucudq.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mmc.sysykeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://wph.fehbvm.com

Ruby: def add(a, b); a + b; end
来源：http://paz.cucudq.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vqs.hnqzz.top

[C02] 默认参数
来源：http://iih.sjlbkw.cn

Py:   def greet(name="World"): return name
来源：http://svs.jinqigfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qkz.aizwys.cn

JS:   function greet(name = "World") { return name; }
来源：http://zkb.xuetiantiany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hna.sjlbkw.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qaf.sysykeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ekb.jianghu66.top

Ruby: def greet(name = "World") = name
来源：http://zly.ppjwa.cn

C#:   string Greet(string name = "World") => name;
来源：http://xnv.iojbl.cn

[C03] 可变参数
来源：http://rkm.9152youxi.cn

Py:   def total(*args): return sum(args)
来源：http://bcy.dashuyun.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rxv.shuidangran.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nnh.tianlin.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://krk.jyoumei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ghp.hesvh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xzj.hnqzz.top

Ruby: def total(*nums); nums.sum; end
来源：http://qbn.gogol.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eya.cdnleiting.top

[C04] 命名参数 / 关键字参数
来源：http://jhf.shangyingyoupin.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dqw.aizwys.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zbo.0kj1m.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hly.gogol.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jmh.aizwys.cn

Java: // 无：用 Builder 模式或 record
来源：http://czy.yonumen.top

Go:   // 无：用配置结构体参数
来源：http://hii.iojbl.cn

Ruby: f(a: 1, b: 2)
来源：http://xww.ywan-chungtsiang.top

C#:   f(a: 1, b: 2)
来源：http://whk.hcnkem.com

[C05] 返回多个值
来源：http://pho.mhx1999.top

Py:   return a, b
来源：http://rir.feifeiyinyue.top

PHP:  return [$a, $b];
来源：http://btq.jlsjyb.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dtv.aibaodan.cn

TS:   return { a, b };
来源：http://hcs.fzhhl.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nxn.havefunace.top

Go:   return a, b
来源：http://cbi.gaohongyu789.top

Ruby: return a, b
来源：http://fdw.jlsjyb.cn

C#:   return (a, b);              // ValueTuple
来源：http://tsz.mhx1999.top

[C06] 匿名函数 / lambda
来源：http://vgc.hesvh.cn

Py:   square = lambda x: x * x
来源：http://zef.sweek.top

PHP:  $square = fn($x) => $x * $x;
来源：http://pcu.fktsv.cn

JS:   const square = x => x * x;
来源：http://vmc.jlsjyb.cn

TS:   const square = (x: number): number => x * x;
来源：http://eda.guowangkeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qup.kuanghao11.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hmh.guannengcc.top

Ruby: square = ->(x) { x * x }
来源：http://rzh.daxiang520.top

C#:   Func<int, int> square = x => x * x;
来源：http://rnn.fehbvm.com

[C07] 把函数作为参数传入
来源：http://sqd.hongshengwenyu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mhq.cashguo.top

PHP:  array_map("strtoupper", $arr);
来源：http://dxl.hcnkem.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gjk.bbcook.cn

TS:   arr.map(String)
来源：http://zud.gogol.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vky.chenlongwang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nns.cashguo.top

Ruby: arr.map(&:upcase)
来源：http://kzy.fanxiaobao.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://tdd.ydzc1.top

[C08] 闭包
来源：http://siq.316326.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cty.yj202588.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uvh.zdqjudy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cqc.yfazqb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fha.yvedp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://abu.zhaomingkeji.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yyq.chenzaomai.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gbf.birdmap.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wxw.zhengqikj.top

[C09] 递归
来源：http://ina.daxiang520.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mki.jqgufenzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://flu.fehbvm.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mcv.vehdjk.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ikq.hfpthk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ucl.pengpengdd.cyou

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kik.aizwys.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fvi.nanxuanxn.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xqz.hammf.cn

[C10] 变量作用域
来源：http://ycb.zhiwuduotai.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://aqx.yanxiufei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mez.vehdjk.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://otq.nanxuanxn.top

TS:   同 JS
来源：http://voz.aizwys.cn

Java: 方法内为块级作用域
来源：http://xan.uphjek.com

Go:   花括号块级作用域
来源：http://wer.feifeiyinyue.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nem.hesvh.cn

C#:   块级作用域
来源：http://tgu.jinghuilouyu.cn

[C11] 模块导入与导出
来源：http://dbl.haohaochexian.top

Py:   from module import func
来源：http://pef.sufxvd.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zzp.zdbjq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://uqj.epnwcf.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hhc.smart0.xyz

Java: import java.util.List;
来源：http://blm.cucudq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rtg.52xcode.cn

Ruby: require "json"; require_relative "./util"
来源：http://xrm.hcnkem.com

C#:   using System.Text;
来源：http://mem.yj202588.top

[C12] 立即执行函数 IIFE
来源：http://zsp.ehwqpu.com

Py:   (lambda: print("run"))()
来源：http://pir.nwbrower.top

PHP:  (function () { echo "run"; })();
来源：http://sza.ydjk.org.cn

JS:   (() => { console.log("run"); })();
来源：http://wan.9152youxi.cn

TS:   (() => { console.log("run"); })();
来源：http://soq.gzhubu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zav.jlsjyb.cn

Go:   func() { fmt.Println("run") }()
来源：http://dzw.tarul.cn

Ruby: -> { puts "run" }.call
来源：http://vib.daxiang520.top

C#:   // 无 IIFE：用静态构造函数
来源：http://tmi.guowangkeji.top

[C13] 类型声明 / 类型注解
来源：http://kqy.ydzc1.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uzk.pengpengdd.cyou

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yhg.cdnleiting.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wqe.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gfo.nwbrower.top

Java: int add(int a, int b) { return a + b; }
来源：http://qpn.gogol.net.cn

Go:   func add(a, b int) int
来源：http://fpi.fengsongda.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://opl.nwbrower.top

C#:   int Add(int a, int b) => a + b;
来源：http://nul.chenzaomai.com

[C14] 泛型函数
来源：http://bml.shanyushiyangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zds.nanxuanxn.top

PHP:  // 无泛型
来源：http://fhv.quarkkingdee.top

JS:   // 无泛型
来源：http://xov.yj202588.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mbw.ydjk.org.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://voy.jinghuilouyu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ovx.chenjidiqi.icu

Ruby: # 无泛型
来源：http://gdj.sxryk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xve.yj202588.top

[C15] 解构 / 展开参数
来源：http://tcv.shuidangran.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://iqy.jinqigfzy.top

PHP:  [$a, $b] = $pair;
来源：http://fje.fktsv.cn


<!-- 参考信息 -->