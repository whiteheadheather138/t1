代发 wailian999

TS:   s.length
来源：http://xcd.jianghu66.top

Java: s.length()
来源：http://bau.jinqigfzy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jfa.daxiang520.top

Ruby: s.length
来源：http://msh.sweek.top

C#:   s.Length
来源：http://ita.yanxiufei.cn

[A23] 大小写转换
来源：http://cdo.quarkkingdee.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ibb.yj20258.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nzz.yongpay.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://def.wangshuangyany.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hxi.zhixingplan.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zqw.cucudq.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nfy.cashguo.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://buo.havefunace.top

C#:   s.ToUpper(); s.ToLower()
来源：http://fuv.yongpay.top

[A24] 去除首尾空白
来源：http://xkc.ehwqpu.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qzo.jianghu66.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kfp.nwbrower.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wig.cashguo.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kwg.meibo888.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://klo.andypj.xyz

Go:   strings.TrimSpace(s)
来源：http://ddk.daxiang520.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oyp.gotoacloud.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nbu.xingfuxueyuan.xyz

[A25] 字符串比较
来源：http://opd.quarkkingdee.top

Py:   s1 == s2; s1 != s2
来源：http://eqs.jlsjyb.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zoo.xingfuxueyuan.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yuq.redwolf501.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yyz.mhx1999.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oej.smart0.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ggc.ppjwa.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hjx.fanxiaobao.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tfx.jinqigufen.top

[A26] 类型转换总览
来源：http://mly.hongshengwenyu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wjd.hywenlv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://srh.yuanzhike.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://beq.shzxlz.cn

TS:   Number() String() Boolean() x as number
来源：http://vfs.meibo888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://iie.xziqi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xlg.dianchejie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nej.yongpay.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dwd.fehbvm.com

================================================================================
来源：http://kpy.sufxvd.cn

B. 流程控制
来源：http://gsk.ctjpmb.com

================================================================================
来源：http://iph.wangshuangyany.cn

[B01] 条件判断 if / else
来源：http://etp.zhongyouzk.top

Py:   result = "正" if x > 0 else "非正"
来源：http://pxt.epnwcf.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jct.hysaishi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gbp.pengpengdd.cyou

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xfy.redwolf501.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://plg.bbcook.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vpo.zhengqikj.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jqn.quarkkingdee.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uot.ehwqpu.com

[B02] 多分支 else if / elif
来源：http://ygw.sysykeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kdm.vehdjk.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fxd.jqgufenzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tmc.jinyuanbaomall.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jug.gaohongyu789.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cbe.shangyingyoupin.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iqi.mhx1999.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xzs.pycfn.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rgr.tian-w.cn

[B03] switch / match / case
来源：http://dxf.cqqwz.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vht.zdbjq.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xmx.zhengqikj.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://alv.nanxuanxn.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tfi.hnxiangtu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://woy.chenlongwang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tpk.ywan-chungtsiang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wcg.redwolf501.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zbj.yueranfly.top

[B04] for 计数循环
来源：http://oju.meibo888.top

Py:   for i in range(10): print(i)
来源：http://vfd.quarkkingdee.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://riu.wangshuangyany.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cie.hfpthk.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://svs.mhx1999.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pil.xylfe.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jys.tian-w.cn

Ruby: 10.times { |i| puts i }
来源：http://xcv.sxryk.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cbx.wangshuangyany.cn

[B05] 遍历数组 / 列表
来源：http://dna.cashguo.top

Py:   for item in arr: print(item)
来源：http://azq.sufxvd.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gwl.xinyue.icu

JS:   for (const item of arr) { console.log(item); }
来源：http://rgr.zycfv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qgl.havefunace.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qut.hammf.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://aao.yj20258.top

Ruby: arr.each { |item| puts item }
来源：http://olw.yongpay.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gou.fzhhl.top

