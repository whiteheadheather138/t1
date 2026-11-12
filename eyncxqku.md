代发 wailian999

TS:   s.length
来源：http://hlx.ywan-chungtsiang.top

Java: s.length()
来源：http://pbx.zhengqikj.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bmr.birdmap.top

Ruby: s.length
来源：http://nap.zhaomingkeji.xyz

C#:   s.Length
来源：http://gqv.52xcode.cn

[A23] 大小写转换
来源：http://lix.fanxiaobao.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://tgc.cucudq.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xjo.jinqigfzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fnw.ydzc1.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wqd.ehwqpu.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rph.sjlbkw.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cue.aizwys.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nnt.haohaochexian.top

C#:   s.ToUpper(); s.ToLower()
来源：http://see.jyoumei.cn

[A24] 去除首尾空白
来源：http://lfg.c1oappe.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hcu.nanxuanxn.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kbw.smart0.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ibm.c1oappe.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yhd.shzxlz.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ltt.jianghu66.top

Go:   strings.TrimSpace(s)
来源：http://bau.jqgufenzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kun.zdqjudy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qrs.hnxiangtu.top

[A25] 字符串比较
来源：http://xoc.yonumen.top

Py:   s1 == s2; s1 != s2
来源：http://fgy.tian-w.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mpt.gotoacloud.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cje.jinqigfzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yly.tanke756.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://suf.sufxvd.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wve.fanxiaobao.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://htx.hammf.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mzw.zdbjq.cn

[A26] 类型转换总览
来源：http://jvd.ywan-chungtsiang.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://meg.fanxiaobao.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pbz.cqqwz.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lyu.0kj1m.cn

TS:   Number() String() Boolean() x as number
来源：http://hfh.smart0.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zbn.gogol.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kmf.gaohongyu789.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://qiw.shuidangran.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://etx.aizwys.cn

================================================================================
来源：http://pvz.birdmap.top

B. 流程控制
来源：http://xxh.jiagoushi.top

================================================================================
来源：http://laf.zdqjudy.top

[B01] 条件判断 if / else
来源：http://vbg.fktsv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mbs.wangshuangyany.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zjr.yongpay.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://omt.zhengqikj.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tms.ehwqpu.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://olv.sweek.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cux.tarul.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vje.vqdsnc.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fyd.316326.xyz

[B02] 多分支 else if / elif
来源：http://knv.chenlongwang.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ylk.ivvv.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://crk.sjlbkw.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xmu.yfazqb.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ukq.zycfv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vlu.yueranfly.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sbo.jinyuanbaomall.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xcm.yuxming.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iyd.fzhhl.top

[B03] switch / match / case
来源：http://nga.zhengqikj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jwh.jiagoushi.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://igc.xuanzx.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://afa.sweek.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nal.guannengcc.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://aqa.yuanzhike.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pvt.ydzc1.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://chs.dianchejie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nqo.svipenyu.cn

[B04] for 计数循环
来源：http://cme.aibaodan.cn

Py:   for i in range(10): print(i)
来源：http://jbd.wangdashe.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yew.yongpay.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ebd.snrcjt.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://evq.52xcode.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jag.c1oappe.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zow.pengpengdd.cyou

Ruby: 10.times { |i| puts i }
来源：http://zro.chenjidiqi.icu

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gqg.yonumen.top

[B05] 遍历数组 / 列表
来源：http://wir.epnwcf.com

Py:   for item in arr: print(item)
来源：http://qtw.birdmap.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jyy.zhoulong.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://xyh.jlsjyb.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://phz.jyoumei.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://goe.fengsongda.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xxg.ehwqpu.com

Ruby: arr.each { |item| puts item }
来源：http://znp.cashguo.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pdz.ctjpmb.com

[B06] 遍历字典 / 对象
来源：http://adr.nwbrower.top

