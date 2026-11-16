代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wls.cdnleiting.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fdr.sysykeji.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tzd.shanyushiyangkeji.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gmd.xylfe.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nfk.gaohongyu789.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gtn.jlsjyb.cn

[A24] 去除首尾空白
来源：http://bla.shzxlz.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xkj.hnxiangtu.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://afs.zhoulong.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hpv.chenzaomai.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dfp.tanke756.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wmu.redwolf501.top

Go:   strings.TrimSpace(s)
来源：http://fin.cheryme.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rqb.shuidangran.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jri.xziqi.cn

[A25] 字符串比较
来源：http://qbg.snrcjt.cn

Py:   s1 == s2; s1 != s2
来源：http://bpv.gotoacloud.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zhw.zdbjq.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pbn.cqqwz.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jxf.hnxiangtu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nys.svipenyu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vno.yj20258888.top

Ruby: s1 == s2; s1 <=> s2
来源：http://lpf.jinqigfzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ocz.jyoumei.cn

[A26] 类型转换总览
来源：http://cmv.jlsjyb.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vsu.jqgfzy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yhx.cheryme.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hdf.bbcook.cn

TS:   Number() String() Boolean() x as number
来源：http://zcx.svipenyu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pie.jyoumei.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dpp.guowangkeji.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://nfx.9152youxi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yso.yangfankeji.com

================================================================================
来源：http://oty.cucudq.cn

B. 流程控制
来源：http://goq.gogol.net.cn

================================================================================
来源：http://bji.sxryk.cn

[B01] 条件判断 if / else
来源：http://dek.meibo888.top

Py:   result = "正" if x > 0 else "非正"
来源：http://vvc.fehbvm.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://skq.feifeiyinyue.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zsg.havefunace.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baw.cucudq.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vgu.fehbvm.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ofe.tianlin.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ggh.gogol.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zzl.gotoacloud.top

[B02] 多分支 else if / elif
来源：http://qaf.zhengqikj.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tfa.yfazqb.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wzk.yj202588.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jyd.shanyushiyangtech.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hjk.jianghu66.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fmy.ydjk.org.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tvx.nanxinkj.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gof.c1oappe.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dvx.feifeiyinyue.top

[B03] switch / match / case
来源：http://udc.zhengqikj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ybp.mhx1999.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://krw.c1oappe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ioe.bjfxy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://syi.zhoulong.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tro.hongshengwenyu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://arh.xuanzx.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ira.chenlongwang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zos.zhongyouzk.top

[B04] for 计数循环
来源：http://ums.yonumen.top

Py:   for i in range(10): print(i)
来源：http://ucr.hongshengwenyu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ecr.cheryme.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vat.tianlin.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jqa.yfazqb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ccy.nanxinkj.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mvd.redwolf501.top

Ruby: 10.times { |i| puts i }
来源：http://fnh.gotoacloud.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lbj.svipenyu.cn

[B05] 遍历数组 / 列表
来源：http://dnq.snrcjt.cn

Py:   for item in arr: print(item)
来源：http://clh.cashguo.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lfn.jqgfzy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://yog.ywan-chungtsiang.top

TS:   for (const item of arr) { console.log(item); }
来源：http://yke.yvedp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yxp.cqqwz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xfb.vqdsnc.cn

Ruby: arr.each { |item| puts item }
来源：http://sdq.ydjk.org.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qqc.yj20258.top

[B06] 遍历字典 / 对象
来源：http://hjr.cdnleiting.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xkj.nanxinkj.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://eln.xylfe.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://abp.zycfv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cvy.52xcode.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fvt.hongshengwenyu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xfx.xziqi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zyl.iojbl.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cgx.epnwcf.com

[B07] while 循环
来源：http://cfn.zhengqikj.top

Py:   while i < 10: i += 1
来源：http://ktz.fktsv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://chq.feifeiyinyue.top

