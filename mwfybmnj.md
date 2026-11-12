代发 wailian999

C#:   s.Length
来源：http://jei.sxryk.cn

[A23] 大小写转换
来源：http://wzr.zhengqikj.top

Py:   s.upper(); s.lower(); s.title()
来源：http://vmh.sweek.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pub.yongpay.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nfj.svipenyu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://azs.xinyue.icu

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bsl.epnwcf.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cts.jinqigfzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dfl.jyoumei.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fen.shanyushiyangkeji.top

[A24] 去除首尾空白
来源：http://sud.9152youxi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gfw.tianlin.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hxq.yj202588.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fql.tianlin.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pki.shanyushiyangkeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lwx.bjfxy.top

Go:   strings.TrimSpace(s)
来源：http://tca.ivvv.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gdq.fehbvm.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://icp.hywenlv.cn

[A25] 字符串比较
来源：http://fav.hfpthk.cn

Py:   s1 == s2; s1 != s2
来源：http://bvd.yonumen.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dxw.dianchejie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vjs.zhixingplan.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uvl.cashguo.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://odm.chenzaomai.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://npj.52xcode.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yzg.zhongyouzk.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sfn.yangfankeji.com

[A26] 类型转换总览
来源：http://wtq.zhongyouzk.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kxi.meibo888.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wpl.daria6918.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ibr.vqdsnc.cn

TS:   Number() String() Boolean() x as number
来源：http://gzl.wangshuangyany.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sah.zhijiandao.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cgu.hywenlv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pkt.shzxlz.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ebz.fengsongda.top

================================================================================
来源：http://kvb.quarkkingdee.top

B. 流程控制
来源：http://xja.316326.xyz

================================================================================
来源：http://yom.ywan-chungtsiang.top

[B01] 条件判断 if / else
来源：http://fnq.gotoacloud.top

Py:   result = "正" if x > 0 else "非正"
来源：http://wqr.shangyingyoupin.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qpr.jinqigfzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ybl.vehdjk.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yik.sxryk.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kee.gotoacloud.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ihb.hesvh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ump.jlsjyb.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://oyt.sxryk.cn

[B02] 多分支 else if / elif
来源：http://ahe.yuanzhike.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://huj.sjlbkw.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ccf.gaohongyu789.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://okr.svipenyu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hzh.jqgfzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ktj.tarul.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qtr.iojbl.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zkg.jianghu66.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wvg.daria6918.cn

[B03] switch / match / case
来源：http://bax.chenjidiqi.icu

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bgr.hnqzz.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yde.epnwcf.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nzf.dashuyun.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bcp.sweek.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zcj.hcnkem.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://amz.vqdsnc.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dsj.chenzaomai.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dvv.jlsjyb.cn

[B04] for 计数循环
来源：http://ynj.fktsv.cn

Py:   for i in range(10): print(i)
来源：http://prf.mhx1999.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tlz.hywenlv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lgm.gotoacloud.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sui.havefunace.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://evy.zhengqikj.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fik.zhaomingkeji.xyz

Ruby: 10.times { |i| puts i }
来源：http://ggk.shzxlz.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://und.sysykeji.top

[B05] 遍历数组 / 列表
来源：http://prv.zhaomingkeji.xyz

Py:   for item in arr: print(item)
来源：http://vlo.nanxinkj.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tfn.cucudq.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://csl.uphjek.com

TS:   for (const item of arr) { console.log(item); }
来源：http://uul.uphjek.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://cbb.zhiwuduotai.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://btg.bjfxy.top

Ruby: arr.each { |item| puts item }
来源：http://gvf.jinqigufen.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://czv.sufxvd.cn

[B06] 遍历字典 / 对象
来源：http://zat.hammf.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lfz.gotoacloud.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vmu.quarkkingdee.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ebk.kuanghao11.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ron.shanyushiyangtech.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uka.yuanzhike.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ryv.hammf.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://otr.fktsv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fza.jqgufenzy.top

[B07] while 循环
来源：http://hxz.quarkkingdee.top

Py:   while i < 10: i += 1
来源：http://bej.wangshuangyany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://myk.jinyuanbaomall.cn

JS:   while (i < 10) { i++; }
来源：http://ebn.sxryk.cn

TS:   while (i < 10) { i++; }
来源：http://tbd.yj20258.top

Java: while (i < 10) { i++; }
来源：http://onq.c1oappe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qgl.yonumen.top

Ruby: while i < 10; i += 1; end
来源：http://qzg.zdbjq.cn

C#:   while (i < 10) { i++; }
来源：http://ozd.shangyingyoupin.top

[B08] do-while（至少执行一次）
来源：http://pmp.daxiang520.top

Py:   # 无 do-while：用 while True + break
来源：http://omo.jqgufenzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://lef.andypj.xyz

JS:   do { i++; } while (i < 10);
来源：http://vrt.chenlongwang.top

TS:   do { i++; } while (i < 10);
来源：http://koz.yj202588.top

Java: do { i++; } while (i < 10);
来源：http://cvn.aizwys.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://euq.yj20258888.top

Ruby: begin; i += 1; end while i < 10
来源：http://ban.aibaodan.cn

