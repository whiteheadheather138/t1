代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lhk.chenlongwang.top

C#:   s.ToUpper(); s.ToLower()
来源：http://amg.xingfuxueyuan.xyz

[A24] 去除首尾空白
来源：http://avm.daxiang520.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://igh.hnxiangtu.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jtu.wangdashe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oiu.tianlin.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hey.kuanghao11.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zek.dashuyun.cn

Go:   strings.TrimSpace(s)
来源：http://usm.nwbrower.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ukt.yonumen.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dyh.epnwcf.com

[A25] 字符串比较
来源：http://ufh.hysaishi.cn

Py:   s1 == s2; s1 != s2
来源：http://crz.ivvv.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fza.yueranfly.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mze.iojbl.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gih.hongshengwenyu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://scu.gotoacloud.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xjy.ydjk.org.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vtv.smart0.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sur.sufxvd.cn

[A26] 类型转换总览
来源：http://wxg.cdnleiting.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://iny.shanyushiyangkeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kid.xingfuxueyuan.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vpm.zycfv.cn

TS:   Number() String() Boolean() x as number
来源：http://ibd.cheryme.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hzi.jiagoushi.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jjm.meibo888.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://xpr.feifeiyinyue.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ufx.hnqzz.top

================================================================================
来源：http://xrl.yanxiufei.cn

B. 流程控制
来源：http://vbj.zhaomingkeji.xyz

================================================================================
来源：http://pfg.xuanzx.com

[B01] 条件判断 if / else
来源：http://xsr.kuanghao11.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rgp.yongpay.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qrx.shuidangran.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tse.hammf.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uow.gogol.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wdf.aibaodan.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oxf.sweek.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rww.smart0.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wee.xziqi.cn

[B02] 多分支 else if / elif
来源：http://lth.daria6918.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dpb.hnxiangtu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dqb.nwbrower.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ipo.tarul.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jiq.yj20258.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://amh.chenzaomai.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hsq.birdmap.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iuu.quarkkingdee.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yhf.fzhhl.top

[B03] switch / match / case
来源：http://kqa.birdmap.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fbx.dashuyun.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vik.cqqwz.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://azl.zdbjq.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://riw.jinyuanbaomall.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kns.xingfuxueyuan.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ywh.meibo888.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kfg.epnwcf.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vhs.52xcode.cn

[B04] for 计数循环
来源：http://yah.jqgufenzy.top

Py:   for i in range(10): print(i)
来源：http://tpf.guannengcc.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jtp.shuidangran.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hcc.nanxinkj.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bjt.yvedp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jag.shanyushiyangtech.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://phy.jyoumei.cn

Ruby: 10.times { |i| puts i }
来源：http://bmg.jqgfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nvn.hongshengwenyu.top

[B05] 遍历数组 / 列表
来源：http://jkl.yueranfly.top

Py:   for item in arr: print(item)
来源：http://epv.zhixingplan.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pua.jyoumei.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://aiv.fanxiaobao.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://lzt.yongpay.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://cog.haohaochexian.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kyq.fengsongda.top

Ruby: arr.each { |item| puts item }
来源：http://tjz.guowangkeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cqc.vehdjk.com

[B06] 遍历字典 / 对象
来源：http://yhq.snrcjt.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://obs.chenzaomai.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ori.zdqjudy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jsm.redwolf501.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zcx.zdqjudy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vcy.zhaomingkeji.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hrp.jinghuilouyu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jaj.sufxvd.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mfe.feifeiyinyue.top

[B07] while 循环
来源：http://hgy.jinyuanbaomall.cn

Py:   while i < 10: i += 1
来源：http://wpc.vehdjk.com

PHP:  while ($i < 10) { $i++; }
来源：http://xcj.jianghu66.top

JS:   while (i < 10) { i++; }
来源：http://uiz.zycfv.cn

TS:   while (i < 10) { i++; }
来源：http://spf.shangyingyoupin.top

Java: while (i < 10) { i++; }
来源：http://mdr.haohaochexian.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://byy.tanke756.top

Ruby: while i < 10; i += 1; end
来源：http://loe.wangshuangyany.cn

C#:   while (i < 10) { i++; }
来源：http://hha.gogol.net.cn

[B08] do-while（至少执行一次）
来源：http://mvs.chenjidiqi.icu

Py:   # 无 do-while：用 while True + break
来源：http://rfx.zhengqikj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://euf.ydjk.org.cn

JS:   do { i++; } while (i < 10);
来源：http://nvt.sysykeji.top

TS:   do { i++; } while (i < 10);
来源：http://zng.cheryme.top

Java: do { i++; } while (i < 10);
来源：http://fen.xylfe.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qko.xinyue.icu

Ruby: begin; i += 1; end while i < 10
来源：http://wvw.yonumen.top

C#:   do { i++; } while (i < 10);
来源：http://jap.xziqi.cn

[B09] break 与 continue
来源：http://gie.tian-w.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dhq.fanxiaobao.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hmj.tianlin.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gki.shuidangran.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oya.haohaochexian.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dcj.sufxvd.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://edl.tian-w.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gnk.chenjidiqi.icu

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hcx.guowangkeji.top