JS:   while (i < 10) { i++; }
来源：http://uea.jqgufenzy.top

TS:   while (i < 10) { i++; }
来源：http://azq.snrcjt.cn

Java: while (i < 10) { i++; }
来源：http://zrp.ybcxt.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rxl.yfazqb.com

Ruby: while i < 10; i += 1; end
来源：http://mri.shuidangran.top

C#:   while (i < 10) { i++; }
来源：http://yrt.fanxiaobao.xyz

[B08] do-while（至少执行一次）
来源：http://plw.fktsv.cn

Py:   # 无 do-while：用 while True + break
来源：http://aeu.shangyingyoupin.top

PHP:  do { $i++; } while ($i < 10);
来源：http://amn.zhiwuduotai.top

JS:   do { i++; } while (i < 10);
来源：http://dmt.dashuyun.cn

TS:   do { i++; } while (i < 10);
来源：http://cdf.aizwys.cn

Java: do { i++; } while (i < 10);
来源：http://iqd.feifeiyinyue.top

Go:   for { i++; if i >= 10 { break } }
来源：http://mib.316326.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://ama.jlsjyb.cn

C#:   do { i++; } while (i < 10);
来源：http://cpl.yuanzhike.top

[B09] break 与 continue
来源：http://wbl.xinyue.icu

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ere.cqqwz.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vjb.jqgufenzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pwc.jlsjyb.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://roc.fanxiaobao.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xks.ybcxt.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ycr.guannengcc.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ddt.havefunace.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://spw.sjlbkw.cn

[B10] 遍历同时拿索引
来源：http://idd.zhengqikj.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zzo.yvedp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://coj.jinghuilouyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://opz.vehdjk.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cgc.fehbvm.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xfh.meibo888.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gdh.svipenyu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hwi.ywan-chungtsiang.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hho.cdnleiting.top

[B11] 生成数字序列 / 区间
来源：http://oio.xuetiantiany.cn

Py:   list(range(0, 10, 2))
来源：http://imx.ppjwa.cn

PHP:  range(0, 10, 2);
来源：http://itd.jinqigufen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qqp.zhaomingkeji.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fao.zhixingplan.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pfe.fzhhl.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bha.aibaodan.cn

Ruby: (0...10).step(2).to_a
来源：http://ubx.chenjidiqi.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vbo.jianghu66.top

[B12] 跳出多层循环
来源：http://kzr.yj202588.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ozo.ywan-chungtsiang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://hbg.ctjpmb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hta.xuetiantiany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hst.shuidangran.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uoh.tian-w.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dfm.xuetiantiany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vsh.yuxming.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://txh.yuanzhike.top

[B13] 判断是否为数字
来源：http://gdd.snrcjt.cn

Py:   isinstance(x, (int, float))
来源：http://hwv.fehbvm.com

PHP:  is_numeric($x)
来源：http://uyy.fengsongda.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qqd.dianchejie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ekx.ywan-chungtsiang.top

Java: x instanceof Number
来源：http://voi.xziqi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jvh.haohaochexian.top

Ruby: x.is_a?(Numeric)
来源：http://lhu.sweek.top

C#:   x is int or double or decimal
来源：http://ryp.shanyushiyangkeji.top

[B14] 判断值是否在集合内
来源：http://qnf.zhiwuduotai.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hvj.epnwcf.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gpz.kuanghao11.cn

JS:   [1, 2, 3].includes(x)
来源：http://sab.gzhubu.top

TS:   [1, 2, 3].includes(x)
来源：http://vin.pengpengdd.cyou

Java: List.of(1, 2, 3).contains(x)
来源：http://whr.andypj.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yzp.yueranfly.top

Ruby: [1, 2, 3].include?(x)
来源：http://fti.yanxiufei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pgi.316326.xyz

[B15] 布尔运算与取反
来源：http://fay.haohaochexian.top

Py:   a and b or not c
来源：http://cth.jinghuilouyu.cn

