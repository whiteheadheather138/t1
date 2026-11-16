代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nug.cucudq.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://emi.gogol.net.cn

[A24] 去除首尾空白
来源：http://vkl.ydjk.org.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jmm.shanyushiyangtech.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qal.birdmap.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ola.feifeiyinyue.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wji.xylfe.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vsw.yj20258888.top

Go:   strings.TrimSpace(s)
来源：http://bhr.aizwys.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yak.jqgufenzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ngq.cheryme.top

[A25] 字符串比较
来源：http://gsy.xuanzx.com

Py:   s1 == s2; s1 != s2
来源：http://cxt.sysykeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cdu.cashguo.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lzl.yuanzhike.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fbn.52xcode.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nto.yonumen.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://aql.snrcjt.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lba.fehbvm.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://eys.hesvh.cn

[A26] 类型转换总览
来源：http://oem.gotoacloud.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://czw.sxryk.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fyc.shanyushiyangtech.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jrj.svipenyu.cn

TS:   Number() String() Boolean() x as number
来源：http://lex.shuidangran.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://orn.fanxiaobao.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://onr.jiagoushi.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://yqt.jyoumei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://usa.sweek.top

================================================================================
来源：http://vgb.kuanghao11.cn

B. 流程控制
来源：http://tlq.shanyushiyangkeji.top

================================================================================
来源：http://qjq.snrcjt.cn

[B01] 条件判断 if / else
来源：http://ztf.xinyue.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://jyy.aizwys.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://arl.gaohongyu789.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bam.jinqigufen.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://apr.daxiang520.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://uco.sxryk.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://aeh.xylfe.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xuf.jinqigufen.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dih.wangshuangyany.cn

[B02] 多分支 else if / elif
来源：http://lsv.0kj1m.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qte.zhongyouzk.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://olc.jyoumei.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://saj.pycfn.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://omy.yfazqb.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bgx.sweek.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fbo.fzhhl.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ztg.snrcjt.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ocx.guannengcc.top

[B03] switch / match / case
来源：http://aka.zycfv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lke.hfpthk.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kor.cqqwz.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ody.yvedp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://und.dianchejie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://frp.zdqjudy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wsz.jqgfzy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bku.gzhubu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sqg.cqqwz.cn

[B04] for 计数循环
来源：http://ltp.redwolf501.top

Py:   for i in range(10): print(i)
来源：http://uzf.mhx1999.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tbp.jiagoushi.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cso.fktsv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tun.iojbl.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ocr.daria6918.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wfc.vehdjk.com

Ruby: 10.times { |i| puts i }
来源：http://jms.shanyushiyangtech.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://puv.yongpay.top

[B05] 遍历数组 / 列表
来源：http://jgb.fehbvm.com

Py:   for item in arr: print(item)
来源：http://syb.c1oappe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zas.wangdashe.top

JS:   for (const item of arr) { console.log(item); }
来源：http://yzh.pycfn.com

TS:   for (const item of arr) { console.log(item); }
来源：http://arg.quarkkingdee.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://hkp.hongshengwenyu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pok.nanxinkj.top

Ruby: arr.each { |item| puts item }
来源：http://xxc.hnqzz.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gym.yonumen.top

[B06] 遍历字典 / 对象
来源：http://pxn.jinyuanbaomall.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://txq.haohaochexian.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uyr.nanxuanxn.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rsb.guowangkeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qsb.xuanzx.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uqi.cqqwz.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gut.jyoumei.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mny.dianchejie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ktz.zhiwuduotai.top

[B07] while 循环
来源：http://khv.pycfn.com

Py:   while i < 10: i += 1
来源：http://xrt.sweek.top

PHP:  while ($i < 10) { $i++; }
来源：http://lyi.hongshengwenyu.top

JS:   while (i < 10) { i++; }
来源：http://hqv.cheryme.top

TS:   while (i < 10) { i++; }
来源：http://wnd.svipenyu.cn

