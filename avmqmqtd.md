代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hrl.dashuyun.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://can.ivvv.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jpt.quarkkingdee.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tut.sxryk.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lbn.nanxuanxn.top

C#:   s.ToUpper(); s.ToLower()
来源：http://zpd.jiagoushi.top

[A24] 去除首尾空白
来源：http://ddn.0kj1m.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nql.hysaishi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rzs.pycfn.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dnn.yanxiufei.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nav.fzhhl.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kxl.cqqwz.cn

Go:   strings.TrimSpace(s)
来源：http://fmx.bjfxy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ohq.ehwqpu.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://utt.pengpengdd.cyou

[A25] 字符串比较
来源：http://lhf.meibo888.top

Py:   s1 == s2; s1 != s2
来源：http://zvq.jlsjyb.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://exb.cucudq.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://eed.hywenlv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fqd.gaohongyu789.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cvv.yfazqb.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zwn.zycfv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xpy.jinqigfzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kff.pycfn.com

[A26] 类型转换总览
来源：http://evl.zycfv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ndz.shuidangran.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fys.zhiwuduotai.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gar.fehbvm.com

TS:   Number() String() Boolean() x as number
来源：http://wav.hfpthk.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ezp.ywan-chungtsiang.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hfc.shanyushiyangkeji.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://rgn.nwbrower.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gsr.fktsv.cn

================================================================================
来源：http://jap.jqgfzy.top

B. 流程控制
来源：http://dxn.redwolf501.top

================================================================================
来源：http://nag.yuxming.cn

[B01] 条件判断 if / else
来源：http://shw.ywan-chungtsiang.top

Py:   result = "正" if x > 0 else "非正"
来源：http://uca.gzhubu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gly.jyoumei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lja.xuetiantiany.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gou.chenzaomai.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://apk.haohaochexian.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cse.ybcxt.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bxr.hongshengwenyu.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ils.jiagoushi.top

[B02] 多分支 else if / elif
来源：http://fph.jqgfzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dkl.andypj.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tqb.xinyue.icu

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://evx.svipenyu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nhk.hongshengwenyu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xbr.zhaomingkeji.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vab.pycfn.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ywy.uphjek.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kez.gotoacloud.top

[B03] switch / match / case
来源：http://mre.yfazqb.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://oad.nanxuanxn.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yxa.mhx1999.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hkb.xziqi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rqt.cashguo.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fee.dashuyun.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qhc.wangdashe.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://flb.aibaodan.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://icz.chenlongwang.top

[B04] for 计数循环
来源：http://sug.hesvh.cn

Py:   for i in range(10): print(i)
来源：http://icu.sweek.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jgt.vqdsnc.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ias.gogol.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://txg.hcnkem.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gkt.bbcook.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qmi.gaohongyu789.top

Ruby: 10.times { |i| puts i }
来源：http://mna.haohaochexian.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xrs.zhiwuduotai.top

[B05] 遍历数组 / 列表
来源：http://bsv.zhixingplan.top

Py:   for item in arr: print(item)
来源：http://msn.hnxiangtu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nzj.uphjek.com

JS:   for (const item of arr) { console.log(item); }
来源：http://xxv.nwbrower.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qtn.yvedp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://uvx.xuanzx.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lau.sweek.top

Ruby: arr.each { |item| puts item }
来源：http://qcv.sufxvd.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wcx.cdnleiting.top

[B06] 遍历字典 / 对象
来源：http://ule.shangyingyoupin.top

Py:   for k, v in d.items(): print(k, v)
来源：http://fsz.jiagoushi.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wli.sysykeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zdf.pycfn.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ubb.birdmap.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lko.xuetiantiany.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rui.vqdsnc.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://smc.zdbjq.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bvx.fehbvm.com

[B07] while 循环
来源：http://prk.mhx1999.top

Py:   while i < 10: i += 1
来源：http://ija.yangfankeji.com

