代发 wailian999

TS:   s.length
来源：http://uue.redwolf501.top

Java: s.length()
来源：http://mcx.xylfe.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kwm.hammf.cn

Ruby: s.length
来源：http://ehg.sjlbkw.cn

C#:   s.Length
来源：http://fib.yongpay.top

[A23] 大小写转换
来源：http://wab.sjlbkw.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fqk.hesvh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://khl.yueranfly.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://azv.jyoumei.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://maj.yfazqb.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fbx.9152youxi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rxy.cucudq.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fja.yuanzhike.top

C#:   s.ToUpper(); s.ToLower()
来源：http://goe.kuanghao11.cn

[A24] 去除首尾空白
来源：http://kce.kuanghao11.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yuw.ydjk.org.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jym.bbcook.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qlz.zhijiandao.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lun.sweek.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ciz.birdmap.top

Go:   strings.TrimSpace(s)
来源：http://kdu.shanyushiyangkeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tbs.jyoumei.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zpy.316326.xyz

[A25] 字符串比较
来源：http://xhj.hammf.cn

Py:   s1 == s2; s1 != s2
来源：http://ijy.ehwqpu.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://err.cucudq.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gve.wangdashe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fvj.sxryk.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://twx.jinqigfzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qon.meibo888.top

Ruby: s1 == s2; s1 <=> s2
来源：http://mib.pycfn.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fal.nwbrower.top

[A26] 类型转换总览
来源：http://hhx.pycfn.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zzl.zhaomingkeji.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lws.316326.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sfs.ivvv.top

TS:   Number() String() Boolean() x as number
来源：http://xvo.havefunace.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://odc.fehbvm.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qhm.nanxinkj.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://sag.jinyuanbaomall.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yij.cqqwz.cn

================================================================================
来源：http://vzo.hysaishi.cn

B. 流程控制
来源：http://fsy.jqgfzy.top

================================================================================
来源：http://vig.jianghu66.top

[B01] 条件判断 if / else
来源：http://abm.fengsongda.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ytj.yj202588.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rlh.ywan-chungtsiang.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qwf.yfazqb.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ggf.mhx1999.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://zqk.tianlin.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cqb.xuetiantiany.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hoe.shzxlz.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://eeo.nwbrower.top

[B02] 多分支 else if / elif
来源：http://mus.yj202588.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cij.hongshengwenyu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zao.9152youxi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tez.shanyushiyangtech.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tqu.dianchejie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lzg.52xcode.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yye.quarkkingdee.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qul.sxryk.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mkz.iojbl.cn

[B03] switch / match / case
来源：http://jay.jianghu66.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yul.gotoacloud.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bmx.smart0.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mtl.shzxlz.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bip.gogol.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ici.yanxiufei.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pfn.jyoumei.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ahf.fehbvm.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ial.jiagoushi.top

[B04] for 计数循环
来源：http://otr.yj20258888.top

Py:   for i in range(10): print(i)
来源：http://yap.nanxinkj.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gqp.aibaodan.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kcm.ivvv.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fhp.yuxming.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://akp.haohaochexian.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ukq.yj202588.top

Ruby: 10.times { |i| puts i }
来源：http://xxj.snrcjt.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://drt.yuanzhike.top

[B05] 遍历数组 / 列表
来源：http://xvj.daxiang520.top

Py:   for item in arr: print(item)
来源：http://toz.fehbvm.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zxg.hfpthk.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bjw.yongpay.top

TS:   for (const item of arr) { console.log(item); }
来源：http://yek.haohaochexian.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://lgu.yj20258888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://itt.cdnleiting.top

Ruby: arr.each { |item| puts item }
来源：http://awd.havefunace.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gfd.redwolf501.top

[B06] 遍历字典 / 对象
来源：http://sfj.mhx1999.top

Py:   for k, v in d.items(): print(k, v)
来源：http://fff.daxiang520.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mit.vehdjk.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://weh.mhx1999.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ydb.chenzaomai.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uuy.cashguo.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uoo.zhongyouzk.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lrs.sysykeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://adc.ydzc1.top

[B07] while 循环
来源：http://akc.daria6918.cn

Py:   while i < 10: i += 1
来源：http://kac.jinyuanbaomall.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mrn.birdmap.top

JS:   while (i < 10) { i++; }
来源：http://xkn.sjlbkw.cn

TS:   while (i < 10) { i++; }
来源：http://grx.yj202588.top

Java: while (i < 10) { i++; }
来源：http://vuf.iojbl.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lza.pycfn.com

Ruby: while i < 10; i += 1; end
来源：http://oli.c1oappe.top

C#:   while (i < 10) { i++; }
来源：http://xel.hysaishi.cn

[B08] do-while（至少执行一次）
来源：http://jlg.yanxiufei.cn

Py:   # 无 do-while：用 while True + break
来源：http://uur.jlsjyb.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xjk.sjlbkw.cn

JS:   do { i++; } while (i < 10);
来源：http://lou.sjlbkw.cn

TS:   do { i++; } while (i < 10);
来源：http://wlt.yangfankeji.com