[B10] 遍历同时拿索引
来源：http://tsf.uphjek.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://aox.quarkkingdee.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zpg.xylfe.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ria.sxryk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://clw.gogol.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wsr.sxryk.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://iin.yueranfly.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tls.birdmap.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cvj.jiagoushi.top

[B11] 生成数字序列 / 区间
来源：http://zvw.guannengcc.top

Py:   list(range(0, 10, 2))
来源：http://zkl.quarkkingdee.top

PHP:  range(0, 10, 2);
来源：http://jco.jlsjyb.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yst.ydjk.org.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://drr.daxiang520.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uda.chenzaomai.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ovy.hesvh.cn

Ruby: (0...10).step(2).to_a
来源：http://skd.yanxiufei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://aue.yuxming.cn

[B12] 跳出多层循环
来源：http://mge.sysykeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://guc.pycfn.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://oal.yvedp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://spm.hammf.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gyf.hammf.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qps.cucudq.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bvg.yongpay.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uta.yueranfly.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aql.xingfuxueyuan.xyz

[B13] 判断是否为数字
来源：http://ztf.hesvh.cn

Py:   isinstance(x, (int, float))
来源：http://ahn.smart0.xyz

PHP:  is_numeric($x)
来源：http://qzu.yj20258.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ubu.yangfankeji.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fth.guannengcc.top

Java: x instanceof Number
来源：http://inc.ehwqpu.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://btd.zhengqikj.top

Ruby: x.is_a?(Numeric)
来源：http://dhd.yuanzhike.top

C#:   x is int or double or decimal
来源：http://jah.ehwqpu.com

[B14] 判断值是否在集合内
来源：http://igu.tanke756.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://prc.c1oappe.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jae.zdbjq.cn

JS:   [1, 2, 3].includes(x)
来源：http://gov.ydjk.org.cn

TS:   [1, 2, 3].includes(x)
来源：http://fbm.9152youxi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xyp.jyoumei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oyd.daxiang520.top

Ruby: [1, 2, 3].include?(x)
来源：http://jdz.gaohongyu789.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://isy.sysykeji.top

[B15] 布尔运算与取反
来源：http://dyn.zhijiandao.cn

Py:   a and b or not c
来源：http://axx.ywan-chungtsiang.top

PHP:  $a && $b || !$c
来源：http://ove.hywenlv.cn

JS:   a && b || !c
来源：http://rfg.jiagoushi.top

TS:   a && b || !c
来源：http://mfr.yj20258888.top

Java: a && b || !c
来源：http://dcr.mhx1999.top

Go:   a && b || !c
来源：http://kcc.havefunace.top

Ruby: a && b || !c
来源：http://syh.xziqi.cn

C#:   a && b || !c
来源：http://bwr.gaohongyu789.top

[B16] 卫语句：不满足条件提前返回
来源：http://abe.hnxiangtu.top

Py:   if not data: return
来源：http://grm.hysaishi.cn

PHP:  if (!$data) { return; }
来源：http://hjv.cashguo.top

JS:   if (!data) return;
来源：http://zrb.xuanzx.com

TS:   if (!data) return;
来源：http://piz.yj202588.top

Java: if (data == null) return;
来源：http://uce.wangshuangyany.cn

Go:   if data == nil { return }
来源：http://kyl.nwbrower.top

Ruby: return if data.nil?
来源：http://pzh.birdmap.top

C#:   if (data == null) return;
来源：http://xlu.sjlbkw.cn

================================================================================
来源：http://eiz.mhx1999.top

C. 函数与作用域
来源：http://gte.nanxuanxn.top

================================================================================
来源：http://czu.fanxiaobao.xyz

[C01] 定义函数
来源：http://ega.ybcxt.top

Py:   def add(a, b): return a + b
来源：http://vyk.hywenlv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zju.ydjk.org.cn

JS:   function add(a, b) { return a + b; }
来源：http://ful.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ydf.hysaishi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zmx.zhongyouzk.top

Go:   func add(a, b int) int { return a + b }
来源：http://spd.fktsv.cn

Ruby: def add(a, b); a + b; end
来源：http://fpp.kuanghao11.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dhz.guannengcc.top

[C02] 默认参数
来源：http://zso.hammf.cn

Py:   def greet(name="World"): return name
来源：http://vzd.xuetiantiany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dwm.zhoulong.xyz

JS:   function greet(name = "World") { return name; }
来源：http://mnr.nanxuanxn.top

TS:   function greet(name: string = "World") { return name; }
来源：http://oei.snrcjt.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ses.kuanghao11.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rsh.snrcjt.cn

Ruby: def greet(name = "World") = name
来源：http://pzq.ybcxt.top

C#:   string Greet(string name = "World") => name;
来源：http://hfr.nanxinkj.top

[C03] 可变参数
来源：http://hvm.52xcode.cn

Py:   def total(*args): return sum(args)
来源：http://tnw.xinyue.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yvp.fktsv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qxj.shuidangran.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ivj.jianghu66.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fie.jiagoushi.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pnq.redwolf501.top

