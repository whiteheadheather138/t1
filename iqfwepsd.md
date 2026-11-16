代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://eeg.gaohongyu789.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://igs.hammf.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lfa.jinqigufen.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vzg.yanxiufei.cn

Go:   strings.TrimSpace(s)
来源：http://fdb.hammf.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kyg.sweek.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zvg.pycfn.com

[A25] 字符串比较
来源：http://sgk.havefunace.top

Py:   s1 == s2; s1 != s2
来源：http://arl.bbcook.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sxw.ehwqpu.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jml.yuxming.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ifo.meibo888.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://toj.hcnkem.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kjh.zycfv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lbo.ydjk.org.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kjs.shuidangran.top

[A26] 类型转换总览
来源：http://hww.ivvv.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yru.pengpengdd.cyou

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pff.mhx1999.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ceh.daria6918.cn

TS:   Number() String() Boolean() x as number
来源：http://tyh.hesvh.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ixh.zdqjudy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uci.ydzc1.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://jqp.jlsjyb.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ole.jinghuilouyu.cn

================================================================================
来源：http://waz.jinyuanbaomall.cn

B. 流程控制
来源：http://azn.hongshengwenyu.top

================================================================================
来源：http://eiu.dashuyun.cn

[B01] 条件判断 if / else
来源：http://mwb.0kj1m.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vtl.yj20258888.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://teu.hongshengwenyu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://akx.hnxiangtu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://eio.zhijiandao.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mzg.ehwqpu.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://egk.haohaochexian.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dia.zhixingplan.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qiz.dashuyun.cn

[B02] 多分支 else if / elif
来源：http://ovf.jinqigfzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fal.zhixingplan.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://brx.yangfankeji.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rva.ppjwa.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wuc.yueranfly.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://noq.havefunace.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://scg.hywenlv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ykp.bbcook.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://prv.feifeiyinyue.top

[B03] switch / match / case
来源：http://ryx.havefunace.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nib.yj20258888.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ahf.wangdashe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vvj.xziqi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bkl.redwolf501.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rpa.jinqigfzy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zay.zhoulong.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://eax.smart0.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kyx.andypj.xyz

[B04] for 计数循环
来源：http://lnp.zhaomingkeji.xyz

Py:   for i in range(10): print(i)
来源：http://jxq.ppjwa.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zzj.zycfv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xxm.ivvv.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kzd.cashguo.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xnc.yonumen.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qll.52xcode.cn

Ruby: 10.times { |i| puts i }
来源：http://gkd.smart0.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mtf.ywan-chungtsiang.top

[B05] 遍历数组 / 列表
来源：http://xap.cucudq.cn

Py:   for item in arr: print(item)
来源：http://bry.hcnkem.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://duk.meibo888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://aez.yonumen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tdk.9152youxi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gvf.dianchejie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://brc.tianlin.xyz

Ruby: arr.each { |item| puts item }
来源：http://uyo.iojbl.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qqy.fengsongda.top

[B06] 遍历字典 / 对象
来源：http://hrt.nwbrower.top

Py:   for k, v in d.items(): print(k, v)
来源：http://lit.gogol.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hyb.jyoumei.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ptl.shuidangran.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yxp.zhaomingkeji.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bqw.kuanghao11.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://goy.tanke756.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qag.cqqwz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xiy.jinqigfzy.top

[B07] while 循环
来源：http://ueg.smart0.xyz

Py:   while i < 10: i += 1
来源：http://spr.ydjk.org.cn

PHP:  while ($i < 10) { $i++; }
来源：http://iko.wangdashe.top

JS:   while (i < 10) { i++; }
来源：http://suy.smart0.xyz

TS:   while (i < 10) { i++; }
来源：http://gwk.hesvh.cn

Java: while (i < 10) { i++; }
来源：http://awb.jianghu66.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wdw.guowangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://git.xylfe.cn

C#:   while (i < 10) { i++; }
来源：http://qqq.kuanghao11.cn

[B08] do-while（至少执行一次）
来源：http://abt.sjlbkw.cn

Py:   # 无 do-while：用 while True + break
来源：http://xru.zhaomingkeji.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://nlt.pengpengdd.cyou

JS:   do { i++; } while (i < 10);
来源：http://gfi.jqgfzy.top

TS:   do { i++; } while (i < 10);
来源：http://mwm.zhixingplan.top

Java: do { i++; } while (i < 10);
来源：http://lxt.andypj.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://ybn.nanxuanxn.top

Ruby: begin; i += 1; end while i < 10
来源：http://bgu.jiagoushi.top

C#:   do { i++; } while (i < 10);
来源：http://frv.hcnkem.com

[B09] break 与 continue
来源：http://amk.yfazqb.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bim.kuanghao11.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bcu.jqgfzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hbw.shzxlz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sif.hnqzz.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tzb.0kj1m.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zyy.316326.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pti.ydzc1.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://thi.fehbvm.com