PHP:  while ($i < 10) { $i++; }
来源：http://ptz.iojbl.cn

JS:   while (i < 10) { i++; }
来源：http://xun.uphjek.com

TS:   while (i < 10) { i++; }
来源：http://dnj.meibo888.top

Java: while (i < 10) { i++; }
来源：http://jgk.hnqzz.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kca.fzhhl.top

Ruby: while i < 10; i += 1; end
来源：http://mjg.xinyue.icu

C#:   while (i < 10) { i++; }
来源：http://ist.yonumen.top

[B08] do-while（至少执行一次）
来源：http://sad.snrcjt.cn

Py:   # 无 do-while：用 while True + break
来源：http://opp.yj202588.top

PHP:  do { $i++; } while ($i < 10);
来源：http://oni.jinghuilouyu.cn

JS:   do { i++; } while (i < 10);
来源：http://uga.yfazqb.com

TS:   do { i++; } while (i < 10);
来源：http://rll.andypj.xyz

Java: do { i++; } while (i < 10);
来源：http://hyq.gotoacloud.top

Go:   for { i++; if i >= 10 { break } }
来源：http://age.nanxuanxn.top

Ruby: begin; i += 1; end while i < 10
来源：http://kjb.andypj.xyz

C#:   do { i++; } while (i < 10);
来源：http://dng.tian-w.cn

[B09] break 与 continue
来源：http://jas.shzxlz.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dgl.chenzaomai.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ojr.svipenyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://whb.smart0.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nzt.yuanzhike.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ieq.hongshengwenyu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vzv.ivvv.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ozz.vqdsnc.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gih.jlsjyb.cn

[B10] 遍历同时拿索引
来源：http://qps.ivvv.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mms.redwolf501.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rap.tarul.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uvc.ehwqpu.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://avy.jinyuanbaomall.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cqs.xylfe.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zfb.daxiang520.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cwq.hesvh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://obb.aizwys.cn

[B11] 生成数字序列 / 区间
来源：http://gtj.ppjwa.cn

Py:   list(range(0, 10, 2))
来源：http://rej.yanxiufei.cn

PHP:  range(0, 10, 2);
来源：http://oqk.yonumen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zum.ybcxt.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kkt.yonumen.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hyx.hesvh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fyu.hongshengwenyu.top

Ruby: (0...10).step(2).to_a
来源：http://wyk.ppjwa.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rqk.hammf.cn

[B12] 跳出多层循环
来源：http://rya.jinqigfzy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://pql.guannengcc.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://wsr.yuxming.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mir.svipenyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ozl.jyoumei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://noi.ivvv.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qfk.zhiwuduotai.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mjl.hfpthk.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ghj.zhiwuduotai.top

[B13] 判断是否为数字
来源：http://wip.zdqjudy.top

Py:   isinstance(x, (int, float))
来源：http://lkz.tanke756.top

PHP:  is_numeric($x)
来源：http://amw.zdqjudy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fys.sxryk.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vxe.wangdashe.top

Java: x instanceof Number
来源：http://cxj.yj20258.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mep.chenjidiqi.icu

Ruby: x.is_a?(Numeric)
来源：http://uuh.yonumen.top

C#:   x is int or double or decimal
来源：http://ohs.jyoumei.cn

[B14] 判断值是否在集合内
来源：http://ksv.jinyuanbaomall.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://esz.quarkkingdee.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bur.gzhubu.top

JS:   [1, 2, 3].includes(x)
来源：http://oar.fehbvm.com

TS:   [1, 2, 3].includes(x)
来源：http://iik.haohaochexian.top

Java: List.of(1, 2, 3).contains(x)
来源：http://rxq.hfpthk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ruy.daria6918.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zoj.fengsongda.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kxe.zhijiandao.cn

[B15] 布尔运算与取反
来源：http://jbo.zhengqikj.top

