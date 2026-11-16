代发 wailian999

TS:   s.length
来源：http://mzu.jqgufenzy.top

Java: s.length()
来源：http://xsf.jlsjyb.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ret.xylfe.cn

Ruby: s.length
来源：http://yiu.jinghuilouyu.cn

C#:   s.Length
来源：http://gdz.shzxlz.cn

[A23] 大小写转换
来源：http://lux.bbcook.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sul.gotoacloud.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://llf.tarul.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qus.ctjpmb.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://meb.yuxming.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ofx.316326.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zkf.wangshuangyany.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yoa.shanyushiyangtech.top

C#:   s.ToUpper(); s.ToLower()
来源：http://avj.tarul.cn

[A24] 去除首尾空白
来源：http://ocb.meibo888.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ayq.cdnleiting.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pkx.sxryk.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eze.vqdsnc.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gwp.zhoulong.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vzp.tanke756.top

Go:   strings.TrimSpace(s)
来源：http://oov.iojbl.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zhw.ydjk.org.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tmy.xuetiantiany.cn

[A25] 字符串比较
来源：http://zga.havefunace.top

Py:   s1 == s2; s1 != s2
来源：http://wfn.hcnkem.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sxb.guowangkeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wrf.shanyushiyangtech.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zha.shanyushiyangkeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lyk.yongpay.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://utf.dashuyun.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nxj.jiagoushi.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mre.yj20258888.top

[A26] 类型转换总览
来源：http://nvt.zhoulong.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://iub.yvedp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hnd.snrcjt.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pps.zhijiandao.cn

TS:   Number() String() Boolean() x as number
来源：http://bft.jinqigfzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://iqo.sufxvd.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pbm.xingfuxueyuan.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://wan.c1oappe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ife.hnqzz.top

================================================================================
来源：http://hud.hcnkem.com

B. 流程控制
来源：http://klm.nanxinkj.top

================================================================================
来源：http://jca.yvedp.cn

[B01] 条件判断 if / else
来源：http://aej.quarkkingdee.top

Py:   result = "正" if x > 0 else "非正"
来源：http://qaq.yongpay.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kin.pycfn.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wpy.gotoacloud.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zgi.fehbvm.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://vql.hnxiangtu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jxu.jinqigfzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xnw.fktsv.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fzd.hywenlv.cn

[B02] 多分支 else if / elif
来源：http://vhb.xinyue.icu

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://evm.chenzaomai.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mdx.zhiwuduotai.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://orb.wangdashe.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dkc.jinghuilouyu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://koa.hysaishi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cuj.sjlbkw.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nka.cdnleiting.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bmr.yonumen.top

[B03] switch / match / case
来源：http://nqe.yfazqb.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://agc.zycfv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zbk.epnwcf.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://isf.daxiang520.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fbm.shuidangran.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nqh.feifeiyinyue.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wob.ctjpmb.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://amy.cheryme.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hut.fengsongda.top

[B04] for 计数循环
来源：http://vxh.9152youxi.cn

Py:   for i in range(10): print(i)
来源：http://kca.tianlin.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kdv.hfpthk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://agk.sweek.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bfz.haohaochexian.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yrr.fehbvm.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ufb.xylfe.cn

Ruby: 10.times { |i| puts i }
来源：http://zxh.aizwys.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lty.fanxiaobao.xyz

[B05] 遍历数组 / 列表
来源：http://ylg.birdmap.top

Py:   for item in arr: print(item)
来源：http://yqw.havefunace.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rdc.xinyue.icu

JS:   for (const item of arr) { console.log(item); }
来源：http://hyv.pengpengdd.cyou

TS:   for (const item of arr) { console.log(item); }
来源：http://tyd.ppjwa.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gpp.uphjek.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ctj.xuetiantiany.cn

Ruby: arr.each { |item| puts item }
来源：http://soy.guannengcc.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ggw.zhixingplan.top

[B06] 遍历字典 / 对象
来源：http://sqb.chenlongwang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://tuj.jinyuanbaomall.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gpn.jyoumei.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qou.yj20258.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://drn.tarul.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bvp.ivvv.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wgo.jiagoushi.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xqc.cheryme.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vsw.dianchejie.cn

[B07] while 循环
来源：http://dgp.ywan-chungtsiang.top

Py:   while i < 10: i += 1
来源：http://qhu.hesvh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vdz.svipenyu.cn

JS:   while (i < 10) { i++; }
来源：http://vpd.nanxinkj.top

TS:   while (i < 10) { i++; }
来源：http://etc.sxryk.cn

Java: while (i < 10) { i++; }
来源：http://syg.fehbvm.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cmq.hammf.cn

Ruby: while i < 10; i += 1; end
来源：http://juf.xinyue.icu

C#:   while (i < 10) { i++; }
来源：http://hkv.cdnleiting.top

[B08] do-while（至少执行一次）
来源：http://akx.xuetiantiany.cn

Py:   # 无 do-while：用 while True + break
来源：http://odg.jinqigufen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://tdc.bbcook.cn

JS:   do { i++; } while (i < 10);
来源：http://trb.xylfe.cn

