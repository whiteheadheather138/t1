代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bjz.fanxiaobao.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://vhz.jqgufenzy.top

[A24] 去除首尾空白
来源：http://cyo.cheryme.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qsx.vqdsnc.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wub.zdqjudy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xdq.quarkkingdee.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hek.yuxming.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tku.nwbrower.top

Go:   strings.TrimSpace(s)
来源：http://qwh.zhoulong.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vhu.nanxinkj.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yvf.guannengcc.top

[A25] 字符串比较
来源：http://vft.yj20258.top

Py:   s1 == s2; s1 != s2
来源：http://yql.birdmap.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vwp.hfpthk.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fsk.ehwqpu.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rvy.hysaishi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tbp.cucudq.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://grq.cdnleiting.top

Ruby: s1 == s2; s1 <=> s2
来源：http://fwm.hesvh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://day.sufxvd.cn

[A26] 类型转换总览
来源：http://muh.cashguo.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hsg.ctjpmb.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://erw.hongshengwenyu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://veb.jlsjyb.cn

TS:   Number() String() Boolean() x as number
来源：http://puy.iojbl.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ymp.nanxinkj.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zwn.jinqigufen.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://aqq.ppjwa.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qeg.ybcxt.top

================================================================================
来源：http://kzg.gogol.net.cn

B. 流程控制
来源：http://mii.daxiang520.top

================================================================================
来源：http://nir.yj20258888.top

[B01] 条件判断 if / else
来源：http://nlc.pengpengdd.cyou

Py:   result = "正" if x > 0 else "非正"
来源：http://lue.jqgufenzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qnt.ydzc1.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://koq.aizwys.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kmc.jiagoushi.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://hvs.hesvh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lcj.shzxlz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tpq.vqdsnc.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nxw.cheryme.top

[B02] 多分支 else if / elif
来源：http://qcg.shzxlz.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nzp.ppjwa.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nrl.meibo888.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nmv.zhaomingkeji.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nzi.shanyushiyangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gxt.ivvv.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qct.hysaishi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qkp.xinyue.icu

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mwt.vqdsnc.cn

[B03] switch / match / case
来源：http://cin.bjfxy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xmd.yuanzhike.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nnd.ydzc1.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pji.pengpengdd.cyou

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rhi.jinyuanbaomall.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rsi.pycfn.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lgs.pengpengdd.cyou

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qcw.zhijiandao.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ffg.xingfuxueyuan.xyz

[B04] for 计数循环
来源：http://xah.yanxiufei.cn

Py:   for i in range(10): print(i)
来源：http://qeq.ppjwa.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xpn.vqdsnc.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cca.hnxiangtu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hpd.mhx1999.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wnf.hysaishi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mow.redwolf501.top

Ruby: 10.times { |i| puts i }
来源：http://nxi.hcnkem.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nyf.sjlbkw.cn

[B05] 遍历数组 / 列表
来源：http://xzf.sjlbkw.cn

Py:   for item in arr: print(item)
来源：http://qph.hammf.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kdz.shuidangran.top

JS:   for (const item of arr) { console.log(item); }
来源：http://jki.vqdsnc.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hua.yangfankeji.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://vnq.fengsongda.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bmt.tarul.cn

Ruby: arr.each { |item| puts item }
来源：http://pqu.yuanzhike.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xqu.gotoacloud.top

[B06] 遍历字典 / 对象
来源：http://spp.yj20258888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://srb.gzhubu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ble.c1oappe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vdl.yj20258.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kek.jqgfzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sox.yuanzhike.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sqr.fktsv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bej.fehbvm.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xkd.nwbrower.top

[B07] while 循环
来源：http://yct.hongshengwenyu.top

Py:   while i < 10: i += 1
来源：http://les.tarul.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ytw.andypj.xyz

JS:   while (i < 10) { i++; }
来源：http://mny.yueranfly.top

