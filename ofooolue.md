代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uuk.daria6918.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://knh.uphjek.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dez.havefunace.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://inv.meibo888.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dbv.fehbvm.com

C#:   s.ToUpper(); s.ToLower()
来源：http://hgw.gaohongyu789.top

[A24] 去除首尾空白
来源：http://zen.hnxiangtu.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qqq.jinqigfzy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wrz.svipenyu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vps.yvedp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nbn.fengsongda.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ytv.daxiang520.top

Go:   strings.TrimSpace(s)
来源：http://gzd.yuxming.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ykp.bjfxy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://auj.zdbjq.cn

[A25] 字符串比较
来源：http://uqw.kuanghao11.cn

Py:   s1 == s2; s1 != s2
来源：http://btk.0kj1m.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://iez.shanyushiyangtech.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://afv.wangdashe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tnd.guowangkeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nwe.yj20258.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qyh.feifeiyinyue.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ylk.havefunace.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mqg.jinqigufen.top

[A26] 类型转换总览
来源：http://apz.gotoacloud.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://efc.pycfn.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vuv.fengsongda.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cdn.xuetiantiany.cn

TS:   Number() String() Boolean() x as number
来源：http://len.zhijiandao.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wyi.jqgfzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mrj.hywenlv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pms.xziqi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ozq.tarul.cn

================================================================================
来源：http://yse.yj20258888.top

B. 流程控制
来源：http://zgf.hongshengwenyu.top

================================================================================
来源：http://gfl.yueranfly.top

[B01] 条件判断 if / else
来源：http://juk.tian-w.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ecn.sufxvd.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hcf.daxiang520.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://srk.sufxvd.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vfh.aizwys.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sxg.shangyingyoupin.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lgv.hesvh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wxu.zhiwuduotai.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://etf.zhaomingkeji.xyz

[B02] 多分支 else if / elif
来源：http://gva.yuxming.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gyn.sxryk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ual.fengsongda.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qbl.zhongyouzk.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rft.shzxlz.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zte.hesvh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://glo.jianghu66.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lcj.sweek.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iap.iojbl.cn

[B03] switch / match / case
来源：http://xzt.ydzc1.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hyo.epnwcf.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gxd.xingfuxueyuan.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kzo.redwolf501.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://izo.shanyushiyangtech.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qqd.ydjk.org.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sfo.jyoumei.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cgo.ivvv.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mxe.hongshengwenyu.top

[B04] for 计数循环
来源：http://urn.birdmap.top

Py:   for i in range(10): print(i)
来源：http://uqq.fktsv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zlm.fengsongda.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zfx.guowangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ijn.c1oappe.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zuf.guannengcc.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dnd.svipenyu.cn

Ruby: 10.times { |i| puts i }
来源：http://uop.jqgufenzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://adt.xingfuxueyuan.xyz

[B05] 遍历数组 / 列表
来源：http://odi.pycfn.com

Py:   for item in arr: print(item)
来源：http://eol.sjlbkw.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zie.daria6918.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hjp.shuidangran.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ekv.cucudq.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ckm.vqdsnc.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tyb.gotoacloud.top

Ruby: arr.each { |item| puts item }
来源：http://azn.cheryme.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gsy.ydzc1.top

[B06] 遍历字典 / 对象
来源：http://iit.nanxuanxn.top

Py:   for k, v in d.items(): print(k, v)
来源：http://jpz.zhengqikj.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dbw.yongpay.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vrc.hysaishi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://usj.dashuyun.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rqs.andypj.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mkj.pycfn.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ium.cucudq.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://efg.cheryme.top

[B07] while 循环
来源：http://qsf.shanyushiyangkeji.top

Py:   while i < 10: i += 1
来源：http://icx.tianlin.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://nqr.ybcxt.top

JS:   while (i < 10) { i++; }
来源：http://cvb.uphjek.com

TS:   while (i < 10) { i++; }
来源：http://fcj.shanyushiyangtech.top

Java: while (i < 10) { i++; }
来源：http://hqw.ybcxt.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nrx.fehbvm.com

Ruby: while i < 10; i += 1; end
来源：http://sod.yongpay.top

C#:   while (i < 10) { i++; }
来源：http://zmj.xuanzx.com

[B08] do-while（至少执行一次）
来源：http://eyr.smart0.xyz

Py:   # 无 do-while：用 while True + break
来源：http://qgm.kuanghao11.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gsl.ybcxt.top

JS:   do { i++; } while (i < 10);
来源：http://gtx.gzhubu.top

TS:   do { i++; } while (i < 10);
来源：http://eod.fanxiaobao.xyz

Java: do { i++; } while (i < 10);
来源：http://wnz.xinyue.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://ygv.sjlbkw.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hjr.shangyingyoupin.top

C#:   do { i++; } while (i < 10);
来源：http://mzg.jinqigfzy.top

[B09] break 与 continue
来源：http://bqe.cdnleiting.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kyg.0kj1m.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lcn.xingfuxueyuan.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pnp.hongshengwenyu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cti.tian-w.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zve.kuanghao11.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://htj.zhoulong.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://imx.haohaochexian.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ina.yj20258.top

