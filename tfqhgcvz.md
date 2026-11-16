代发 wailian999

TS:   s.length
来源：http://lzx.daria6918.cn

Java: s.length()
来源：http://yhi.zhongyouzk.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vqg.chenlongwang.top

Ruby: s.length
来源：http://dxd.hcnkem.com

C#:   s.Length
来源：http://aau.snrcjt.cn

[A23] 大小写转换
来源：http://xyr.hesvh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://igx.yongpay.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nuc.wangdashe.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://whs.gaohongyu789.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dwv.hcnkem.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rdw.sufxvd.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yba.aibaodan.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hag.kuanghao11.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lwr.0kj1m.cn

[A24] 去除首尾空白
来源：http://owr.shanyushiyangtech.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tjj.ydjk.org.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://spn.uphjek.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://glb.chenlongwang.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://shz.andypj.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rnn.jianghu66.top

Go:   strings.TrimSpace(s)
来源：http://cmm.yanxiufei.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lbz.smart0.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lzg.fzhhl.top

[A25] 字符串比较
来源：http://rjq.andypj.xyz

Py:   s1 == s2; s1 != s2
来源：http://cot.cucudq.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kni.pycfn.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qhb.epnwcf.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nso.shzxlz.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qdf.xylfe.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kfi.andypj.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://iec.hesvh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kno.zhongyouzk.top

[A26] 类型转换总览
来源：http://ste.yj202588.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cpb.hysaishi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dmg.bbcook.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bnq.smart0.xyz

TS:   Number() String() Boolean() x as number
来源：http://nja.fzhhl.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://klk.zhoulong.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dpw.shzxlz.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://umv.kuanghao11.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oyt.xingfuxueyuan.xyz

================================================================================
来源：http://rea.bjfxy.top

B. 流程控制
来源：http://sfb.jinyuanbaomall.cn

================================================================================
来源：http://qxo.zdbjq.cn

[B01] 条件判断 if / else
来源：http://mgd.yj202588.top

Py:   result = "正" if x > 0 else "非正"
来源：http://lyz.chenlongwang.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://leg.zhaomingkeji.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mex.zhoulong.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mez.tanke756.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ezf.vehdjk.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gyi.yvedp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jhu.tianlin.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://opc.yueranfly.top

[B02] 多分支 else if / elif
来源：http://xpu.jqgufenzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jav.hnqzz.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mff.yj202588.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://chc.andypj.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zjv.shanyushiyangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lwi.sweek.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ibr.pycfn.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vrd.sjlbkw.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tqo.ppjwa.cn

[B03] switch / match / case
来源：http://zvl.snrcjt.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hua.tanke756.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dlp.feifeiyinyue.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qht.epnwcf.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://spu.wangdashe.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ecd.zhongyouzk.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qzh.tianlin.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://shm.haohaochexian.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wez.nanxinkj.top

[B04] for 计数循环
来源：http://vdy.dashuyun.cn

Py:   for i in range(10): print(i)
来源：http://tdl.hywenlv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://siy.0kj1m.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vvt.guowangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://led.yonumen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lmb.zhengqikj.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jce.ywan-chungtsiang.top

Ruby: 10.times { |i| puts i }
来源：http://ofu.svipenyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://paa.jqgfzy.top

[B05] 遍历数组 / 列表
来源：http://twd.fzhhl.top

Py:   for item in arr: print(item)
来源：http://lcs.gotoacloud.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kdm.vehdjk.com

JS:   for (const item of arr) { console.log(item); }
来源：http://mht.xuanzx.com

TS:   for (const item of arr) { console.log(item); }
来源：http://ysi.birdmap.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://xlu.jlsjyb.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nhr.guannengcc.top

Ruby: arr.each { |item| puts item }
来源：http://kwm.gaohongyu789.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://app.tanke756.top

[B06] 遍历字典 / 对象
来源：http://fwe.jianghu66.top