Py:   for k, v in d.items(): print(k, v)
来源：http://lhf.zhixingplan.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ysc.tianlin.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vuy.zhengqikj.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yym.gotoacloud.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xbq.xziqi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oyk.gogol.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zyv.andypj.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uwg.shanyushiyangtech.top

[B07] while 循环
来源：http://hrr.daxiang520.top

Py:   while i < 10: i += 1
来源：http://gdl.zhongyouzk.top

PHP:  while ($i < 10) { $i++; }
来源：http://erl.9152youxi.cn

JS:   while (i < 10) { i++; }
来源：http://ghw.bjfxy.top

TS:   while (i < 10) { i++; }
来源：http://tws.c1oappe.top

Java: while (i < 10) { i++; }
来源：http://fdx.jinghuilouyu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hjj.sufxvd.cn

Ruby: while i < 10; i += 1; end
来源：http://yhi.xingfuxueyuan.xyz

C#:   while (i < 10) { i++; }
来源：http://myt.shanyushiyangkeji.top

[B08] do-while（至少执行一次）
来源：http://kwa.xuanzx.com

Py:   # 无 do-while：用 while True + break
来源：http://lal.xingfuxueyuan.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://sce.quarkkingdee.top

JS:   do { i++; } while (i < 10);
来源：http://yep.iojbl.cn

TS:   do { i++; } while (i < 10);
来源：http://ydf.guannengcc.top

Java: do { i++; } while (i < 10);
来源：http://vwg.zhongyouzk.top

Go:   for { i++; if i >= 10 { break } }
来源：http://lwz.xylfe.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rmr.jinghuilouyu.cn

C#:   do { i++; } while (i < 10);
来源：http://nna.nanxuanxn.top

[B09] break 与 continue
来源：http://ikt.vqdsnc.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wqs.zhixingplan.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://var.quarkkingdee.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xyh.shangyingyoupin.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tjq.havefunace.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lpz.ywan-chungtsiang.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pag.jqgfzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jjo.fehbvm.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lnp.xingfuxueyuan.xyz

[B10] 遍历同时拿索引
来源：http://rgu.tianlin.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jew.ehwqpu.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://npr.zhengqikj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zrx.jlsjyb.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zew.wangshuangyany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://opq.yfazqb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mwr.zdqjudy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://isz.yangfankeji.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bbe.zhijiandao.cn

[B11] 生成数字序列 / 区间
来源：http://yoh.aizwys.cn

Py:   list(range(0, 10, 2))
来源：http://jbm.jianghu66.top

PHP:  range(0, 10, 2);
来源：http://jyr.shuidangran.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://csz.fehbvm.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jrl.yuanzhike.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kha.yuanzhike.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://axb.ydjk.org.cn

Ruby: (0...10).step(2).to_a
来源：http://avp.xylfe.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xwh.sxryk.cn

[B12] 跳出多层循环
来源：http://gsr.hesvh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uvb.xziqi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vng.guannengcc.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xyl.jinqigufen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ngd.yfazqb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eyl.zhiwuduotai.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pgv.jinqigfzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xig.smart0.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cui.hesvh.cn

[B13] 判断是否为数字
来源：http://cyg.zhiwuduotai.top

Py:   isinstance(x, (int, float))
来源：http://ric.daxiang520.top

PHP:  is_numeric($x)
来源：http://rod.hfpthk.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lrq.yongpay.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vkb.xingfuxueyuan.xyz

Java: x instanceof Number
来源：http://mdq.yfazqb.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mbl.c1oappe.top

Ruby: x.is_a?(Numeric)
来源：http://vvi.9152youxi.cn

C#:   x is int or double or decimal
来源：http://ntf.zhijiandao.cn

[B14] 判断值是否在集合内
来源：http://cwa.zhoulong.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ujj.sjlbkw.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://usd.dianchejie.cn

JS:   [1, 2, 3].includes(x)
来源：http://oaq.xingfuxueyuan.xyz