[B10] 遍历同时拿索引
来源：http://owh.yongpay.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kcw.fengsongda.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dyj.zhixingplan.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://epg.xuetiantiany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://aob.jinyuanbaomall.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cpv.pengpengdd.cyou

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ozq.ydzc1.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zel.cqqwz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hgj.dianchejie.cn

[B11] 生成数字序列 / 区间
来源：http://qav.ybcxt.top

Py:   list(range(0, 10, 2))
来源：http://ltt.52xcode.cn

PHP:  range(0, 10, 2);
来源：http://yfh.0kj1m.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://agt.sweek.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yfj.c1oappe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nzd.zdqjudy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ett.aibaodan.cn

Ruby: (0...10).step(2).to_a
来源：http://pwr.ivvv.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tna.shzxlz.cn

[B12] 跳出多层循环
来源：http://dbw.sweek.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://viz.epnwcf.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://zlj.jqgufenzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ups.yj20258.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rrf.zhaomingkeji.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bdo.fanxiaobao.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rpk.guowangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wco.gotoacloud.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bdt.bbcook.cn

[B13] 判断是否为数字
来源：http://grb.nanxuanxn.top

Py:   isinstance(x, (int, float))
来源：http://hpm.gogol.net.cn

PHP:  is_numeric($x)
来源：http://qfq.zdqjudy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qky.fanxiaobao.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lvd.tanke756.top

Java: x instanceof Number
来源：http://obm.hywenlv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ecp.xziqi.cn

Ruby: x.is_a?(Numeric)
来源：http://khy.yuanzhike.top

C#:   x is int or double or decimal
来源：http://nrd.ppjwa.cn

[B14] 判断值是否在集合内
来源：http://uoo.yongpay.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mob.cqqwz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fhv.ywan-chungtsiang.top

JS:   [1, 2, 3].includes(x)
来源：http://pqx.gzhubu.top

TS:   [1, 2, 3].includes(x)
来源：http://bjx.zhengqikj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ilq.guannengcc.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yrd.sweek.top

Ruby: [1, 2, 3].include?(x)
来源：http://ydh.wangshuangyany.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://orw.jiagoushi.top

[B15] 布尔运算与取反
来源：http://tmy.gzhubu.top

Py:   a and b or not c
来源：http://oid.tanke756.top

PHP:  $a && $b || !$c
来源：http://ads.snrcjt.cn

JS:   a && b || !c
来源：http://xkr.ivvv.top

TS:   a && b || !c
来源：http://ehe.xingfuxueyuan.xyz

Java: a && b || !c
来源：http://bay.ctjpmb.com

Go:   a && b || !c
来源：http://lml.bbcook.cn

Ruby: a && b || !c
来源：http://mwc.0kj1m.cn

C#:   a && b || !c
来源：http://swo.andypj.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://axp.jinqigufen.top

Py:   if not data: return
来源：http://mxy.ehwqpu.com

PHP:  if (!$data) { return; }
来源：http://cwt.xuetiantiany.cn

JS:   if (!data) return;
来源：http://wdc.hnqzz.top

TS:   if (!data) return;
来源：http://ail.haohaochexian.top

Java: if (data == null) return;
来源：http://udq.pengpengdd.cyou

Go:   if data == nil { return }
来源：http://hen.tarul.cn

Ruby: return if data.nil?
来源：http://qgy.yj202588.top

C#:   if (data == null) return;
来源：http://vcn.jianghu66.top

================================================================================
来源：http://vwh.yvedp.cn

C. 函数与作用域
来源：http://jkn.gaohongyu789.top

================================================================================
来源：http://tef.jqgufenzy.top

[C01] 定义函数
来源：http://stj.zhaomingkeji.xyz

Py:   def add(a, b): return a + b
来源：http://wzb.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cyn.zhoulong.xyz

JS:   function add(a, b) { return a + b; }
来源：http://pmx.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hzk.yonumen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://bar.haohaochexian.top

Go:   func add(a, b int) int { return a + b }
来源：http://aju.yanxiufei.cn

Ruby: def add(a, b); a + b; end
来源：http://bbv.9152youxi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dqo.sysykeji.top

[C02] 默认参数
来源：http://snw.shuidangran.top

Py:   def greet(name="World"): return name
来源：http://erv.guowangkeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://pxp.pengpengdd.cyou

JS:   function greet(name = "World") { return name; }
来源：http://lkv.52xcode.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fzc.aizwys.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mmu.zdbjq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://asp.haohaochexian.top

Ruby: def greet(name = "World") = name
来源：http://str.pycfn.com

C#:   string Greet(string name = "World") => name;
来源：http://lca.ydjk.org.cn

[C03] 可变参数
来源：http://kcx.jqgfzy.top

Py:   def total(*args): return sum(args)
来源：http://tmv.jinqigfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qlk.iojbl.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bcx.sysykeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eio.jqgufenzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qzu.haohaochexian.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://duu.haohaochexian.top

Ruby: def total(*nums); nums.sum; end
来源：http://ojx.ydjk.org.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://crd.9152youxi.cn