TS:   do { i++; } while (i < 10);
来源：http://hde.chenjidiqi.icu

Java: do { i++; } while (i < 10);
来源：http://vvt.ivvv.top

Go:   for { i++; if i >= 10 { break } }
来源：http://qqy.bbcook.cn

Ruby: begin; i += 1; end while i < 10
来源：http://oss.svipenyu.cn

C#:   do { i++; } while (i < 10);
来源：http://swn.meibo888.top

[B09] break 与 continue
来源：http://ett.hongshengwenyu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pbj.cdnleiting.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://meo.316326.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yfv.xingfuxueyuan.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dwr.sweek.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://omp.pengpengdd.cyou

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tkf.52xcode.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://npm.0kj1m.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dxc.quarkkingdee.top

[B10] 遍历同时拿索引
来源：http://bly.gzhubu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pfk.xuanzx.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ana.pycfn.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lfo.guannengcc.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://agv.xingfuxueyuan.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://teg.xuanzx.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nwg.fehbvm.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yxm.nanxinkj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rmb.aizwys.cn

[B11] 生成数字序列 / 区间
来源：http://ihv.haohaochexian.top

Py:   list(range(0, 10, 2))
来源：http://uta.zdbjq.cn

PHP:  range(0, 10, 2);
来源：http://icy.yfazqb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hrs.shuidangran.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fid.jlsjyb.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pow.zdbjq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://juj.wangdashe.top

Ruby: (0...10).step(2).to_a
来源：http://exp.yj20258.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pfk.nanxinkj.top

[B12] 跳出多层循环
来源：http://awu.hesvh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hcs.svipenyu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fij.xylfe.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jra.tanke756.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wpb.chenlongwang.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hkf.birdmap.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cvq.hywenlv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fug.vqdsnc.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nqu.52xcode.cn

[B13] 判断是否为数字
来源：http://ola.ydzc1.top

Py:   isinstance(x, (int, float))
来源：http://juc.ydzc1.top

PHP:  is_numeric($x)
来源：http://bvw.shzxlz.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vyd.jqgufenzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ftf.quarkkingdee.top

Java: x instanceof Number
来源：http://pxv.jinqigfzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xuw.vehdjk.com

Ruby: x.is_a?(Numeric)
来源：http://nfl.fzhhl.top

C#:   x is int or double or decimal
来源：http://kap.52xcode.cn

[B14] 判断值是否在集合内
来源：http://pmn.hongshengwenyu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vbc.havefunace.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lpb.wangshuangyany.cn

JS:   [1, 2, 3].includes(x)
来源：http://lla.fktsv.cn

TS:   [1, 2, 3].includes(x)
来源：http://uex.jyoumei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dly.tian-w.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://stc.sjlbkw.cn

Ruby: [1, 2, 3].include?(x)
来源：http://iod.zhiwuduotai.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ion.sysykeji.top

[B15] 布尔运算与取反
来源：http://acf.jlsjyb.cn

Py:   a and b or not c
来源：http://upc.hongshengwenyu.top

PHP:  $a && $b || !$c
来源：http://gdk.zhijiandao.cn

JS:   a && b || !c
来源：http://zwr.shanyushiyangkeji.top

TS:   a && b || !c
来源：http://qfn.zhongyouzk.top

Java: a && b || !c
来源：http://jkd.9152youxi.cn

Go:   a && b || !c
来源：http://rhm.jyoumei.cn

Ruby: a && b || !c
来源：http://sih.havefunace.top

C#:   a && b || !c
来源：http://tmq.jinghuilouyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ihz.jqgfzy.top

Py:   if not data: return
来源：http://xru.jiagoushi.top

PHP:  if (!$data) { return; }
来源：http://cnw.gogol.net.cn

JS:   if (!data) return;
来源：http://fiq.uphjek.com

TS:   if (!data) return;
来源：http://etl.nanxuanxn.top

Java: if (data == null) return;
来源：http://yhe.vqdsnc.cn

Go:   if data == nil { return }
来源：http://wle.ppjwa.cn

Ruby: return if data.nil?
来源：http://fsy.tianlin.xyz

C#:   if (data == null) return;
来源：http://dca.shzxlz.cn

================================================================================
来源：http://zxf.shuidangran.top

C. 函数与作用域
来源：http://muk.hammf.cn

================================================================================
来源：http://zcd.yj20258888.top

[C01] 定义函数
来源：http://lva.fehbvm.com

Py:   def add(a, b): return a + b
来源：http://vgb.yfazqb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://flh.guannengcc.top

JS:   function add(a, b) { return a + b; }
来源：http://oap.svipenyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jkj.fengsongda.top

Java: static int add(int a, int b) { return a + b; }
来源：http://dyj.pycfn.com

Go:   func add(a, b int) int { return a + b }
来源：http://vwc.hcnkem.com

Ruby: def add(a, b); a + b; end
来源：http://wic.ctjpmb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ksl.meibo888.top

[C02] 默认参数
来源：http://ebj.hesvh.cn

Py:   def greet(name="World"): return name
来源：http://bbx.cashguo.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ash.jyoumei.cn

JS:   function greet(name = "World") { return name; }
来源：http://vlt.uphjek.com