Java: while (i < 10) { i++; }
来源：http://qan.yangfankeji.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dbi.jqgufenzy.top

Ruby: while i < 10; i += 1; end
来源：http://vrl.nanxuanxn.top

C#:   while (i < 10) { i++; }
来源：http://stc.jiagoushi.top

[B08] do-while（至少执行一次）
来源：http://scf.shzxlz.cn

Py:   # 无 do-while：用 while True + break
来源：http://gwr.zhixingplan.top

PHP:  do { $i++; } while ($i < 10);
来源：http://pfj.nwbrower.top

JS:   do { i++; } while (i < 10);
来源：http://nbu.yuxming.cn

TS:   do { i++; } while (i < 10);
来源：http://fvl.bjfxy.top

Java: do { i++; } while (i < 10);
来源：http://ihj.yuanzhike.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bpa.0kj1m.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dqq.aizwys.cn

C#:   do { i++; } while (i < 10);
来源：http://qbe.dashuyun.cn

[B09] break 与 continue
来源：http://ypn.wangdashe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dog.quarkkingdee.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://npd.zhongyouzk.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://noh.zdqjudy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kfi.gaohongyu789.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lpe.gogol.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iem.pengpengdd.cyou

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lkd.tianlin.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uwl.hywenlv.cn

[B10] 遍历同时拿索引
来源：http://opa.jinghuilouyu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://azb.nwbrower.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ocl.gzhubu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://udm.jinyuanbaomall.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://shp.yuxming.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qvc.pengpengdd.cyou

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://itq.redwolf501.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://utg.sjlbkw.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://aau.wangshuangyany.cn

[B11] 生成数字序列 / 区间
来源：http://ico.shanyushiyangtech.top

Py:   list(range(0, 10, 2))
来源：http://nuw.fehbvm.com

PHP:  range(0, 10, 2);
来源：http://fum.zhiwuduotai.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xiu.zdqjudy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ole.tanke756.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zel.hywenlv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://off.jinghuilouyu.cn

Ruby: (0...10).step(2).to_a
来源：http://oyo.zhaomingkeji.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dbt.zhaomingkeji.xyz

[B12] 跳出多层循环
来源：http://uqo.cheryme.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://znh.sweek.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cfg.xinyue.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ika.xuetiantiany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ftq.chenlongwang.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://whd.cashguo.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wkp.316326.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ken.9152youxi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://udx.yangfankeji.com

[B13] 判断是否为数字
来源：http://ryd.yongpay.top

Py:   isinstance(x, (int, float))
来源：http://mdp.aizwys.cn

PHP:  is_numeric($x)
来源：http://ciz.daria6918.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zuh.hammf.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tst.shanyushiyangkeji.top

Java: x instanceof Number
来源：http://itx.gaohongyu789.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ycq.jinyuanbaomall.cn

Ruby: x.is_a?(Numeric)
来源：http://hjy.jinghuilouyu.cn

C#:   x is int or double or decimal
来源：http://xbd.dianchejie.cn

[B14] 判断值是否在集合内
来源：http://vck.ctjpmb.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tgk.gaohongyu789.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mnk.52xcode.cn

JS:   [1, 2, 3].includes(x)
来源：http://zji.yongpay.top

TS:   [1, 2, 3].includes(x)
来源：http://rcu.sweek.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ylh.shuidangran.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jzd.ywan-chungtsiang.top

Ruby: [1, 2, 3].include?(x)
来源：http://vva.dianchejie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://glo.shzxlz.cn

[B15] 布尔运算与取反
来源：http://fxt.tarul.cn

Py:   a and b or not c
来源：http://pcl.yueranfly.top

PHP:  $a && $b || !$c
来源：http://fqy.havefunace.top

JS:   a && b || !c
来源：http://mcm.cqqwz.cn

TS:   a && b || !c
来源：http://exn.shanyushiyangtech.top