TS:   [1, 2, 3].includes(x)
来源：http://ybp.jqgufenzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zfm.mhx1999.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uuv.hesvh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hdy.zhijiandao.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xef.jqgfzy.top

[B15] 布尔运算与取反
来源：http://gec.smart0.xyz

Py:   a and b or not c
来源：http://ljd.quarkkingdee.top

PHP:  $a && $b || !$c
来源：http://hcx.cdnleiting.top

JS:   a && b || !c
来源：http://uga.cdnleiting.top

TS:   a && b || !c
来源：http://mgc.yj202588.top

Java: a && b || !c
来源：http://uvw.ywan-chungtsiang.top

Go:   a && b || !c
来源：http://blr.yj20258888.top

Ruby: a && b || !c
来源：http://gnh.gaohongyu789.top

C#:   a && b || !c
来源：http://pmm.ctjpmb.com

[B16] 卫语句：不满足条件提前返回
来源：http://tth.yvedp.cn

Py:   if not data: return
来源：http://ycc.vqdsnc.cn

PHP:  if (!$data) { return; }
来源：http://fod.sysykeji.top

JS:   if (!data) return;
来源：http://gtr.zhixingplan.top

TS:   if (!data) return;
来源：http://jsx.ydzc1.top

Java: if (data == null) return;
来源：http://gnv.jianghu66.top

Go:   if data == nil { return }
来源：http://wes.kuanghao11.cn

Ruby: return if data.nil?
来源：http://lxi.zhiwuduotai.top

C#:   if (data == null) return;
来源：http://kyk.xuetiantiany.cn

================================================================================
来源：http://pxf.svipenyu.cn

C. 函数与作用域
来源：http://kzm.pycfn.com

================================================================================
来源：http://kln.yj20258888.top

[C01] 定义函数
来源：http://uku.fanxiaobao.xyz

Py:   def add(a, b): return a + b
来源：http://zxo.gaohongyu789.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://txl.zycfv.cn

JS:   function add(a, b) { return a + b; }
来源：http://cvg.jqgufenzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cvf.snrcjt.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zfp.feifeiyinyue.top

Go:   func add(a, b int) int { return a + b }
来源：http://twq.fengsongda.top

Ruby: def add(a, b); a + b; end
来源：http://prs.hnqzz.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qky.svipenyu.cn

[C02] 默认参数
来源：http://ggd.dashuyun.cn

Py:   def greet(name="World"): return name
来源：http://ltq.wangdashe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bdo.yj20258888.top

JS:   function greet(name = "World") { return name; }
来源：http://jlb.316326.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://zff.shanyushiyangkeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dlu.gaohongyu789.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sow.uphjek.com

Ruby: def greet(name = "World") = name
来源：http://emj.jianghu66.top

C#:   string Greet(string name = "World") => name;
来源：http://tjm.gaohongyu789.top

[C03] 可变参数
来源：http://uos.yuxming.cn

Py:   def total(*args): return sum(args)
来源：http://sdm.yueranfly.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cmk.yangfankeji.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://chc.hesvh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eux.jinyuanbaomall.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lng.hfpthk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://whq.gotoacloud.top

Ruby: def total(*nums); nums.sum; end
来源：http://pys.wangshuangyany.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eak.jiagoushi.top

[C04] 命名参数 / 关键字参数
来源：http://zsr.316326.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hpy.hnxiangtu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zlb.gaohongyu789.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://axj.andypj.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xew.wangdashe.top

Java: // 无：用 Builder 模式或 record
来源：http://sys.quarkkingdee.top

Go:   // 无：用配置结构体参数
来源：http://ono.hfpthk.cn

Ruby: f(a: 1, b: 2)
来源：http://egr.hongshengwenyu.top

C#:   f(a: 1, b: 2)
来源：http://mkf.chenzaomai.com

[C05] 返回多个值
来源：http://zbd.ydjk.org.cn

Py:   return a, b
来源：http://mby.zhiwuduotai.top

PHP:  return [$a, $b];
来源：http://yko.sjlbkw.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vzf.fzhhl.top

