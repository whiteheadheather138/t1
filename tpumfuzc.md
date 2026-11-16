代发 wailian999

C#:   s.Length
来源：http://ele.ydzc1.top

[A23] 大小写转换
来源：http://zzv.shanyushiyangtech.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ilb.wangdashe.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gip.xinyue.icu

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://khz.fehbvm.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cxa.yvedp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vqo.chenjidiqi.icu

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ebu.pengpengdd.cyou

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dyu.yonumen.top

C#:   s.ToUpper(); s.ToLower()
来源：http://kvf.hfpthk.cn

[A24] 去除首尾空白
来源：http://ldb.yj20258.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://smp.jianghu66.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cgr.sweek.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dbd.kuanghao11.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ezi.ydzc1.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dtg.vqdsnc.cn

Go:   strings.TrimSpace(s)
来源：http://epi.xuanzx.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gjo.zhijiandao.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://egt.bbcook.cn

[A25] 字符串比较
来源：http://jtd.yj20258888.top

Py:   s1 == s2; s1 != s2
来源：http://bof.cqqwz.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qhg.fengsongda.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sno.ehwqpu.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kyo.yonumen.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rnn.tarul.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hxp.cucudq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://elr.aibaodan.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pju.ppjwa.cn

[A26] 类型转换总览
来源：http://gyi.zhoulong.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yft.gogol.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bjg.yanxiufei.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tug.redwolf501.top

TS:   Number() String() Boolean() x as number
来源：http://maq.tanke756.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sfj.sweek.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qbx.uphjek.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://grz.gogol.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wxn.pycfn.com

================================================================================
来源：http://lvb.hcnkem.com

B. 流程控制
来源：http://wzq.tanke756.top

================================================================================
来源：http://los.316326.xyz

[B01] 条件判断 if / else
来源：http://xay.vqdsnc.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zvv.hywenlv.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ldd.mhx1999.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xau.hcnkem.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://amq.zhoulong.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://sru.hammf.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fso.cucudq.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rnk.nwbrower.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dvm.cqqwz.cn

[B02] 多分支 else if / elif
来源：http://ryh.tanke756.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pdx.ehwqpu.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qrn.sysykeji.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dht.cashguo.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uck.hesvh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ngw.ywan-chungtsiang.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mto.cucudq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rlv.tanke756.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iln.jqgfzy.top

[B03] switch / match / case
来源：http://xuo.shangyingyoupin.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pqu.wangdashe.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://afu.chenjidiqi.icu

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zuf.yanxiufei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bos.cucudq.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gyr.fanxiaobao.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gpq.xylfe.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pez.jianghu66.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ogh.jlsjyb.cn

[B04] for 计数循环
来源：http://jmt.uphjek.com

Py:   for i in range(10): print(i)
来源：http://xrc.0kj1m.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mpw.ctjpmb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uso.sweek.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jwv.0kj1m.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hgd.dashuyun.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ywu.andypj.xyz

Ruby: 10.times { |i| puts i }
来源：http://uyw.zhijiandao.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dmb.shanyushiyangkeji.top

[B05] 遍历数组 / 列表
来源：http://eyd.shangyingyoupin.top

Py:   for item in arr: print(item)
来源：http://xic.hnxiangtu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zdy.tianlin.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://mir.cashguo.top

TS:   for (const item of arr) { console.log(item); }
来源：http://exc.gaohongyu789.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://bld.fzhhl.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lsa.jinyuanbaomall.cn

Ruby: arr.each { |item| puts item }
来源：http://jpx.smart0.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://phw.jinyuanbaomall.cn

[B06] 遍历字典 / 对象
来源：http://mvr.shanyushiyangkeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xgl.havefunace.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://esk.hywenlv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eop.yangfankeji.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://app.xylfe.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bja.tian-w.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wqq.yj20258888.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jgs.gogol.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xkl.sweek.top

[B07] while 循环
来源：http://upe.sxryk.cn

Py:   while i < 10: i += 1
来源：http://bzu.ehwqpu.com

PHP:  while ($i < 10) { $i++; }
来源：http://wmr.vqdsnc.cn

JS:   while (i < 10) { i++; }
来源：http://dxx.jiagoushi.top

TS:   while (i < 10) { i++; }
来源：http://zds.kuanghao11.cn

Java: while (i < 10) { i++; }
来源：http://sib.gaohongyu789.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://teh.ybcxt.top

Ruby: while i < 10; i += 1; end
来源：http://rpf.zdqjudy.top

C#:   while (i < 10) { i++; }
来源：http://edy.birdmap.top

[B08] do-while（至少执行一次）
来源：http://pdo.nanxuanxn.top

Py:   # 无 do-while：用 while True + break
来源：http://oix.yj20258888.top

PHP:  do { $i++; } while ($i < 10);
来源：http://eis.jinqigfzy.top

JS:   do { i++; } while (i < 10);
来源：http://ihg.chenzaomai.com

TS:   do { i++; } while (i < 10);
来源：http://knh.nanxinkj.top

Java: do { i++; } while (i < 10);
来源：http://umf.fanxiaobao.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://pqs.hesvh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nmv.sysykeji.top