[B10] 遍历同时拿索引
来源：http://thl.yfazqb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://puq.quarkkingdee.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ubp.xuetiantiany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://efl.sxryk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tbt.hnxiangtu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pkl.redwolf501.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nky.dianchejie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rza.yuanzhike.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cgy.havefunace.top

[B11] 生成数字序列 / 区间
来源：http://ykd.zdbjq.cn

Py:   list(range(0, 10, 2))
来源：http://lzz.ivvv.top

PHP:  range(0, 10, 2);
来源：http://yap.fehbvm.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kow.ppjwa.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wce.zhoulong.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nhp.nwbrower.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vzm.yangfankeji.com

Ruby: (0...10).step(2).to_a
来源：http://jbv.xuetiantiany.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wuu.xziqi.cn

[B12] 跳出多层循环
来源：http://nom.jinqigufen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ndu.daria6918.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zmj.yj202588.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pcg.jiagoushi.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nka.daria6918.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jge.xuanzx.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kcn.ydzc1.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mom.shangyingyoupin.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xqd.jinyuanbaomall.cn

[B13] 判断是否为数字
来源：http://qwb.redwolf501.top

Py:   isinstance(x, (int, float))
来源：http://utu.chenzaomai.com

PHP:  is_numeric($x)
来源：http://cpd.jyoumei.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wmb.aizwys.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wsk.zhixingplan.top

Java: x instanceof Number
来源：http://bfx.fktsv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ybm.yuxming.cn

Ruby: x.is_a?(Numeric)
来源：http://oxc.c1oappe.top

C#:   x is int or double or decimal
来源：http://okk.mhx1999.top

[B14] 判断值是否在集合内
来源：http://zlf.zhongyouzk.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nrd.andypj.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ica.zdbjq.cn

JS:   [1, 2, 3].includes(x)
来源：http://mbr.c1oappe.top

TS:   [1, 2, 3].includes(x)
来源：http://yws.chenlongwang.top

Java: List.of(1, 2, 3).contains(x)
来源：http://tio.yanxiufei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pbn.hongshengwenyu.top

Ruby: [1, 2, 3].include?(x)
来源：http://deh.sjlbkw.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ufi.wangdashe.top

[B15] 布尔运算与取反
来源：http://osa.316326.xyz

Py:   a and b or not c
来源：http://ppi.jyoumei.cn

PHP:  $a && $b || !$c
来源：http://uco.ppjwa.cn

JS:   a && b || !c
来源：http://vxl.tarul.cn

TS:   a && b || !c
来源：http://xop.52xcode.cn

Java: a && b || !c
来源：http://lpt.jqgufenzy.top

Go:   a && b || !c
来源：http://kko.cashguo.top

Ruby: a && b || !c
来源：http://xbh.shangyingyoupin.top

C#:   a && b || !c
来源：http://ixv.yonumen.top

[B16] 卫语句：不满足条件提前返回
来源：http://srm.tanke756.top

Py:   if not data: return
来源：http://qor.fehbvm.com

PHP:  if (!$data) { return; }
来源：http://err.bbcook.cn

JS:   if (!data) return;
来源：http://rit.kuanghao11.cn

TS:   if (!data) return;
来源：http://ftz.chenzaomai.com

Java: if (data == null) return;
来源：http://ssv.xingfuxueyuan.xyz

Go:   if data == nil { return }
来源：http://xiz.zhoulong.xyz

Ruby: return if data.nil?
来源：http://tdt.shuidangran.top

C#:   if (data == null) return;
来源：http://sry.fehbvm.com

================================================================================
来源：http://mwy.chenjidiqi.icu

C. 函数与作用域
来源：http://cxx.yj20258.top

================================================================================
来源：http://pdl.epnwcf.com

[C01] 定义函数
来源：http://pkp.hnqzz.top

Py:   def add(a, b): return a + b
来源：http://mdv.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mpp.zhiwuduotai.top

JS:   function add(a, b) { return a + b; }
来源：http://gpt.fanxiaobao.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ayr.zhixingplan.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kws.nwbrower.top

Go:   func add(a, b int) int { return a + b }
来源：http://tte.yonumen.top

Ruby: def add(a, b); a + b; end
来源：http://fbb.haohaochexian.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wda.jlsjyb.cn

[C02] 默认参数
来源：http://lvr.uphjek.com

Py:   def greet(name="World"): return name
来源：http://jaj.yanxiufei.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pba.shanyushiyangtech.top

JS:   function greet(name = "World") { return name; }
来源：http://hkf.jinqigufen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rkl.uphjek.com

Java: // 无默认参数：方法重载或 Optional
来源：http://hma.hywenlv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wbk.redwolf501.top

Ruby: def greet(name = "World") = name
来源：http://czb.yj202588.top

C#:   string Greet(string name = "World") => name;
来源：http://dpp.shanyushiyangkeji.top

[C03] 可变参数
来源：http://yje.jiagoushi.top

Py:   def total(*args): return sum(args)
来源：http://jnx.hfpthk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wue.xuanzx.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pfv.hesvh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tch.zhijiandao.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rno.zhaomingkeji.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lcj.nanxinkj.top

