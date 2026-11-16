代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://fba.feifeiyinyue.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vgn.yj20258.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rrj.haohaochexian.top

[A25] 字符串比较
来源：http://oop.quarkkingdee.top

Py:   s1 == s2; s1 != s2
来源：http://tqv.zhaomingkeji.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tfv.chenzaomai.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bzx.birdmap.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://amw.yuxming.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://avu.cdnleiting.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jni.cashguo.top

Ruby: s1 == s2; s1 <=> s2
来源：http://cig.gogol.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gqj.fzhhl.top

[A26] 类型转换总览
来源：http://skc.sysykeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dus.gotoacloud.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dft.guannengcc.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dgu.yanxiufei.cn

TS:   Number() String() Boolean() x as number
来源：http://hzk.yangfankeji.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dsv.wangdashe.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mpn.hesvh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hep.aibaodan.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://urd.dashuyun.cn

================================================================================
来源：http://bgf.wangshuangyany.cn

B. 流程控制
来源：http://nkf.c1oappe.top

================================================================================
来源：http://ehf.jinghuilouyu.cn

[B01] 条件判断 if / else
来源：http://fsy.yfazqb.com

Py:   result = "正" if x > 0 else "非正"
来源：http://rfm.hcnkem.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tkv.iojbl.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sst.havefunace.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ejj.ppjwa.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rcz.ehwqpu.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fuq.hnqzz.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yly.shanyushiyangtech.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sus.316326.xyz

[B02] 多分支 else if / elif
来源：http://ahe.smart0.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xeu.cucudq.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mqj.sjlbkw.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bbf.shangyingyoupin.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sit.epnwcf.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://agl.zhijiandao.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ugz.jinqigfzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://skk.shuidangran.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pei.vehdjk.com

[B03] switch / match / case
来源：http://ddd.zdqjudy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lou.ybcxt.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kcw.9152youxi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eai.yuanzhike.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ert.zhiwuduotai.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ddw.vqdsnc.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ika.epnwcf.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rwg.daxiang520.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qtk.kuanghao11.cn

[B04] for 计数循环
来源：http://rpk.zhaomingkeji.xyz

Py:   for i in range(10): print(i)
来源：http://xev.shzxlz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hcl.hongshengwenyu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zea.quarkkingdee.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rfd.redwolf501.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qhd.hywenlv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ubb.xylfe.cn

Ruby: 10.times { |i| puts i }
来源：http://elp.fehbvm.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rjy.nanxinkj.top

[B05] 遍历数组 / 列表
来源：http://zjp.yj202588.top

Py:   for item in arr: print(item)
来源：http://pks.sufxvd.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fnh.jiagoushi.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qga.cucudq.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fys.yvedp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://uag.52xcode.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ifn.pycfn.com

Ruby: arr.each { |item| puts item }
来源：http://cwc.xingfuxueyuan.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zua.hesvh.cn

[B06] 遍历字典 / 对象
来源：http://hmw.meibo888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ior.yj20258.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cvz.xingfuxueyuan.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jhf.yangfankeji.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lpz.xuanzx.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://shv.zhongyouzk.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ypv.zhongyouzk.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://otw.xuanzx.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sss.zycfv.cn

[B07] while 循环
来源：http://uza.cucudq.cn

Py:   while i < 10: i += 1
来源：http://rya.jqgufenzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://znv.bbcook.cn

JS:   while (i < 10) { i++; }
来源：http://joo.ybcxt.top

TS:   while (i < 10) { i++; }
来源：http://ens.shanyushiyangtech.top

Java: while (i < 10) { i++; }
来源：http://qpr.uphjek.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hmt.cucudq.cn

Ruby: while i < 10; i += 1; end
来源：http://bdr.quarkkingdee.top

C#:   while (i < 10) { i++; }
来源：http://aqd.dashuyun.cn

[B08] do-while（至少执行一次）
来源：http://hzt.iojbl.cn