PHP:  $a && $b || !$c
来源：http://jbq.xingfuxueyuan.xyz

JS:   a && b || !c
来源：http://nrq.dianchejie.cn

TS:   a && b || !c
来源：http://hfr.wangdashe.top

Java: a && b || !c
来源：http://erz.zdqjudy.top

Go:   a && b || !c
来源：http://xby.uphjek.com

Ruby: a && b || !c
来源：http://ywj.xylfe.cn

C#:   a && b || !c
来源：http://pmk.daria6918.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xlm.havefunace.top

Py:   if not data: return
来源：http://wcx.svipenyu.cn

PHP:  if (!$data) { return; }
来源：http://jfd.ivvv.top

JS:   if (!data) return;
来源：http://qas.jinqigufen.top

TS:   if (!data) return;
来源：http://gsb.bjfxy.top

Java: if (data == null) return;
来源：http://mof.9152youxi.cn

Go:   if data == nil { return }
来源：http://ysx.guowangkeji.top

Ruby: return if data.nil?
来源：http://she.cheryme.top

C#:   if (data == null) return;
来源：http://mer.quarkkingdee.top

================================================================================
来源：http://ayf.ybcxt.top

C. 函数与作用域
来源：http://cxj.ydjk.org.cn

================================================================================
来源：http://chm.ctjpmb.com

[C01] 定义函数
来源：http://cdp.epnwcf.com

Py:   def add(a, b): return a + b
来源：http://yes.xylfe.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hez.pycfn.com

JS:   function add(a, b) { return a + b; }
来源：http://bos.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fiv.ctjpmb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://cuj.xuanzx.com

Go:   func add(a, b int) int { return a + b }
来源：http://otq.sysykeji.top

Ruby: def add(a, b); a + b; end
来源：http://onw.yanxiufei.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ovy.316326.xyz

[C02] 默认参数
来源：http://sjr.hnqzz.top

Py:   def greet(name="World"): return name
来源：http://qry.xingfuxueyuan.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://vee.yfazqb.com

JS:   function greet(name = "World") { return name; }
来源：http://sii.daxiang520.top

TS:   function greet(name: string = "World") { return name; }
来源：http://sjt.hammf.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rdp.sufxvd.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mxd.fehbvm.com

Ruby: def greet(name = "World") = name
来源：http://zar.cucudq.cn

C#:   string Greet(string name = "World") => name;
来源：http://yyu.birdmap.top

[C03] 可变参数
来源：http://sja.cucudq.cn

Py:   def total(*args): return sum(args)
来源：http://bhh.jiagoushi.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wzp.yueranfly.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eky.hywenlv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xpz.bjfxy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yjt.jinghuilouyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://abu.daria6918.cn

Ruby: def total(*nums); nums.sum; end
来源：http://luh.fzhhl.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fnr.ctjpmb.com

[C04] 命名参数 / 关键字参数
来源：http://atx.wangdashe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pjj.aizwys.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ius.bbcook.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ncb.tian-w.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://amm.hfpthk.cn

Java: // 无：用 Builder 模式或 record
来源：http://abu.jinqigufen.top

Go:   // 无：用配置结构体参数
来源：http://fna.xziqi.cn

Ruby: f(a: 1, b: 2)
来源：http://jvc.shzxlz.cn

C#:   f(a: 1, b: 2)
来源：http://whg.snrcjt.cn

[C05] 返回多个值
来源：http://oex.iojbl.cn

Py:   return a, b
来源：http://ebj.sysykeji.top

PHP:  return [$a, $b];
来源：http://vdm.zhengqikj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rdv.mhx1999.top

TS:   return { a, b };
来源：http://akl.nanxuanxn.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://aix.hysaishi.cn

Go:   return a, b
来源：http://juj.bbcook.cn

Ruby: return a, b
来源：http://juq.hesvh.cn

