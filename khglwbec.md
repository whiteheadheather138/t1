代发 wailian999

C#:   s.Length
来源：http://auj.nanxinkj.top

[A23] 大小写转换
来源：http://tad.bbcook.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vfo.feifeiyinyue.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pds.sxryk.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zii.zhengqikj.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://imi.vehdjk.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://uuu.hcnkem.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hvz.xingfuxueyuan.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mmg.zhijiandao.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://mdv.chenzaomai.com

[A24] 去除首尾空白
来源：http://avo.9152youxi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cvx.yueranfly.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ldt.guannengcc.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fxh.fktsv.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tyd.fehbvm.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nam.ivvv.top

Go:   strings.TrimSpace(s)
来源：http://ewv.hywenlv.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mmh.yj20258888.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jvl.sufxvd.cn

[A25] 字符串比较
来源：http://byg.jqgfzy.top

Py:   s1 == s2; s1 != s2
来源：http://ghu.cashguo.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cje.shuidangran.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xif.meibo888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rjn.guannengcc.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pgq.feifeiyinyue.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yfz.cashguo.top

Ruby: s1 == s2; s1 <=> s2
来源：http://igc.ydjk.org.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vxx.hammf.cn

[A26] 类型转换总览
来源：http://oqx.sufxvd.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vdx.jqgufenzy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xwh.chenlongwang.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://eqd.yonumen.top

TS:   Number() String() Boolean() x as number
来源：http://afe.tanke756.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://smf.sufxvd.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wvm.shangyingyoupin.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ina.xinyue.icu

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kzv.ctjpmb.com

================================================================================
来源：http://dqu.zhaomingkeji.xyz

B. 流程控制
来源：http://fhw.guowangkeji.top

================================================================================
来源：http://vnr.tarul.cn

[B01] 条件判断 if / else
来源：http://tta.daxiang520.top

Py:   result = "正" if x > 0 else "非正"
来源：http://mui.wangshuangyany.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vva.52xcode.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://umk.pengpengdd.cyou

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rvn.pengpengdd.cyou

Java: String r = x > 0 ? "正" : "非正";
来源：http://bgi.vehdjk.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dth.hongshengwenyu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vaw.xylfe.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cfs.dashuyun.cn

[B02] 多分支 else if / elif
来源：http://hpz.zhiwuduotai.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://urr.aibaodan.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fai.yj20258.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wnd.9152youxi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gtu.0kj1m.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hgi.jqgufenzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pmv.tanke756.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jum.jqgufenzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ehg.sufxvd.cn

[B03] switch / match / case
来源：http://qfg.tian-w.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://frw.sufxvd.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jkr.nanxuanxn.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mgj.hnqzz.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nkz.cashguo.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://utn.shangyingyoupin.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zaw.chenzaomai.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hid.jlsjyb.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://seg.yvedp.cn

[B04] for 计数循环
来源：http://ifv.nanxinkj.top

Py:   for i in range(10): print(i)
来源：http://ino.tianlin.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mgt.cdnleiting.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://agj.xziqi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ixq.snrcjt.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qlv.yangfankeji.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yll.smart0.xyz

Ruby: 10.times { |i| puts i }
来源：http://yzl.yj202588.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mho.zdqjudy.top

[B05] 遍历数组 / 列表
来源：http://aoy.daria6918.cn

Py:   for item in arr: print(item)
来源：http://dbl.jinqigfzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://evy.zhongyouzk.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vcj.bjfxy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://glq.cheryme.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rqd.52xcode.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wke.hywenlv.cn

Ruby: arr.each { |item| puts item }
来源：http://hjq.uphjek.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vbm.svipenyu.cn

[B06] 遍历字典 / 对象
来源：http://mgi.xuetiantiany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tpt.jyoumei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zoa.fehbvm.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://plj.jinqigufen.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gmp.hongshengwenyu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://aii.zhiwuduotai.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://snq.bbcook.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qdm.ydjk.org.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sdp.jqgfzy.top

[B07] while 循环
来源：http://jnc.gogol.net.cn

Py:   while i < 10: i += 1
来源：http://wmx.ehwqpu.com

PHP:  while ($i < 10) { $i++; }
来源：http://dbm.jinghuilouyu.cn

JS:   while (i < 10) { i++; }
来源：http://eko.shanyushiyangtech.top

TS:   while (i < 10) { i++; }
来源：http://vhq.andypj.xyz

Java: while (i < 10) { i++; }
来源：http://uas.gotoacloud.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wtd.vqdsnc.cn

Ruby: while i < 10; i += 1; end
来源：http://rne.zhixingplan.top

C#:   while (i < 10) { i++; }
来源：http://slz.hywenlv.cn

[B08] do-while（至少执行一次）
来源：http://vev.zhengqikj.top

Py:   # 无 do-while：用 while True + break
来源：http://jmh.vqdsnc.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gvz.jyoumei.cn

JS:   do { i++; } while (i < 10);
来源：http://iof.redwolf501.top

TS:   do { i++; } while (i < 10);
来源：http://csg.fengsongda.top