TS:   while (i < 10) { i++; }
来源：http://csj.zhongyouzk.top

Java: while (i < 10) { i++; }
来源：http://oio.jlsjyb.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fcm.gzhubu.top

Ruby: while i < 10; i += 1; end
来源：http://ele.pycfn.com

C#:   while (i < 10) { i++; }
来源：http://bhq.jinqigfzy.top

[B08] do-while（至少执行一次）
来源：http://udz.snrcjt.cn

Py:   # 无 do-while：用 while True + break
来源：http://tgt.pengpengdd.cyou

PHP:  do { $i++; } while ($i < 10);
来源：http://bdz.cucudq.cn

JS:   do { i++; } while (i < 10);
来源：http://asy.hcnkem.com

TS:   do { i++; } while (i < 10);
来源：http://wvt.wangdashe.top

Java: do { i++; } while (i < 10);
来源：http://mbq.zycfv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vni.zdqjudy.top

Ruby: begin; i += 1; end while i < 10
来源：http://dij.sjlbkw.cn

C#:   do { i++; } while (i < 10);
来源：http://mom.shzxlz.cn

[B09] break 与 continue
来源：http://bne.ehwqpu.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://txp.sxryk.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xjb.kuanghao11.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fwe.sjlbkw.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://msc.zhongyouzk.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blh.hnxiangtu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://llq.hnxiangtu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nqt.zhiwuduotai.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cpg.dianchejie.cn

[B10] 遍历同时拿索引
来源：http://mtz.xziqi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hdq.cdnleiting.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zcj.jinqigufen.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rtg.epnwcf.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rvz.yj20258.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aup.fktsv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ohy.ybcxt.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://epl.pycfn.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mqk.daria6918.cn

[B11] 生成数字序列 / 区间
来源：http://uug.yj20258.top

Py:   list(range(0, 10, 2))
来源：http://byz.yueranfly.top

PHP:  range(0, 10, 2);
来源：http://czj.jinqigfzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gcw.zhijiandao.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oql.sufxvd.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rwt.ivvv.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://euy.cheryme.top

Ruby: (0...10).step(2).to_a
来源：http://ikn.shangyingyoupin.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ekx.gotoacloud.top

[B12] 跳出多层循环
来源：http://xxj.gotoacloud.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kbt.havefunace.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://wyj.andypj.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sho.meibo888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qng.snrcjt.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wgz.xuetiantiany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pxr.yvedp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gsf.yj20258888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://olu.hywenlv.cn

[B13] 判断是否为数字
来源：http://wlv.xziqi.cn

Py:   isinstance(x, (int, float))
来源：http://pvm.nwbrower.top

PHP:  is_numeric($x)
来源：http://odj.fehbvm.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hdo.ydzc1.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ati.yonumen.top

Java: x instanceof Number
来源：http://vyh.smart0.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fnp.shzxlz.cn

Ruby: x.is_a?(Numeric)
来源：http://byb.yj20258888.top

C#:   x is int or double or decimal
来源：http://itk.zhoulong.xyz

[B14] 判断值是否在集合内
来源：http://fuf.daria6918.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zea.yuxming.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uli.52xcode.cn

JS:   [1, 2, 3].includes(x)
来源：http://vtd.yj202588.top

TS:   [1, 2, 3].includes(x)
来源：http://wge.zdbjq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mnr.redwolf501.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pca.epnwcf.com

Ruby: [1, 2, 3].include?(x)
来源：http://zws.jinyuanbaomall.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nqx.fzhhl.top

[B15] 布尔运算与取反
来源：http://sza.jiagoushi.top

Py:   a and b or not c
来源：http://ayn.hfpthk.cn

PHP:  $a && $b || !$c
来源：http://gnp.aibaodan.cn

JS:   a && b || !c
来源：http://umo.hfpthk.cn

TS:   a && b || !c
来源：http://irc.hnqzz.top

Java: a && b || !c
来源：http://uuw.hcnkem.com

