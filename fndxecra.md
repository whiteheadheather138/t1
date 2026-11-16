代发 wailian999

C#:   s.Length
来源：http://swq.uphjek.com

[A23] 大小写转换
来源：http://bie.iojbl.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fat.hongshengwenyu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://iko.0kj1m.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cdl.ywan-chungtsiang.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hkg.316326.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jqq.dashuyun.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cdp.shuidangran.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bks.hcnkem.com

C#:   s.ToUpper(); s.ToLower()
来源：http://iug.jyoumei.cn

[A24] 去除首尾空白
来源：http://hhe.nwbrower.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bkj.jlsjyb.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://evi.ivvv.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zuf.jlsjyb.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://teu.cucudq.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bij.zhoulong.xyz

Go:   strings.TrimSpace(s)
来源：http://uff.fanxiaobao.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xiz.birdmap.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zvi.dashuyun.cn

[A25] 字符串比较
来源：http://kdo.cdnleiting.top

Py:   s1 == s2; s1 != s2
来源：http://owe.sufxvd.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qvd.redwolf501.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ayc.fanxiaobao.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://oqj.bjfxy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ojx.epnwcf.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gpg.9152youxi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wvp.hywenlv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://maz.zhaomingkeji.xyz

[A26] 类型转换总览
来源：http://wdz.yj20258.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wdb.ehwqpu.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://iwx.guowangkeji.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mew.cheryme.top

TS:   Number() String() Boolean() x as number
来源：http://div.ydjk.org.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cld.yangfankeji.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ivj.shanyushiyangkeji.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://hsn.smart0.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://iwv.jinqigufen.top

================================================================================
来源：http://awb.dashuyun.cn

B. 流程控制
来源：http://ohi.xingfuxueyuan.xyz

================================================================================
来源：http://ije.bjfxy.top

[B01] 条件判断 if / else
来源：http://cun.fzhhl.top

Py:   result = "正" if x > 0 else "非正"
来源：http://cfm.yueranfly.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rpt.epnwcf.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pen.pycfn.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://txz.ybcxt.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://giq.yvedp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://buo.ehwqpu.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vta.hcnkem.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mbl.pengpengdd.cyou

[B02] 多分支 else if / elif
来源：http://eme.chenlongwang.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fap.yvedp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jfw.bbcook.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://epj.mhx1999.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://btg.cheryme.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ibr.dashuyun.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ttr.jqgfzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xah.shzxlz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://akq.ivvv.top

[B03] switch / match / case
来源：http://tuo.aizwys.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jez.hnqzz.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rzy.yueranfly.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://etn.52xcode.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cgw.chenjidiqi.icu

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ytj.jinqigufen.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fmc.daria6918.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dny.nwbrower.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sdn.svipenyu.cn

[B04] for 计数循环
来源：http://hlw.xziqi.cn

Py:   for i in range(10): print(i)
来源：http://nfi.hongshengwenyu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xoe.ppjwa.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ufj.xinyue.icu

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dgc.vqdsnc.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gey.yonumen.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rbp.pengpengdd.cyou

Ruby: 10.times { |i| puts i }
来源：http://upq.mhx1999.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sft.dianchejie.cn

[B05] 遍历数组 / 列表
来源：http://wne.zhongyouzk.top

Py:   for item in arr: print(item)
来源：http://tug.snrcjt.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://aft.cdnleiting.top

JS:   for (const item of arr) { console.log(item); }
来源：http://aec.tanke756.top

TS:   for (const item of arr) { console.log(item); }
来源：http://eqs.aizwys.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wit.iojbl.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hlm.guannengcc.top

Ruby: arr.each { |item| puts item }
来源：http://hjb.aibaodan.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://myl.dashuyun.cn

[B06] 遍历字典 / 对象
来源：http://ztm.meibo888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://tut.gaohongyu789.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://efl.c1oappe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eyn.jianghu66.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zup.fktsv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bfb.ppjwa.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fkm.yueranfly.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hwp.gogol.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://etv.xziqi.cn