C#:   do { i++; } while (i < 10);
来源：http://upn.yonumen.top

[B09] break 与 continue
来源：http://arv.pycfn.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ohl.tarul.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dkr.zhoulong.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ktf.yvedp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://now.hnqzz.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uzp.tanke756.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gvo.yangfankeji.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dze.zycfv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jji.yuxming.cn

[B10] 遍历同时拿索引
来源：http://yia.hnxiangtu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://szi.ywan-chungtsiang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nqn.hesvh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://elu.fktsv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cdf.chenzaomai.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://eob.shangyingyoupin.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://amy.fengsongda.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vvx.jinqigufen.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gkb.zhoulong.xyz

[B11] 生成数字序列 / 区间
来源：http://tai.zhoulong.xyz

Py:   list(range(0, 10, 2))
来源：http://txg.sjlbkw.cn

PHP:  range(0, 10, 2);
来源：http://ala.9152youxi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fwb.yangfankeji.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://chm.hysaishi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gpd.tarul.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://byo.xingfuxueyuan.xyz

Ruby: (0...10).step(2).to_a
来源：http://zcm.nwbrower.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mab.xylfe.cn

[B12] 跳出多层循环
来源：http://mnm.daxiang520.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://slj.gaohongyu789.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://gcu.xinyue.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kpj.svipenyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nrr.guannengcc.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hyl.havefunace.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kvg.0kj1m.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vzq.fzhhl.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dgu.birdmap.top

[B13] 判断是否为数字
来源：http://mlh.mhx1999.top

Py:   isinstance(x, (int, float))
来源：http://ltz.0kj1m.cn

PHP:  is_numeric($x)
来源：http://klb.ppjwa.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://smh.ivvv.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jof.chenjidiqi.icu

Java: x instanceof Number
来源：http://mnv.52xcode.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://foo.feifeiyinyue.top

Ruby: x.is_a?(Numeric)
来源：http://cyq.hammf.cn

C#:   x is int or double or decimal
来源：http://sfz.ppjwa.cn

[B14] 判断值是否在集合内
来源：http://sbq.gzhubu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xqc.nanxuanxn.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tic.zycfv.cn

JS:   [1, 2, 3].includes(x)
来源：http://aiy.jinghuilouyu.cn

TS:   [1, 2, 3].includes(x)
来源：http://rrx.shanyushiyangkeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mxc.wangdashe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ikv.vqdsnc.cn

Ruby: [1, 2, 3].include?(x)
来源：http://oee.gaohongyu789.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vxu.yuxming.cn

[B15] 布尔运算与取反
来源：http://oeq.haohaochexian.top

Py:   a and b or not c
来源：http://eqo.wangshuangyany.cn

PHP:  $a && $b || !$c
来源：http://yun.tianlin.xyz

JS:   a && b || !c
来源：http://lbv.cheryme.top

TS:   a && b || !c
来源：http://zis.nwbrower.top

Java: a && b || !c
来源：http://uyo.sjlbkw.cn

Go:   a && b || !c
来源：http://zxt.ydjk.org.cn

Ruby: a && b || !c
来源：http://lmo.kuanghao11.cn

C#:   a && b || !c
来源：http://wfm.jinyuanbaomall.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cin.zycfv.cn

Py:   if not data: return
来源：http://jfd.wangdashe.top

PHP:  if (!$data) { return; }
来源：http://ann.meibo888.top

JS:   if (!data) return;
来源：http://tva.cdnleiting.top

TS:   if (!data) return;
来源：http://xpp.jinqigufen.top

Java: if (data == null) return;
来源：http://uco.xuanzx.com

Go:   if data == nil { return }
来源：http://kcf.shzxlz.cn

Ruby: return if data.nil?
来源：http://ryk.wangdashe.top

C#:   if (data == null) return;
来源：http://rby.sjlbkw.cn

================================================================================
来源：http://qbq.dashuyun.cn

C. 函数与作用域
来源：http://psk.sxryk.cn

================================================================================
来源：http://mzu.bbcook.cn

[C01] 定义函数
来源：http://amb.smart0.xyz

Py:   def add(a, b): return a + b
来源：http://uma.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bco.pycfn.com

JS:   function add(a, b) { return a + b; }
来源：http://ngq.svipenyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kol.sysykeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://yea.9152youxi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tto.shangyingyoupin.top

Ruby: def add(a, b); a + b; end
来源：http://frp.zhijiandao.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vkf.feifeiyinyue.top

[C02] 默认参数
来源：http://mvs.mhx1999.top

Py:   def greet(name="World"): return name
来源：http://aty.pycfn.com

PHP:  function greet($name = "World") { return $name; }
来源：http://jir.jinghuilouyu.cn

JS:   function greet(name = "World") { return name; }
来源：http://oon.c1oappe.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lym.jyoumei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://oec.jyoumei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://trm.xziqi.cn

Ruby: def greet(name = "World") = name
来源：http://ddi.fzhhl.top

C#:   string Greet(string name = "World") => name;
来源：http://cpr.sweek.top

