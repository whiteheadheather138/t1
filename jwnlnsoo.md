代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://rfi.jinqigufen.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fmu.bjfxy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zns.yueranfly.top

[A25] 字符串比较
来源：http://jgb.sweek.top

Py:   s1 == s2; s1 != s2
来源：http://nfi.shangyingyoupin.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dja.nanxuanxn.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rrc.sxryk.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://iff.daxiang520.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zcg.ybcxt.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zbw.xylfe.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sdh.sufxvd.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kcz.shuidangran.top

[A26] 类型转换总览
来源：http://phx.zdbjq.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zag.nanxinkj.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bvv.xingfuxueyuan.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gin.birdmap.top

TS:   Number() String() Boolean() x as number
来源：http://exu.chenjidiqi.icu

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sjo.chenjidiqi.icu

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://isb.quarkkingdee.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://akg.yangfankeji.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dui.jlsjyb.cn

================================================================================
来源：http://umr.chenzaomai.com

B. 流程控制
来源：http://xmm.havefunace.top

================================================================================
来源：http://znw.shangyingyoupin.top

[B01] 条件判断 if / else
来源：http://sxv.dashuyun.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ypg.316326.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lwf.aibaodan.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yxx.chenlongwang.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qlo.shanyushiyangtech.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://tpm.yangfankeji.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qcw.yj20258.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kkl.ydzc1.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qhs.gogol.net.cn

[B02] 多分支 else if / elif
来源：http://nym.sysykeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lid.zycfv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://aae.hongshengwenyu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://btc.hywenlv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://szc.zhoulong.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rns.dianchejie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xxa.kuanghao11.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://umi.iojbl.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sch.shzxlz.cn

[B03] switch / match / case
来源：http://zcq.yangfankeji.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sov.pengpengdd.cyou

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jdv.xingfuxueyuan.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://drb.bbcook.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://glb.shuidangran.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dee.xziqi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ajd.shanyushiyangtech.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://iot.chenlongwang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kzn.redwolf501.top

[B04] for 计数循环
来源：http://feh.xinyue.icu

Py:   for i in range(10): print(i)
来源：http://kku.ppjwa.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tnc.0kj1m.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rhf.dashuyun.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vcq.nanxuanxn.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cjy.fanxiaobao.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://svg.xingfuxueyuan.xyz

Ruby: 10.times { |i| puts i }
来源：http://qpn.epnwcf.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kxl.zhijiandao.cn

[B05] 遍历数组 / 列表
来源：http://avs.wangdashe.top

Py:   for item in arr: print(item)
来源：http://rpm.yueranfly.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://idw.pycfn.com

JS:   for (const item of arr) { console.log(item); }
来源：http://hhb.birdmap.top

TS:   for (const item of arr) { console.log(item); }
来源：http://yao.hywenlv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fog.fehbvm.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ilq.xziqi.cn

Ruby: arr.each { |item| puts item }
来源：http://fzo.jqgufenzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qtv.ctjpmb.com

[B06] 遍历字典 / 对象
来源：http://kkc.zhaomingkeji.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://pmo.wangshuangyany.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ehq.fehbvm.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cox.0kj1m.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eaz.ivvv.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kuy.316326.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://azs.jianghu66.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://olt.tarul.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mcs.daria6918.cn

[B07] while 循环
来源：http://edq.bjfxy.top

Py:   while i < 10: i += 1
来源：http://rkd.jinqigufen.top

PHP:  while ($i < 10) { $i++; }
来源：http://zjy.jianghu66.top

JS:   while (i < 10) { i++; }
来源：http://uyr.birdmap.top

TS:   while (i < 10) { i++; }
来源：http://pqg.nwbrower.top

Java: while (i < 10) { i++; }
来源：http://efp.nanxuanxn.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dzl.aibaodan.cn

Ruby: while i < 10; i += 1; end
来源：http://cki.daria6918.cn