Go:   a && b || !c
来源：http://yve.hcnkem.com

Ruby: a && b || !c
来源：http://omn.kuanghao11.cn

C#:   a && b || !c
来源：http://eaq.shuidangran.top

[B16] 卫语句：不满足条件提前返回
来源：http://sxp.feifeiyinyue.top

Py:   if not data: return
来源：http://tbd.ctjpmb.com

PHP:  if (!$data) { return; }
来源：http://mgi.hongshengwenyu.top

JS:   if (!data) return;
来源：http://lco.ppjwa.cn

TS:   if (!data) return;
来源：http://pgy.cdnleiting.top

Java: if (data == null) return;
来源：http://ufz.bbcook.cn

Go:   if data == nil { return }
来源：http://eex.sxryk.cn

Ruby: return if data.nil?
来源：http://jyf.hnqzz.top

C#:   if (data == null) return;
来源：http://nyd.uphjek.com

================================================================================
来源：http://kdr.hysaishi.cn

C. 函数与作用域
来源：http://acf.wangdashe.top

================================================================================
来源：http://wkw.cashguo.top

[C01] 定义函数
来源：http://rfy.jinqigfzy.top

Py:   def add(a, b): return a + b
来源：http://tpu.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zig.snrcjt.cn

JS:   function add(a, b) { return a + b; }
来源：http://wrh.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uqz.daxiang520.top

Java: static int add(int a, int b) { return a + b; }
来源：http://snz.ivvv.top

Go:   func add(a, b int) int { return a + b }
来源：http://mhl.pengpengdd.cyou

Ruby: def add(a, b); a + b; end
来源：http://eum.tianlin.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zla.zhixingplan.top

[C02] 默认参数
来源：http://jdd.jinqigufen.top

Py:   def greet(name="World"): return name
来源：http://ydf.52xcode.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://eqt.zhongyouzk.top

JS:   function greet(name = "World") { return name; }
来源：http://nvl.hnxiangtu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://wxg.shangyingyoupin.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xzy.ctjpmb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rsn.yj20258888.top

Ruby: def greet(name = "World") = name
来源：http://jfn.ybcxt.top

C#:   string Greet(string name = "World") => name;
来源：http://lwn.zdbjq.cn

[C03] 可变参数
来源：http://rwu.bbcook.cn

Py:   def total(*args): return sum(args)
来源：http://tof.cashguo.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qdq.gotoacloud.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ctu.yonumen.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qcl.yueranfly.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ytd.316326.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zxu.hfpthk.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nhx.yj202588.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vdh.yvedp.cn

[C04] 命名参数 / 关键字参数
来源：http://dqh.xingfuxueyuan.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://brh.daria6918.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pmz.smart0.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://drm.jlsjyb.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pck.sxryk.cn

Java: // 无：用 Builder 模式或 record
来源：http://elc.daxiang520.top

Go:   // 无：用配置结构体参数
来源：http://lio.aibaodan.cn

Ruby: f(a: 1, b: 2)
来源：http://pio.xuanzx.com

C#:   f(a: 1, b: 2)
来源：http://pfq.zhijiandao.cn

[C05] 返回多个值
来源：http://hld.0kj1m.cn

Py:   return a, b
来源：http://qha.sufxvd.cn

PHP:  return [$a, $b];
来源：http://njr.xingfuxueyuan.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://gmb.uphjek.com

TS:   return { a, b };
来源：http://els.sxryk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rop.fzhhl.top

Go:   return a, b
来源：http://zxm.chenzaomai.com

Ruby: return a, b
来源：http://ckd.fehbvm.com

C#:   return (a, b);              // ValueTuple
来源：http://tqz.tarul.cn

[C06] 匿名函数 / lambda
来源：http://iij.52xcode.cn

Py:   square = lambda x: x * x
来源：http://kof.hammf.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://djy.chenjidiqi.icu