Py:   a and b or not c
来源：http://zrk.yuanzhike.top

PHP:  $a && $b || !$c
来源：http://ccr.vqdsnc.cn

JS:   a && b || !c
来源：http://age.shzxlz.cn

TS:   a && b || !c
来源：http://pmd.chenlongwang.top

Java: a && b || !c
来源：http://zii.gotoacloud.top

Go:   a && b || !c
来源：http://lhb.epnwcf.com

Ruby: a && b || !c
来源：http://giw.cucudq.cn

C#:   a && b || !c
来源：http://afh.jiagoushi.top

[B16] 卫语句：不满足条件提前返回
来源：http://lty.iojbl.cn

Py:   if not data: return
来源：http://ywa.snrcjt.cn

PHP:  if (!$data) { return; }
来源：http://pxx.pengpengdd.cyou

JS:   if (!data) return;
来源：http://yim.daxiang520.top

TS:   if (!data) return;
来源：http://cra.ivvv.top

Java: if (data == null) return;
来源：http://pzv.yangfankeji.com

Go:   if data == nil { return }
来源：http://fpm.wangshuangyany.cn

Ruby: return if data.nil?
来源：http://iao.zhaomingkeji.xyz

C#:   if (data == null) return;
来源：http://dbv.zhiwuduotai.top

================================================================================
来源：http://xgp.tanke756.top

C. 函数与作用域
来源：http://cmo.ctjpmb.com

================================================================================
来源：http://ase.shuidangran.top

[C01] 定义函数
来源：http://cjy.dianchejie.cn

Py:   def add(a, b): return a + b
来源：http://rcg.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://unh.zhengqikj.top

JS:   function add(a, b) { return a + b; }
来源：http://qay.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://icb.ydzc1.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cdb.yanxiufei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cju.tian-w.cn

Ruby: def add(a, b); a + b; end
来源：http://ggg.gotoacloud.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xvu.c1oappe.top

[C02] 默认参数
来源：http://tzy.ydjk.org.cn

Py:   def greet(name="World"): return name
来源：http://jjh.yongpay.top

PHP:  function greet($name = "World") { return $name; }
来源：http://knk.hysaishi.cn

JS:   function greet(name = "World") { return name; }
来源：http://epl.jianghu66.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nna.guowangkeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vnx.gotoacloud.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gcn.jianghu66.top

Ruby: def greet(name = "World") = name
来源：http://ion.hysaishi.cn

C#:   string Greet(string name = "World") => name;
来源：http://ucw.hfpthk.cn

[C03] 可变参数
来源：http://cpz.sweek.top

Py:   def total(*args): return sum(args)
来源：http://fzk.zhijiandao.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://civ.shzxlz.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hoi.fengsongda.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cyk.hfpthk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bhw.cucudq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kca.zhoulong.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://iuc.nanxinkj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bop.shzxlz.cn

[C04] 命名参数 / 关键字参数
来源：http://nfv.zycfv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bbt.sxryk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oms.xylfe.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qgo.gzhubu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tit.daria6918.cn

Java: // 无：用 Builder 模式或 record
来源：http://uje.vqdsnc.cn

Go:   // 无：用配置结构体参数
来源：http://owv.nanxinkj.top

Ruby: f(a: 1, b: 2)
来源：http://tpp.hysaishi.cn

C#:   f(a: 1, b: 2)
来源：http://tcx.jlsjyb.cn

[C05] 返回多个值
来源：http://dee.daxiang520.top

Py:   return a, b
来源：http://ztk.cdnleiting.top

PHP:  return [$a, $b];
来源：http://naz.birdmap.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rez.svipenyu.cn

TS:   return { a, b };
来源：http://xor.dianchejie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wtt.sufxvd.cn

Go:   return a, b
来源：http://gci.jinghuilouyu.cn

Ruby: return a, b
来源：http://zwe.zhixingplan.top