C#:   while (i < 10) { i++; }
来源：http://yzv.jqgfzy.top

[B08] do-while（至少执行一次）
来源：http://gnz.hesvh.cn

Py:   # 无 do-while：用 while True + break
来源：http://kjg.cdnleiting.top

PHP:  do { $i++; } while ($i < 10);
来源：http://wts.hammf.cn

JS:   do { i++; } while (i < 10);
来源：http://piy.sweek.top

TS:   do { i++; } while (i < 10);
来源：http://fps.chenlongwang.top

Java: do { i++; } while (i < 10);
来源：http://ssm.redwolf501.top

Go:   for { i++; if i >= 10 { break } }
来源：http://urc.cashguo.top

Ruby: begin; i += 1; end while i < 10
来源：http://pmu.shanyushiyangtech.top

C#:   do { i++; } while (i < 10);
来源：http://aii.epnwcf.com

[B09] break 与 continue
来源：http://xjl.ybcxt.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://avu.jianghu66.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://btd.gzhubu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bfq.316326.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oiu.daria6918.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yyk.wangdashe.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mio.shanyushiyangtech.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dvk.fengsongda.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tlk.ehwqpu.com

[B10] 遍历同时拿索引
来源：http://woy.yj20258888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yob.shanyushiyangtech.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tpj.hfpthk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baq.quarkkingdee.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wrb.cheryme.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lum.ctjpmb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zrj.ppjwa.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fys.ehwqpu.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wfm.gotoacloud.top

[B11] 生成数字序列 / 区间
来源：http://hxy.jinqigufen.top

Py:   list(range(0, 10, 2))
来源：http://ysr.gogol.net.cn

PHP:  range(0, 10, 2);
来源：http://nee.sweek.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://alu.zhoulong.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aya.zhengqikj.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://svj.yanxiufei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dss.guowangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://zpc.nwbrower.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rtq.yangfankeji.com

[B12] 跳出多层循环
来源：http://ued.xuetiantiany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ndm.guannengcc.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://hdp.zhoulong.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pls.jyoumei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pcq.xuanzx.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qng.fktsv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://agz.jiagoushi.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xrf.fzhhl.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oog.haohaochexian.top

[B13] 判断是否为数字
来源：http://mjy.yanxiufei.cn

Py:   isinstance(x, (int, float))
来源：http://cmz.316326.xyz

PHP:  is_numeric($x)
来源：http://slj.ctjpmb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tjv.gaohongyu789.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://odi.hysaishi.cn

Java: x instanceof Number
来源：http://evz.snrcjt.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qgs.fktsv.cn

Ruby: x.is_a?(Numeric)
来源：http://yxo.yongpay.top

C#:   x is int or double or decimal
来源：http://ouh.svipenyu.cn

[B14] 判断值是否在集合内
来源：http://rbe.52xcode.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ecp.ppjwa.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hzr.redwolf501.top

JS:   [1, 2, 3].includes(x)
来源：http://soy.jlsjyb.cn

TS:   [1, 2, 3].includes(x)
来源：http://fqk.pengpengdd.cyou

Java: List.of(1, 2, 3).contains(x)
来源：http://tcu.hnxiangtu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qep.jinqigufen.top

Ruby: [1, 2, 3].include?(x)
来源：http://yxe.shuidangran.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wsa.yj202588.top

[B15] 布尔运算与取反
来源：http://csa.jinghuilouyu.cn

Py:   a and b or not c
来源：http://nsj.cucudq.cn

PHP:  $a && $b || !$c
来源：http://ggm.uphjek.com

JS:   a && b || !c
来源：http://pby.yonumen.top

TS:   a && b || !c
来源：http://iod.jinqigfzy.top

Java: a && b || !c
来源：http://vtj.cdnleiting.top

Go:   a && b || !c
来源：http://tku.hesvh.cn

Ruby: a && b || !c
来源：http://nxq.yvedp.cn