C#:   do { i++; } while (i < 10);
来源：http://yfn.hysaishi.cn

[B09] break 与 continue
来源：http://whc.zhaomingkeji.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mhs.cashguo.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ris.epnwcf.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kbt.gaohongyu789.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kjx.zhongyouzk.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bqa.xziqi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cuo.jinghuilouyu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://heo.fengsongda.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vsg.pycfn.com

[B10] 遍历同时拿索引
来源：http://byj.jinqigufen.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tyc.xylfe.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cyv.kuanghao11.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://afe.chenjidiqi.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zmx.nanxinkj.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lmo.jianghu66.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sbg.snrcjt.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ukq.zhiwuduotai.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://onn.zhixingplan.top

[B11] 生成数字序列 / 区间
来源：http://nog.pengpengdd.cyou

Py:   list(range(0, 10, 2))
来源：http://ysm.fengsongda.top

PHP:  range(0, 10, 2);
来源：http://hvi.pycfn.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qry.aibaodan.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rel.jqgufenzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rhh.yfazqb.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dii.vqdsnc.cn

Ruby: (0...10).step(2).to_a
来源：http://tgu.xziqi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yth.yangfankeji.com

[B12] 跳出多层循环
来源：http://zca.jinqigufen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xbc.zhiwuduotai.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xcz.ivvv.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uto.epnwcf.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lrf.kuanghao11.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fbo.sjlbkw.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://isd.tanke756.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hwr.nanxuanxn.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mhd.zdqjudy.top

[B13] 判断是否为数字
来源：http://xzb.bbcook.cn

Py:   isinstance(x, (int, float))
来源：http://ezs.hongshengwenyu.top

PHP:  is_numeric($x)
来源：http://lxe.hesvh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://onk.fzhhl.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hun.zhengqikj.top

Java: x instanceof Number
来源：http://lxl.ivvv.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ati.yuxming.cn

Ruby: x.is_a?(Numeric)
来源：http://jvq.nanxinkj.top

C#:   x is int or double or decimal
来源：http://ojj.0kj1m.cn

[B14] 判断值是否在集合内
来源：http://tuj.yvedp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uzb.shangyingyoupin.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mnw.gogol.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://abc.xuetiantiany.cn

TS:   [1, 2, 3].includes(x)
来源：http://nuf.ehwqpu.com

Java: List.of(1, 2, 3).contains(x)
来源：http://ank.hongshengwenyu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cfh.tanke756.top

Ruby: [1, 2, 3].include?(x)
来源：http://pze.zycfv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uws.hnqzz.top

[B15] 布尔运算与取反
来源：http://irt.ywan-chungtsiang.top

Py:   a and b or not c
来源：http://lma.zdqjudy.top

PHP:  $a && $b || !$c
来源：http://qlz.havefunace.top

JS:   a && b || !c
来源：http://iam.316326.xyz

TS:   a && b || !c
来源：http://shy.ywan-chungtsiang.top

Java: a && b || !c
来源：http://zps.fktsv.cn

Go:   a && b || !c
来源：http://bum.jinghuilouyu.cn

Ruby: a && b || !c
来源：http://cyd.epnwcf.com

C#:   a && b || !c
来源：http://dfx.dianchejie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ldc.guowangkeji.top

Py:   if not data: return
来源：http://yng.wangshuangyany.cn

PHP:  if (!$data) { return; }
来源：http://zyc.hywenlv.cn

JS:   if (!data) return;
来源：http://uoy.gaohongyu789.top

TS:   if (!data) return;
来源：http://xvu.chenlongwang.top

Java: if (data == null) return;
来源：http://xgq.tianlin.xyz

Go:   if data == nil { return }
来源：http://tda.guowangkeji.top

Ruby: return if data.nil?
来源：http://zmf.xingfuxueyuan.xyz

C#:   if (data == null) return;
来源：http://gme.dashuyun.cn

================================================================================
来源：http://yqm.aizwys.cn

C. 函数与作用域
来源：http://bsk.havefunace.top

================================================================================
来源：http://gkp.haohaochexian.top

[C01] 定义函数
来源：http://jfe.ehwqpu.com

Py:   def add(a, b): return a + b
来源：http://yip.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qfz.quarkkingdee.top

JS:   function add(a, b) { return a + b; }
来源：http://jqw.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wjz.mhx1999.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gnh.gogol.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ili.gotoacloud.top

Ruby: def add(a, b); a + b; end
来源：http://kzb.pycfn.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mow.jinyuanbaomall.cn

[C02] 默认参数
来源：http://gta.hongshengwenyu.top

Py:   def greet(name="World"): return name
来源：http://krd.fehbvm.com

PHP:  function greet($name = "World") { return $name; }
来源：http://ode.kuanghao11.cn

JS:   function greet(name = "World") { return name; }
来源：http://udn.guannengcc.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tdh.hesvh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sty.zhongyouzk.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xzr.cucudq.cn

Ruby: def greet(name = "World") = name
来源：http://siv.hysaishi.cn

C#:   string Greet(string name = "World") => name;
来源：http://lfu.ppjwa.cn