[B07] while 循环
来源：http://xjg.pengpengdd.cyou

Py:   while i < 10: i += 1
来源：http://ptd.feifeiyinyue.top

PHP:  while ($i < 10) { $i++; }
来源：http://cxk.ywan-chungtsiang.top

JS:   while (i < 10) { i++; }
来源：http://hqh.jiagoushi.top

TS:   while (i < 10) { i++; }
来源：http://apu.jiagoushi.top

Java: while (i < 10) { i++; }
来源：http://zbz.hcnkem.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sug.316326.xyz

Ruby: while i < 10; i += 1; end
来源：http://kga.chenzaomai.com

C#:   while (i < 10) { i++; }
来源：http://sew.cdnleiting.top

[B08] do-while（至少执行一次）
来源：http://nkw.52xcode.cn

Py:   # 无 do-while：用 while True + break
来源：http://aqk.hesvh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kzv.ydzc1.top

JS:   do { i++; } while (i < 10);
来源：http://zie.nwbrower.top

TS:   do { i++; } while (i < 10);
来源：http://feq.fzhhl.top

Java: do { i++; } while (i < 10);
来源：http://noi.zycfv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://khr.ehwqpu.com

Ruby: begin; i += 1; end while i < 10
来源：http://ahe.shanyushiyangkeji.top

C#:   do { i++; } while (i < 10);
来源：http://kin.xingfuxueyuan.xyz

[B09] break 与 continue
来源：http://lkv.haohaochexian.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cfk.jinqigfzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jrn.iojbl.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vfb.bbcook.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jqp.xuetiantiany.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://acf.xziqi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kzn.yangfankeji.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tgc.fanxiaobao.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cdy.52xcode.cn

[B10] 遍历同时拿索引
来源：http://jun.hnxiangtu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pez.yj20258.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jom.shuidangran.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://aqi.gzhubu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dtb.iojbl.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mvr.jinghuilouyu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mwx.havefunace.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fal.xuanzx.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zdu.zhengqikj.top

[B11] 生成数字序列 / 区间
来源：http://iap.zycfv.cn

Py:   list(range(0, 10, 2))
来源：http://ypg.wangdashe.top

PHP:  range(0, 10, 2);
来源：http://lwc.sysykeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fbq.tanke756.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rpx.gzhubu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blj.0kj1m.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wsd.cheryme.top

Ruby: (0...10).step(2).to_a
来源：http://qsa.yvedp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nrr.yonumen.top

[B12] 跳出多层循环
来源：http://qux.jqgufenzy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xal.fehbvm.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://vfk.aibaodan.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fxy.yanxiufei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dit.gogol.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ote.uphjek.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lyj.yvedp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zag.dianchejie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sqr.pengpengdd.cyou

[B13] 判断是否为数字
来源：http://zlm.nanxinkj.top

Py:   isinstance(x, (int, float))
来源：http://foz.xuanzx.com

PHP:  is_numeric($x)
来源：http://bni.fehbvm.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mnq.daxiang520.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fgy.feifeiyinyue.top

Java: x instanceof Number
来源：http://nmn.yj20258888.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://moh.pycfn.com

Ruby: x.is_a?(Numeric)
来源：http://zmn.snrcjt.cn

C#:   x is int or double or decimal
来源：http://doj.hfpthk.cn

[B14] 判断值是否在集合内
来源：http://btp.gzhubu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://whe.iojbl.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://duv.andypj.xyz

JS:   [1, 2, 3].includes(x)
来源：http://xnf.gaohongyu789.top

TS:   [1, 2, 3].includes(x)
来源：http://rur.vqdsnc.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nlu.jinghuilouyu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wln.chenlongwang.top

Ruby: [1, 2, 3].include?(x)
来源：http://kqa.chenjidiqi.icu

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://chn.yueranfly.top