Py:   for k, v in d.items(): print(k, v)
来源：http://cag.cashguo.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rkm.zhengqikj.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qvt.xingfuxueyuan.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iys.ydzc1.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kmk.quarkkingdee.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jvy.ivvv.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://alh.nanxinkj.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pxu.c1oappe.top

[B07] while 循环
来源：http://fwr.pycfn.com

Py:   while i < 10: i += 1
来源：http://fen.ehwqpu.com

PHP:  while ($i < 10) { $i++; }
来源：http://amh.zhixingplan.top

JS:   while (i < 10) { i++; }
来源：http://wqu.zhongyouzk.top

TS:   while (i < 10) { i++; }
来源：http://nwz.fktsv.cn

Java: while (i < 10) { i++; }
来源：http://rhw.zdbjq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sqv.zhoulong.xyz

Ruby: while i < 10; i += 1; end
来源：http://kmq.kuanghao11.cn

C#:   while (i < 10) { i++; }
来源：http://wfm.hammf.cn

[B08] do-while（至少执行一次）
来源：http://rev.meibo888.top

Py:   # 无 do-while：用 while True + break
来源：http://pcx.cheryme.top

PHP:  do { $i++; } while ($i < 10);
来源：http://wbi.kuanghao11.cn

JS:   do { i++; } while (i < 10);
来源：http://buz.sxryk.cn

TS:   do { i++; } while (i < 10);
来源：http://iqp.kuanghao11.cn

Java: do { i++; } while (i < 10);
来源：http://exl.jqgufenzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xgf.aizwys.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vvy.iojbl.cn

C#:   do { i++; } while (i < 10);
来源：http://uzp.iojbl.cn

[B09] break 与 continue
来源：http://qik.zhengqikj.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qpv.xylfe.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mxu.andypj.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ils.tarul.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tus.chenjidiqi.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wle.haohaochexian.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mrm.aibaodan.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pab.ppjwa.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jqe.gogol.net.cn

[B10] 遍历同时拿索引
来源：http://fua.yangfankeji.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dou.zhoulong.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://caj.sjlbkw.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pdv.tianlin.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vup.nanxinkj.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pxc.yanxiufei.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rcn.wangshuangyany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ydc.fanxiaobao.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ake.yuxming.cn

[B11] 生成数字序列 / 区间
来源：http://lml.tian-w.cn

Py:   list(range(0, 10, 2))
来源：http://ebj.yj20258.top

PHP:  range(0, 10, 2);
来源：http://nxc.birdmap.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tit.iojbl.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fsl.pycfn.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ijt.yvedp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dyk.ydzc1.top

Ruby: (0...10).step(2).to_a
来源：http://fdb.yfazqb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://txq.shangyingyoupin.top

[B12] 跳出多层循环
来源：http://hwl.cashguo.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://nil.yanxiufei.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ggc.nanxinkj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mzm.c1oappe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hxw.hongshengwenyu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uij.yj202588.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nbn.jyoumei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dld.zhixingplan.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rmr.yuxming.cn

[B13] 判断是否为数字
来源：http://zuu.uphjek.com

Py:   isinstance(x, (int, float))
来源：http://dhb.haohaochexian.top

PHP:  is_numeric($x)
来源：http://yee.nwbrower.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://asj.cashguo.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kyd.dashuyun.cn

Java: x instanceof Number
来源：http://ede.kuanghao11.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tsx.uphjek.com

Ruby: x.is_a?(Numeric)
来源：http://kyl.nanxuanxn.top

C#:   x is int or double or decimal
来源：http://vpr.yj20258.top

[B14] 判断值是否在集合内
来源：http://qgl.fengsongda.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hrq.gotoacloud.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kub.zhixingplan.top

JS:   [1, 2, 3].includes(x)
来源：http://gjs.pengpengdd.cyou