[C04] 命名参数 / 关键字参数
来源：http://eah.yongpay.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wfe.dianchejie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nck.cashguo.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oew.tarul.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gxp.yuxming.cn

Java: // 无：用 Builder 模式或 record
来源：http://pag.sxryk.cn

Go:   // 无：用配置结构体参数
来源：http://vsq.ehwqpu.com

Ruby: f(a: 1, b: 2)
来源：http://lwo.zhixingplan.top

C#:   f(a: 1, b: 2)
来源：http://sax.cdnleiting.top

[C05] 返回多个值
来源：http://pos.meibo888.top

Py:   return a, b
来源：http://fml.jianghu66.top

PHP:  return [$a, $b];
来源：http://mzx.yuanzhike.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://uvz.yj20258888.top

TS:   return { a, b };
来源：http://ggx.pengpengdd.cyou

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uyf.quarkkingdee.top

Go:   return a, b
来源：http://yaw.yfazqb.com

Ruby: return a, b
来源：http://aog.guowangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://hkg.kuanghao11.cn

[C06] 匿名函数 / lambda
来源：http://wbo.zhixingplan.top

Py:   square = lambda x: x * x
来源：http://dch.smart0.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://byp.ivvv.top

JS:   const square = x => x * x;
来源：http://ena.sysykeji.top

TS:   const square = (x: number): number => x * x;
来源：http://xjj.wangshuangyany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fas.shzxlz.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zyu.sufxvd.cn

Ruby: square = ->(x) { x * x }
来源：http://ftm.jinqigfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://byh.yj202588.top

[C07] 把函数作为参数传入
来源：http://xzn.sysykeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://owj.aizwys.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vfp.vqdsnc.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://omx.cdnleiting.top

TS:   arr.map(String)
来源：http://nmh.jianghu66.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zfj.daria6918.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pbg.chenzaomai.com

Ruby: arr.map(&:upcase)
来源：http://wus.vqdsnc.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hbf.yj202588.top

[C08] 闭包
来源：http://zjx.ydjk.org.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mjr.fzhhl.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://met.jlsjyb.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nya.yvedp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qur.bbcook.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hsn.mhx1999.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ail.nanxuanxn.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://aax.ctjpmb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sya.sweek.top

[C09] 递归
来源：http://mmh.meibo888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://plx.shangyingyoupin.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tyo.gotoacloud.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vsl.yanxiufei.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uru.fehbvm.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://scq.shangyingyoupin.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hnv.zhongyouzk.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://smp.cqqwz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yli.9152youxi.cn

[C10] 变量作用域
来源：http://evw.ybcxt.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ldt.jinghuilouyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kqd.nanxuanxn.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nqd.chenjidiqi.icu

TS:   同 JS
来源：http://tqd.zhixingplan.top

Java: 方法内为块级作用域
来源：http://wdx.316326.xyz

Go:   花括号块级作用域
来源：http://ude.kuanghao11.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://smy.gaohongyu789.top

C#:   块级作用域
来源：http://qpp.redwolf501.top

[C11] 模块导入与导出
来源：http://crd.svipenyu.cn

Py:   from module import func
来源：http://igu.svipenyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bnw.xingfuxueyuan.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://drw.yuxming.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vsn.ydjk.org.cn

Java: import java.util.List;
来源：http://dbg.fanxiaobao.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://niw.ppjwa.cn

Ruby: require "json"; require_relative "./util"
来源：http://sea.zhaomingkeji.xyz

C#:   using System.Text;
来源：http://ovz.gaohongyu789.top

[C12] 立即执行函数 IIFE
来源：http://cqs.guowangkeji.top

Py:   (lambda: print("run"))()
来源：http://lea.yj20258888.top

PHP:  (function () { echo "run"; })();
来源：http://xxs.xingfuxueyuan.xyz

JS:   (() => { console.log("run"); })();
来源：http://wmt.xuanzx.com

TS:   (() => { console.log("run"); })();
来源：http://kxb.ydzc1.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mvx.shzxlz.cn

Go:   func() { fmt.Println("run") }()
来源：http://ghh.epnwcf.com

Ruby: -> { puts "run" }.call
来源：http://uub.chenlongwang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://hui.sysykeji.top

[C13] 类型声明 / 类型注解
来源：http://zfr.shzxlz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wkk.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wvo.tian-w.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hyw.tarul.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mbw.yongpay.top

Java: int add(int a, int b) { return a + b; }
来源：http://yzg.ctjpmb.com

Go:   func add(a, b int) int
来源：http://llg.jyoumei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nzt.wangshuangyany.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vbx.yvedp.cn

[C14] 泛型函数
来源：http://cbb.yj20258888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://znf.hnxiangtu.top

PHP:  // 无泛型
来源：http://grj.jyoumei.cn

JS:   // 无泛型
来源：http://fvw.xziqi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cfc.jlsjyb.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qtw.andypj.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fjv.sjlbkw.cn

Ruby: # 无泛型
来源：http://hyx.yj202588.top


<!-- 参考信息 -->