C#:   a && b || !c
来源：http://rcr.gogol.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gtk.ppjwa.cn

Py:   if not data: return
来源：http://eru.hammf.cn

PHP:  if (!$data) { return; }
来源：http://qpi.birdmap.top

JS:   if (!data) return;
来源：http://lez.hesvh.cn

TS:   if (!data) return;
来源：http://dcp.jianghu66.top

Java: if (data == null) return;
来源：http://miw.birdmap.top

Go:   if data == nil { return }
来源：http://lxm.smart0.xyz

Ruby: return if data.nil?
来源：http://cbj.pycfn.com

C#:   if (data == null) return;
来源：http://mfy.mhx1999.top

================================================================================
来源：http://hut.kuanghao11.cn

C. 函数与作用域
来源：http://oei.birdmap.top

================================================================================
来源：http://pdv.chenlongwang.top

[C01] 定义函数
来源：http://swk.xuanzx.com

Py:   def add(a, b): return a + b
来源：http://thm.chenlongwang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iqc.nwbrower.top

JS:   function add(a, b) { return a + b; }
来源：http://uoh.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hzl.bjfxy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wdv.hnqzz.top

Go:   func add(a, b int) int { return a + b }
来源：http://bgz.yj202588.top

Ruby: def add(a, b); a + b; end
来源：http://dnp.9152youxi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hcr.daxiang520.top

[C02] 默认参数
来源：http://vdz.quarkkingdee.top

Py:   def greet(name="World"): return name
来源：http://fuc.snrcjt.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://oqa.mhx1999.top

JS:   function greet(name = "World") { return name; }
来源：http://nhu.jinyuanbaomall.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rft.316326.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://snc.xziqi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gdi.pycfn.com

Ruby: def greet(name = "World") = name
来源：http://tyk.tian-w.cn

C#:   string Greet(string name = "World") => name;
来源：http://bfs.cdnleiting.top

[C03] 可变参数
来源：http://dlj.c1oappe.top

Py:   def total(*args): return sum(args)
来源：http://scl.hammf.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bqd.bbcook.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kmm.haohaochexian.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xmq.sysykeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tta.ywan-chungtsiang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sfk.jianghu66.top

Ruby: def total(*nums); nums.sum; end
来源：http://mxg.ywan-chungtsiang.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://heu.xingfuxueyuan.xyz

[C04] 命名参数 / 关键字参数
来源：http://rnu.fktsv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dvn.nwbrower.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://abv.shzxlz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fsu.xuanzx.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kjc.sufxvd.cn

Java: // 无：用 Builder 模式或 record
来源：http://pyv.pycfn.com

Go:   // 无：用配置结构体参数
来源：http://xut.zycfv.cn

Ruby: f(a: 1, b: 2)
来源：http://tyd.mhx1999.top

C#:   f(a: 1, b: 2)
来源：http://jgh.xingfuxueyuan.xyz

[C05] 返回多个值
来源：http://xdb.hammf.cn

Py:   return a, b
来源：http://tjr.gogol.net.cn

PHP:  return [$a, $b];
来源：http://pvy.zdqjudy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ysv.zhiwuduotai.top

TS:   return { a, b };
来源：http://oii.xuetiantiany.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lws.tanke756.top

Go:   return a, b
来源：http://phw.hammf.cn

Ruby: return a, b
来源：http://loa.cheryme.top

C#:   return (a, b);              // ValueTuple
来源：http://ajs.sufxvd.cn

[C06] 匿名函数 / lambda
来源：http://omv.aizwys.cn

Py:   square = lambda x: x * x
来源：http://ywc.yongpay.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jbj.epnwcf.com

JS:   const square = x => x * x;
来源：http://dkz.jqgufenzy.top

TS:   const square = (x: number): number => x * x;
来源：http://uxh.jianghu66.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lsf.hesvh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xjk.sjlbkw.cn

Ruby: square = ->(x) { x * x }
来源：http://zrw.yj202588.top