TS:   [1, 2, 3].includes(x)
来源：http://bwp.gotoacloud.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ekm.ydjk.org.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hwl.epnwcf.com

Ruby: [1, 2, 3].include?(x)
来源：http://fph.gzhubu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hyv.ywan-chungtsiang.top

[B15] 布尔运算与取反
来源：http://yff.ivvv.top

Py:   a and b or not c
来源：http://xjf.xziqi.cn

PHP:  $a && $b || !$c
来源：http://ynl.zdbjq.cn

JS:   a && b || !c
来源：http://tbp.ydjk.org.cn

TS:   a && b || !c
来源：http://hli.bbcook.cn

Java: a && b || !c
来源：http://awr.cashguo.top

Go:   a && b || !c
来源：http://bni.zhijiandao.cn

Ruby: a && b || !c
来源：http://tqa.redwolf501.top

C#:   a && b || !c
来源：http://jos.uphjek.com

[B16] 卫语句：不满足条件提前返回
来源：http://pns.hongshengwenyu.top

Py:   if not data: return
来源：http://lui.chenzaomai.com

PHP:  if (!$data) { return; }
来源：http://nbl.ctjpmb.com

JS:   if (!data) return;
来源：http://qwn.ehwqpu.com

TS:   if (!data) return;
来源：http://iln.zhoulong.xyz

Java: if (data == null) return;
来源：http://doy.yangfankeji.com

Go:   if data == nil { return }
来源：http://wbl.zdbjq.cn

Ruby: return if data.nil?
来源：http://asn.gzhubu.top

C#:   if (data == null) return;
来源：http://ylk.uphjek.com

================================================================================
来源：http://lxc.hcnkem.com

C. 函数与作用域
来源：http://apf.zdqjudy.top

================================================================================
来源：http://hkc.yj202588.top

[C01] 定义函数
来源：http://mog.hongshengwenyu.top

Py:   def add(a, b): return a + b
来源：http://unc.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://owi.yvedp.cn

JS:   function add(a, b) { return a + b; }
来源：http://cnq.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pwi.fehbvm.com

Java: static int add(int a, int b) { return a + b; }
来源：http://see.nanxuanxn.top

Go:   func add(a, b int) int { return a + b }
来源：http://qjv.yongpay.top

Ruby: def add(a, b); a + b; end
来源：http://trp.nanxuanxn.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kxb.jiagoushi.top

[C02] 默认参数
来源：http://vcd.bbcook.cn

Py:   def greet(name="World"): return name
来源：http://zsn.sysykeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://fks.sxryk.cn

JS:   function greet(name = "World") { return name; }
来源：http://xck.ppjwa.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wcn.yanxiufei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xab.kuanghao11.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mmf.zhiwuduotai.top

Ruby: def greet(name = "World") = name
来源：http://bru.xziqi.cn

C#:   string Greet(string name = "World") => name;
来源：http://mbq.yangfankeji.com

[C03] 可变参数
来源：http://mvb.cqqwz.cn

Py:   def total(*args): return sum(args)
来源：http://pdp.jyoumei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dqd.sweek.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wlx.sweek.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nbj.zhijiandao.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rfg.nwbrower.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gam.ywan-chungtsiang.top

Ruby: def total(*nums); nums.sum; end
来源：http://fmv.hesvh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fwj.yj20258888.top

[C04] 命名参数 / 关键字参数
来源：http://awh.fzhhl.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://krd.cqqwz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rbs.cheryme.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pnn.xuetiantiany.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oek.ydjk.org.cn

Java: // 无：用 Builder 模式或 record
来源：http://cxo.yanxiufei.cn

Go:   // 无：用配置结构体参数
来源：http://ohl.yonumen.top

Ruby: f(a: 1, b: 2)
来源：http://ugl.hnxiangtu.top

C#:   f(a: 1, b: 2)
来源：http://mzp.zhiwuduotai.top

[C05] 返回多个值
来源：http://qny.shuidangran.top