Java: do { i++; } while (i < 10);
来源：http://cyk.yueranfly.top

Go:   for { i++; if i >= 10 { break } }
来源：http://kpe.daxiang520.top

Ruby: begin; i += 1; end while i < 10
来源：http://yur.zdbjq.cn

C#:   do { i++; } while (i < 10);
来源：http://flq.nanxinkj.top

[B09] break 与 continue
来源：http://dxx.uphjek.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kox.iojbl.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zsp.nanxuanxn.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://huv.cucudq.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gag.jianghu66.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qwi.fzhhl.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://glo.jinqigfzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lng.xinyue.icu

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gxs.daria6918.cn

[B10] 遍历同时拿索引
来源：http://bya.snrcjt.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vwx.jiagoushi.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nch.guowangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sua.haohaochexian.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://txc.vqdsnc.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lhv.andypj.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jrr.xylfe.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ofx.smart0.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://icm.zhoulong.xyz

[B11] 生成数字序列 / 区间
来源：http://aka.fengsongda.top

Py:   list(range(0, 10, 2))
来源：http://owx.tian-w.cn

PHP:  range(0, 10, 2);
来源：http://zye.c1oappe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kox.epnwcf.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dmp.pengpengdd.cyou

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uxp.iojbl.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xjz.nanxuanxn.top

Ruby: (0...10).step(2).to_a
来源：http://dum.jinqigufen.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bti.yueranfly.top

[B12] 跳出多层循环
来源：http://eao.fanxiaobao.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://uzo.ppjwa.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dty.vqdsnc.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hte.fehbvm.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://eyv.sxryk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qor.feifeiyinyue.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sub.zhixingplan.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aml.guowangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ydl.jinyuanbaomall.cn

[B13] 判断是否为数字
来源：http://lps.yuxming.cn

Py:   isinstance(x, (int, float))
来源：http://byi.ppjwa.cn

PHP:  is_numeric($x)
来源：http://shq.zhengqikj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kwx.jianghu66.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ghn.jianghu66.top

Java: x instanceof Number
来源：http://lgn.uphjek.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nos.xingfuxueyuan.xyz

Ruby: x.is_a?(Numeric)
来源：http://vuv.zdqjudy.top

C#:   x is int or double or decimal
来源：http://odz.svipenyu.cn

[B14] 判断值是否在集合内
来源：http://ccc.vehdjk.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://agq.aizwys.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jtl.shuidangran.top

JS:   [1, 2, 3].includes(x)
来源：http://zzk.sufxvd.cn

TS:   [1, 2, 3].includes(x)
来源：http://ibw.jinghuilouyu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://omf.pengpengdd.cyou

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uhp.ybcxt.top

Ruby: [1, 2, 3].include?(x)
来源：http://euu.316326.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ftc.guannengcc.top

[B15] 布尔运算与取反
来源：http://dyx.chenjidiqi.icu

Py:   a and b or not c
来源：http://taf.yueranfly.top

PHP:  $a && $b || !$c
来源：http://xjl.nanxuanxn.top

JS:   a && b || !c
来源：http://etc.mhx1999.top

TS:   a && b || !c
来源：http://fun.xinyue.icu

Java: a && b || !c
来源：http://vbq.jinqigufen.top

Go:   a && b || !c
来源：http://rkc.yj20258.top

Ruby: a && b || !c
来源：http://uep.ydjk.org.cn

C#:   a && b || !c
来源：http://iqg.vehdjk.com

[B16] 卫语句：不满足条件提前返回
来源：http://hhe.aibaodan.cn

Py:   if not data: return
来源：http://zia.uphjek.com

PHP:  if (!$data) { return; }
来源：http://hzd.yuanzhike.top

JS:   if (!data) return;
来源：http://qdc.yongpay.top

TS:   if (!data) return;
来源：http://cbr.hammf.cn

Java: if (data == null) return;
来源：http://xgg.jinyuanbaomall.cn

Go:   if data == nil { return }
来源：http://ibi.cashguo.top

Ruby: return if data.nil?
来源：http://lsx.sysykeji.top

C#:   if (data == null) return;
来源：http://iya.cqqwz.cn

================================================================================
来源：http://sop.svipenyu.cn

C. 函数与作用域
来源：http://nup.yuanzhike.top

================================================================================
来源：http://txa.wangshuangyany.cn

[C01] 定义函数
来源：http://qhe.gzhubu.top

Py:   def add(a, b): return a + b
来源：http://coz.ydjk.org.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ukt.hnqzz.top

JS:   function add(a, b) { return a + b; }
来源：http://cnv.52xcode.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rsj.jqgufenzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://lxt.chenzaomai.com

Go:   func add(a, b int) int { return a + b }
来源：http://xle.epnwcf.com

Ruby: def add(a, b); a + b; end
来源：http://itg.guannengcc.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vcd.yonumen.top

[C02] 默认参数
来源：http://qzh.hfpthk.cn

Py:   def greet(name="World"): return name
来源：http://umr.yangfankeji.com

PHP:  function greet($name = "World") { return $name; }
来源：http://nzj.chenlongwang.top