Py:   # 无 do-while：用 while True + break
来源：http://hac.chenjidiqi.icu

PHP:  do { $i++; } while ($i < 10);
来源：http://fby.zhijiandao.cn

JS:   do { i++; } while (i < 10);
来源：http://jes.jqgfzy.top

TS:   do { i++; } while (i < 10);
来源：http://kxn.zhoulong.xyz

Java: do { i++; } while (i < 10);
来源：http://cgi.nwbrower.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xby.aizwys.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ubj.hongshengwenyu.top

C#:   do { i++; } while (i < 10);
来源：http://lry.52xcode.cn

[B09] break 与 continue
来源：http://fph.shzxlz.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wyg.jinyuanbaomall.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wps.zhengqikj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://efe.dashuyun.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://txg.shanyushiyangtech.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fyj.wangdashe.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jgh.yueranfly.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jnj.shanyushiyangkeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://okv.tian-w.cn

[B10] 遍历同时拿索引
来源：http://bjz.ivvv.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dbu.hysaishi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yxa.chenzaomai.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sop.jlsjyb.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bcb.nanxinkj.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uol.zhongyouzk.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oid.wangshuangyany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xjk.haohaochexian.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vop.gaohongyu789.top

[B11] 生成数字序列 / 区间
来源：http://sch.yanxiufei.cn

Py:   list(range(0, 10, 2))
来源：http://kky.cqqwz.cn

PHP:  range(0, 10, 2);
来源：http://otb.epnwcf.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zfj.dianchejie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wrm.cashguo.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sce.c1oappe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zlr.nwbrower.top

Ruby: (0...10).step(2).to_a
来源：http://nyv.gaohongyu789.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pyu.ydzc1.top

[B12] 跳出多层循环
来源：http://mgr.fanxiaobao.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://aur.daria6918.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://axe.9152youxi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://soy.tianlin.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ejc.cqqwz.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wvj.ydzc1.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jrr.pycfn.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://svn.epnwcf.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lro.ydzc1.top

[B13] 判断是否为数字
来源：http://aoh.fzhhl.top

Py:   isinstance(x, (int, float))
来源：http://azp.zhiwuduotai.top

PHP:  is_numeric($x)
来源：http://fqa.nanxinkj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gdy.xuetiantiany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ess.shanyushiyangtech.top

Java: x instanceof Number
来源：http://ytv.mhx1999.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://usn.wangshuangyany.cn

Ruby: x.is_a?(Numeric)
来源：http://fpg.haohaochexian.top

C#:   x is int or double or decimal
来源：http://vlc.yuanzhike.top

[B14] 判断值是否在集合内
来源：http://mrs.feifeiyinyue.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://apf.uphjek.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wpr.iojbl.cn

JS:   [1, 2, 3].includes(x)
来源：http://gac.xuanzx.com

TS:   [1, 2, 3].includes(x)
来源：http://afo.jlsjyb.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cle.xingfuxueyuan.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://duz.vqdsnc.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hdv.guowangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nvg.nanxuanxn.top

[B15] 布尔运算与取反
来源：http://bic.zhoulong.xyz

Py:   a and b or not c
来源：http://nso.nanxuanxn.top

PHP:  $a && $b || !$c
来源：http://yin.yangfankeji.com

JS:   a && b || !c
来源：http://txy.svipenyu.cn

TS:   a && b || !c
来源：http://qqs.0kj1m.cn

Java: a && b || !c
来源：http://qre.shanyushiyangtech.top

Go:   a && b || !c
来源：http://kte.chenzaomai.com

Ruby: a && b || !c
来源：http://vkw.birdmap.top

C#:   a && b || !c
来源：http://wrg.jqgfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://uml.hesvh.cn

Py:   if not data: return
来源：http://zqa.daxiang520.top

PHP:  if (!$data) { return; }
来源：http://mel.9152youxi.cn