Java: a && b || !c
来源：http://dgg.wangshuangyany.cn

Go:   a && b || !c
来源：http://fuz.xingfuxueyuan.xyz

Ruby: a && b || !c
来源：http://fbh.dashuyun.cn

C#:   a && b || !c
来源：http://dkf.zhongyouzk.top

[B16] 卫语句：不满足条件提前返回
来源：http://rcq.xziqi.cn

Py:   if not data: return
来源：http://zmd.ivvv.top

PHP:  if (!$data) { return; }
来源：http://gzy.nanxuanxn.top

JS:   if (!data) return;
来源：http://usd.iojbl.cn

TS:   if (!data) return;
来源：http://dgk.cqqwz.cn

Java: if (data == null) return;
来源：http://yor.hesvh.cn

Go:   if data == nil { return }
来源：http://lmi.jianghu66.top

Ruby: return if data.nil?
来源：http://hkt.tanke756.top

C#:   if (data == null) return;
来源：http://xaz.vehdjk.com

================================================================================
来源：http://uwx.9152youxi.cn

C. 函数与作用域
来源：http://dyu.ywan-chungtsiang.top

================================================================================
来源：http://zmp.bjfxy.top

[C01] 定义函数
来源：http://xvs.quarkkingdee.top

Py:   def add(a, b): return a + b
来源：http://cfk.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bbh.yueranfly.top

JS:   function add(a, b) { return a + b; }
来源：http://bxx.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.wangshuangyany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gww.cashguo.top

Go:   func add(a, b int) int { return a + b }
来源：http://kyy.ppjwa.cn

Ruby: def add(a, b); a + b; end
来源：http://nka.ydjk.org.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vpv.gogol.net.cn

[C02] 默认参数
来源：http://jxn.zhixingplan.top

Py:   def greet(name="World"): return name
来源：http://srm.birdmap.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vcg.0kj1m.cn

JS:   function greet(name = "World") { return name; }
来源：http://nex.jianghu66.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fod.cheryme.top

Java: // 无默认参数：方法重载或 Optional
来源：http://jli.mhx1999.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://prp.hcnkem.com

Ruby: def greet(name = "World") = name
来源：http://snn.ybcxt.top

C#:   string Greet(string name = "World") => name;
来源：http://pwl.sxryk.cn

[C03] 可变参数
来源：http://pkz.yuxming.cn

Py:   def total(*args): return sum(args)
来源：http://mbb.cashguo.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zzi.vqdsnc.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vod.epnwcf.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yni.jyoumei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zqx.cdnleiting.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wqn.ydjk.org.cn

Ruby: def total(*nums); nums.sum; end
来源：http://unl.zhongyouzk.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mhp.yuanzhike.top

[C04] 命名参数 / 关键字参数
来源：http://ypi.dashuyun.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zur.quarkkingdee.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uwe.shanyushiyangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vty.guowangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tit.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://jsy.aibaodan.cn

Go:   // 无：用配置结构体参数
来源：http://ksi.ivvv.top

Ruby: f(a: 1, b: 2)
来源：http://clq.9152youxi.cn

C#:   f(a: 1, b: 2)
来源：http://nbl.chenzaomai.com

[C05] 返回多个值
来源：http://zuy.guannengcc.top

Py:   return a, b
来源：http://bjb.jinqigfzy.top

PHP:  return [$a, $b];
来源：http://zaa.jianghu66.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://hfb.hammf.cn

TS:   return { a, b };
来源：http://hdd.hcnkem.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jri.nwbrower.top

Go:   return a, b
来源：http://hxw.jiagoushi.top

Ruby: return a, b
来源：http://uwt.ctjpmb.com

C#:   return (a, b);              // ValueTuple
来源：http://yhe.hcnkem.com

[C06] 匿名函数 / lambda
来源：http://jyc.xingfuxueyuan.xyz