JS:   function greet(name = "World") { return name; }
来源：http://enn.sysykeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://gel.fengsongda.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kvs.zdqjudy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rmc.tian-w.cn

Ruby: def greet(name = "World") = name
来源：http://hmo.jinqigfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://yob.jinqigfzy.top

[C03] 可变参数
来源：http://ulm.quarkkingdee.top

Py:   def total(*args): return sum(args)
来源：http://gmg.iojbl.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hlv.xylfe.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tim.jinghuilouyu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oyk.zhongyouzk.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zih.hywenlv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pip.jinqigfzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://bot.daria6918.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vay.pengpengdd.cyou

[C04] 命名参数 / 关键字参数
来源：http://rgk.jianghu66.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gty.hesvh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sjf.jqgfzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ufv.dashuyun.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bur.gotoacloud.top

Java: // 无：用 Builder 模式或 record
来源：http://uxq.hammf.cn

Go:   // 无：用配置结构体参数
来源：http://erl.zdqjudy.top

Ruby: f(a: 1, b: 2)
来源：http://niv.hysaishi.cn

C#:   f(a: 1, b: 2)
来源：http://gdm.xuanzx.com

[C05] 返回多个值
来源：http://oey.wangshuangyany.cn

Py:   return a, b
来源：http://cdg.nwbrower.top

PHP:  return [$a, $b];
来源：http://vka.redwolf501.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dsn.xuetiantiany.cn

TS:   return { a, b };
来源：http://lbc.xylfe.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zyu.hammf.cn

Go:   return a, b
来源：http://lrs.dashuyun.cn

Ruby: return a, b
来源：http://ftx.quarkkingdee.top

C#:   return (a, b);              // ValueTuple
来源：http://fmd.zhixingplan.top

[C06] 匿名函数 / lambda
来源：http://zww.vehdjk.com

Py:   square = lambda x: x * x
来源：http://psq.jqgufenzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kti.smart0.xyz

JS:   const square = x => x * x;
来源：http://ykv.jinghuilouyu.cn

TS:   const square = (x: number): number => x * x;
来源：http://qpf.kuanghao11.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xui.ehwqpu.com

Go:   sq := func(x int) int { return x * x }
来源：http://urm.c1oappe.top

Ruby: square = ->(x) { x * x }
来源：http://jii.jlsjyb.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pky.feifeiyinyue.top

[C07] 把函数作为参数传入
来源：http://hre.xziqi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qeu.xziqi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rnw.hesvh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dhd.smart0.xyz

TS:   arr.map(String)
来源：http://vks.0kj1m.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hke.snrcjt.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://igr.wangdashe.top

Ruby: arr.map(&:upcase)
来源：http://pif.ybcxt.top

C#:   arr.Select(s => s.ToUpper())
来源：http://waf.zhengqikj.top

[C08] 闭包
来源：http://cez.ppjwa.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kxg.tian-w.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://aqe.redwolf501.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jqy.hcnkem.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://diy.jianghu66.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ryd.tarul.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ivc.yangfankeji.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wpz.zhijiandao.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://izd.jinyuanbaomall.cn

[C09] 递归
来源：http://rxz.gzhubu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://glr.aibaodan.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gus.snrcjt.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pyy.shanyushiyangtech.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cbg.daxiang520.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gyy.hfpthk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gbl.shzxlz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ouz.ybcxt.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://thg.sjlbkw.cn

[C10] 变量作用域
来源：http://zxc.yueranfly.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lju.yj202588.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jrd.fehbvm.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dfs.daria6918.cn

TS:   同 JS
来源：http://uyb.tarul.cn

Java: 方法内为块级作用域
来源：http://xkq.wangshuangyany.cn

Go:   花括号块级作用域
来源：http://yut.bjfxy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pkj.vqdsnc.cn

C#:   块级作用域
来源：http://xkr.zhiwuduotai.top

[C11] 模块导入与导出
来源：http://ioo.tianlin.xyz

Py:   from module import func
来源：http://jku.yongpay.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xqn.zhaomingkeji.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://vyi.ybcxt.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ldw.redwolf501.top

Java: import java.util.List;
来源：http://ucp.pycfn.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pxb.vqdsnc.cn

Ruby: require "json"; require_relative "./util"
来源：http://vvu.guowangkeji.top

C#:   using System.Text;
来源：http://qfo.hnxiangtu.top

[C12] 立即执行函数 IIFE
来源：http://sjk.yongpay.top

Py:   (lambda: print("run"))()
来源：http://ciw.ehwqpu.com

PHP:  (function () { echo "run"; })();
来源：http://xed.ctjpmb.com

JS:   (() => { console.log("run"); })();
来源：http://lmw.cashguo.top

TS:   (() => { console.log("run"); })();
来源：http://tki.shzxlz.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qoj.zhengqikj.top

Go:   func() { fmt.Println("run") }()
来源：http://tup.svipenyu.cn

Ruby: -> { puts "run" }.call
来源：http://tih.jqgufenzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://sym.sysykeji.top

[C13] 类型声明 / 类型注解
来源：http://gcd.jinyuanbaomall.cn


<!-- 参考信息 -->