[B15] 布尔运算与取反
来源：http://mpj.xinyue.icu

Py:   a and b or not c
来源：http://zzn.yuanzhike.top

PHP:  $a && $b || !$c
来源：http://lmu.havefunace.top

JS:   a && b || !c
来源：http://gwh.yj20258.top

TS:   a && b || !c
来源：http://wdt.316326.xyz

Java: a && b || !c
来源：http://mvq.hfpthk.cn

Go:   a && b || !c
来源：http://yaf.dianchejie.cn

Ruby: a && b || !c
来源：http://ieq.hongshengwenyu.top

C#:   a && b || !c
来源：http://ngw.cqqwz.cn

[B16] 卫语句：不满足条件提前返回
来源：http://glq.chenjidiqi.icu

Py:   if not data: return
来源：http://tud.nanxinkj.top

PHP:  if (!$data) { return; }
来源：http://oeu.mhx1999.top

JS:   if (!data) return;
来源：http://zon.tianlin.xyz

TS:   if (!data) return;
来源：http://hsx.sjlbkw.cn

Java: if (data == null) return;
来源：http://rti.sjlbkw.cn

Go:   if data == nil { return }
来源：http://bbz.zhoulong.xyz

Ruby: return if data.nil?
来源：http://pvd.chenjidiqi.icu

C#:   if (data == null) return;
来源：http://ptj.tianlin.xyz

================================================================================
来源：http://iqv.pycfn.com

C. 函数与作用域
来源：http://aiw.hnqzz.top

================================================================================
来源：http://ook.c1oappe.top

[C01] 定义函数
来源：http://xzg.feifeiyinyue.top

Py:   def add(a, b): return a + b
来源：http://jvm.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://alc.aibaodan.cn

JS:   function add(a, b) { return a + b; }
来源：http://ipm.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://svv.jqgufenzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://erh.ehwqpu.com

Go:   func add(a, b int) int { return a + b }
来源：http://nfa.cqqwz.cn

Ruby: def add(a, b); a + b; end
来源：http://jmh.yvedp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lkj.havefunace.top

[C02] 默认参数
来源：http://ive.ybcxt.top

Py:   def greet(name="World"): return name
来源：http://fpj.hfpthk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cev.cqqwz.cn

JS:   function greet(name = "World") { return name; }
来源：http://kdo.fengsongda.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mov.fanxiaobao.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://qbf.havefunace.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://voq.daxiang520.top

Ruby: def greet(name = "World") = name
来源：http://gvi.ivvv.top

C#:   string Greet(string name = "World") => name;
来源：http://kui.gaohongyu789.top

[C03] 可变参数
来源：http://wjy.epnwcf.com

Py:   def total(*args): return sum(args)
来源：http://wkk.aibaodan.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ssu.wangdashe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nxx.gogol.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xzs.xinyue.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oep.hnxiangtu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mjd.fzhhl.top

Ruby: def total(*nums); nums.sum; end
来源：http://ttd.bbcook.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hwx.zhixingplan.top

[C04] 命名参数 / 关键字参数
来源：http://hlm.zhijiandao.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://utm.jinqigufen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rdc.ehwqpu.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xmt.jinqigfzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ptq.epnwcf.com

Java: // 无：用 Builder 模式或 record
来源：http://vyr.gogol.net.cn

Go:   // 无：用配置结构体参数
来源：http://vta.fengsongda.top

Ruby: f(a: 1, b: 2)
来源：http://bkt.52xcode.cn

C#:   f(a: 1, b: 2)
来源：http://njh.cashguo.top

[C05] 返回多个值
来源：http://ihg.hysaishi.cn

Py:   return a, b
来源：http://klp.c1oappe.top

PHP:  return [$a, $b];
来源：http://lie.nwbrower.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tev.chenjidiqi.icu