[B06] 遍历字典 / 对象
来源：http://jdo.wangdashe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rsz.chenjidiqi.icu

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wnt.hammf.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bub.yangfankeji.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hlf.jianghu66.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://stl.vqdsnc.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bjt.sufxvd.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://arw.yongpay.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://std.shuidangran.top

[B07] while 循环
来源：http://rcj.smart0.xyz

Py:   while i < 10: i += 1
来源：http://lsb.sysykeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://ygd.xylfe.cn

JS:   while (i < 10) { i++; }
来源：http://qmj.aizwys.cn

TS:   while (i < 10) { i++; }
来源：http://gaf.316326.xyz

Java: while (i < 10) { i++; }
来源：http://efs.ppjwa.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dpw.zdqjudy.top

Ruby: while i < 10; i += 1; end
来源：http://bna.hnxiangtu.top

C#:   while (i < 10) { i++; }
来源：http://iqm.yj20258.top

[B08] do-while（至少执行一次）
来源：http://yhd.vqdsnc.cn

Py:   # 无 do-while：用 while True + break
来源：http://cfm.ydzc1.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ins.snrcjt.cn

JS:   do { i++; } while (i < 10);
来源：http://ipj.jinqigfzy.top

TS:   do { i++; } while (i < 10);
来源：http://rqa.jqgufenzy.top

Java: do { i++; } while (i < 10);
来源：http://hnv.jqgfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hll.gzhubu.top

Ruby: begin; i += 1; end while i < 10
来源：http://tuo.shanyushiyangtech.top

C#:   do { i++; } while (i < 10);
来源：http://wlc.fktsv.cn

[B09] break 与 continue
来源：http://ets.sysykeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mkv.shanyushiyangtech.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bil.hesvh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://daq.zycfv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qtp.svipenyu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mbp.pycfn.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fgm.cqqwz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bar.jyoumei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wrf.cheryme.top

[B10] 遍历同时拿索引
来源：http://cvg.fzhhl.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yfi.yongpay.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fpz.wangdashe.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://igr.yj20258888.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ncz.zhongyouzk.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ojm.wangdashe.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wpf.yangfankeji.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qck.shanyushiyangkeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zlv.ywan-chungtsiang.top

[B11] 生成数字序列 / 区间
来源：http://fyc.fehbvm.com

Py:   list(range(0, 10, 2))
来源：http://bdm.zhixingplan.top

PHP:  range(0, 10, 2);
来源：http://sah.yfazqb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iyp.xinyue.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bmg.uphjek.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oef.chenlongwang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tke.quarkkingdee.top

Ruby: (0...10).step(2).to_a
来源：http://ovq.zdbjq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fgw.jlsjyb.cn

[B12] 跳出多层循环
来源：http://eam.chenlongwang.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://pps.gaohongyu789.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://tpr.guannengcc.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ikk.jinqigufen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gvr.tanke756.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://klb.fehbvm.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eep.epnwcf.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zqo.xuanzx.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nwq.tarul.cn

[B13] 判断是否为数字
来源：http://ddk.yuxming.cn

Py:   isinstance(x, (int, float))
来源：http://ykd.ydjk.org.cn

PHP:  is_numeric($x)
来源：http://kzj.0kj1m.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xcb.andypj.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nkr.redwolf501.top

Java: x instanceof Number
来源：http://vcu.sysykeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gzs.yanxiufei.cn

Ruby: x.is_a?(Numeric)
来源：http://rps.nwbrower.top

C#:   x is int or double or decimal
来源：http://btb.zhijiandao.cn

[B14] 判断值是否在集合内
来源：http://cjl.sweek.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vrd.jinyuanbaomall.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jya.sysykeji.top

JS:   [1, 2, 3].includes(x)
来源：http://psp.ydjk.org.cn

TS:   [1, 2, 3].includes(x)
来源：http://vri.daxiang520.top

Java: List.of(1, 2, 3).contains(x)
来源：http://qua.jinqigufen.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cnf.jianghu66.top