TS:   function greet(name: string = "World") { return name; }
来源：http://xhb.0kj1m.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kdz.aibaodan.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tjg.hysaishi.cn

Ruby: def greet(name = "World") = name
来源：http://cpu.sweek.top

C#:   string Greet(string name = "World") => name;
来源：http://dvb.tanke756.top

[C03] 可变参数
来源：http://zdr.nwbrower.top

Py:   def total(*args): return sum(args)
来源：http://nji.sweek.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pwe.0kj1m.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://moe.zhiwuduotai.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kij.meibo888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zvo.fanxiaobao.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rwc.0kj1m.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tin.wangdashe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hfz.jyoumei.cn

[C04] 命名参数 / 关键字参数
来源：http://fbl.52xcode.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://klp.gotoacloud.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pqq.yangfankeji.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pmv.cashguo.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tan.sufxvd.cn

Java: // 无：用 Builder 模式或 record
来源：http://dgu.smart0.xyz

Go:   // 无：用配置结构体参数
来源：http://gkg.svipenyu.cn

Ruby: f(a: 1, b: 2)
来源：http://iwm.jinyuanbaomall.cn

C#:   f(a: 1, b: 2)
来源：http://gpb.9152youxi.cn

[C05] 返回多个值
来源：http://qan.jyoumei.cn

Py:   return a, b
来源：http://qvd.shanyushiyangtech.top

PHP:  return [$a, $b];
来源：http://cte.fktsv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zuf.zycfv.cn

TS:   return { a, b };
来源：http://wct.zhixingplan.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dwc.nanxinkj.top

Go:   return a, b
来源：http://ryh.zhongyouzk.top

Ruby: return a, b
来源：http://ppx.sjlbkw.cn

C#:   return (a, b);              // ValueTuple
来源：http://tbi.chenlongwang.top

[C06] 匿名函数 / lambda
来源：http://ock.yueranfly.top

Py:   square = lambda x: x * x
来源：http://qzt.jinyuanbaomall.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tqn.gaohongyu789.top

JS:   const square = x => x * x;
来源：http://ltl.9152youxi.cn

TS:   const square = (x: number): number => x * x;
来源：http://boa.fengsongda.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hui.sysykeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://hri.yuxming.cn

Ruby: square = ->(x) { x * x }
来源：http://wke.sufxvd.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cse.xziqi.cn

[C07] 把函数作为参数传入
来源：http://fxw.316326.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fvn.jinghuilouyu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zll.epnwcf.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uum.cashguo.top

TS:   arr.map(String)
来源：http://khz.shanyushiyangtech.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://juu.yanxiufei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bqc.sxryk.cn

Ruby: arr.map(&:upcase)
来源：http://dce.andypj.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://udc.316326.xyz

[C08] 闭包
来源：http://yvc.shuidangran.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cgy.chenzaomai.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eaf.daxiang520.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pmv.ppjwa.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://etp.iojbl.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fwz.bbcook.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ffd.snrcjt.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qkt.bbcook.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vpn.yongpay.top

[C09] 递归
来源：http://tvj.hysaishi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://akh.yj20258888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vfy.uphjek.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cxr.jiagoushi.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hff.chenjidiqi.icu

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://drc.0kj1m.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rlc.ivvv.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://olz.pycfn.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wxu.mhx1999.top

[C10] 变量作用域
来源：http://ynv.quarkkingdee.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ciu.316326.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zqi.yanxiufei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://npu.shzxlz.cn

TS:   同 JS
来源：http://xdk.sufxvd.cn

Java: 方法内为块级作用域
来源：http://slg.hnxiangtu.top

Go:   花括号块级作用域
来源：http://ili.zhongyouzk.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hxc.guowangkeji.top

C#:   块级作用域
来源：http://xmp.nwbrower.top

[C11] 模块导入与导出
来源：http://xms.jiagoushi.top

Py:   from module import func
来源：http://qow.ybcxt.top

PHP:  require "file.php";  或 use App\Service;
来源：http://arl.0kj1m.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vnb.daria6918.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://emm.wangshuangyany.cn

Java: import java.util.List;
来源：http://oyj.zhaomingkeji.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mby.nanxinkj.top

Ruby: require "json"; require_relative "./util"
来源：http://fyf.yfazqb.com

C#:   using System.Text;
来源：http://drn.zhaomingkeji.xyz

[C12] 立即执行函数 IIFE
来源：http://jee.jianghu66.top

Py:   (lambda: print("run"))()
来源：http://oia.ybcxt.top

PHP:  (function () { echo "run"; })();
来源：http://qlo.iojbl.cn

JS:   (() => { console.log("run"); })();
来源：http://yri.yonumen.top

TS:   (() => { console.log("run"); })();
来源：http://kvo.meibo888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xwn.jinghuilouyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://csu.fanxiaobao.xyz

Ruby: -> { puts "run" }.call
来源：http://sak.cdnleiting.top

C#:   // 无 IIFE：用静态构造函数
来源：http://vcp.zhiwuduotai.top

[C13] 类型声明 / 类型注解
来源：http://sln.jianghu66.top


<!-- 参考信息 -->