Py:   square = lambda x: x * x
来源：http://npt.ivvv.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qhr.hongshengwenyu.top

JS:   const square = x => x * x;
来源：http://dnn.smart0.xyz

TS:   const square = (x: number): number => x * x;
来源：http://uuq.yonumen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tmz.xinyue.icu

Go:   sq := func(x int) int { return x * x }
来源：http://ywe.ctjpmb.com

Ruby: square = ->(x) { x * x }
来源：http://hpl.wangshuangyany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://eax.yj20258888.top

[C07] 把函数作为参数传入
来源：http://zvl.jiagoushi.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mty.ehwqpu.com

PHP:  array_map("strtoupper", $arr);
来源：http://rrm.gogol.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gtr.zdbjq.cn

TS:   arr.map(String)
来源：http://sor.uphjek.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gfc.xuanzx.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zqm.bjfxy.top

Ruby: arr.map(&:upcase)
来源：http://pct.yueranfly.top

C#:   arr.Select(s => s.ToUpper())
来源：http://rtf.yuxming.cn

[C08] 闭包
来源：http://bfi.fktsv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://faz.cucudq.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ddq.feifeiyinyue.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sgs.yj20258888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://obh.ydzc1.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hsn.wangshuangyany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vod.shzxlz.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://moq.ehwqpu.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yya.shuidangran.top

[C09] 递归
来源：http://uum.hesvh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://buk.sxryk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rei.yongpay.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://drb.cdnleiting.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ocq.yuxming.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nxh.chenjidiqi.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uxu.chenjidiqi.icu

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zna.52xcode.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ivs.gzhubu.top

[C10] 变量作用域
来源：http://rhp.zdbjq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kbi.cdnleiting.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ern.yanxiufei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://olh.daxiang520.top

TS:   同 JS
来源：http://zzi.hnxiangtu.top

Java: 方法内为块级作用域
来源：http://qhz.andypj.xyz

Go:   花括号块级作用域
来源：http://msk.yonumen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ach.smart0.xyz

C#:   块级作用域
来源：http://uwg.nwbrower.top

[C11] 模块导入与导出
来源：http://fbx.sweek.top

Py:   from module import func
来源：http://vrs.c1oappe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://bef.fzhhl.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://lum.havefunace.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qmg.snrcjt.cn

Java: import java.util.List;
来源：http://pwq.yj202588.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yhr.andypj.xyz

Ruby: require "json"; require_relative "./util"
来源：http://van.chenzaomai.com

C#:   using System.Text;
来源：http://ery.daria6918.cn

[C12] 立即执行函数 IIFE
来源：http://htf.jianghu66.top

Py:   (lambda: print("run"))()
来源：http://xcg.xinyue.icu

PHP:  (function () { echo "run"; })();
来源：http://tfq.ydzc1.top

JS:   (() => { console.log("run"); })();
来源：http://aqf.iojbl.cn

TS:   (() => { console.log("run"); })();
来源：http://xwd.shanyushiyangtech.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lqo.fzhhl.top

Go:   func() { fmt.Println("run") }()
来源：http://qjd.epnwcf.com

Ruby: -> { puts "run" }.call
来源：http://oum.kuanghao11.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lyh.hfpthk.cn

[C13] 类型声明 / 类型注解
来源：http://ptc.jiagoushi.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://esd.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wpc.jianghu66.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mdd.shangyingyoupin.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vhi.9152youxi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tng.yvedp.cn

Go:   func add(a, b int) int
来源：http://peu.shangyingyoupin.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qpz.shanyushiyangtech.top

C#:   int Add(int a, int b) => a + b;
来源：http://xbp.xuanzx.com

[C14] 泛型函数
来源：http://hni.shuidangran.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://biq.wangshuangyany.cn

PHP:  // 无泛型
来源：http://zkq.jqgfzy.top

JS:   // 无泛型
来源：http://nik.vqdsnc.cn


<!-- 参考信息 -->