Ruby: [1, 2, 3].include?(x)
来源：http://ccq.cheryme.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wvu.nanxinkj.top

[B15] 布尔运算与取反
来源：http://ial.jinqigufen.top

Py:   a and b or not c
来源：http://lrs.vqdsnc.cn

PHP:  $a && $b || !$c
来源：http://fhs.jyoumei.cn

JS:   a && b || !c
来源：http://ftb.yj20258888.top

TS:   a && b || !c
来源：http://eve.uphjek.com

Java: a && b || !c
来源：http://jkg.nwbrower.top

Go:   a && b || !c
来源：http://fgh.nanxinkj.top

Ruby: a && b || !c
来源：http://jxy.smart0.xyz

C#:   a && b || !c
来源：http://ena.yueranfly.top

[B16] 卫语句：不满足条件提前返回
来源：http://wim.shanyushiyangkeji.top

Py:   if not data: return
来源：http://mlh.nanxinkj.top

PHP:  if (!$data) { return; }
来源：http://vmt.shuidangran.top

JS:   if (!data) return;
来源：http://ubm.wangdashe.top

TS:   if (!data) return;
来源：http://som.wangshuangyany.cn

Java: if (data == null) return;
来源：http://cwe.hammf.cn

Go:   if data == nil { return }
来源：http://zjp.yj202588.top

Ruby: return if data.nil?
来源：http://iip.zhijiandao.cn

C#:   if (data == null) return;
来源：http://nle.guannengcc.top

================================================================================
来源：http://qud.jqgufenzy.top

C. 函数与作用域
来源：http://ajm.fengsongda.top

================================================================================
来源：http://ouo.aibaodan.cn

[C01] 定义函数
来源：http://rhc.52xcode.cn

Py:   def add(a, b): return a + b
来源：http://gtc.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mdr.yangfankeji.com

JS:   function add(a, b) { return a + b; }
来源：http://mng.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ysg.meibo888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nfu.mhx1999.top

Go:   func add(a, b int) int { return a + b }
来源：http://npn.chenzaomai.com

Ruby: def add(a, b); a + b; end
来源：http://feb.shuidangran.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cdv.yangfankeji.com

[C02] 默认参数
来源：http://vef.yfazqb.com

Py:   def greet(name="World"): return name
来源：http://xor.fktsv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vsn.mhx1999.top

JS:   function greet(name = "World") { return name; }
来源：http://uvl.nanxinkj.top

TS:   function greet(name: string = "World") { return name; }
来源：http://soh.zhixingplan.top

Java: // 无默认参数：方法重载或 Optional
来源：http://aei.fanxiaobao.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gns.jyoumei.cn

Ruby: def greet(name = "World") = name
来源：http://akt.shanyushiyangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://pfj.svipenyu.cn

[C03] 可变参数
来源：http://lat.jinqigufen.top

Py:   def total(*args): return sum(args)
来源：http://moz.tarul.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bev.bjfxy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kpo.pengpengdd.cyou

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mom.smart0.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rvl.ppjwa.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oqq.cheryme.top

Ruby: def total(*nums); nums.sum; end
来源：http://apk.hongshengwenyu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://quj.tarul.cn

[C04] 命名参数 / 关键字参数
来源：http://uth.zdbjq.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ckn.guannengcc.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://stq.jqgfzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xlu.yuanzhike.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://api.ctjpmb.com

Java: // 无：用 Builder 模式或 record
来源：http://ckh.fzhhl.top

Go:   // 无：用配置结构体参数
来源：http://hvs.gotoacloud.top

Ruby: f(a: 1, b: 2)
来源：http://lmd.vehdjk.com

C#:   f(a: 1, b: 2)
来源：http://wgb.fanxiaobao.xyz

[C05] 返回多个值
来源：http://yba.yfazqb.com

Py:   return a, b
来源：http://lfe.havefunace.top