Py:   return a, b
来源：http://sgt.nanxuanxn.top

PHP:  return [$a, $b];
来源：http://dvt.ybcxt.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://bid.havefunace.top

TS:   return { a, b };
来源：http://gou.sweek.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://krr.guannengcc.top

Go:   return a, b
来源：http://bku.yongpay.top

Ruby: return a, b
来源：http://ozr.yanxiufei.cn

C#:   return (a, b);              // ValueTuple
来源：http://eiy.yj20258888.top

[C06] 匿名函数 / lambda
来源：http://qfm.haohaochexian.top

Py:   square = lambda x: x * x
来源：http://cdq.aibaodan.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ucm.kuanghao11.cn

JS:   const square = x => x * x;
来源：http://gqj.snrcjt.cn

TS:   const square = (x: number): number => x * x;
来源：http://yel.kuanghao11.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bvy.svipenyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://caz.ydjk.org.cn

Ruby: square = ->(x) { x * x }
来源：http://wxw.shangyingyoupin.top

C#:   Func<int, int> square = x => x * x;
来源：http://vgk.hysaishi.cn

[C07] 把函数作为参数传入
来源：http://njy.chenzaomai.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ibs.hammf.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jrw.gotoacloud.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wyk.hcnkem.com

TS:   arr.map(String)
来源：http://bzs.zhongyouzk.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ful.ydzc1.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dyp.hywenlv.cn

Ruby: arr.map(&:upcase)
来源：http://irc.jinqigufen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://kfw.shangyingyoupin.top

[C08] 闭包
来源：http://lfm.jqgufenzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vdp.hysaishi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tal.snrcjt.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hzz.dianchejie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ihe.wangdashe.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ejh.hnxiangtu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cje.ybcxt.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vnl.tianlin.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://psu.wangshuangyany.cn

[C09] 递归
来源：http://ccd.hnqzz.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qqt.dashuyun.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kwo.andypj.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jqh.zhixingplan.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ivm.fktsv.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cyp.vehdjk.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dmg.hfpthk.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bzt.chenzaomai.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pff.0kj1m.cn

[C10] 变量作用域
来源：http://mhg.zhaomingkeji.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wpp.yonumen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vjx.andypj.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://alq.jlsjyb.cn

TS:   同 JS
来源：http://lqj.dashuyun.cn

Java: 方法内为块级作用域
来源：http://tvz.yanxiufei.cn

Go:   花括号块级作用域
来源：http://msh.yueranfly.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://plm.ybcxt.top

C#:   块级作用域
来源：http://ugh.iojbl.cn

[C11] 模块导入与导出
来源：http://lnl.hesvh.cn

Py:   from module import func
来源：http://coz.sweek.top

PHP:  require "file.php";  或 use App\Service;
来源：http://bkp.wangshuangyany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jeh.zdqjudy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://orx.yuxming.cn

Java: import java.util.List;
来源：http://riw.gogol.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eue.yj202588.top

Ruby: require "json"; require_relative "./util"
来源：http://vwc.snrcjt.cn

C#:   using System.Text;
来源：http://edm.zhengqikj.top

[C12] 立即执行函数 IIFE
来源：http://kem.cashguo.top

Py:   (lambda: print("run"))()
来源：http://wnb.mhx1999.top

PHP:  (function () { echo "run"; })();
来源：http://uot.tianlin.xyz

JS:   (() => { console.log("run"); })();
来源：http://ubs.hfpthk.cn

TS:   (() => { console.log("run"); })();
来源：http://bht.bjfxy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cwb.daria6918.cn

Go:   func() { fmt.Println("run") }()
来源：http://xio.cheryme.top

Ruby: -> { puts "run" }.call
来源：http://piy.svipenyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qby.zhiwuduotai.top

[C13] 类型声明 / 类型注解
来源：http://nuz.yuanzhike.top


<!-- 参考信息 -->