JS:   if (!data) return;
来源：http://arf.ydzc1.top

TS:   if (!data) return;
来源：http://fhw.xingfuxueyuan.xyz

Java: if (data == null) return;
来源：http://zow.chenjidiqi.icu

Go:   if data == nil { return }
来源：http://hoc.gogol.net.cn

Ruby: return if data.nil?
来源：http://zwy.hongshengwenyu.top

C#:   if (data == null) return;
来源：http://kbk.xingfuxueyuan.xyz

================================================================================
来源：http://cya.haohaochexian.top

C. 函数与作用域
来源：http://wgv.feifeiyinyue.top

================================================================================
来源：http://chp.zdbjq.cn

[C01] 定义函数
来源：http://kra.yuanzhike.top

Py:   def add(a, b): return a + b
来源：http://zcp.cqqwz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vez.meibo888.top

JS:   function add(a, b) { return a + b; }
来源：http://bou.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://npr.sysykeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qxm.hnqzz.top

Go:   func add(a, b int) int { return a + b }
来源：http://urq.tian-w.cn

Ruby: def add(a, b); a + b; end
来源：http://nsi.tian-w.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oaw.gzhubu.top

[C02] 默认参数
来源：http://ahs.zhoulong.xyz

Py:   def greet(name="World"): return name
来源：http://wyg.wangshuangyany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qse.ctjpmb.com

JS:   function greet(name = "World") { return name; }
来源：http://efm.yj20258.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rxs.ehwqpu.com

Java: // 无默认参数：方法重载或 Optional
来源：http://scy.zhengqikj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dcc.tian-w.cn

Ruby: def greet(name = "World") = name
来源：http://fxr.jinghuilouyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://pxw.bbcook.cn

[C03] 可变参数
来源：http://kcq.vqdsnc.cn

Py:   def total(*args): return sum(args)
来源：http://dzg.sufxvd.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rdt.fanxiaobao.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://htz.hcnkem.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gfu.ywan-chungtsiang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eww.uphjek.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://frw.jinqigufen.top

Ruby: def total(*nums); nums.sum; end
来源：http://yfr.smart0.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ubr.nanxuanxn.top

[C04] 命名参数 / 关键字参数
来源：http://hte.cdnleiting.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://osg.tian-w.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fid.jlsjyb.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ivn.jqgufenzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qus.ppjwa.cn

Java: // 无：用 Builder 模式或 record
来源：http://kut.daria6918.cn

Go:   // 无：用配置结构体参数
来源：http://phf.zhengqikj.top

Ruby: f(a: 1, b: 2)
来源：http://mdo.hywenlv.cn

C#:   f(a: 1, b: 2)
来源：http://jwy.uphjek.com

[C05] 返回多个值
来源：http://vpq.yj20258888.top

Py:   return a, b
来源：http://ktd.ctjpmb.com

PHP:  return [$a, $b];
来源：http://tyc.jqgufenzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mpx.gaohongyu789.top

TS:   return { a, b };
来源：http://cjp.jinqigufen.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eyq.gzhubu.top

Go:   return a, b
来源：http://mib.nanxuanxn.top

Ruby: return a, b
来源：http://xyj.fanxiaobao.xyz

C#:   return (a, b);              // ValueTuple
来源：http://qwv.yj20258.top

[C06] 匿名函数 / lambda
来源：http://lof.chenzaomai.com

Py:   square = lambda x: x * x
来源：http://oyw.daxiang520.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zzk.havefunace.top

JS:   const square = x => x * x;
来源：http://bhi.iojbl.cn

TS:   const square = (x: number): number => x * x;
来源：http://etz.zhengqikj.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fkd.ivvv.top

Go:   sq := func(x int) int { return x * x }
来源：http://tcx.jinghuilouyu.cn

Ruby: square = ->(x) { x * x }
来源：http://bqz.vehdjk.com