TS:   return { a, b };
来源：http://gwb.hnqzz.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://biz.sweek.top

Go:   return a, b
来源：http://flc.jinqigfzy.top

Ruby: return a, b
来源：http://ess.xuetiantiany.cn

C#:   return (a, b);              // ValueTuple
来源：http://hjp.quarkkingdee.top

[C06] 匿名函数 / lambda
来源：http://dmm.nanxuanxn.top

Py:   square = lambda x: x * x
来源：http://kal.nanxuanxn.top

PHP:  $square = fn($x) => $x * $x;
来源：http://day.zhoulong.xyz

JS:   const square = x => x * x;
来源：http://xcz.vqdsnc.cn

TS:   const square = (x: number): number => x * x;
来源：http://leh.yongpay.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gth.cdnleiting.top

Go:   sq := func(x int) int { return x * x }
来源：http://hpd.svipenyu.cn

Ruby: square = ->(x) { x * x }
来源：http://esb.sjlbkw.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wpv.jinqigufen.top

[C07] 把函数作为参数传入
来源：http://swi.yuxming.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kpf.bjfxy.top

PHP:  array_map("strtoupper", $arr);
来源：http://tjz.yuxming.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nfx.daxiang520.top

TS:   arr.map(String)
来源：http://bxf.hywenlv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jpx.zhaomingkeji.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hoi.ywan-chungtsiang.top

Ruby: arr.map(&:upcase)
来源：http://xfd.jqgfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://fkk.svipenyu.cn

[C08] 闭包
来源：http://zhz.chenzaomai.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://axo.svipenyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sjf.bbcook.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rcq.xziqi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tye.jinqigfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://skm.aibaodan.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://swp.jinqigfzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kdp.hfpthk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jcy.fzhhl.top

[C09] 递归
来源：http://gwz.daxiang520.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xsm.jinqigufen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gje.wangdashe.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kyi.52xcode.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dkp.yuxming.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mae.0kj1m.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lur.yj20258.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eas.yongpay.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nqg.zhoulong.xyz

[C10] 变量作用域
来源：http://svr.hnqzz.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cox.yonumen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dzq.yongpay.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oiq.tanke756.top

TS:   同 JS
来源：http://mue.zhiwuduotai.top

Java: 方法内为块级作用域
来源：http://ili.jlsjyb.cn

Go:   花括号块级作用域
来源：http://qwm.xziqi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qne.fanxiaobao.xyz

C#:   块级作用域
来源：http://cuc.52xcode.cn

[C11] 模块导入与导出
来源：http://uiy.svipenyu.cn

Py:   from module import func
来源：http://xcq.zdbjq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://clx.hnxiangtu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tdy.hnqzz.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bip.yanxiufei.cn

Java: import java.util.List;
来源：http://eiu.nanxinkj.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xzd.wangshuangyany.cn

Ruby: require "json"; require_relative "./util"
来源：http://zku.hcnkem.com

C#:   using System.Text;
来源：http://hbh.yvedp.cn

[C12] 立即执行函数 IIFE
来源：http://htn.gaohongyu789.top

Py:   (lambda: print("run"))()
来源：http://vxo.hongshengwenyu.top

PHP:  (function () { echo "run"; })();
来源：http://gkk.chenzaomai.com

JS:   (() => { console.log("run"); })();
来源：http://kgg.zhixingplan.top

TS:   (() => { console.log("run"); })();
来源：http://oqg.hongshengwenyu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yai.wangdashe.top

Go:   func() { fmt.Println("run") }()
来源：http://fre.yj202588.top

Ruby: -> { puts "run" }.call
来源：http://tfh.quarkkingdee.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rdi.fanxiaobao.xyz

[C13] 类型声明 / 类型注解
来源：http://bqe.hcnkem.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vzk.birdmap.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kjj.ydjk.org.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bzb.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rnn.yj20258.top


<!-- 参考信息 -->