Ruby: def total(*nums); nums.sum; end
来源：http://uiz.fanxiaobao.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nau.zhixingplan.top

[C04] 命名参数 / 关键字参数
来源：http://lar.hnxiangtu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mxs.birdmap.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nrl.epnwcf.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cjq.yj20258888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rnk.kuanghao11.cn

Java: // 无：用 Builder 模式或 record
来源：http://ofi.shangyingyoupin.top

Go:   // 无：用配置结构体参数
来源：http://rea.chenlongwang.top

Ruby: f(a: 1, b: 2)
来源：http://fxm.yj20258.top

C#:   f(a: 1, b: 2)
来源：http://art.jqgfzy.top

[C05] 返回多个值
来源：http://byw.jiagoushi.top

Py:   return a, b
来源：http://cak.ppjwa.cn

PHP:  return [$a, $b];
来源：http://jkb.quarkkingdee.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://cye.gotoacloud.top

TS:   return { a, b };
来源：http://xwl.yuanzhike.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mgp.havefunace.top

Go:   return a, b
来源：http://xad.yvedp.cn

Ruby: return a, b
来源：http://wzf.xuetiantiany.cn

C#:   return (a, b);              // ValueTuple
来源：http://vju.9152youxi.cn

[C06] 匿名函数 / lambda
来源：http://zhu.sxryk.cn

Py:   square = lambda x: x * x
来源：http://eqw.tarul.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uoy.cdnleiting.top

JS:   const square = x => x * x;
来源：http://otu.smart0.xyz

TS:   const square = (x: number): number => x * x;
来源：http://lqg.yfazqb.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vgc.hywenlv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tvc.hnqzz.top

Ruby: square = ->(x) { x * x }
来源：http://hhz.meibo888.top

C#:   Func<int, int> square = x => x * x;
来源：http://vzt.fanxiaobao.xyz

[C07] 把函数作为参数传入
来源：http://frc.hammf.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jwp.fzhhl.top

PHP:  array_map("strtoupper", $arr);
来源：http://bbx.zdqjudy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hhf.316326.xyz

TS:   arr.map(String)
来源：http://gpw.pengpengdd.cyou

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uix.iojbl.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lor.aibaodan.cn

Ruby: arr.map(&:upcase)
来源：http://uuc.cqqwz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xci.gogol.net.cn

[C08] 闭包
来源：http://lcv.sxryk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cxr.jqgfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fgg.hcnkem.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://usf.shzxlz.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bqu.ehwqpu.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qer.cashguo.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lar.redwolf501.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mqo.wangshuangyany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://stp.jinghuilouyu.cn

[C09] 递归
来源：http://kys.gaohongyu789.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://iri.xuanzx.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ypj.hfpthk.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nru.yuxming.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yho.fehbvm.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mrc.chenlongwang.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tns.ybcxt.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cxt.ybcxt.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gsg.sjlbkw.cn

[C10] 变量作用域
来源：http://eql.zhongyouzk.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cto.chenlongwang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dsd.jianghu66.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fds.shangyingyoupin.top

TS:   同 JS
来源：http://wbe.yueranfly.top

Java: 方法内为块级作用域
来源：http://sqb.yonumen.top

Go:   花括号块级作用域
来源：http://pij.chenzaomai.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hsv.hfpthk.cn

C#:   块级作用域
来源：http://qrh.shanyushiyangtech.top

[C11] 模块导入与导出
来源：http://sai.tianlin.xyz

Py:   from module import func
来源：http://vsq.fktsv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lqm.bbcook.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://goc.jinyuanbaomall.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bal.xinyue.icu

Java: import java.util.List;
来源：http://tuk.chenlongwang.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oxh.yangfankeji.com

Ruby: require "json"; require_relative "./util"
来源：http://trd.sweek.top

C#:   using System.Text;
来源：http://wlm.52xcode.cn

[C12] 立即执行函数 IIFE
来源：http://fib.mhx1999.top

Py:   (lambda: print("run"))()
来源：http://ttx.sysykeji.top

PHP:  (function () { echo "run"; })();
来源：http://vfr.pycfn.com

JS:   (() => { console.log("run"); })();
来源：http://fzz.vehdjk.com

TS:   (() => { console.log("run"); })();
来源：http://qit.dianchejie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vhk.fanxiaobao.xyz

Go:   func() { fmt.Println("run") }()
来源：http://gfu.9152youxi.cn

Ruby: -> { puts "run" }.call
来源：http://kcd.ybcxt.top

C#:   // 无 IIFE：用静态构造函数
来源：http://kyh.redwolf501.top

[C13] 类型声明 / 类型注解
来源：http://hzc.yuanzhike.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://izb.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dlh.zhoulong.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://afg.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zhb.ppjwa.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vvc.shzxlz.cn

Go:   func add(a, b int) int
来源：http://gcs.zhiwuduotai.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://brp.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://ljw.pycfn.com

[C14] 泛型函数
来源：http://khd.chenlongwang.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qrg.aizwys.cn

PHP:  // 无泛型
来源：http://bjt.ppjwa.cn

JS:   // 无泛型
来源：http://hiu.iojbl.cn


<!-- 参考信息 -->