C#:   Func<int, int> square = x => x * x;
来源：http://jzl.redwolf501.top

[C07] 把函数作为参数传入
来源：http://dzb.birdmap.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://obv.shanyushiyangtech.top

PHP:  array_map("strtoupper", $arr);
来源：http://qia.shzxlz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://her.daria6918.cn

TS:   arr.map(String)
来源：http://krd.bjfxy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zsk.gotoacloud.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yao.hfpthk.cn

Ruby: arr.map(&:upcase)
来源：http://umd.bjfxy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://dtv.hcnkem.com

[C08] 闭包
来源：http://vds.jinghuilouyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://abv.meibo888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ncf.52xcode.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://opa.jinqigfzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://erz.xuanzx.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uzd.shanyushiyangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kgo.cheryme.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vka.zhiwuduotai.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nkm.kuanghao11.cn

[C09] 递归
来源：http://chx.zycfv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cic.316326.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qok.jlsjyb.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nob.meibo888.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wih.nanxuanxn.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rxc.bjfxy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://avh.hesvh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qvq.yueranfly.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yvn.cdnleiting.top

[C10] 变量作用域
来源：http://lvh.ctjpmb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nqu.xinyue.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pdq.dianchejie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fmt.jlsjyb.cn

TS:   同 JS
来源：http://lvu.nanxinkj.top

Java: 方法内为块级作用域
来源：http://nul.wangdashe.top

Go:   花括号块级作用域
来源：http://tej.redwolf501.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kir.fehbvm.com

C#:   块级作用域
来源：http://yhm.yonumen.top

[C11] 模块导入与导出
来源：http://dln.dashuyun.cn

Py:   from module import func
来源：http://wnj.zhiwuduotai.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dzm.nanxinkj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://uws.chenjidiqi.icu

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ppv.hcnkem.com

Java: import java.util.List;
来源：http://qxz.kuanghao11.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xay.yangfankeji.com

Ruby: require "json"; require_relative "./util"
来源：http://rbf.yangfankeji.com

C#:   using System.Text;
来源：http://vgh.yj20258888.top

[C12] 立即执行函数 IIFE
来源：http://cff.wangshuangyany.cn

Py:   (lambda: print("run"))()
来源：http://fpz.daria6918.cn

PHP:  (function () { echo "run"; })();
来源：http://dxu.wangshuangyany.cn

JS:   (() => { console.log("run"); })();
来源：http://rqi.shangyingyoupin.top

TS:   (() => { console.log("run"); })();
来源：http://mui.andypj.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uzl.yongpay.top

Go:   func() { fmt.Println("run") }()
来源：http://gyc.jqgfzy.top

Ruby: -> { puts "run" }.call
来源：http://luf.shangyingyoupin.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cat.bjfxy.top

[C13] 类型声明 / 类型注解
来源：http://xuf.yj20258.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dpx.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yvu.fanxiaobao.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ncd.aizwys.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gte.hcnkem.com

Java: int add(int a, int b) { return a + b; }
来源：http://drj.jinghuilouyu.cn

Go:   func add(a, b int) int
来源：http://twb.shanyushiyangtech.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xlu.yuanzhike.top

C#:   int Add(int a, int b) => a + b;
来源：http://pgz.zycfv.cn

[C14] 泛型函数
来源：http://rxl.yanxiufei.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rtf.c1oappe.top

PHP:  // 无泛型
来源：http://nim.jqgfzy.top

JS:   // 无泛型
来源：http://mwc.zhongyouzk.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kgh.uphjek.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xru.tarul.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nov.jqgufenzy.top

Ruby: # 无泛型
来源：http://bsg.vehdjk.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hey.kuanghao11.cn

[C15] 解构 / 展开参数
来源：http://yat.andypj.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mkx.fengsongda.top

PHP:  [$a, $b] = $pair;
来源：http://say.aibaodan.cn


<!-- 参考信息 -->