Ruby: def total(*nums); nums.sum; end
来源：http://ebw.tianlin.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xpm.gzhubu.top

[C04] 命名参数 / 关键字参数
来源：http://zrw.vqdsnc.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sep.ehwqpu.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nbl.c1oappe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lsl.zhengqikj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://odb.zhijiandao.cn

Java: // 无：用 Builder 模式或 record
来源：http://vsg.zycfv.cn

Go:   // 无：用配置结构体参数
来源：http://lho.guannengcc.top

Ruby: f(a: 1, b: 2)
来源：http://dwm.jqgfzy.top

C#:   f(a: 1, b: 2)
来源：http://jzo.pengpengdd.cyou

[C05] 返回多个值
来源：http://xoq.quarkkingdee.top

Py:   return a, b
来源：http://sbq.jlsjyb.cn

PHP:  return [$a, $b];
来源：http://vwy.jlsjyb.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://oxw.jinyuanbaomall.cn

TS:   return { a, b };
来源：http://tqr.kuanghao11.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yzl.gotoacloud.top

Go:   return a, b
来源：http://oon.ctjpmb.com

Ruby: return a, b
来源：http://rjq.yvedp.cn

C#:   return (a, b);              // ValueTuple
来源：http://yoj.xuetiantiany.cn

[C06] 匿名函数 / lambda
来源：http://yzo.shanyushiyangtech.top

Py:   square = lambda x: x * x
来源：http://cpa.guowangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://uct.haohaochexian.top

JS:   const square = x => x * x;
来源：http://qey.zhengqikj.top

TS:   const square = (x: number): number => x * x;
来源：http://kvx.fktsv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uzc.ybcxt.top

Go:   sq := func(x int) int { return x * x }
来源：http://yvk.shzxlz.cn

Ruby: square = ->(x) { x * x }
来源：http://yav.yangfankeji.com

C#:   Func<int, int> square = x => x * x;
来源：http://aap.chenjidiqi.icu

[C07] 把函数作为参数传入
来源：http://zuq.ehwqpu.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jfd.xziqi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mnn.fanxiaobao.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://azq.daria6918.cn

TS:   arr.map(String)
来源：http://ytp.gaohongyu789.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sci.tanke756.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://eqq.zhiwuduotai.top

Ruby: arr.map(&:upcase)
来源：http://ltd.haohaochexian.top

C#:   arr.Select(s => s.ToUpper())
来源：http://upf.chenlongwang.top

[C08] 闭包
来源：http://grr.kuanghao11.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zox.wangshuangyany.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lsm.wangshuangyany.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xtr.jinyuanbaomall.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zkr.gotoacloud.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rvm.tanke756.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://emq.zhixingplan.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zeb.ydjk.org.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rqm.ywan-chungtsiang.top

[C09] 递归
来源：http://auj.fanxiaobao.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nir.daria6918.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gnt.hywenlv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nou.havefunace.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://crr.yvedp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ogf.chenzaomai.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cun.fengsongda.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jhp.shanyushiyangtech.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ewp.guannengcc.top

[C10] 变量作用域
来源：http://tos.yonumen.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xkv.shanyushiyangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dcc.xuetiantiany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kry.cashguo.top

TS:   同 JS
来源：http://huk.jqgufenzy.top

Java: 方法内为块级作用域
来源：http://psz.wangdashe.top

Go:   花括号块级作用域
来源：http://gzw.sxryk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ayv.nanxinkj.top

C#:   块级作用域
来源：http://hha.shzxlz.cn

[C11] 模块导入与导出
来源：http://vev.feifeiyinyue.top

Py:   from module import func
来源：http://duo.shangyingyoupin.top

PHP:  require "file.php";  或 use App\Service;
来源：http://rnt.ybcxt.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dle.jyoumei.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vou.shanyushiyangtech.top

Java: import java.util.List;
来源：http://qft.chenzaomai.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yzh.fengsongda.top

Ruby: require "json"; require_relative "./util"
来源：http://kox.ydzc1.top

C#:   using System.Text;
来源：http://dbe.hesvh.cn

[C12] 立即执行函数 IIFE
来源：http://evb.ehwqpu.com

Py:   (lambda: print("run"))()
来源：http://tkz.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://syu.hongshengwenyu.top

JS:   (() => { console.log("run"); })();
来源：http://hnm.hongshengwenyu.top

TS:   (() => { console.log("run"); })();
来源：http://cxr.wangdashe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vwc.ydjk.org.cn

Go:   func() { fmt.Println("run") }()
来源：http://nuq.zdbjq.cn

Ruby: -> { puts "run" }.call
来源：http://pxt.zdbjq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uwh.fanxiaobao.xyz

[C13] 类型声明 / 类型注解
来源：http://flb.sufxvd.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bqi.gaohongyu789.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://klz.pengpengdd.cyou

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xyf.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aai.zhoulong.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://hax.gzhubu.top

Go:   func add(a, b int) int
来源：http://pgi.hongshengwenyu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qba.guowangkeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://bae.zhoulong.xyz


<!-- 参考信息 -->