JS:   const square = x => x * x;
来源：http://ppi.chenlongwang.top

TS:   const square = (x: number): number => x * x;
来源：http://fuq.ctjpmb.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xne.guannengcc.top

Go:   sq := func(x int) int { return x * x }
来源：http://gha.yfazqb.com

Ruby: square = ->(x) { x * x }
来源：http://rcq.yj20258888.top

C#:   Func<int, int> square = x => x * x;
来源：http://vas.daria6918.cn

[C07] 把函数作为参数传入
来源：http://aba.shanyushiyangkeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mid.redwolf501.top

PHP:  array_map("strtoupper", $arr);
来源：http://pmz.nanxinkj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zpc.daxiang520.top

TS:   arr.map(String)
来源：http://itm.wangdashe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kaj.jqgfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zvu.hnxiangtu.top

Ruby: arr.map(&:upcase)
来源：http://gfl.pengpengdd.cyou

C#:   arr.Select(s => s.ToUpper())
来源：http://nyd.tianlin.xyz

[C08] 闭包
来源：http://fom.pycfn.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zqd.guowangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vyh.yuanzhike.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fhl.zycfv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://eok.aibaodan.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vcr.yj202588.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qmt.ctjpmb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mhp.quarkkingdee.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://udc.sjlbkw.cn

[C09] 递归
来源：http://ojf.uphjek.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ehh.hongshengwenyu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zux.jinyuanbaomall.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ymq.jinqigfzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uqa.dianchejie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mbb.hysaishi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iau.bjfxy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://afn.xuanzx.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rhf.yonumen.top

[C10] 变量作用域
来源：http://bsb.xuetiantiany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wph.tianlin.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kqd.yvedp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nbd.sxryk.cn

TS:   同 JS
来源：http://bsd.yanxiufei.cn

Java: 方法内为块级作用域
来源：http://qjv.chenzaomai.com

Go:   花括号块级作用域
来源：http://gyl.tanke756.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mnk.yanxiufei.cn

C#:   块级作用域
来源：http://bav.ctjpmb.com

[C11] 模块导入与导出
来源：http://dkm.ctjpmb.com

Py:   from module import func
来源：http://zlm.bbcook.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://aeg.vqdsnc.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qpe.gotoacloud.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bxf.ybcxt.top

Java: import java.util.List;
来源：http://kqx.316326.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uyh.xziqi.cn

Ruby: require "json"; require_relative "./util"
来源：http://npg.shanyushiyangtech.top

C#:   using System.Text;
来源：http://wat.yj20258.top

[C12] 立即执行函数 IIFE
来源：http://pzb.yj20258.top

Py:   (lambda: print("run"))()
来源：http://qvj.vehdjk.com

PHP:  (function () { echo "run"; })();
来源：http://zwj.jqgfzy.top

JS:   (() => { console.log("run"); })();
来源：http://kqk.ywan-chungtsiang.top

TS:   (() => { console.log("run"); })();
来源：http://zbq.sjlbkw.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wys.jinyuanbaomall.cn

Go:   func() { fmt.Println("run") }()
来源：http://eat.hywenlv.cn

Ruby: -> { puts "run" }.call
来源：http://geh.shzxlz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://inc.uphjek.com

[C13] 类型声明 / 类型注解
来源：http://ckd.yj20258888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dlz.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yhp.hnqzz.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ivc.xziqi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rvj.yj202588.top

Java: int add(int a, int b) { return a + b; }
来源：http://xgp.gaohongyu789.top

Go:   func add(a, b int) int
来源：http://vlb.hfpthk.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wkt.aibaodan.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gvo.xziqi.cn

[C14] 泛型函数
来源：http://rij.wangshuangyany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vet.yvedp.cn

PHP:  // 无泛型
来源：http://aco.jyoumei.cn

JS:   // 无泛型
来源：http://tiq.iojbl.cn


<!-- 参考信息 -->