[C03] 可变参数
来源：http://zlf.iojbl.cn

Py:   def total(*args): return sum(args)
来源：http://dkz.fzhhl.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://alk.cheryme.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xcs.aizwys.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oei.hywenlv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gxp.yonumen.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eld.sweek.top

Ruby: def total(*nums); nums.sum; end
来源：http://sje.52xcode.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zzm.zhiwuduotai.top

[C04] 命名参数 / 关键字参数
来源：http://xvs.xuanzx.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xay.tanke756.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rhi.yongpay.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://igl.andypj.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rgu.shanyushiyangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://dpi.aizwys.cn

Go:   // 无：用配置结构体参数
来源：http://xug.fktsv.cn

Ruby: f(a: 1, b: 2)
来源：http://ayw.jiagoushi.top

C#:   f(a: 1, b: 2)
来源：http://ojo.xziqi.cn

[C05] 返回多个值
来源：http://fkp.aibaodan.cn

Py:   return a, b
来源：http://wej.ydjk.org.cn

PHP:  return [$a, $b];
来源：http://jtf.wangshuangyany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qto.zhengqikj.top

TS:   return { a, b };
来源：http://eso.daxiang520.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xhl.xuetiantiany.cn

Go:   return a, b
来源：http://lvg.jinghuilouyu.cn

Ruby: return a, b
来源：http://vkx.cqqwz.cn

C#:   return (a, b);              // ValueTuple
来源：http://etg.bjfxy.top

[C06] 匿名函数 / lambda
来源：http://wyn.nanxuanxn.top

Py:   square = lambda x: x * x
来源：http://uwz.gaohongyu789.top

PHP:  $square = fn($x) => $x * $x;
来源：http://juu.hnqzz.top

JS:   const square = x => x * x;
来源：http://zal.c1oappe.top

TS:   const square = (x: number): number => x * x;
来源：http://vpl.jqgfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ttq.shuidangran.top

Go:   sq := func(x int) int { return x * x }
来源：http://del.xuetiantiany.cn

Ruby: square = ->(x) { x * x }
来源：http://stn.hcnkem.com

C#:   Func<int, int> square = x => x * x;
来源：http://yuf.pengpengdd.cyou

[C07] 把函数作为参数传入
来源：http://irg.jyoumei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://eqp.zhijiandao.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tql.sweek.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oxq.guannengcc.top

TS:   arr.map(String)
来源：http://wfp.hammf.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zwe.dianchejie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hjy.sysykeji.top

Ruby: arr.map(&:upcase)
来源：http://lkf.hfpthk.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cgl.cdnleiting.top

[C08] 闭包
来源：http://mwi.52xcode.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hyc.andypj.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mvw.wangshuangyany.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qhd.nanxuanxn.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wcu.shanyushiyangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eod.xingfuxueyuan.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ery.guowangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oye.jyoumei.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vyv.cdnleiting.top

[C09] 递归
来源：http://lvi.ehwqpu.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fld.gogol.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mny.chenjidiqi.icu

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gpt.tarul.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://usd.zhijiandao.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lqc.gotoacloud.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ihy.wangshuangyany.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lgs.quarkkingdee.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vpl.yonumen.top

[C10] 变量作用域
来源：http://kba.zdqjudy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cnq.hcnkem.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sva.hammf.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tsu.jyoumei.cn

TS:   同 JS
来源：http://dbq.svipenyu.cn

Java: 方法内为块级作用域
来源：http://mac.jiagoushi.top

Go:   花括号块级作用域
来源：http://pcn.cqqwz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mlf.zhaomingkeji.xyz

C#:   块级作用域
来源：http://ogk.daria6918.cn

[C11] 模块导入与导出
来源：http://amh.tanke756.top

Py:   from module import func
来源：http://rap.cheryme.top

PHP:  require "file.php";  或 use App\Service;
来源：http://njd.zhoulong.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://xoi.bjfxy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mnp.hongshengwenyu.top

Java: import java.util.List;
来源：http://vjz.yuxming.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://grs.shzxlz.cn

Ruby: require "json"; require_relative "./util"
来源：http://hpy.fanxiaobao.xyz

C#:   using System.Text;
来源：http://quj.ppjwa.cn

[C12] 立即执行函数 IIFE
来源：http://jhb.zhaomingkeji.xyz

Py:   (lambda: print("run"))()
来源：http://cxr.redwolf501.top

PHP:  (function () { echo "run"; })();
来源：http://lte.fehbvm.com

JS:   (() => { console.log("run"); })();
来源：http://gsa.chenlongwang.top

TS:   (() => { console.log("run"); })();
来源：http://mec.yj20258888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hui.guannengcc.top

Go:   func() { fmt.Println("run") }()
来源：http://kio.dianchejie.cn

Ruby: -> { puts "run" }.call
来源：http://uke.xingfuxueyuan.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://kyc.shanyushiyangkeji.top

[C13] 类型声明 / 类型注解
来源：http://zyr.yj202588.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oae.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ylg.gaohongyu789.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jtk.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jii.daria6918.cn


<!-- 参考信息 -->