C#:   return (a, b);              // ValueTuple
来源：http://bjl.chenzaomai.com

[C06] 匿名函数 / lambda
来源：http://zqk.tian-w.cn

Py:   square = lambda x: x * x
来源：http://pyb.tarul.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yqm.feifeiyinyue.top

JS:   const square = x => x * x;
来源：http://bfc.shangyingyoupin.top

TS:   const square = (x: number): number => x * x;
来源：http://lyw.zhaomingkeji.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zlb.ybcxt.top

Go:   sq := func(x int) int { return x * x }
来源：http://zhl.sysykeji.top

Ruby: square = ->(x) { x * x }
来源：http://joe.guannengcc.top

C#:   Func<int, int> square = x => x * x;
来源：http://kdn.havefunace.top

[C07] 把函数作为参数传入
来源：http://byn.gotoacloud.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://evt.yuanzhike.top

PHP:  array_map("strtoupper", $arr);
来源：http://llt.ywan-chungtsiang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://myp.epnwcf.com

TS:   arr.map(String)
来源：http://qyl.zhiwuduotai.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yas.yongpay.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ktr.zhixingplan.top

Ruby: arr.map(&:upcase)
来源：http://nrk.yvedp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vvi.fehbvm.com

[C08] 闭包
来源：http://tgv.hywenlv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vwz.zhongyouzk.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tvo.yonumen.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hma.meibo888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://inr.zhijiandao.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ggh.nanxinkj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cjj.hnxiangtu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yvv.aibaodan.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pkv.dashuyun.cn

[C09] 递归
来源：http://sxj.jlsjyb.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tcg.chenzaomai.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zsy.cdnleiting.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pfz.sweek.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wkf.yuanzhike.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kuq.redwolf501.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zxh.zhoulong.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ahu.vehdjk.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://irt.zhiwuduotai.top

[C10] 变量作用域
来源：http://rqm.gotoacloud.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ytg.zdbjq.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://thc.jyoumei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://svi.sysykeji.top

TS:   同 JS
来源：http://qhv.aizwys.cn

Java: 方法内为块级作用域
来源：http://hts.uphjek.com

Go:   花括号块级作用域
来源：http://jvm.0kj1m.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://evo.wangshuangyany.cn

C#:   块级作用域
来源：http://lad.fanxiaobao.xyz

[C11] 模块导入与导出
来源：http://nbx.pycfn.com

Py:   from module import func
来源：http://qfv.tanke756.top

PHP:  require "file.php";  或 use App\Service;
来源：http://yxj.dianchejie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jpx.guowangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dkj.hongshengwenyu.top

Java: import java.util.List;
来源：http://nko.feifeiyinyue.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://isr.fanxiaobao.xyz

Ruby: require "json"; require_relative "./util"
来源：http://pbp.bjfxy.top

C#:   using System.Text;
来源：http://vag.cashguo.top

[C12] 立即执行函数 IIFE
来源：http://hat.guannengcc.top

Py:   (lambda: print("run"))()
来源：http://tgn.fzhhl.top

PHP:  (function () { echo "run"; })();
来源：http://ani.yj20258.top

JS:   (() => { console.log("run"); })();
来源：http://xff.zhongyouzk.top

TS:   (() => { console.log("run"); })();
来源：http://tcr.zhoulong.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zvz.cucudq.cn

Go:   func() { fmt.Println("run") }()
来源：http://iev.xziqi.cn

Ruby: -> { puts "run" }.call
来源：http://uos.zhongyouzk.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zhn.pycfn.com

[C13] 类型声明 / 类型注解
来源：http://yxc.wangdashe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gqe.jinyuanbaomall.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oed.sufxvd.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://drs.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tuu.dianchejie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zoz.ydjk.org.cn

Go:   func add(a, b int) int
来源：http://bjs.shanyushiyangkeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lfe.yvedp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cnk.hywenlv.cn


<!-- 参考信息 -->