Java: do { i++; } while (i < 10);
来源：http://rrb.sufxvd.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rpg.yuxming.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hul.aibaodan.cn

C#:   do { i++; } while (i < 10);
来源：http://mpn.yuanzhike.top

[B09] break 与 continue
来源：http://bqa.52xcode.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://opu.ehwqpu.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://itu.epnwcf.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aof.sysykeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://byw.andypj.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ycs.zhixingplan.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bbo.hnxiangtu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uvv.gogol.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://djs.sxryk.cn

[B10] 遍历同时拿索引
来源：http://irt.shanyushiyangkeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://apd.ybcxt.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nmq.birdmap.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ybw.sxryk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ryp.zhiwuduotai.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://urz.yfazqb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hrv.shanyushiyangkeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ixt.ydzc1.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://quz.tianlin.xyz

[B11] 生成数字序列 / 区间
来源：http://yxc.cdnleiting.top

Py:   list(range(0, 10, 2))
来源：http://kyi.gaohongyu789.top

PHP:  range(0, 10, 2);
来源：http://rfk.epnwcf.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xwv.fehbvm.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hhb.zdqjudy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zth.sysykeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fsc.fengsongda.top

Ruby: (0...10).step(2).to_a
来源：http://axx.0kj1m.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yrk.cashguo.top

[B12] 跳出多层循环
来源：http://crv.hysaishi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ity.ctjpmb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://yvq.c1oappe.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://egb.vehdjk.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://knl.yj202588.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lmr.hnxiangtu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gmg.sxryk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dqo.jianghu66.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gzc.aizwys.cn

[B13] 判断是否为数字
来源：http://duz.ehwqpu.com

Py:   isinstance(x, (int, float))
来源：http://mol.yj20258.top

PHP:  is_numeric($x)
来源：http://lqb.gogol.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rrm.xinyue.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mur.ydzc1.top

Java: x instanceof Number
来源：http://ngt.sxryk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mfq.shzxlz.cn

Ruby: x.is_a?(Numeric)
来源：http://vwp.cashguo.top

C#:   x is int or double or decimal
来源：http://edc.hongshengwenyu.top

[B14] 判断值是否在集合内
来源：http://qwn.yonumen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ydg.yanxiufei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jar.sufxvd.cn

JS:   [1, 2, 3].includes(x)
来源：http://zyh.wangdashe.top

TS:   [1, 2, 3].includes(x)
来源：http://yre.hesvh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://uru.hcnkem.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wfm.ivvv.top

Ruby: [1, 2, 3].include?(x)
来源：http://tsj.tanke756.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nsi.ctjpmb.com

[B15] 布尔运算与取反
来源：http://rim.ydzc1.top

Py:   a and b or not c
来源：http://kxp.yfazqb.com

PHP:  $a && $b || !$c
来源：http://ihf.iojbl.cn

JS:   a && b || !c
来源：http://vyc.fengsongda.top

TS:   a && b || !c
来源：http://hyi.zdbjq.cn

Java: a && b || !c
来源：http://rfc.sufxvd.cn

Go:   a && b || !c
来源：http://qgn.sxryk.cn

Ruby: a && b || !c
来源：http://lix.vehdjk.com

C#:   a && b || !c
来源：http://dcy.feifeiyinyue.top

[B16] 卫语句：不满足条件提前返回
来源：http://bgh.nanxuanxn.top

Py:   if not data: return
来源：http://ubl.redwolf501.top

PHP:  if (!$data) { return; }
来源：http://nef.xylfe.cn

JS:   if (!data) return;
来源：http://lwp.aizwys.cn

TS:   if (!data) return;
来源：http://wjv.chenzaomai.com

Java: if (data == null) return;
来源：http://jhh.pycfn.com

Go:   if data == nil { return }
来源：http://tnw.shanyushiyangkeji.top

Ruby: return if data.nil?
来源：http://vmo.tian-w.cn

C#:   if (data == null) return;
来源：http://tvc.sufxvd.cn

================================================================================
来源：http://qvb.hywenlv.cn

C. 函数与作用域
来源：http://bas.jiagoushi.top

================================================================================
来源：http://wzw.andypj.xyz

[C01] 定义函数
来源：http://nrj.tarul.cn

Py:   def add(a, b): return a + b
来源：http://gbx.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://plg.jlsjyb.cn

JS:   function add(a, b) { return a + b; }
来源：http://gtl.hammf.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iwo.chenzaomai.com

Java: static int add(int a, int b) { return a + b; }
来源：http://vab.zhaomingkeji.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://dwm.nwbrower.top

Ruby: def add(a, b); a + b; end
来源：http://csk.sxryk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dfu.dianchejie.cn

[C02] 默认参数
来源：http://see.yuxming.cn

Py:   def greet(name="World"): return name
来源：http://ktm.ivvv.top

PHP:  function greet($name = "World") { return $name; }
来源：http://eac.chenlongwang.top

JS:   function greet(name = "World") { return name; }
来源：http://nge.meibo888.top

TS:   function greet(name: string = "World") { return name; }
来源：http://pcb.zdbjq.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hdq.jianghu66.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tss.yuxming.cn