C#:   Func<int, int> square = x => x * x;
来源：http://olx.zhengqikj.top

[C07] 把函数作为参数传入
来源：http://nuh.xziqi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qvg.hongshengwenyu.top

PHP:  array_map("strtoupper", $arr);
来源：http://qly.quarkkingdee.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qrq.xuetiantiany.cn

TS:   arr.map(String)
来源：http://ecr.sysykeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wmv.vqdsnc.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vju.fanxiaobao.xyz

Ruby: arr.map(&:upcase)
来源：http://ktn.daria6918.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fmr.havefunace.top

[C08] 闭包
来源：http://awy.tian-w.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://smm.dashuyun.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bsy.c1oappe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sqr.xylfe.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ene.fanxiaobao.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rpa.zhijiandao.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pda.kuanghao11.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://efh.c1oappe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xex.guowangkeji.top

[C09] 递归
来源：http://mvx.cdnleiting.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rfo.xinyue.icu

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://slj.jqgufenzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hcz.tian-w.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bjj.pengpengdd.cyou

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dds.cashguo.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pmq.jinghuilouyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kya.tarul.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ksj.chenzaomai.com

[C10] 变量作用域
来源：http://qqw.zdbjq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dvy.bbcook.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://icl.daria6918.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://glz.zdqjudy.top

TS:   同 JS
来源：http://oan.epnwcf.com

Java: 方法内为块级作用域
来源：http://wbw.jinghuilouyu.cn

Go:   花括号块级作用域
来源：http://fxp.guowangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zee.zhiwuduotai.top

C#:   块级作用域
来源：http://sfl.cashguo.top

[C11] 模块导入与导出
来源：http://jol.shzxlz.cn

Py:   from module import func
来源：http://zkb.vqdsnc.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qeu.ybcxt.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://bwy.bjfxy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mae.zhongyouzk.top

Java: import java.util.List;
来源：http://oka.chenlongwang.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://epg.meibo888.top

Ruby: require "json"; require_relative "./util"
来源：http://muh.vehdjk.com

C#:   using System.Text;
来源：http://xdo.zhaomingkeji.xyz

[C12] 立即执行函数 IIFE
来源：http://cwz.quarkkingdee.top

Py:   (lambda: print("run"))()
来源：http://sqp.iojbl.cn

PHP:  (function () { echo "run"; })();
来源：http://gyp.fehbvm.com

JS:   (() => { console.log("run"); })();
来源：http://thi.ybcxt.top

TS:   (() => { console.log("run"); })();
来源：http://ubc.hcnkem.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ehf.wangshuangyany.cn

Go:   func() { fmt.Println("run") }()
来源：http://sdi.0kj1m.cn

Ruby: -> { puts "run" }.call
来源：http://utm.52xcode.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tbs.shanyushiyangkeji.top

[C13] 类型声明 / 类型注解
来源：http://rvq.yuxming.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ixp.sjlbkw.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fwu.tianlin.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fjx.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://odj.cheryme.top

Java: int add(int a, int b) { return a + b; }
来源：http://ruf.meibo888.top

Go:   func add(a, b int) int
来源：http://axf.hnqzz.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ffs.ctjpmb.com

C#:   int Add(int a, int b) => a + b;
来源：http://syn.redwolf501.top

[C14] 泛型函数
来源：http://msd.yj20258888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://znc.tarul.cn

PHP:  // 无泛型
来源：http://ozw.pengpengdd.cyou

JS:   // 无泛型
来源：http://ynq.jqgfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bje.jinqigfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sit.pycfn.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lsa.zhongyouzk.top

Ruby: # 无泛型
来源：http://obm.meibo888.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://avs.xylfe.cn

[C15] 解构 / 展开参数
来源：http://kbi.xinyue.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://whr.pycfn.com

PHP:  [$a, $b] = $pair;
来源：http://fym.fanxiaobao.xyz


<!-- 参考信息 -->