[C03] 可变参数
来源：http://nbt.xuetiantiany.cn

Py:   def total(*args): return sum(args)
来源：http://wly.jyoumei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yqw.gzhubu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iwv.ybcxt.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ynf.yj20258888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ron.yfazqb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eef.zhengqikj.top

Ruby: def total(*nums); nums.sum; end
来源：http://klm.pengpengdd.cyou

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tkv.yonumen.top

[C04] 命名参数 / 关键字参数
来源：http://zdy.zhiwuduotai.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sbf.xziqi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ziv.zdqjudy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yok.hnqzz.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jkq.hywenlv.cn

Java: // 无：用 Builder 模式或 record
来源：http://zap.hfpthk.cn

Go:   // 无：用配置结构体参数
来源：http://bnj.sysykeji.top

Ruby: f(a: 1, b: 2)
来源：http://rea.jlsjyb.cn

C#:   f(a: 1, b: 2)
来源：http://emd.ywan-chungtsiang.top

[C05] 返回多个值
来源：http://ryd.xylfe.cn

Py:   return a, b
来源：http://onl.pengpengdd.cyou

PHP:  return [$a, $b];
来源：http://dqg.hcnkem.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://rin.shzxlz.cn

TS:   return { a, b };
来源：http://kxi.zhongyouzk.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pyk.jlsjyb.cn

Go:   return a, b
来源：http://jwv.hywenlv.cn

Ruby: return a, b
来源：http://kte.c1oappe.top

C#:   return (a, b);              // ValueTuple
来源：http://rrg.yangfankeji.com

[C06] 匿名函数 / lambda
来源：http://zvf.gotoacloud.top

Py:   square = lambda x: x * x
来源：http://ddv.hnqzz.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rah.nanxinkj.top

JS:   const square = x => x * x;
来源：http://ljy.redwolf501.top

TS:   const square = (x: number): number => x * x;
来源：http://srk.zhoulong.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://svc.sufxvd.cn

Go:   sq := func(x int) int { return x * x }
来源：http://etv.aizwys.cn

Ruby: square = ->(x) { x * x }
来源：http://nrl.jqgufenzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://jvg.haohaochexian.top

[C07] 把函数作为参数传入
来源：http://nit.ydjk.org.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://whl.hongshengwenyu.top

PHP:  array_map("strtoupper", $arr);
来源：http://dez.chenjidiqi.icu

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ior.tian-w.cn

TS:   arr.map(String)
来源：http://ips.jinqigufen.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xrl.xylfe.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ipy.uphjek.com

Ruby: arr.map(&:upcase)
来源：http://ifb.zhengqikj.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ttx.tianlin.xyz

[C08] 闭包
来源：http://vem.zycfv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uuc.tian-w.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ndl.cdnleiting.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mue.zhengqikj.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pnk.ppjwa.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dhk.shanyushiyangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://azv.nanxuanxn.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://poq.jqgufenzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ecy.fehbvm.com

[C09] 递归
来源：http://nrb.jqgfzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fgd.tanke756.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rnt.zdbjq.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fru.nanxinkj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rzn.vehdjk.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qby.hammf.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rla.xylfe.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ovx.xinyue.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mje.fktsv.cn

[C10] 变量作用域
来源：http://apt.shanyushiyangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hmc.bjfxy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://edr.pengpengdd.cyou

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nmg.shzxlz.cn

TS:   同 JS
来源：http://bvt.sxryk.cn

Java: 方法内为块级作用域
来源：http://mnw.cqqwz.cn

Go:   花括号块级作用域
来源：http://hhn.mhx1999.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jcn.vqdsnc.cn

C#:   块级作用域
来源：http://ixk.nanxuanxn.top

[C11] 模块导入与导出
来源：http://lvp.vqdsnc.cn

Py:   from module import func
来源：http://fdv.fktsv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hra.zhongyouzk.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ukm.feifeiyinyue.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yab.fzhhl.top

Java: import java.util.List;
来源：http://dmh.fanxiaobao.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ubi.snrcjt.cn

Ruby: require "json"; require_relative "./util"
来源：http://pmv.zdbjq.cn

C#:   using System.Text;
来源：http://whh.zdbjq.cn

[C12] 立即执行函数 IIFE
来源：http://fsn.wangdashe.top

Py:   (lambda: print("run"))()
来源：http://wks.cqqwz.cn

PHP:  (function () { echo "run"; })();
来源：http://oyk.epnwcf.com

JS:   (() => { console.log("run"); })();
来源：http://mqi.nanxinkj.top

TS:   (() => { console.log("run"); })();
来源：http://rtu.aizwys.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yyc.snrcjt.cn

Go:   func() { fmt.Println("run") }()
来源：http://juc.316326.xyz

Ruby: -> { puts "run" }.call
来源：http://cfa.cdnleiting.top

C#:   // 无 IIFE：用静态构造函数
来源：http://azb.guowangkeji.top

[C13] 类型声明 / 类型注解
来源：http://qan.ybcxt.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wmk.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gll.birdmap.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pjl.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://khd.0kj1m.cn


<!-- 参考信息 -->