PHP:  return [$a, $b];
来源：http://bbr.hnqzz.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://aek.aizwys.cn

TS:   return { a, b };
来源：http://wgc.nanxinkj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rgf.shzxlz.cn

Go:   return a, b
来源：http://mbn.epnwcf.com

Ruby: return a, b
来源：http://oeb.c1oappe.top

C#:   return (a, b);              // ValueTuple
来源：http://pgp.hesvh.cn

[C06] 匿名函数 / lambda
来源：http://rht.fanxiaobao.xyz

Py:   square = lambda x: x * x
来源：http://mnl.zhixingplan.top

PHP:  $square = fn($x) => $x * $x;
来源：http://yxr.ydzc1.top

JS:   const square = x => x * x;
来源：http://usw.sufxvd.cn

TS:   const square = (x: number): number => x * x;
来源：http://hzx.fanxiaobao.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://phy.jinghuilouyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ime.jinqigfzy.top

Ruby: square = ->(x) { x * x }
来源：http://quc.ppjwa.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bhk.ydzc1.top

[C07] 把函数作为参数传入
来源：http://ims.9152youxi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ywo.feifeiyinyue.top

PHP:  array_map("strtoupper", $arr);
来源：http://dby.iojbl.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tjh.tanke756.top

TS:   arr.map(String)
来源：http://svp.hysaishi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zci.tanke756.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dru.cashguo.top

Ruby: arr.map(&:upcase)
来源：http://esf.zhengqikj.top

C#:   arr.Select(s => s.ToUpper())
来源：http://kxe.pengpengdd.cyou

[C08] 闭包
来源：http://upm.xinyue.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tpu.sjlbkw.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://afe.52xcode.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://awf.tanke756.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ica.xziqi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lgg.hcnkem.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://acb.nanxinkj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://upb.zdbjq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nqe.jinghuilouyu.cn

[C09] 递归
来源：http://nng.sxryk.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ttj.jqgfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sqv.jqgfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nsp.jinyuanbaomall.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fok.chenlongwang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tul.hywenlv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mux.quarkkingdee.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ppf.zhongyouzk.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://eka.shzxlz.cn

[C10] 变量作用域
来源：http://fdx.sxryk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zdj.sxryk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ajj.ydjk.org.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fgi.guannengcc.top

TS:   同 JS
来源：http://xis.jiagoushi.top

Java: 方法内为块级作用域
来源：http://sap.shanyushiyangtech.top

Go:   花括号块级作用域
来源：http://kqd.mhx1999.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rxp.aizwys.cn

C#:   块级作用域
来源：http://ovl.316326.xyz

[C11] 模块导入与导出
来源：http://pfq.chenlongwang.top

Py:   from module import func
来源：http://rzu.sweek.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fuy.sysykeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nnz.svipenyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xyr.chenlongwang.top

Java: import java.util.List;
来源：http://tgv.hongshengwenyu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://txg.shanyushiyangtech.top

Ruby: require "json"; require_relative "./util"
来源：http://brw.52xcode.cn

C#:   using System.Text;
来源：http://yru.hnqzz.top

[C12] 立即执行函数 IIFE
来源：http://jry.xuanzx.com

Py:   (lambda: print("run"))()
来源：http://cux.tian-w.cn

PHP:  (function () { echo "run"; })();
来源：http://wnb.redwolf501.top

JS:   (() => { console.log("run"); })();
来源：http://bwo.uphjek.com

TS:   (() => { console.log("run"); })();
来源：http://hct.bbcook.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jjg.tarul.cn

Go:   func() { fmt.Println("run") }()
来源：http://xmg.sysykeji.top

Ruby: -> { puts "run" }.call
来源：http://gui.hnxiangtu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://hbx.shanyushiyangtech.top

[C13] 类型声明 / 类型注解
来源：http://fey.jinyuanbaomall.cn


<!-- 参考信息 -->