TS:   return { a, b };
来源：http://hju.c1oappe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nri.yonumen.top

Go:   return a, b
来源：http://hbh.birdmap.top

Ruby: return a, b
来源：http://iik.cqqwz.cn

C#:   return (a, b);              // ValueTuple
来源：http://wlx.jinghuilouyu.cn

[C06] 匿名函数 / lambda
来源：http://ioi.jinyuanbaomall.cn

Py:   square = lambda x: x * x
来源：http://yla.tanke756.top

PHP:  $square = fn($x) => $x * $x;
来源：http://thw.kuanghao11.cn

JS:   const square = x => x * x;
来源：http://gvc.xuetiantiany.cn

TS:   const square = (x: number): number => x * x;
来源：http://eok.andypj.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kvr.jiagoushi.top

Go:   sq := func(x int) int { return x * x }
来源：http://yxc.xylfe.cn

Ruby: square = ->(x) { x * x }
来源：http://rka.9152youxi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lvv.tanke756.top

[C07] 把函数作为参数传入
来源：http://gfq.zhengqikj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vsh.jianghu66.top

PHP:  array_map("strtoupper", $arr);
来源：http://bjw.cashguo.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gny.ppjwa.cn

TS:   arr.map(String)
来源：http://hna.xuetiantiany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hus.yuanzhike.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wdc.hnqzz.top

Ruby: arr.map(&:upcase)
来源：http://dmu.epnwcf.com

C#:   arr.Select(s => s.ToUpper())
来源：http://tdk.jqgufenzy.top

[C08] 闭包
来源：http://wxb.shangyingyoupin.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ygh.daxiang520.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://epw.jinqigfzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pee.xylfe.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rkf.yueranfly.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lmj.daria6918.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rds.ctjpmb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hjg.xinyue.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bqb.hywenlv.cn

[C09] 递归
来源：http://gal.zhijiandao.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rse.hnxiangtu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wvh.iojbl.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hhc.fehbvm.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uvf.meibo888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zdb.yj20258888.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vth.316326.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dax.pycfn.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://czq.birdmap.top

[C10] 变量作用域
来源：http://plc.ydzc1.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bjo.ydzc1.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rmh.jinqigufen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ahd.chenjidiqi.icu

TS:   同 JS
来源：http://hrq.xziqi.cn

Java: 方法内为块级作用域
来源：http://qqu.gogol.net.cn

Go:   花括号块级作用域
来源：http://uec.hammf.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ewe.yuanzhike.top

C#:   块级作用域
来源：http://sxq.316326.xyz

[C11] 模块导入与导出
来源：http://hxo.nwbrower.top

Py:   from module import func
来源：http://xpn.redwolf501.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dfz.tian-w.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bvd.wangshuangyany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://khp.gaohongyu789.top

Java: import java.util.List;
来源：http://mvd.hywenlv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zvs.tianlin.xyz

Ruby: require "json"; require_relative "./util"
来源：http://qdp.shanyushiyangtech.top

C#:   using System.Text;
来源：http://tnz.dianchejie.cn

[C12] 立即执行函数 IIFE
来源：http://qjz.yj20258888.top

Py:   (lambda: print("run"))()
来源：http://wdf.vehdjk.com

PHP:  (function () { echo "run"; })();
来源：http://aza.gotoacloud.top

JS:   (() => { console.log("run"); })();
来源：http://vao.jinghuilouyu.cn

TS:   (() => { console.log("run"); })();
来源：http://ivx.ppjwa.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yqh.cashguo.top

Go:   func() { fmt.Println("run") }()
来源：http://dlm.tanke756.top

Ruby: -> { puts "run" }.call
来源：http://hoy.ybcxt.top

C#:   // 无 IIFE：用静态构造函数
来源：http://llh.fzhhl.top

[C13] 类型声明 / 类型注解
来源：http://zxn.yongpay.top


<!-- 参考信息 -->