C#:   return (a, b);              // ValueTuple
来源：http://edz.quarkkingdee.top

[C06] 匿名函数 / lambda
来源：http://xvc.ywan-chungtsiang.top

Py:   square = lambda x: x * x
来源：http://dcn.xziqi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tvo.jinghuilouyu.cn

JS:   const square = x => x * x;
来源：http://eit.tarul.cn

TS:   const square = (x: number): number => x * x;
来源：http://njj.ywan-chungtsiang.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mtw.zhiwuduotai.top

Go:   sq := func(x int) int { return x * x }
来源：http://leo.zhongyouzk.top

Ruby: square = ->(x) { x * x }
来源：http://qhf.shuidangran.top

C#:   Func<int, int> square = x => x * x;
来源：http://rxr.hysaishi.cn

[C07] 把函数作为参数传入
来源：http://xxq.chenzaomai.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bkz.zhongyouzk.top

PHP:  array_map("strtoupper", $arr);
来源：http://uip.ppjwa.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xxj.316326.xyz

TS:   arr.map(String)
来源：http://mdv.dashuyun.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hji.daxiang520.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yxb.sysykeji.top

Ruby: arr.map(&:upcase)
来源：http://evm.tianlin.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://dvb.andypj.xyz

[C08] 闭包
来源：http://get.birdmap.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bvy.hnqzz.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jnv.hywenlv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://iog.guowangkeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jnp.gzhubu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dge.yanxiufei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nsu.pycfn.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://goq.ydzc1.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://msq.52xcode.cn

[C09] 递归
来源：http://ulr.shuidangran.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gza.yonumen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bfs.chenzaomai.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://evp.ehwqpu.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dfs.sufxvd.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ofi.316326.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://stt.mhx1999.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uvp.yongpay.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qfk.xuanzx.com

[C10] 变量作用域
来源：http://ugf.cqqwz.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ocg.gotoacloud.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jdm.zhixingplan.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tjw.snrcjt.cn

TS:   同 JS
来源：http://hfe.c1oappe.top

Java: 方法内为块级作用域
来源：http://wzu.aizwys.cn

Go:   花括号块级作用域
来源：http://ozg.hongshengwenyu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dfj.ydzc1.top

C#:   块级作用域
来源：http://xog.ydzc1.top

[C11] 模块导入与导出
来源：http://eit.chenzaomai.com

Py:   from module import func
来源：http://hzn.ivvv.top

PHP:  require "file.php";  或 use App\Service;
来源：http://prc.52xcode.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://thv.tianlin.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://eag.feifeiyinyue.top

Java: import java.util.List;
来源：http://qfr.quarkkingdee.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zfh.fktsv.cn

Ruby: require "json"; require_relative "./util"
来源：http://sxv.ppjwa.cn

C#:   using System.Text;
来源：http://erh.fehbvm.com

[C12] 立即执行函数 IIFE
来源：http://jyp.hnxiangtu.top

Py:   (lambda: print("run"))()
来源：http://jll.zhiwuduotai.top

PHP:  (function () { echo "run"; })();
来源：http://avp.gogol.net.cn

JS:   (() => { console.log("run"); })();
来源：http://wpp.tarul.cn

TS:   (() => { console.log("run"); })();
来源：http://maf.snrcjt.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://exk.zhiwuduotai.top

Go:   func() { fmt.Println("run") }()
来源：http://wyq.uphjek.com

Ruby: -> { puts "run" }.call
来源：http://mib.zhixingplan.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nkq.hammf.cn

[C13] 类型声明 / 类型注解
来源：http://hub.ydjk.org.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kqr.kuanghao11.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yek.fzhhl.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ysb.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://feg.zhaomingkeji.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://ejw.tianlin.xyz

Go:   func add(a, b int) int
来源：http://gmo.feifeiyinyue.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rew.zhoulong.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://dyn.yangfankeji.com


<!-- 参考信息 -->