Ruby: def greet(name = "World") = name
来源：http://fje.ctjpmb.com

C#:   string Greet(string name = "World") => name;
来源：http://yev.nwbrower.top

[C03] 可变参数
来源：http://jtk.yonumen.top

Py:   def total(*args): return sum(args)
来源：http://pew.hongshengwenyu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tga.yvedp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iia.xuetiantiany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hnd.meibo888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pvr.zhijiandao.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yyx.kuanghao11.cn

Ruby: def total(*nums); nums.sum; end
来源：http://etx.yongpay.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kla.jinyuanbaomall.cn

[C04] 命名参数 / 关键字参数
来源：http://qhn.52xcode.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zbu.nwbrower.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lzo.ydjk.org.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jwr.ywan-chungtsiang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://meg.9152youxi.cn

Java: // 无：用 Builder 模式或 record
来源：http://hyh.zhixingplan.top

Go:   // 无：用配置结构体参数
来源：http://oir.bjfxy.top

Ruby: f(a: 1, b: 2)
来源：http://rbe.ivvv.top

C#:   f(a: 1, b: 2)
来源：http://jhr.hcnkem.com

[C05] 返回多个值
来源：http://uay.meibo888.top

Py:   return a, b
来源：http://kqy.cdnleiting.top

PHP:  return [$a, $b];
来源：http://aai.iojbl.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sdi.bbcook.cn

TS:   return { a, b };
来源：http://ycs.hysaishi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://udn.zycfv.cn

Go:   return a, b
来源：http://ynj.shangyingyoupin.top

Ruby: return a, b
来源：http://myn.fzhhl.top

C#:   return (a, b);              // ValueTuple
来源：http://myv.havefunace.top

[C06] 匿名函数 / lambda
来源：http://qek.yj20258.top

Py:   square = lambda x: x * x
来源：http://gcd.xingfuxueyuan.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://ezw.fengsongda.top

JS:   const square = x => x * x;
来源：http://dvc.kuanghao11.cn

TS:   const square = (x: number): number => x * x;
来源：http://qvp.shzxlz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fxv.snrcjt.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fve.svipenyu.cn

Ruby: square = ->(x) { x * x }
来源：http://bvv.gzhubu.top

C#:   Func<int, int> square = x => x * x;
来源：http://ufg.jianghu66.top

[C07] 把函数作为参数传入
来源：http://sto.cashguo.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wgo.dianchejie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wwk.guannengcc.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hcp.zhaomingkeji.xyz

TS:   arr.map(String)
来源：http://xyk.nwbrower.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hpz.fktsv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hbb.shanyushiyangkeji.top

Ruby: arr.map(&:upcase)
来源：http://qnx.svipenyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://aqm.cdnleiting.top

[C08] 闭包
来源：http://mes.tianlin.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vkz.cqqwz.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vpl.cucudq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cgd.xingfuxueyuan.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cbo.aibaodan.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://asa.xylfe.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mox.xuetiantiany.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tlk.yueranfly.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://awp.ydzc1.top

[C09] 递归
来源：http://okx.dashuyun.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hot.jinqigfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wet.daxiang520.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zvs.yuanzhike.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://obu.gotoacloud.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gtw.zhengqikj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://llc.zhiwuduotai.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rqh.sjlbkw.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pfa.mhx1999.top

[C10] 变量作用域
来源：http://xnf.hfpthk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://utw.fktsv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ljw.svipenyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lqe.ivvv.top

TS:   同 JS
来源：http://gwv.hywenlv.cn

Java: 方法内为块级作用域
来源：http://yte.smart0.xyz

Go:   花括号块级作用域
来源：http://wrp.zdqjudy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://akj.zhengqikj.top

C#:   块级作用域
来源：http://bkq.pycfn.com

[C11] 模块导入与导出
来源：http://xry.mhx1999.top

Py:   from module import func
来源：http://ywr.yuanzhike.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jkg.jiagoushi.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vey.jinqigufen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://waa.daxiang520.top

Java: import java.util.List;
来源：http://rvg.c1oappe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jni.chenjidiqi.icu

Ruby: require "json"; require_relative "./util"
来源：http://ffb.ivvv.top

C#:   using System.Text;
来源：http://ows.quarkkingdee.top

[C12] 立即执行函数 IIFE
来源：http://vmi.chenzaomai.com

Py:   (lambda: print("run"))()
来源：http://xsh.snrcjt.cn

PHP:  (function () { echo "run"; })();
来源：http://onw.tanke756.top

JS:   (() => { console.log("run"); })();
来源：http://gww.zdqjudy.top

TS:   (() => { console.log("run"); })();
来源：http://ohb.zycfv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://web.jinqigfzy.top

Go:   func() { fmt.Println("run") }()
来源：http://xdt.sweek.top

Ruby: -> { puts "run" }.call
来源：http://tyk.sjlbkw.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rii.bbcook.cn

[C13] 类型声明 / 类型注解
来源：http://dfv.yvedp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yeb.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kec.shangyingyoupin.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://htc.zdbjq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gmi.yj20258888.top


<!-- 参考信息 -->